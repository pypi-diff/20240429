# Comparing `tmp/chroptiks-0.1.3.tar.gz` & `tmp/chroptiks-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chroptiks-0.1.3.tar", last modified: Mon Nov 20 17:48:47 2023, max compression
+gzip compressed data, was "chroptiks-0.1.4.tar", last modified: Mon Apr 29 06:02:10 2024, max compression
```

## Comparing `chroptiks-0.1.3.tar` & `chroptiks-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 cagostino   (503) staff       (20)        0 2023-11-20 17:48:47.070462 chroptiks-0.1.3/
--rw-r--r--   0 cagostino   (503) staff       (20)     3149 2023-11-20 17:48:47.070279 chroptiks-0.1.3/PKG-INFO
--rw-r--r--   0 cagostino   (503) staff       (20)     2759 2023-11-20 17:48:06.000000 chroptiks-0.1.3/README.md
-drwxr-xr-x   0 cagostino   (503) staff       (20)        0 2023-11-20 17:48:47.068352 chroptiks-0.1.3/chroptiks/
--rw-r--r--   0 cagostino   (503) staff       (20)        0 2023-11-17 14:09:58.000000 chroptiks-0.1.3/chroptiks/__init__.py
--rw-r--r--   0 cagostino   (503) staff       (20)    17248 2023-11-17 19:09:54.000000 chroptiks-0.1.3/chroptiks/plotting_utils.py
-drwxr-xr-x   0 cagostino   (503) staff       (20)        0 2023-11-20 17:48:47.069945 chroptiks-0.1.3/chroptiks.egg-info/
--rw-r--r--   0 cagostino   (503) staff       (20)     3149 2023-11-20 17:48:47.000000 chroptiks-0.1.3/chroptiks.egg-info/PKG-INFO
--rw-r--r--   0 cagostino   (503) staff       (20)      232 2023-11-20 17:48:47.000000 chroptiks-0.1.3/chroptiks.egg-info/SOURCES.txt
--rw-r--r--   0 cagostino   (503) staff       (20)        1 2023-11-20 17:48:47.000000 chroptiks-0.1.3/chroptiks.egg-info/dependency_links.txt
--rw-r--r--   0 cagostino   (503) staff       (20)       23 2023-11-20 17:48:47.000000 chroptiks-0.1.3/chroptiks.egg-info/requires.txt
--rw-r--r--   0 cagostino   (503) staff       (20)       10 2023-11-20 17:48:47.000000 chroptiks-0.1.3/chroptiks.egg-info/top_level.txt
--rw-r--r--   0 cagostino   (503) staff       (20)       38 2023-11-20 17:48:47.070503 chroptiks-0.1.3/setup.cfg
--rw-r--r--   0 cagostino   (503) staff       (20)      722 2023-11-20 17:48:39.000000 chroptiks-0.1.3/setup.py
+drwxrwxr-x   0 caug      (1000) caug      (1000)        0 2024-04-29 06:02:10.508986 chroptiks-0.1.4/
+-rw-r--r--   0 caug      (1000) caug      (1000)     2801 2024-04-29 06:02:10.508986 chroptiks-0.1.4/PKG-INFO
+-rw-rw-r--   0 caug      (1000) caug      (1000)     2365 2024-04-29 05:57:47.000000 chroptiks-0.1.4/README.md
+drwxrwxr-x   0 caug      (1000) caug      (1000)        0 2024-04-29 06:02:10.508986 chroptiks-0.1.4/chroptiks/
+-rw-rw-r--   0 caug      (1000) caug      (1000)        0 2024-04-29 05:14:41.000000 chroptiks-0.1.4/chroptiks/__init__.py
+-rw-rw-r--   0 caug      (1000) caug      (1000)    26925 2024-04-29 05:38:59.000000 chroptiks-0.1.4/chroptiks/plotting_utils.py
+drwxrwxr-x   0 caug      (1000) caug      (1000)        0 2024-04-29 06:02:10.508986 chroptiks-0.1.4/chroptiks.egg-info/
+-rw-r--r--   0 caug      (1000) caug      (1000)     2801 2024-04-29 06:02:10.000000 chroptiks-0.1.4/chroptiks.egg-info/PKG-INFO
+-rw-rw-r--   0 caug      (1000) caug      (1000)      232 2024-04-29 06:02:10.000000 chroptiks-0.1.4/chroptiks.egg-info/SOURCES.txt
+-rw-rw-r--   0 caug      (1000) caug      (1000)        1 2024-04-29 06:02:10.000000 chroptiks-0.1.4/chroptiks.egg-info/dependency_links.txt
+-rw-rw-r--   0 caug      (1000) caug      (1000)       23 2024-04-29 06:02:10.000000 chroptiks-0.1.4/chroptiks.egg-info/requires.txt
+-rw-rw-r--   0 caug      (1000) caug      (1000)       10 2024-04-29 06:02:10.000000 chroptiks-0.1.4/chroptiks.egg-info/top_level.txt
+-rw-rw-r--   0 caug      (1000) caug      (1000)       38 2024-04-29 06:02:10.508986 chroptiks-0.1.4/setup.cfg
+-rw-rw-r--   0 caug      (1000) caug      (1000)      700 2024-04-29 05:56:10.000000 chroptiks-0.1.4/setup.py
```

### Comparing `chroptiks-0.1.3/PKG-INFO` & `chroptiks-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,45 @@
 Metadata-Version: 2.1
 Name: chroptiks
