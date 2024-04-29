# Comparing `tmp/uk_std_libraries-0.0.7.tar.gz` & `tmp/uk_std_libraries-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk_std_libraries-0.0.7.tar", last modified: Sun Apr 28 21:47:29 2024, max compression
+gzip compressed data, was "uk_std_libraries-0.0.8.tar", last modified: Mon Apr 29 09:50:06 2024, max compression
```

## Comparing `uk_std_libraries-0.0.7.tar` & `uk_std_libraries-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 21:47:29.358604 uk_std_libraries-0.0.7/
--rw-rw-rw-   0        0        0      718 2024-04-28 21:47:29.358604 uk_std_libraries-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-04-28 20:33:57.000000 uk_std_libraries-0.0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-28 21:47:29.359608 uk_std_libraries-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      945 2024-04-28 21:47:14.000000 uk_std_libraries-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-28 21:47:29.348877 uk_std_libraries-0.0.7/додаток/
-drwxrwxrwx   0        0        0        0 2024-04-28 21:47:29.357628 uk_std_libraries-0.0.7/додаток/uk_std_libraries.egg-info/
--rw-rw-rw-   0        0        0      718 2024-04-28 21:47:29.000000 uk_std_libraries-0.0.7/додаток/uk_std_libraries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2024-04-28 21:47:29.000000 uk_std_libraries-0.0.7/додаток/uk_std_libraries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 21:47:29.000000 uk_std_libraries-0.0.7/додаток/uk_std_libraries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-28 21:47:29.000000 uk_std_libraries-0.0.7/додаток/uk_std_libraries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       36 2024-04-28 21:47:29.000000 uk_std_libraries-0.0.7/додаток/uk_std_libraries.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-28 21:47:29.356604 uk_std_libraries-0.0.7/додаток/вбудовані_елементи/
--rw-rw-rw-   0        0        0      140 2024-04-28 20:51:17.000000 uk_std_libraries-0.0.7/додаток/вбудовані_елементи/__init__.py
--rw-rw-rw-   0        0        0      600 2024-04-28 20:50:40.000000 uk_std_libraries-0.0.7/додаток/вбудовані_елементи/вбудовані_функції.py
--rw-rw-rw-   0        0        0       82 2024-04-28 20:42:54.000000 uk_std_libraries-0.0.7/додаток/вбудовані_елементи/типи_данних.py
--rw-rw-rw-   0        0        0       45 2024-04-28 20:14:14.000000 uk_std_libraries-0.0.7/додаток/вбудовані_елементи/фіксовані_значення.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:50:06.308377 uk_std_libraries-0.0.8/
+-rw-rw-rw-   0        0        0      718 2024-04-29 09:50:06.307374 uk_std_libraries-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-28 20:33:57.000000 uk_std_libraries-0.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 09:50:06.308377 uk_std_libraries-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      987 2024-04-29 09:46:15.000000 uk_std_libraries-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:50:06.288857 uk_std_libraries-0.0.8/вбудовані_елементи/
+drwxrwxrwx   0        0        0        0 2024-04-29 09:50:06.305379 uk_std_libraries-0.0.8/вбудовані_елементи/uk_std_libraries.egg-info/
+-rw-rw-rw-   0        0        0      718 2024-04-29 09:50:06.000000 uk_std_libraries-0.0.8/вбудовані_елементи/uk_std_libraries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2024-04-29 09:50:06.000000 uk_std_libraries-0.0.8/вбудовані_елементи/uk_std_libraries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 09:50:06.000000 uk_std_libraries-0.0.8/вбудовані_елементи/uk_std_libraries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-29 09:50:06.000000 uk_std_libraries-0.0.8/вбудовані_елементи/uk_std_libraries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 09:50:06.000000 uk_std_libraries-0.0.8/вбудовані_елементи/uk_std_libraries.egg-info/top_level.txt
```

### Comparing `uk_std_libraries-0.0.7/PKG-INFO` & `uk_std_libraries-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_std_libraries
-Version: 0.0.7
+Version: 0.0.8
 Summary: Україномовна бібліотека адаптації мови Python
 Home-page: https://github.com/NeoUKR/uk_std_libraries.git
 Author: Коваленко Костянтин
 Author-email: neokkv@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `uk_std_libraries-0.0.7/setup.py` & `uk_std_libraries-0.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 setup(
     name="uk_std_libraries",
-    version="0.0.7",
+    version="0.0.8",
     description="Україномовна бібліотека адаптації мови Python",
-    package_dir={"": "додаток"},
-    packages=find_packages(where="додаток"),
+    package_dir={"": "вбудовані_елементи"},
+    packages=find_packages(where="вбудовані_елементи"),
     long_description="Україномовна бібліотека адаптації мови Python",
     long_description_content_type="text/markdown",
     url="https://github.com/NeoUKR/uk_std_libraries.git",
     author="Коваленко Костянтин",
     author_email="neokkv@gmail.com",
     license="MIT",
     classifiers=[
```

### Comparing `uk_std_libraries-0.0.7/додаток/uk_std_libraries.egg-info/PKG-INFO` & `uk_std_libraries-0.0.8/вбудовані_елементи/uk_std_libraries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_std_libraries
-Version: 0.0.7
+Version: 0.0.8
 Summary: Україномовна бібліотека адаптації мови Python
 Home-page: https://github.com/NeoUKR/uk_std_libraries.git
 Author: Коваленко Костянтин
 Author-email: neokkv@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

