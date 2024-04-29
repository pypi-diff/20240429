# Comparing `tmp/cria-1.5.0.tar.gz` & `tmp/cria-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cria-1.5.0.tar", max compression
+gzip compressed data, was "cria-1.6.2.tar", max compression
```

## Comparing `cria-1.5.0.tar` & `cria-1.6.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2024-04-22 15:05:46.071382 cria-1.5.0/LICENSE.md
--rw-r--r--   0        0        0     8748 2024-04-22 15:05:46.071382 cria-1.5.0/README.md
--rw-r--r--   0        0        0      824 2024-04-22 15:05:46.071382 cria-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     8512 2024-04-22 15:05:46.071382 cria-1.5.0/src/cria.py
--rw-r--r--   0        0        0     9387 1970-01-01 00:00:00.000000 cria-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-29 15:24:13.797190 cria-1.6.2/LICENSE.md
+-rw-r--r--   0        0        0     8790 2024-04-29 15:24:13.797190 cria-1.6.2/README.md
+-rw-r--r--   0        0        0      824 2024-04-29 15:24:13.797190 cria-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     9555 2024-04-29 15:24:13.797190 cria-1.6.2/src/cria.py
+-rw-r--r--   0        0        0     9429 1970-01-01 00:00:00.000000 cria-1.6.2/PKG-INFO
```

### Comparing `cria-1.5.0/LICENSE.md` & `cria-1.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cria-1.5.0/README.md` & `cria-1.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -47,32 +47,36 @@
 ```python
 import cria
 
 ai = cria.Cria()
 
 prompt = "Who is the CEO of OpenAI?"
 for chunk in ai.chat(prompt):
-    print(chunk, end="") # The CEO of OpenAI is Sam Altman!
-
-ai.close() # Not required, but best practice.
+    print(chunk, end="")
 ```
-
-Another example.
+```
+>>> The CEO of OpenAI is Sam Altman!
+```
+or, you can run this more configurable example.
 
 ```python
 import cria
 
 with cria.Model() as ai:
   prompt = "Who is the CEO of OpenAI?"
-  response = ai.chat(prompt, stream=False) # The CEO of OpenAI is Sam Altman!
+  response = ai.chat(prompt, stream=False)
+  print(response)
+```
+```
+>>> The CEO of OpenAI is Sam Altman!
 ```
 
 If no model is configured, Cria runs the default model: `llama3:8b`. If the default model is not installed on your machine, Cria will install it automatically.
 
