# Comparing `tmp/sphinxcontrib-budoux-0.1.5.tar.gz` & `tmp/sphinxcontrib_budoux-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-budoux-0.1.5.tar", max compression
+gzip compressed data, was "sphinxcontrib_budoux-0.1.6.tar", max compression
```

## Comparing `sphinxcontrib-budoux-0.1.5.tar` & `sphinxcontrib_budoux-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    11358 2022-07-19 13:46:21.811766 sphinxcontrib-budoux-0.1.5/LICENSE
--rw-r--r--   0        0        0     1310 2022-07-19 13:46:21.811766 sphinxcontrib-budoux-0.1.5/README.rst
--rw-r--r--   0        0        0     1374 2022-07-19 13:46:21.811766 sphinxcontrib-budoux-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1592 2022-07-19 13:46:21.811766 sphinxcontrib-budoux-0.1.5/sphinxcontrib/budoux.py
--rw-r--r--   0        0        0     2054 2022-07-19 13:46:36.370198 sphinxcontrib-budoux-0.1.5/setup.py
--rw-r--r--   0        0        0     2488 2022-07-19 13:46:36.370522 sphinxcontrib-budoux-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-29 12:54:38.170086 sphinxcontrib_budoux-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1358 2024-04-29 12:54:38.170086 sphinxcontrib_budoux-0.1.6/README.rst
+-rw-r--r--   0        0        0     1482 2024-04-29 12:54:38.170086 sphinxcontrib_budoux-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1592 2024-04-29 12:54:38.170086 sphinxcontrib_budoux-0.1.6/sphinxcontrib/budoux.py
+-rw-r--r--   0        0        0     2638 1970-01-01 00:00:00.000000 sphinxcontrib_budoux-0.1.6/PKG-INFO
```

### Comparing `sphinxcontrib-budoux-0.1.5/LICENSE` & `sphinxcontrib_budoux-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-budoux-0.1.5/README.rst` & `sphinxcontrib_budoux-0.1.6/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -58,8 +58,8 @@
 Main targets for edit are heading text, not but contents of paragraph.
 
 If you set ``p``, ``li`` and others into `budoux_targets``, this may not work correctly that you think.
 
 Example
 =======
 
-See `doc <doc/>`_ (written by Japanese).
+See `doc <https://attakei-lab.github.io/sphinxcontrib-budoux/>`__ (written by Japanese).
```

### Comparing `sphinxcontrib-budoux-0.1.5/pyproject.toml` & `sphinxcontrib_budoux-0.1.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-budoux"
-version = "0.1.5"
+version = "0.1.6"
 description = "This is Sphinx extension to break line of heading texts by BudouX."
 license = "Apache-2.0"
 authors = ["Kazuya Takei <myself@attakei.net>"]
 readme = "README.rst"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Sphinx",
@@ -15,25 +15,27 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Software Development",
     "Topic :: Software Development :: Documentation",
     "Topic :: Text Processing :: Markup :: HTML",
 ]
 packages = [
     { include = "sphinxcontrib" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7 | ^3.8 | ^3.9 | ^3.10"
+python = "^3.7 | ^3.8 | ^3.9 | ^3.10 | ^3.11 | ^3.12"
 Sphinx = "*"
 BudouX = "*"
 beautifulsoup4 = "*"
 
 [tool.poetry.dev-dependencies]
 sphinx-rtd-theme = "^1.0.0"
 pytest = "^7.1.2"
```

### Comparing `sphinxcontrib-budoux-0.1.5/sphinxcontrib/budoux.py` & `sphinxcontrib_budoux-0.1.6/sphinxcontrib/budoux.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-budoux-0.1.5/PKG-INFO` & `sphinxcontrib_budoux-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-budoux
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is Sphinx extension to break line of heading texts by BudouX.
 License: Apache-2.0
 Author: Kazuya Takei
 Author-email: myself@attakei.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Requires-Dist: BudouX
 Requires-Dist: Sphinx
 Requires-Dist: beautifulsoup4
@@ -88,9 +90,9 @@
 Main targets for edit are heading text, not but contents of paragraph.
 
 If you set ``p``, ``li`` and others into `budoux_targets``, this may not work correctly that you think.
 
 Example
 =======
 
-See `doc <doc/>`_ (written by Japanese).
+See `doc <https://attakei-lab.github.io/sphinxcontrib-budoux/>`__ (written by Japanese).
```

