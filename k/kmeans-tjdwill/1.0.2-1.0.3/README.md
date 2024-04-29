# Comparing `tmp/kmeans_tjdwill-1.0.2.tar.gz` & `tmp/kmeans_tjdwill-1.0.3.tar.gz`

## Comparing `kmeans_tjdwill-1.0.2.tar` & `kmeans_tjdwill-1.0.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/requirements.txt
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/.github/workflows/sitebuild.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/Makefile
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/api-dev.rst
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/api-user.rst
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/conf.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/index.rst
--rwxr-xr-x   0        0        0      800 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/make.bat
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/docs/modules.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/__init__.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/animate.py
--rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/base_funcs.py
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/clustering.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/segmentation.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_animate2D.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_animate3D.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_assign_cluster.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_clustering.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_datavalidation.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_distances.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_gen_means.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/test_segmentation.py
--rw-r--r--   0        0        0    13710 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/output/seg_groups04.jpg
--rw-r--r--   0        0        0    15340 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/output/seg_groups10.jpg
--rw-r--r--   0        0        0    18720 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/output/seg_rand_groups04.jpg
--rw-r--r--   0        0        0    25980 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/tests/output/seg_rand_groups10.jpg
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/LICENSE
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/README.md
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/.github/workflows/sitebuild.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/docs/Makefile
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/docs/api-dev.rst
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/docs/api-user.rst
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/docs/conf.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/docs/make.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/docs/modules.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/__init__.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/animate.py
+-rw-r--r--   0        0        0     8754 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/base_funcs.py
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/clustering.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/segmentation.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/test_animate2D.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/test_animate3D.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/test_assign_cluster.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/test_clustering.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/test_datavalidation.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/test_distances.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/test_gen_means.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/test_segmentation.py
+-rw-r--r--   0        0        0    13710 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/output/seg_groups04.jpg
+-rw-r--r--   0        0        0    15340 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/output/seg_groups10.jpg
+-rw-r--r--   0        0        0    18720 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/output/seg_rand_groups04.jpg
+-rw-r--r--   0        0        0    25980 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/tests/output/seg_rand_groups10.jpg
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/LICENSE
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/README.md
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 kmeans_tjdwill-1.0.3/PKG-INFO
```

### Comparing `kmeans_tjdwill-1.0.2/requirements.txt` & `kmeans_tjdwill-1.0.3/requirements.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-alabaster==0.7.16
-anyio==4.3.0
-Babel==2.14.0
-beautifulsoup4==4.12.3
-build==1.2.1
-certifi==2024.2.2
-charset-normalizer==3.3.2
-click==8.1.7
-colorama==0.4.6
-contourpy==1.2.1
-css-html-js-minify==2.5.5
-cycler==0.12.1
-distlib==0.3.8
-docutils==0.20.1
-editables==0.5
-filelock==3.13.4
-fonttools==4.51.0
-furo==2024.4.27
-h11==0.14.0
-hatch==1.9.7
-hatchling==1.21.1
-httpcore==1.0.5
-httpx==0.27.0
-hyperlink==21.0.0
-idna==3.7
-imagesize==1.4.1
-importlib_metadata==7.1.0
-jaraco.classes==3.4.0
-jaraco.context==5.3.0
-jaraco.functools==4.0.1
-Jinja2==3.1.3
-keyring==25.2.0
-kiwisolver==1.4.5
-lxml==5.2.1
-markdown-it-py==3.0.0
-MarkupSafe==2.1.5
-matplotlib==3.8.4
-mdurl==0.1.2
-more-itertools==10.2.0
-nh3==0.2.17
-numpy==1.26.4
-packaging==24.0
-pathspec==0.12.1
-pexpect==4.9.0
-pillow==10.3.0
-pkginfo==1.10.0
-platformdirs==4.2.1
-pluggy==1.5.0
-ptyprocess==0.7.0
-Pygments==2.17.2
-pyparsing==3.1.2
-pyproject_hooks==1.0.0
-python-dateutil==2.9.0.post0
-python-docs-theme==2024.4
-python-slugify==8.0.4
-pywin32-ctypes==0.2.2
-readme_renderer==43.0
-requests==2.31.0
-requests-toolbelt==1.0.0
-rfc3986==2.0.0
-rich==13.7.1
-shellingham==1.5.4
-six==1.16.0
-sniffio==1.3.1
-snowballstemmer==2.2.0
-soupsieve==2.5
-Sphinx==7.3.7
-sphinx-basic-ng==1.0.0b2
-sphinx-material==0.0.36
-sphinx-rtd-theme==2.0.0
-sphinxcontrib-applehelp==1.0.8
-sphinxcontrib-devhelp==1.0.6
-sphinxcontrib-htmlhelp==2.0.5
-sphinxcontrib-jquery==4.1
-sphinxcontrib-jsmath==1.0.1
-sphinxcontrib-qthelp==1.0.7
-sphinxcontrib-serializinghtml==1.1.10
-text-unidecode==1.3
-tomli_w==1.0.0
-tomlkit==0.12.4
-trove-classifiers==2024.4.10
-twine==5.0.0
-Unidecode==1.3.8
-urllib3==2.2.1
-userpath==1.9.2
-virtualenv==20.25.3
-zipp==3.18.1
-zstandard==0.22.0
+alabaster==0.7.16
+anyio==4.3.0
+Babel==2.14.0
+beautifulsoup4==4.12.3
+build==1.2.1
+certifi==2024.2.2
+charset-normalizer==3.3.2
+click==8.1.7
+colorama==0.4.6
+contourpy==1.2.1
+css-html-js-minify==2.5.5
+cycler==0.12.1
+distlib==0.3.8
+docutils==0.20.1
+editables==0.5
+filelock==3.13.4
+fonttools==4.51.0
+furo==2024.4.27
+h11==0.14.0
+hatch==1.9.7
+hatchling==1.21.1
+httpcore==1.0.5
+httpx==0.27.0
+hyperlink==21.0.0
+idna==3.7
+imagesize==1.4.1
+importlib_metadata==7.1.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
+Jinja2==3.1.3
+keyring==25.2.0
+kiwisolver==1.4.5
+lxml==5.2.1
+markdown-it-py==3.0.0
+MarkupSafe==2.1.5
+matplotlib==3.8.4
+mdurl==0.1.2
+more-itertools==10.2.0
+nh3==0.2.17
+numpy==1.26.4
+packaging==24.0
+pathspec==0.12.1
+pexpect==4.9.0
+pillow==10.3.0
+pkginfo==1.10.0
+platformdirs==4.2.1
+pluggy==1.5.0
+ptyprocess==0.7.0
+Pygments==2.17.2
+pyparsing==3.1.2
+pyproject_hooks==1.0.0
+python-dateutil==2.9.0.post0
+python-docs-theme==2024.4
+python-slugify==8.0.4
+pywin32-ctypes==0.2.2
+readme_renderer==43.0
+requests==2.31.0
+requests-toolbelt==1.0.0
+rfc3986==2.0.0
+rich==13.7.1
+shellingham==1.5.4
+six==1.16.0
+sniffio==1.3.1
+snowballstemmer==2.2.0
+soupsieve==2.5
+Sphinx==7.3.7
+sphinx-basic-ng==1.0.0b2
+sphinx-material==0.0.36
+sphinx-rtd-theme==2.0.0
+sphinxcontrib-applehelp==1.0.8
+sphinxcontrib-devhelp==1.0.6
+sphinxcontrib-htmlhelp==2.0.5
+sphinxcontrib-jquery==4.1
+sphinxcontrib-jsmath==1.0.1
+sphinxcontrib-qthelp==1.0.7
+sphinxcontrib-serializinghtml==1.1.10
+text-unidecode==1.3
+tomli_w==1.0.0
+tomlkit==0.12.4
+trove-classifiers==2024.4.10
+twine==5.0.0
+Unidecode==1.3.8
+urllib3==2.2.1
+userpath==1.9.2
+virtualenv==20.25.3
+zipp==3.18.1
+zstandard==0.22.0
```

### Comparing `kmeans_tjdwill-1.0.2/docs/Makefile` & `kmeans_tjdwill-1.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/docs/api-dev.rst` & `kmeans_tjdwill-1.0.3/docs/api-dev.rst`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-Developer API
-=============
-
-The following entries are all of the functions and classes developed for this
-package as submodules. The `source code <https://github.com/tjdwill/kmeans/tree/main/src/kmeans-tjdwill/kmeans>`_
-is available.
-
-kmeans.base\_funcs module
---------------------------
-
-.. automodule:: kmeans.base_funcs
-   :members:
-   :private-members:
-   :undoc-members:
-   :show-inheritance:
-
-
-kmeans.clustering module
---------------------------
-
-.. automodule:: kmeans.clustering
-   :members:
-   :private-members:
-   :undoc-members:
-   :show-inheritance:
-
-kmeans.animate module
---------------------------
-
-.. automodule:: kmeans.animate
-   :members:
-   :private-members:
-   :undoc-members:
-   :show-inheritance:
-
-
-kmeans.segmentation module
---------------------------
-
-.. automodule:: kmeans.segmentation
-   :members:
-   :private-members:
-   :undoc-members:
+Developer API
+=============
+
+The following entries are all of the functions and classes developed for this
+package as submodules. The `source code <https://github.com/tjdwill/kmeans/tree/main/src/kmeans-tjdwill/kmeans>`_
+is available.
+
+kmeans.base\_funcs module
+--------------------------
+
+.. automodule:: kmeans.base_funcs
+   :members:
+   :private-members:
+   :undoc-members:
+   :show-inheritance:
+
+
+kmeans.clustering module
+--------------------------
+
+.. automodule:: kmeans.clustering
+   :members:
+   :private-members:
+   :undoc-members:
+   :show-inheritance:
+
+kmeans.animate module
+--------------------------
+
+.. automodule:: kmeans.animate
+   :members:
+   :private-members:
+   :undoc-members:
+   :show-inheritance:
+
+
+kmeans.segmentation module
+--------------------------
+
+.. automodule:: kmeans.segmentation
+   :members:
+   :private-members:
+   :undoc-members:
    :show-inheritance:
