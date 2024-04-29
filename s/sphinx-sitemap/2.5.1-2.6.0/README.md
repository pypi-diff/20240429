# Comparing `tmp/sphinx-sitemap-2.5.1.tar.gz` & `tmp/sphinx_sitemap-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-sitemap-2.5.1.tar", last modified: Fri Aug 18 04:26:19 2023, max compression
+gzip compressed data, was "sphinx_sitemap-2.6.0.tar", last modified: Mon Apr 29 00:02:48 2024, max compression
```

## Comparing `sphinx-sitemap-2.5.1.tar` & `sphinx_sitemap-2.6.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 jared.dillard (1788608735) domain^users (1788600513)        0 2023-08-18 04:26:19.539137 sphinx-sitemap-2.5.1/
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     1070 2022-11-12 06:19:32.000000 sphinx-sitemap-2.5.1/LICENSE
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       16 2022-11-12 06:19:32.000000 sphinx-sitemap-2.5.1/MANIFEST.in
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     3189 2023-08-18 04:26:19.539137 sphinx-sitemap-2.5.1/PKG-INFO
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     2207 2023-08-18 04:01:30.000000 sphinx-sitemap-2.5.1/README.rst
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     1094 2023-08-18 04:01:30.000000 sphinx-sitemap-2.5.1/pyproject.toml
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)      225 2023-08-18 04:26:19.539137 sphinx-sitemap-2.5.1/setup.cfg
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       69 2023-08-18 04:01:30.000000 sphinx-sitemap-2.5.1/setup.py
-drwxr-xr-x   0 jared.dillard (1788608735) domain^users (1788600513)        0 2023-08-18 04:26:19.539137 sphinx-sitemap-2.5.1/sphinx_sitemap/
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     7247 2023-08-18 04:25:18.000000 sphinx-sitemap-2.5.1/sphinx_sitemap/__init__.py
-drwxr-xr-x   0 jared.dillard (1788608735) domain^users (1788600513)        0 2023-08-18 04:26:19.539137 sphinx-sitemap-2.5.1/sphinx_sitemap.egg-info/
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     3189 2023-08-18 04:26:19.000000 sphinx-sitemap-2.5.1/sphinx_sitemap.egg-info/PKG-INFO
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)      329 2023-08-18 04:26:19.000000 sphinx-sitemap-2.5.1/sphinx_sitemap.egg-info/SOURCES.txt
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)        1 2023-08-18 04:26:19.000000 sphinx-sitemap-2.5.1/sphinx_sitemap.egg-info/dependency_links.txt
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       12 2023-08-18 04:26:19.000000 sphinx-sitemap-2.5.1/sphinx_sitemap.egg-info/requires.txt
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       15 2023-08-18 04:26:19.000000 sphinx-sitemap-2.5.1/sphinx_sitemap.egg-info/top_level.txt
-drwxr-xr-x   0 jared.dillard (1788608735) domain^users (1788600513)        0 2023-08-18 04:26:19.539137 sphinx-sitemap-2.5.1/tests/
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)      862 2023-08-18 04:25:18.000000 sphinx-sitemap-2.5.1/tests/test_parallel_mode.py
--rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     2361 2023-08-18 04:25:18.000000 sphinx-sitemap-2.5.1/tests/test_simple.py
+drwxr-xr-x   0 jared.dillard (1788608735) domain^users (1788600513)        0 2024-04-29 00:02:48.487882 sphinx_sitemap-2.6.0/
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     1070 2022-11-12 06:19:32.000000 sphinx_sitemap-2.6.0/LICENSE
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       16 2022-11-12 06:19:32.000000 sphinx_sitemap-2.6.0/MANIFEST.in
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     3421 2024-04-29 00:02:48.487882 sphinx_sitemap-2.6.0/PKG-INFO
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     2214 2024-01-18 05:13:58.000000 sphinx_sitemap-2.6.0/README.rst
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     1193 2024-04-29 00:00:03.000000 sphinx_sitemap-2.6.0/pyproject.toml
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       42 2023-08-18 04:01:30.000000 sphinx_sitemap-2.6.0/requirements_dev.txt
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)      225 2024-04-29 00:02:48.487882 sphinx_sitemap-2.6.0/setup.cfg
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       69 2023-08-18 04:01:30.000000 sphinx_sitemap-2.6.0/setup.py
+drwxr-xr-x   0 jared.dillard (1788608735) domain^users (1788600513)        0 2024-04-29 00:02:48.483882 sphinx_sitemap-2.6.0/sphinx_sitemap/
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     7385 2024-04-29 00:00:03.000000 sphinx_sitemap-2.6.0/sphinx_sitemap/__init__.py
+drwxr-xr-x   0 jared.dillard (1788608735) domain^users (1788600513)        0 2024-04-29 00:02:48.483882 sphinx_sitemap-2.6.0/sphinx_sitemap.egg-info/
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     3421 2024-04-29 00:02:48.000000 sphinx_sitemap-2.6.0/sphinx_sitemap.egg-info/PKG-INFO
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)      350 2024-04-29 00:02:48.000000 sphinx_sitemap-2.6.0/sphinx_sitemap.egg-info/SOURCES.txt
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)        1 2024-04-29 00:02:48.000000 sphinx_sitemap-2.6.0/sphinx_sitemap.egg-info/dependency_links.txt
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       61 2024-04-29 00:02:48.000000 sphinx_sitemap-2.6.0/sphinx_sitemap.egg-info/requires.txt
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)       15 2024-04-29 00:02:48.000000 sphinx_sitemap-2.6.0/sphinx_sitemap.egg-info/top_level.txt
+drwxr-xr-x   0 jared.dillard (1788608735) domain^users (1788600513)        0 2024-04-29 00:02:48.483882 sphinx_sitemap-2.6.0/tests/
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)      862 2023-08-18 04:25:18.000000 sphinx_sitemap-2.6.0/tests/test_parallel_mode.py
+-rw-r--r--   0 jared.dillard (1788608735) domain^users (1788600513)     3146 2024-04-29 00:00:03.000000 sphinx_sitemap-2.6.0/tests/test_simple.py
```

### Comparing `sphinx-sitemap-2.5.1/LICENSE` & `sphinx_sitemap-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-sitemap-2.5.1/README.rst` & `sphinx_sitemap-2.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 .. _sitemaps.org: https://www.sitemaps.org/protocol.html
 .. _sphinx-sitemap documentation: https://sphinx-sitemap.readthedocs.io/en/latest/index.html
 
 .. |PyPI version| image:: https://img.shields.io/pypi/v/sphinx-sitemap.svg
    :target: https://pypi.python.org/pypi/sphinx-sitemap
 .. |Conda Forge| image:: https://img.shields.io/conda/vn/conda-forge/sphinx-sitemap.svg
    :target: https://anaconda.org/conda-forge/sphinx-sitemap
