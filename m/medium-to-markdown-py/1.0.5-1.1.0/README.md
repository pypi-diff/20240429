# Comparing `tmp/medium_to_markdown_py-1.0.5.tar.gz` & `tmp/medium_to_markdown_py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_to_markdown_py-1.0.5.tar", last modified: Sun Apr 28 14:38:18 2024, max compression
+gzip compressed data, was "medium_to_markdown_py-1.1.0.tar", last modified: Sun Apr 28 14:43:41 2024, max compression
```

## Comparing `medium_to_markdown_py-1.0.5.tar` & `medium_to_markdown_py-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:38:18.743062 medium_to_markdown_py-1.0.5/
--rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.0.5/LICENSE
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-28 14:38:18.742993 medium_to_markdown_py-1.0.5/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      633 2024-04-28 14:20:07.000000 medium_to_markdown_py-1.0.5/README.md
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:38:18.741662 medium_to_markdown_py-1.0.5/medium_to_markdown/
--rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 14:38:16.000000 medium_to_markdown_py-1.0.5/medium_to_markdown/__init__.py
--rw-r--r--   0 shin       (501) staff       (20)     7314 2024-04-28 14:27:56.000000 medium_to_markdown_py-1.0.5/medium_to_markdown/medium_to_markdown.py
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:38:18.742787 medium_to_markdown_py-1.0.5/medium_to_markdown_py.egg-info/
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-28 14:38:18.000000 medium_to_markdown_py-1.0.5/medium_to_markdown_py.egg-info/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      376 2024-04-28 14:38:18.000000 medium_to_markdown_py-1.0.5/medium_to_markdown_py.egg-info/SOURCES.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:38:18.000000 medium_to_markdown_py-1.0.5/medium_to_markdown_py.egg-info/dependency_links.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 04:36:12.000000 medium_to_markdown_py-1.0.5/medium_to_markdown_py.egg-info/not-zip-safe
--rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 14:38:18.000000 medium_to_markdown_py-1.0.5/medium_to_markdown_py.egg-info/requires.txt
--rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-28 14:38:18.000000 medium_to_markdown_py-1.0.5/medium_to_markdown_py.egg-info/top_level.txt
--rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 14:38:18.743259 medium_to_markdown_py-1.0.5/setup.cfg
--rw-r--r--   0 shin       (501) staff       (20)      612 2024-04-28 14:38:10.000000 medium_to_markdown_py-1.0.5/setup.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:43:41.611638 medium_to_markdown_py-1.1.0/
+-rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.0/LICENSE
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-28 14:43:41.611565 medium_to_markdown_py-1.1.0/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      640 2024-04-28 14:43:34.000000 medium_to_markdown_py-1.1.0/README.md
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:43:41.609990 medium_to_markdown_py-1.1.0/medium_to_markdown/
+-rw-r--r--   0 shin       (501) staff       (20)     7314 2024-04-28 14:42:30.000000 medium_to_markdown_py-1.1.0/medium_to_markdown/Parser.py
+-rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 14:43:18.000000 medium_to_markdown_py-1.1.0/medium_to_markdown/__init__.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:43:41.611351 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      364 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/not-zip-safe
+-rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/requires.txt
+-rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/top_level.txt
+-rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 14:43:41.611860 medium_to_markdown_py-1.1.0/setup.cfg
+-rw-r--r--   0 shin       (501) staff       (20)      612 2024-04-28 14:43:14.000000 medium_to_markdown_py-1.1.0/setup.py
```

### Comparing `medium_to_markdown_py-1.0.5/LICENSE` & `medium_to_markdown_py-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.0.5/README.md` & `medium_to_markdown_py-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ```
 
 ## Usage
 
 The command-line interface (CLI) accepts a Medium blog post URL and a filename as input and generates the Markdown content.
 
 ``` python
-from medium_to_markdown import MediumParser
+from medium_to_markdown.Parser import MediumParser
 
 url = "https://~~~~"
 filename = ""
 is_image_download = True
 ssl_verify = True
 
 parser = MediumParser(url, filename, is_image_download, ssl_verify)
```

### Comparing `medium_to_markdown_py-1.0.5/medium_to_markdown/medium_to_markdown.py` & `medium_to_markdown_py-1.1.0/medium_to_markdown/Parser.py`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.0.5/setup.py` & `medium_to_markdown_py-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medium_to_markdown_py',
-    version='1.0.5',
+    version='1.1.0',
     description='medium-to-medium_to_markdown_py-py is a Python package that converts Medium articles to Markdown format.',
     author='knowslog',
     author_email='scshin88@gmail.com',
     url='https://github.com/tourbut/medium-to-markdown_python',
     install_requires=['beautifulsoup4', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['medium', 'knowslog', 'markdown', 'medium to markdown'],
```

