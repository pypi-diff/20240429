# Comparing `tmp/chart_review-1.0.0.tar.gz` & `tmp/chart_review-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chart_review-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "chart_review-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `chart_review-1.0.0.tar` & `chart_review-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0     1635 2024-01-18 20:53:34.070061 chart_review-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-10-11 13:26:00.032976 chart_review-1.0.0/LICENSE
--rw-r--r--   0        0        0     1451 2024-01-18 20:53:34.070061 chart_review-1.0.0/README.md
--rw-r--r--   0        0        0       61 2024-01-19 14:52:39.461991 chart_review-1.0.0/chart_review/__init__.py
--rw-r--r--   0        0        0     7643 2024-01-18 19:57:00.548786 chart_review-1.0.0/chart_review/agree.py
--rw-r--r--   0        0        0     2306 2024-01-18 19:57:00.548786 chart_review-1.0.0/chart_review/cli.py
--rw-r--r--   0        0        0     5888 2024-01-18 19:57:00.548786 chart_review-1.0.0/chart_review/cohort.py
--rw-r--r--   0        0        0        0 2023-10-17 15:04:22.584830 chart_review-1.0.0/chart_review/commands/__init__.py
--rw-r--r--   0        0        0     1880 2024-01-18 19:57:00.548786 chart_review-1.0.0/chart_review/commands/accuracy.py
--rw-r--r--   0        0        0     3901 2024-01-18 19:57:00.548786 chart_review-1.0.0/chart_review/common.py
--rw-r--r--   0        0        0     4055 2024-01-18 19:57:00.544787 chart_review-1.0.0/chart_review/config.py
--rw-r--r--   0        0        0     5001 2024-01-18 19:57:00.544787 chart_review-1.0.0/chart_review/external.py
--rw-r--r--   0        0        0      987 2023-11-14 14:33:28.318843 chart_review-1.0.0/chart_review/kappa.py
--rw-r--r--   0        0        0     5139 2024-01-12 20:08:39.785103 chart_review-1.0.0/chart_review/labelstudio.py
--rw-r--r--   0        0        0     4506 2024-01-18 19:57:00.544787 chart_review-1.0.0/chart_review/simplify.py
--rw-r--r--   0        0        0     3374 2024-01-18 19:57:00.544787 chart_review-1.0.0/chart_review/term_freq.py
--rw-r--r--   0        0        0     1179 2024-01-18 19:57:00.544787 chart_review-1.0.0/chart_review/types.py
--rw-r--r--   0        0        0      278 2024-01-18 20:53:34.070061 chart_review-1.0.0/docs/README.md
--rw-r--r--   0        0        0     1426 2024-01-18 20:53:34.070061 chart_review-1.0.0/docs/accuracy.md
--rw-r--r--   0        0        0     4469 2024-01-18 20:53:34.070061 chart_review-1.0.0/docs/config.md
--rw-r--r--   0        0        0     1753 2024-01-18 20:53:34.070061 chart_review-1.0.0/docs/index.md
--rw-r--r--   0        0        0      643 2024-01-18 20:53:34.070061 chart_review-1.0.0/docs/setup.md
--rw-r--r--   0        0        0     1169 2024-01-19 15:00:01.859643 chart_review-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-17 19:50:20.284880 chart_review-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      231 2023-12-28 20:12:31.083940 chart_review-1.0.0/tests/data/cold/config.yaml
--rw-r--r--   0        0        0     3519 2024-01-18 18:06:03.449172 chart_review-1.0.0/tests/data/cold/labelstudio-export.json
--rw-r--r--   0        0        0       93 2024-01-18 18:06:03.449172 chart_review-1.0.0/tests/data/external/config.yaml
--rw-r--r--   0        0        0      166 2024-01-18 18:06:03.449172 chart_review-1.0.0/tests/data/external/doc.csv
--rw-r--r--   0        0        0      176 2024-01-18 18:06:03.453172 chart_review-1.0.0/tests/data/external/enc.csv
--rw-r--r--   0        0        0     1215 2024-01-18 18:06:03.453172 chart_review-1.0.0/tests/data/external/labelstudio-export.json
--rw-r--r--   0        0        0       85 2024-01-18 18:06:03.453172 chart_review-1.0.0/tests/data/ignore/config.yaml
--rw-r--r--   0        0        0     2386 2024-01-18 18:06:03.453172 chart_review-1.0.0/tests/data/ignore/labelstudio-export.json
--rw-r--r--   0        0        0     1643 2024-01-18 19:57:00.544787 chart_review-1.0.0/tests/test_agree.py
--rw-r--r--   0        0        0     3734 2024-01-18 19:57:00.548786 chart_review-1.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     2698 2024-01-18 19:57:00.544787 chart_review-1.0.0/tests/test_config.py
--rw-r--r--   0        0        0     1757 2024-01-18 19:57:00.544787 chart_review-1.0.0/tests/test_external.py
--rw-r--r--   0        0        0     2361 2024-01-18 19:57:00.544787 chart_review-1.0.0/tests/test_simplify.py
--rw-r--r--   0        0        0      849 2024-01-18 19:57:00.544787 chart_review-1.0.0/tests/test_term_freq.py
--rw-r--r--   0        0        0     2397 1970-01-01 00:00:00.000000 chart_review-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1635 2024-04-29 17:36:40.289858 chart_review-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2024-04-29 17:36:40.289858 chart_review-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1504 2024-04-29 17:36:40.289858 chart_review-1.1.0/README.md
+-rw-r--r--   0        0        0       61 2024-04-29 17:36:40.289858 chart_review-1.1.0/chart_review/__init__.py
+-rw-r--r--   0        0        0     8468 2024-04-29 17:36:40.289858 chart_review-1.1.0/chart_review/agree.py
+-rw-r--r--   0        0        0     2306 2024-04-29 17:36:40.289858 chart_review-1.1.0/chart_review/cli.py
+-rw-r--r--   0        0        0     5888 2024-04-29 17:36:40.289858 chart_review-1.1.0/chart_review/cohort.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:36:40.289858 chart_review-1.1.0/chart_review/commands/__init__.py
+-rw-r--r--   0        0        0     1880 2024-04-29 17:36:40.293858 chart_review-1.1.0/chart_review/commands/accuracy.py
+-rw-r--r--   0        0        0     3902 2024-04-29 17:36:40.293858 chart_review-1.1.0/chart_review/common.py
+-rw-r--r--   0        0        0     4055 2024-04-29 17:36:40.293858 chart_review-1.1.0/chart_review/config.py
+-rw-r--r--   0        0        0     5001 2024-04-29 17:36:40.293858 chart_review-1.1.0/chart_review/external.py
+-rw-r--r--   0        0        0     5139 2024-04-29 17:36:40.293858 chart_review-1.1.0/chart_review/labelstudio.py
+-rw-r--r--   0        0        0     4506 2024-04-29 17:36:40.293858 chart_review-1.1.0/chart_review/simplify.py
+-rw-r--r--   0        0        0     3374 2024-04-29 17:36:40.293858 chart_review-1.1.0/chart_review/term_freq.py
+-rw-r--r--   0        0        0     1179 2024-04-29 17:36:40.293858 chart_review-1.1.0/chart_review/types.py
+-rw-r--r--   0        0        0      278 2024-04-29 17:36:40.293858 chart_review-1.1.0/docs/README.md
+-rw-r--r--   0        0        0     1353 2024-04-29 17:36:40.293858 chart_review-1.1.0/docs/accuracy.md
+-rw-r--r--   0        0        0     4469 2024-04-29 17:36:40.293858 chart_review-1.1.0/docs/config.md
+-rw-r--r--   0        0        0     1752 2024-04-29 17:36:40.293858 chart_review-1.1.0/docs/index.md
+-rw-r--r--   0        0        0      643 2024-04-29 17:36:40.293858 chart_review-1.1.0/docs/setup.md
+-rw-r--r--   0        0        0     1209 2024-04-29 17:36:40.293858 chart_review-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      231 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/data/cold/config.yaml
+-rw-r--r--   0        0        0     3519 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/data/cold/labelstudio-export.json
+-rw-r--r--   0        0        0       93 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/data/external/config.yaml
+-rw-r--r--   0        0        0      166 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/data/external/doc.csv
+-rw-r--r--   0        0        0      176 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/data/external/enc.csv
+-rw-r--r--   0        0        0     1215 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/data/external/labelstudio-export.json
+-rw-r--r--   0        0        0       85 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/data/ignore/config.yaml
+-rw-r--r--   0        0        0     2386 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/data/ignore/labelstudio-export.json
+-rw-r--r--   0        0        0     3249 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/test_agree.py
+-rw-r--r--   0        0        0     3904 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2698 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     1757 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/test_external.py
+-rw-r--r--   0        0        0     2361 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/test_simplify.py
+-rw-r--r--   0        0        0      849 2024-04-29 17:36:40.293858 chart_review-1.1.0/tests/test_term_freq.py
+-rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 chart_review-1.1.0/PKG-INFO
```

### Comparing `chart_review-1.0.0/CONTRIBUTING.md` & `chart_review-1.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/LICENSE` & `chart_review-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/README.md` & `chart_review-1.1.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Chart Review
 
