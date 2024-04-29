# Comparing `tmp/uk_std_libraries-0.0.12.tar.gz` & `tmp/uk_std_libraries-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uk_std_libraries-0.0.12.tar", last modified: Mon Apr 29 10:47:26 2024, max compression
+gzip compressed data, was "uk_std_libraries-0.0.13.tar", last modified: Mon Apr 29 11:10:55 2024, max compression
```

## Comparing `uk_std_libraries-0.0.12.tar` & `uk_std_libraries-0.0.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:47:26.525171 uk_std_libraries-0.0.12/
--rw-rw-rw-   0        0        0      719 2024-04-29 10:47:26.523166 uk_std_libraries-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-04-28 20:33:57.000000 uk_std_libraries-0.0.12/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 10:47:26.525171 uk_std_libraries-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0      958 2024-04-29 10:34:48.000000 uk_std_libraries-0.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:47:26.508073 uk_std_libraries-0.0.12/бібліотека/
-drwxrwxrwx   0        0        0        0 2024-04-29 10:47:26.522165 uk_std_libraries-0.0.12/бібліотека/uk_std_libraries.egg-info/
--rw-rw-rw-   0        0        0      719 2024-04-29 10:47:26.000000 uk_std_libraries-0.0.12/бібліотека/uk_std_libraries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2024-04-29 10:47:26.000000 uk_std_libraries-0.0.12/бібліотека/uk_std_libraries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:47:26.000000 uk_std_libraries-0.0.12/бібліотека/uk_std_libraries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-29 10:47:26.000000 uk_std_libraries-0.0.12/бібліотека/uk_std_libraries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       36 2024-04-29 10:47:26.000000 uk_std_libraries-0.0.12/бібліотека/uk_std_libraries.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 10:47:26.521158 uk_std_libraries-0.0.12/бібліотека/вбудовані_елементи/
--rw-rw-rw-   0        0        0      140 2024-04-29 10:28:12.000000 uk_std_libraries-0.0.12/бібліотека/вбудовані_елементи/__init__.py
--rw-rw-rw-   0        0        0      600 2024-04-28 20:50:40.000000 uk_std_libraries-0.0.12/бібліотека/вбудовані_елементи/вбудовані_функції.py
--rw-rw-rw-   0        0        0       82 2024-04-28 20:42:54.000000 uk_std_libraries-0.0.12/бібліотека/вбудовані_елементи/типи_данних.py
--rw-rw-rw-   0        0        0       56 2024-04-29 10:38:32.000000 uk_std_libraries-0.0.12/бібліотека/вбудовані_елементи/фіксовані_значення.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:10:55.949202 uk_std_libraries-0.0.13/
+-rw-rw-rw-   0        0        0      719 2024-04-29 11:10:55.948176 uk_std_libraries-0.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-04-28 20:33:57.000000 uk_std_libraries-0.0.13/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 11:10:55.949202 uk_std_libraries-0.0.13/setup.cfg
+-rw-rw-rw-   0        0        0      958 2024-04-29 11:10:47.000000 uk_std_libraries-0.0.13/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 11:10:55.936473 uk_std_libraries-0.0.13/бібліотека/
+drwxrwxrwx   0        0        0        0 2024-04-29 11:10:55.947194 uk_std_libraries-0.0.13/бібліотека/uk_std_libraries.egg-info/
+-rw-rw-rw-   0        0        0      719 2024-04-29 11:10:55.000000 uk_std_libraries-0.0.13/бібліотека/uk_std_libraries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2024-04-29 11:10:55.000000 uk_std_libraries-0.0.13/бібліотека/uk_std_libraries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 11:10:55.000000 uk_std_libraries-0.0.13/бібліотека/uk_std_libraries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-29 11:10:55.000000 uk_std_libraries-0.0.13/бібліотека/uk_std_libraries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       36 2024-04-29 11:10:55.000000 uk_std_libraries-0.0.13/бібліотека/uk_std_libraries.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 11:10:55.946178 uk_std_libraries-0.0.13/бібліотека/вбудовані_елементи/
+-rw-rw-rw-   0        0        0      140 2024-04-29 10:28:12.000000 uk_std_libraries-0.0.13/бібліотека/вбудовані_елементи/__init__.py
+-rw-rw-rw-   0        0        0      600 2024-04-28 20:50:40.000000 uk_std_libraries-0.0.13/бібліотека/вбудовані_елементи/вбудовані_функції.py
+-rw-rw-rw-   0        0        0      103 2024-04-29 11:10:32.000000 uk_std_libraries-0.0.13/бібліотека/вбудовані_елементи/типи_данних.py
+-rw-rw-rw-   0        0        0       56 2024-04-29 10:38:32.000000 uk_std_libraries-0.0.13/бібліотека/вбудовані_елементи/фіксовані_значення.py
```

### Comparing `uk_std_libraries-0.0.12/PKG-INFO` & `uk_std_libraries-0.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_std_libraries
-Version: 0.0.12
+Version: 0.0.13
 Summary: Україномовна бібліотека адаптації мови Python
 Home-page: https://github.com/NeoUKR/uk_std_libraries.git
 Author: Коваленко Костянтин
 Author-email: neokkv@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `uk_std_libraries-0.0.12/setup.py` & `uk_std_libraries-0.0.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="uk_std_libraries",
-    version="0.0.12",
+    version="0.0.13",
     description="Україномовна бібліотека адаптації мови Python",
     package_dir={"": "бібліотека"},
     packages=find_packages(where="бібліотека"),
     long_description="Україномовна бібліотека адаптації мови Python",
     long_description_content_type="text/markdown",
     url="https://github.com/NeoUKR/uk_std_libraries.git",
     author="Коваленко Костянтин",
```

### Comparing `uk_std_libraries-0.0.12/бібліотека/uk_std_libraries.egg-info/PKG-INFO` & `uk_std_libraries-0.0.13/бібліотека/uk_std_libraries.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uk_std_libraries
-Version: 0.0.12
+Version: 0.0.13
 Summary: Україномовна бібліотека адаптації мови Python
 Home-page: https://github.com/NeoUKR/uk_std_libraries.git
 Author: Коваленко Костянтин
 Author-email: neokkv@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `uk_std_libraries-0.0.12/бібліотека/uk_std_libraries.egg-info/SOURCES.txt` & `uk_std_libraries-0.0.13/бібліотека/uk_std_libraries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uk_std_libraries-0.0.12/бібліотека/вбудовані_елементи/вбудовані_функції.py` & `uk_std_libraries-0.0.13/бібліотека/вбудовані_елементи/вбудовані_функції.py`

 * *Files identical despite different names*

