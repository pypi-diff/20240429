# Comparing `tmp/seeact-0.2.1.tar.gz` & `tmp/seeact-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeact-0.2.1.tar", last modified: Mon Apr 29 00:16:30 2024, max compression
+gzip compressed data, was "seeact-0.2.2.tar", last modified: Mon Apr 29 00:46:11 2024, max compression
```

## Comparing `seeact-0.2.1.tar` & `seeact-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.665407 seeact-0.2.1/
--rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-29 00:05:59.000000 seeact-0.2.1/LICENSE
--rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 00:16:30.665061 seeact-0.2.1/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)     1123 2024-04-29 00:16:12.000000 seeact-0.2.1/pyproject.toml
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.661679 seeact-0.2.1/seeact/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    32175 2024-04-29 00:14:47.000000 seeact-0.2.1/seeact/agent.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.663189 seeact-0.2.1/seeact/data_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/data_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/data_utils/format_prompt_utils.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/data_utils/prompts.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.664458 seeact-0.2.1/seeact/demo_utils/
--rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/demo_utils/__init__.py
--rw-r--r--   0 geminigby   (501) staff       (20)    12899 2024-04-29 00:12:06.000000 seeact-0.2.1/seeact/demo_utils/browser_helper.py
--rw-r--r--   0 geminigby   (501) staff       (20)     7555 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/demo_utils/format_prompt.py
--rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-29 00:05:59.000000 seeact-0.2.1/seeact/demo_utils/inference_engine.py
-drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:16:30.664794 seeact-0.2.1/seeact.egg-info/
--rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/PKG-INFO
--rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/SOURCES.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/dependency_links.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/requires.txt
--rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-04-29 00:16:30.000000 seeact-0.2.1/seeact.egg-info/top_level.txt
--rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-04-29 00:16:30.665475 seeact-0.2.1/setup.cfg
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:46:11.227926 seeact-0.2.2/
+-rw-r--r--   0 geminigby   (501) staff       (20)    11495 2024-04-29 00:05:59.000000 seeact-0.2.2/LICENSE
+-rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 00:46:11.227646 seeact-0.2.2/PKG-INFO
+-rw-r--r--   0 geminigby   (501) staff       (20)     1123 2024-04-29 00:46:08.000000 seeact-0.2.2/pyproject.toml
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:46:11.224239 seeact-0.2.2/seeact/
+-rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.2/seeact/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)    32175 2024-04-29 00:45:49.000000 seeact-0.2.2/seeact/agent.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:46:11.225944 seeact-0.2.2/seeact/data_utils/
+-rw-r--r--   0 geminigby   (501) staff       (20)      607 2024-04-29 00:05:59.000000 seeact-0.2.2/seeact/data_utils/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     4278 2024-04-29 00:05:59.000000 seeact-0.2.2/seeact/data_utils/format_prompt_utils.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     7487 2024-04-29 00:05:59.000000 seeact-0.2.2/seeact/data_utils/prompts.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:46:11.226900 seeact-0.2.2/seeact/demo_utils/
+-rw-r--r--   0 geminigby   (501) staff       (20)        0 2024-04-29 00:05:59.000000 seeact-0.2.2/seeact/demo_utils/__init__.py
+-rw-r--r--   0 geminigby   (501) staff       (20)    13193 2024-04-29 00:45:49.000000 seeact-0.2.2/seeact/demo_utils/browser_helper.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     7555 2024-04-29 00:05:59.000000 seeact-0.2.2/seeact/demo_utils/format_prompt.py
+-rw-r--r--   0 geminigby   (501) staff       (20)     8411 2024-04-29 00:05:59.000000 seeact-0.2.2/seeact/demo_utils/inference_engine.py
+drwxr-xr-x   0 geminigby   (501) staff       (20)        0 2024-04-29 00:46:11.227384 seeact-0.2.2/seeact.egg-info/
+-rw-r--r--   0 geminigby   (501) staff       (20)    13352 2024-04-29 00:46:11.000000 seeact-0.2.2/seeact.egg-info/PKG-INFO
+-rw-r--r--   0 geminigby   (501) staff       (20)      445 2024-04-29 00:46:11.000000 seeact-0.2.2/seeact.egg-info/SOURCES.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)        1 2024-04-29 00:46:11.000000 seeact-0.2.2/seeact.egg-info/dependency_links.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)       53 2024-04-29 00:46:11.000000 seeact-0.2.2/seeact.egg-info/requires.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)        7 2024-04-29 00:46:11.000000 seeact-0.2.2/seeact.egg-info/top_level.txt
+-rw-r--r--   0 geminigby   (501) staff       (20)       38 2024-04-29 00:46:11.227999 seeact-0.2.2/setup.cfg
```

### Comparing `seeact-0.2.1/LICENSE` & `seeact-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seeact-0.2.1/PKG-INFO` & `seeact-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.1
+Version: 0.2.2
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
 Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
