# Comparing `tmp/ngstoolkits-0.0.0rc1.tar.gz` & `tmp/ngstoolkits-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/liubo/git_sync/ngstools/dist/.tmp-1dis9eim/ngstoolkits-0.0.0rc1.tar", last modified: Tue Apr 23 02:38:55 2024, max compression
+gzip compressed data, was "/Users/liubo/git_sync/ngstoolkits/dist/.tmp-9t8w5zie/ngstoolkits-1.0.0rc1.tar", last modified: Mon Apr 29 06:59:22 2024, max compression
```

## Comparing `ngstoolkits-0.0.0rc1.tar` & `ngstoolkits-1.0.0rc1.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-23 02:38:55.619184 ngstoolkits-0.0.0rc1/
--rw-r--r--   0 liubo      (501) staff       (20)      591 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/.coveragerc
--rw-r--r--   0 liubo      (501) staff       (20)      566 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/.gitignore
--rw-r--r--   0 liubo      (501) staff       (20)      530 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/.readthedocs.yml
--rw-r--r--   0 liubo      (501) staff       (20)       80 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/AUTHORS.md
--rw-r--r--   0 liubo      (501) staff       (20)      115 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/CHANGELOG.md
--rw-r--r--   0 liubo      (501) staff       (20)    13490 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0 liubo      (501) staff       (20)     1084 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/LICENSE.txt
--rw-r--r--   0 liubo      (501) staff       (20)     2105 2024-04-23 02:38:55.618768 ngstoolkits-0.0.0rc1/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)     1326 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/README.md
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-23 02:38:55.587367 ngstoolkits-0.0.0rc1/docs/
--rw-r--r--   0 liubo      (501) staff       (20)     1154 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/Makefile
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-23 02:38:55.588400 ngstoolkits-0.0.0rc1/docs/_static/
--rw-r--r--   0 liubo      (501) staff       (20)       18 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/_static/.gitignore
--rw-r--r--   0 liubo      (501) staff       (20)       71 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/authors.md
--rw-r--r--   0 liubo      (501) staff       (20)       73 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/changelog.md
--rw-r--r--   0 liubo      (501) staff       (20)    10039 2024-04-22 07:54:20.000000 ngstoolkits-0.0.0rc1/docs/conf.py
--rw-r--r--   0 liubo      (501) staff       (20)       76 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/contributing.md
--rw-r--r--   0 liubo      (501) staff       (20)      953 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/index.md
--rw-r--r--   0 liubo      (501) staff       (20)       66 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/license.md
--rw-r--r--   0 liubo      (501) staff       (20)       70 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/readme.md
--rw-r--r--   0 liubo      (501) staff       (20)      254 2024-04-02 09:40:50.000000 ngstoolkits-0.0.0rc1/docs/requirements.txt
--rw-r--r--   0 liubo      (501) staff       (20)      346 2024-04-22 08:12:01.000000 ngstoolkits-0.0.0rc1/pyproject.toml
--rw-r--r--   0 liubo      (501) staff       (20)     1335 2024-04-23 02:38:55.621855 ngstoolkits-0.0.0rc1/setup.cfg
--rw-r--r--   0 liubo      (501) staff       (20)      475 2024-04-23 02:37:43.000000 ngstoolkits-0.0.0rc1/setup.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-23 02:38:55.552598 ngstoolkits-0.0.0rc1/src/
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-23 02:38:55.594676 ngstoolkits-0.0.0rc1/src/ngstoolkits/
--rw-r--r--   0 liubo      (501) staff       (20)      477 2024-04-23 02:38:33.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits/__init__.py
--rw-r--r--   0 liubo      (501) staff       (20)      811 2024-04-23 02:24:04.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits/ngs_class.py
--rw-r--r--   0 liubo      (501) staff       (20)     4193 2024-04-22 08:26:47.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits/skeleton.py
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-23 02:38:55.609600 ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/
--rw-r--r--   0 liubo      (501) staff       (20)     2105 2024-04-23 02:38:55.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/PKG-INFO
--rw-r--r--   0 liubo      (501) staff       (20)      653 2024-04-23 02:38:55.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/SOURCES.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-23 02:38:55.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/dependency_links.txt
--rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-23 02:38:55.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/not-zip-safe
--rw-r--r--   0 liubo      (501) staff       (20)       86 2024-04-23 02:38:55.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/requires.txt
--rw-r--r--   0 liubo      (501) staff       (20)       12 2024-04-23 02:38:55.000000 ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/top_level.txt
-drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-23 02:38:55.608288 ngstoolkits-0.0.0rc1/tests/
--rw-r--r--   0 liubo      (501) staff       (20)      673 2024-04-23 02:26:24.000000 ngstoolkits-0.0.0rc1/tests/test_class.py
--rw-r--r--   0 liubo      (501) staff       (20)     2854 2024-04-22 08:41:28.000000 ngstoolkits-0.0.0rc1/tox.ini
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.383310 ngstoolkits-1.0.0rc1/
+-rw-r--r--   0 liubo      (501) staff       (20)      594 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/.coveragerc
+-rw-r--r--   0 liubo      (501) staff       (20)      566 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/.gitignore
+-rw-r--r--   0 liubo      (501) staff       (20)      530 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/.readthedocs.yml
+-rw-r--r--   0 liubo      (501) staff       (20)       80 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/AUTHORS.md
+-rw-r--r--   0 liubo      (501) staff       (20)      115 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/CHANGELOG.md
+-rw-r--r--   0 liubo      (501) staff       (20)    13529 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 liubo      (501) staff       (20)     1084 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/LICENSE.txt
+-rw-r--r--   0 liubo      (501) staff       (20)     1973 2024-04-29 06:59:22.383063 ngstoolkits-1.0.0rc1/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)     1323 2024-04-29 06:03:51.000000 ngstoolkits-1.0.0rc1/README.md
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.370253 ngstoolkits-1.0.0rc1/docs/
+-rw-r--r--   0 liubo      (501) staff       (20)     1154 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/Makefile
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.371210 ngstoolkits-1.0.0rc1/docs/_static/
+-rw-r--r--   0 liubo      (501) staff       (20)       18 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/_static/.gitignore
+-rw-r--r--   0 liubo      (501) staff       (20)       71 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/authors.md
+-rw-r--r--   0 liubo      (501) staff       (20)       73 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/changelog.md
+-rw-r--r--   0 liubo      (501) staff       (20)    10054 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/conf.py
+-rw-r--r--   0 liubo      (501) staff       (20)       76 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/contributing.md
+-rw-r--r--   0 liubo      (501) staff       (20)      956 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/index.md
+-rw-r--r--   0 liubo      (501) staff       (20)       66 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/license.md
+-rw-r--r--   0 liubo      (501) staff       (20)       70 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/docs/readme.md
+-rw-r--r--   0 liubo      (501) staff       (20)      254 2024-04-29 06:45:11.000000 ngstoolkits-1.0.0rc1/docs/requirements.txt
+-rw-r--r--   0 liubo      (501) staff       (20)      354 2024-04-29 06:52:27.000000 ngstoolkits-1.0.0rc1/pyproject.toml
+-rw-r--r--   0 liubo      (501) staff       (20)     1225 2024-04-29 06:59:22.385547 ngstoolkits-1.0.0rc1/setup.cfg
+-rw-r--r--   0 liubo      (501) staff       (20)      982 2024-04-29 06:21:59.000000 ngstoolkits-1.0.0rc1/setup.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.353069 ngstoolkits-1.0.0rc1/src/
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.374088 ngstoolkits-1.0.0rc1/src/ngstoolkits/
+-rw-r--r--   0 liubo      (501) staff       (20)      373 2024-04-29 06:59:08.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits/__init__.py
+-rw-r--r--   0 liubo      (501) staff       (20)    10740 2024-04-29 06:17:19.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits/ngs_class.py
+-rw-r--r--   0 liubo      (501) staff       (20)      725 2024-04-29 06:45:25.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits/sequence.py
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.381195 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/
+-rw-r--r--   0 liubo      (501) staff       (20)     1973 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/PKG-INFO
+-rw-r--r--   0 liubo      (501) staff       (20)      671 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/SOURCES.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/dependency_links.txt
+-rw-r--r--   0 liubo      (501) staff       (20)        1 2024-04-29 06:53:14.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/not-zip-safe
+-rw-r--r--   0 liubo      (501) staff       (20)       86 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/requires.txt
+-rw-r--r--   0 liubo      (501) staff       (20)       12 2024-04-29 06:59:22.000000 ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/top_level.txt
+drwxr-xr-x   0 liubo      (501) staff       (20)        0 2024-04-29 06:59:22.380163 ngstoolkits-1.0.0rc1/tests/
+-rw-r--r--   0 liubo      (501) staff       (20)      279 2024-04-23 06:02:43.000000 ngstoolkits-1.0.0rc1/tests/conftest.py
+-rw-r--r--   0 liubo      (501) staff       (20)      738 2024-04-29 06:03:05.000000 ngstoolkits-1.0.0rc1/tests/test_class.py
+-rw-r--r--   0 liubo      (501) staff       (20)     2861 2024-04-29 06:44:15.000000 ngstoolkits-1.0.0rc1/tox.ini
```

### Comparing `ngstoolkits-0.0.0rc1/.coveragerc` & `ngstoolkits-1.0.0rc1/.coveragerc`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # .coveragerc to control coverage.py
 [run]
 branch = True
-source = ngstools
+source = ngstoolkits
 # omit = bad_file.py
 
 [paths]
 source =
     src/
     */site-packages/
```

