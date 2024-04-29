# Comparing `tmp/streamlit_chat_handler-0.1.3.dev3.tar.gz` & `tmp/streamlit_chat_handler-0.1.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_chat_handler-0.1.3.dev3.tar", last modified: Sun Apr 28 02:59:18 2024, max compression
+gzip compressed data, was "streamlit_chat_handler-0.1.4.dev1.tar", last modified: Mon Apr 29 01:18:08 2024, max compression
```

## Comparing `streamlit_chat_handler-0.1.3.dev3.tar` & `streamlit_chat_handler-0.1.4.dev1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:59:18.612244 streamlit_chat_handler-0.1.3.dev3/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.3.dev3/LICENSE
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:59:18.612244 streamlit_chat_handler-0.1.3.dev3/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.3.dev3/README.md
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:59:18.608244 streamlit_chat_handler-0.1.3.dev3/examples/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      690 2024-04-28 02:33:43.000000 streamlit_chat_handler-0.1.3.dev3/examples/template.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-28 02:59:11.000000 streamlit_chat_handler-0.1.3.dev3/pyproject.toml
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.3.dev3/requirements.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-28 02:59:18.612244 streamlit_chat_handler-0.1.3.dev3/setup.cfg
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:59:18.608244 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/__init__.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     9804 2024-04-28 02:57:51.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/_handler.py
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2312 2024-04-28 02:51:11.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/types.py
-drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-28 02:59:18.608244 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/
--rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/PKG-INFO
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      401 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/SOURCES.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/dependency_links.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/requires.txt
--rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-28 02:59:18.000000 streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/top_level.txt
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:18:08.279330 streamlit_chat_handler-0.1.4.dev1/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1083 2024-04-23 04:06:28.000000 streamlit_chat_handler-0.1.4.dev1/LICENSE
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-29 01:18:08.279330 streamlit_chat_handler-0.1.4.dev1/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2780 2024-04-23 04:03:07.000000 streamlit_chat_handler-0.1.4.dev1/README.md
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:18:08.279330 streamlit_chat_handler-0.1.4.dev1/examples/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      728 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.4.dev1/examples/template.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1291 2024-04-28 03:20:11.000000 streamlit_chat_handler-0.1.4.dev1/examples/template_expander.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     1313 2024-04-29 01:17:25.000000 streamlit_chat_handler-0.1.4.dev1/pyproject.toml
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      363 2024-04-25 04:44:43.000000 streamlit_chat_handler-0.1.4.dev1/requirements.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       38 2024-04-29 01:18:08.279330 streamlit_chat_handler-0.1.4.dev1/setup.cfg
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:18:08.279330 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler/
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      110 2024-04-23 00:45:47.000000 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler/__init__.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)    10831 2024-04-29 01:16:55.000000 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler/_handler.py
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)     2313 2024-04-28 03:22:35.000000 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler/types.py
+drwxrwxr-x   0 eduardo   (1000) eduardo   (1000)        0 2024-04-29 01:18:08.279330 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler.egg-info/
+-rw-r--r--   0 eduardo   (1000) eduardo   (1000)     3737 2024-04-29 01:18:08.000000 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler.egg-info/PKG-INFO
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      431 2024-04-29 01:18:08.000000 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler.egg-info/SOURCES.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)        1 2024-04-29 01:18:08.000000 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler.egg-info/dependency_links.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)      279 2024-04-29 01:18:08.000000 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler.egg-info/requires.txt
+-rw-rw-r--   0 eduardo   (1000) eduardo   (1000)       42 2024-04-29 01:18:08.000000 streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler.egg-info/top_level.txt
```

### Comparing `streamlit_chat_handler-0.1.3.dev3/LICENSE` & `streamlit_chat_handler-0.1.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev3/PKG-INFO` & `streamlit_chat_handler-0.1.4.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.3.dev3
+Version: 0.1.4.dev1
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

### Comparing `streamlit_chat_handler-0.1.3.dev3/README.md` & `streamlit_chat_handler-0.1.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_chat_handler-0.1.3.dev3/examples/template.py` & `streamlit_chat_handler-0.1.4.dev1/examples/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 from streamlit_chat_handler import StreamlitChatHandler
 
 
 if "session_id" not in st.session_state:
     st.session_state["session_id"] = str(uuid.uuid4())
 
-print(type(st.session_state))
-
 st.title("Template")
 
 chat_handler = StreamlitChatHandler(
     st.session_state,
     session_id=st.session_state["session_id"],
 ).render()
 
 if prompt := st.chat_input("Digite aqui..."):
     chat_handler.append(role="user", type="markdown", content=prompt, render=True)
 
     with st.spinner("Processando..."):
         sleep(1)
         chat_handler.append(
-            role="assistant", type="markdown", content="resposta", render=True
+            role="assistant",
+            type="markdown",
+            content=f'{chat_handler.step_counter} - resposta',
+            render=True,
         )
+
```

### Comparing `streamlit_chat_handler-0.1.3.dev3/pyproject.toml` & `streamlit_chat_handler-0.1.4.dev1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 keywords = ["sample", "setuptools", "development"]
 authors = [
   {name = "Eduardo Messias de Morais", email = "emdemor415@gmail.com" },
 ]