```

### Comparing `seeact-0.2.1/pyproject.toml` & `seeact-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seeact"
-version = "0.2.1"
+version = "0.2.2"
 description = "SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents."
 authors = [
     {name = "Boyu Gou", email = "gou.43@buckeyemail.osu.edu"},
     {name = "Boyuan Zheng", email = "zheng.2372@osu.edu"},
     {name = "Zheng Du", email = "du.913@buckeyemail.osu.edu"}
 ]
 license = {file="LICENSE"}
```

### Comparing `seeact-0.2.1/seeact/__init__.py` & `seeact-0.2.2/seeact/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.1/seeact/agent.py` & `seeact-0.2.2/seeact/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,19 +626,19 @@
         final_json = {"task": self.tasks, "website": self.config["basic"]["default_website"],
                       "num_step": len(self.taken_actions), "action_history": self.taken_actions}
 
         def locator_serializer(obj):
             """Convert non-serializable objects to a serializable format."""
             if isinstance(obj, Locator):
                 # Assuming Locator has attributes 'frame' and 'selector' you want to serialize
-                return {'frame': str(obj.frame), 'selector': str(obj.selector)}
+                return str(obj)
             raise TypeError(f"Object of type {obj.__class__.__name__} is not JSON serializable")
 
         # Using the custom default function in json.dump
-        with open('all_predictions.json', 'w') as f:
+        with open(os.path.join(self.main_path, 'all_predictions.json'), 'w', encoding='utf-8') as f:
             json.dump(self.predictions, f, default=locator_serializer, indent=4)
 
 
         with open(os.path.join(self.main_path, 'result.json'), 'w', encoding='utf-8') as file:
             json.dump(final_json, file, indent=4)
         self.logger.info("Agent stopped.")
```

### Comparing `seeact-0.2.1/seeact/data_utils/__init__.py` & `seeact-0.2.2/seeact/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.1/seeact/data_utils/format_prompt_utils.py` & `seeact-0.2.2/seeact/data_utils/format_prompt_utils.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.1/seeact/data_utils/prompts.py` & `seeact-0.2.2/seeact/data_utils/prompts.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.1/seeact/demo_utils/browser_helper.py` & `seeact-0.2.2/seeact/demo_utils/browser_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,15 +115,18 @@
         return first_line
 
 async def get_element_description(element, tag_name, role_value, type_value):
     '''
          Asynchronously generates a descriptive text for a web element based on its tag type.
          Handles various HTML elements like 'select', 'input', and 'textarea', extracting attributes and content relevant to accessibility and interaction.
     '''