### Comparing `ngstoolkits-0.0.0rc1/.gitignore` & `ngstoolkits-1.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `ngstoolkits-0.0.0rc1/.readthedocs.yml` & `ngstoolkits-1.0.0rc1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ngstoolkits-0.0.0rc1/CONTRIBUTING.md` & `ngstoolkits-1.0.0rc1/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
    this template, but there are a few extra contents that you might decide to
    also include, like mentioning labels of your issue tracker or automated
    releases.
 ```
 
 # Contributing
 
-Welcome to `ngstools` contributor's guide.
+Welcome to `ngstoolkits` contributor's guide.
 
 This document focuses on getting any potential contributor familiarized with
 the development processes, but [other kinds of contributions] are also appreciated.
 
 If you are new to using [git] or have never collaborated in a project previously,
 please have a look at [contribution-guide.org]. Other resources are also
 listed in the excellent [guide created by FreeCodeCamp] [^contrib1].
@@ -39,15 +39,15 @@
 Please notice, all users and contributors are expected to be **open,
 considerate, reasonable, and respectful**. When in doubt,
 [Python Software Foundation's Code of Conduct] is a good reference in terms of
 behavior guidelines.
 
 ## Issue Reports
 
-If you experience bugs or general issues with `ngstools`, please have a look
+If you experience bugs or general issues with `ngstoolkits`, please have a look
 on the [issue tracker].
 If you don't see anything useful there, please feel free to fire an issue report.
 
 :::{tip}
 Please don't forget to include the closed issues in your search.
 Sometimes a solution was already reported, and the problem is considered
 **solved**.
@@ -57,31 +57,31 @@
 (e.g., operating system, Python version) and steps to reproduce the problem.
 Please try also to simplify the reproduction steps to a very minimal example
 that still illustrates the problem you are facing. By removing other factors,
 you help us to identify the root cause of the issue.
 
 ## Documentation Improvements
 
-You can help improve `ngstools` docs by making them more readable and coherent, or
+You can help improve `ngstoolkits` docs by making them more readable and coherent, or
 by adding missing information and correcting mistakes.
 
-`ngstools` documentation uses [Sphinx] as its main documentation compiler.
+`ngstoolkits` documentation uses [Sphinx] as its main documentation compiler.
 This means that the docs are kept in the same repository as the project code, and
 that any documentation update is done in the same way was a code contribution.
 
 ```{todo} Don't forget to mention which markup language you are using.
 
     e.g.,  [reStructuredText] or [CommonMark] with [MyST] extensions.
 ```
 
 ```{todo} If your project is hosted on GitHub, you can also mention the following tip:
 
    :::{tip}
       Please notice that the [GitHub web interface] provides a quick way of
