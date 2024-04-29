# Comparing `tmp/ood_detectors-0.0.1.tar.gz` & `tmp/ood_detectors-0.0.2.tar.gz`

## Comparing `ood_detectors-0.0.1.tar` & `ood_detectors-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,22 @@
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/src/ood_detectors/__about__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/src/ood_detectors/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/tests/init_test.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/LICENSE
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/README.md
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 ood_detectors-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/docki.yaml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/requirements_dev.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/__init__.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/ddm_likelihood.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/eval_utils.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/losses.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/ood_utils.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/ops_utils.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/plot_utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/residual.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/train.py
+-rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/src/ood_detectors/models/mlp.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/tests/init_test.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/LICENSE
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/README.md
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 ood_detectors-0.0.2/PKG-INFO
```

### Comparing `ood_detectors-0.0.1/.github/workflows/publish.yml` & `ood_detectors-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.1/LICENSE` & `ood_detectors-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.1/pyproject.toml` & `ood_detectors-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.1/PKG-INFO` & `ood_detectors-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ood_detectors
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/Arty-Facts/ood_detectors#readme
 Project-URL: Issues, https://github.com/Arty-Facts/ood_detectors/issues
 Project-URL: Source, https://github.com/Arty-Facts/ood_detectors
 Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>, Yifan Ding <yifan.ding@liu.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -15,28 +15,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-# inverters
+# ood_detectors
 
-[![PyPI - Version](https://img.shields.io/pypi/v/inverters.svg)](https://pypi.org/project/inverters)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/inverters.svg)](https://pypi.org/project/inverters)
+[![PyPI - Version](https://img.shields.io/pypi/v/ood_detectors.svg)](https://pypi.org/project/ood_detectors)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ood_detectors.svg)](https://pypi.org/project/ood_detectors)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
 
 ## Installation
 
 ```console
-pip install inverters
+pip install ood_detectors
 ```
 
 ## License
 
-`inverters` is distributed under the terms of the [apache-2.0](https://choosealicense.com/licenses/apache-2.0/) license.
+`ood_detectors` is distributed under the terms of the [apache-2.0](https://choosealicense.com/licenses/apache-2.0/) license.
```

