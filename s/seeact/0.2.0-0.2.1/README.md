# Comparing `tmp/seeact-0.2.0.tar.gz` & `tmp/seeact-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeact-0.2.0.tar", last modified: Sun Apr 28 14:58:47 2024, max compression
+gzip compressed data, was "seeact-0.2.1.tar", last modified: Mon Apr 29 00:16:30 2024, max compression
```

## Comparing `seeact-0.2.0.tar` & `seeact-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-28 14:58:47.745902 seeact-0.2.0/
--rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-27 21:47:13.000000 seeact-0.2.0/LICENSE
--rw-r--r--   0 geminigby   (501) staff       (20)    13313 2024-04-28 14:58:47.745491 seeact-0.2.0/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)     1060 2024-04-28 14:58:45.000000 seeact-0.2.0/pyproject.toml
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-28 14:58:47.742756 seeact-0.2.0/seeact/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-28 14:31:27.000000 seeact-0.2.0/seeact/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    31589 2024-04-28 14:31:27.000000 seeact-0.2.0/seeact/agent.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-28 14:58:47.744104 seeact-0.2.0/seeact/data_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-28 14:31:27.000000 seeact-0.2.0/seeact/data_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-04-27 21:47:13.000000 seeact-0.2.0/seeact/data_utils/format_prompt_utils.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-27 21:47:13.000000 seeact-0.2.0/seeact/data_utils/prompts.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-28 14:58:47.744909 seeact-0.2.0/seeact/demo_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-27 21:47:13.000000 seeact-0.2.0/seeact/demo_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    12699 2024-04-28 13:08:43.000000 seeact-0.2.0/seeact/demo_utils/browser_helper.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7555 2024-04-28 12:43:23.000000 seeact-0.2.0/seeact/demo_utils/format_prompt.py
--rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-27 22:00:35.000000 seeact-0.2.0/seeact/demo_utils/inference_engine.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-28 14:58:47.745233 seeact-0.2.0/seeact.egg-info/
--rw-r--r--   0 geminigby   (501) staff       (20)    13313 2024-04-28 14:58:47.000000 seeact-0.2.0/seeact.egg-info/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-04-28 14:58:47.000000 seeact-0.2.0/seeact.egg-info/SOURCES.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-04-28 14:58:47.000000 seeact-0.2.0/seeact.egg-info/dependency_links.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-04-28 14:58:47.000000 seeact-0.2.0/seeact.egg-info/requires.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-04-28 14:58:47.000000 seeact-0.2.0/seeact.egg-info/top_level.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-04-28 14:58:47.745982 seeact-0.2.0/setup.cfg
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.665407 seeact-0.2.1/
+-rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-29 00:05:59.000000 seeact-0.2.1/LICENSE
+-rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 00:16:30.665061 seeact-0.2.1/PKG-INFO
+-rw-r--r--   0 geminigby   (501) staff       (20)     1123 2024-04-29 00:16:12.000000 seeact-0.2.1/pyproject.toml
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.661679 seeact-0.2.1/seeact/
+-rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)    32175 2024-04-29 00:14:47.000000 seeact-0.2.1/seeact/agent.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.663189 seeact-0.2.1/seeact/data_utils/
+-rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/data_utils/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/data_utils/format_prompt_utils.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/data_utils/prompts.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.664458 seeact-0.2.1/seeact/demo_utils/
+-rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/demo_utils/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)    12899 2024-04-29 00:12:06.000000 seeact-0.2.1/seeact/demo_utils/browser_helper.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     7555 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/demo_utils/format_prompt.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/demo_utils/inference_engine.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.664794 seeact-0.2.1/seeact.egg-info/
+-rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/PKG-INFO
+-rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/SOURCES.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/dependency_links.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/requires.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/top_level.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-04-29 00:16:30.665475 seeact-0.2.1/setup.cfg
```

### Comparing `seeact-0.2.0/LICENSE` & `seeact-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seeact-0.2.0/PKG-INFO` & `seeact-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.0
+Version: 0.2.1
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
-Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>
+Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
         
         Copyright (c) 2024 OSU Natural Language Processing Group
