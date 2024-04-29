# Comparing `tmp/ood_detectors-0.0.3.tar.gz` & `tmp/ood_detectors-0.0.4.tar.gz`

## Comparing `ood_detectors-0.0.3.tar` & `ood_detectors-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/docki.yaml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/requirements.txt
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/requirements_dev.txt
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/__init__.py
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/ddm_likelihood.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/eval_utils.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/losses.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/ood_utils.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/ops_utils.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/plot_utils.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/residual.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/train.py
--rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/src/ood_detectors/models/mlp.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/tests/init_test.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/LICENSE
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/README.md
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 ood_detectors-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/docki.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/requirements_dev.txt
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/__init__.py
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/ddm_likelihood.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/eval_utils.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/losses.py
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/ood_utils.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/ops_utils.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/plot_utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/residual.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/train.py
+-rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/src/ood_detectors/models/mlp.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/tests/init_test.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/LICENSE
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/README.md
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ood_detectors-0.0.4/PKG-INFO
```

### Comparing `ood_detectors-0.0.3/docki.yaml` & `ood_detectors-0.0.4/docki.yaml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/.github/workflows/publish.yml` & `ood_detectors-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/ddm_likelihood.py` & `ood_detectors-0.0.4/src/ood_detectors/ddm_likelihood.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/eval_utils.py` & `ood_detectors-0.0.4/src/ood_detectors/eval_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/losses.py` & `ood_detectors-0.0.4/src/ood_detectors/losses.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/ood_utils.py` & `ood_detectors-0.0.4/src/ood_detectors/ood_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/ops_utils.py` & `ood_detectors-0.0.4/src/ood_detectors/ops_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/plot_utils.py` & `ood_detectors-0.0.4/src/ood_detectors/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/residual.py` & `ood_detectors-0.0.4/src/ood_detectors/residual.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/train.py` & `ood_detectors-0.0.4/src/ood_detectors/train.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/src/ood_detectors/models/mlp.py` & `ood_detectors-0.0.4/src/ood_detectors/models/mlp.py`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/LICENSE` & `ood_detectors-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/README.md` & `ood_detectors-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/pyproject.toml` & `ood_detectors-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ood_detectors-0.0.3/PKG-INFO` & `ood_detectors-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ood_detectors
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/Arty-Facts/ood_detectors#readme
 Project-URL: Issues, https://github.com/Arty-Facts/ood_detectors/issues
 Project-URL: Source, https://github.com/Arty-Facts/ood_detectors
 Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>, Yifan Ding <yifan.ding@liu.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: docker
 Requires-Dist: einops
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
-Requires-Dist: spacy[cuda11x]
+Requires-Dist: seaborn
 Requires-Dist: torch
 Requires-Dist: torchdiffeq
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # ood_detectors
```