-**Measure agreement between chart annotators.**
+**Measure agreement between chart reviewers.**
 
 Whether your chart annotations come from humans, machine-learning, or coded data like ICD-10,
 `chart-review` can compare them to reveal interesting statistics like:
 
 **Accuracy**
 * F1-score ([agreement](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1090460/))
 * [Sensitivity and Specificity](https://en.wikipedia.org/wiki/Sensitivity_and_specificity)
@@ -24,21 +24,21 @@
 
 ## Example
 
 ```shell
 $ ls
 config.yaml  labelstudio-export.json
 
-$ chart-review accuracy jane john
-accuracy-jane-john:
-F1     Sens  Spec  PPV  NPV  TP  FN  TN  FP  Label
-0.889  0.8   1.0   1.0  0.5  4   1   1   0   *
-1.0    1.0   1.0   1.0  1.0  1   0   1   0   Cough
-0      0     0     0    0    2   0   0   0   Fatigue
-0      0     0     0    0    1   1   0   0   Headache
+$ chart-review accuracy jill jane
+accuracy-jill-jane:
+F1     Sens  Spec  PPV  NPV   Kappa  TP  FN  TN  FP  Label   
+0.667  0.75  0.6   0.6  0.75  0.341  3   1   3   2   *       
+0.667  0.5   1.0   1.0  0.5   0.4    1   1   1   0   Cough   
+1.0    1.0   1.0   1.0  1.0   1.0    2   0   1   0   Fatigue 
+0      0     0     0    0     0      0   0   1   2   Headache
 ```
 
 ## Contributing
 
 We love 💖 contributions!
 
 If you have a good suggestion 💡 or found a bug 🐛,
```

### Comparing `chart_review-1.0.0/chart_review/agree.py` & `chart_review-1.1.0/chart_review/agree.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,48 +82,76 @@
     """
     added = {}
     for header in ["TP", "FP", "FN", "TN"]:
         added[header] = first[header] + second[header]
     return added
 
 
+def score_kappa(matrix: dict) -> float:
+    """
+    Computes Cohen kappa for pair-wise annotators.
+    https://en.wikipedia.org/wiki/Cohen%27s_kappa
+
+    :param matrix: confusion matrix with TN/TP/FN/FP values
+    :return: Cohen kappa statistic
+    """
+    tp = len(matrix["TP"])  # true positive
+    tn = len(matrix["TN"])  # true negative
+    fp = len(matrix["FP"])  # false positive
+    fn = len(matrix["FN"])  # false negative
+    total = tp + tn + fp + fn
+
+    # observed agreement A (Po)
+    observed = (tp + tn) / total
+
+    # expected agreement E (Pe)
+    expected_pos = ((tp + fp) / total) * ((tp + fn) / total)
+    expected_neg = ((tn + fp) / total) * ((tn + fn) / total)
+    expected = expected_pos + expected_neg
+
+    return (observed - expected) / (1 - expected)
+
+
 def score_matrix(matrix: dict, sig_digits=3) -> dict:
     """
-    Score F1 measure with precision (PPV) and recall (sensitivity).
+    Score F1 and Kappa measures with precision (PPV) and recall (sensitivity).
     F1 deliberately ignores "True Negatives" because TN inflates scoring (AUROC)
     @return: dict with keys {'f1', 'precision', 'recall'} vals are %score
     """
-    true_pos = matrix["TP"]
-    true_neg = matrix["TN"]
-    false_pos = matrix["FP"]
-    false_neg = matrix["FN"]
+    true_pos = len(matrix["TP"])
+    true_neg = len(matrix["TN"])
+    false_pos = len(matrix["FP"])
+    false_neg = len(matrix["FN"])
 
-    if 0 == len(true_pos) or 0 == len(true_neg):
+    if 0 == true_pos or 0 == true_neg:
         sens = 0
         spec = 0
         ppv = 0
         npv = 0
         f1 = 0
+        kappa = 0
     else:
-        sens = len(true_pos) / (len(true_pos) + len(false_neg))
-        spec = len(true_neg) / (len(true_neg) + len(false_pos))
-        ppv = len(true_pos) / (len(true_pos) + len(false_pos))
-        npv = len(true_neg) / (len(true_neg) + len(false_neg))
+        sens = true_pos / (true_pos + false_neg)
+        spec = true_neg / (true_neg + false_pos)
+        ppv = true_pos / (true_pos + false_pos)
+        npv = true_neg / (true_neg + false_neg)
         f1 = (2 * ppv * sens) / (ppv + sens)
+        kappa = score_kappa(matrix)
 
     return {
         "F1": round(f1, sig_digits),
         "Sens": round(sens, sig_digits),
         "Spec": round(spec, sig_digits),
         "PPV": round(ppv, sig_digits),
         "NPV": round(npv, sig_digits),
-        "TP": len(true_pos),
-        "FP": len(false_pos),
-        "FN": len(false_neg),
-        "TN": len(true_neg),
+        "Kappa": round(kappa, sig_digits),
+        "TP": true_pos,
+        "FP": false_pos,
+        "FN": false_neg,
+        "TN": true_neg,
     }
 
 
 def avg_scores(first: dict, second: dict, sig_digits=3) -> dict:
     merged = {}
     for header in csv_header():
         added = first[header] + second[header]
@@ -168,15 +196,15 @@
 def csv_header(pick_label=False, as_string=False):
     """
     Table Header
     F1, PPV (precision), Recall (sensitivity), True Pos, False Pos, False Neg
     :param pick_label: default= None
     :return: header
     """
-    as_list = ["F1", "Sens", "Spec", "PPV", "NPV", "TP", "FN", "TN", "FP"]
+    as_list = ["F1", "Sens", "Spec", "PPV", "NPV", "Kappa", "TP", "FN", "TN", "FP"]
 
     if not as_string:
         return as_list
 
     header = as_list
     header.append(pick_label if pick_label else "Label")
     return "\t".join(header)
```

### Comparing `chart_review-1.0.0/chart_review/cli.py` & `chart_review-1.1.0/chart_review/cli.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/chart_review/cohort.py` & `chart_review-1.1.0/chart_review/cohort.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/chart_review/commands/accuracy.py` & `chart_review-1.1.0/chart_review/commands/accuracy.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/chart_review/common.py` & `chart_review-1.1.0/chart_review/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility methods"""
+
 from enum import Enum, EnumMeta
 from typing import Optional, Union
 from collections.abc import Iterable
 import logging
 import json
 
 ###############################################################################
```

### Comparing `chart_review-1.0.0/chart_review/config.py` & `chart_review-1.1.0/chart_review/config.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/chart_review/external.py` & `chart_review-1.1.0/chart_review/external.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/chart_review/labelstudio.py` & `chart_review-1.1.0/chart_review/labelstudio.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/chart_review/simplify.py` & `chart_review-1.1.0/chart_review/simplify.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/chart_review/term_freq.py` & `chart_review-1.1.0/chart_review/term_freq.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/chart_review/types.py` & `chart_review-1.1.0/chart_review/types.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/docs/accuracy.md` & `chart_review-1.1.0/docs/accuracy.md`

 * *Files 20% similar despite different names*

```diff
@@ -13,22 +13,21 @@
 
 Provide two annotator names (the first name will be considered the ground truth) and
 your accuracy scores will be printed to the console.
 
 ## Example
 
 ```shell
-$ chart-review accuracy jane john
-accuracy-jane-john:
-F1     Sens   Spec   PPV    NPV    TP  FN  TN  FP  Label           
-0.929  0.958  0.908  0.901  0.961  91  4   99  10  *               
-0.895  0.895  0.938  0.895  0.938  17  2   30  2   cough     
-0.815  0.917  0.897  0.733  0.972  11  1   35  4   fever  
-0.959  1.0    0.812  0.921  1.0    35  0   13  3   headache   
-0.966  0.966  0.955  0.966  0.955  28  1   21  1   stuffy-nose
+$ chart-review accuracy jill jane
+accuracy-jill-jane:
+F1     Sens  Spec  PPV  NPV   Kappa  TP  FN  TN  FP  Label   
+0.667  0.75  0.6   0.6  0.75  0.341  3   1   3   2   *       
+0.667  0.5   1.0   1.0  0.5   0.4    1   1   1   0   Cough   
+1.0    1.0   1.0   1.0  1.0   1.0    2   0   1   0   Fatigue 
+0      0     0     0    0     0      0   0   1   2   Headache
 ```
 
 ## Options
 
 ### `--config=PATH`
 
 Use this to point to a secondary (non-default) config file.
```

### Comparing `chart_review-1.0.0/docs/config.md` & `chart_review-1.1.0/docs/config.md`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/docs/index.md` & `chart_review-1.1.0/docs/index.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 has_children: true
 # audience: non-programmers new to this project
 # type: explanation
 ---
 
 # Chart Review
 
-**Measure agreement between chart annotators.**
+**Measure agreement between chart reviewers.**
 
 Whether your chart annotations come from humans, machine-learning, or coded data like ICD-10,
 Chart Review can compare them to reveal interesting statistics like:
 
 **Accuracy**
 * F1-score ([agreement](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1090460/))
 * [Sensitivity and Specificity](https://en.wikipedia.org/wiki/Sensitivity_and_specificity)
```

### Comparing `chart_review-1.0.0/docs/setup.md` & `chart_review-1.1.0/docs/setup.md`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/tests/data/cold/labelstudio-export.json` & `chart_review-1.1.0/tests/data/cold/labelstudio-export.json`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/tests/data/external/labelstudio-export.json` & `chart_review-1.1.0/tests/data/external/labelstudio-export.json`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/tests/data/ignore/labelstudio-export.json` & `chart_review-1.1.0/tests/data/ignore/labelstudio-export.json`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/tests/test_cli.py` & `chart_review-1.1.0/tests/test_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,62 +26,66 @@
             self.assertEqual(
                 {
                     "F1": 0.667,
                     "Sens": 0.75,
                     "Spec": 0.6,
                     "PPV": 0.6,
                     "NPV": 0.75,
+                    "Kappa": 0.341,
                     "TP": 3,
                     "FN": 1,
                     "TN": 3,
                     "FP": 2,
                     "Cough": {
                         "F1": 0.667,
                         "FN": 1,
                         "FP": 0,
                         "NPV": 0.5,
                         "PPV": 1.0,
                         "Sens": 0.5,
                         "Spec": 1.0,
                         "TN": 1,
                         "TP": 1,
+                        "Kappa": 0.4,
                     },
                     "Fatigue": {
                         "F1": 1.0,
                         "FN": 0,
                         "FP": 0,
                         "NPV": 1.0,
                         "PPV": 1.0,
                         "Sens": 1.0,
                         "Spec": 1.0,
                         "TN": 1,
                         "TP": 2,
+                        "Kappa": 1.0,
                     },
                     "Headache": {
                         "F1": 0,
                         "FN": 0,
                         "FP": 2,
                         "NPV": 0,
                         "PPV": 0,
                         "Sens": 0,
                         "Spec": 0,
                         "TN": 1,
                         "TP": 0,
+                        "Kappa": 0,
                     },
                 },
                 accuracy_json,
             )
 
             accuracy_csv = common.read_text(f"{tmpdir}/accuracy-jill-jane.csv")
             self.assertEqual(
-                """F1	Sens	Spec	PPV	NPV	TP	FN	TN	FP	Label
-0.667	0.75	0.6	0.6	0.75	3	1	3	2	*
-0.667	0.5	1.0	1.0	0.5	1	1	1	0	Cough
-1.0	1.0	1.0	1.0	1.0	2	0	1	0	Fatigue
-0	0	0	0	0	0	0	1	2	Headache
+                """F1	Sens	Spec	PPV	NPV	Kappa	TP	FN	TN	FP	Label
+0.667	0.75	0.6	0.6	0.75	0.341	3	1	3	2	*
+0.667	0.5	1.0	1.0	0.5	0.4	1	1	1	0	Cough
+1.0	1.0	1.0	1.0	1.0	1.0	2	0	1	0	Fatigue
+0	0	0	0	0	0	0	0	1	2	Headache
 """,
                 accuracy_csv,
             )
 
     def test_ignored_ids(self):
         with tempfile.TemporaryDirectory() as tmpdir:
             shutil.copytree(f"{DATA_DIR}/ignore", tmpdir, dirs_exist_ok=True)
```

### Comparing `chart_review-1.0.0/tests/test_config.py` & `chart_review-1.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/tests/test_external.py` & `chart_review-1.1.0/tests/test_external.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/tests/test_simplify.py` & `chart_review-1.1.0/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/tests/test_term_freq.py` & `chart_review-1.1.0/tests/test_term_freq.py`

 * *Files identical despite different names*

### Comparing `chart_review-1.0.0/PKG-INFO` & `chart_review-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: chart-review
-Version: 1.0.0
+Version: 1.1.0
 Summary: Medical Record Chart Review Calculator
 Requires-Python: >= 3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ctakesclient
 Requires-Dist: pyyaml >= 6
 Requires-Dist: rich
-Requires-Dist: black == 23.11.0 ; extra == "dev"
+Requires-Dist: bandit[toml] ; extra == "dev"
+Requires-Dist: black >= 24, < 25 ; extra == "dev"
+Requires-Dist: pycodestyle ; extra == "dev"
 Requires-Dist: pylint ; extra == "dev"
 Requires-Dist: ddt ; extra == "tests"
 Requires-Dist: pytest ; extra == "tests"
 Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/chart-review/
 Project-URL: Home, https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/
 Project-URL: Source, https://github.com/smart-on-fhir/chart-review
 Provides-Extra: dev
 Provides-Extra: tests
 
 # Chart Review
 
-**Measure agreement between chart annotators.**
+**Measure agreement between chart reviewers.**
 
 Whether your chart annotations come from humans, machine-learning, or coded data like ICD-10,
 `chart-review` can compare them to reveal interesting statistics like:
 
 **Accuracy**
 * F1-score ([agreement](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1090460/))
 * [Sensitivity and Specificity](https://en.wikipedia.org/wiki/Sensitivity_and_specificity)
@@ -47,21 +49,21 @@
 
 ## Example
 
 ```shell
 $ ls
 config.yaml  labelstudio-export.json
 
-$ chart-review accuracy jane john
-accuracy-jane-john:
-F1     Sens  Spec  PPV  NPV  TP  FN  TN  FP  Label
-0.889  0.8   1.0   1.0  0.5  4   1   1   0   *
-1.0    1.0   1.0   1.0  1.0  1   0   1   0   Cough
-0      0     0     0    0    2   0   0   0   Fatigue
-0      0     0     0    0    1   1   0   0   Headache
+$ chart-review accuracy jill jane
+accuracy-jill-jane:
+F1     Sens  Spec  PPV  NPV   Kappa  TP  FN  TN  FP  Label   
+0.667  0.75  0.6   0.6  0.75  0.341  3   1   3   2   *       
+0.667  0.5   1.0   1.0  0.5   0.4    1   1   1   0   Cough   
+1.0    1.0   1.0   1.0  1.0   1.0    2   0   1   0   Fatigue 
+0      0     0     0    0     0      0   0   1   2   Headache
 ```
 
 ## Contributing
 
 We love 💖 contributions!
 
 If you have a good suggestion 💡 or found a bug 🐛,
```