-.. |Downloads| image:: https://pepy.tech/badge/sphinx-sitemap/month
+.. |Downloads| image:: https://static.pepy.tech/badge/sphinx-sitemap/month
     :target: https://pepy.tech/project/sphinx-sitemap
 .. |Code style: Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
 .. |Parallel Safe| image:: https://img.shields.io/badge/parallel%20safe-true-brightgreen
    :target: #
 .. |Docs Build| image:: https://readthedocs.org/projects/sphinx-sitemap/badge/?version=latest
    :target: https://sphinx-sitemap.readthedocs.io/en/latest/?badge=latest
```

### Comparing `sphinx-sitemap-2.5.1/pyproject.toml` & `sphinx_sitemap-2.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -13,28 +13,32 @@
 ]
 maintainers = [
     {name = "Jared Dillard", email = "jared.dillard@gmail.com"},
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Topic :: Documentation :: Sphinx",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Framework :: Sphinx :: Extension",
 ]
 license = {text = "MIT"}
 readme = "README.rst"
 dynamic = [
     "version",
+    "dependencies",
+    "optional-dependencies",
 ]
 
 [project.urls]
 documentation = "https://sphinx-sitemap.readthedocs.io/en/latest/index.html"
 download = "https://pypi.org/project/sphinx-sitemap/"
 source = "https://github.com/jdillard/sphinx-sitemap"
 changelog = "https://github.com/jdillard/sphinx-sitemap/blob/master/CHANGELOG.rst"
 
