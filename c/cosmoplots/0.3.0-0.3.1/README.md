# Comparing `tmp/cosmoplots-0.3.0.tar.gz` & `tmp/cosmoplots-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmoplots-0.3.0.tar", max compression
+gzip compressed data, was "cosmoplots-0.3.1.tar", max compression
```

## Comparing `cosmoplots-0.3.0.tar` & `cosmoplots-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/LICENSE
--rw-r--r--   0        0        0     3464 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/README.md
--rw-r--r--   0        0        0      145 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/cosmoplots/__init__.py
--rw-r--r--   0        0        0     2241 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/cosmoplots/axes.py
--rw-r--r--   0        0        0     2723 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/cosmoplots/colors.py
--rw-r--r--   0        0        0     1150 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/cosmoplots/default.mplstyle
--rw-r--r--   0        0        0     5516 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/cosmoplots/figure_defs.py
--rw-r--r--   0        0        0       37 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/cosmoplots/thick_line.mplstyle
--rw-r--r--   0        0        0      251 2023-08-14 08:55:29.956224 cosmoplots-0.3.0/cosmoplots/two_columns.mplstyle
--rw-r--r--   0        0        0      515 2023-08-14 08:55:44.872335 cosmoplots-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4222 1970-01-01 00:00:00.000000 cosmoplots-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3907 2024-04-29 09:48:24.735133 cosmoplots-0.3.1/README.md
+-rw-r--r--   0        0        0      145 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/__init__.py
+-rw-r--r--   0        0        0     3090 2024-04-29 09:48:24.735133 cosmoplots-0.3.1/cosmoplots/axes.py
+-rw-r--r--   0        0        0     2723 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/colors.py
+-rw-r--r--   0        0        0     1150 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/default.mplstyle
+-rw-r--r--   0        0        0     5516 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/figure_defs.py
+-rw-r--r--   0        0        0       37 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/thick_line.mplstyle
+-rw-r--r--   0        0        0      251 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/two_columns.mplstyle
+-rw-r--r--   0        0        0      515 2024-04-29 09:48:24.735133 cosmoplots-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 cosmoplots-0.3.1/PKG-INFO
```

### Comparing `cosmoplots-0.3.0/LICENSE` & `cosmoplots-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.0/README.md` & `cosmoplots-0.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -38,27 +38,42 @@
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
 import cosmoplots
 import matplotlib as mpl
 
+# Setup
 mpl.style.use("cosmoplots.default")
-a = np.exp(np.linspace(-3, 5, 100))
+a = np.exp(np.linspace(-3, 1, 100))
+
+# Plotting
+fig = plt.figure()
+ax1 = plt.gca()
+ax1.set_xlabel("X Axis")
+ax1.set_ylabel("Y Axis")
+base = 2  # Default is 10, but 2 works equally well
+# Do plotting ...
+ax1.semilogx(a)
+# It is recommended to call the change_log_axis_base function after doing all the
+# plotting. By default, it will try to infer the scaling used for the axis and only
+# adjust accordingly.
+cosmoplots.change_log_axis_base(ax1, base=base)
+# Plotting
 fig = plt.figure()
-ax = plt.gca()
-ax.set_xlabel("X Axis")
-ax.set_ylabel("Y Axis")
+ax2 = plt.gca()
+ax2.set_xlabel("X Axis")
+ax2.set_ylabel("Y Axis")
 base = 2  # Default is 10, but 2 works equally well
-cosmoplots.change_log_axis_base(ax, "x", base=base)
+cosmoplots.change_log_axis_base(ax2, "x", base=base)
 # Do plotting ...
 # If you use "plot", the change_log_axis_base can be called at the top (along with add_axes
 # etc.), but using loglog, semilogx, semilogy will re-set, and the change_log_axis_base
 # function must be called again.
-ax.plot(a)
+ax2.plot(a)
 plt.show()
 ```
 
 ## `matplotlib` vs. `cosmoplots` defaults
 
 ```python
 import cosmoplots
```

### Comparing `cosmoplots-0.3.0/cosmoplots/colors.py` & `cosmoplots-0.3.1/cosmoplots/colors.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.0/cosmoplots/default.mplstyle` & `cosmoplots-0.3.1/cosmoplots/default.mplstyle`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.0/cosmoplots/figure_defs.py` & `cosmoplots-0.3.1/cosmoplots/figure_defs.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.0/pyproject.toml` & `cosmoplots-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cosmoplots"
-version = "0.3.0"
+version = "0.3.1"
 description = "Routines to get a sane default configuration for production quality plots."
 homepage = "https://github.com/uit-cosmo/cosmoplots"
 authors = ["gregordecristoforo <gregor.decristoforo@gmail.com>"]
 license = "MIT License"
 readme = 'README.md'
 
 [tool.poetry.dependencies]
```

### Comparing `cosmoplots-0.3.0/PKG-INFO` & `cosmoplots-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cosmoplots
-Version: 0.3.0
+Version: 0.3.1
 Summary: Routines to get a sane default configuration for production quality plots.
 Home-page: https://github.com/uit-cosmo/cosmoplots
 License: MIT
 Author: gregordecristoforo
 Author-email: gregor.decristoforo@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: importlib-metadata (>=6.6.0,<7.0.0)
 Requires-Dist: matplotlib (>=3.3.2)
 Requires-Dist: numpy (>=1.15.0)
 Description-Content-Type: text/markdown
 
 # cosmoplots
 
@@ -58,27 +59,42 @@
 
 ```python
 import matplotlib.pyplot as plt
 import numpy as np
 import cosmoplots
 import matplotlib as mpl
 
+# Setup
 mpl.style.use("cosmoplots.default")
-a = np.exp(np.linspace(-3, 5, 100))
+a = np.exp(np.linspace(-3, 1, 100))
+
+# Plotting
+fig = plt.figure()
+ax1 = plt.gca()
+ax1.set_xlabel("X Axis")
+ax1.set_ylabel("Y Axis")
+base = 2  # Default is 10, but 2 works equally well
+# Do plotting ...
+ax1.semilogx(a)
+# It is recommended to call the change_log_axis_base function after doing all the
+# plotting. By default, it will try to infer the scaling used for the axis and only
+# adjust accordingly.
+cosmoplots.change_log_axis_base(ax1, base=base)
+# Plotting
 fig = plt.figure()
-ax = plt.gca()
-ax.set_xlabel("X Axis")
-ax.set_ylabel("Y Axis")
+ax2 = plt.gca()
+ax2.set_xlabel("X Axis")
+ax2.set_ylabel("Y Axis")
 base = 2  # Default is 10, but 2 works equally well
-cosmoplots.change_log_axis_base(ax, "x", base=base)
+cosmoplots.change_log_axis_base(ax2, "x", base=base)
 # Do plotting ...
 # If you use "plot", the change_log_axis_base can be called at the top (along with add_axes
 # etc.), but using loglog, semilogx, semilogy will re-set, and the change_log_axis_base
 # function must be called again.
-ax.plot(a)
+ax2.plot(a)
 plt.show()
 ```
 
 ## `matplotlib` vs. `cosmoplots` defaults
 
 ```python
 import cosmoplots
```