```

### Comparing `kmeans_tjdwill-1.0.2/docs/conf.py` & `kmeans_tjdwill-1.0.3/docs/conf.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# Configuration file for the Sphinx documentation builder.
-#
-# For the full list of built-in configuration values, see the documentation:
-# https://www.sphinx-doc.org/en/master/usage/configuration.html
-
-# -- Project information -----------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information\
-
-# Add package to path
-from pathlib import Path
-import sys
-
-sys.path.insert(0, str(Path("../src/kmeans-tjdwill").resolve()))
-import kmeans
-
-project = 'K-Means Clustering'
-copyright = '2024, Terrance Williams (tjdwill)'
-author = 'Terrance Williams (tjdwill)'
-release = kmeans.__version__
-
-# -- General configuration ---------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
-
-extensions = [
-    "sphinx.ext.autodoc",
-    "sphinx.ext.napoleon"
-]
-
-templates_path = ['_templates']
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
-
-python_maximum_signature_line_length = 88
-
-
-# -- Options for HTML output -------------------------------------------------
-# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
-
-themes = {
-    "material": "sphinx_material",
-    "readthedocs": "sphinx_rtd_theme",
-    "furo": "furo",
-    "python": "python_docs_theme"
-}
-html_theme = themes['furo']
-html_static_path = ['_static']
-
+# Configuration file for the Sphinx documentation builder.
+#
+# For the full list of built-in configuration values, see the documentation:
+# https://www.sphinx-doc.org/en/master/usage/configuration.html
+
+# -- Project information -----------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information\
+
+# Add package to path
+from pathlib import Path
+import sys
+
+sys.path.insert(0, str(Path("../src/kmeans-tjdwill").resolve()))
+import kmeans
+
+project = 'K-Means Clustering'
+copyright = '2024, Terrance Williams (tjdwill)'
+author = 'Terrance Williams (tjdwill)'
+release = kmeans.__version__
+
+# -- General configuration ---------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
+
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.napoleon"
+]
+
+templates_path = ['_templates']
+exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+
+python_maximum_signature_line_length = 88
+
+
+# -- Options for HTML output -------------------------------------------------
+# https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
+
+themes = {
+    "material": "sphinx_material",
+    "readthedocs": "sphinx_rtd_theme",
+    "furo": "furo",
+    "python": "python_docs_theme"
+}
+html_theme = themes['furo']
+html_static_path = ['_static']
+
```

### Comparing `kmeans_tjdwill-1.0.2/docs/index.rst` & `kmeans_tjdwill-1.0.3/docs/index.rst`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-.. K-Means Clustering documentation master file, created by
-   sphinx-quickstart on Sat Apr 27 13:15:22 2024.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
-Welcome to K-Means Clustering's documentation!
-==============================================
-
-.. toctree::
-   :maxdepth: 2
-   :caption: Contents:
-
-   modules
-
-This is a package for easily performing k-means clustering on a set of data. 
-Unique to this implementation is its ability to specify the dimension up to
-which the data is clustered. For example::
-
-   >>> from kmeans import cluster
-   >>> import numpy as np
-   >>> np.random.seed(27)   # For reproducible results
-   >>> data = np.random.random((15, 5)).round(3)
-   >>> data[0]
-   array([0.426, 0.815, 0.735, 0.868, 0.383])
-   >>> # Cluster using only first two dimensions
-   >>> clusters, centroids = cluster(data, k=3, ndim=2, tolerance=0.001)
-   >>> centroids
-   array([[0.9004, 0.79  ],
-       [0.5795, 0.3995],
-       [0.254 , 0.6325]])
-   >>> clusters  # visually compare centroids with first two elements of each data entry.
-   {0: array([[0.979, 0.893, 0.21 , 0.742, 0.663],
-        [0.887, 0.858, 0.749, 0.87 , 0.187],
-        [0.966, 0.583, 0.092, 0.014, 0.837],
-        [0.915, 0.705, 0.387, 0.706, 0.923],
-        [0.755, 0.911, 0.242, 0.976, 0.304]]),
-    1: array([[0.326, 0.373, 0.794, 0.151, 0.17 ],
-        [0.701, 0.181, 0.599, 0.415, 0.514],
-        [0.477, 0.493, 0.595, 0.076, 0.117],
-        [0.489, 0.596, 0.264, 0.992, 0.21 ],
-        [0.583, 0.649, 0.911, 0.122, 0.676],
-        [0.901, 0.105, 0.673, 0.87 , 0.561]]),
-    2: array([[0.426, 0.815, 0.735, 0.868, 0.383],
-        [0.081, 0.305, 0.783, 0.163, 0.071],
-        [0.221, 0.726, 0.849, 0.929, 0.736],
-        [0.288, 0.684, 0.52 , 0.877, 0.924]])}
-
-Installation
-============
-
-The package can be installed via `PyPI <https://pypi.org/project/kmeans-tjdwill/>`_:
-
-.. code-block:: console
-
-   $ pip install kmeans-tjdwill
-
-Issues
-======
-
-Create an issue on the `GitHub page <https://github.com/tjdwill/kmeans/issues>`_.
-Please be civil, professional, and kind.
-
-License
-=======
-
-This work is licensed under the `MIT License <https://github.com/tjdwill/kmeans/blob/main/LICENSE>`_.
-
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+.. K-Means Clustering documentation master file, created by
+   sphinx-quickstart on Sat Apr 27 13:15:22 2024.
+   You can adapt this file completely to your liking, but it should at least
+   contain the root `toctree` directive.
+
+Welcome to K-Means Clustering's documentation!
+==============================================
+
+.. toctree::
+   :maxdepth: 2
+   :caption: Contents:
+
+   modules
+
+This is a package for easily performing k-means clustering on a set of data. 
+Unique to this implementation is its ability to specify the dimension up to
+which the data is clustered. For example::
+
+   >>> from kmeans import cluster
+   >>> import numpy as np
+   >>> np.random.seed(27)   # For reproducible results
+   >>> data = np.random.random((15, 5)).round(3)
+   >>> data[0]
+   array([0.426, 0.815, 0.735, 0.868, 0.383])
+   >>> # Cluster using only first two dimensions
+   >>> clusters, centroids = cluster(data, k=3, ndim=2, tolerance=0.001)
+   >>> centroids
+   array([[0.9004, 0.79  ],
+       [0.5795, 0.3995],
+       [0.254 , 0.6325]])
+   >>> clusters  # visually compare centroids with first two elements of each data entry.
+   {0: array([[0.979, 0.893, 0.21 , 0.742, 0.663],
+        [0.887, 0.858, 0.749, 0.87 , 0.187],
+        [0.966, 0.583, 0.092, 0.014, 0.837],
+        [0.915, 0.705, 0.387, 0.706, 0.923],
+        [0.755, 0.911, 0.242, 0.976, 0.304]]),
+    1: array([[0.326, 0.373, 0.794, 0.151, 0.17 ],
+        [0.701, 0.181, 0.599, 0.415, 0.514],
+        [0.477, 0.493, 0.595, 0.076, 0.117],
+        [0.489, 0.596, 0.264, 0.992, 0.21 ],
+        [0.583, 0.649, 0.911, 0.122, 0.676],
+        [0.901, 0.105, 0.673, 0.87 , 0.561]]),
+    2: array([[0.426, 0.815, 0.735, 0.868, 0.383],
+        [0.081, 0.305, 0.783, 0.163, 0.071],
+        [0.221, 0.726, 0.849, 0.929, 0.736],
+        [0.288, 0.684, 0.52 , 0.877, 0.924]])}
+
+Installation
+============
+
+The package can be installed via `PyPI <https://pypi.org/project/kmeans-tjdwill/>`_:
+
+.. code-block:: console
+
+   $ pip install kmeans-tjdwill
+
+Issues
+======
+
+Create an issue on the `GitHub page <https://github.com/tjdwill/kmeans/issues>`_.
+Please be civil, professional, and kind.
+
+License
+=======
+
+This work is licensed under the `MIT License <https://github.com/tjdwill/kmeans/blob/main/LICENSE>`_.
+
+Indices and tables
+==================
+
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
```

### Comparing `kmeans_tjdwill-1.0.2/docs/make.bat` & `kmeans_tjdwill-1.0.3/docs/make.bat`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-@ECHO OFF
-
-pushd %~dp0
-
-REM Command file for Sphinx documentation
-
-if "%SPHINXBUILD%" == "" (
-	set SPHINXBUILD=sphinx-build
-)
-set SOURCEDIR=.
-set BUILDDIR=_build
-
-%SPHINXBUILD% >NUL 2>NUL
-if errorlevel 9009 (
-	echo.
-	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
-	echo.installed, then set the SPHINXBUILD environment variable to point
-	echo.to the full path of the 'sphinx-build' executable. Alternatively you
-	echo.may add the Sphinx directory to PATH.
-	echo.
-	echo.If you don't have Sphinx installed, grab it from
-	echo.https://www.sphinx-doc.org/
-	exit /b 1
-)
-
-if "%1" == "" goto help
-
-%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-goto end
-
-:help
-%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
-
-:end
-popd
+@ECHO OFF
+
+pushd %~dp0
+
+REM Command file for Sphinx documentation
+
+if "%SPHINXBUILD%" == "" (
+	set SPHINXBUILD=sphinx-build
+)
+set SOURCEDIR=.
+set BUILDDIR=_build
+
+%SPHINXBUILD% >NUL 2>NUL
+if errorlevel 9009 (
+	echo.
+	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
+	echo.installed, then set the SPHINXBUILD environment variable to point
+	echo.to the full path of the 'sphinx-build' executable. Alternatively you
+	echo.may add the Sphinx directory to PATH.
+	echo.
+	echo.If you don't have Sphinx installed, grab it from
+	echo.https://www.sphinx-doc.org/
+	exit /b 1
+)
+
+if "%1" == "" goto help
+
+%SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+goto end
+
+:help
+%SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
+
+:end
+popd
```

