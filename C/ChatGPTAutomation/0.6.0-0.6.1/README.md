# Comparing `tmp/ChatGPTAutomation-0.6.0.tar.gz` & `tmp/chatgptautomation-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatGPTAutomation-0.6.0.tar", last modified: Sat Jan  6 16:32:19 2024, max compression
+gzip compressed data, was "chatgptautomation-0.6.1.tar", last modified: Mon Apr 29 07:49:31 2024, max compression
```

## Comparing `ChatGPTAutomation-0.6.0.tar` & `chatgptautomation-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-01-06 16:32:19.182067 ChatGPTAutomation-0.6.0/
-drwxrwxrwx   0        0        0        0 2024-01-06 16:32:19.182067 ChatGPTAutomation-0.6.0/ChatGPTAutomation.egg-info/
--rw-rw-rw-   0        0        0     9629 2024-01-06 16:32:18.000000 ChatGPTAutomation-0.6.0/ChatGPTAutomation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2024-01-06 16:32:18.000000 ChatGPTAutomation-0.6.0/ChatGPTAutomation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-06 16:32:18.000000 ChatGPTAutomation-0.6.0/ChatGPTAutomation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      827 2024-01-06 16:32:18.000000 ChatGPTAutomation-0.6.0/ChatGPTAutomation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-01-06 16:32:18.000000 ChatGPTAutomation-0.6.0/ChatGPTAutomation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2023-12-19 11:28:47.000000 ChatGPTAutomation-0.6.0/LICENCE.md
--rw-rw-rw-   0        0        0     9629 2024-01-06 16:32:19.182067 ChatGPTAutomation-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     6925 2024-01-06 16:27:51.000000 ChatGPTAutomation-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-01-06 16:32:19.166434 ChatGPTAutomation-0.6.0/chatgpt_automation/
--rw-rw-rw-   0        0        0        0 2023-12-19 11:28:47.000000 ChatGPTAutomation-0.6.0/chatgpt_automation/__init__.py
--rw-rw-rw-   0        0        0    39524 2024-01-06 16:23:55.000000 ChatGPTAutomation-0.6.0/chatgpt_automation/chatgpt_automation.py
--rw-rw-rw-   0        0        0      272 2024-01-06 12:29:47.000000 ChatGPTAutomation-0.6.0/chatgpt_automation/test.py
--rw-rw-rw-   0        0        0       42 2024-01-06 16:32:19.182067 ChatGPTAutomation-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1454 2024-01-06 16:30:17.000000 ChatGPTAutomation-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-06 16:32:19.182067 ChatGPTAutomation-0.6.0/tests/
--rw-rw-rw-   0        0        0        0 2023-12-19 11:28:47.000000 ChatGPTAutomation-0.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-12-19 11:28:47.000000 ChatGPTAutomation-0.6.0/tests/test_chatgpt_automation.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:49:31.454935 chatgptautomation-0.6.1/
+drwxrwxrwx   0        0        0        0 2024-04-29 07:49:31.451560 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/
+-rw-rw-rw-   0        0        0     9679 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      399 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      827 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-29 07:49:31.000000 chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/LICENCE.md
+-rw-rw-rw-   0        0        0     9679 2024-04-29 07:49:31.453810 chatgptautomation-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6925 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 07:49:31.446225 chatgptautomation-0.6.1/chatgpt_automation/
+-rw-rw-rw-   0        0        0        0 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/chatgpt_automation/__init__.py
+-rw-rw-rw-   0        0        0    39539 2024-04-29 07:29:15.000000 chatgptautomation-0.6.1/chatgpt_automation/chatgpt_automation.py
+-rw-rw-rw-   0        0        0     5956 2024-04-29 07:35:24.000000 chatgptautomation-0.6.1/chatgpt_automation/chromedriver_manager.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 07:49:31.454935 chatgptautomation-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1504 2024-04-29 07:39:58.000000 chatgptautomation-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 07:49:31.449880 chatgptautomation-0.6.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2762 2024-04-28 19:36:18.000000 chatgptautomation-0.6.1/tests/test_chatgpt_automation.py
```

### Comparing `ChatGPTAutomation-0.6.0/ChatGPTAutomation.egg-info/PKG-INFO` & `chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ChatGPTAutomation
-Version: 0.6.0
-Summary: A Python package for automating interactions with ChatGPT using Selenium.
+Version: 0.6.1
+Summary: A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation
 Home-page: https://github.com/iamseyedalipro/ChatGPTAutomation
 Author: Seyed Ali Hosseini
 Author-email: iamseyedalipro@gmail.com
 Keywords: chatgpt automation selenium openai chatbot test automation webdriver gpt-3 automation gpt-4 automation file upload automation chat history retrieval login automation developers QA testers automation engineers pytest robot framework python library automation library best chatgpt automation tool selenium chatgpt integration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `ChatGPTAutomation-0.6.0/ChatGPTAutomation.egg-info/requires.txt` & `chatgptautomation-0.6.1/ChatGPTAutomation.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ChatGPTAutomation-0.6.0/LICENCE.md` & `chatgptautomation-0.6.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `ChatGPTAutomation-0.6.0/PKG-INFO` & `chatgptautomation-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ChatGPTAutomation