```

### Comparing `seeact-0.2.0/pyproject.toml` & `seeact-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seeact"
-version = "0.2.0"
+version = "0.2.1"
 description = "SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents."
 authors = [
     {name = "Boyu Gou", email = "gou.43@buckeyemail.osu.edu"},
-    {name = "Boyuan Zheng", email = "zheng.2372@osu.edu"}
+    {name = "Boyuan Zheng", email = "zheng.2372@osu.edu"},
+    {name = "Zheng Du", email = "du.913@buckeyemail.osu.edu"}
 ]
 license = {file="LICENSE"}
 readme = "https://github.com/OSU-NLP-Group/SeeAct/blob/main/README.md"
 requires-python = ">=3.9"
 
 dependencies = [
     "backoff",
```

### Comparing `seeact-0.2.0/seeact/__init__.py` & `seeact-0.2.1/seeact/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.0/seeact/agent.py` & `seeact-0.2.1/seeact/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 import traceback
 from datetime import datetime
-
+import json
 import toml
-from playwright.async_api import async_playwright
+from playwright.async_api import async_playwright,Locator
 
 from .data_utils.format_prompt_utils import get_index_from_option_name, generate_new_query_prompt, \
     generate_new_referring_prompt, format_options
 from .demo_utils.browser_helper import normal_launch_async, normal_new_context_async, \
     get_interactive_elements_with_playwright, select_option, saveconfig
 from .demo_utils.format_prompt import format_choices, postprocess_action_lmm
 from .demo_utils.inference_engine import OpenAIEngine, load_openai_api_key
@@ -620,16 +620,28 @@
             self.session_control['context'] = None
             await close_context.close()
             self.logger.info("Browser context closed.")
         except Exception as e:
             self.logger.info(e)
 
         final_json = {"task": self.tasks, "website": self.config["basic"]["default_website"],
-                      "num_step": len(self.taken_actions), "action_history": self.taken_actions,"all_predictions":self.predictions}
-        import json
+                      "num_step": len(self.taken_actions), "action_history": self.taken_actions}
+
+        def locator_serializer(obj):
+            """Convert non-serializable objects to a serializable format."""
+            if isinstance(obj, Locator):
+                # Assuming Locator has attributes 'frame' and 'selector' you want to serialize
+                return {'frame': str(obj.frame), 'selector': str(obj.selector)}
+            raise TypeError(f"Object of type {obj.__class__.__name__} is not JSON serializable")
+
+        # Using the custom default function in json.dump
+        with open('all_predictions.json', 'w') as f:
+            json.dump(self.predictions, f, default=locator_serializer, indent=4)
+
+
         with open(os.path.join(self.main_path, 'result.json'), 'w', encoding='utf-8') as file:
             json.dump(final_json, file, indent=4)
         self.logger.info("Agent stopped.")
 
         saveconfig(self.config, os.path.join(self.main_path, 'config.toml'))
 
     def clear_action_history(self):
```

### Comparing `seeact-0.2.0/seeact/data_utils/__init__.py` & `seeact-0.2.1/seeact/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.0/seeact/data_utils/format_prompt_utils.py` & `seeact-0.2.1/seeact/data_utils/format_prompt_utils.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.0/seeact/data_utils/prompts.py` & `seeact-0.2.1/seeact/data_utils/prompts.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.0/seeact/demo_utils/browser_helper.py` & `seeact-0.2.1/seeact/demo_utils/browser_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 import asyncio
 from difflib import SequenceMatcher
 from playwright.sync_api import Playwright, expect, sync_playwright
+# from playwright.async_api import async_playwright
 from pathlib import Path
 import toml
 import os
 
 async def normal_launch_async(playwright: Playwright,headless=False,args=None):
     browser = await playwright.chromium.launch(
         traces_dir=None,
@@ -256,14 +257,19 @@
             real_tag_name = await element.evaluate("element => element.tagName.toLowerCase()", timeout=0)
             if real_tag_name in tag_name_list:
                 # already detected
                 return None
             else:
                 tag_head = real_tag_name
 
+        text_element = ['p', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'td', "div"]
+
+        if real_tag_name in text_element:
+            return None
+
         role_value = await element.get_attribute('role', timeout=0)
         type_value = await element.get_attribute('type', timeout=0)
         # await aprint("start to get element description",element,tag_name )
         description = await get_element_description(element, real_tag_name, role_value, type_value)
         if not description:
             return None
 
@@ -360,14 +366,16 @@
 
 
 def saveconfig(config, save_file):
     """
     config is a dictionary.
     save_path: saving path include file name.
     """
+
+
     if isinstance(save_file, str):
         save_file = Path(save_file)
     if isinstance(config, dict):
         with open(save_file, 'w') as f:
             config_without_key = config
             config_without_key["openai"]["api_key"] = "Your API key here"
             toml.dump(config_without_key, f)
```

### Comparing `seeact-0.2.0/seeact/demo_utils/format_prompt.py` & `seeact-0.2.1/seeact/demo_utils/format_prompt.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.0/seeact/demo_utils/inference_engine.py` & `seeact-0.2.1/seeact/demo_utils/inference_engine.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.0/seeact.egg-info/PKG-INFO` & `seeact-0.2.1/seeact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.0
+Version: 0.2.1
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
-Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>
+Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
         
         Copyright (c) 2024 OSU Natural Language Processing Group
```