### Comparing `kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/animate.py` & `kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/animate.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/base_funcs.py` & `kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/base_funcs.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/clustering.py` & `kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/clustering.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/src/kmeans-tjdwill/kmeans/segmentation.py` & `kmeans_tjdwill-1.0.3/src/kmeans-tjdwill/kmeans/segmentation.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/test_assign_cluster.py` & `kmeans_tjdwill-1.0.3/tests/test_assign_cluster.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/test_clustering.py` & `kmeans_tjdwill-1.0.3/tests/test_clustering.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/test_datavalidation.py` & `kmeans_tjdwill-1.0.3/tests/test_datavalidation.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/test_distances.py` & `kmeans_tjdwill-1.0.3/tests/test_distances.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/test_segmentation.py` & `kmeans_tjdwill-1.0.3/tests/test_segmentation.py`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/output/seg_groups04.jpg` & `kmeans_tjdwill-1.0.3/tests/output/seg_groups04.jpg`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/output/seg_groups10.jpg` & `kmeans_tjdwill-1.0.3/tests/output/seg_groups10.jpg`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/output/seg_rand_groups04.jpg` & `kmeans_tjdwill-1.0.3/tests/output/seg_rand_groups04.jpg`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/tests/output/seg_rand_groups10.jpg` & `kmeans_tjdwill-1.0.3/tests/output/seg_rand_groups10.jpg`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/README.md` & `kmeans_tjdwill-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # K-Means Clustering
 
