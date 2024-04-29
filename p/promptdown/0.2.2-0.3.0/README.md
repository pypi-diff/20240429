# Comparing `tmp/promptdown-0.2.2.tar.gz` & `tmp/promptdown-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptdown-0.2.2.tar", last modified: Wed Apr 10 21:39:07 2024, max compression
+gzip compressed data, was "promptdown-0.3.0.tar", last modified: Mon Apr 29 01:55:25 2024, max compression
```

## Comparing `promptdown-0.2.2.tar` & `promptdown-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-10 21:38:52.798120 promptdown-0.2.2/LICENSE
--rw-r--r--   0        0        0     2145 2024-04-10 21:38:52.798120 promptdown-0.2.2/README.md
--rw-r--r--   0        0        0     1074 2024-04-10 21:39:07.210296 promptdown-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       93 2024-04-10 21:38:52.802121 promptdown-0.2.2/src/promptdown/__init__.py
--rw-r--r--   0        0        0      124 2024-04-10 21:39:05.750278 promptdown-0.2.2/src/promptdown/__init__.pyi
--rw-r--r--   0        0        0     6149 2024-04-10 21:38:52.802121 promptdown-0.2.2/src/promptdown/promptdown.py
--rw-r--r--   0        0        0      755 2024-04-10 21:39:05.750278 promptdown-0.2.2/src/promptdown/promptdown.pyi
--rw-r--r--   0        0        0     2950 1970-01-01 00:00:00.000000 promptdown-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-29 01:55:14.881076 promptdown-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3223 2024-04-29 01:55:14.881076 promptdown-0.3.0/README.md
+-rw-r--r--   0        0        0     1074 2024-04-29 01:55:25.985123 promptdown-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2024-04-29 01:55:14.881076 promptdown-0.3.0/src/promptdown/__init__.py
+-rw-r--r--   0        0        0      124 2024-04-29 01:55:24.577118 promptdown-0.3.0/src/promptdown/__init__.pyi
+-rw-r--r--   0        0        0     7357 2024-04-29 01:55:14.881076 promptdown-0.3.0/src/promptdown/promptdown.py
+-rw-r--r--   0        0        0      870 2024-04-29 01:55:24.577118 promptdown-0.3.0/src/promptdown/promptdown.pyi
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 promptdown-0.3.0/PKG-INFO
```

### Comparing `promptdown-0.2.2/LICENSE` & `promptdown-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `promptdown-0.2.2/README.md` & `promptdown-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -44,23 +44,29 @@
 ```
 
 Then, you can parse this file into a `StructuredPrompt` object using Promptdown:
 
 ```python
 from promptdown import StructuredPrompt
 
-structured_prompt = StructuredPrompt.from_promptdown_file('path/to/my_prompt.prompt.md')
+structured_prompt = StructuredPrompt.from_promptdown_file('path/to/your_prompt_file.prompt.md')
 print(structured_prompt)
 ```
 
 ### Advanced Usage
 
-You can also parse a Promptdown string directly:
+Promptdown provides several methods for loading and utilizing structured prompts beyond the basic file usage. Here are more advanced ways to integrate Promptdown into your projects:
+
+#### Parsing a Prompt from a String
+
+For scenarios where you have the prompt data as a string (perhaps dynamically generated or retrieved from an external source), you can parse it directly:
 
 ```python
+from promptdown import StructuredPrompt
+
 promptdown_string = """
 # My Prompt
 
 ## System Message
 
 You are a helpful assistant.
 
@@ -74,14 +80,28 @@
 | Assistant | I'd be happy to help. What seems to be the problem? |
 """
 
 structured_prompt = StructuredPrompt.from_promptdown_string(promptdown_string)
 print(structured_prompt)
 ```
 
+#### Loading Prompts from Package Resources
+
+For applications where prompts are bundled within Python packages, Promptdown can load prompts directly from these resources. This approach is useful for distributing prompts alongside Python libraries or applications:
+
+```python
+from promptdown import StructuredPrompt
+
+# Replace 'your_package' with the actual package name and 'your_prompt_file.prompt.md' with the resource file name
+structured_prompt = StructuredPrompt.from_package_resource('your_package', 'your_prompt_file.prompt.md')
+print(structured_prompt)
+```
+
+This method facilitates easy management of prompts within a package, ensuring that they can be versioned, shared, and reused effectively.
+
 ## Contributing
 
 Contributions are welcome! Feel free to open an issue or submit a pull request.
 
 ## License
 
 Promptdown is released under the [MIT License](LICENSE).
