# Comparing `tmp/pdme-0.9.3.tar.gz` & `tmp/pdme-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdme-0.9.3.tar", max compression
+gzip compressed data, was "pdme-1.0.0.tar", max compression
```

## Comparing `pdme-0.9.3.tar` & `pdme-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,46 @@
--rw-r--r--   0        0        0     1229 2024-02-26 23:36:04.098696 pdme-0.9.3/README.md
--rw-r--r--   0        0        0      154 2024-02-26 23:36:04.098696 pdme-0.9.3/pdme/__init__.py
--rw-r--r--   0        0        0      184 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/inputs/__init__.py
--rw-r--r--   0        0        0      688 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/inputs/dot_inputs.py
--rw-r--r--   0        0        0      536 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/measurement/__init__.py
--rw-r--r--   0        0        0      984 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/measurement/dot_measure.py
--rw-r--r--   0        0        0     1224 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/measurement/dot_pair_measure.py
--rw-r--r--   0        0        0     1131 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/measurement/input_types.py
--rw-r--r--   0        0        0     5219 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/measurement/oscillating_dipole.py
--rw-r--r--   0        0        0       70 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/meta.py
--rw-r--r--   0        0        0     1066 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/model/__init__.py
--rw-r--r--   0        0        0     2367 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/model/fixed_magnitude_model.py
--rw-r--r--   0        0        0     5158 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
--rw-r--r--   0        0        0     5332 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/model/log_spaced_random_choice_model.py
--rw-r--r--   0        0        0     4699 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/model/log_spaced_random_choice_xy_model.py
--rw-r--r--   0        0        0     3594 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/model/model.py
--rw-r--r--   0        0        0     2560 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/model/multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0     3076 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/model/random_count_multidipole_fixed_magnitude_model.py
--rw-r--r--   0        0        0        0 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/py.typed
--rw-r--r--   0        0        0     1364 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/subspace_simulation/__init__.py
--rw-r--r--   0        0        0      575 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/subspace_simulation/mcmc_costs.py
--rw-r--r--   0        0        0        0 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/util/__init__.py
--rw-r--r--   0        0        0     3192 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/util/fast_nonlocal_spectrum.py
--rw-r--r--   0        0        0     3604 2024-02-26 23:36:04.102696 pdme-0.9.3/pdme/util/fast_v_calc.py
--rw-r--r--   0        0        0      965 2024-02-26 23:36:04.102696 pdme-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     1972 2024-02-26 23:37:21.115165 pdme-0.9.3/setup.py
--rw-r--r--   0        0        0     1720 2024-02-26 23:37:21.115697 pdme-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1229 2024-04-29 02:29:58.024469 pdme-1.0.0/README.md
+-rw-r--r--   0        0        0      154 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/inputs/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-29 02:30:19.109512 pdme-1.0.0/pdme/inputs/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1471 2024-04-29 02:30:19.109512 pdme-1.0.0/pdme/inputs/__pycache__/dot_inputs.cpython-39.pyc
+-rw-r--r--   0        0        0      688 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/inputs/dot_inputs.py
+-rw-r--r--   0        0        0      536 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/__init__.py
+-rw-r--r--   0        0        0      642 2024-04-29 02:30:20.821596 pdme-1.0.0/pdme/measurement/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1642 2024-04-29 02:30:20.825596 pdme-1.0.0/pdme/measurement/__pycache__/dot_measure.cpython-39.pyc
+-rw-r--r--   0        0        0     1864 2024-04-29 02:30:20.825596 pdme-1.0.0/pdme/measurement/__pycache__/dot_pair_measure.cpython-39.pyc
+-rw-r--r--   0        0        0     1818 2024-04-29 02:30:20.833597 pdme-1.0.0/pdme/measurement/__pycache__/input_types.cpython-39.pyc
+-rw-r--r--   0        0        0     8295 2024-04-29 02:30:20.829597 pdme-1.0.0/pdme/measurement/__pycache__/oscillating_dipole.cpython-39.pyc
+-rw-r--r--   0        0        0      984 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/dot_measure.py
+-rw-r--r--   0        0        0     1224 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/dot_pair_measure.py
+-rw-r--r--   0        0        0     1131 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/input_types.py
+-rw-r--r--   0        0        0     5219 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/measurement/oscillating_dipole.py
+-rw-r--r--   0        0        0       70 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/meta.py
+-rw-r--r--   0        0        0     1066 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/model/__init__.py
+-rw-r--r--   0        0        0      988 2024-04-29 02:30:20.861598 pdme-1.0.0/pdme/model/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2740 2024-04-29 02:30:20.873599 pdme-1.0.0/pdme/model/__pycache__/fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5039 2024-04-29 02:30:20.885599 pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_fixed_orientation_model.cpython-39.pyc
+-rw-r--r--   0        0        0     5083 2024-04-29 02:30:20.881599 pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_model.cpython-39.pyc
+-rw-r--r--   0        0        0     4757 2024-04-29 02:30:20.885599 pdme-1.0.0/pdme/model/__pycache__/log_spaced_random_choice_xy_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3850 2024-04-29 02:30:20.865599 pdme-1.0.0/pdme/model/__pycache__/model.cpython-39.pyc
+-rw-r--r--   0        0        0     2928 2024-04-29 02:30:20.877599 pdme-1.0.0/pdme/model/__pycache__/multidipole_fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     3362 2024-04-29 02:30:20.877599 pdme-1.0.0/pdme/model/__pycache__/random_count_multidipole_fixed_magnitude_model.cpython-39.pyc
+-rw-r--r--   0        0        0     2367 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/model/fixed_magnitude_model.py
+-rw-r--r--   0        0        0     5158 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py
+-rw-r--r--   0        0        0     5332 2024-04-29 02:29:58.024469 pdme-1.0.0/pdme/model/log_spaced_random_choice_model.py
+-rw-r--r--   0        0        0     4699 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/model/log_spaced_random_choice_xy_model.py
+-rw-r--r--   0        0        0     3594 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/model/model.py
+-rw-r--r--   0        0        0     2560 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/model/multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0     3076 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py
+-rw-r--r--   0        0        0        0 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/py.typed
+-rw-r--r--   0        0        0     1364 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/subspace_simulation/__init__.py
+-rw-r--r--   0        0        0     2144 2024-04-29 02:30:20.865599 pdme-1.0.0/pdme/subspace_simulation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      842 2024-04-29 02:30:20.869599 pdme-1.0.0/pdme/subspace_simulation/__pycache__/mcmc_costs.cpython-39.pyc
+-rw-r--r--   0        0        0      575 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/subspace_simulation/mcmc_costs.py
+-rw-r--r--   0        0        0        0 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/util/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-29 02:30:20.869599 pdme-1.0.0/pdme/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4177 2024-04-29 02:30:21.121611 pdme-1.0.0/pdme/util/__pycache__/fast_nonlocal_spectrum.cpython-39.pyc
+-rw-r--r--   0        0        0     3833 2024-04-29 02:30:20.869599 pdme-1.0.0/pdme/util/__pycache__/fast_v_calc.cpython-39.pyc
+-rw-r--r--   0        0        0     7925 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/util/fast_nonlocal_spectrum.py
+-rw-r--r--   0        0        0     3604 2024-04-29 02:29:58.028469 pdme-1.0.0/pdme/util/fast_v_calc.py
+-rw-r--r--   0        0        0      965 2024-04-29 02:29:58.028469 pdme-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1720 1970-01-01 00:00:00.000000 pdme-1.0.0/PKG-INFO
```

### Comparing `pdme-0.9.3/README.md` & `pdme-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/inputs/dot_inputs.py` & `pdme-1.0.0/pdme/inputs/dot_inputs.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/measurement/__init__.py` & `pdme-1.0.0/pdme/measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/measurement/dot_measure.py` & `pdme-1.0.0/pdme/measurement/dot_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/measurement/dot_pair_measure.py` & `pdme-1.0.0/pdme/measurement/dot_pair_measure.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/measurement/input_types.py` & `pdme-1.0.0/pdme/measurement/input_types.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/measurement/oscillating_dipole.py` & `pdme-1.0.0/pdme/measurement/oscillating_dipole.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/model/__init__.py` & `pdme-1.0.0/pdme/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/model/fixed_magnitude_model.py` & `pdme-1.0.0/pdme/model/fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/model/log_spaced_random_choice_fixed_orientation_model.py` & `pdme-1.0.0/pdme/model/log_spaced_random_choice_fixed_orientation_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/model/log_spaced_random_choice_model.py` & `pdme-1.0.0/pdme/model/log_spaced_random_choice_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/model/log_spaced_random_choice_xy_model.py` & `pdme-1.0.0/pdme/model/log_spaced_random_choice_xy_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/model/model.py` & `pdme-1.0.0/pdme/model/model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/model/multidipole_fixed_magnitude_model.py` & `pdme-1.0.0/pdme/model/multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/model/random_count_multidipole_fixed_magnitude_model.py` & `pdme-1.0.0/pdme/model/random_count_multidipole_fixed_magnitude_model.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/subspace_simulation/__init__.py` & `pdme-1.0.0/pdme/subspace_simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/subspace_simulation/mcmc_costs.py` & `pdme-1.0.0/pdme/subspace_simulation/mcmc_costs.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pdme/util/fast_v_calc.py` & `pdme-1.0.0/pdme/util/fast_v_calc.py`

 * *Files identical despite different names*

### Comparing `pdme-0.9.3/pyproject.toml` & `pdme-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdme"
-version = "0.9.3"
+version = "1.0.0"
 description = "Python dipole model evaluator"
 authors = ["Deepak <dmallubhotla+github@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
```

### Comparing `pdme-0.9.3/PKG-INFO` & `pdme-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdme
-Version: 0.9.3
+Version: 1.0.0
 Summary: Python dipole model evaluator
 License: GPL-3.0-only
 Author: Deepak
 Author-email: dmallubhotla+github@gmail.com
 Requires-Python: >=3.8.1,<3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

