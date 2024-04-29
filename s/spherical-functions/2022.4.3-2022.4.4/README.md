# Comparing `tmp/spherical_functions-2022.4.3.tar.gz` & `tmp/spherical_functions-2022.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spherical_functions-2022.4.3.tar", max compression
+gzip compressed data, was "spherical_functions-2022.4.4.tar", max compression
```

## Comparing `spherical_functions-2022.4.3.tar` & `spherical_functions-2022.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1078 2024-03-22 00:49:17.839842 spherical_functions-2022.4.3/LICENSE
--rw-r--r--   0        0        0     6895 2024-03-22 00:49:17.839842 spherical_functions-2022.4.3/README.md
--rw-r--r--   0        0        0     1055 2024-03-22 00:49:51.551805 spherical_functions-2022.4.3/pyproject.toml
--rw-r--r--   0        0        0    13720 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH/__init__.py
--rw-r--r--   0        0        0     6639 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_grids/__init__.py
--rw-r--r--   0        0        0     6756 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_grids/algebra.py
--rw-r--r--   0        0        0     9059 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_grids/ufuncs.py
--rw-r--r--   0        0        0     2746 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_grids/utilities.py
--rw-r--r--   0        0        0     9513 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_modes/__init__.py
--rw-r--r--   0        0        0    11783 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_modes/algebra.py
--rw-r--r--   0        0        0    14859 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_modes/derivatives.py
--rw-r--r--   0        0        0     9154 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_modes/ufuncs.py
--rw-r--r--   0        0        0     5237 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/SWSH_modes/utilities.py
--rw-r--r--   0        0        0    17712 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/WignerD/WignerDRecursion.py
--rw-r--r--   0        0        0    30163 2024-03-22 00:49:17.843843 spherical_functions-2022.4.3/spherical_functions/WignerD/__init__.py
--rw-r--r--   0        0        0   749400 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/Wigner_coefficients.npy
--rw-r--r--   0        0        0    11312 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/__init__.py
--rw-r--r--   0        0        0     2537 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/_generate_coefficients.py
--rw-r--r--   0        0        0    17240 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/binomial_coefficients.npy
--rw-r--r--   0        0        0    17240 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/ladder_operator_coefficients.npy
--rw-r--r--   0        0        0     9583 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/mode_conversions.py
--rw-r--r--   0        0        0     4410 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/multiplication.py
--rw-r--r--   0        0        0     4995 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/recursions/__init__.py
--rw-r--r--   0        0        0     3328 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/recursions/associated_legendre_functions.py
--rw-r--r--   0        0        0     2743 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/recursions/complex_powers.py
--rw-r--r--   0        0        0    14029 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/recursions/wigner3j.py
--rw-r--r--   0        0        0    19158 2024-03-22 00:49:17.847843 spherical_functions-2022.4.3/spherical_functions/recursions/wignerH.py
--rw-r--r--   0        0        0     7744 1970-01-01 00:00:00.000000 spherical_functions-2022.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-04-29 20:48:10.909041 spherical_functions-2022.4.4/LICENSE
+-rw-r--r--   0        0        0     6895 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/README.md
+-rw-r--r--   0        0        0     1049 2024-04-29 20:48:32.137073 spherical_functions-2022.4.4/pyproject.toml
+-rw-r--r--   0        0        0    13720 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH/__init__.py
+-rw-r--r--   0        0        0     6639 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_grids/__init__.py
+-rw-r--r--   0        0        0     6756 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_grids/algebra.py
+-rw-r--r--   0        0        0     9059 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_grids/ufuncs.py
+-rw-r--r--   0        0        0     2746 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_grids/utilities.py
+-rw-r--r--   0        0        0     9513 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_modes/__init__.py
+-rw-r--r--   0        0        0    11783 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_modes/algebra.py
+-rw-r--r--   0        0        0    14859 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_modes/derivatives.py
+-rw-r--r--   0        0        0     9154 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_modes/ufuncs.py
+-rw-r--r--   0        0        0     5237 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/SWSH_modes/utilities.py
+-rw-r--r--   0        0        0    17712 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/WignerD/WignerDRecursion.py
+-rw-r--r--   0        0        0    30163 2024-04-29 20:48:10.913041 spherical_functions-2022.4.4/spherical_functions/WignerD/__init__.py
+-rw-r--r--   0        0        0   749400 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/Wigner_coefficients.npy
+-rw-r--r--   0        0        0    11312 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/__init__.py
+-rw-r--r--   0        0        0     2537 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/_generate_coefficients.py
+-rw-r--r--   0        0        0    17240 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/binomial_coefficients.npy
+-rw-r--r--   0        0        0    17240 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/ladder_operator_coefficients.npy
+-rw-r--r--   0        0        0     9583 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/mode_conversions.py
+-rw-r--r--   0        0        0     4410 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/multiplication.py
+-rw-r--r--   0        0        0     4995 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/recursions/__init__.py
+-rw-r--r--   0        0        0     3328 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/recursions/associated_legendre_functions.py
+-rw-r--r--   0        0        0     2743 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/recursions/complex_powers.py
+-rw-r--r--   0        0        0    14029 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/recursions/wigner3j.py
+-rw-r--r--   0        0        0    19158 2024-04-29 20:48:10.917041 spherical_functions-2022.4.4/spherical_functions/recursions/wignerH.py
+-rw-r--r--   0        0        0     7789 1970-01-01 00:00:00.000000 spherical_functions-2022.4.4/PKG-INFO
```

### Comparing `spherical_functions-2022.4.3/LICENSE` & `spherical_functions-2022.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/README.md` & `spherical_functions-2022.4.4/README.md`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/pyproject.toml` & `spherical_functions-2022.4.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "spherical-functions"
 description = "Python/numba implementation of Wigner D Matrices, spin-weighted spherical harmonics, and associated functions"
-version = "2022.4.3"
+version = "2022.4.4"
 readme = "README.md"
 license = "MIT"
 authors = ["Michael Boyle <mob22@cornell.edu>"]
 homepage = "https://github.com/moble/spherical_functions"
 packages = [{include = "spherical_functions" }]
 include = ["spherical_functions/*.npy"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8"
 numpy = ">=1.20"
 scipy = "^1.0"
 numba = ">=0.55"
 numpy-quaternion = ">=2022"
 spinsfast = ">=2022"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH/__init__.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_grids/__init__.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_grids/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_grids/algebra.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_grids/algebra.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_grids/ufuncs.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_grids/ufuncs.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_grids/utilities.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_grids/utilities.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_modes/__init__.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_modes/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_modes/algebra.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_modes/algebra.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_modes/derivatives.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_modes/derivatives.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_modes/ufuncs.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_modes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/SWSH_modes/utilities.py` & `spherical_functions-2022.4.4/spherical_functions/SWSH_modes/utilities.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/WignerD/WignerDRecursion.py` & `spherical_functions-2022.4.4/spherical_functions/WignerD/WignerDRecursion.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/WignerD/__init__.py` & `spherical_functions-2022.4.4/spherical_functions/WignerD/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/Wigner_coefficients.npy` & `spherical_functions-2022.4.4/spherical_functions/Wigner_coefficients.npy`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/__init__.py` & `spherical_functions-2022.4.4/spherical_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/_generate_coefficients.py` & `spherical_functions-2022.4.4/spherical_functions/_generate_coefficients.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/binomial_coefficients.npy` & `spherical_functions-2022.4.4/spherical_functions/binomial_coefficients.npy`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/ladder_operator_coefficients.npy` & `spherical_functions-2022.4.4/spherical_functions/ladder_operator_coefficients.npy`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/mode_conversions.py` & `spherical_functions-2022.4.4/spherical_functions/mode_conversions.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/multiplication.py` & `spherical_functions-2022.4.4/spherical_functions/multiplication.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/recursions/__init__.py` & `spherical_functions-2022.4.4/spherical_functions/recursions/__init__.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/recursions/associated_legendre_functions.py` & `spherical_functions-2022.4.4/spherical_functions/recursions/associated_legendre_functions.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/recursions/complex_powers.py` & `spherical_functions-2022.4.4/spherical_functions/recursions/complex_powers.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/recursions/wigner3j.py` & `spherical_functions-2022.4.4/spherical_functions/recursions/wigner3j.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/spherical_functions/recursions/wignerH.py` & `spherical_functions-2022.4.4/spherical_functions/recursions/wignerH.py`

 * *Files identical despite different names*

### Comparing `spherical_functions-2022.4.3/PKG-INFO` & `spherical_functions-2022.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: spherical-functions
-Version: 2022.4.3
+Version: 2022.4.4
 Summary: Python/numba implementation of Wigner D Matrices, spin-weighted spherical harmonics, and associated functions
 Home-page: https://github.com/moble/spherical_functions
 License: MIT
 Author: Michael Boyle
 Author-email: mob22@cornell.edu
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numba (>=0.55)
 Requires-Dist: numpy (>=1.20)
 Requires-Dist: numpy-quaternion (>=2022)
 Requires-Dist: scipy (>=1.0,<2.0)
 Requires-Dist: spinsfast (>=2022)
 Description-Content-Type: text/markdown
```

