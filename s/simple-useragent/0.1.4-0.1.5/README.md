# Comparing `tmp/simple-useragent-0.1.4.tar.gz` & `tmp/simple_useragent-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-useragent-0.1.4.tar", last modified: Wed Feb 14 22:39:11 2024, max compression
+gzip compressed data, was "simple_useragent-0.1.5.tar", last modified: Mon Apr 29 18:26:50 2024, max compression
```

## Comparing `simple-useragent-0.1.4.tar` & `simple_useragent-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-02-14 22:39:11.861760 simple-useragent-0.1.4/
--rw-r--r--   0 lennart    (501) staff       (20)      847 2024-02-07 10:43:36.000000 simple-useragent-0.1.4/ACKNOWLEDGMENTS
--rw-r--r--   0 lennart    (501) staff       (20)    35149 2024-02-04 17:22:51.000000 simple-useragent-0.1.4/LICENSE
--rw-r--r--   0 lennart    (501) staff       (20)      224 2024-02-13 14:30:51.000000 simple-useragent-0.1.4/MANIFEST.in
--rw-r--r--   0 lennart    (501) staff       (20)    13017 2024-02-14 22:39:11.861677 simple-useragent-0.1.4/PKG-INFO
--rw-------   0 lennart    (501) staff       (20)    11480 2024-02-14 22:39:09.000000 simple-useragent-0.1.4/README.md
--rw-r--r--   0 lennart    (501) staff       (20)       87 2024-02-04 17:22:51.000000 simple-useragent-0.1.4/pyproject.toml
--rw-r--r--   0 lennart    (501) staff       (20)       96 2024-02-13 19:59:57.000000 simple-useragent-0.1.4/requirements-dev.txt
--rw-r--r--   0 lennart    (501) staff       (20)       78 2024-02-13 14:36:08.000000 simple-useragent-0.1.4/requirements.txt
--rw-------   0 lennart    (501) staff       (20)     1551 2024-02-14 22:39:11.862049 simple-useragent-0.1.4/setup.cfg
-drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-02-14 22:39:11.858841 simple-useragent-0.1.4/src/
-drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-02-14 22:39:11.860349 simple-useragent-0.1.4/src/simple_useragent/
--rw-r--r--   0 lennart    (501) staff       (20)     1849 2024-02-14 22:36:01.000000 simple-useragent-0.1.4/src/simple_useragent/__init__.py
--rw-r--r--   0 lennart    (501) staff       (20)    33452 2024-02-14 22:36:09.000000 simple-useragent-0.1.4/src/simple_useragent/core.py
-drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-02-14 22:39:11.861282 simple-useragent-0.1.4/src/simple_useragent/data/
--rw-r--r--   0 lennart    (501) staff       (20)     8342 2024-02-04 17:22:51.000000 simple-useragent-0.1.4/src/simple_useragent/data/fallback.json
-drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-02-14 22:39:11.861443 simple-useragent-0.1.4/src/simple_useragent.egg-info/
--rw-r--r--   0 lennart    (501) staff       (20)    13017 2024-02-14 22:39:11.000000 simple-useragent-0.1.4/src/simple_useragent.egg-info/PKG-INFO
--rw-r--r--   0 lennart    (501) staff       (20)      472 2024-02-14 22:39:11.000000 simple-useragent-0.1.4/src/simple_useragent.egg-info/SOURCES.txt
--rw-r--r--   0 lennart    (501) staff       (20)        1 2024-02-14 22:39:11.000000 simple-useragent-0.1.4/src/simple_useragent.egg-info/dependency_links.txt
--rw-r--r--   0 lennart    (501) staff       (20)        1 2024-02-14 22:39:11.000000 simple-useragent-0.1.4/src/simple_useragent.egg-info/not-zip-safe
--rw-r--r--   0 lennart    (501) staff       (20)       78 2024-02-14 22:39:11.000000 simple-useragent-0.1.4/src/simple_useragent.egg-info/requires.txt
--rw-r--r--   0 lennart    (501) staff       (20)       17 2024-02-14 22:39:11.000000 simple-useragent-0.1.4/src/simple_useragent.egg-info/top_level.txt
+drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-04-29 18:26:50.354344 simple_useragent-0.1.5/
+-rw-r--r--   0 lennart    (501) staff       (20)      847 2024-04-29 17:38:25.000000 simple_useragent-0.1.5/ACKNOWLEDGMENTS
+-rw-r--r--   0 lennart    (501) staff       (20)    35149 2024-02-04 17:22:51.000000 simple_useragent-0.1.5/LICENSE
+-rw-r--r--   0 lennart    (501) staff       (20)      224 2024-04-29 17:38:25.000000 simple_useragent-0.1.5/MANIFEST.in
+-rw-r--r--   0 lennart    (501) staff       (20)    12841 2024-04-29 18:26:50.354236 simple_useragent-0.1.5/PKG-INFO
+-rw-------   0 lennart    (501) staff       (20)    11304 2024-04-29 18:26:49.000000 simple_useragent-0.1.5/README.md
+-rw-r--r--   0 lennart    (501) staff       (20)       87 2024-02-04 17:22:51.000000 simple_useragent-0.1.5/pyproject.toml
+-rw-r--r--   0 lennart    (501) staff       (20)       96 2024-04-29 17:38:25.000000 simple_useragent-0.1.5/requirements-dev.txt
+-rw-r--r--   0 lennart    (501) staff       (20)       78 2024-04-29 17:38:25.000000 simple_useragent-0.1.5/requirements.txt
+-rw-------   0 lennart    (501) staff       (20)     1551 2024-04-29 18:26:50.354658 simple_useragent-0.1.5/setup.cfg
+drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-04-29 18:26:50.350571 simple_useragent-0.1.5/src/
+drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-04-29 18:26:50.352278 simple_useragent-0.1.5/src/simple_useragent/
+-rw-r--r--   0 lennart    (501) staff       (20)     1928 2024-04-29 18:25:38.000000 simple_useragent-0.1.5/src/simple_useragent/__init__.py
+-rw-r--r--   0 lennart    (501) staff       (20)    34095 2024-04-29 18:25:38.000000 simple_useragent-0.1.5/src/simple_useragent/core.py
+drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-04-29 18:26:50.353589 simple_useragent-0.1.5/src/simple_useragent/data/
+-rw-r--r--   0 lennart    (501) staff       (20)     8342 2024-04-29 17:38:25.000000 simple_useragent-0.1.5/src/simple_useragent/data/fallback.json
+drwxr-xr-x   0 lennart    (501) staff       (20)        0 2024-04-29 18:26:50.353990 simple_useragent-0.1.5/src/simple_useragent.egg-info/
+-rw-r--r--   0 lennart    (501) staff       (20)    12841 2024-04-29 18:26:50.000000 simple_useragent-0.1.5/src/simple_useragent.egg-info/PKG-INFO
+-rw-r--r--   0 lennart    (501) staff       (20)      472 2024-04-29 18:26:50.000000 simple_useragent-0.1.5/src/simple_useragent.egg-info/SOURCES.txt
+-rw-r--r--   0 lennart    (501) staff       (20)        1 2024-04-29 18:26:50.000000 simple_useragent-0.1.5/src/simple_useragent.egg-info/dependency_links.txt
+-rw-r--r--   0 lennart    (501) staff       (20)        1 2024-04-29 18:26:50.000000 simple_useragent-0.1.5/src/simple_useragent.egg-info/not-zip-safe
+-rw-r--r--   0 lennart    (501) staff       (20)       78 2024-04-29 18:26:50.000000 simple_useragent-0.1.5/src/simple_useragent.egg-info/requires.txt
+-rw-r--r--   0 lennart    (501) staff       (20)       17 2024-04-29 18:26:50.000000 simple_useragent-0.1.5/src/simple_useragent.egg-info/top_level.txt
```

### Comparing `simple-useragent-0.1.4/ACKNOWLEDGMENTS` & `simple_useragent-0.1.5/ACKNOWLEDGMENTS`

 * *Files identical despite different names*

### Comparing `simple-useragent-0.1.4/LICENSE` & `simple_useragent-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-useragent-0.1.4/PKG-INFO` & `simple_useragent-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-useragent
-Version: 0.1.4
+Version: 0.1.5
 Summary: Seamlessly fetch authentic and current user agents with ease
 Home-page: https://github.com/Lennolium/simple-useragent
 Author: Lennart Haack
 Author-email: info@lennolium.dev
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Lennolium/simple-useragent/issues
 Project-URL: Source, https://github.com/Lennolium/simple-useragent