-      propose changes in `ngstools`'s files. While this mechanism can
+      propose changes in `ngstoolkits`'s files. While this mechanism can
       be tricky for normal code contributions, it works perfectly fine for
       contributing to the docs, and can be quite handy.
 
       If you are interested in trying this method out, please navigate to
       the `docs` folder in the source [repository], find which file you
       would like to propose changes and click in the little pencil icon at the
       top, to open [GitHub's code editor]. Once you finish editing the file,
@@ -130,30 +130,30 @@
 virtualenv <PATH TO VENV>
 source <PATH TO VENV>/bin/activate
 ```
 
 or [Miniconda]:
 
 ```
-conda create -n ngstools python=3 six virtualenv pytest pytest-cov
-conda activate ngstools
+conda create -n ngstoolkits python=3 six virtualenv pytest pytest-cov
+conda activate ngstoolkits
 ```
 
 ### Clone the repository
 
 1. Create an user account on GitHub if you do not already have one.
 
 2. Fork the project [repository]: click on the *Fork* button near the top of the
    page. This creates a copy of the code under your account on GitHub.
 
 3. Clone this copy to your local disk:
 
    ```
-   git clone git@github.com:YourLogin/ngstools.git
-   cd ngstools
+   git clone git@github.com:YourLogin/ngstoolkits.git
+   cd ngstoolkits
    ```
 
 4. You should run:
 
    ```
    pip install -U pip setuptools -e .
    ```
@@ -166,15 +166,15 @@
 5. Install [pre-commit]:
 
    ```
    pip install pre-commit
    pre-commit install
    ```
 
-   `ngstools` comes with a lot of hooks configured to automatically help the
+   `ngstoolkits` comes with a lot of hooks configured to automatically help the
    developer to check the code being written.
 
 ### Implement your changes
 
 1. Create a branch to hold your changes:
 
    ```
@@ -310,15 +310,15 @@
 
    If instead you are using a different/private package index, please update
    the instructions accordingly.
 ```
 
 If you are part of the group of maintainers and have correct user permissions
 on [PyPI], the following steps can be used to release a new version for
-`ngstools`:
+`ngstoolkits`:
 
 1. Make sure all unit tests are successful.
 2. Tag the current commit on the main branch with a release tag, e.g., `v1.2.3`.
 3. Push the new tag to the upstream [repository],
    e.g., `git push upstream v1.2.3`
 4. Clean up the `dist` and `build` folders with `tox -e clean`
    (or `rm -rf dist build`)
@@ -363,9 +363,9 @@
 [virtual environment]: https://realpython.com/python-virtual-environments-a-primer/
 [virtualenv]: https://virtualenv.pypa.io/en/stable/
 
 
 ```{todo} Please review and change the following definitions:
 ```
 
-[repository]: https://github.com/<USERNAME>/ngstools
-[issue tracker]: https://github.com/<USERNAME>/ngstools/issues
+[repository]: https://github.com/<USERNAME>/ngstoolkits
+[issue tracker]: https://github.com/<USERNAME>/ngstoolkits/issues
```

### Comparing `ngstoolkits-0.0.0rc1/LICENSE.txt` & `ngstoolkits-1.0.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ngstoolkits-0.0.0rc1/PKG-INFO` & `ngstoolkits-1.0.0rc1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ngstoolkits
-Version: 0.0.0rc1
+Version: 1.0.0rc1
 Summary: ngstools
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Liubo
 Author-email: 614347533@qq.com
 License: MIT
-Project-URL: Documentation, https://github.com/Ben-unbelieveable/python_package_ngstools/README.md
-Project-URL: Source, https://github.com/Ben-unbelieveable/python_package_ngstools
+Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: testing
@@ -31,18 +30,20 @@
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/ngstools)
 -->
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # ngstools
 
