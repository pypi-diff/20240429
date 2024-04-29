# Comparing `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.3.tar.gz` & `tmp/openai_api_with_easy_tools_and_web_browsing-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.3.tar", last modified: Sat Apr 27 15:17:53 2024, max compression
+gzip compressed data, was "openai_api_with_easy_tools_and_web_browsing-1.0.5.tar", last modified: Mon Apr 29 21:34:54 2024, max compression
```

## Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.3.tar` & `openai_api_with_easy_tools_and_web_browsing-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 15:17:53.368651 openai_api_with_easy_tools_and_web_browsing-1.0.3/
--rw-rw-rw-   0        0        0     1087 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     4568 2024-04-27 15:17:53.366649 openai_api_with_easy_tools_and_web_browsing-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3841 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/README.md
--rw-rw-rw-   0        0        0      715 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-27 15:17:53.368651 openai_api_with_easy_tools_and_web_browsing-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-27 15:17:53.344296 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 15:17:53.366649 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
--rw-rw-rw-   0        0        0     4568 2024-04-27 15:17:53.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2024-04-27 15:17:53.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 15:17:53.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-27 15:17:53.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11022 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.py
-drwxrwxrwx   0        0        0        0 2024-04-27 15:17:53.360646 openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/
--rw-rw-rw-   0        0        0     2851 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/test.py
--rw-rw-rw-   0        0        0     2990 2024-04-27 15:15:58.000000 openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/test_fr.py
+drwxrwxrwx   0        0        0        0 2024-04-29 21:34:54.263247 openai_api_with_easy_tools_and_web_browsing-1.0.5/
+-rw-rw-rw-   0        0        0     1087 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4627 2024-04-29 21:34:54.263247 openai_api_with_easy_tools_and_web_browsing-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3837 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/README.md
+-rw-rw-rw-   0        0        0      879 2024-04-29 21:31:52.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 21:34:54.264249 openai_api_with_easy_tools_and_web_browsing-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 21:34:54.252159 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 21:34:54.262244 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/
+-rw-rw-rw-   0        0        0     4627 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2024-04-29 21:34:54.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11022 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.py
+drwxrwxrwx   0        0        0        0 2024-04-29 21:34:54.261244 openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/
+-rw-rw-rw-   0        0        0     2851 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/test.py
+-rw-rw-rw-   0        0        0     2990 2024-04-29 21:19:18.000000 openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/test_fr.py
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.3/LICENSE` & `openai_api_with_easy_tools_and_web_browsing-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.3/PKG-INFO` & `openai_api_with_easy_tools_and_web_browsing-1.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: openai_api_with_easy_tools_and_web_browsing
-Version: 1.0.3
+Version: 1.0.5
 Summary: An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools
 Author-email: ThomLecha <hamster12@hotmail.fr>
 Project-URL: Homepage, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing
 Project-URL: Issues, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openai>=1.3.5
+Requires-Dist: requests>=2.31.0
 
 # openai-api-with-easy-tools-and-web-browsing
 An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools.
 
 Here is an example of capabilities of this library:
 
 If you ask the program:
@@ -26,15 +28,15 @@
 See code below to reproduce this example.
 
 First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
 
 Then, you can use the following code to get started:
 
 ```
-import src.openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
+import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
 
 ### Creation of the Bing search tool ###
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.3/README.md` & `openai_api_with_easy_tools_and_web_browsing-1.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 See code below to reproduce this example.
 
 First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
 
 Then, you can use the following code to get started:
 
 ```
-import src.openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
+import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
 
 ### Creation of the Bing search tool ###
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO` & `openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: openai_api_with_easy_tools_and_web_browsing
-Version: 1.0.3
+Version: 1.0.5
 Summary: An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools
 Author-email: ThomLecha <hamster12@hotmail.fr>
 Project-URL: Homepage, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing
 Project-URL: Issues, https://github.com/ThomLecha/openai-api-with-easy-tools-and-web-browsing/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: openai>=1.3.5
+Requires-Dist: requests>=2.31.0
 
 # openai-api-with-easy-tools-and-web-browsing
 An unofficial OpenAI library for Python, featuring an integrated Bing Custom Search API for web browsing (free) and easy-to-use custom tools.
 
 Here is an example of capabilities of this library:
 
 If you ask the program:
@@ -26,15 +28,15 @@
 See code below to reproduce this example.
 
 First, get the library with [pip](https://pypi.org/project/openai-api-with-easy-tools-and-web-browsing/): **pip install openai-api-with-easy-tools-and-web-browsing**
 
 Then, you can use the following code to get started:
 
 ```
-import src.openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
+import openai_api_with_easy_tools_and_web_browsing as webBrowsingApiGPT
 
 # Enter our API keys
 subscriptionKey = ""
 openAIAPIKey = ""
 
 ### Creation of the Bing search tool ###
```

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.3/src/openai_api_with_easy_tools_and_web_browsing.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.5/src/openai_api_with_easy_tools_and_web_browsing.py`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/test.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/test.py`

 * *Files identical despite different names*

### Comparing `openai_api_with_easy_tools_and_web_browsing-1.0.3/tests/test_fr.py` & `openai_api_with_easy_tools_and_web_browsing-1.0.5/tests/test_fr.py`

 * *Files identical despite different names*