+[tool.setuptools.dynamic]
+optional-dependencies = {dev = { file = ["requirements_dev.txt"] }}
+
 [tool.isort]
 profile = "black"
```

### Comparing `sphinx-sitemap-2.5.1/sphinx_sitemap/__init__.py` & `sphinx_sitemap-2.6.0/sphinx_sitemap/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 from xml.etree import ElementTree
 
 from sphinx.application import Sphinx
 from sphinx.util.logging import getLogger
 
-__version__ = "2.5.1"
+__version__ = "2.6.0"
 
 logger = getLogger(__name__)
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     """
     Sphinx extension setup function.
@@ -38,14 +38,16 @@
     app.add_config_value(
         "sitemap_url_scheme", default="{lang}{version}{link}", rebuild=""
     )
     app.add_config_value("sitemap_locales", default=None, rebuild="")
 
     app.add_config_value("sitemap_filename", default="sitemap.xml", rebuild="")
 
+    app.add_config_value("sitemap_excludes", default=[], rebuild="")
+
     try:
         app.add_config_value("html_baseurl", default=None, rebuild="")
     except BaseException:
         pass
 
     app.connect("builder-inited", record_builder_type)
     app.connect("html-page-context", add_html_link)
@@ -139,15 +141,16 @@
         elif pagename.endswith("/index"):
             sitemap_link = pagename[:-6] + "/"
         else:
             sitemap_link = pagename + "/"
     else:
         sitemap_link = pagename + file_suffix
 
-    env.app.sitemap_links.put(sitemap_link)  # type: ignore
+    if sitemap_link not in app.builder.config.sitemap_excludes:
+        env.app.sitemap_links.put(sitemap_link)  # type: ignore
 
 
 def create_sitemap(app: Sphinx, exception):
     """
     Generates the sitemap.xml from the collected HTML page links.
 
     :param app: The Sphinx Application instance
```

### Comparing `sphinx-sitemap-2.5.1/tests/test_parallel_mode.py` & `sphinx_sitemap-2.6.0/tests/test_parallel_mode.py`

 * *Files identical despite different names*

### Comparing `sphinx-sitemap-2.5.1/tests/test_simple.py` & `sphinx_sitemap-2.6.0/tests/test_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,7 +95,40 @@
             "ipsum/",
             "dolor/",
             "elitr/",
             "genindex/",
             "search/",
         ]
     }
+
+
+@pytest.mark.sphinx(
+    "html",
+    freshenv=True,
+    confoverrides={
+        "html_baseurl": "https://example.org/docs/",
+        "language": "en",
+        "sitemap_excludes": ["search.html", "genindex.html"],
+    },
+)
+def test_simple_excludes(app, status, warning):
+    app.warningiserror = True
+    app.build()
+    assert "sitemap.xml" in os.listdir(app.outdir)
+    doc = etree.parse(app.outdir / "sitemap.xml")
+    urls = {
+        e.text
+        for e in doc.findall(".//{http://www.sitemaps.org/schemas/sitemap/0.9}loc")
+    }
+
+    assert urls == {
+        f"https://example.org/docs/en/{d}.html"
+        for d in [
+            "index",
+            "foo",
+            "bar",
+            "lorem",
+            "ipsum",
+            "dolor",
+            "elitr",
+        ]
+    }
```