@@ -55,15 +55,15 @@
     <img src="https://app.codacy.com/project/badge/Grade/747e8fea69394b10a1f4627babddcf4f" alt="code quality" >
     <a></a>
    <a href="https://github.com/Lennolium/simple-useragent/commits/main" > 
     <img src="https://img.shields.io/github/commit-activity/m/Lennolium/simple-useragent?label=Commit%20Activity&color=yellow" 
 alt="commit activity" >
      <a></a>
   <a href="https://github.com/Lennolium/simple-useragent/releases" > 
-    <img src="https://img.shields.io/badge/Version-0.1.4-brightgreen" 
+    <img src="https://img.shields.io/badge/Version-0.1.5-brightgreen" 
 alt="stable version" >
      <br>
   <a href="https://github.com/Lennolium/simple-useragent/issues" > 
     <img src="https://img.shields.io/github/issues-raw/Lennolium/simple-useragent?label=Open%20Issues&color=critical" alt="open issues" >
   <a href="https://github.com/Lennolium/simple-useragent/issues?q=is%3Aissue+is%3Aclosed" > 
     <img src="https://img.shields.io/github/issues-closed-raw/Lennolium/simple-useragent?label=Closed%20Issues&color=inactive" alt="closed issues" > 
      <a href="https://pepy.tech/project/simple-useragent" > 