-Version: 0.1.3
-Summary: A set of helper functions for quickly making matplotlib plots using latex fonts and with a high number of built-in options.
+Version: 0.1.4
+Summary: A set of helper functions for quickly making matplotlib plots with a high number of built-in options.
 Home-page: https://github.com/cagostino/chroptiks
 Author: Chris Agostino
 Author-email: cjp.agostino@gmail.com
 License: MIT
 Keywords: matplotlib plotting utilities
 Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
 
 # chroptiks
 
 ## Description
 chroptiks is a Python package that offers advanced plotting utilities, making it easier to create complex and informative visualizations. It extends the functionality of libraries like matplotlib and scipy, providing a user-friendly interface for a variety of plotting needs.
 
 
 ## Requirements
 
 Python libraries: matplotlib, numpy, scipy
 
-Other: LaTeX. If you don't want to use LaTeX in the plotting, edit the `plotting_utils.py` file and either comment out the line : `plt.rc('text', usetex=True)`, or set the `usetex` keyword to be `False` before installing the package. 
-
-
 ## Installation
 
-To install chroptiks from source, run:
+To install chroptiks, run:
 
 ```bash
-git clone https://github.com/cagostino/chroptiks.git
-cd chroptiks
-python setup.py install
+pip install chroptiks
 ```
-Otherwise simply install from pip:
 
+or if you want to install from source:
 ```bash
-pip install chroptiks
+git clone https://github.com/cagostino/chroptiks.git
+cd chroptiks
+python setup.py install
 ```
-## Usage
-
-Here's how you can use your_package_name in your projects:
-
-from chroptiks.plotting_utils import hist2d, hist1d, scatter, plot3d, plotbar
-
 
 
 ## Features
 
 ---2D Histograms (hist2d): Easily create 2D histograms for data analysis.
 
 ---1D Histograms (hist1d): Simplify the process of creating and customizing 1D histograms.
```

### Comparing `chroptiks-0.1.3/README.md` & `chroptiks-0.1.4/chroptiks.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+Metadata-Version: 2.1
+Name: chroptiks
+Version: 0.1.4
+Summary: A set of helper functions for quickly making matplotlib plots with a high number of built-in options.
+Home-page: https://github.com/cagostino/chroptiks
+Author: Chris Agostino
+Author-email: cjp.agostino@gmail.com
+License: MIT
+Keywords: matplotlib plotting utilities
+Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: scipy
+
 # chroptiks
 
 ## Description
 chroptiks is a Python package that offers advanced plotting utilities, making it easier to create complex and informative visualizations. It extends the functionality of libraries like matplotlib and scipy, providing a user-friendly interface for a variety of plotting needs.
 
 
 ## Requirements
 
 Python libraries: matplotlib, numpy, scipy
 
