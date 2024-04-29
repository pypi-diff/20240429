# Comparing `tmp/cosmoplots-0.3.1.tar.gz` & `tmp/cosmoplots-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmoplots-0.3.1.tar", max compression
+gzip compressed data, was "cosmoplots-0.4.0.tar", max compression
```

## Comparing `cosmoplots-0.3.1.tar` & `cosmoplots-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1076 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/LICENSE
--rw-r--r--   0        0        0     3907 2024-04-29 09:48:24.735133 cosmoplots-0.3.1/README.md
--rw-r--r--   0        0        0      145 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/__init__.py
--rw-r--r--   0        0        0     3090 2024-04-29 09:48:24.735133 cosmoplots-0.3.1/cosmoplots/axes.py
--rw-r--r--   0        0        0     2723 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/colors.py
--rw-r--r--   0        0        0     1150 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/default.mplstyle
--rw-r--r--   0        0        0     5516 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/figure_defs.py
--rw-r--r--   0        0        0       37 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/thick_line.mplstyle
--rw-r--r--   0        0        0      251 2024-04-29 09:48:14.814936 cosmoplots-0.3.1/cosmoplots/two_columns.mplstyle
--rw-r--r--   0        0        0      515 2024-04-29 09:48:24.735133 cosmoplots-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4716 1970-01-01 00:00:00.000000 cosmoplots-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-29 10:53:14.105787 cosmoplots-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5662 2024-04-29 10:53:25.985825 cosmoplots-0.4.0/README.md
+-rw-r--r--   0        0        0      167 2024-04-29 10:53:25.985825 cosmoplots-0.4.0/cosmoplots/__init__.py
+-rw-r--r--   0        0        0     3090 2024-04-29 10:53:14.109787 cosmoplots-0.4.0/cosmoplots/axes.py
+-rw-r--r--   0        0        0     2723 2024-04-29 10:53:14.109787 cosmoplots-0.4.0/cosmoplots/colors.py
+-rw-r--r--   0        0        0    10355 2024-04-29 10:53:25.985825 cosmoplots-0.4.0/cosmoplots/concat.py
+-rw-r--r--   0        0        0     1150 2024-04-29 10:53:14.109787 cosmoplots-0.4.0/cosmoplots/default.mplstyle
+-rw-r--r--   0        0        0     5516 2024-04-29 10:53:14.109787 cosmoplots-0.4.0/cosmoplots/figure_defs.py
+-rw-r--r--   0        0        0       37 2024-04-29 10:53:14.109787 cosmoplots-0.4.0/cosmoplots/thick_line.mplstyle
+-rw-r--r--   0        0        0      251 2024-04-29 10:53:14.109787 cosmoplots-0.4.0/cosmoplots/two_columns.mplstyle
+-rw-r--r--   0        0        0      577 2024-04-29 10:53:25.989825 cosmoplots-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6477 1970-01-01 00:00:00.000000 cosmoplots-0.4.0/PKG-INFO
```

### Comparing `cosmoplots-0.3.1/LICENSE` & `cosmoplots-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.1/README.md` & `cosmoplots-0.4.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -134,7 +134,72 @@
 
 plt.savefig("./assets/hex_colors_example.png")
 plt.show()
 ```
 | `hex_colors.png` | hex_colors_example.png |
 | :--------: | :--------: | 
 | ![colors](./assets/hex_colors.png) | ![colors](./assets/hex_colors_example.png) |
+
+## `combine`
+
+Sometimes, plots might be related and better placed as subfigures in a larger figure. If
+combining the plots using the `subfigure` environment in latex or similar is not an
+option, this is easily done with [`imagemagick`](https://imagemagick.org/index.php) in a
+systematic way.
+
+The `Combine` class within the `concat` module implements such procedures, and is also
+conveniently available from the `combine` function in `cosmoplots`.
+
+An example is shown below. Also see the [`tests`](./tests/) directory for more examples.
+A `help` method that prints the `imagemagick` commands that are used under the hood is
+also available.
+
+```python
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import numpy as np
+
+import cosmoplots
+
+mpl.style.use("cosmoplots.default")
+
+
+def plot(i) -> None:
+    """Create a simple plot."""
+    a = np.exp(np.linspace(-3, 5, 100))
+    fig = plt.figure()
+    ax = fig.add_subplot()
+    ax.set_xlabel("X Axis")
+    ax.set_ylabel("Y Axis")
+    ax.semilogy(a)
+    plt.savefig(f"./assets/{i}.png")
+    plt.close(fig)
+
+plot(1)
+plot(2)
+plot(3)
+plot(4)
+plot(5)
+plot(6)
+plot(7)
+plot(8)
+plot(9)
+plot(10)
+# See `convert -list font` for all available fonts.
+figs = [f"./assets/{i}.png" for i in range(1, 11)]
+cosmoplots.combine(*figs).using(
+    font="JetBrainsMonoNL-NFM-Medium",
+    fontsize=60,
+    gravity="southeast",
+    pos=(100, 200),
+    color="green",
+).in_grid(w=3, h=4).with_labels(  # Specifying labels is optional
+    "one", "four", "three", "two", "eight", "six", "seven", "five", "nine", "ten"
+).save("./assets/concat.png")
+
+# Note that cosmoplots.combine() == cosmoplots.Combine().combine()
+cosmoplots.combine().help()
+# Or equivalently
+cosmoplots.Combine().help()
+```
+
+![concat](./assets/concat.png)
```