+[![PyPI version](https://badge.fury.io/py/kmeans-tjdwill.svg)](https://badge.fury.io/py/kmeans-tjdwill)
+[![Docs](https://github.com/tjdwill/kmeans/actions/workflows/sitebuild.yml/badge.svg)](https://tjdwill.github.io/kmeans) 
+
 
 A repository documenting the implementation of k-Means clustering in Python. Usage examples can be found in the `tests` directory.
 
 
 The thing that makes this k-means clustering module different from others is that it allows the user to specify the number of dimensions to use for the clustering operation.
 
 For example, given some data where each element is of form
```

### Comparing `kmeans_tjdwill-1.0.2/pyproject.toml` & `kmeans_tjdwill-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kmeans_tjdwill-1.0.2/PKG-INFO` & `kmeans_tjdwill-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kmeans-tjdwill
-Version: 1.0.2
+Version: 1.0.3
 Summary: A function-based implementation of k-means clustering that maintains data association.
 Project-URL: Homepage, https://github.com/tjdwill/kmeans
 Project-URL: Issues, https://github.com/tjdwill/kmeans/issues
 Author-email: Terrance Williams <tjdwill.gh@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 tjdwill
@@ -38,14 +38,17 @@
 Requires-Python: >=3.9
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Description-Content-Type: text/markdown
 
 # K-Means Clustering
 
+[![PyPI version](https://badge.fury.io/py/kmeans-tjdwill.svg)](https://badge.fury.io/py/kmeans-tjdwill)
+[![Docs](https://github.com/tjdwill/kmeans/actions/workflows/sitebuild.yml/badge.svg)](https://tjdwill.github.io/kmeans) 
+
 
 A repository documenting the implementation of k-Means clustering in Python. Usage examples can be found in the `tests` directory.
 
 
 The thing that makes this k-means clustering module different from others is that it allows the user to specify the number of dimensions to use for the clustering operation.
 
 For example, given some data where each element is of form
```

