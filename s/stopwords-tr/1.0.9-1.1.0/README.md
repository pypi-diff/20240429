# Comparing `tmp/stopwords_tr-1.0.9.tar.gz` & `tmp/stopwords_tr-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.0.9.tar", last modified: Mon Apr 29 20:09:15 2024, max compression
+gzip compressed data, was "stopwords_tr-1.1.0.tar", last modified: Mon Apr 29 20:19:57 2024, max compression
```

## Comparing `stopwords_tr-1.0.9.tar` & `stopwords_tr-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 20:09:15.993284 stopwords_tr-1.0.9/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     1051 2024-04-29 20:09:15.993284 stopwords_tr-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 20:09:15.994285 stopwords_tr-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1468 2024-04-29 18:44:04.000000 stopwords_tr-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 20:09:15.983284 stopwords_tr-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 20:09:15.986283 stopwords_tr-1.0.9/src/stopwords_tr/
--rw-rw-rw-   0        0        0      160 2024-04-29 20:05:07.000000 stopwords_tr-1.0.9/src/stopwords_tr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 20:09:15.991283 stopwords_tr-1.0.9/src/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0     1051 2024-04-29 20:09:15.000000 stopwords_tr-1.0.9/src/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-04-29 20:09:15.000000 stopwords_tr-1.0.9/src/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 20:09:15.000000 stopwords_tr-1.0.9/src/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 20:09:15.000000 stopwords_tr-1.0.9/src/stopwords_tr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 20:19:57.815972 stopwords_tr-1.1.0/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1051 2024-04-29 20:19:57.814972 stopwords_tr-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 20:19:57.815972 stopwords_tr-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1472 2024-04-29 20:19:55.000000 stopwords_tr-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 20:19:57.806972 stopwords_tr-1.1.0/stopwords_tr/
+drwxrwxrwx   0        0        0        0 2024-04-29 20:19:57.813972 stopwords_tr-1.1.0/stopwords_tr/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1051 2024-04-29 20:19:57.000000 stopwords_tr-1.1.0/stopwords_tr/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-29 20:19:57.000000 stopwords_tr-1.1.0/stopwords_tr/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 20:19:57.000000 stopwords_tr-1.1.0/stopwords_tr/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 20:19:57.000000 stopwords_tr-1.1.0/stopwords_tr/stopwords_tr.egg-info/top_level.txt
```

### Comparing `stopwords_tr-1.0.9/LICENSE` & `stopwords_tr-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.0.9/PKG-INFO` & `stopwords_tr-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.0.9
+Version: 1.1.0
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.0.9/setup.py` & `stopwords_tr-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.0.9',
+    version='1.1.0',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
@@ -26,11 +26,11 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12'
     ],
     # birden fazla dosya olduğundan sil 'py_modules'
     #py_modules=["stopwords_tr"]
-    package_dir={'':'src'},
-    packages= find_packages("src")
+    package_dir={'':'stopwords_tr'},
+    packages= find_packages()
     #bunları aktif edince kod dosyalarını src klasörü içine 'kütüphane ismi' klasörü oluşturup içine at
 )
```

### Comparing `stopwords_tr-1.0.9/src/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.1.0/stopwords_tr/stopwords_tr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.0.9
+Version: 1.1.0
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp, filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