### Comparing `cosmoplots-0.3.1/cosmoplots/axes.py` & `cosmoplots-0.4.0/cosmoplots/axes.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.1/cosmoplots/colors.py` & `cosmoplots-0.4.0/cosmoplots/colors.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.1/cosmoplots/default.mplstyle` & `cosmoplots-0.4.0/cosmoplots/default.mplstyle`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.1/cosmoplots/figure_defs.py` & `cosmoplots-0.4.0/cosmoplots/figure_defs.py`

 * *Files identical despite different names*

### Comparing `cosmoplots-0.3.1/pyproject.toml` & `cosmoplots-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 [tool.poetry]
 name = "cosmoplots"
-version = "0.3.1"
+version = "0.4.0"
 description = "Routines to get a sane default configuration for production quality plots."
 homepage = "https://github.com/uit-cosmo/cosmoplots"
 authors = ["gregordecristoforo <gregor.decristoforo@gmail.com>"]
 license = "MIT License"
 readme = 'README.md'
 
 [tool.poetry.dependencies]
-python = ">=3.8"
+python = ">=3.8,<3.13"
 numpy = ">=1.15.0"
 matplotlib = ">=3.3.2"
 importlib-metadata = "^6.6.0"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.3"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cosmoplots-0.3.1/PKG-INFO` & `cosmoplots-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cosmoplots
-Version: 0.3.1
+Version: 0.4.0
 Summary: Routines to get a sane default configuration for production quality plots.
 Home-page: https://github.com/uit-cosmo/cosmoplots
 License: MIT
 Author: gregordecristoforo
 Author-email: gregor.decristoforo@gmail.com
-Requires-Python: >=3.8
+Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -156,7 +156,72 @@
 plt.savefig("./assets/hex_colors_example.png")
 plt.show()
 ```
 | `hex_colors.png` | hex_colors_example.png |
 | :--------: | :--------: | 
 | ![colors](./assets/hex_colors.png) | ![colors](./assets/hex_colors_example.png) |
 
+## `combine`
+
+Sometimes, plots might be related and better placed as subfigures in a larger figure. If
+combining the plots using the `subfigure` environment in latex or similar is not an
+option, this is easily done with [`imagemagick`](https://imagemagick.org/index.php) in a
+systematic way.
+
+The `Combine` class within the `concat` module implements such procedures, and is also
+conveniently available from the `combine` function in `cosmoplots`.
+
+An example is shown below. Also see the [`tests`](./tests/) directory for more examples.
+A `help` method that prints the `imagemagick` commands that are used under the hood is
+also available.
+
+```python
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import numpy as np
+
+import cosmoplots
+
+mpl.style.use("cosmoplots.default")
+
+
+def plot(i) -> None:
+    """Create a simple plot."""
+    a = np.exp(np.linspace(-3, 5, 100))
+    fig = plt.figure()
+    ax = fig.add_subplot()
+    ax.set_xlabel("X Axis")
+    ax.set_ylabel("Y Axis")
+    ax.semilogy(a)
+    plt.savefig(f"./assets/{i}.png")
+    plt.close(fig)
+
+plot(1)
+plot(2)
+plot(3)
+plot(4)
+plot(5)
+plot(6)
+plot(7)
+plot(8)
+plot(9)
+plot(10)
+# See `convert -list font` for all available fonts.
+figs = [f"./assets/{i}.png" for i in range(1, 11)]
+cosmoplots.combine(*figs).using(
+    font="JetBrainsMonoNL-NFM-Medium",
+    fontsize=60,
+    gravity="southeast",
+    pos=(100, 200),
+    color="green",
+).in_grid(w=3, h=4).with_labels(  # Specifying labels is optional
+    "one", "four", "three", "two", "eight", "six", "seven", "five", "nine", "ten"
+).save("./assets/concat.png")
+
+# Note that cosmoplots.combine() == cosmoplots.Combine().combine()
+cosmoplots.combine().help()
+# Or equivalently
+cosmoplots.Combine().help()
+```
+
+![concat](./assets/concat.png)
+
```