```

### Comparing `promptdown-0.2.2/pyproject.toml` & `promptdown-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promptdown"
-version = "0.2.2"
+version = "0.3.0"
 description = "A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts"
 authors = [
     { name = "B.T. Franklin", email = "brandon.franklin@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
@@ -37,10 +37,10 @@
 [tool.pdm.build]
 excludes = [
     "tests/**",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "pytest>=8.1.1",
+    "pytest>=8.2.0",
     "flake8>=7.0.0",
 ]
```

### Comparing `promptdown-0.2.2/src/promptdown/promptdown.py` & `promptdown-0.3.0/src/promptdown/promptdown.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import logging
 from dataclasses import dataclass
+import importlib.resources as pkg_resources
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @dataclass
 class Message:
     role: str
@@ -109,23 +110,58 @@
 
         conversation = cls._parse_conversation(conversation_lines)
 
         return cls(name=name, system_message=system_message, conversation=conversation)
 
     @classmethod
     def from_promptdown_file(cls, file_path: str) -> StructuredPrompt:
-        promptdown_string = ""
+        """
+        Load a promptdown file from a filesystem path.
 
-        # Check if the file path ends with ".prompt.md"
+        Args:
+        file_path: The path to the promptdown file.
+
+        Returns:
+        A StructuredPrompt object loaded from the specified file.
+        """
         if not file_path.endswith(".prompt.md"):
             _LOGGER.warning("Promptdown files should end with '.prompt.md'")
 
-        # Load the file from the path
-        with open(file_path, "r") as file:
-            promptdown_string = file.read()
+        try:
+            with open(file_path, "r") as file:
+                promptdown_string = file.read()
+        except FileNotFoundError:
+            _LOGGER.error(f"File {file_path} not found.")
+            raise
+
+        return cls.from_promptdown_string(promptdown_string)
+
+    @classmethod
+    def from_package_resource(
+        cls, package: str, resource_name: str
+    ) -> StructuredPrompt:
+        """
+        Load a promptdown file as a structured prompt from a package resource.
+
+        Args:
+        package: The package name where the resource is located.
+        resource_name: The name of the promptdown resource file.
+
+        Returns:
+        A StructuredPrompt object loaded from the specified package resource.
+        """
+        if not resource_name.endswith(".prompt.md"):
+            _LOGGER.warning("Promptdown files should end with '.prompt.md'")
+
+        try:
+            with pkg_resources.open_text(package, resource_name) as file:
+                promptdown_string = file.read()
+        except FileNotFoundError:
+            _LOGGER.error(f"File {resource_name} not found in package {package}.")
+            raise
 
         return cls.from_promptdown_string(promptdown_string)
 
     def to_promptdown_string(self) -> str:
         lines: list[str] = []
 
         # Add the name of the prompt
```

### Comparing `promptdown-0.2.2/src/promptdown/promptdown.pyi` & `promptdown-0.3.0/src/promptdown/promptdown.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 @dataclass
 class Message:
     role: str
     content: str
     name: str | None = ...
     def __eq__(self, other: object) -> bool: ...
-    def __init__(self, role, content, name) -> None: ...
+    def __init__(self, role, content, name=...) -> None: ...
 
 @dataclass
 class StructuredPrompt:
     name: str
     system_message: str
     conversation: list[Message]
     def __eq__(self, other: object) -> bool: ...
     @classmethod
     def from_promptdown_string(cls, promptdown_string: str) -> StructuredPrompt: ...
     @classmethod
     def from_promptdown_file(cls, file_path: str) -> StructuredPrompt: ...
+    @classmethod
+    def from_package_resource(cls, package: str, resource_name: str) -> StructuredPrompt: ...
     def to_promptdown_string(self) -> str: ...
     def to_promptdown_file(self, file_path: str) -> None: ...
     def __init__(self, name, system_message, conversation) -> None: ...
```

### Comparing `promptdown-0.2.2/PKG-INFO` & `promptdown-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: promptdown
-Version: 0.2.2
+Version: 0.3.0
 Summary: A package for loading promptdown files, which are a special type of markdown file for defining structured LLM prompts
-Author-Email: B.T. Franklin <brandon.franklin@gmail.com>
+Author-Email: "B.T. Franklin" <brandon.franklin@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: File Formats
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -62,23 +62,29 @@
 ```
 
 Then, you can parse this file into a `StructuredPrompt` object using Promptdown:
 
 ```python
 from promptdown import StructuredPrompt
 
-structured_prompt = StructuredPrompt.from_promptdown_file('path/to/my_prompt.prompt.md')
+structured_prompt = StructuredPrompt.from_promptdown_file('path/to/your_prompt_file.prompt.md')
 print(structured_prompt)
 ```
 
 ### Advanced Usage
 
-You can also parse a Promptdown string directly:
+Promptdown provides several methods for loading and utilizing structured prompts beyond the basic file usage. Here are more advanced ways to integrate Promptdown into your projects:
+
+#### Parsing a Prompt from a String
+
+For scenarios where you have the prompt data as a string (perhaps dynamically generated or retrieved from an external source), you can parse it directly:
 
 ```python
+from promptdown import StructuredPrompt
+
 promptdown_string = """
 # My Prompt
 
 ## System Message
 
 You are a helpful assistant.
 
@@ -92,14 +98,28 @@
 | Assistant | I'd be happy to help. What seems to be the problem? |
 """
 
 structured_prompt = StructuredPrompt.from_promptdown_string(promptdown_string)
 print(structured_prompt)
 ```
 
+#### Loading Prompts from Package Resources
+
+For applications where prompts are bundled within Python packages, Promptdown can load prompts directly from these resources. This approach is useful for distributing prompts alongside Python libraries or applications:
+
+```python
+from promptdown import StructuredPrompt
+
+# Replace 'your_package' with the actual package name and 'your_prompt_file.prompt.md' with the resource file name
+structured_prompt = StructuredPrompt.from_package_resource('your_package', 'your_prompt_file.prompt.md')
+print(structured_prompt)
+```
+
+This method facilitates easy management of prompts within a package, ensuring that they can be versioned, shared, and reused effectively.
+
 ## Contributing
 
 Contributions are welcome! Feel free to open an issue or submit a pull request.
 
 ## License
 
 Promptdown is released under the [MIT License](LICENSE).
```

