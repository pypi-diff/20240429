# Comparing `tmp/basiclingua-1.0.0.tar.gz` & `tmp/basiclingua-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\basiclingua-1.0.0.tar", last modified: Sun Mar  3 14:51:20 2024, max compression
+gzip compressed data, was "dist\basiclingua-2.0.0.tar", last modified: Mon Apr 29 13:34:10 2024, max compression
```

## Comparing `basiclingua-1.0.0.tar` & `basiclingua-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-03 14:51:20.494626 basiclingua-1.0.0/
--rw-rw-rw-   0        0        0    14567 2024-03-03 14:51:20.494626 basiclingua-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    12506 2024-03-03 14:51:10.000000 basiclingua-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-03 14:51:20.455192 basiclingua-1.0.0/basiclingua/
--rw-rw-rw-   0        0        0    61496 2024-03-03 11:09:02.000000 basiclingua-1.0.0/basiclingua/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-03 14:51:20.494626 basiclingua-1.0.0/basiclingua.egg-info/
--rw-rw-rw-   0        0        0    14567 2024-03-03 14:51:20.000000 basiclingua-1.0.0/basiclingua.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2024-03-03 14:51:20.000000 basiclingua-1.0.0/basiclingua.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-03 14:51:20.000000 basiclingua-1.0.0/basiclingua.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-03-03 14:51:20.000000 basiclingua-1.0.0/basiclingua.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-03 14:51:20.000000 basiclingua-1.0.0/basiclingua.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-03 14:51:20.494626 basiclingua-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1330 2024-03-03 11:07:01.000000 basiclingua-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:34:10.692248 basiclingua-2.0.0/
+-rw-rw-rw-   0        0        0    21622 2024-04-29 13:34:10.690879 basiclingua-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    18632 2024-04-29 13:26:01.000000 basiclingua-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 13:34:10.650964 basiclingua-2.0.0/basiclingua/
+-rw-rw-rw-   0        0        0   143803 2024-04-29 13:26:33.000000 basiclingua-2.0.0/basiclingua/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:34:10.689219 basiclingua-2.0.0/basiclingua.egg-info/
+-rw-rw-rw-   0        0        0    21622 2024-04-29 13:34:10.000000 basiclingua-2.0.0/basiclingua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2024-04-29 13:34:10.000000 basiclingua-2.0.0/basiclingua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 13:34:10.000000 basiclingua-2.0.0/basiclingua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-04-29 13:34:10.000000 basiclingua-2.0.0/basiclingua.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-29 13:34:10.000000 basiclingua-2.0.0/basiclingua.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 13:34:10.692248 basiclingua-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2024-04-29 13:32:59.000000 basiclingua-2.0.0/setup.py
```

### Comparing `basiclingua-1.0.0/setup.py` & `basiclingua-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
-VERSION = '1.0.0'
-DESCRIPTION = 'A Python library based on Google Gemini LLM to perform basic and advanced natural language processing (NLP) tasks'
-LONG_DESCRIPTION = 'Basiclingua is a Gemini LLM based Python library that provides functionalities for linguistic tasks such as tokenization, stemming, lemmatization, and many others.'
+VERSION = '2.0.0'
+DESCRIPTION = 'A Python library based on various LLMs to perform basic and advanced natural language processing (NLP) tasks'
 
 # Setting up
 setup(
     name="basiclingua",
     version=VERSION,
-    author="Fareed Hassan Khan, Syed Asad Rizvi",
-    author_email="<fareedhassankhan12@gmail.com>, <syedasad44@gmail.com>",
+    author="Fareed Hassan Khan",
+    author_email="<fareedhassankhan12@gmail.com>",
     description=DESCRIPTION,
     long_description=read('README.md'),
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=["google-generativeai", "grpcio", "grpcio-tools"],  # Add any dependencies here
+    install_requires=["google-generativeai", "grpcio", "grpcio-tools", "openai", "emoji", "PyMuPDF"],  # Add any dependencies here
     keywords=['python', 'NLP', 'Natural Language Processing', 'Linguistics', 'Gemini LLM', 'Google Gemini LLM'],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
-        "Operating System :: Microsoft :: Windows",
         "License :: OSI Approved :: MIT License",
     ]
 )
```

