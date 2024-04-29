# Comparing `tmp/stopwords_tr-1.0.3.tar.gz` & `tmp/stopwords_tr-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stopwords_tr-1.0.3.tar", last modified: Mon Apr 29 14:36:50 2024, max compression
+gzip compressed data, was "stopwords_tr-1.0.4.tar", last modified: Mon Apr 29 15:05:25 2024, max compression
```

## Comparing `stopwords_tr-1.0.3.tar` & `stopwords_tr-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 14:36:50.254748 stopwords_tr-1.0.3/
--rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      946 2024-04-29 14:36:50.251628 stopwords_tr-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 14:36:50.255729 stopwords_tr-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1112 2024-04-29 14:36:34.000000 stopwords_tr-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 14:36:50.248629 stopwords_tr-1.0.3/stopwords_tr.egg-info/
--rw-rw-rw-   0        0        0      946 2024-04-29 14:36:50.000000 stopwords_tr-1.0.3/stopwords_tr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-04-29 14:36:50.000000 stopwords_tr-1.0.3/stopwords_tr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 14:36:50.000000 stopwords_tr-1.0.3/stopwords_tr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 14:36:50.000000 stopwords_tr-1.0.3/stopwords_tr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      170 2024-04-29 14:23:22.000000 stopwords_tr-1.0.3/stopwords_tr.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:05:25.780287 stopwords_tr-1.0.4/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 06:28:23.000000 stopwords_tr-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1050 2024-04-29 15:05:25.777298 stopwords_tr-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2024-04-26 06:38:36.000000 stopwords_tr-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 15:05:25.780660 stopwords_tr-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1214 2024-04-29 15:05:17.000000 stopwords_tr-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 15:05:25.774223 stopwords_tr-1.0.4/stopwords_tr.egg-info/
+-rw-rw-rw-   0        0        0     1050 2024-04-29 15:05:25.000000 stopwords_tr-1.0.4/stopwords_tr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-04-29 15:05:25.000000 stopwords_tr-1.0.4/stopwords_tr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 15:05:25.000000 stopwords_tr-1.0.4/stopwords_tr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-29 15:05:25.000000 stopwords_tr-1.0.4/stopwords_tr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      159 2024-04-29 14:58:53.000000 stopwords_tr-1.0.4/stopwords_tr.py
```

### Comparing `stopwords_tr-1.0.3/LICENSE` & `stopwords_tr-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stopwords_tr-1.0.3/PKG-INFO` & `stopwords_tr-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp,filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1>STOPWORDS FOR TURKISH LANGUAGE</h1>
 <h3>import stopwordstr</h3></h3>
 <h3>stopwordstr.stopwords()</h3>
```

### Comparing `stopwords_tr-1.0.3/setup.py` & `stopwords_tr-1.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name= 'stopwords_tr',
-    version='1.0.3',
+    version='1.0.4',
     license='MIT',
     author="Metin Oktay DENIZ",
     author_email='metinoktaydenizz@gmail.com',
     description="Stopwords filter for Turkish languages",
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
     url='https://github.com/metinoktayd/StopWords-Turkish-Language',
@@ -20,11 +20,13 @@
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12'
     ],
     py_modules=["stopwords_tr"]
 )
```

### Comparing `stopwords_tr-1.0.3/stopwords_tr.egg-info/PKG-INFO` & `stopwords_tr-1.0.4/stopwords_tr.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: stopwords_tr
-Version: 1.0.3
+Version: 1.0.4
 Summary: Stopwords filter for Turkish languages
 Home-page: https://github.com/metinoktayd/StopWords-Turkish-Language
 Author: Metin Oktay DENIZ
 Author-email: metinoktaydenizz@gmail.com
 License: MIT
 Keywords: stopwords, language processing, nlp,filter, turkish stopwords, stopwords for tr, stop for tr, Türkçe Stopwords, Turkish stop, Türkçe Stop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1>STOPWORDS FOR TURKISH LANGUAGE</h1>
 <h3>import stopwordstr</h3></h3>
 <h3>stopwordstr.stopwords()</h3>
```