-**Important**: `llama:8b` is about **4.7GB**, and will likely take a while to download.
+**Important**: `llama3:8b` is about **4.7GB**, and will likely take a while to download.
 
 ## Installation
 
 1. Cria uses [`ollama`](https://ollama.com/), to install it, run the following.
 
    ### Windows
 
@@ -146,15 +150,15 @@
 prompt = "Tell me more about him."
 response = ai.chat(prompt, stream=False)
 print(response) # Sam Altman is an American entrepreneur and technologist who serves as the CEO of OpenAI...
 ```
 
 #### Clear Message History
 
-Clear history by running `the clear` method.
+You can reset message history by running the `clear` method.
 
 ```python
 prompt = "Who is the CEO of OpenAI?"
 response = ai.chat(prompt, stream=False)
 print(response) # Sam Altman is an American entrepreneur and technologist who serves as the CEO of OpenAI...
 
 ai.clear()
@@ -264,28 +268,26 @@
 print(response) # I apologize, but I think there may have been some confusion earlier. As this...
 ```
 
 ### Running Standalone
 
 When you run `cria.Cria()`, an `ollama` instance will start up if one is not already running. When the program exits, this instance will terminate.
 
-To prevent this behavior, either run your own `ollama` instance in another terminal, or run a managed subprocess.
+However, if you want to save resources by not exiting `ollama`, either run your own `ollama` instance in another terminal, or run a managed subprocess.
 
 #### Running Your Own Ollama Instance
 
 ```bash
 ollama serve
 ```
 
 ```python
-ai = cria.Cria()
 prompt = "Who is the CEO of OpenAI?"
-
-with cria.Model("llama3") as llama3:
-    response = llama3.generate("Who is the CEO of OpenAI?", stream=False)
+with cria.Model() as ai:
+    response = ai.generate("Who is the CEO of OpenAI?", stream=False)
     print(response)
 ```
 
 #### Running A Managed Subprocess (Reccomended)
 
 ```python
 ai = cria.Cria(standalone=True, close_on_exit=False)
```

#### html2text {}

```diff
@@ -14,96 +14,97 @@
 context) - [Multiple Models and Parallel Conversations](#multiple-models-and-
 parallel-conversations) - [Models](#models) - [With](#with-model) -
 [Standalone](#standalone-model) - [Running Standalone](#running-standalone) -
 [Contributing](#contributing) - [License](#license) ## Quickstart Running Cria
 is easy. After installation, you need just five lines of code â no
 configurations, no manual downloads, and no servers to worry about. ```python
 import cria ai = cria.Cria() prompt = "Who is the CEO of OpenAI?" for chunk in
-ai.chat(prompt): print(chunk, end="") # The CEO of OpenAI is Sam Altman!
-ai.close() # Not required, but best practice. ``` Another example. ```python
-import cria with cria.Model() as ai: prompt = "Who is the CEO of OpenAI?"
-response = ai.chat(prompt, stream=False) # The CEO of OpenAI is Sam Altman! ```
-If no model is configured, Cria runs the default model: `llama3:8b`. If the
-default model is not installed on your machine, Cria will install it
-automatically. **Important**: `llama:8b` is about **4.7GB**, and will likely
-take a while to download. ## Installation 1. Cria uses [`ollama`](https://
-ollama.com/), to install it, run the following. ### Windows [Download](https://
-ollama.com/download/windows) ### Mac [Download](https://ollama.com/download/
-mac) ### Linux ``` curl -fsSL https://ollama.com/install.sh | sh ``` 2. Install
-Cria with `pip`. ``` pip install cria ``` ## Advanced Usage ### Custom Models
-To run other LLMs, pass them into your `ai` variable. ```python import cria ai
-= cria.Cria("llama2") prompt = "Who is the CEO of OpenAI?" for chunk in ai.chat
-(prompt): print(chunk, end="") # The CEO of OpenAI is Sam Altman. He co-founded
-OpenAI in 2015 with... ``` You can find available models [here](https://
-ollama.com/library). ### Streams Streams are used by default in Cria, but you
-can turn them off by passing in a boolean for the `stream` parameter. ```python
+ai.chat(prompt): print(chunk, end="") ``` ``` >>> The CEO of OpenAI is Sam
+Altman! ``` or, you can run this more configurable example. ```python import
+cria with cria.Model() as ai: prompt = "Who is the CEO of OpenAI?" response =
+ai.chat(prompt, stream=False) print(response) ``` ``` >>> The CEO of OpenAI is
+Sam Altman! ``` If no model is configured, Cria runs the default model:
+`llama3:8b`. If the default model is not installed on your machine, Cria will
+install it automatically. **Important**: `llama3:8b` is about **4.7GB**, and
+will likely take a while to download. ## Installation 1. Cria uses [`ollama`]
+(https://ollama.com/), to install it, run the following. ### Windows [Download]
+(https://ollama.com/download/windows) ### Mac [Download](https://ollama.com/
+download/mac) ### Linux ``` curl -fsSL https://ollama.com/install.sh | sh ```
+2. Install Cria with `pip`. ``` pip install cria ``` ## Advanced Usage ###
+Custom Models To run other LLMs, pass them into your `ai` variable. ```python
+import cria ai = cria.Cria("llama2") prompt = "Who is the CEO of OpenAI?" for
+chunk in ai.chat(prompt): print(chunk, end="") # The CEO of OpenAI is Sam
+Altman. He co-founded OpenAI in 2015 with... ``` You can find available models
+[here](https://ollama.com/library). ### Streams Streams are used by default in
+Cria, but you can turn them off by passing in a boolean for the `stream`
+parameter. ```python prompt = "Who is the CEO of OpenAI?" response = ai.chat
+(prompt, stream=False) print(response) # The CEO of OpenAI is Sam Altman! ```
+### Closing By default, models are closed when you exit the Python program, but
+closing them manually is a best practice. ```python ai.close() ``` You can also
+use [`with`](#with-model) statements to close models automatically
+(recommended). ### Message History #### Follow-Up Message history is
+automatically saved in Cria, so asking follow-up questions is easy. ```python
 prompt = "Who is the CEO of OpenAI?" response = ai.chat(prompt, stream=False)
-print(response) # The CEO of OpenAI is Sam Altman! ``` ### Closing By default,
-models are closed when you exit the Python program, but closing them manually
-is a best practice. ```python ai.close() ``` You can also use [`with`](#with-
-model) statements to close models automatically (recommended). ### Message
-History #### Follow-Up Message history is automatically saved in Cria, so
-asking follow-up questions is easy. ```python prompt = "Who is the CEO of
-OpenAI?" response = ai.chat(prompt, stream=False) print(response) # The CEO of
-OpenAI is Sam Altman. prompt = "Tell me more about him." response = ai.chat
-(prompt, stream=False) print(response) # Sam Altman is an American entrepreneur
-and technologist who serves as the CEO of OpenAI... ``` #### Clear Message
-History Clear history by running `the clear` method. ```python prompt = "Who is
-the CEO of OpenAI?" response = ai.chat(prompt, stream=False) print(response) #
-Sam Altman is an American entrepreneur and technologist who serves as the CEO
-of OpenAI... ai.clear() prompt = "Tell me more about him." response = ai.chat
-(prompt, stream=False) print(response) # I apologize, but I don't have any
-information about "him" because the conversation just started... ``` ####
-Passing In Custom Context You can also create a custom message history, and
-pass in your own context. ```python context = "Our AI system employed a hybrid
-approach combining reinforcement learning and generative adversarial networks
-(GANs) to optimize the decision-making..." messages = [ {"role": "system",
-"content": "You are a technical documentation writer"}, {"role": "user",
-"content": context}, ] prompt = "Write some documentation using the text I gave
-you." for chunk in ai.chat(messages=messages, prompt=prompt): print(chunk,
-end="") # AI System Optimization: Hybrid Approach Combining Reinforcement
-Learning and... ``` In the example, instructions are given to the LLM as the
-`system`. Then, extra context is given as the `user`. Finally, the prompt is
-entered (as a `user`). You can use any mixture of roles to specify the LLM to
-your liking. The available roles for messages are: - `user` - Pass prompts as
-the user. - `system` - Give instructions as the system. - `assistant` - Act as
-the AI assistant yourself, and give the LLM lines. The prompt parameter will
-always be appended to messages under the `user` role, to override this, you can
-choose to pass in nothing for `prompt`. ### Multiple Models and Parallel
-Conversations #### Models If you are running multiple models or parallel
-conversations, the `Model` class is also available. This is recommended for
-most use cases. ```python import cria ai = cria.Model() prompt = "Who is the
-CEO of OpenAI?" response = ai.chat(prompt, stream=False) print(response) # The
-CEO of OpenAI is Sam Altman. ``` _All methods that apply to the `Cria` class
-also apply to `Model`._ #### With Model Multiple models can be run through a
-`with` statement. This automatically closes them after use. ```python import
-cria prompt = "Who is the CEO of OpenAI?" with cria.Model("llama3") as ai:
-response = ai.chat(prompt, stream=False) print(response) # OpenAI's CEO is Sam
-Altman, who also... with cria.Model("llama2") as ai: response = ai.chat(prompt,
+print(response) # The CEO of OpenAI is Sam Altman. prompt = "Tell me more about
+him." response = ai.chat(prompt, stream=False) print(response) # Sam Altman is
+an American entrepreneur and technologist who serves as the CEO of OpenAI...
+``` #### Clear Message History You can reset message history by running the
+`clear` method. ```python prompt = "Who is the CEO of OpenAI?" response =
+ai.chat(prompt, stream=False) print(response) # Sam Altman is an American
+entrepreneur and technologist who serves as the CEO of OpenAI... ai.clear()
+prompt = "Tell me more about him." response = ai.chat(prompt, stream=False)
+print(response) # I apologize, but I don't have any information about "him"
+because the conversation just started... ``` #### Passing In Custom Context You
+can also create a custom message history, and pass in your own context.
+```python context = "Our AI system employed a hybrid approach combining
+reinforcement learning and generative adversarial networks (GANs) to optimize
+the decision-making..." messages = [ {"role": "system", "content": "You are a
+technical documentation writer"}, {"role": "user", "content": context}, ]
+prompt = "Write some documentation using the text I gave you." for chunk in
+ai.chat(messages=messages, prompt=prompt): print(chunk, end="") # AI System
+Optimization: Hybrid Approach Combining Reinforcement Learning and... ``` In
+the example, instructions are given to the LLM as the `system`. Then, extra
+context is given as the `user`. Finally, the prompt is entered (as a `user`).
+You can use any mixture of roles to specify the LLM to your liking. The
+available roles for messages are: - `user` - Pass prompts as the user. -
+`system` - Give instructions as the system. - `assistant` - Act as the AI
+assistant yourself, and give the LLM lines. The prompt parameter will always be
+appended to messages under the `user` role, to override this, you can choose to
+pass in nothing for `prompt`. ### Multiple Models and Parallel Conversations
+#### Models If you are running multiple models or parallel conversations, the
+`Model` class is also available. This is recommended for most use cases.
+```python import cria ai = cria.Model() prompt = "Who is the CEO of OpenAI?"
+response = ai.chat(prompt, stream=False) print(response) # The CEO of OpenAI is
+Sam Altman. ``` _All methods that apply to the `Cria` class also apply to
+`Model`._ #### With Model Multiple models can be run through a `with`
+statement. This automatically closes them after use. ```python import cria
+prompt = "Who is the CEO of OpenAI?" with cria.Model("llama3") as ai: response
+= ai.chat(prompt, stream=False) print(response) # OpenAI's CEO is Sam Altman,
+who also... with cria.Model("llama2") as ai: response = ai.chat(prompt,
 stream=False) print(response) # The CEO of OpenAI is Sam Altman. ``` ####
 Standalone Model Or, models can be run traditionally. ```python import cria
 prompt = "Who is the CEO of OpenAI?" llama3 = cria.Model("llama3") response =
 llama3.chat(prompt, stream=False) print(response) # OpenAI's CEO is Sam Altman,
 who also... llama2 = cria.Model("llama2") response = llama2.chat(prompt,
 stream=False) print(response) # The CEO of OpenAI is Sam Altman. # Not
 required, but best practice. llama3.close() llama2.close() ``` ### Generate
 Cria also has a `generate` method. ```python prompt = "Who is the CEO of
 OpenAI?" for chunk in ai.generate(prompt): print(chunk, end="") # The CEO of
 OpenAI (Open-source Artificial Intelligence) is Sam Altman. promt = "Tell me
 more about him." response = ai.generate(prompt, stream=False) print(response) #
 I apologize, but I think there may have been some confusion earlier. As this...
 ``` ### Running Standalone When you run `cria.Cria()`, an `ollama` instance
 will start up if one is not already running. When the program exits, this
-instance will terminate. To prevent this behavior, either run your own `ollama`
-instance in another terminal, or run a managed subprocess. #### Running Your
-Own Ollama Instance ```bash ollama serve ``` ```python ai = cria.Cria() prompt
-= "Who is the CEO of OpenAI?" with cria.Model("llama3") as llama3: response =
-llama3.generate("Who is the CEO of OpenAI?", stream=False) print(response) ```
-#### Running A Managed Subprocess (Reccomended) ```python ai = cria.Cria
-(standalone=True, close_on_exit=False) prompt = "Who is the CEO of OpenAI?" #
-Ollama will already be running. with cria.Model("llama2") as llama2: response =
-llama2.generate("Who is the CEO of OpenAI?", stream=False) print(response) with
-cria.Model("llama3") as llama3: response = llama3.generate("Who is the CEO of
-OpenAI?", stream=False) print(response) quit() # Olama will keep running, and
-be used the next time this program starts. ``` ## Contributing If you have a
-feature request, feel free to make an issue! Contributions are highly
-appreciated. ## License [MIT](./LICENSE.md)
+instance will terminate. However, if you want to save resources by not exiting
+`ollama`, either run your own `ollama` instance in another terminal, or run a
+managed subprocess. #### Running Your Own Ollama Instance ```bash ollama serve
+``` ```python prompt = "Who is the CEO of OpenAI?" with cria.Model() as ai:
+response = ai.generate("Who is the CEO of OpenAI?", stream=False) print
+(response) ``` #### Running A Managed Subprocess (Reccomended) ```python ai =
+cria.Cria(standalone=True, close_on_exit=False) prompt = "Who is the CEO of
+OpenAI?" # Ollama will already be running. with cria.Model("llama2") as llama2:
+response = llama2.generate("Who is the CEO of OpenAI?", stream=False) print
+(response) with cria.Model("llama3") as llama3: response = llama3.generate("Who
+is the CEO of OpenAI?", stream=False) print(response) quit() # Olama will keep
+running, and be used the next time this program starts. ``` ## Contributing If
+you have a feature request, feel free to make an issue! Contributions are
+highly appreciated. ## License [MIT](./LICENSE.md)
```

### Comparing `cria-1.5.0/pyproject.toml` & `cria-1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cria"
-version = "1.5.0"
+version = "1.6.2"
 authors = [{ name = "leftmove", email = "100anonyo@gmail.com" }]
 description = "Run AI locally with as little friction as possible"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -13,15 +13,15 @@
 
 [project.urls]
 Homepage = "https://github.com/leftmove/cria"
 Issues = "https://github.com/leftmove/cria/issues"
 
 [tool.poetry]
 name = "cria"
-version = "1.5.0"
+version = "1.6.2"
 description = "Run AI locally with as little friction as possible."
 authors = ["leftmove"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cria-1.5.0/src/cria.py` & `cria-1.6.2/src/cria.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,86 +2,46 @@
 from typing import Optional
 
 import psutil
 import atexit
 import subprocess
 import time
 
-from httpx import ConnectError, ReadError
-from ollama._client import Client as OllamaClient
 import ollama
+import httpx
+
+from ollama._client import Client as OllamaClient
 
 DEFAULT_MODEL = "llama3:8b"
 DEFAULT_MESSAGE_HISTORY = [
     {"role": "system", "content": "You are a helpful AI assistant."}
 ]
 
 
-def check_models(model, silence_output):
-    model_list = ollama.list().get("models", [])
-    for m in model_list:
-        m_name = m.get("name", "")
-        if m_name == model:
-            return model
-        if model in m_name:
-            m_without_version = next(iter(m_name.split(":")), "")
-            if model == m_without_version:
-                if not silence_output:
-                    print(f"LLM model found, running {m_name}...")
-                return m_name
-            else:
-                if not silence_output:
-                    print(f"LLM partial match found, running {m_name}...")
-                return m_name
-    model_match = next(
-        (True if m.get("name") == model else False for m in model_list), False
-    )
-    if model_match:
-        return
-
-    if not silence_output:
-        print(f"LLM model not found, searching '{model}'...")
-
-    try:
-        progress = ollama.pull(model, stream=True)
-        print(
-            f"LLM model {model} found, downloading... (this will probably take a while)"
-        )
-        if not silence_output:
-            for chunk in progress:
-                print(chunk)
-            print(f"'{model}' downloaded, starting processes.")
-        return model
-    except Exception as e:
-        print(e)
-        raise ValueError(
-            "Invalid model passed. See the model library here: https://ollama.com/library"
-        )
-
-
 class Client(OllamaClient):
-    def chat_stream(self, messages):
+    def chat_stream(self, messages, **kwargs):
         model = self.model
         ai = ollama
 
         response = ""
 
-        for chunk in ai.chat(model=model, messages=messages, stream=True):
+        for chunk in ai.chat(model=model, messages=messages, stream=True, **kwargs):
             content = chunk["message"]["content"]
             response += content
             yield content
 
         messages.append({"role": "assistant", "content": response})
         self.messages = messages
 
     def chat(
         self,
         prompt: Optional[str] = None,
         messages: Optional[list] = DEFAULT_MESSAGE_HISTORY,
         stream: Optional[bool] = True,
+        **kwargs,
     ) -> str:
         model = self.model
         ai = ollama
 
         if not prompt and not messages:
             raise ValueError("You must pass in a prompt.")
 
@@ -92,54 +52,107 @@
                 messages,
             )
 
         if prompt:
             messages.append({"role": "user", "content": prompt})
 
         if stream:
-            return self.chat_stream(messages)
+            return self.chat_stream(messages, **kwargs)
 
-        chunk = ai.chat(model=model, messages=messages, stream=stream)
+        chunk = ai.chat(model=model, messages=messages, stream=False, **kwargs)
         response = "".join(chunk["message"]["content"])
 
         messages.append({"role": "assistant", "content": response})
         self.messages = messages
 
         return response
 
-    def generate_stream(self, prompt):
+    def generate_stream(self, prompt, **kwargs):
         model = self.model
         ai = ollama
 
-        for chunk in ai.generate(model=model, prompt=prompt, stream=True):
+        for chunk in ai.generate(model=model, prompt=prompt, stream=True, **kwargs):
             content = chunk["response"]
             yield content
 
-    def generate(
-        self,
-        prompt: str,
-        stream: Optional[bool] = True,
-    ) -> str:
+    def generate(self, prompt: str, stream: Optional[bool] = True, **kwargs) -> str:
         model = self.model
         ai = ollama
 
         if stream:
             return self.generate_stream(prompt)
 
-        chunk = ai.generate(model=model, prompt=prompt, stream=False)
+        chunk = ai.generate(model=model, prompt=prompt, stream=False, **kwargs)
         response = chunk["response"]
 
         return response
 
     def clear(self):
         self.messages = [
             {"role": "system", "content": "You are a helpful AI assistant."}
         ]
 
 
+def check_models(model, silence_output):
+    model_list = ollama.list().get("models", [])
+    for m in model_list:
+        m_name = m.get("name", "")
+        if m_name == model:
+            return model
+        if model in m_name:
+            m_without_version = next(iter(m_name.split(":")), "")
+            if model == m_without_version:
+                if not silence_output:
+                    print(f"LLM model found, running {m_name}...")
+                return m_name
+            else:
+                if not silence_output:
+                    print(f"LLM partial match found, running {m_name}...")
+                return m_name
+    model_match = next(
+        (True if m.get("name") == model else False for m in model_list), False
+    )
+    if model_match:
+        return model
+
+    if not silence_output:
+        print(f"LLM model not found, searching '{model}'...")
+
+    try:
+        progress = ollama.pull(model, stream=True)
+        print(
+            f"LLM model {model} found, downloading... (this will probably take a while)"
+        )
+        if not silence_output:
+            for chunk in progress:
+                print(chunk)
+            print(f"'{model}' downloaded, starting processes.")
+        return model
+    except Exception as e:
+        print(e)
+        raise ValueError(
+            "Invalid model passed. See the model library here: https://ollama.com/library"
+        )
+
+
+def find_process(command, process_name="ollama"):
+    process = None
+    for proc in psutil.process_iter(attrs=["cmdline"]):
+        try:
+            if process_name.lower() in proc.name().lower():
+                proc_command = proc.info["cmdline"]
+                if proc_command[: len(command)] != command:
+                    continue
+                process = psutil.Process(pid=proc.pid)
+                break
+        except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+            pass
+    return process
+
+
 class Cria(Client):
     def __init__(
         self,
         model: Optional[str] = DEFAULT_MODEL,
         standalone: Optional[bool] = False,
         run_subprocess: Optional[bool] = False,
         capture_output: Optional[bool] = False,
@@ -147,71 +160,59 @@
         close_on_exit: Optional[bool] = True,
     ) -> None:
         self.run_subprocess = run_subprocess
         self.capture_output = capture_output
         self.silence_output = silence_output
         self.close_on_exit = close_on_exit
 
-        process_name = "ollama"
-        ollama_pids = []
-        ollama_running = False
-        for proc in psutil.process_iter():
-            try:
-                if process_name.lower() in proc.name().lower():
-                    ollama_pids.append(proc.pid)
-                    ollama_running = True
-                    break
-            except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
-                pass
-
-        if ollama_running:
-            self.ollama_pids = ollama_pids
-        else:
-            self.ollama_pids = None
+        ollama_process = find_process(["ollama", "serve"])
+        self.ollama_process = ollama_process
 
-        if ollama_running and run_subprocess:
-            for ollama_pid in self.ollama_pids:
-                ollama_process = psutil.Process(pid=ollama_pid)
-                ollama_process.kill()
-            ollama_running = False
+        if ollama_process and run_subprocess:
+            self.ollama_process.kill()
 
         try:
             ollama.list()
-        except (ConnectError, ReadError):
-            ollama_running = False
+        except (httpx.ConnectError, httpx.ReadError):
+            ollama_process = None
 
-        if not ollama_running:
+        if not ollama_process:
             ollama_stdout = subprocess.PIPE if capture_output else subprocess.DEVNULL
             ollama_stderr = subprocess.PIPE if capture_output else subprocess.DEVNULL
             try:
                 self.ollama_subrprocess = subprocess.Popen(
-                ["ollama", "serve"], stdout=ollama_stdout, stderr=ollama_stderr
-            )
+                    ["ollama", "serve"], stdout=ollama_stdout, stderr=ollama_stderr
+                )
             except FileNotFoundError:
-                raise FileNotFoundError("Ollama is not installed, please install ollama from 'https://ollama.com/download'")
+                raise FileNotFoundError(
+                    "Ollama is not installed, please install ollama from 'https://ollama.com/download'"
+                )
             retries = 10
             while retries:
                 try:
                     ollama.list()
                     break
-                except (ConnectError, ReadError):
+                except (httpx.ConnectError, httpx.ReadError):
                     time.sleep(2)
                     retries -= 1
         else:
             self.ollama_subrprocess = None
 
-        model = check_models(model, silence_output)
-        self.model = model
+        self.model = check_models(model, silence_output)
 
         if not standalone:
-            self.llm = subprocess.Popen(
-                ["ollama", "run", model],
-                stdout=subprocess.DEVNULL,
-                stderr=subprocess.DEVNULL,
-            )
+            self.llm = find_process(["ollama", "run", self.model])
+
+            if self.llm and run_subprocess:
+                self.llm.kill()
+                self.llm = subprocess.Popen(
+                    ["ollama", "run", self.model],
+                    stdout=subprocess.DEVNULL,
+                    stderr=subprocess.DEVNULL,
+                )
 
         if close_on_exit and self.ollama_subrprocess:
             atexit.register(lambda: self.ollama_subrprocess.kill())
 
         if close_on_exit and not standalone:
             atexit.register(lambda: self.llm.kill())
 
@@ -233,14 +234,16 @@
         llm.kill()
 
 
 class Model(Cria, ContextDecorator):
     def __init__(
         self,
         model: Optional[str] = DEFAULT_MODEL,
+        run_attached: Optional[bool] = False,
+        run_subprocess: Optional[bool] = False,
         capture_output: Optional[bool] = False,
         silence_output: Optional[bool] = False,
         close_on_exit: Optional[bool] = True,
     ) -> None:
         super().__init__(
             model=model,
             capture_output=capture_output,
@@ -249,19 +252,38 @@
             close_on_exit=close_on_exit,
         )
 
         self.capture_output = capture_output
         self.silence_output = silence_output
         self.close_on_exit = close_on_exit
 
-        llm_stdout = subprocess.PIPE if capture_output else subprocess.DEVNULL
-        llm_stderr = subprocess.PIPE if capture_output else subprocess.DEVNULL
-        self.llm = subprocess.Popen(
-            ["ollama", "run", model], stdout=llm_stdout, stderr=llm_stderr
-        )
+        self.model = check_models(model, silence_output)
+
+        if run_attached and run_subprocess:
+            raise ValueError(
+                "You cannot run attach to an LLM and run it as a subprocess at the same time."
+            )
+
+        if not run_attached:
+            llm_stdout = subprocess.PIPE if capture_output else subprocess.DEVNULL
+            llm_stderr = subprocess.PIPE if capture_output else subprocess.DEVNULL
+            self.llm = subprocess.Popen(
+                ["ollama", "run", self.model], stdout=llm_stdout, stderr=llm_stderr
+            )
+        else:
+            self.llm = find_process(["ollama", "run", self.model])
+
+        if self.llm and run_subprocess:
+            self.llm.kill()
+
+            llm_stdout = subprocess.PIPE if capture_output else subprocess.DEVNULL
+            llm_stderr = subprocess.PIPE if capture_output else subprocess.DEVNULL
+            self.llm = subprocess.Popen(
+                ["ollama", "run", self.model], stdout=llm_stdout, stderr=llm_stderr
+            )
 
         if close_on_exit:
             atexit.register(lambda: self.llm.kill())
 
     def capture_output(self):
         if not self.capture_output:
             raise ValueError(
```

### Comparing `cria-1.5.0/PKG-INFO` & `cria-1.6.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cria
-Version: 1.5.0
+Version: 1.6.2
 Summary: Run AI locally with as little friction as possible.
 License: MIT
 Author: leftmove
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -65,32 +65,36 @@
 ```python
 import cria
 
 ai = cria.Cria()
 
 prompt = "Who is the CEO of OpenAI?"
 for chunk in ai.chat(prompt):
-    print(chunk, end="") # The CEO of OpenAI is Sam Altman!
-
-ai.close() # Not required, but best practice.
+    print(chunk, end="")
 ```
-
-Another example.
+```
+>>> The CEO of OpenAI is Sam Altman!
+```
+or, you can run this more configurable example.
 
 ```python
 import cria
 
 with cria.Model() as ai:
   prompt = "Who is the CEO of OpenAI?"
-  response = ai.chat(prompt, stream=False) # The CEO of OpenAI is Sam Altman!
+  response = ai.chat(prompt, stream=False)
+  print(response)
+```
+```
+>>> The CEO of OpenAI is Sam Altman!
 ```
 
 If no model is configured, Cria runs the default model: `llama3:8b`. If the default model is not installed on your machine, Cria will install it automatically.
 
-**Important**: `llama:8b` is about **4.7GB**, and will likely take a while to download.
+**Important**: `llama3:8b` is about **4.7GB**, and will likely take a while to download.
 
 ## Installation
 
 1. Cria uses [`ollama`](https://ollama.com/), to install it, run the following.
 
    ### Windows
 
@@ -164,15 +168,15 @@
 prompt = "Tell me more about him."
 response = ai.chat(prompt, stream=False)
 print(response) # Sam Altman is an American entrepreneur and technologist who serves as the CEO of OpenAI...
 ```
 
 #### Clear Message History
 
-Clear history by running `the clear` method.
+You can reset message history by running the `clear` method.
 
 ```python
 prompt = "Who is the CEO of OpenAI?"
 response = ai.chat(prompt, stream=False)
 print(response) # Sam Altman is an American entrepreneur and technologist who serves as the CEO of OpenAI...
 
 ai.clear()
@@ -282,28 +286,26 @@
 print(response) # I apologize, but I think there may have been some confusion earlier. As this...
 ```
 
 ### Running Standalone
 
 When you run `cria.Cria()`, an `ollama` instance will start up if one is not already running. When the program exits, this instance will terminate.
 
-To prevent this behavior, either run your own `ollama` instance in another terminal, or run a managed subprocess.
+However, if you want to save resources by not exiting `ollama`, either run your own `ollama` instance in another terminal, or run a managed subprocess.
 
 #### Running Your Own Ollama Instance
 
 ```bash
 ollama serve
 ```
 
 ```python
-ai = cria.Cria()
 prompt = "Who is the CEO of OpenAI?"
-
-with cria.Model("llama3") as llama3:
-    response = llama3.generate("Who is the CEO of OpenAI?", stream=False)
+with cria.Model() as ai:
+    response = ai.generate("Who is the CEO of OpenAI?", stream=False)
     print(response)
 ```
 
 #### Running A Managed Subprocess (Reccomended)
 
 ```python
 ai = cria.Cria(standalone=True, close_on_exit=False)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cria Version: 1.5.0 Summary: Run AI locally with as
+Metadata-Version: 2.1 Name: cria Version: 1.6.2 Summary: Run AI locally with as
 little friction as possible. License: MIT Author: leftmove Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: ollama (>=0.1.8,<0.2.0) Requires-Dist: psutil (>=5.9.8,<6.0.0)
@@ -23,96 +23,97 @@
 context) - [Multiple Models and Parallel Conversations](#multiple-models-and-
 parallel-conversations) - [Models](#models) - [With](#with-model) -
 [Standalone](#standalone-model) - [Running Standalone](#running-standalone) -
 [Contributing](#contributing) - [License](#license) ## Quickstart Running Cria
 is easy. After installation, you need just five lines of code â no
 configurations, no manual downloads, and no servers to worry about. ```python
 import cria ai = cria.Cria() prompt = "Who is the CEO of OpenAI?" for chunk in
-ai.chat(prompt): print(chunk, end="") # The CEO of OpenAI is Sam Altman!
-ai.close() # Not required, but best practice. ``` Another example. ```python
-import cria with cria.Model() as ai: prompt = "Who is the CEO of OpenAI?"
-response = ai.chat(prompt, stream=False) # The CEO of OpenAI is Sam Altman! ```
-If no model is configured, Cria runs the default model: `llama3:8b`. If the
-default model is not installed on your machine, Cria will install it
-automatically. **Important**: `llama:8b` is about **4.7GB**, and will likely
-take a while to download. ## Installation 1. Cria uses [`ollama`](https://
-ollama.com/), to install it, run the following. ### Windows [Download](https://
-ollama.com/download/windows) ### Mac [Download](https://ollama.com/download/
-mac) ### Linux ``` curl -fsSL https://ollama.com/install.sh | sh ``` 2. Install
-Cria with `pip`. ``` pip install cria ``` ## Advanced Usage ### Custom Models
-To run other LLMs, pass them into your `ai` variable. ```python import cria ai
-= cria.Cria("llama2") prompt = "Who is the CEO of OpenAI?" for chunk in ai.chat
-(prompt): print(chunk, end="") # The CEO of OpenAI is Sam Altman. He co-founded
-OpenAI in 2015 with... ``` You can find available models [here](https://
-ollama.com/library). ### Streams Streams are used by default in Cria, but you
-can turn them off by passing in a boolean for the `stream` parameter. ```python
+ai.chat(prompt): print(chunk, end="") ``` ``` >>> The CEO of OpenAI is Sam
+Altman! ``` or, you can run this more configurable example. ```python import
+cria with cria.Model() as ai: prompt = "Who is the CEO of OpenAI?" response =
+ai.chat(prompt, stream=False) print(response) ``` ``` >>> The CEO of OpenAI is
+Sam Altman! ``` If no model is configured, Cria runs the default model:
+`llama3:8b`. If the default model is not installed on your machine, Cria will
+install it automatically. **Important**: `llama3:8b` is about **4.7GB**, and
+will likely take a while to download. ## Installation 1. Cria uses [`ollama`]
+(https://ollama.com/), to install it, run the following. ### Windows [Download]
+(https://ollama.com/download/windows) ### Mac [Download](https://ollama.com/
+download/mac) ### Linux ``` curl -fsSL https://ollama.com/install.sh | sh ```
+2. Install Cria with `pip`. ``` pip install cria ``` ## Advanced Usage ###
+Custom Models To run other LLMs, pass them into your `ai` variable. ```python
+import cria ai = cria.Cria("llama2") prompt = "Who is the CEO of OpenAI?" for
+chunk in ai.chat(prompt): print(chunk, end="") # The CEO of OpenAI is Sam
+Altman. He co-founded OpenAI in 2015 with... ``` You can find available models
+[here](https://ollama.com/library). ### Streams Streams are used by default in
+Cria, but you can turn them off by passing in a boolean for the `stream`
+parameter. ```python prompt = "Who is the CEO of OpenAI?" response = ai.chat
+(prompt, stream=False) print(response) # The CEO of OpenAI is Sam Altman! ```
+### Closing By default, models are closed when you exit the Python program, but
+closing them manually is a best practice. ```python ai.close() ``` You can also
+use [`with`](#with-model) statements to close models automatically
+(recommended). ### Message History #### Follow-Up Message history is
+automatically saved in Cria, so asking follow-up questions is easy. ```python
 prompt = "Who is the CEO of OpenAI?" response = ai.chat(prompt, stream=False)
-print(response) # The CEO of OpenAI is Sam Altman! ``` ### Closing By default,
-models are closed when you exit the Python program, but closing them manually
-is a best practice. ```python ai.close() ``` You can also use [`with`](#with-
-model) statements to close models automatically (recommended). ### Message
-History #### Follow-Up Message history is automatically saved in Cria, so
-asking follow-up questions is easy. ```python prompt = "Who is the CEO of
-OpenAI?" response = ai.chat(prompt, stream=False) print(response) # The CEO of
-OpenAI is Sam Altman. prompt = "Tell me more about him." response = ai.chat
-(prompt, stream=False) print(response) # Sam Altman is an American entrepreneur
-and technologist who serves as the CEO of OpenAI... ``` #### Clear Message
-History Clear history by running `the clear` method. ```python prompt = "Who is
-the CEO of OpenAI?" response = ai.chat(prompt, stream=False) print(response) #
-Sam Altman is an American entrepreneur and technologist who serves as the CEO
-of OpenAI... ai.clear() prompt = "Tell me more about him." response = ai.chat
-(prompt, stream=False) print(response) # I apologize, but I don't have any
-information about "him" because the conversation just started... ``` ####
-Passing In Custom Context You can also create a custom message history, and
-pass in your own context. ```python context = "Our AI system employed a hybrid
-approach combining reinforcement learning and generative adversarial networks
-(GANs) to optimize the decision-making..." messages = [ {"role": "system",
-"content": "You are a technical documentation writer"}, {"role": "user",
-"content": context}, ] prompt = "Write some documentation using the text I gave
-you." for chunk in ai.chat(messages=messages, prompt=prompt): print(chunk,
-end="") # AI System Optimization: Hybrid Approach Combining Reinforcement
-Learning and... ``` In the example, instructions are given to the LLM as the
-`system`. Then, extra context is given as the `user`. Finally, the prompt is
-entered (as a `user`). You can use any mixture of roles to specify the LLM to
-your liking. The available roles for messages are: - `user` - Pass prompts as
-the user. - `system` - Give instructions as the system. - `assistant` - Act as
-the AI assistant yourself, and give the LLM lines. The prompt parameter will
-always be appended to messages under the `user` role, to override this, you can
-choose to pass in nothing for `prompt`. ### Multiple Models and Parallel
-Conversations #### Models If you are running multiple models or parallel
-conversations, the `Model` class is also available. This is recommended for
-most use cases. ```python import cria ai = cria.Model() prompt = "Who is the
-CEO of OpenAI?" response = ai.chat(prompt, stream=False) print(response) # The
-CEO of OpenAI is Sam Altman. ``` _All methods that apply to the `Cria` class
-also apply to `Model`._ #### With Model Multiple models can be run through a
-`with` statement. This automatically closes them after use. ```python import
-cria prompt = "Who is the CEO of OpenAI?" with cria.Model("llama3") as ai:
-response = ai.chat(prompt, stream=False) print(response) # OpenAI's CEO is Sam
-Altman, who also... with cria.Model("llama2") as ai: response = ai.chat(prompt,
+print(response) # The CEO of OpenAI is Sam Altman. prompt = "Tell me more about
+him." response = ai.chat(prompt, stream=False) print(response) # Sam Altman is
+an American entrepreneur and technologist who serves as the CEO of OpenAI...
+``` #### Clear Message History You can reset message history by running the
+`clear` method. ```python prompt = "Who is the CEO of OpenAI?" response =
+ai.chat(prompt, stream=False) print(response) # Sam Altman is an American
+entrepreneur and technologist who serves as the CEO of OpenAI... ai.clear()
+prompt = "Tell me more about him." response = ai.chat(prompt, stream=False)
+print(response) # I apologize, but I don't have any information about "him"
+because the conversation just started... ``` #### Passing In Custom Context You
+can also create a custom message history, and pass in your own context.
+```python context = "Our AI system employed a hybrid approach combining
+reinforcement learning and generative adversarial networks (GANs) to optimize
+the decision-making..." messages = [ {"role": "system", "content": "You are a
+technical documentation writer"}, {"role": "user", "content": context}, ]
+prompt = "Write some documentation using the text I gave you." for chunk in
+ai.chat(messages=messages, prompt=prompt): print(chunk, end="") # AI System
+Optimization: Hybrid Approach Combining Reinforcement Learning and... ``` In
+the example, instructions are given to the LLM as the `system`. Then, extra
+context is given as the `user`. Finally, the prompt is entered (as a `user`).
+You can use any mixture of roles to specify the LLM to your liking. The
+available roles for messages are: - `user` - Pass prompts as the user. -
+`system` - Give instructions as the system. - `assistant` - Act as the AI
+assistant yourself, and give the LLM lines. The prompt parameter will always be
+appended to messages under the `user` role, to override this, you can choose to
+pass in nothing for `prompt`. ### Multiple Models and Parallel Conversations
+#### Models If you are running multiple models or parallel conversations, the
+`Model` class is also available. This is recommended for most use cases.
+```python import cria ai = cria.Model() prompt = "Who is the CEO of OpenAI?"
+response = ai.chat(prompt, stream=False) print(response) # The CEO of OpenAI is
+Sam Altman. ``` _All methods that apply to the `Cria` class also apply to
+`Model`._ #### With Model Multiple models can be run through a `with`
+statement. This automatically closes them after use. ```python import cria
+prompt = "Who is the CEO of OpenAI?" with cria.Model("llama3") as ai: response
+= ai.chat(prompt, stream=False) print(response) # OpenAI's CEO is Sam Altman,
+who also... with cria.Model("llama2") as ai: response = ai.chat(prompt,
 stream=False) print(response) # The CEO of OpenAI is Sam Altman. ``` ####
 Standalone Model Or, models can be run traditionally. ```python import cria
 prompt = "Who is the CEO of OpenAI?" llama3 = cria.Model("llama3") response =
 llama3.chat(prompt, stream=False) print(response) # OpenAI's CEO is Sam Altman,
 who also... llama2 = cria.Model("llama2") response = llama2.chat(prompt,
 stream=False) print(response) # The CEO of OpenAI is Sam Altman. # Not
 required, but best practice. llama3.close() llama2.close() ``` ### Generate
 Cria also has a `generate` method. ```python prompt = "Who is the CEO of
 OpenAI?" for chunk in ai.generate(prompt): print(chunk, end="") # The CEO of
 OpenAI (Open-source Artificial Intelligence) is Sam Altman. promt = "Tell me
 more about him." response = ai.generate(prompt, stream=False) print(response) #
 I apologize, but I think there may have been some confusion earlier. As this...
 ``` ### Running Standalone When you run `cria.Cria()`, an `ollama` instance
 will start up if one is not already running. When the program exits, this
-instance will terminate. To prevent this behavior, either run your own `ollama`
-instance in another terminal, or run a managed subprocess. #### Running Your
-Own Ollama Instance ```bash ollama serve ``` ```python ai = cria.Cria() prompt
-= "Who is the CEO of OpenAI?" with cria.Model("llama3") as llama3: response =
-llama3.generate("Who is the CEO of OpenAI?", stream=False) print(response) ```
-#### Running A Managed Subprocess (Reccomended) ```python ai = cria.Cria
-(standalone=True, close_on_exit=False) prompt = "Who is the CEO of OpenAI?" #
-Ollama will already be running. with cria.Model("llama2") as llama2: response =
-llama2.generate("Who is the CEO of OpenAI?", stream=False) print(response) with
-cria.Model("llama3") as llama3: response = llama3.generate("Who is the CEO of
-OpenAI?", stream=False) print(response) quit() # Olama will keep running, and
-be used the next time this program starts. ``` ## Contributing If you have a
-feature request, feel free to make an issue! Contributions are highly
-appreciated. ## License [MIT](./LICENSE.md)
+instance will terminate. However, if you want to save resources by not exiting
+`ollama`, either run your own `ollama` instance in another terminal, or run a
+managed subprocess. #### Running Your Own Ollama Instance ```bash ollama serve
+``` ```python prompt = "Who is the CEO of OpenAI?" with cria.Model() as ai:
+response = ai.generate("Who is the CEO of OpenAI?", stream=False) print
+(response) ``` #### Running A Managed Subprocess (Reccomended) ```python ai =
+cria.Cria(standalone=True, close_on_exit=False) prompt = "Who is the CEO of
+OpenAI?" # Ollama will already be running. with cria.Model("llama2") as llama2:
+response = llama2.generate("Who is the CEO of OpenAI?", stream=False) print
+(response) with cria.Model("llama3") as llama3: response = llama3.generate("Who
+is the CEO of OpenAI?", stream=False) print(response) quit() # Olama will keep
+running, and be used the next time this program starts. ``` ## Contributing If
+you have a feature request, feel free to make an issue! Contributions are
+highly appreciated. ## License [MIT](./LICENSE.md)
```

