# Comparing `tmp/optibioseq-0.1.5.tar.gz` & `tmp/optibioseq-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\optibioseq-0.1.5.tar", last modified: Wed Nov  1 16:20:02 2023, max compression
+gzip compressed data, was "optibioseq-0.1.6.tar", last modified: Mon Apr 29 21:45:29 2024, max compression
```

## Comparing `optibioseq-0.1.5.tar` & `optibioseq-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-11-01 16:20:02.049512 optibioseq-0.1.5/
--rw-rw-rw-   0        0        0      333 2023-11-01 16:20:02.049512 optibioseq-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-11-01 16:20:02.049512 optibioseq-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      824 2023-11-01 16:19:38.000000 optibioseq-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-01 16:20:02.024812 optibioseq-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-11-01 16:20:02.040606 optibioseq-0.1.5/src/optibioseq/
--rw-rw-rw-   0        0        0      116 2023-10-31 17:47:01.000000 optibioseq-0.1.5/src/optibioseq/__init__.py
--rw-rw-rw-   0        0        0      257 2022-02-09 01:16:02.000000 optibioseq-0.1.5/src/optibioseq/__main__.py
--rw-rw-rw-   0        0        0     3324 2022-02-14 16:15:20.000000 optibioseq-0.1.5/src/optibioseq/abc.py
--rw-rw-rw-   0        0        0     7747 2023-10-31 19:22:29.000000 optibioseq-0.1.5/src/optibioseq/bce.py
--rw-rw-rw-   0        0        0     2224 2022-02-14 16:19:59.000000 optibioseq-0.1.5/src/optibioseq/bepi.py
--rw-rw-rw-   0        0        0     3161 2022-02-14 16:29:05.000000 optibioseq-0.1.5/src/optibioseq/iedb1.py
--rw-rw-rw-   0        0        0     3144 2022-02-14 16:50:54.000000 optibioseq-0.1.5/src/optibioseq/iedb2.py
-drwxrwxrwx   0        0        0        0 2023-11-01 16:20:02.049512 optibioseq-0.1.5/src/optibioseq.egg-info/
--rw-rw-rw-   0        0        0      333 2023-11-01 16:20:01.000000 optibioseq-0.1.5/src/optibioseq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-11-01 16:20:02.000000 optibioseq-0.1.5/src/optibioseq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-01 16:20:01.000000 optibioseq-0.1.5/src/optibioseq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-11-01 16:20:01.000000 optibioseq-0.1.5/src/optibioseq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-11-01 16:20:01.000000 optibioseq-0.1.5/src/optibioseq.egg-info/top_level.txt
+drwxrwxrwx   0 ice       (1000) ice       (1000)        0 2024-04-29 21:45:29.434449 optibioseq-0.1.6/
+-rwxrwxrwx   0 ice       (1000) ice       (1000)      311 2024-04-29 21:45:29.437447 optibioseq-0.1.6/PKG-INFO
+-rwxrwxrwx   0 ice       (1000) ice       (1000)       38 2024-04-29 21:45:29.451447 optibioseq-0.1.6/setup.cfg
+-rwxrwxrwx   0 ice       (1000) ice       (1000)      824 2024-04-29 21:42:23.000000 optibioseq-0.1.6/setup.py
+drwxrwxrwx   0 ice       (1000) ice       (1000)        0 2024-04-29 21:45:28.939668 optibioseq-0.1.6/src/
+drwxrwxrwx   0 ice       (1000) ice       (1000)        0 2024-04-29 21:45:29.154685 optibioseq-0.1.6/src/optibioseq/
+-rwxrwxrwx   0 ice       (1000) ice       (1000)      116 2023-10-31 17:47:01.000000 optibioseq-0.1.6/src/optibioseq/__init__.py
+-rwxrwxrwx   0 ice       (1000) ice       (1000)      257 2022-02-09 01:16:02.000000 optibioseq-0.1.6/src/optibioseq/__main__.py
+-rwxrwxrwx   0 ice       (1000) ice       (1000)     3324 2022-02-14 16:15:20.000000 optibioseq-0.1.6/src/optibioseq/abc.py
+-rwxrwxrwx   0 ice       (1000) ice       (1000)     7747 2023-10-31 19:22:29.000000 optibioseq-0.1.6/src/optibioseq/bce.py
+-rwxrwxrwx   0 ice       (1000) ice       (1000)     2224 2022-02-14 16:19:59.000000 optibioseq-0.1.6/src/optibioseq/bepi.py
+-rwxrwxrwx   0 ice       (1000) ice       (1000)     3161 2022-02-14 16:29:05.000000 optibioseq-0.1.6/src/optibioseq/iedb1.py
+-rwxrwxrwx   0 ice       (1000) ice       (1000)     3143 2024-04-29 21:15:37.000000 optibioseq-0.1.6/src/optibioseq/iedb2.py
+drwxrwxrwx   0 ice       (1000) ice       (1000)        0 2024-04-29 21:45:29.349173 optibioseq-0.1.6/src/optibioseq.egg-info/
+-rwxrwxrwx   0 ice       (1000) ice       (1000)      311 2024-04-29 21:45:28.000000 optibioseq-0.1.6/src/optibioseq.egg-info/PKG-INFO
+-rwxrwxrwx   0 ice       (1000) ice       (1000)      376 2024-04-29 21:45:28.000000 optibioseq-0.1.6/src/optibioseq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ice       (1000) ice       (1000)        1 2024-04-29 21:45:28.000000 optibioseq-0.1.6/src/optibioseq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ice       (1000) ice       (1000)       83 2024-04-29 21:45:28.000000 optibioseq-0.1.6/src/optibioseq.egg-info/requires.txt
+-rwxrwxrwx   0 ice       (1000) ice       (1000)       11 2024-04-29 21:45:28.000000 optibioseq-0.1.6/src/optibioseq.egg-info/top_level.txt
```

### Comparing `optibioseq-0.1.5/setup.py` & `optibioseq-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['bs4>=0.0.1,<0.0.2',
  'numpy>=1.22.2,<2.0.0',
  'openpyxl>=3.0.9,<4.0.0',
  'pandas>=1.4.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'optibioseq',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Program that helps wetlab members to analyze results from popular epitope prediction tools',
     'long_description': None,
     'author': 'Iván Corona Guerrero',
     'author_email': '<ivan.corona@uaq.mx>',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `optibioseq-0.1.5/src/optibioseq/abc.py` & `optibioseq-0.1.6/src/optibioseq/abc.py`

 * *Files identical despite different names*

### Comparing `optibioseq-0.1.5/src/optibioseq/bce.py` & `optibioseq-0.1.6/src/optibioseq/bce.py`

 * *Files identical despite different names*

### Comparing `optibioseq-0.1.5/src/optibioseq/bepi.py` & `optibioseq-0.1.6/src/optibioseq/bepi.py`

 * *Files identical despite different names*

### Comparing `optibioseq-0.1.5/src/optibioseq/iedb1.py` & `optibioseq-0.1.6/src/optibioseq/iedb1.py`

 * *Files identical despite different names*

### Comparing `optibioseq-0.1.5/src/optibioseq/iedb2.py` & `optibioseq-0.1.6/src/optibioseq/iedb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     #Lista donde cada renglón se divide como lista
     sopa_table2 = []
     for i in sopa_table:
         sopa_table2.append(i.split())
         #Crear una lista únicamente con los resultados.
     sopa_table3 = []
     for i in sopa_table2:
-        if len(i) == 29:
+        if len(i) == 9:
             sopa_table3.append(i)
     del sopa_table3[0]
     #Hacer una lista con los datos relevantes para el análisis antigénicos
     chosen_ones = []
     for i in sopa_table3:
         if float(i[8]) <= 2:
             chosen_ones.append(i)
```