-> Add a short description here!
+> Useful toolkits for NGS analysis
 
-A longer description of your project goes here...
+## Main Class
+### mutation
 
+## Main Function
 
 <!-- pyscaffold-notes -->
 
 ## Note
 
 This project has been set up using PyScaffold 4.5. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `ngstoolkits-0.0.0rc1/README.md` & `ngstoolkits-1.0.0rc1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/ngstools)
 -->
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # ngstools
 
-> Add a short description here!
+> Useful toolkits for NGS analysis
 
-A longer description of your project goes here...
+## Main Class
+### mutation
 
+## Main Function
 
 <!-- pyscaffold-notes -->
 
 ## Note
 
 This project has been set up using PyScaffold 4.5. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `ngstoolkits-0.0.0rc1/docs/Makefile` & `ngstoolkits-1.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ngstoolkits-0.0.0rc1/docs/conf.py` & `ngstoolkits-1.0.0rc1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 try:  # for Sphinx >= 1.7
     from sphinx.ext import apidoc
 except ImportError:
     from sphinx import apidoc
 
 output_dir = os.path.join(__location__, "api")
-module_dir = os.path.join(__location__, "../src/ngstools")
+module_dir = os.path.join(__location__, "../src/ngstoolkits")
 try:
     shutil.rmtree(output_dir)
 except FileNotFoundError:
     pass
 
 try:
     import sphinx
