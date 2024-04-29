# Comparing `tmp/unifyai-0.8.1.tar.gz` & `tmp/unifyai-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.8.1.tar", max compression
+gzip compressed data, was "unifyai-0.8.2.tar", max compression
```

## Comparing `unifyai-0.8.1.tar` & `unifyai-0.8.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.8.1/LICENSE
--rw-r--r--   0        0        0     6303 2024-04-15 01:21:08.867568 unifyai-0.8.1/README.md
--rw-r--r--   0        0        0     1041 2024-04-15 01:21:17.047568 unifyai-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      131 2024-04-15 01:21:08.867568 unifyai-0.8.1/unify/__init__.py
--rw-r--r--   0        0        0     6724 2024-04-15 01:21:08.867568 unifyai-0.8.1/unify/chat.py
--rw-r--r--   0        0        0    15107 2024-04-15 01:21:08.867568 unifyai-0.8.1/unify/clients.py
--rw-r--r--   0        0        0     1166 2024-04-15 01:21:08.867568 unifyai-0.8.1/unify/exceptions.py
--rw-r--r--   0        0        0     4321 2024-04-15 01:21:08.867568 unifyai-0.8.1/unify/tests.py
--rw-r--r--   0        0        0     1820 2024-04-15 01:21:27.171568 unifyai-0.8.1/unify/utils.py
--rw-r--r--   0        0        0     6964 1970-01-01 00:00:00.000000 unifyai-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-29 10:34:46.881584 unifyai-0.8.2/LICENSE
+-rw-r--r--   0        0        0     6589 2024-04-29 19:44:46.290194 unifyai-0.8.2/README.md
+-rw-r--r--   0        0        0     1041 2024-04-29 19:45:50.778195 unifyai-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-04-29 19:44:46.294194 unifyai-0.8.2/unify/__init__.py
+-rw-r--r--   0        0        0     6875 2024-04-29 19:44:46.294194 unifyai-0.8.2/unify/chat.py
+-rw-r--r--   0        0        0    15137 2024-04-29 19:44:46.294194 unifyai-0.8.2/unify/clients.py
+-rw-r--r--   0        0        0     1166 2024-04-29 10:34:46.885583 unifyai-0.8.2/unify/exceptions.py
+-rw-r--r--   0        0        0     4321 2024-04-29 10:34:46.885583 unifyai-0.8.2/unify/tests.py
+-rw-r--r--   0        0        0     3472 2024-04-29 19:44:46.302193 unifyai-0.8.2/unify/utils.py
+-rw-r--r--   0        0        0     7250 1970-01-01 00:00:00.000000 unifyai-0.8.2/PKG-INFO
```

### Comparing `unifyai-0.8.1/LICENSE` & `unifyai-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.8.1/README.md` & `unifyai-0.8.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,22 @@
 unify.set_model("mistral-7b-instruct-v0.1")
 unify.set_provider("deepinfra")
 ```
 
 ### Supported Models
 The list of supported models and providers is available in [the platform](https://unify.ai/hub).
 
+You can also get this information directly in Python using `list_models()`, `list_providers()` and `list_endpoints()`.
+
+```python
+models = unify.list_models()
+providers = unify.list_providers("mistral-7b-instruct-v0.1")
+endpoints = unify.list_endpoints("mistral-7b-instruct-v0.1")
+```
+
 ### API Key
 You can get an API Key from [the Unify console](https://console.unify.ai/)
 
 > [!NOTE]
 > You can provide an `api_key` keyword argument, but
 > we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 > to add `UNIFY_KEY="My API Key"` to your `.env` file
```

### Comparing `unifyai-0.8.1/pyproject.toml` & `unifyai-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "unifyai"
 packages = [{include = "unify"}]