-Other: LaTeX. If you don't want to use LaTeX in the plotting, edit the `plotting_utils.py` file and either comment out the line : `plt.rc('text', usetex=True)`, or set the `usetex` keyword to be `False` before installing the package. 
-
-
 ## Installation
 
-To install chroptiks from source, run:
+To install chroptiks, run:
 
 ```bash
-git clone https://github.com/cagostino/chroptiks.git
-cd chroptiks
-python setup.py install
+pip install chroptiks
 ```
-Otherwise simply install from pip:
 
+or if you want to install from source:
 ```bash
-pip install chroptiks
+git clone https://github.com/cagostino/chroptiks.git
+cd chroptiks
+python setup.py install
 ```
-## Usage
-
-Here's how you can use your_package_name in your projects:
-
-from chroptiks.plotting_utils import hist2d, hist1d, scatter, plot3d, plotbar
-
 
 
 ## Features
 
 ---2D Histograms (hist2d): Easily create 2D histograms for data analysis.
 
 ---1D Histograms (hist1d): Simplify the process of creating and customizing 1D histograms.
```

### Comparing `chroptiks-0.1.3/chroptiks.egg-info/PKG-INFO` & `chroptiks-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,31 @@
-Metadata-Version: 2.1
-Name: chroptiks
-Version: 0.1.3
-Summary: A set of helper functions for quickly making matplotlib plots using latex fonts and with a high number of built-in options.
-Home-page: https://github.com/cagostino/chroptiks
-Author: Chris Agostino
-Author-email: cjp.agostino@gmail.com
-License: MIT
-Keywords: matplotlib plotting utilities
-Description-Content-Type: text/markdown
-
 # chroptiks
 
 ## Description
 chroptiks is a Python package that offers advanced plotting utilities, making it easier to create complex and informative visualizations. It extends the functionality of libraries like matplotlib and scipy, providing a user-friendly interface for a variety of plotting needs.
 
 
 ## Requirements
 
 Python libraries: matplotlib, numpy, scipy
 
-Other: LaTeX. If you don't want to use LaTeX in the plotting, edit the `plotting_utils.py` file and either comment out the line : `plt.rc('text', usetex=True)`, or set the `usetex` keyword to be `False` before installing the package. 
-
-
 ## Installation
 
-To install chroptiks from source, run:
+To install chroptiks, run:
 
 ```bash
-git clone https://github.com/cagostino/chroptiks.git
-cd chroptiks
-python setup.py install
+pip install chroptiks
 ```
-Otherwise simply install from pip:
 
+or if you want to install from source:
 ```bash
-pip install chroptiks
+git clone https://github.com/cagostino/chroptiks.git
+cd chroptiks
+python setup.py install
 ```
-## Usage
-
-Here's how you can use your_package_name in your projects:
-
-from chroptiks.plotting_utils import hist2d, hist1d, scatter, plot3d, plotbar
-
 
 
 ## Features
 
 ---2D Histograms (hist2d): Easily create 2D histograms for data analysis.
 
 ---1D Histograms (hist1d): Simplify the process of creating and customizing 1D histograms.
```

### Comparing `chroptiks-0.1.3/setup.py` & `chroptiks-0.1.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chroptiks',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     install_requires=[
         'matplotlib', 'numpy', 'scipy'  # Add your dependencies here
     ],
     # Additional metadata
     author='Chris Agostino',
     author_email='cjp.agostino@gmail.com',
     long_description=open('README.md').read(),  # or README.rst if using RST
     long_description_content_type='text/markdown',
 
-    description='A set of helper functions for quickly making matplotlib plots using latex fonts and with a high number of built-in options.',
+    description='A set of helper functions for quickly making matplotlib plots with a high number of built-in options.',
     license='MIT',
     keywords='matplotlib plotting utilities',
     url='https://github.com/cagostino/chroptiks', # Optional
 )
```