@@ -101,27 +101,27 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
-project = "ngstools"
+project = "ngstoolkits"
 copyright = "2024, Ben-unbelieveable"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # version: The short X.Y version.
 # release: The full version, including alpha/beta/rc tags.
 # If you don’t need the separation provided between version and release,
 # just set them both to the same value.
 try:
-    from ngstools import __version__ as version
+    from ngstoolkits import __version__ as version
 except ImportError:
     version = ""
 
 if not version or version.lower() == "unknown":
     version = os.getenv("READTHEDOCS_VERSION", "unknown")  # automatically set by RTD
 
 release = version
@@ -243,15 +243,15 @@
 # base URL from which the finished HTML is served.
 # html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = "ngstools-doc"
+htmlhelp_basename = "ngstoolkits-doc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ("letterpaper" or "a4paper").
     # "papersize": "letterpaper",
@@ -260,15 +260,15 @@
     # Additional stuff for the LaTeX preamble.
     # "preamble": "",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ("index", "user_guide.tex", "ngstools Documentation", "Ben-unbelieveable", "manual")
+    ("index", "user_guide.tex", "ngstoolkits Documentation", "Ben-unbelieveable", "manual")
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
```

### Comparing `ngstoolkits-0.0.0rc1/docs/index.md` & `ngstoolkits-1.0.0rc1/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ngstools
+# ngstoolkits
 
 Add a short description here!
 
 
 ## Note
 
 > This is the main page of your project's [Sphinx] documentation. It is
```

### Comparing `ngstoolkits-0.0.0rc1/setup.cfg` & `ngstoolkits-1.0.0rc1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
-name = ngstools
-description = mange some useful class & function in NGS analysis
+name = ngstoolkits
+versison = 1.0.0rc1
+description = Add a short description here!
 author = Ben-unbelieveable
 author_email = 614347533@qq.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/pyscaffold/pyscaffold/
 project_urls = 