-version = "0.8.1"
+version = "0.8.2"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
 repository = "https://github.com/unifyai/unify"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `unifyai-0.8.1/unify/chat.py` & `unifyai-0.8.2/unify/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import sys
+from typing import Dict, Generator, List, Optional
 
-from typing import Optional
 from unify.clients import Unify
+from unify.exceptions import UnifyError
 
 
 class ChatBot:  # noqa: WPS338
     """Agent class represents an LLM chat agent."""
 
     def __init__(
         self,
         api_key: Optional[str] = None,
         endpoint: Optional[str] = None,
         model: Optional[str] = None,
         provider: Optional[str] = None,
-        ) -> None:
+    ) -> None:
         """
         Initializes the ChatBot object.
 
         Args:
             api_key (str, optional): API key for accessing the Unify API.
                 If None, it attempts to retrieve the API key from the
                 environment variable UNIFY_KEY.
@@ -31,25 +32,25 @@
             endpoint must be provided.
 
             provider (str, optional): Name of the provider. If None,
             endpoint must be provided.
         Raises:
             UnifyError: If the API key is missing.
         """
-        self._message_history = []
+        self._message_history: List[Dict[str, str]] = []
         self._paused = False
         self._client = Unify(
             api_key=api_key,
             endpoint=endpoint,
             model=model,
             provider=provider,
         )
 
     @property
-    def client(self) -> str:
+    def client(self) -> Unify:
         """
         Get the client object.  # noqa: DAR201.
 
         Returns:
             str: The model name.
         """
         return self._client
@@ -62,15 +63,14 @@
             value: The unify client.
         """
         if isinstance(value, Unify):
             self._client = value
         else:
             raise UnifyError("Invalid client!")
 
-
     @property
     def model(self) -> str:
         """
         Get the model name.  # noqa: DAR201.
 
         Returns:
             str: The model name.
@@ -105,15 +105,15 @@
         """
         Set the provider name.  # noqa: DAR101.
 
         Args:
             value (str): The provider name.
         """
         self._client.set_provider(value)
-        self._client.set_endpoint("@".join([self._model, value]))
+        self._client.set_endpoint("@".join([self._client._model, value]))
 
     @property
     def endpoint(self) -> str:
         """
         Get the endpoint name.  # noqa: DAR201.
 
         Returns:
@@ -128,80 +128,82 @@
         Args:
             value (str): The endpoint name.
         """
         self._client.set_endpoint(value)
         self._client.set_model(value.split("@")[0])
         self._client.set_provider(value.split("@")[1])
 
-    def _get_credits(self):
+    def _get_credits(self) -> float:
         """
         Retrieves the current credit balance from associated with the UNIFY account.
 
         Returns:
             float: Current credit balance.
         """
         return self._client.get_credit_balance()
 
-    def _process_input(self, inp: str, show_credits: bool, show_provider: bool):
+    def _process_input(
+        self, inp: str, show_credits: bool, show_provider: bool
+    ) -> Generator[str, None, None]:
         """
         Processes the user input to generate AI response.
 
         Args:
             inp (str): User input message.
             show_credits (bool): Whether to show credit consumption.
             show_credits (bool): Whether to show provider used.
 
         Yields:
             str: Generated AI response chunks.
         """
-        self._update_message_history(role = "user", content = inp)
+        self._update_message_history(role="user", content=inp)
         initial_credit_balance = self._get_credits()
         stream = self._client.generate(
             messages=self._message_history,
             stream=True,
         )
         words = ""
         for chunk in stream:
             words += chunk
             yield chunk
 
         self._update_message_history(
-                role = "assistant",
-                content = words,
+            role="assistant",
+            content=words,
         )
         final_credit_balance = self._get_credits()
         if show_credits:
             sys.stdout.write(
                 "\n(spent {:.6f} credits)".format(
                     initial_credit_balance - final_credit_balance,
                 ),
             )
         if show_provider:
             sys.stdout.write("\n(provider: {})".format(self._client.provider))
 
-    def _update_message_history(self, role: str, content: str):
+    def _update_message_history(self, role: str, content: str) -> None:
         """
         Updates message history with user input.
 
         Args:
             role (str): Either "assistant" or "user".
             content (str): User input message.
         """
         self._message_history.append(
             {
                 "role": role,
                 "content": content,
             },
         )
 
-    def clear_chat_history(self):
+    def clear_chat_history(self) -> None:
         """Clears the chat history."""
         self._message_history.clear()
 
-    def run(self, show_credits: bool = False, show_provider: bool = False):
+    def run(self, show_credits: bool = False, show_provider: bool = False) -> None:
         """
         Starts the chat interaction loop.
 
         Args:
             show_credits (bool, optional): Whether to show credit consumption.
             Defaults to False.
             show_provider (bool, optional): Whether to show the provider used.
```

### Comparing `unifyai-0.8.1/unify/clients.py` & `unifyai-0.8.2/unify/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         else:
             raise UnifyError("You must provider either the user_prompt or messages!")
 
         if stream:
             return self._generate_stream(contents, self._endpoint)
         return self._generate_non_stream(contents, self._endpoint)
 
-    def get_credit_balance(self) -> Optional[int]:
+    def get_credit_balance(self) -> float:
         # noqa: DAR201, DAR401
         """
         Get the remaining credits left on your account.
 
         Returns:
             int or None: The remaining credits on the account
             if successful, otherwise None.
@@ -218,17 +218,19 @@
     ) -> str:
         try:
             chat_completion = self.client.chat.completions.create(
                 model=endpoint,
                 messages=messages,  # type: ignore[arg-type]
                 stream=False,
             )
-            self.set_provider(chat_completion.model.split(  # type: ignore[union-attr]
-                "@",
-            )[-1])
+            self.set_provider(
+                chat_completion.model.split(  # type: ignore[union-attr]
+                    "@",
+                )[-1]
+            )
 
             return chat_completion.choices[0].message.content.strip(" ")  # type: ignore # noqa: E501, WPS219
         except openai.APIStatusError as e:
             raise status_error_map[e.status_code](e.message) from None
 
 
 class AsyncUnify:
```

### Comparing `unifyai-0.8.1/unify/exceptions.py` & `unifyai-0.8.2/unify/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.8.1/unify/tests.py` & `unifyai-0.8.2/unify/tests.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.8.1/PKG-INFO` & `unifyai-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.8.1
+Version: 0.8.2
 Summary: A Python package for interacting with the Unify API
 Home-page: https://github.com/unifyai/unify
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -73,14 +73,22 @@
 unify.set_model("mistral-7b-instruct-v0.1")
 unify.set_provider("deepinfra")
 ```
 
 ### Supported Models
 The list of supported models and providers is available in [the platform](https://unify.ai/hub).
 
+You can also get this information directly in Python using `list_models()`, `list_providers()` and `list_endpoints()`.
+
+```python
+models = unify.list_models()
+providers = unify.list_providers("mistral-7b-instruct-v0.1")
+endpoints = unify.list_endpoints("mistral-7b-instruct-v0.1")
+```
+
 ### API Key
 You can get an API Key from [the Unify console](https://console.unify.ai/)
 
 > [!NOTE]
 > You can provide an `api_key` keyword argument, but
 > we recommend using [python-dotenv](https://pypi.org/project/python-dotenv/)
 > to add `UNIFY_KEY="My API Key"` to your `.env` file
```