-Version: 0.6.0
-Summary: A Python package for automating interactions with ChatGPT using Selenium.
+Version: 0.6.1
+Summary: A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation
 Home-page: https://github.com/iamseyedalipro/ChatGPTAutomation
 Author: Seyed Ali Hosseini
 Author-email: iamseyedalipro@gmail.com
 Keywords: chatgpt automation selenium openai chatbot test automation webdriver gpt-3 automation gpt-4 automation file upload automation chat history retrieval login automation developers QA testers automation engineers pytest robot framework python library automation library best chatgpt automation tool selenium chatgpt integration
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
```

### Comparing `ChatGPTAutomation-0.6.0/README.md` & `chatgptautomation-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ChatGPTAutomation-0.6.0/chatgpt_automation/chatgpt_automation.py` & `chatgptautomation-0.6.1/chatgpt_automation/chatgpt_automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from selenium.common.exceptions import TimeoutException
 from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import WebDriverException
 from selenium.webdriver.common.action_chains import ActionChains
 import logging
 import platform
 import pyperclip
-from webdriver_manager.chrome import ChromeDriverManager
+from chatgpt_automation.chromedriver_manager import ChromeDriverManager
 # Configure logging
 logging.basicConfig(filename='chatgpt_automation.log', level=logging.INFO,
                     format='%(asctime)s:%(levelname)s:%(message)s')
 
 
 class ChatGPTLocators:
     MSG_BOX_INPUT = (By.CSS_SELECTOR, 'textarea#prompt-textarea')
```

### Comparing `ChatGPTAutomation-0.6.0/setup.py` & `chatgptautomation-0.6.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 # Read requirements from the requirements.txt file
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='ChatGPTAutomation',
-    version='0.6.0',
+    version='0.6.1',
     author='Seyed Ali Hosseini',
     author_email='iamseyedalipro@gmail.com',
-    description='A Python package for automating interactions with ChatGPT using Selenium.',
+    description='A Python package for automating interactions with ChatGPT using Selenium. Chatgpt automation without api. Chatgptautomation',
     long_description=open('README.md', encoding="utf8").read(),
     long_description_content_type='text/markdown',
     url='https://github.com/iamseyedalipro/ChatGPTAutomation',
     packages=find_packages(),
     install_requires=requirements,
     classifiers=[
         'Development Status :: 3 - Alpha',
```

### Comparing `ChatGPTAutomation-0.6.0/tests/test_chatgpt_automation.py` & `chatgptautomation-0.6.1/tests/test_chatgpt_automation.py`

 * *Files identical despite different names*