@@ -132,89 +132,89 @@
 
 <!--- Installation -->
 
 ## Installation
 
 Just install the package from [PyPi](https://pypi.org/project/simple-useragent/) using pip:
 
-   ```bash
-    pip install simple-useragent
-   ```
+```bash
+pip install simple-useragent
+```
 
 &nbsp;
 
 <!--- Usage -->
 
 ## Usage
 
 #### Quickstart
 
 Just import the package and use the convenience functions. For more advanced usage, you can initialize the class to set custom settings.
 
-   ```python
-    import simple_useragent as sua
+```python
+import simple_useragent as sua
 
-    sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agents (attributes explained below).
-    # [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-    
-    sua.get_list(shuffle=True, force_cached=True)  # Random list of available desktop user agents strings.
-    # ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
-    
-    sua.get_dict()  # Dictionary with all desktop and mobile user agents.
-    # {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
-   ```
+sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agents (attributes explained below).
+# [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+
+sua.get_list(shuffle=True, force_cached=True)  # Random list of available desktop user agents strings.
+# ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
+
+sua.get_dict()  # Dictionary with all desktop and mobile user agents.
+# {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
+```
 &nbsp;
 
 #### Advanced Usage
 
 Import the package and initialize the UserAgents class to set custom settings (optional, see [Settings and Parameters](#settings-and-parameters) for details).
-   ```python
-    import simple_useragent as sua
+```python
+import simple_useragent as sua
 
-    simple_ua = sua.UserAgents(max_retries=3, timeout=5, cache_duration=86400, cache_location='example/path/to/folder')
-   ```
+simple_ua = sua.UserAgents(max_retries=3, timeout=5, cache_duration=86400, cache_location='example/path/to/folder')
+```
 &nbsp;
 
 Fetching User Agents.
-   ```python
-    # Fetch a specified number of random mobile user agent instances (with settings from the class above).
-    simple_ua.get(num=2, shuffle=True, mobile=True)
-    # [UserAgent('Mozilla/5.0 (iPhone ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-   ```  
+```python
+# Fetch a specified number of random mobile user agent instances (with settings from the class above).
+simple_ua.get(num=2, shuffle=True, mobile=True)
+# [UserAgent('Mozilla/5.0 (iPhone ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+```  
 &nbsp;
 
 You can also use the convenience functions to get user agents without initializing the class.
-   ```python
-    sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agent (attributes explained below).
-    # [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-    
-    sua.get_list(force_cached=True)  # List of all available desktop user agents as strings.
-    # ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
-    
-    sua.get_dict()  # Dictionary with all desktop and mobile user agents.
-    # {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
-   ```
+```python
+sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agent (attributes explained below).
+# [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+
+sua.get_list(force_cached=True)  # List of all available desktop user agents as strings.
+# ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
+
+sua.get_dict()  # Dictionary with all desktop and mobile user agents.
+# {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
+```
 &nbsp;
 
 The instance offers attributes for the user agent properties.
-   ```python
-    # Parse a custom string directly to the UserAgent class and access its attributes.
-    obj = sua.parse('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36')
-    obj.string  # 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit ...'
-    obj.browser  # 'Chrome', 'Firefox', 'Safari', 'Edge', 'IE', 'Opera', 'Whale', 'QQ Browser', 'Samsung Browser', 'Other'
-    obj.browser_version  # '110', '109', '537', ...
-    obj.browser_version_minor  # '0', '1', '36', ...
-
-    # You can also access the attributes with square brackets.
-    obj = sua.get(num=1, shuffle=True)[0]
-    obj['os']  # 'Windows', 'macOS', 'Linux', 'Android', 'iOS', 'Other'
-    obj['os_version']  # '10', '7', '11', '14', ...
-    obj['os_version_minor']  # '0', '1', '2', ...
-    obj['mobile']  # True / False
-   ```
+```python
+# Parse a custom string directly to the UserAgent class and access its attributes.
+obj = sua.parse('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36')
+obj.string  # 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit ...'
+obj.browser  # 'Chrome', 'Firefox', 'Safari', 'Edge', 'IE', 'Opera', 'Whale', 'QQ Browser', 'Samsung Browser', 'Other'
+obj.browser_version  # '110', '109', '537', ...
+obj.browser_version_minor  # '0', '1', '36', ...
+
+# You can also access the attributes with square brackets.
+obj = sua.get(num=1, shuffle=True)[0]
+obj['os']  # 'Windows', 'macOS', 'Linux', 'Android', 'iOS', 'Other'
+obj['os_version']  # '10', '7', '11', '14', ...
+obj['os_version_minor']  # '0', '1', '2', ...
+obj['mobile']  # True / False
+```
 &nbsp;
 
 #### Settings and Parameters
 
 The functions can take the following parameters:
 
 - __num:__ The number of user agents to fetch (default: _None_ = gets you all user agents available).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simple-useragent Version: 0.1.4 Summary: Seamlessly
+Metadata-Version: 2.1 Name: simple-useragent Version: 0.1.5 Summary: Seamlessly
 fetch authentic and current user agents with ease Home-page: https://
 github.com/Lennolium/simple-useragent Author: Lennart Haack Author-email:
 info@lennolium.dev License: GPL-3.0 Project-URL: Bug Tracker, https://
 github.com/Lennolium/simple-useragent/issues Project-URL: Source, https://
 github.com/Lennolium/simple-useragent Project-URL: Download, https://
 github.com/Lennolium/simple-useragent/releases/latest Project-URL:
 Documentation, https://github.com/Lennolium/simple-useragent/README.md
```

### Comparing `simple-useragent-0.1.4/README.md` & `simple_useragent-0.1.5/src/simple_useragent.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: simple-useragent
+Version: 0.1.5
+Summary: Seamlessly fetch authentic and current user agents with ease
+Home-page: https://github.com/Lennolium/simple-useragent
+Author: Lennart Haack
+Author-email: info@lennolium.dev
+License: GPL-3.0
+Project-URL: Bug Tracker, https://github.com/Lennolium/simple-useragent/issues
+Project-URL: Source, https://github.com/Lennolium/simple-useragent
+Project-URL: Download, https://github.com/Lennolium/simple-useragent/releases/latest
+Project-URL: Documentation, https://github.com/Lennolium/simple-useragent/README.md
+Platform: any
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Natural Language :: English
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4==4.12.3
+Requires-Dist: platformdirs==4.2.0
+Requires-Dist: requests==2.31.0
+Requires-Dist: ua-parser==0.18.0
+
 <!--- Logo -->
 
 <div align="center">  
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Lennolium/simple-useragent/main/img/banner_dark.png" width="750vw">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Lennolium/simple-useragent/main/img/banner_light.png" width="750vw">
   <img alt="Application Banner" src="https://raw.githubusercontent.com/Lennolium/simple-useragent/main/img/banner_light.png" width="750vw">
@@ -19,15 +55,15 @@
     <img src="https://app.codacy.com/project/badge/Grade/747e8fea69394b10a1f4627babddcf4f" alt="code quality" >
     <a></a>
    <a href="https://github.com/Lennolium/simple-useragent/commits/main" > 
     <img src="https://img.shields.io/github/commit-activity/m/Lennolium/simple-useragent?label=Commit%20Activity&color=yellow" 
 alt="commit activity" >
      <a></a>
   <a href="https://github.com/Lennolium/simple-useragent/releases" > 
-    <img src="https://img.shields.io/badge/Version-0.1.4-brightgreen" 
+    <img src="https://img.shields.io/badge/Version-0.1.5-brightgreen" 
 alt="stable version" >
      <br>
   <a href="https://github.com/Lennolium/simple-useragent/issues" > 
     <img src="https://img.shields.io/github/issues-raw/Lennolium/simple-useragent?label=Open%20Issues&color=critical" alt="open issues" >
   <a href="https://github.com/Lennolium/simple-useragent/issues?q=is%3Aissue+is%3Aclosed" > 
     <img src="https://img.shields.io/github/issues-closed-raw/Lennolium/simple-useragent?label=Closed%20Issues&color=inactive" alt="closed issues" > 
      <a href="https://pepy.tech/project/simple-useragent" > 
@@ -96,89 +132,89 @@
 
 <!--- Installation -->
 
 ## Installation
 
 Just install the package from [PyPi](https://pypi.org/project/simple-useragent/) using pip:
 
-   ```bash
-    pip install simple-useragent
-   ```
+```bash
+pip install simple-useragent
+```
 
 &nbsp;
 
 <!--- Usage -->
 
 ## Usage
 
 #### Quickstart
 
 Just import the package and use the convenience functions. For more advanced usage, you can initialize the class to set custom settings.
 
-   ```python
-    import simple_useragent as sua
+```python
+import simple_useragent as sua
+
+sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agents (attributes explained below).
+# [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+
+sua.get_list(shuffle=True, force_cached=True)  # Random list of available desktop user agents strings.
+# ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
 
-    sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agents (attributes explained below).
-    # [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-    
-    sua.get_list(shuffle=True, force_cached=True)  # Random list of available desktop user agents strings.
-    # ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
-    
-    sua.get_dict()  # Dictionary with all desktop and mobile user agents.
-    # {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
-   ```
+sua.get_dict()  # Dictionary with all desktop and mobile user agents.
+# {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
+```
 &nbsp;
 
 #### Advanced Usage
 
 Import the package and initialize the UserAgents class to set custom settings (optional, see [Settings and Parameters](#settings-and-parameters) for details).
-   ```python
-    import simple_useragent as sua
+```python
+import simple_useragent as sua
 
-    simple_ua = sua.UserAgents(max_retries=3, timeout=5, cache_duration=86400, cache_location='example/path/to/folder')
-   ```
+simple_ua = sua.UserAgents(max_retries=3, timeout=5, cache_duration=86400, cache_location='example/path/to/folder')
+```
 &nbsp;
 
 Fetching User Agents.
-   ```python
-    # Fetch a specified number of random mobile user agent instances (with settings from the class above).
-    simple_ua.get(num=2, shuffle=True, mobile=True)
-    # [UserAgent('Mozilla/5.0 (iPhone ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-   ```  
+```python
+# Fetch a specified number of random mobile user agent instances (with settings from the class above).
+simple_ua.get(num=2, shuffle=True, mobile=True)
+# [UserAgent('Mozilla/5.0 (iPhone ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+```  
 &nbsp;
 
 You can also use the convenience functions to get user agents without initializing the class.
-   ```python
-    sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agent (attributes explained below).
-    # [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-    
-    sua.get_list(force_cached=True)  # List of all available desktop user agents as strings.
-    # ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
-    
-    sua.get_dict()  # Dictionary with all desktop and mobile user agents.
-    # {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
-   ```
+```python
+sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agent (attributes explained below).
+# [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+
+sua.get_list(force_cached=True)  # List of all available desktop user agents as strings.
+# ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
+
+sua.get_dict()  # Dictionary with all desktop and mobile user agents.
+# {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
+```
 &nbsp;
 
 The instance offers attributes for the user agent properties.
-   ```python
-    # Parse a custom string directly to the UserAgent class and access its attributes.
-    obj = sua.parse('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36')
-    obj.string  # 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit ...'
-    obj.browser  # 'Chrome', 'Firefox', 'Safari', 'Edge', 'IE', 'Opera', 'Whale', 'QQ Browser', 'Samsung Browser', 'Other'
-    obj.browser_version  # '110', '109', '537', ...
-    obj.browser_version_minor  # '0', '1', '36', ...
-
-    # You can also access the attributes with square brackets.
-    obj = sua.get(num=1, shuffle=True)[0]
-    obj['os']  # 'Windows', 'macOS', 'Linux', 'Android', 'iOS', 'Other'
-    obj['os_version']  # '10', '7', '11', '14', ...
-    obj['os_version_minor']  # '0', '1', '2', ...
-    obj['mobile']  # True / False
-   ```
+```python
+# Parse a custom string directly to the UserAgent class and access its attributes.
+obj = sua.parse('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36')
+obj.string  # 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit ...'
+obj.browser  # 'Chrome', 'Firefox', 'Safari', 'Edge', 'IE', 'Opera', 'Whale', 'QQ Browser', 'Samsung Browser', 'Other'
+obj.browser_version  # '110', '109', '537', ...
+obj.browser_version_minor  # '0', '1', '36', ...
+
+# You can also access the attributes with square brackets.
+obj = sua.get(num=1, shuffle=True)[0]
+obj['os']  # 'Windows', 'macOS', 'Linux', 'Android', 'iOS', 'Other'
+obj['os_version']  # '10', '7', '11', '14', ...
+obj['os_version_minor']  # '0', '1', '2', ...
+obj['mobile']  # True / False
+```
 &nbsp;
 
 #### Settings and Parameters
 
 The functions can take the following parameters:
 
 - __num:__ The number of user agents to fetch (default: _None_ = gets you all user agents available).
```

#### html2text {}

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1 Name: simple-useragent Version: 0.1.5 Summary: Seamlessly
+fetch authentic and current user agents with ease Home-page: https://
+github.com/Lennolium/simple-useragent Author: Lennart Haack Author-email:
+info@lennolium.dev License: GPL-3.0 Project-URL: Bug Tracker, https://
+github.com/Lennolium/simple-useragent/issues Project-URL: Source, https://
+github.com/Lennolium/simple-useragent Project-URL: Download, https://
+github.com/Lennolium/simple-useragent/releases/latest Project-URL:
+Documentation, https://github.com/Lennolium/simple-useragent/README.md
+Platform: any Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Utilities Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
+Only Classifier: License :: OSI Approved :: GNU General Public License v3
+(GPLv3) Classifier: Operating System :: OS Independent Classifier: Operating
+System :: POSIX :: Linux Classifier: Operating System :: Unix Classifier:
+Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
+Classifier: Natural Language :: English Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Science/Research Requires-Python:
+>=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
+Dist: beautifulsoup4==4.12.3 Requires-Dist: platformdirs==4.2.0 Requires-Dist:
+requests==2.31.0 Requires-Dist: ua-parser==0.18.0
                              [Application Banner]
 
                                 _[_l_a_s_t_ _u_p_d_a_t_e_d_]
                                 _[_c_o_d_e_ _q_u_a_l_i_t_y_]
                                _[_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]
                                _[_s_t_a_b_l_e_ _v_e_r_s_i_o_n_]
                                  _[_o_p_e_n_ _i_s_s_u_e_s_]
```

### Comparing `simple-useragent-0.1.4/setup.cfg` & `simple_useragent-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = simple-useragent
-version = 0.1.4
+version = 0.1.5
 author = Lennart Haack
 author_email = info@lennolium.dev
 license = GPL-3.0
 license_files = LICENSE
 description = Seamlessly fetch authentic and current user agents with ease
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `simple-useragent-0.1.4/src/simple_useragent/__init__.py` & `simple_useragent-0.1.5/src/simple_useragent/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 >> UserAgent('Mozilla/5.0 (iPhone, Safari ...')
 """
 
 # Header.
 __author__ = "Lennart Haack"
 __email__ = "simple-useragent@lennolium.dev"
 __license__ = "GNU GPLv3"
-__version__ = "0.1.4"
-__date__ = "2024-02-14"
+__version__ = "0.1.5"
+__date__ = "2024-04-29"
 __status__ = "Development"
 __github__ = "https://github.com/Lennolium/simple-useragent"
 
 # Imports.
 from .core import UserAgents, UserAgent, get_dict, get_list, get, parse
+
+__all__ = ("UserAgents", "UserAgent", "get_dict", "get_list", "get", "parse")
```

### Comparing `simple-useragent-0.1.4/src/simple_useragent/core.py` & `simple_useragent-0.1.5/src/simple_useragent/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 """
 core.py: Responsible for the core functionality of the package.
 
 This module contains the UserAgent and UserAgents classes, which are
 responsible for parsing and fetching user agents from the public
 'useragents.me' API and caching them locally. You can use the UserAgent
 class to parse a single, custom user agent string and gain access to its
-parsed attributes. 
+parsed attributes.
 """
 from __future__ import annotations
 
 # Header.
 __author__ = "Lennart Haack"
 __email__ = "simple-useragent@lennolium.dev"
 __license__ = "GNU GPLv3"
-__version__ = "0.1.4"
-__date__ = "2024-02-14"
+__version__ = "0.1.5"
+__date__ = "2024-04-29"
 __status__ = "Development"
 __github__ = "https://github.com/Lennolium/simple-useragent"
 
 # Imports.
 import json
 import logging
 import os.path
@@ -35,28 +35,40 @@
 
 # Logging.
 LOGGER = logging.getLogger(__name__)
 logging.basicConfig(level=os.environ.get("LOGLEVEL", "INFO"))
 
 # Fallback user agents if API is not reachable and no cached version
 # is available.
-_FALLBACK_DESKTOP = ["Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
-                     "AppleWebKit/537.36 (KHTML, like Gecko) "
-                     "Chrome/110.0.0.0 Safari/537.36"]
-_FALLBACK_MOBILE = ["Mozilla/5.0 (Linux; Android 10; K) "
-                    "AppleWebKit/537.36 (KHTML, like Gecko) "
-                    "Chrome/120.0.0.0 Mobile Safari/537.3"]
-
-_FALLBACK_JSON = pathlib.Path(os.path.dirname(__file__),
-                              "data",
-                              "fallback.json"
-                              )
-
-_SUPPORTED_BROWSERS = ["Chrome", "Firefox", "Safari", "Opera", "Edge",
-                       "IE", "Samsung Browser", "Whale", "QQ Browser"]
+_FALLBACK_DESKTOP = [
+        "Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
+        "AppleWebKit/537.36 (KHTML, like Gecko) "
+        "Chrome/110.0.0.0 Safari/537.36"
+        ]
+_FALLBACK_MOBILE = [
+        "Mozilla/5.0 (Linux; Android 10; K) "
+        "AppleWebKit/537.36 (KHTML, like Gecko) "
+        "Chrome/120.0.0.0 Mobile Safari/537.3"
+        ]
+
+_FALLBACK_JSON = pathlib.Path(
+        os.path.dirname(__file__), "data", "fallback.json"
+        )
+
+_SUPPORTED_BROWSERS = [
+        "Chrome",
+        "Firefox",
+        "Safari",
+        "Opera",
+        "Edge",
+        "IE",
+        "Samsung Browser",
+        "Whale",
+        "QQ Browser",
+        ]
 _SUPPORTED_OS = ["Windows", "macOS", "Linux", "Android", "iOS"]
 
 
 class UserAgent:
     """
     A class to represent a single parsed user agent.
     """
@@ -80,23 +92,25 @@
         self.browser_version = None
         self.browser_version_minor = None
         self.mobile = None
         self.string = None
 
         # Validate user agent string.
         if not isinstance(user_agent, str):
-            LOGGER.warning(f"User agent string must be of type str. "
-                           f"No {self.__class__.__name__} instance created. "
-                           f"Returning 'None'."
-                           )
+            LOGGER.warning(
+                    f"User agent string must be of type str. "
+                    f"No {self.__class__.__name__} instance created. "
+                    f"Returning 'None'."
+                    )
         elif not user_agent or user_agent.isspace():
-            LOGGER.warning(f"User agent string must not be empty. "
-                           f"No {self.__class__.__name__} instance created. "
-                           f"Returning 'None'."
-                           )
+            LOGGER.warning(
+                    f"User agent string must not be empty. "
+                    f"No {self.__class__.__name__} instance created. "
+                    f"Returning 'None'."
+                    )
         # Input valid: Parse ua string and save to class attributes.
         else:
             self.parse(user_agent)
 
     def __str__(self) -> str:
         """
         Returns the UserAgent instance as a readable string.
@@ -114,15 +128,16 @@
 
         return (
                 f"OS: {self.os} {self.os_version}{os_dot}"
                 f"{self.os_version_minor}, "
                 f"Browser: {self.browser} {self.browser_version}{browser_dot}"
                 f"{self.browser_version_minor}, "
                 f"Mobile: {self.mobile}, "
-                f"String: {self.string}")
+                f"String: {self.string}"
+        )
 
     def __repr__(self) -> str:
         """
         Returns the user agent instance as a representation for fast
         reconstruction.
 
         :return: The UserAgent instance as a shortened representation.
@@ -237,32 +252,33 @@
                 ("chromium", "Chrome"),
                 ("huawei", "Chrome"),
                 ("safari", "Safari"),
                 ("opera", "Opera"),
                 ("microsoft", "Edge"),
                 ("edge", "Edge"),
                 ("ie", "IE"),
-                ("samsung", "Samsung Browser")
+                ("samsung", "Samsung Browser"),
                 ]
 
         browser = parsed["user_agent"]["family"]
         if browser not in _SUPPORTED_BROWSERS:
             browser_lower = browser.lower()
             for key, value in browser_mapping:
                 if key in browser_lower:
                     browser = value
                     break
             else:
                 browser = "Other"
 
         # Fix for Safari on Linux and Windows (not possible).
-        if (browser == "Safari"
-                and (parsed["os"]["family"] == "Linux"
-                     or parsed["os"]["family"] == "Windows"
-                     or parsed["os"]["family"] == "Android")):
+        if browser == "Safari" and (
+                parsed["os"]["family"] == "Linux"
+                or parsed["os"]["family"] == "Windows"
+                or parsed["os"]["family"] == "Android"
+        ):
             browser = "Other"
 
         return browser
 
     @staticmethod
     def __parse_os(parsed: user_agent_parser.Parse) -> str:
         """
@@ -279,15 +295,15 @@
                 ("mac", "macOS"),
                 ("windows", "Windows"),
                 ("linux", "Linux"),
                 ("ubuntu", "Linux"),
                 ("debian", "Linux"),
                 ("fedora", "Linux"),
                 ("android", "Android"),
-                ("ios", "iOS")
+                ("ios", "iOS"),
                 ]
 
         os = parsed["os"]["family"]
         if os not in _SUPPORTED_OS:
             os_lower = os.lower()
             for key, value in os_mapping:
                 if key in os_lower:
@@ -295,19 +311,15 @@
                     break
             else:
                 os = "Other"
 
         return os
 
     @staticmethod
-    def __parse_mobile(
-            string: str,
-            os: str,
-            browser: str
-            ) -> bool:
+    def __parse_mobile(string: str, os: str, browser: str) -> bool:
         """
         Parses if the OS/device is mobile from the user agent string.
 
         :param string: User agent string.
         :type string: str
         :param os: OS name.
         :type os: str
@@ -318,16 +330,19 @@
         """
 
         # Check if OS/device is mobile.
         string_lower = string.lower()
         if os in _SUPPORTED_OS[-2:]:
             return True
 
-        return (browser == "Samsung Browser" or "android" in string_lower or
-                "iphone" in string_lower or "mobile" in string_lower)
+        return (
+                "android" in string_lower
+                or "iphone" in string_lower
+                or "mobile" in string_lower
+        )
 
     def parse(self, string: str) -> None:
         """
         Parses the user agent string and saves the results to the
         class attributes.
 
         This function is called automatically during initialization.
@@ -368,27 +383,30 @@
                         if value is not None:
                             setattr(self, f"{data}_version_minor", value)
                         else:
                             setattr(self, f"{data}_version_minor", "")
 
             # Check if OS/device is mobile.
             self.mobile = self.__parse_mobile(
-                    string=self.string,
-                    os=self.os,
-                    browser=self.browser
+                    string=self.string, os=self.os, browser=self.browser
                     )
 
         except Exception as e:
-            LOGGER.warning(f"Could not parse version numbering from "
-                           f"'user_agent_parser' data: "
-                           f"{str(e.__class__.__name__)}: {str(e)}"
-                           )
+            LOGGER.warning(
+                    f"Could not parse version numbering from "
+                    f"'user_agent_parser' data: "
+                    f"{str(e.__class__.__name__)}: {str(e)}"
+                    )
 
-            for attr in ["browser_version", "browser_version_minor",
-                         "os_version", "os_version_minor"]:
+            for attr in [
+                    "browser_version",
+                    "browser_version_minor",
+                    "os_version",
+                    "os_version_minor",
+                    ]:
                 setattr(self, attr, "")
 
 
 class UserAgents:
     """
     Fetch real world user agents from the public 'useragents.me' API for
     use in a web scraping process to avoid bot detection.
@@ -402,15 +420,15 @@
     :type max_retries: int
     :var timeout: Timeout in seconds for the API request (default=5).
     :type timeout: int
     :var cache_duration: The duration in seconds after which the
         cached user agents are refreshed (default=86400).
     :type cache_duration: int
     :var cache_location: The folder to save the cached user agents in.
-    :type cache_location: str
+    :type cache_location: str.
     """
 
     _user_agents_cached = None
 
     def __init__(
             self,
             max_retries: int = 3,
@@ -483,44 +501,47 @@
 
     def __repr__(self) -> str:
         """
         Returns the UserAgents instance as a representation for fast
         reconstruction.
         """
 
-        return (f"{self.__class__.__name__}"
+        return (
+                f"{self.__class__.__name__}"
                 f"(max_retries={self._max_retries!r}, "
                 f"timeout={self._timeout!r}, "
                 f"cache_duration={self._cache_duration!r}, "
-                f"cache_location={self._cache_location!r})")
+                f"cache_location={self._cache_location!r})"
+        )
 
     @staticmethod
     def __convert_to_list(response_data: list[dict]) -> list[str]:
         """
         Converts the response data from API to a list of user agents,
         sorted by usage percentage.
 
         :param response_data: The response data from the API.
         :type response_data: list[dict]
         :return: A list of user agents sorted by usage percentage.
         :rtype: list[str]
         """
 
         try:
-            sorted_data = sorted(response_data, key=lambda x: x['pct'],
-                                 reverse=True
-                                 )
-            ua_list = [entry['ua'] for entry in sorted_data]
+            sorted_data = sorted(
+                    response_data, key=lambda x: x["pct"], reverse=True
+                    )
+            ua_list = [entry["ua"] for entry in sorted_data]
 
         except Exception as e:
-            LOGGER.warning(f"Could not convert response data from "
-                           f"'useragents.me' to list. Maybe the API changed "
-                           f"its response format? "
-                           f"{str(e.__class__.__name__)}: {str(e)}"
-                           )
+            LOGGER.warning(
+                    f"Could not convert response data from "
+                    f"'useragents.me' to list. Maybe the API changed "
+                    f"its response format? "
+                    f"{str(e.__class__.__name__)}: {str(e)}"
+                    )
             return []
 
         return ua_list
 
     @staticmethod
     def __fallback() -> dict[str, list[str]] | None:
         """
@@ -538,42 +559,39 @@
 
             with open(_FALLBACK_JSON, "r") as fh:
                 response_data = json.load(fh)
 
             return response_data
 
         except Exception as e:
-            LOGGER.error(f"Could not find fallback file, that is shipped "
-                         f"with the package! Verify that the file exists "
-                         f"and if it does, report the issue please.\n"
-                         f"{str(e.__class__.__name__)}: {str(e)}"
-                         )
+            LOGGER.error(
+                    f"Could not find fallback file, that is shipped "
+                    f"with the package! Verify that the file exists "
+                    f"and if it does, report the issue please.\n"
+                    f"{str(e.__class__.__name__)}: {str(e)}"
+                    )
             return
 
-    def __response_data(
-            self,
-            url: str
-            ) -> requests.Response | None:
+    def __response_data(self, url: str) -> requests.Response | None:
         """
         Tries to reach the API for maximum of _max_retries times and
         returns the response data or None if API could not be reached.
 
         :param url: The url to reach.
         :type url: str
         :return: The response data or None if API could not be reached.
         :rtype: requests.Response or None
         """
 
         # Try to reach API for maximum 3 times (default).
         for i in range(1, self._max_retries + 1):
             try:
-                response = requests.get(url=url,
-                                        timeout=self._timeout,
-                                        allow_redirects=True
-                                        )
+                response = requests.get(
+                        url=url, timeout=self._timeout, allow_redirects=True
+                        )
 
             # If connection fails with exception, retry after delay.
             except Exception as e:
                 LOGGER.warning(
                         f"({i}/{self._max_retries}) Try to reach "
                         f"'useragents.me' API failed with exception: "
                         f"{str(e.__class__.__name__)}: {str(e)}. Retrying in "
@@ -626,64 +644,79 @@
             the API or None if the API could not be reached after
             _max_retries.
         :rtype: dict or None
         """
 
         # For mobile user agents, we can not use the api endpoint.
         endpoints = {
-                "desktop": "https://www.useragents.me/api",
+                "desktop": "https://www.useragents.me/",
                 "mobile": "https://www.useragents.me/",
                 }
         response_data = {"desktop": None, "mobile": None, "cached": None}
 
         # Fetch desktop and mobile user agents from API.
         for device, endpoint in endpoints.items():
 
             response = self.__response_data(endpoint)
 
             if not response:
                 return
 
             # For desktop UA, we can use the json response of the API.
+            # FIX: API is offline for several months now. Changed to
+            # parsing the HTML response (Thanks to Nathan Easton).
             if device == "desktop":
+                try:
+                    soup = BeautifulSoup(response.text, "html.parser")
+                    row = soup.find(
+                            "div",
+                            id="most-common-desktop-useragents-json-csv",
+                            class_="row",
+                            )
+                    content = row.find("textarea", class_="form-control").text
 
-                # Rate limit reached.
-                for key in response.json():
-                    if "error" in key:
-                        LOGGER.warning(
-                                "Rate limit reached for 'useragents.me' "
-                                "(15 requests/h)."
-                                )
-                        return
-
-                response_data["desktop"] = \
-                    self.__convert_to_list(response.json()["data"])
+                    # Remove newlines and whitespaces.
+                    content = content.replace("\n", "").replace("  ", "")
+                    print(content)
+                    response_data["desktop"] = self.__convert_to_list(
+                            json.loads(content)
+                            )
 
+                except Exception as e:
+                    LOGGER.warning(
+                            f"Could not parse HTML response from "
+                            f"'useragents.me': "
+                            f"{str(e.__class__.__name__)}: {str(e)}"
+                            )
+                    return
             # For mobile UA, we need to parse the HTML response and
             # extract the user agents from the textarea.
             else:
                 try:
                     soup = BeautifulSoup(response.text, "html.parser")
                     row = soup.find(
-                            "div", id="most-common-mobile-useragents-json-csv",
-                            class_="row"
+                            "div",
+                            id="most-common-mobile-useragents-json-csv",
+                            class_="row",
                             )
                     content = row.find("textarea", class_="form-control").text
 
                     # Remove newlines and whitespaces.
                     content = content.replace("\n", "").replace("  ", "")
 
-                    response_data["mobile"] = \
-                        self.__convert_to_list(json.loads(content))
+                    response_data["mobile"] = self.__convert_to_list(
+                            json.loads(content)
+                            )
 
                 except Exception as e:
-                    LOGGER.warning(f"Could not parse HTML response from "
-                                   f"'useragents.me': "
-                                   f"{str(e.__class__.__name__)}: {str(e)}"
-                                   )
+                    LOGGER.warning(
+                            f"Could not parse HTML response from "
+                            f"'useragents.me': "
+                            f"{str(e.__class__.__name__)}: {str(e)}"
+                            )
                     return
 
         if response_data["desktop"] and response_data["mobile"]:
             # Add current unix timestamp to response data.
             response_data["cached"] = int(time.time())
             return response_data
 
@@ -700,25 +733,23 @@
         :return: A dictionary containing the user agents fetched from
             the local cache or None if local cache could not be read.
         :rtype: dict or None
         """
 
         # Load cached user agents from json file.
         try:
-            fp = pathlib.Path(self._cache_location,
-                              "user_agents.json"
-                              )
+            fp = pathlib.Path(self._cache_location, "user_agents.json")
 
             with open(fp, "r") as fh:
                 response_data = json.load(fh)
 
                 return response_data
 
         except FileNotFoundError:
-            LOGGER.info(
+            LOGGER.debug(
                     "No cached 'user_agents.json' found. Maybe your first run?"
                     )
             return
 
         except Exception as e:
             LOGGER.warning(
                     f"Could not load cached 'user_agents.json': "
@@ -731,47 +762,52 @@
         Checks if the cached user agents are young enough.
 
         :return: True if cached user agents are young enough.
         :rtype: bool
         """
 
         if self._user_agents_cached:
-            if ((int(time.time()) - self._user_agents_cached["cached"]) <
-                    self._cache_duration):
+            if (
+                    int(time.time()) - self._user_agents_cached["cached"]
+            ) < self._cache_duration:
                 return True
 
         return False
 
     @staticmethod
-    def __check_num(num: int,
-                    mobile: bool
-                    ) -> tuple[int, str]:
+    def __check_num(num: int, mobile: bool) -> tuple[int, str]:
         """
         Checks if the requested number of user agents is valid.
 
         :param num: Requested number of user agents.
         :type num: int
         :param mobile: Mobile or desktop user agents requested.
         :return:
         """
 
         # Catch invalid num parameter.
         if num is not None:
             try:
                 num = int(num)
             except (TypeError, ValueError):
-                LOGGER.warning(f"Could not convert '{num}' to int. "
-                               "Returning empty list ..."
-                               )
+                LOGGER.warning(
+                        f"Could not convert '{num}' to int. "
+                        "Returning "
+                        "empty list ..."
+                        )
                 return 0, "mobile"
 
         if num and num < 1:
-            LOGGER.warning(f"You requested '{num}' user agents. "
-                           "Returning empty list ..."
-                           )
+            LOGGER.warning(
+                    f"You requested '{num}' user agents. "
+                    "Returning empty "
+                    ""
+                    ""
+                    "list ..."
+                    )
             return 0, "mobile"  # Device type does not matter.
 
         # Enforce maximum of 45 (23 for mobile) retrievable user agents.
         if mobile:
             device = "mobile"
             num_max = 23
 
@@ -806,59 +842,57 @@
             (default=None).
         :type force_cached: bool
         :return: A dict of desktop and mobile user agents.
         :rtype: dict[str, list[str]]
         """
 
         # 1. Check for memory cached user agents (class attributes).
-        if (self._user_agents_cached
+        if (
+                self._user_agents_cached
                 and self._user_agents_cached["desktop"]
                 and self._user_agents_cached["mobile"]
-                and force_cached is not False):
+                and force_cached is not False
+        ):
 
             # Check if the cached uas are young enough.
             if self.__check_cached():
                 return self._user_agents_cached
 
         # 1.5. Forced use of local file cached user agents.
         if force_cached:
-            LOGGER.info("Forcing the use of local cached user agents ...")
+            LOGGER.debug("Forcing the use of local cached user agents ...")
             self._user_agents_cached = self.__useragents_cached()
 
             if self._user_agents_cached:
                 return self._user_agents_cached
 
             # If no local cached user agents are available.
-            LOGGER.warning("Falling back to historic user agent."
-                           )
-            return {"desktop": _FALLBACK_DESKTOP,
-                    "mobile": _FALLBACK_MOBILE
-                    }
+            LOGGER.warning("Falling back to historic user agent.")
+            return {"desktop": _FALLBACK_DESKTOP, "mobile": _FALLBACK_MOBILE}
 
         # 2. Check for local file cached user agents.
         if force_cached is not False:
             self._user_agents_cached = self.__useragents_cached()
 
             # Check if the cached uas are young enough and return them.
             if self.__check_cached():
                 return self._user_agents_cached
 
         # 3. Call API to fetch user agents and save them to local cache.
         if force_cached is False:
-            LOGGER.info("Forcing the use of 'useragents.me' API instead "
-                        "of local cached user agents first ..."
-                        )
+            LOGGER.debug(
+                    "Forcing the use of 'useragents.me' API instead "
+                    "of local cached user agents first ..."
+                    )
 
         self._user_agents_cached = self.__useragents_api()
 
         if self._user_agents_cached:
             try:
-                fp = pathlib.Path(self._cache_location,
-                                  "user_agents.json"
-                                  )
+                fp = pathlib.Path(self._cache_location, "user_agents.json")
 
                 # Save user agents to local file cache.
                 with open(fp, "w") as fh:
                     json.dump(self._user_agents_cached, fh)
 
             except Exception as e:
                 LOGGER.warning(
@@ -873,30 +907,28 @@
         # 4. Fall back to historic local file user agents.
         LOGGER.error("Falling back to historic file user agents.")
         self._user_agents_cached = self.__fallback()
         if self._user_agents_cached:
             return self._user_agents_cached
 
         # 5. Final fall back to historic hard-coded user agents.
-        LOGGER.critical("Falling back to historic hard-coded user agents."
-                        "These are not up to date and limited in number."
-                        "This should never happen. Please report this issue."
-                        )
-        return {"desktop": _FALLBACK_DESKTOP,
-                "mobile": _FALLBACK_MOBILE
-                }
+        LOGGER.critical(
+                "Falling back to historic hard-coded user agents."
+                "These are not up to date and limited in number."
+                "This should never happen. Please report this issue."
+                )
+        return {"desktop": _FALLBACK_DESKTOP, "mobile": _FALLBACK_MOBILE}
 
     def get_list(
             self,
             num: int = None,
             mobile: bool = False,
             shuffle: bool = False,
             force_cached: bool = None,
             ) -> list[str]:
-
         """
         Fetches a list of usage weighted user agents as strings.
 
         :param num: The number of user agents to fetch (desktop=45,
             mobile=23).
         :type num: int
         :param mobile: Fetches mobile user agents (default=False).
@@ -964,7 +996,13 @@
 
 
 # Convenience functions (for more settings, initialize the class).
 get_list = UserAgents().get_list
 get_dict = UserAgents().get_dict
 get = UserAgents().get
 parse = UserAgent
+
+if __name__ == "__main__":
+    # Test the package.
+    ua = get(num=5)
+    for i, u in enumerate(ua):
+        print(f"{i + 1}. {u}")
```

### Comparing `simple-useragent-0.1.4/src/simple_useragent/data/fallback.json` & `simple_useragent-0.1.5/src/simple_useragent/data/fallback.json`

 * *Files identical despite different names*

### Comparing `simple-useragent-0.1.4/src/simple_useragent.egg-info/PKG-INFO` & `simple_useragent-0.1.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: simple-useragent
-Version: 0.1.4
-Summary: Seamlessly fetch authentic and current user agents with ease
-Home-page: https://github.com/Lennolium/simple-useragent
-Author: Lennart Haack
-Author-email: info@lennolium.dev
-License: GPL-3.0
-Project-URL: Bug Tracker, https://github.com/Lennolium/simple-useragent/issues
-Project-URL: Source, https://github.com/Lennolium/simple-useragent
-Project-URL: Download, https://github.com/Lennolium/simple-useragent/releases/latest
-Project-URL: Documentation, https://github.com/Lennolium/simple-useragent/README.md
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Natural Language :: English
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: beautifulsoup4==4.12.3
-Requires-Dist: platformdirs==4.2.0
-Requires-Dist: requests==2.31.0
-Requires-Dist: ua-parser==0.18.0
-
 <!--- Logo -->
 
 <div align="center">  
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Lennolium/simple-useragent/main/img/banner_dark.png" width="750vw">
   <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Lennolium/simple-useragent/main/img/banner_light.png" width="750vw">
   <img alt="Application Banner" src="https://raw.githubusercontent.com/Lennolium/simple-useragent/main/img/banner_light.png" width="750vw">
@@ -55,15 +19,15 @@
     <img src="https://app.codacy.com/project/badge/Grade/747e8fea69394b10a1f4627babddcf4f" alt="code quality" >
     <a></a>
    <a href="https://github.com/Lennolium/simple-useragent/commits/main" > 
     <img src="https://img.shields.io/github/commit-activity/m/Lennolium/simple-useragent?label=Commit%20Activity&color=yellow" 
 alt="commit activity" >
      <a></a>
   <a href="https://github.com/Lennolium/simple-useragent/releases" > 
-    <img src="https://img.shields.io/badge/Version-0.1.4-brightgreen" 
+    <img src="https://img.shields.io/badge/Version-0.1.5-brightgreen" 
 alt="stable version" >
      <br>
   <a href="https://github.com/Lennolium/simple-useragent/issues" > 
     <img src="https://img.shields.io/github/issues-raw/Lennolium/simple-useragent?label=Open%20Issues&color=critical" alt="open issues" >
   <a href="https://github.com/Lennolium/simple-useragent/issues?q=is%3Aissue+is%3Aclosed" > 
     <img src="https://img.shields.io/github/issues-closed-raw/Lennolium/simple-useragent?label=Closed%20Issues&color=inactive" alt="closed issues" > 
      <a href="https://pepy.tech/project/simple-useragent" > 
@@ -132,89 +96,89 @@
 
 <!--- Installation -->
 
 ## Installation
 
 Just install the package from [PyPi](https://pypi.org/project/simple-useragent/) using pip:
 
-   ```bash
-    pip install simple-useragent
-   ```
+```bash
+pip install simple-useragent
+```
 
 &nbsp;
 
 <!--- Usage -->
 
 ## Usage
 
 #### Quickstart
 
 Just import the package and use the convenience functions. For more advanced usage, you can initialize the class to set custom settings.
 
-   ```python
-    import simple_useragent as sua
+```python
+import simple_useragent as sua
+
+sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agents (attributes explained below).
+# [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+
+sua.get_list(shuffle=True, force_cached=True)  # Random list of available desktop user agents strings.
+# ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
 
-    sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agents (attributes explained below).
-    # [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-    
-    sua.get_list(shuffle=True, force_cached=True)  # Random list of available desktop user agents strings.
-    # ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
-    
-    sua.get_dict()  # Dictionary with all desktop and mobile user agents.
-    # {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
-   ```
+sua.get_dict()  # Dictionary with all desktop and mobile user agents.
+# {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
+```
 &nbsp;
 
 #### Advanced Usage
 
 Import the package and initialize the UserAgents class to set custom settings (optional, see [Settings and Parameters](#settings-and-parameters) for details).
-   ```python
-    import simple_useragent as sua
+```python
+import simple_useragent as sua
 
-    simple_ua = sua.UserAgents(max_retries=3, timeout=5, cache_duration=86400, cache_location='example/path/to/folder')
-   ```
+simple_ua = sua.UserAgents(max_retries=3, timeout=5, cache_duration=86400, cache_location='example/path/to/folder')
+```
 &nbsp;
 
 Fetching User Agents.
-   ```python
-    # Fetch a specified number of random mobile user agent instances (with settings from the class above).
-    simple_ua.get(num=2, shuffle=True, mobile=True)
-    # [UserAgent('Mozilla/5.0 (iPhone ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-   ```  
+```python
+# Fetch a specified number of random mobile user agent instances (with settings from the class above).
+simple_ua.get(num=2, shuffle=True, mobile=True)
+# [UserAgent('Mozilla/5.0 (iPhone ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+```  
 &nbsp;
 
 You can also use the convenience functions to get user agents without initializing the class.
-   ```python
-    sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agent (attributes explained below).
-    # [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
-    
-    sua.get_list(force_cached=True)  # List of all available desktop user agents as strings.
-    # ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
-    
-    sua.get_dict()  # Dictionary with all desktop and mobile user agents.
-    # {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
-   ```
+```python
+sua.get(num=2, mobile=True)  # List of the 2 most common mobile user agent (attributes explained below).
+# [UserAgent('Mozilla/5.0 (Android ...'), UserAgent('Mozilla/5.0 (iPhone; ...')]
+
+sua.get_list(force_cached=True)  # List of all available desktop user agents as strings.
+# ['Mozilla/5.0 ...', 'Mozilla/5.0 (iPhone ...', 'Mozilla/5.0 (iPhone ...', ...]
+
+sua.get_dict()  # Dictionary with all desktop and mobile user agents.
+# {'desktop': ['Mozilla/5.0 ...', ...] 'mobile': ['Mozilla/5.0 (iPhone ...', ...]}
+```
 &nbsp;
 
 The instance offers attributes for the user agent properties.
-   ```python
-    # Parse a custom string directly to the UserAgent class and access its attributes.
-    obj = sua.parse('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36')
-    obj.string  # 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit ...'
-    obj.browser  # 'Chrome', 'Firefox', 'Safari', 'Edge', 'IE', 'Opera', 'Whale', 'QQ Browser', 'Samsung Browser', 'Other'
-    obj.browser_version  # '110', '109', '537', ...
-    obj.browser_version_minor  # '0', '1', '36', ...
-
-    # You can also access the attributes with square brackets.
-    obj = sua.get(num=1, shuffle=True)[0]
-    obj['os']  # 'Windows', 'macOS', 'Linux', 'Android', 'iOS', 'Other'
-    obj['os_version']  # '10', '7', '11', '14', ...
-    obj['os_version_minor']  # '0', '1', '2', ...
-    obj['mobile']  # True / False
-   ```
+```python
+# Parse a custom string directly to the UserAgent class and access its attributes.
+obj = sua.parse('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/110.0.0.0 Safari/537.36')
+obj.string  # 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit ...'
+obj.browser  # 'Chrome', 'Firefox', 'Safari', 'Edge', 'IE', 'Opera', 'Whale', 'QQ Browser', 'Samsung Browser', 'Other'
+obj.browser_version  # '110', '109', '537', ...
+obj.browser_version_minor  # '0', '1', '36', ...
+
+# You can also access the attributes with square brackets.
+obj = sua.get(num=1, shuffle=True)[0]
+obj['os']  # 'Windows', 'macOS', 'Linux', 'Android', 'iOS', 'Other'
+obj['os_version']  # '10', '7', '11', '14', ...
+obj['os_version_minor']  # '0', '1', '2', ...
+obj['mobile']  # True / False
+```
 &nbsp;
 
 #### Settings and Parameters
 
 The functions can take the following parameters:
 
 - __num:__ The number of user agents to fetch (default: _None_ = gets you all user agents available).
```

#### html2text {}

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1 Name: simple-useragent Version: 0.1.4 Summary: Seamlessly
-fetch authentic and current user agents with ease Home-page: https://
-github.com/Lennolium/simple-useragent Author: Lennart Haack Author-email:
-info@lennolium.dev License: GPL-3.0 Project-URL: Bug Tracker, https://
-github.com/Lennolium/simple-useragent/issues Project-URL: Source, https://
-github.com/Lennolium/simple-useragent Project-URL: Download, https://
-github.com/Lennolium/simple-useragent/releases/latest Project-URL:
-Documentation, https://github.com/Lennolium/simple-useragent/README.md
-Platform: any Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Utilities Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
-Only Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Operating System :: OS Independent Classifier: Operating
-System :: POSIX :: Linux Classifier: Operating System :: Unix Classifier:
-Operating System :: MacOS Classifier: Operating System :: Microsoft :: Windows
-Classifier: Natural Language :: English Classifier: Intended Audience ::
-Developers Classifier: Intended Audience :: Science/Research Requires-Python:
->=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: beautifulsoup4==4.12.3 Requires-Dist: platformdirs==4.2.0 Requires-Dist:
-requests==2.31.0 Requires-Dist: ua-parser==0.18.0
                              [Application Banner]
 
                                 _[_l_a_s_t_ _u_p_d_a_t_e_d_]
                                 _[_c_o_d_e_ _q_u_a_l_i_t_y_]
                                _[_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]
                                _[_s_t_a_b_l_e_ _v_e_r_s_i_o_n_]
                                  _[_o_p_e_n_ _i_s_s_u_e_s_]
```