-	Documentation = https://github.com/Ben-unbelieveable/python_package_ngstools/README.md
-	Source = https://github.com/Ben-unbelieveable/python_package_ngstools
+	Documentation = https://pyscaffold.org/
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
@@ -36,15 +36,15 @@
 	pytest
 	pytest-cov
 
 [options.entry_points]
 
 [tool:pytest]
 addopts = 
-	--cov ngstools --cov-report term-missing
+	--cov ngstoolkits --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
 
@@ -60,15 +60,15 @@
 	build
 	dist
 	.eggs
 	docs/conf.py
 
 [pyscaffold]
 version = 4.5
-package = ngstools
+package = ngstoolkits
 extensions = 
 	markdown
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/PKG-INFO` & `ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ngstoolkits
-Version: 0.0.0rc1
+Version: 1.0.0rc1
 Summary: ngstools
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Liubo
 Author-email: 614347533@qq.com
 License: MIT
-Project-URL: Documentation, https://github.com/Ben-unbelieveable/python_package_ngstools/README.md
-Project-URL: Source, https://github.com/Ben-unbelieveable/python_package_ngstools
+Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: testing
@@ -31,18 +30,20 @@
 [![Twitter](https://img.shields.io/twitter/url/http/shields.io.svg?style=social&label=Twitter)](https://twitter.com/ngstools)
 -->
 
 [![Project generated with PyScaffold](https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold)](https://pyscaffold.org/)
 
 # ngstools
 
-> Add a short description here!
+> Useful toolkits for NGS analysis
 
-A longer description of your project goes here...
+## Main Class
+### mutation
 
+## Main Function
 
 <!-- pyscaffold-notes -->
 
 ## Note
 
 This project has been set up using PyScaffold 4.5. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `ngstoolkits-0.0.0rc1/src/ngstoolkits.egg-info/SOURCES.txt` & `ngstoolkits-1.0.0rc1/src/ngstoolkits.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 docs/index.md
 docs/license.md
 docs/readme.md
 docs/requirements.txt
 docs/_static/.gitignore
 src/ngstoolkits/__init__.py
 src/ngstoolkits/ngs_class.py
-src/ngstoolkits/skeleton.py
+src/ngstoolkits/sequence.py
 src/ngstoolkits.egg-info/PKG-INFO
 src/ngstoolkits.egg-info/SOURCES.txt
 src/ngstoolkits.egg-info/dependency_links.txt
 src/ngstoolkits.egg-info/not-zip-safe
 src/ngstoolkits.egg-info/requires.txt
 src/ngstoolkits.egg-info/top_level.txt
+tests/conftest.py
 tests/test_class.py
```

### Comparing `ngstoolkits-0.0.0rc1/tox.ini` & `ngstoolkits-1.0.0rc1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tox configuration file
 # Read more under https://tox.wiki/
 # THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
 
 [tox]
-minversion = 1.0.0a0
+minversion = 3.24
 envlist = default
 isolated_build = True
 
 
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
@@ -40,14 +40,15 @@
     build: Build the package in isolation according to PEP517, see https://github.com/pypa/build
     clean: Remove old distribution files and temporary build artifacts (./build and ./dist)
 # https://setuptools.pypa.io/en/stable/build_meta.html#how-to-use-it
 skip_install = True
 changedir = {toxinidir}
 deps =
     build: build[virtualenv]
+    pysam
 passenv =
     SETUPTOOLS_*
 commands =
     clean: python -c 'import shutil; [shutil.rmtree(p, True) for p in ("build", "dist", "docs/_build")]'
     clean: python -c 'import pathlib, shutil; [shutil.rmtree(p, True) for p in pathlib.Path("src").glob("*.egg-info")]'
     build: python -m build {posargs}
 # By default, both `sdist` and `wheel` are built. If your sdist is too big or you don't want
```

