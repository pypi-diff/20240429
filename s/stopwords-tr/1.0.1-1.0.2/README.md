# Comparing `tmp/stopwords_tr-1.0.1.tar.gz` & `tmp/stopwords_tr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.0.1.tar", last modified: Mon Apr 29 14:18:29 2024, max compression
+gzip compressed data, was "stopwords_tr-1.0.2.tar", last modified: Mon Apr 29 14:24:58 2024, max compression
```

## Comparing `stopwords_tr-1.0.1.tar` & `stopwords_tr-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 14:18:29.597592 stopwords_tr-1.0.1/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      946 2024-04-29 14:18:29.593184 stopwords_tr-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 14:18:29.599715 stopwords_tr-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1112 2024-04-29 13:56:01.000000 stopwords_tr-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:18:29.590798 stopwords_tr-1.0.1/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0      946 2024-04-29 14:18:29.000000 stopwords_tr-1.0.1/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-29 14:18:29.000000 stopwords_tr-1.0.1/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 14:18:29.000000 stopwords_tr-1.0.1/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 14:18:29.000000 stopwords_tr-1.0.1/stopwords_tr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      159 2024-04-29 14:06:19.000000 stopwords_tr-1.0.1/stopwords_tr.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:24:58.744477 stopwords_tr-1.0.2/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      946 2024-04-29 14:24:58.741328 stopwords_tr-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 14:24:58.744477 stopwords_tr-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2024-04-29 14:23:22.000000 stopwords_tr-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 14:24:58.739327 stopwords_tr-1.0.2/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0      946 2024-04-29 14:24:58.000000 stopwords_tr-1.0.2/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-29 14:24:58.000000 stopwords_tr-1.0.2/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 14:24:58.000000 stopwords_tr-1.0.2/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 14:24:58.000000 stopwords_tr-1.0.2/stopwords_tr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      170 2024-04-29 14:23:22.000000 stopwords_tr-1.0.2/stopwords_tr.py
```

### Comparing `stopwords_tr-1.0.1/LICENSE` & `stopwords_tr-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.0.1/PKG-INFO` & `stopwords_tr-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.0.1
+Version: 1.0.2
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp,filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `stopwords_tr-1.0.1/setup.py` & `stopwords_tr-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.0.1',
+    version='1.0.2',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
```

### Comparing `stopwords_tr-1.0.1/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.0.2/stopwords_tr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.0.1
+Version: 1.0.2
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp,filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
```

