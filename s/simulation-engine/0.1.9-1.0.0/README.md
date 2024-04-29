# Comparing `tmp/simulation_engine-0.1.9.tar.gz` & `tmp/simulation-engine-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simulation_engine-0.1.9.tar", last modified: Thu Dec  7 22:20:22 2023, max compression
+gzip compressed data, was "simulation-engine-1.0.0.tar", last modified: Mon Apr 29 04:39:27 2024, max compression
```

## Comparing `simulation_engine-0.1.9.tar` & `simulation-engine-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-12-07 22:20:22.774011 simulation_engine-0.1.9/
--rw-rw-rw-   0        0        0      409 2023-12-07 22:20:22.774011 simulation_engine-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-12-07 22:20:22.774510 simulation_engine-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      745 2023-12-07 22:20:17.000000 simulation_engine-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-07 22:20:22.770507 simulation_engine-0.1.9/simulation_engine/
--rw-rw-rw-   0        0        0     4947 2023-12-07 22:19:18.000000 simulation_engine-0.1.9/simulation_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 22:20:22.773010 simulation_engine-0.1.9/simulation_engine.egg-info/
--rw-rw-rw-   0        0        0      409 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-12-07 22:20:22.000000 simulation_engine-0.1.9/simulation_engine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 04:39:27.316659 simulation-engine-1.0.0/
+-rw-rw-rw-   0        0        0      572 2024-04-29 04:39:27.315660 simulation-engine-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:39:27.316659 simulation-engine-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      840 2024-04-29 04:39:24.000000 simulation-engine-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:39:27.293667 simulation-engine-1.0.0/simulation_engine/
+-rw-rw-rw-   0        0        0       66 2024-04-29 04:31:27.000000 simulation-engine-1.0.0/simulation_engine/__init__.py
+-rw-rw-rw-   0        0        0    17374 2024-04-29 04:35:42.000000 simulation-engine-1.0.0/simulation_engine/simulation_engine.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:39:27.315660 simulation-engine-1.0.0/simulation_engine.egg-info/
+-rw-rw-rw-   0        0        0      572 2024-04-29 04:39:27.000000 simulation-engine-1.0.0/simulation_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-04-29 04:39:27.000000 simulation-engine-1.0.0/simulation_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:39:27.000000 simulation-engine-1.0.0/simulation_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-29 04:39:27.000000 simulation-engine-1.0.0/simulation_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 04:39:27.000000 simulation-engine-1.0.0/simulation_engine.egg-info/top_level.txt
```

### Comparing `simulation_engine-0.1.9/setup.py` & `simulation-engine-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.9' 
-DESCRIPTION = 'Engine for simulating relic drops in Warframe.'
-LONG_DESCRIPTION = 'Engine for simulating relic drops in Warframe, has several features and is very extensible.'
+VERSION = '1.0.0'
+DESCRIPTION = 'Engine for simulating relic in Warframe.'
+LONG_DESCRIPTION = 'Engine that allows the full simluation of any relic in Warframe, shows each individual reward screen as well as the number of each "best drop," the order at which the best drop is chosen is customizable.'
+
 
 setup(
-        name="simulation_engine", 
-        version=VERSION,
-        author="Jacob McBride",
-        author_email="jake55111@gmail.com",
-        description=DESCRIPTION,
-        long_description=LONG_DESCRIPTION,
-        packages=find_packages(),
-        install_requires=['relic_engine'],
-        keywords=['warframe','relics','simulation'],
-        classifiers= [
-            "Programming Language :: Python :: 3",
-            "Operating System :: OS Independent",
-        ]
-)
+    name='simulation-engine',
+    version=VERSION,
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    author='Jacob McBride',
+    author_email='jake55111@gmail.com',
+    packages=find_packages(),
+    keywords=['warframe', 'fissures'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "Operating System :: OS Independent",
+    ],
+    install_requires=[
+        'numpy~=1.26.4',
+        'relic-engine~=0.2.8'
+    ],
+)
```