-version = "0.1.3dev03"
+version = "0.1.4dev01"
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 lint = [
     "black==23.7.0",
     "flake8==6.1.0",
     "Flake8-pyproject==1.2.3",
```

### Comparing `streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/_handler.py` & `streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler/_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import uuid
-from typing import Any, Literal, Tuple
+from typing import Any, List, Literal, Tuple
 from collections import OrderedDict
 
 import streamlit as st
 from loguru import logger
 from streamlit.runtime.state.session_state_proxy import SessionStateProxy
 
 from streamlit_chat_handler.types import StreamlitChatElement
@@ -69,18 +69,18 @@
     def append(
         self,
         role: Literal["user", "assistant"] = None,
         type: str = None,
         content: Any = None,
         index: str | None = None,
         render: bool = False,
-        chat_element: StreamlitChatElement | None = None,
         parent: str | None = None,
         parent_args: Tuple[Any, ...] = (),
         parent_kwargs: dict[str, Any] = {},
+        chat_element: StreamlitChatElement | None = None,
         *args,
         **kwargs,
     ) -> Any | None:
         """Append a new chat element to the session state.
 
         Args:
             role: The role of the message ('user' or 'assistant').
@@ -109,14 +109,41 @@
 
         self.session_state[self.elements_label][index] = chat_element
 
         if render:
             return chat_element.render()
         return self
 
+    def append_multiple(
+        self, elements: list[StreamlitChatElement], render: bool = False
+    ) -> None:
+        """Append multiple chat elements to the session state."""
+
+        chat_element = OrderedDict({self._set_index(): element for element in elements})
+
+        for index, element in chat_element.items:
+            self.append(
+                role=element.role,
+                type=element.type,
+                content=element.content,
+                index=index,
+                render=False,  # Aqui, os componentes serão renderizados separadamente
+                parent=element.parent,
+                parent_args=element.parent_args,
+                parent_kwargs=element.parent_kwargs,
+            )
+
+        if render:
+            response = self._render_elements(chat_element)
+
+            for index, value in response.items():
+                if index in self.rendered_elements:
+                    del self.rendered_elements[index]
+                self.rendered_elements[index] = value
+
     def increment_step_counter(self) -> None:
         """Finish the current step."""
         self.step_counter += 1
 
     def render_last(self) -> None:
         """Render the last added chat element."""
         last_key, last_element = _get_last_item(self.session_state[self.elements_label])
@@ -141,15 +168,15 @@
             index: The index to set.
 
         Returns:
             The set index.
         """
         if index is None:
             index = uuid.uuid4().hex
-        index = f"{str(self.step_counter).zfill(6)}{index}"
+            return f"{str(self.step_counter).zfill(6)}{index}"
         return index
 
     def _get_chat_element(
         self,
         role: Literal["user", "assistant"] = None,
         type: str = None,
         content: Any = None,
@@ -171,29 +198,29 @@
                 parent_kwargs=parent_kwargs,
                 args=args,
                 kwargs=kwargs,
             )
         else:
             raise ValueError("Missing required arguments for StreamlitChatElement.")
 
-    @staticmethod
     def _render_elements(
-        chat_element: StreamlitChatElement | OrderedDict[str, StreamlitChatElement]
+        self,
+        chat_element: StreamlitChatElement | OrderedDict[str, StreamlitChatElement],
     ) -> OrderedDict[str, Any]:
         """Render chat elements, handling both individual elements and collections.
 
         Args:
             chat_element: A single StreamlitChatElement or an OrderedDict of them.
 
         Returns:
             An OrderedDict where keys are the chat element IDs and values are the rendered elements.
         """
 
         if isinstance(chat_element, StreamlitChatElement):
-            chat_element = OrderedDict({uuid.uuid4().hex: chat_element})
+            chat_element = OrderedDict({self._set_index(): chat_element})
 
         chat_element_list = [v for v in chat_element.values()]
         element_groups = _group_elements_by_role(chat_element_list)
 
         response = OrderedDict({})
         count = 0
         for element_list in element_groups:
@@ -275,8 +302,8 @@
 
     return grouped_elements
 
 
 def _check_argument(argument: Any):
     if argument is not None:
         return True
-    return False
+    return False
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler/types.py` & `streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler/types.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
         Example:
             # Assuming an instance `chat_element` with type 'text':
             chat_element.render()  # This would render the content using `st.text()`.
         """
 
         chat_message = st.chat_message(self.role)
         _parent = getattr(chat_message, self.parent)(*self.parent_args, **self.parent_kwargs) if self.parent else chat_message
-        return getattr(_parent, self.type)(self.content, *self.args, **self.kwargs)
+        return getattr(_parent, self.type)(self.content, *self.args, **self.kwargs)
```

### Comparing `streamlit_chat_handler-0.1.3.dev3/streamlit_chat_handler.egg-info/PKG-INFO` & `streamlit_chat_handler-0.1.4.dev1/streamlit_chat_handler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_chat_handler
-Version: 0.1.3.dev3
+Version: 0.1.4.dev1
 Summary: ...
 Author-email: Eduardo Messias de Morais <emdemor415@gmail.com>
 Keywords: sample,setuptools,development
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit==1.33.0
```

