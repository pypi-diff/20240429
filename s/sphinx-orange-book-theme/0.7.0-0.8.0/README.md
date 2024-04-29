# Comparing `tmp/sphinx_orange_book_theme-0.7.0.tar.gz` & `tmp/sphinx_orange_book_theme-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_orange_book_theme-0.7.0.tar", max compression
+gzip compressed data, was "sphinx_orange_book_theme-0.8.0.tar", max compression
```

## Comparing `sphinx_orange_book_theme-0.7.0.tar` & `sphinx_orange_book_theme-0.8.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-03-15 17:28:43.653336 sphinx_orange_book_theme-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0     1812 2024-03-15 17:28:43.653336 sphinx_orange_book_theme-0.7.0/README.md
--rw-r--r--   0        0        0     2006 2024-03-15 17:28:43.656336 sphinx_orange_book_theme-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      365 2024-03-15 17:28:43.657336 sphinx_orange_book_theme-0.7.0/sphinx_orange_book_theme/__init__.py
--rw-r--r--   0        0        0     2691 2024-03-15 17:28:43.657336 sphinx_orange_book_theme-0.7.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme-colors.css
--rw-r--r--   0        0        0     1216 2024-03-15 17:28:43.657336 sphinx_orange_book_theme-0.7.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme.css
--rw-r--r--   0        0        0       85 2024-03-15 17:28:43.657336 sphinx_orange_book_theme-0.7.0/sphinx_orange_book_theme/theme.conf
--rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 sphinx_orange_book_theme-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-29 16:23:42.134320 sphinx_orange_book_theme-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     1812 2024-04-29 16:23:42.134320 sphinx_orange_book_theme-0.8.0/README.md
+-rw-r--r--   0        0        0     2008 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      365 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/__init__.py
+-rw-r--r--   0        0        0     2691 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme-colors.css
+-rw-r--r--   0        0        0     1216 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme.css
+-rw-r--r--   0        0        0       85 2024-04-29 16:23:42.137320 sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/theme.conf
+-rw-r--r--   0        0        0     3065 1970-01-01 00:00:00.000000 sphinx_orange_book_theme-0.8.0/PKG-INFO
```

### Comparing `sphinx_orange_book_theme-0.7.0/LICENSE.txt` & `sphinx_orange_book_theme-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sphinx_orange_book_theme-0.7.0/README.md` & `sphinx_orange_book_theme-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinx_orange_book_theme-0.7.0/pyproject.toml` & `sphinx_orange_book_theme-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinx-orange-book-theme"
-version = "0.7.0"
+version = "0.8.0"
 description = "An orange version of sphinx-book-theme."
 authors = ["Kenta Kabashima <kenta_program37@hotmail.co.jp>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/MusicScience37Projects/utility-libraries/sphinx-orange-book-theme"
 documentation = "https://sphinx-orange-book-theme-musicscience37projects--1dc46f9ab80e60.gitlab.io/"
 repository = "https://gitlab.com/MusicScience37Projects/utility-libraries/sphinx-orange-book-theme.git"
@@ -20,43 +20,43 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Documentation :: Sphinx",
     "Topic :: Software Development :: Documentation",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.10,<3.13"
 sphinx-book-theme = ">=1"
 pydata-sphinx-theme = ">=0.14"
 sphinx = ">=6"
 
 [tool.poetry.group.dev.dependencies]
-pre-commit = "^3.6.2"
-black = "^24.2.0"
+pre-commit = "^3.7.0"
+black = "^24.4.2"
 isort = "^5.13.2"
 opencv-python-headless = "^4.9.0.80"
 numpy = "^1.26.4"
 jinja2 = "^3.1.3"
 
 [tool.poetry.group.doc.dependencies]
 toml = "^0.10.2"
 types-toml = "^0.10.8.20240310"
-sphinx-autobuild = "^2024.2.4"
-myst-parser = "^2.0.0"
+sphinx-autobuild = "^2024.4.16"
+myst-parser = "^3.0.1"
 doc8 = "^1.1.1"
 
 [tool.poetry.group.test.dependencies]
 breathe = "^4.35.0"
-myst-nb = "^1.0.0"
-jupyterlab = "^4.1.5"
+myst-nb = "^1.1.0"
+jupyterlab = "^4.1.8"
 ipywidgets = "^8.1.2"
-ipython = "^8.18.1"
-ipykernel = "^6.29.3"
-plotly = "^5.20.0"
-pandas = "^2.2.1"
+ipython = "^8.24.0"
+ipykernel = "^6.29.4"
+plotly = "^5.21.0"
+pandas = "^2.2.2"
 sphinxext-opengraph = "^0.9.1"
 sphinxcontrib-plantuml = "^0.29"
 sphinxcontrib-bibtex = "^2.6.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sphinx_orange_book_theme-0.7.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme-colors.css` & `sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme-colors.css`

 * *Files 10% similar despite different names*

```diff
@@ -7,70 +7,70 @@
  *************************************************************************** */
 
 /* ****************************************************************************
  * Colors
  *************************************************************************** */
 html[data-theme="light"] {
   /* teal in the original theme */
-  --pst-color-primary: #df671f;
-  --pst-color-primary-bg: #ffe9dd;
+  --pst-color-primary: #d66d32;
+  --pst-color-primary-bg: #fee9e0;
   /* violet in the original theme */
-  --pst-color-secondary: #a58713;
-  --pst-color-secondary-bg: #fcecca;
+  --pst-color-secondary: #a68715;
+  --pst-color-secondary-bg: #ffebbc;
   /* pink in the original theme */
   --pst-color-accent: #379f14;
   --pst-color-accent-bg: #e2f2d9;
   /* gray in the original theme */
   --pst-color-background: white;
   --pst-color-on-background: white;
-  --pst-color-surface: #fff4ee;
-  --pst-color-on-surface: #41210f;
-  --pst-color-text-base: #2c2927;
-  --pst-color-text-muted: #7a6e69;
-  --pst-color-border: #c3bbb7;
-  --pst-color-border-muted: #d8d3d0;
+  --pst-color-surface: #fef4ef;
+  --pst-color-on-surface: #3f2213;
+  --pst-color-text-base: #2d2826;
+  --pst-color-text-muted: #7e6d65;
+  --pst-color-border: #c6bab4;
+  --pst-color-border-muted: #dad3cf;
   /* info, warning, success, danger */
   --pst-color-info: #379f14;
   --pst-color-info-bg: #e2f2d9;
-  --pst-color-warning: #df671f;
-  --pst-color-warning-bg: #ffe9dd;
+  --pst-color-warning: #a68715;
+  --pst-color-warning-bg: #ffebbc;
   --pst-color-success: #379f14;
   --pst-color-success-bg: #e2f2d9;
   --pst-color-danger: #d2304e;
   --pst-color-danger-bg: #fee8e8;
   /* inline code */
-  --pst-color-inline-code-links: #b75316;
+  --pst-color-inline-code-links: #b15725;
   --pst-color-inline-code: #2a6416;
 }
 
 html[data-theme="dark"] {
   /* teal in the original theme */
-  --pst-color-primary: #ee8b54;
-  --pst-color-primary-bg: #41210f;
+  --pst-color-primary: #e68f60;
+  --pst-color-primary-bg: #633319;
   /* violet in the original theme */
-  --pst-color-secondary: #c4a10d;
-  --pst-color-secondary-bg: #312910;
+  --pst-color-secondary: #e1b809;
+  --pst-color-secondary-bg: #4c3e14;
   /* pink in the original theme */
   --pst-color-accent: #59b937;
-  --pst-color-accent-bg: #192f11;
+  --pst-color-accent-bg: #224814;
   /* gray in the original theme */
-  --pst-color-background: #161514;
-  --pst-color-on-background: #2c2927;
-  --pst-color-surface: #41210f;
-  --pst-color-on-surface: #ffe9dd;
-  --pst-color-text-base: #efedec;
-  --pst-color-text-muted: #c3bbb7;
-  --pst-color-border: #7a6e69;
-  --pst-color-border-muted: #5f5652;
+  --pst-color-background: #171514;
+  --pst-color-on-background: #2d2826;
+  --pst-color-surface: #2d2826;
+  --pst-color-on-surface: #f0eceb;
+  --pst-color-text-base: #f7f6f5;
+  --pst-color-text-muted: #c6bab4;
+  --pst-color-border: #7e6d65;
+  --pst-color-border-muted: #61554f;
   /* info, warning, success, danger */
-  --pst-color-info: #59b937;
-  --pst-color-info-bg: #192f11;
-  --pst-color-warning: #ee8b54;
-  --pst-color-warning-bg: #41210f;
+  --pst-color-info: #379f14;
+  --pst-color-info-bg: #224814;
+  --pst-color-warning: #e1b809;
+  --pst-color-warning-bg: #4c3e14;
   --pst-color-success: #59b937;
-  --pst-color-success-bg: #192f11;
-  --pst-color-danger: #ec888d;
+  --pst-color-success-bg: #224814;
+  --pst-color-danger: #e0616d;
   --pst-color-danger-bg: #4e151d;
   /* inline code */
-  --pst-color-inline-code-links: #ee8b54;
+  --pst-color-inline-code-links: #e68f60;
   --pst-color-inline-code: #59b937;
 }
```

### Comparing `sphinx_orange_book_theme-0.7.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme.css` & `sphinx_orange_book_theme-0.8.0/sphinx_orange_book_theme/static/styles/sphinx-orange-book-theme.css`

 * *Files identical despite different names*

### Comparing `sphinx_orange_book_theme-0.7.0/PKG-INFO` & `sphinx_orange_book_theme-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: sphinx-orange-book-theme
-Version: 0.7.0
+Version: 0.8.0
 Summary: An orange version of sphinx-book-theme.
 Home-page: https://gitlab.com/MusicScience37Projects/utility-libraries/sphinx-orange-book-theme
 License: MIT
 Keywords: sphinx
 Author: Kenta Kabashima
 Author-email: kenta_program37@hotmail.co.jp
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: pydata-sphinx-theme (>=0.14)
 Requires-Dist: sphinx (>=6)
 Requires-Dist: sphinx-book-theme (>=1)
 Project-URL: Documentation, https://sphinx-orange-book-theme-musicscience37projects--1dc46f9ab80e60.gitlab.io/
 Project-URL: Repository, https://gitlab.com/MusicScience37Projects/utility-libraries/sphinx-orange-book-theme.git
```