-
+    # text_content = await element.inner_text(timeout=0)
+    # text = (text_content or '').strip()
+    #
+    # print(text)
     salient_attributes = [
         "alt",
         "aria-describedby",
         "aria-label",
         "aria-role",
         "input-checked",
         # "input-value",
@@ -165,14 +168,15 @@
             text4 = " | ".join(options)
 
             if not text4:
                 text4 = await element.text_content(timeout=0)
                 if not text4:
                     text4 = await element.inner_text(timeout=0)
 
+
             return parent_value+text1 + remove_extra_eol(text2.strip()) + text3 + text4
 
     input_value = ""
 
     none_input_type = ["submit", "reset", "checkbox", "radio", "button", "file"]
 
     if tag_name == "input" or tag_name == "textarea":
@@ -180,14 +184,16 @@
             text1 = "input value="
             text2 = await element.input_value(timeout=0)
             if text2:
                 input_value = text1 + "\"" + text2 + "\"" + " "
 
     text_content = await element.text_content(timeout=0)
     text = (text_content or '').strip()
+
+    # print(text)
     if text:
         text = remove_extra_eol(text)
         if len(text) > 80:
             text_content_in = await element.inner_text(timeout=0)
             text_in = (text_content_in or '').strip()
             if text_in:
                 return input_value + remove_extra_eol(text_in)
@@ -234,15 +240,15 @@
             return None
 
 
 
         rect = await element.bounding_box() or {'x': -1, 'y': -1, 'width': 0, 'height': 0}
 
 
-        if rect['x']<0 or rect['y']<0 or rect['width']<=4 or rect['height']<=4 or rect['y']+rect['height']>=viewport_size["height"] or rect['x']+ rect['width']>=viewport_size["width"]:
+        if rect['x']<0 or rect['y']<0 or rect['width']<=4 or rect['height']<=4 or rect['y']+rect['height']>viewport_size["height"] or rect['x']+ rect['width']>viewport_size["width"]:
             return None
 
         box_model = [rect['x'], rect['y'], rect['x'] + rect['width'], rect['y'] + rect['height']]
         center_point = (round((box_model[0] + box_model[2]) / 2 / viewport_size["width"], 3),
                         round((box_model[1] + box_model[3]) / 2 / viewport_size["height"], 3))
 
         if center_point in seen_elements:
@@ -257,23 +263,24 @@
             real_tag_name = await element.evaluate("element => element.tagName.toLowerCase()", timeout=0)
             if real_tag_name in tag_name_list:
                 # already detected
                 return None
             else:
                 tag_head = real_tag_name
 
-        text_element = ['p', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'td', "div"]
+        text_element = ['p', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'td', "div","em","center","strong","b","i","small","mark","abbr","cite","q","blockquote","span","nobr"]
 
         if real_tag_name in text_element:
             return None
 
         role_value = await element.get_attribute('role', timeout=0)
         type_value = await element.get_attribute('type', timeout=0)
         # await aprint("start to get element description",element,tag_name )
         description = await get_element_description(element, real_tag_name, role_value, type_value)
+        # print(description)
         if not description:
             return None
 
         if role_value:
             tag_head += " role=" + "\"" + role_value + "\""
         if type_value:
             tag_head += " type=" + "\"" + type_value + "\""
@@ -285,15 +292,16 @@
                      3. box
                      4. selector
                      5. tag
                      '''
         selector = element
         return {"center_point":center_point,"description":description,"tag_with_role":tag_head,"box":box_model,"selector":selector,"tag":real_tag_name}
         # return [center_point, description, tag_head, box_model, selector, real_tag_name]
-    except:
+    except Exception as e:
+        # print(e)
         return None
 
 
 async def get_interactive_elements_with_playwright(page,viewport_size):
     interactive_elements_selectors = [
         'a', 'button',
         'input',
```

### Comparing `seeact-0.2.1/seeact/demo_utils/format_prompt.py` & `seeact-0.2.2/seeact/demo_utils/format_prompt.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.1/seeact/demo_utils/inference_engine.py` & `seeact-0.2.2/seeact/demo_utils/inference_engine.py`

 * *Files identical despite different names*

### Comparing `seeact-0.2.1/seeact.egg-info/PKG-INFO` & `seeact-0.2.2/seeact.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeact
-Version: 0.2.1
+Version: 0.2.2
 Summary: SeeAct is a system for generalist web agents that autonomously carry out tasks on any given website, with a focus on large multimodal models (LMMs) such as GPT-4V(ision). It consists of two main components: (1) A robust codebase that supports running web agents on live websites, and (2) an innovative framework that utilizes LMMs as generalist web agents.
 Author-email: Boyu Gou <gou.43@buckeyemail.osu.edu>, Boyuan Zheng <zheng.2372@osu.edu>, Zheng Du <du.913@buckeyemail.osu.edu>
 License: AI PUBS OPEN RAIL-S LICENSE
         Version 0.1, March 2, 2023
         
         http://licenses.ai/
```

