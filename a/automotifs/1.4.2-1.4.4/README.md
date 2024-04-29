# Comparing `tmp/automotifs-1.4.2.tar.gz` & `tmp/automotifs-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automotifs-1.4.2.tar", last modified: Sat Apr 20 21:34:42 2024, max compression
+gzip compressed data, was "automotifs-1.4.4.tar", last modified: Mon Apr 29 11:11:19 2024, max compression
```

## Comparing `automotifs-1.4.2.tar` & `automotifs-1.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:34:42.635152 automotifs-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-20 21:34:23.000000 automotifs-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-20 21:34:42.635152 automotifs-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-20 21:34:23.000000 automotifs-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:34:42.631152 automotifs-1.4.2/automotif/
--rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-04-20 21:34:23.000000 automotifs-1.4.2/automotif/GPU_Executor.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-20 21:34:23.000000 automotifs-1.4.2/automotif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17727 2024-04-20 21:34:23.000000 automotifs-1.4.2/automotif/automotif.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:34:42.635152 automotifs-1.4.2/automotifs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-20 21:34:42.000000 automotifs-1.4.2/automotifs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 21:34:42.000000 automotifs-1.4.2/automotifs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 21:34:42.000000 automotifs-1.4.2/automotifs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-20 21:34:42.000000 automotifs-1.4.2/automotifs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-20 21:34:42.000000 automotifs-1.4.2/automotifs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 21:34:42.635152 automotifs-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-20 21:34:23.000000 automotifs-1.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 21:34:42.635152 automotifs-1.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-20 21:34:23.000000 automotifs-1.4.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:11:19.243533 automotifs-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 11:10:55.000000 automotifs-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-29 11:11:19.243533 automotifs-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-29 11:10:55.000000 automotifs-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:11:19.243533 automotifs-1.4.4/automotif/
+-rw-r--r--   0 runner    (1001) docker     (127)    18561 2024-04-29 11:10:55.000000 automotifs-1.4.4/automotif/GPU_Executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 11:10:55.000000 automotifs-1.4.4/automotif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-04-29 11:10:55.000000 automotifs-1.4.4/automotif/automotif.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:11:19.243533 automotifs-1.4.4/automotifs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 11:11:19.000000 automotifs-1.4.4/automotifs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 11:11:19.243533 automotifs-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-29 11:10:55.000000 automotifs-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 11:11:19.243533 automotifs-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-29 11:10:55.000000 automotifs-1.4.4/tests/test.py
```

### Comparing `automotifs-1.4.2/LICENSE` & `automotifs-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automotifs-1.4.2/PKG-INFO` & `automotifs-1.4.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.4.2
+Version: 1.4.4
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.1.5
 Requires-Dist: pylint>=2.6.0
 Requires-Dist: numpy>=1.23
 Requires-Dist: dotmotif>=0.14.0
 Requires-Dist: networkx>=3.2.1
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: seaborn>=0.12.2
 
 # AutoMotif: Automated Motif Detection in Network Graphs
 ## What is it?
 AutoMotif streamlines the identification and cataloging of motifs within network graphs. Utilizing NetworkX for graph manipulation, dotmotif for detecting motifs, and pandas for data management, it simplifies the process of uncovering patterns across both directed and undirected networks. Users can customize searches based on motif size, directionality, executors and the treatment of automorphisms, as well as even having the option to save the results for further analysis.
 
 
 ## Installation
```

### Comparing `automotifs-1.4.2/README.md` & `automotifs-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `automotifs-1.4.2/automotif/GPU_Executor.py` & `automotifs-1.4.4/automotif/GPU_Executor.py`

 * *Files identical despite different names*

### Comparing `automotifs-1.4.2/automotif/automotif.py` & `automotifs-1.4.4/automotif/automotif.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                  upto: bool = False,
                  lower: int = 3, 
                  save: bool = False, 
                  path: str = None,
                  find: bool = False, 
                  verbose: bool = False,
                  use_GrandISO: bool = False,
-                 use_GPU: bool = False
+                 use_GPU: bool = False,
                  personal_executor: executors.Executor = None):
         if not hasattr(Graph, "nodes") or not callable(getattr(Graph, "nodes")):
             raise ValueError("Graph should be a NetworkX graph")
         elif type(size) != int:
             raise ValueError("Size should be an integer")
         elif type(upto) != bool:
             raise ValueError("Upto should be a boolean")
```

### Comparing `automotifs-1.4.2/automotifs.egg-info/PKG-INFO` & `automotifs-1.4.4/automotifs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: automotifs
-Version: 1.4.2
+Version: 1.4.4
 Summary: A wrapper for automatic Motif Detection
 Home-page: https://github.com/GiorgioMB/auto_dotmotif/
 Author: Giorgio Micaletto
 Author-email: giorgio.micaletto@studbocconi.it
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=1.1.5
 Requires-Dist: pylint>=2.6.0
 Requires-Dist: numpy>=1.23
 Requires-Dist: dotmotif>=0.14.0
 Requires-Dist: networkx>=3.2.1
+Requires-Dist: matplotlib>=3.8.0
+Requires-Dist: seaborn>=0.12.2
 
 # AutoMotif: Automated Motif Detection in Network Graphs
 ## What is it?
 AutoMotif streamlines the identification and cataloging of motifs within network graphs. Utilizing NetworkX for graph manipulation, dotmotif for detecting motifs, and pandas for data management, it simplifies the process of uncovering patterns across both directed and undirected networks. Users can customize searches based on motif size, directionality, executors and the treatment of automorphisms, as well as even having the option to save the results for further analysis.
 
 
 ## Installation
```

### Comparing `automotifs-1.4.2/setup.py` & `automotifs-1.4.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,27 +7,29 @@
     def run(self):
         install.run(self)
         # Running pip install for nx-cugraph with the specified extra index URL
         os.system("pip install nx-cugraph-cu11 --extra-index-url https://pypi.nvidia.com")
 
 setup(
     name='automotifs',
-    version='1.4.2', 
+    version='1.4.4', 
     packages=find_packages(),
     description='A wrapper for automatic Motif Detection',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Micaletto',
     author_email='giorgio.micaletto@studbocconi.it',
     url='https://github.com/GiorgioMB/auto_dotmotif/',
     install_requires=[
         'pandas>=1.1.5',
         'pylint>=2.6.0',
         'numpy>=1.23',
         'dotmotif>=0.14.0',
-        'networkx>=3.2.1'
+        'networkx>=3.2.1',
+        'matplotlib>=3.8.0',
+        'seaborn>=0.12.2'
     ],
     python_requires='>=3.6',
     cmdclass={
         'install': PostInstallCommand,
     }
 )
```

### Comparing `automotifs-1.4.2/tests/test.py` & `automotifs-1.4.4/tests/test.py`

 * *Files identical despite different names*

