# Comparing `tmp/dazbo_commons-0.1.2.tar.gz` & `tmp/dazbo_commons-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dazbo_commons-0.1.2.tar", last modified: Sun Apr 28 15:41:01 2024, max compression
+gzip compressed data, was "dazbo_commons-0.1.3.tar", last modified: Sun Apr 28 22:24:44 2024, max compression
```

## Comparing `dazbo_commons-0.1.2.tar` & `dazbo_commons-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.486826 dazbo_commons-0.1.2/
--rw-rw-rw-   0        0        0     1099 2024-04-28 15:08:13.000000 dazbo_commons-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      782 2024-04-28 15:41:01.485826 dazbo_commons-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2619 2024-04-28 15:09:58.000000 dazbo_commons-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 15:41:01.486826 dazbo_commons-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      981 2024-04-28 15:39:58.000000 dazbo_commons-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.466828 dazbo_commons-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.473827 dazbo_commons-0.1.2/src/dazbo_commons/
--rw-rw-rw-   0        0        0      210 2024-04-28 15:08:13.000000 dazbo_commons-0.1.2/src/dazbo_commons/__init__.py
--rw-rw-rw-   0        0        0     4272 2024-04-28 15:08:13.000000 dazbo_commons-0.1.2/src/dazbo_commons/colored_logging.py
-drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.484826 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/
--rw-rw-rw-   0        0        0      782 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-28 15:41:01.000000 dazbo_commons-0.1.2/src/dazbo_commons.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 15:41:01.482828 dazbo_commons-0.1.2/tests/
--rw-rw-rw-   0        0        0     2916 2024-04-28 15:08:13.000000 dazbo_commons-0.1.2/tests/test_colored_logging.py
+drwxrwxrwx   0        0        0        0 2024-04-28 22:24:44.281390 dazbo_commons-0.1.3/
+-rw-rw-rw-   0        0        0     1078 2023-08-13 12:35:48.000000 dazbo_commons-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     4655 2024-04-28 22:24:44.279389 dazbo_commons-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2503 2024-04-28 21:50:38.000000 dazbo_commons-0.1.3/README.md
+-rw-rw-rw-   0        0        0      913 2024-04-28 22:23:58.000000 dazbo_commons-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 22:24:44.281896 dazbo_commons-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 22:24:44.245800 dazbo_commons-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-28 22:24:44.257481 dazbo_commons-0.1.3/src/dazbo_commons/
+-rw-rw-rw-   0        0        0      210 2024-04-28 13:46:13.000000 dazbo_commons-0.1.3/src/dazbo_commons/__init__.py
+-rw-rw-rw-   0        0        0     4272 2024-04-28 13:46:01.000000 dazbo_commons-0.1.3/src/dazbo_commons/colored_logging.py
+drwxrwxrwx   0        0        0        0 2024-04-28 22:24:44.275449 dazbo_commons-0.1.3/src/dazbo_commons.egg-info/
+-rw-rw-rw-   0        0        0     4655 2024-04-28 22:24:44.000000 dazbo_commons-0.1.3/src/dazbo_commons.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2024-04-28 22:24:44.000000 dazbo_commons-0.1.3/src/dazbo_commons.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 22:24:44.000000 dazbo_commons-0.1.3/src/dazbo_commons.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-28 22:24:44.000000 dazbo_commons-0.1.3/src/dazbo_commons.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-28 22:24:44.000000 dazbo_commons-0.1.3/src/dazbo_commons.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 22:24:44.271760 dazbo_commons-0.1.3/tests/
+-rw-rw-rw-   0        0        0     2916 2024-04-28 14:05:12.000000 dazbo_commons-0.1.3/tests/test_colored_logging.py
```

### Comparing `dazbo_commons-0.1.2/LICENSE` & `dazbo_commons-0.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Derailed-Dash (Dazbo)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Derailed-Dash (Dazbo)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `dazbo_commons-0.1.2/README.md` & `dazbo_commons-0.1.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-# Dazbo Commons
-
-## Table of Contents
-
-- [Overview](#overview)
-- [To Install and Use](#to-install-and-use)
-- [Coloured Logging Module](#coloured-logging-module)
-- [To Build From Package Source](#to-build-from-package-source)
-
-## Overview
-
-A reusable utility library.
-
-```text
-dazbo-commons/
-│
-├── src/
-│   └── dazbo_commons/
-│       ├── __init__.py
-│       └── colored_logging.py
-│
-├── tests/
-│   ├── __init__.py
-│   └── test_colored_logging.py
-│
-├── README.md
-├── setup.py
-├── setup.cfg
-├── LICENSE
-└── requirements.txt
-```
-
-## To Install and Use
-
-You can simply install the package from [PyPi](https://pypi.org/project/dazbo-commons/). There's no need to clone this repo.
-
-```bash
-pip install dazbo-commons
-```
-
-Then, in your Python code, include this `import`:
-
-```python
-import dazbo_commons as dc
-```
-
-## Coloured Logging Module
-
-This module provides a function to retrieve a logger that logs to the console, with colour.
-
-Example:
-
-```python
-import logging
-import dazbo_commons as dc
-
-logger_name = __name__ # or just pass in a str
-logger = dc.retrieve_console_logger(logger_name)
-logger.setLevel(logging.INFO) # Set threshold. E.g. INFO, DEBUG, or whatever
-
-logger.info("Some msg") # log at info level
-```
-
-## To Build From Package Source
-
-1. Create a Python virtual environment and activate. E.g.
-
-```bash
-python3 -m venv .dazbo-commons-env
-source .dazbo-commons-env/bin/activate
-```
-
-2. Install dependent packages:
-
-```bash
-py -m pip install -r requirements.txt
-```
-
-3. Run tests. E.g.
-
-```bash
-py -m unittest discover -v -s tests -p '*.py'
-```
-
-4. Install packages for actually creating the build. (If nto already included in `requirements.txt`):
-
-```bash
-py -m pip install twine
-py -m pip install --upgrade build
-```
-
-5. Make any required updates to the `setup.py` file. E.g. the `version` attribute.
-
-6. Build the package.
-
-```bash
-py -m build
-```
-
-This generates a `dist` folder in your project folder.
-
-7. Upload the package to [PyPi](https://pypi.org/). 
-
-Notes:
-- You'll need to create a free account, if you haven't done so already.
-- You'll need to generate an API token in _Account Settings_, for uploading to the API.
-- You may want to delete any previous builds.
-
-```bash
-py -m twine upload dist/*
-```
-
-You'll be prompted for your API token. In my experience, when doing this from a terminal inside VS Code, Ctrl-V doesn't work here. So I use Paste from the menu, and this works.
-
+# Dazbo Commons
+
+## Table of Contents
+
+- [Overview](#overview)
+- [To Install and Use](#to-install-and-use)
+- [Coloured Logging Module](#coloured-logging-module)
+- [To Build From Package Source](#to-build-from-package-source)
+
+## Overview
+
+A reusable utility library.
+
+```text
+dazbo-commons/
+│
+├── src/
+│   └── dazbo_commons/
+│       ├── __init__.py
+│       └── colored_logging.py
+│
+├── tests/
+│   └── test_colored_logging.py
+│
+├── .env
+├── .gitignore
+├── LICENSE
+├── README.md
+├── requirements.txt
+└── setup.py
+```
+
+## To Install and Use
+
+You can simply install the package from [PyPi](https://pypi.org/project/dazbo-commons/). There's no need to clone this repo.
+
+```bash
+pip install --upgrade dazbo-commons
+```
+
+Then, in your Python code, include this `import`:
+
+```python
+import dazbo_commons as dc
+```
+
+## Coloured Logging Module
+
+This module provides a function to retrieve a logger that logs to the console, with colour.
+
+Example:
+
+```python
+import logging
+import dazbo_commons as dc
+
+logger_name = __name__ # or just pass in a str
+logger = dc.retrieve_console_logger(logger_name)
+logger.setLevel(logging.INFO) # Set threshold. E.g. INFO, DEBUG, or whatever
+
+logger.info("Some msg") # log at info level
+```
+
+## To Build From Package Source
+
+1. Create a Python virtual environment and activate. E.g.
+
+```bash
+python3 -m venv .dazbo-commons-env
+source .dazbo-commons-env/bin/activate
+```
+
+2. Install dependent packages:
+
+```bash
+py -m pip install -r requirements.txt
+```
+
+3. Run tests. E.g.
+
+```bash
+py -m unittest discover -v -s tests -p '*.py'
+```
+
+4. Install packages for actually creating the build. (If nto already included in `requirements.txt`):
+
+```bash
+py -m pip install twine
+py -m pip install --upgrade build
+```
+
+5. Make any required updates to the `setup.py` file. E.g. the `version` attribute.
+
+6. Build the package.
+
+```bash
+py -m build
+```
+
+This generates a `dist` folder in your project folder.
+
+7. Upload the package to [PyPi](https://pypi.org/). 
+
+Notes:
+- You'll need to create a free account, if you haven't done so already.
+- You'll need to generate an API token in _Account Settings_, for uploading to the API.
+- You may want to delete any previous builds.
+
+```bash
+py -m twine upload dist/*
+```
+
+You'll be prompted for your API token. In my experience, when doing this from a terminal inside VS Code, Ctrl-V doesn't work here. So I use Paste from the menu, and this works.
+
 And we're done!
```

### Comparing `dazbo_commons-0.1.2/src/dazbo_commons/colored_logging.py` & `dazbo_commons-0.1.3/src/dazbo_commons/colored_logging.py`

 * *Files identical despite different names*

### Comparing `dazbo_commons-0.1.2/tests/test_colored_logging.py` & `dazbo_commons-0.1.3/tests/test_colored_logging.py`

 * *Files identical despite different names*

