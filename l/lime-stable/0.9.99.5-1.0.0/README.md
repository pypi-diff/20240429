# Comparing `tmp/lime-stable-0.9.99.5.tar.gz` & `tmp/lime-stable-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lime-stable-0.9.99.5.tar", last modified: Fri Apr  5 18:40:01 2024, max compression
+gzip compressed data, was "lime-stable-1.0.0.tar", last modified: Mon Apr 29 20:58:27 2024, max compression
```

## Comparing `lime-stable-0.9.99.5.tar` & `lime-stable-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,44 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/
--rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/LICENSE.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)      144 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/MANIFEST.in
--rw-r--r--   0 vital     (1000) vital     (1000)     3638 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     2684 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/README.rst
--rw-rw-r--   0 vital     (1000) vital     (1000)     1149 2024-04-05 18:12:49.000000 lime-stable-0.9.99.5/pyproject.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)      436 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)     1367 2024-02-07 20:40:09.000000 lime-stable-0.9.99.5/setup.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.426581 lime-stable-0.9.99.5/src/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/src/lime/
--rw-rw-r--   0 vital     (1000) vital     (1000)     1528 2024-04-03 19:45:09.000000 lime-stable-0.9.99.5/src/lime/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2438 2024-04-05 18:12:49.000000 lime-stable-0.9.99.5/src/lime/config.toml
--rw-rw-r--   0 vital     (1000) vital     (1000)    31035 2024-04-04 18:46:13.000000 lime-stable-0.9.99.5/src/lime/io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2809 2024-03-20 19:32:47.000000 lime-stable-0.9.99.5/src/lime/logo.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    38583 2024-04-05 18:09:59.000000 lime-stable-0.9.99.5/src/lime/model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    73078 2024-04-05 15:48:29.000000 lime-stable-0.9.99.5/src/lime/observations.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    82193 2024-04-05 14:08:28.000000 lime-stable-0.9.99.5/src/lime/plots.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    70363 2024-04-04 22:15:39.000000 lime-stable-0.9.99.5/src/lime/plots_interactive.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    31175 2024-03-22 14:35:43.000000 lime-stable-0.9.99.5/src/lime/read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17248 2024-04-04 14:44:02.000000 lime-stable-0.9.99.5/src/lime/recognition.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/src/lime/resources/
--rw-rw-r--   0 vital     (1000) vital     (1000)     1100 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/src/lime/resources/GradientDescent_v2_cost1_logNorm.joblib
--rw-rw-r--   0 vital     (1000) vital     (1000)      858 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/src/lime/resources/LogitistRegression_v2_cost1_logNorm.joblib
--rw-rw-r--   0 vital     (1000) vital     (1000)      144 2024-04-05 15:26:56.000000 lime-stable-0.9.99.5/src/lime/resources/adjust_bands_database.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-05 15:27:04.000000 lime-stable-0.9.99.5/src/lime/resources/parent_bands.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    16094 2024-04-05 15:05:16.000000 lime-stable-0.9.99.5/src/lime/resources/parent_mask_v0.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     2842 2024-01-06 20:52:21.000000 lime-stable-0.9.99.5/src/lime/resources/sketch.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     9855 2024-03-27 17:47:48.000000 lime-stable-0.9.99.5/src/lime/resources/types_params.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)     9100 2024-01-31 19:44:41.000000 lime-stable-0.9.99.5/src/lime/resources/types_params2.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)    14172 2024-02-13 22:39:44.000000 lime-stable-0.9.99.5/src/lime/tables.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    37522 2024-04-03 15:58:07.000000 lime-stable-0.9.99.5/src/lime/tools.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    27774 2024-04-05 15:01:34.000000 lime-stable-0.9.99.5/src/lime/transitions.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    35814 2024-04-03 15:31:58.000000 lime-stable-0.9.99.5/src/lime/workflow.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/src/lime_stable.egg-info/
--rw-r--r--   0 vital     (1000) vital     (1000)     3638 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)     1079 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)      257 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/requires.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-04-05 18:40:01.000000 lime-stable-0.9.99.5/src/lime_stable.egg-info/top_level.txt
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-05 18:40:01.430581 lime-stable-0.9.99.5/tests/
--rw-rw-r--   0 vital     (1000) vital     (1000)      993 2024-04-02 21:30:23.000000 lime-stable-0.9.99.5/tests/test_astro.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7092 2024-04-02 21:30:24.000000 lime-stable-0.9.99.5/tests/test_cube.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     3549 2024-04-02 21:30:23.000000 lime-stable-0.9.99.5/tests/test_io.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     7626 2024-04-05 15:36:26.000000 lime-stable-0.9.99.5/tests/test_line.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     4388 2024-02-15 20:55:38.000000 lime-stable-0.9.99.5/tests/test_model.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     2346 2024-01-16 14:15:34.000000 lime-stable-0.9.99.5/tests/test_read_fits.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     1997 2024-04-02 21:30:23.000000 lime-stable-0.9.99.5/tests/test_sample.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    11168 2024-04-02 21:34:26.000000 lime-stable-0.9.99.5/tests/test_spectrum.py
--rw-rw-r--   0 vital     (1000) vital     (1000)    13366 2024-04-02 21:30:23.000000 lime-stable-0.9.99.5/tests/test_tools.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    35608 2024-04-25 13:12:45.000000 lime-stable-1.0.0/LICENSE.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)       63 2024-04-25 13:06:20.000000 lime-stable-1.0.0/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-04-29 20:58:27.066953 lime-stable-1.0.0/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2647 2024-04-25 13:09:22.000000 lime-stable-1.0.0/README.rst
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1179 2024-04-29 20:55:52.000000 lime-stable-1.0.0/pyproject.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)      433 2024-04-29 20:58:27.066953 lime-stable-1.0.0/setup.cfg
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1187 2024-04-25 13:12:39.000000 lime-stable-1.0.0/setup.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.062950 lime-stable-1.0.0/src/
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/src/lime/
+-rw-rw-r--   0 vital     (1000) vital     (1000)     1307 2024-04-25 21:14:21.000000 lime-stable-1.0.0/src/lime/__init__.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3492 2024-04-29 17:25:52.000000 lime-stable-1.0.0/src/lime/config.toml
+-rw-rw-r--   0 vital     (1000) vital     (1000)    30968 2024-04-28 17:14:36.000000 lime-stable-1.0.0/src/lime/io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2795 2024-04-24 14:30:56.000000 lime-stable-1.0.0/src/lime/logo.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    38372 2024-04-29 17:41:51.000000 lime-stable-1.0.0/src/lime/model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    73382 2024-04-29 17:38:28.000000 lime-stable-1.0.0/src/lime/observations.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    82059 2024-04-29 17:23:37.000000 lime-stable-1.0.0/src/lime/plots.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    70627 2024-04-29 17:28:58.000000 lime-stable-1.0.0/src/lime/plots_interactive.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    33262 2024-04-29 19:41:49.000000 lime-stable-1.0.0/src/lime/read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    20126 2024-04-28 17:14:36.000000 lime-stable-1.0.0/src/lime/recognition.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/src/lime/resources/
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:04:12.000000 lime-stable-1.0.0/src/lime/resources/parent_bands.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    17051 2024-04-25 13:03:27.000000 lime-stable-1.0.0/src/lime/resources/parent_bands_BackUp.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    10111 2024-04-22 21:42:02.000000 lime-stable-1.0.0/src/lime/resources/types_params.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)    14146 2024-04-25 13:02:58.000000 lime-stable-1.0.0/src/lime/tables.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    34912 2024-04-28 17:14:36.000000 lime-stable-1.0.0/src/lime/tools.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    29081 2024-04-25 14:14:19.000000 lime-stable-1.0.0/src/lime/transitions.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    37147 2024-04-29 02:03:22.000000 lime-stable-1.0.0/src/lime/workflow.py
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/src/lime_stable.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)     3623 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/PKG-INFO
+-rw-rw-r--   0 vital     (1000) vital     (1000)      853 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/SOURCES.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        1 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/dependency_links.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)      252 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/requires.txt
+-rw-rw-r--   0 vital     (1000) vital     (1000)        5 2024-04-29 20:58:27.000000 lime-stable-1.0.0/src/lime_stable.egg-info/top_level.txt
+drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2024-04-29 20:58:27.066953 lime-stable-1.0.0/tests/
+-rw-rw-r--   0 vital     (1000) vital     (1000)      994 2024-04-24 14:46:28.000000 lime-stable-1.0.0/tests/test_astro.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7088 2024-04-16 20:37:49.000000 lime-stable-1.0.0/tests/test_cube.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     3550 2024-04-24 14:46:41.000000 lime-stable-1.0.0/tests/test_io.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     7795 2024-04-24 16:03:41.000000 lime-stable-1.0.0/tests/test_line.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4345 2024-04-25 13:05:21.000000 lime-stable-1.0.0/tests/test_model.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     4624 2024-04-24 15:30:23.000000 lime-stable-1.0.0/tests/test_read_fits.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)     2013 2024-04-10 16:19:13.000000 lime-stable-1.0.0/tests/test_sample.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    11180 2024-04-24 14:43:43.000000 lime-stable-1.0.0/tests/test_spectrum.py
+-rw-rw-r--   0 vital     (1000) vital     (1000)    13391 2024-04-24 14:25:22.000000 lime-stable-1.0.0/tests/test_tools.py
```

### Comparing `lime-stable-0.9.99.5/LICENSE.rst` & `lime-stable-1.0.0/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 The line measuring library for ionized nebulae (lime) is available under
 the GNU licence (see below) providing you cite the developer Vital Fernandez using the following reference
 
-* Fernandez et al (2021)
+* Fernandez et al (2024)
 
 
 GNU GENERAL PUBLIC LICENSE
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Version 3, 29 June 2007
```

### Comparing `lime-stable-0.9.99.5/PKG-INFO` & `lime-stable-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 0.9.99.5
+Version: 1.0.0
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: joblib==1.3.1
-Requires-Dist: lmfit==1.2.2
-Requires-Dist: matplotlib==3.7.2
-Requires-Dist: mplcursors==0.5.2
-Requires-Dist: nbsphinx==0.9.2
-Requires-Dist: numpy==1.24.4
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: pandas==2.0.3
-Requires-Dist: PyLaTeX==1.4.1
-Requires-Dist: pytest==7.4.0
-Requires-Dist: pytest-cov==4.1.0
-Requires-Dist: pytest-mpl==0.16.1
-Requires-Dist: scipy==1.10.1
-Requires-Dist: toml==0.10.2
+Requires-Dist: asdf~=3.0
+Requires-Dist: astropy~=6.0
+Requires-Dist: joblib~=1.3
+Requires-Dist: lmfit~=1.2
+Requires-Dist: matplotlib~=3.7
+Requires-Dist: mplcursors~=0.5
+Requires-Dist: nbsphinx~=0.9
+Requires-Dist: numpy~=1.24
+Requires-Dist: openpyxl~=3.1
+Requires-Dist: pandas~=2.0
+Requires-Dist: PyLaTeX~=1.4
+Requires-Dist: pytest~=7.4
+Requires-Dist: pytest-cov~=4.1
+Requires-Dist: pytest-mpl~=0.16
+Requires-Dist: scipy~=1.10
+Requires-Dist: toml~=0.10
 Requires-Dist: tomli>=2.0.0; python_version < "3.11"
 
 
 .. image:: https://github.com/Vital-Fernandez/lime/blob/0afedb150b0169deec6c7f159def99750a3a30da/docs/source/_static/logo_transparent.png?raw=true
     :width: 50%
     :align: center
     :alt: Line Measurer (LiMe) library.
 
 |Repo status| |CI badge| |Documentation Status| |Code cov| |PyPI version| |PyPI downloads| |Code Size| |PyPI license|
 
 This library provides a set of tools to fit lines in astronomical spectra. Its design aims for a user-friendly workflow
-for both single lines and large data sets. The library provides tools for masking, detecting, profile fitting
-and storing the results. . The output measurements are focused on the gas chemical and kinematic analysis.
+for both single lines and large data sets. The functions can be used for masking data, detecting lines, fitting profiles
+and storing the results. The output measurements support the chemical and kinematic analysis of the observed transitions.
 
 Please check the `online documentation <https://lime-stable.readthedocs.io/>`_.
 
 Installation
 ============
 
 The library can be installed directly from its PyPi_ project page running the command:
 
 ``pip install lime-stable``
 
 Development
 ===========
 
-LiMe is currently in a beta release. Please check its github_ for the latest version news and tutorials.
-Any comment/issue/request can be added as an issue on the github_ page.
+LiMe is currently on its initial release. Any comment/issue/request can be added as an issue on the github_ page.
 
 .. _PyPi: https://pypi.org/project/lime-stable/
 .. _github: https://github.com/Vital-Fernandez/lime
 
 .. |Repo status| image:: http://www.repostatus.org/badges/latest/active.svg
     :target: http://www.repostatus.org/#active
     :alt: Project Status: Active – The project has reached a stable, usable state and is being actively developed.
```

### Comparing `lime-stable-0.9.99.5/README.rst` & `lime-stable-1.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,31 +3,30 @@
     :width: 50%
     :align: center
     :alt: Line Measurer (LiMe) library.
 
 |Repo status| |CI badge| |Documentation Status| |Code cov| |PyPI version| |PyPI downloads| |Code Size| |PyPI license|
 
 This library provides a set of tools to fit lines in astronomical spectra. Its design aims for a user-friendly workflow
-for both single lines and large data sets. The library provides tools for masking, detecting, profile fitting
-and storing the results. . The output measurements are focused on the gas chemical and kinematic analysis.
+for both single lines and large data sets. The functions can be used for masking data, detecting lines, fitting profiles
+and storing the results. The output measurements support the chemical and kinematic analysis of the observed transitions.
 
 Please check the `online documentation <https://lime-stable.readthedocs.io/>`_.
 
 Installation
 ============
 
 The library can be installed directly from its PyPi_ project page running the command:
 
 ``pip install lime-stable``
 
 Development
 ===========
 
-LiMe is currently in a beta release. Please check its github_ for the latest version news and tutorials.
-Any comment/issue/request can be added as an issue on the github_ page.
+LiMe is currently on its initial release. Any comment/issue/request can be added as an issue on the github_ page.
 
 .. _PyPi: https://pypi.org/project/lime-stable/
 .. _github: https://github.com/Vital-Fernandez/lime
 
 .. |Repo status| image:: http://www.repostatus.org/badges/latest/active.svg
     :target: http://www.repostatus.org/#active
     :alt: Project Status: Active – The project has reached a stable, usable state and is being actively developed.
```

### Comparing `lime-stable-0.9.99.5/pyproject.toml` & `lime-stable-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 [project]
 name = "lime-stable"
-version = "0.9.99.5"
+version = "1.0.0"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "COPYING"}
 authors = [{name = "Vital Fernández", email = "vgf@umich.edu"}]
 description = "Line measuring algorithm for astronomical spectra"
 
-dependencies = ["joblib==1.3.1",
-                "lmfit==1.2.2",
-                "matplotlib==3.7.2",
-                "mplcursors==0.5.2",
-                "nbsphinx==0.9.2",
-                "numpy==1.24.4",
-                "openpyxl==3.1.2",
-                "pandas==2.0.3",
-                "PyLaTeX==1.4.1",
-                "pytest==7.4.0",
-                "pytest-cov==4.1.0",
-                "pytest-mpl==0.16.1",
-                "scipy==1.10.1",
-                "toml==0.10.2",
+dependencies = ["asdf~=3.0",
+                "astropy~=6.0",
+                "joblib~=1.3",
+                "lmfit~=1.2",
+                "matplotlib~=3.7",
+                "mplcursors~=0.5",
+                "nbsphinx~=0.9",
+                "numpy~=1.24",
+                "openpyxl~=3.1",
+                "pandas~=2.0",
+                "PyLaTeX~=1.4",
+                "pytest~=7.4",
+                "pytest-cov~=4.1",
+                "pytest-mpl~=0.16",
+                "scipy~=1.10",
+                "toml~=0.10",
                 "tomli >= 2.0.0 ; python_version < '3.11'"]
 
 classifiers = ["License :: OSI Approved :: MIT License",
                "Programming Language :: Python :: 3",
                "Programming Language :: Python :: 3.7"]
 
 [tool.pytest.ini_options]
```

### Comparing `lime-stable-0.9.99.5/src/lime/__init__.py` & `lime-stable-1.0.0/src/lime/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 LiMe - A python package for measuring lines in astronomical spectra
 """
 
 import os
 import sys
-import configparser
 import logging
 from pathlib import Path
 
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
@@ -21,20 +20,14 @@
 consoleHandle = logging.StreamHandler()
 consoleHandle.setFormatter(logging.Formatter('%(name)s %(levelname)s: %(message)s'))
 _logger.addHandler(consoleHandle)
 
 # Get python version being used
 __python_version__ = sys.version_info
 
-# Read lime configuration .ini
-# _dir_path = os.path.dirname(os.path.realpath(__file__))
-# _setup_cfg = configparser.ConfigParser()
-# _setup_cfg.optionxform = str
-# _setup_cfg.read(os.path.join(_dir_path, 'config.toml'))
-
 # Read lime configuration .toml
 _inst_dir = Path(__file__).parent
 _conf_path = _inst_dir/'config.toml'
 with open(_conf_path, mode="rb") as fp:
     _setup_cfg = tomllib.load(fp)
 
 __version__ = _setup_cfg['metadata']['version']
@@ -47,10 +40,10 @@
 class Error(Exception):
     """LiMe exception function"""
 
 from .observations import Spectrum, Sample, Cube, line_bands
 from .io import *
 from .tools import *
 from .transitions import Line, label_decomposition
-from .read_fits import OpenFits
+from .read_fits import OpenFits, show_instrument_cfg
 from .recognition import detection_function
 from .plots import theme
```

### Comparing `lime-stable-0.9.99.5/src/lime/config.toml` & `lime-stable-1.0.0/src/lime/config.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [metadata]
 name = 'lime-stable'
-version = '0.9.99.5'
+version = '1.0.0'
 
-[lime_colors]
-
-#Default
+[colors] #Default theme
 default.bg = '#FFFFFF'
 default.fg = '#000000'
 default.cont_band = '#8c564b'
 default.line_band = '#b5bd61'
 default.color_cycle = ['#279e68', '#d62728', '#aa40fc', '#8c564b',  '#e377c2', '#7f7f7f',
                        '#b5bd61', '#17becf', '#1f77b4', '#ff7f0e']
 default.match_line = '#b5bd61'
@@ -18,43 +16,65 @@
 default.cont = '#ff7f0e'
 default.error = '#FF0000'
 default.mask_map = 'viridis'
 default.comps_map = 'Dark2'
 default.mask_marker = '#FF0000'
 default.inspection_positive = '#FFFFFF'
 default.inspection_negative = '#ff796c' # 'xkcd:salmon'
+default.fade_fg = "#CCCCCC"
 
+default.single_width = '1'
+default.comp_width = '0.75'
+default.err_width = '2'
+default.cont_width = '0.5'
+default.spectrum_width = '0.75'
 
 #Dark theme
 dark.bg = "#2B2B2B"
 dark.fg = "#CCCCCC"
 dark.cont_band = '#e7298a'
 dark.line_band = '#8fff9f'
 dark.color_cycle = ['#66c2a5', '#fc8d62', '#e68ac3', '#a6d854',  '#ffd92f', '#e5c494',
                        '#8dcbe2', '#e7298a', '#332288', '#88ccee']
 dark.match_line = '#8fff9f'
 dark.peak = '#aa40fc'
 dark.trough = '#7f7f7f'
-dark.profile = '#ddcc77' #'#ffd92f' #'#8dcbe2'
+dark.profile = '#ddcc77'
 dark.cont = "#CCCCCC"
 dark.error = '#FF0000'
 dark.mask_map = 'viridis'
 dark.comps_map = 'PuRd'
 dark.mask_marker = '#FF0000'
 dark.inspection_positive = "#2B2B2B"
 dark.inspection_negative = '#840000'
+dark.fade_fg = "#73879B"
+
+dark.single_width = '2'
+dark.comp_width = '1.5'
+dark.err_width = '3'
+dark.cont_width = '0.5'
+dark.spectrum_width = '0.75'
 
 [matplotlib]
 default."figure.dpi" = 200
-default."figure.figsize" = [8, 5]
-default."axes.titlesize" = 14
-default."axes.labelsize" = 14
-default."legend.fontsize" = 12
-default."xtick.labelsize" = 13
-default."ytick.labelsize" = 13
+default."figure.figsize" = [4.85, 3]
+default."axes.titlesize" = 9
+default."axes.labelsize" = 9
+default."legend.fontsize" = 7
+default."xtick.labelsize" = 8
+default."ytick.labelsize" = 8
+default."font.size" = 5
+
+#default."figure.dpi" = 150
+#default."figure.figsize" = [8, 5]
+#default."axes.titlesize" = 14
+#default."axes.labelsize" = 14
+#default."legend.fontsize" = 12
+#default."xtick.labelsize" = 13
+#default."ytick.labelsize" = 13
 
 high_res."figure.dpi" = 300
 high_res."figure.figsize" = [11, 6]
 high_res."axes.titlesize" = 14
 high_res."axes.labelsize" = 14
 high_res."legend.fontsize" = 12
 high_res."xtick.labelsize" = 12
@@ -69,19 +89,39 @@
 dark.'xtick.color'= "#CCCCCC"
 dark.'ytick.color'= "#CCCCCC"
 dark."text.color" = "#CCCCCC"
 dark."legend.edgecolor" = "inherit"
 dark."legend.facecolor" = "inherit"
 
 # Bands plot
-bands."axes.labelsize" = 14
+bands."axes.labelsize" = 8
+bands."legend.fontsize" = 5
 
 # Grid plot
-grid."axes.titlesize" = 12
+grid."axes.titlesize" = 6
+grid."axes.titlepad" = 1
+
+# Cube
+cube."legend.fontsize" = 5
+cube."axes.titlesize" = 6
+cube."axes.labelsize" = 6
+cube."xtick.labelsize" = 4
+cube."ytick.labelsize" = 4
+
 
 # Cube interactive
-cube_interactive.'figure.figsize' = [16, 8]
-cube_interactive.'axes.titlesize' = 12
-cube_interactive.'legend.fontsize' = 12
-cube_interactive.'axes.labelsize' = 12
-cube_interactive.'xtick.labelsize' = 10
-cube_interactive.'ytick.labelsize' = 10
+cube_interactive.'figure.figsize' = [6.85, 3]
+cube_interactive.'axes.titlesize' = 6
+cube_interactive.'legend.fontsize' = 6
+cube_interactive.'axes.labelsize' = 6
+cube_interactive.'xtick.labelsize' = 4
+cube_interactive.'ytick.labelsize' = 4
+cube_interactive."contour.linewidth" = 0.75
+cube_interactive."axes.labelpad" = 1
+
+#cube_interactive.'figure.figsize' = [16, 8]
+#cube_interactive.'axes.titlesize' = 12
+#cube_interactive.'legend.fontsize' = 12
+#cube_interactive.'axes.labelsize' = 12
+#cube_interactive.'xtick.labelsize' = 10
+#cube_interactive.'ytick.labelsize' = 10
+
```

### Comparing `lime-stable-0.9.99.5/src/lime/io.py` & `lime-stable-1.0.0/src/lime/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     toml_check = False
 
 _logger = logging.getLogger('LiMe')
 
 # Reading file with the format and export status for the measurements
 _LIME_FOLDER = Path(__file__).parent
 _params_table_file = _LIME_FOLDER/'resources/types_params.txt'
-_PARAMS_CONF_TABLE = pd.read_csv(_params_table_file, delim_whitespace=True, header=0, index_col=0)
+_PARAMS_CONF_TABLE = pd.read_csv(_params_table_file, sep='\s+', header=0, index_col=0)
 
 _LINES_DATABASE_FILE = _LIME_FOLDER/'resources/parent_bands.txt'
 _CONF_FILE = _LIME_FOLDER/'config.toml'
 
 # # Read lime configuration file
 # with open(_CONF_FILE, mode="rb") as fp:
 #     _cfg_lime = tomllib.load(fp)
@@ -174,15 +174,15 @@
 def save_cfg(param_dict, output_file, section_name=None, clear_section=False):
 
     """
     This function safes the input dictionary into a configuration file. If no section is provided the input dictionary
     overwrites the data
 
     """
-    # TODO for line_fitting/model save dictionaries as line
+    # TODO for line_fitting/models save dictionaries as line
     output_path = Path(output_file)
 
     if output_path.suffix == '.toml':
         # TODO review convert numpy arrays and floats64
         if toml_check:
             toml_str = toml.dumps(param_dict)
             with open(output_path, "w") as f:
@@ -248,15 +248,15 @@
             # Save to a text file
             with open(output_file, 'w') as f:
                 output_cfg.write(f)
 
     return
 
 
-def load_frame(fname, page: str = 'LINELOG', levels: list = ['id', 'line']):
+def load_frame(fname, page: str = 'FRAME', levels: list = ['id', 'line']):
 
     """
     This function reads the input ``file_address`` as a pandas dataframe.
 
     The expected file types are ".txt", ".pdf", ".fits", ".asdf" and ".xlsx". The dataframes expected format is discussed
     on the `line bands <https://lime-stable.readthedocs.io/en/latest/inputs/n_inputs3_line_bands.html>`_ and `measurements <https://lime-stable.readthedocs.io/en/latest/inputs/n_inputs4_fit_configuration.html>`_ documentation.
 
@@ -305,44 +305,44 @@
 
                 # # Change 'nan' to np.nan
                 # idcs_nan_str = log['group_label'] == 'none'
                 # log.loc[idcs_nan_str, 'group_label'] = None
 
         # Text file
         elif file_type == '.txt':
-            log = pd.read_csv(log_path, delim_whitespace=True, header=0, index_col=0, comment='#')
+            log = pd.read_csv(log_path, sep='\s+', header=0, index_col=0, comment='#')
 
         elif file_type == '.csv':
-            log = pd.read_csv(log_path, sep=',', delim_whitespace=False, header=0, index_col=0, comment='#')
+            log = pd.read_csv(log_path, sep=',', header=0, index_col=0, comment='#')
 
         else:
             _logger.warning(f'File type {file_type} is not recognized. This can cause issues reading the log.')
-            log = pd.read_csv(log_path, delim_whitespace=True, header=0, index_col=0)
+            log = pd.read_csv(log_path, sep='\s+', header=0, index_col=0)
 
     except ValueError as e:
         exit(f'\nERROR: LiMe could not open {file_type} file at {log_path}\n{e}')
 
     # Restore levels if multi-index
     if log.columns.isin(levels).sum() == len(levels):
         log.set_index(levels, inplace=True)
 
     return log
 
 
-def save_frame(fname, dataframe, page='LINELOG', parameters='all', header=None, column_dtypes=None,
+def save_frame(fname, dataframe, page='FRAME', parameters='all', header=None, column_dtypes=None,
                safe_version=True, **kwargs):
 
     """
 
     This function saves the input ``dataframe`` at the ``fname`` provided by the user.
 
     The accepted extensions are ".txt", ".pdf", ".fits", ".asdf" and ".xlsx".
 
     For ".fits" and ".xlsx" files the user can provide a page name for the HDU/sheet with the ``ext`` argument.
-    The default name is "LINELOG".
+    The default name is "FRAME".
 
     The user can specify the ``parameters`` to be saved in the output file.
 
     For ".fits" files the user can provide a dictionary to add to the ``fits_header``. The user can provide a ``column_dtypes``
     string or dictionary for the output fits file record array. This overwrites LiMe deafult formatting and it must have the
     same columns as the file names.
 
@@ -549,15 +549,15 @@
                     param_value = 'none'
 
             log.at[comp, param] = param_value
 
     return
 
 
-def check_file_dataframe(df_variable, variable_type, ext='LINELOG', sample_levels=['id', 'line'], copy_input=True):
+def check_file_dataframe(df_variable, variable_type, ext='FRAME', sample_levels=['id', 'line'], copy_input=True):
 
     if isinstance(df_variable, variable_type):
         if copy_input:
             output = df_variable.copy()
         else:
             output = df_variable
```

### Comparing `lime-stable-0.9.99.5/src/lime/logo.py` & `lime-stable-1.0.0/src/lime/logo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 from lime.model import gaussian_model
 from matplotlib import pyplot as plt, rcParams
 from matplotlib import font_manager
 from pathlib import Path
-import shutil
 import matplotlib
 
 matplotlib.font_manager._load_fontmanager(try_read_cache=False)
 
 np.random.seed(2)
 
 rcParams['font.family'] = ['MTF Saxy']
@@ -78,12 +77,12 @@
 ax.axis('off')
 ax.axes.xaxis.set_visible(False)
 ax.axes.yaxis.set_visible(False)
 
 plt.tight_layout()
 doc_images_folder = Path('../../docs/source/_static/')
 plt.savefig(doc_images_folder/'logo_dark_transparent.png', bbox_inches='tight', transparent=True)
+# plt.show()
 
 # plt.savefig(doc_images_folder/'logo_transparent.png', bbox_inches='tight', transparent=True)
 # plt.savefig(doc_images_folder/'logo_white.png', bbox_inches='tight')
 # print(f'Saving {doc_images_folder}')
-# plt.show()
```

### Comparing `lime-stable-0.9.99.5/src/lime/model.py` & `lime-stable-1.0.0/src/lime/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,25 +409,25 @@
 
         # Confirm the number of gaussian components
         self.n_comps = len(line.list_comps)
 
         # Decide the line reference wavelength
         self.ref_wave = line.wavelength * (1 + redshift) if line.blended_check else np.atleast_1d(line.peak_wave)
 
-        # Continuum model
+        # Continuum models
         self.model = Model(linear_model)
         self.model.prefix = f'line0_'
 
         # Fix or not the continuum
         m_cont_conf = _SLOPE_FIX_PAR if line._cont_from_adjacent else _SLOPE_FREE_PAR
         n_cont_conf = _INTER_FIX_PAR if line._cont_from_adjacent else _INTER_FREE_PAR
         self.define_param(0, line, 'm_cont', line.m_cont, m_cont_conf, user_conf)
         self.define_param(0, line, 'n_cont', line.n_cont, n_cont_conf, user_conf)
 
-        # Add one gaussian model per component
+        # Add one gaussian models per component
         for idx, comp in enumerate(line.list_comps):
 
             # Gaussian comp
             self.model += Model(PROFILE_FUNCTIONS[line._p_shape[idx]], prefix=f'line{idx}_')
 
             # Amplitude configuration
             if line._p_type[idx]:
@@ -494,28 +494,30 @@
                 self.define_param(idx, line, 'c', 2 * line.pixelWidth, _C_PAR, user_conf)
                 self.define_param(idx, line, 'alpha', -2, _ALPHA_PAR, user_conf)
 
         return
 
     def fit(self, line, x, y, err, method):
 
+        # Unpack the mask for LmFit analysis
+        if np.ma.isMaskedArray(x):
+            idcs_good = ~x.mask
+            x_in = x.data[idcs_good]
+            y_in = y.data[idcs_good]
+        else:
+            x_in, y_in = x, y
+
         # Compute weights
         if err is None:
             weights = np.full(x.size, 1.0 / line.cont_err)
+            weights_in = weights
         else:
             weights = 1.0/err
+            weights_in = weights if not np.ma.isMaskedArray(weights) else weights.data[idcs_good]
 
-        # Unpack the mask for LmFit analysis
-        if np.ma.is_masked(x):
-            idcs_good = ~x.mask
-            x_in = x.data[idcs_good]
-            y_in = y.data[idcs_good]
-            weights_in = weights[idcs_good]
-        else:
-            x_in, y_in, weights_in = x, y, weights
 
         # Fit the line
         self.params = self.model.make_params()
 
         with warnings.catch_warnings():
             warnings.simplefilter(_VERBOSE_WARNINGS)
             self.output = self.model.fit(y_in, self.params, x=x_in, weights=weights_in, method=method, nan_policy='omit')
@@ -558,18 +560,19 @@
                 line.profile_flux = np.full(self.n_comps, np.nan)
                 line.profile_flux_err = np.full(self.n_comps, np.nan)
                 line.eqw = np.full(self.n_comps, np.nan)
                 line.eqw_err = np.full(self.n_comps, np.nan)
                 line.FWHM_p = np.full(self.n_comps, np.nan)
                 line.sigma_thermal = np.full(self.n_comps, np.nan)
 
-            # Check for negative sigmas # TODO this needs a better place
-            if line.sigma[i] < 0:
-                _logger.warning(f'Negative value for profile sigma at {line.label}')
-                line.sigma[i] = np.nan
+            # Check for negative -0.0 # TODO this needs a better place # FIXME -0.0 error
+            if np.signbit(line.sigma_err[i]):
+                line.sigma_err[i] = np.nan
+                if self.output.errorbars:
+                    _logger.warning(f'Negative value for profile sigma at {line.label}')
 
             # Compute the profile areas
             profile_flux_dist = AREA_FUNCTIONS[line._p_shape[i]](line, i, 1000)
             line.profile_flux[i] = np.mean(profile_flux_dist)
             line.profile_flux_err[i] = np.std(profile_flux_dist)
 
             # Compute FWHM_p (Profile Full Width Half Maximum)
@@ -681,22 +684,15 @@
         if '_center' in param_ref:
             if user_ref in user_conf:
                 param_user_conf = user_conf[user_ref]
                 for param_conf_entry in ('value', 'min', 'max'):
                     if param_conf_entry in param_user_conf:
                         param_conf[param_conf_entry] = param_conf[param_conf_entry] * (1 + z_obj)
 
-        # Check the limits on the fitting # TODO some params (blended lines) do not have initial value amp wide
-        param_value = param_conf.get('value')
-        # if param_value is not None:
-        #     if (param_value < param_conf['min']) or (param_value > param_conf['max']):
-        #         _logger.warning(f'Initial value for {param_ref} is outside min-max boundaries: '
-        #                         f'{param_conf["min"]} < {param_value} < {param_conf["max"]}')
-
-        # Assign the parameter configuration to the model
+        # Assign the parameter configuration to the models
         self.model.set_param_hint(param_ref, **param_conf)
 
         return
 
     def review_fitting(self, line):
 
         if not self.output.errorbars:
@@ -736,16 +732,14 @@
 
 class LineFitting:
 
     """Class to measure emission line fluxes and fit them as gaussian curves"""
 
     def __init__(self):
 
-        # self.fit_params = {}
-        # self.fit_output = None
         self.profile = None
 
         return
 
     def integrated_properties(self, line, emis_wave, emis_flux, emis_err, cont_wave, cont_flux, cont_err, emission_check,
                               n_steps=1000):
 
@@ -754,29 +748,35 @@
         line.n_pixels = emis_wave.size
         line.peak_wave = emis_wave[peakIdx]
         line.peak_flux = emis_flux[peakIdx]
         line.pixelWidth = np.diff(emis_wave).mean()
 
         # Get non-nan entries for continuum
         if np.ma.isMaskedArray(cont_flux):
-            input_wave, input_flux = cont_wave.data[~cont_wave.mask], cont_flux.data[~cont_wave.mask]
+            idcs_true = ~cont_flux.mask
+            input_wave, input_flux = cont_wave.data[idcs_true], cont_flux.data[idcs_true]
         else:
             input_wave, input_flux = cont_wave, cont_flux
 
+        # Prepare the continuum error
+        if cont_err is None:
+            input_err = np.ones(input_flux.shape)
+        else:
+            input_err = cont_err.data[idcs_true] if np.ma.isMaskedArray(cont_err) else cont_err
+
         # Check if there are valid entries
         valid_cont_bands = True if input_flux.size > 0 else False
 
         # Gradient and interception of linear continuum using adjacent regions
         if line._cont_from_adjacent and valid_cont_bands:
 
             model_linear = LinearModel()
             params = model_linear.make_params()
 
-            weights = np.ones(input_flux.shape) if cont_err is None else 1/cont_err
-            output = model_linear.fit(input_flux, params, x=input_wave, weights=weights, nan_policy='omit')
+            output = model_linear.fit(input_flux, params, x=input_wave, weights=1/input_err, nan_policy='omit')
 
             m_param, n_param = output.params.get('slope', None), output.params.get('intercept', None)
             line.m_cont = np.nan if m_param is None else m_param.value
             line.n_cont = np.nan if n_param is None else n_param.value
             line.m_cont_err_intg = np.nan if m_param is None else m_param.stderr
             line.n_cont_err_intg = np.nan if n_param is None else n_param.stderr
 
@@ -853,29 +853,29 @@
         return
 
     def profile_fitting(self, line, x, y, err, z_obj, user_conf, fit_method='leastsq', temp=10000.0, inst_FWHM=np.nan):
 
         # Compile the Lmfit component models
         self.profile = ProfileModelCompiler(line, z_obj, user_conf, y)
 
-        # Fit the model
+        # Fit the models
         self.profile.fit(line, x, y, err, fit_method)
 
         # Store the results into the line attributes
         self.profile.measurements_calc(line, user_conf, inst_FWHM, temp)
 
         return
 
     def velocity_profile_calc(self, line, vel_array, line_flux, cont_flux, emission_check, min_array_dim=15):
 
         # In case the vel_array has length zero:
         if vel_array.size > 2:
 
             # Only compute the velocity percentiles for line bands with more than 15 pixels
-            valid_pixels = vel_array.size if not np.ma.is_masked(vel_array) else np.sum(~vel_array.mask)
+            valid_pixels = vel_array.size if not np.ma.isMaskedArray(vel_array) else np.sum(~vel_array.mask)
 
             if valid_pixels > min_array_dim:
 
                 peakIdx = np.argmax(line_flux)
                 percentFluxArray = np.cumsum(line_flux-cont_flux) * line.pixelWidth / line.intg_flux * 100
 
                 if emission_check:
```

### Comparing `lime-stable-0.9.99.5/src/lime/observations.py` & `lime-stable-1.0.0/src/lime/observations.py`

 * *Files 8% similar despite different names*

```diff
@@ -110,20 +110,19 @@
 
 def check_spectrum_axes(lime_object):
 
     # Check for masked arrays
     array_labels = ['wave', 'wave_rest', 'flux']
     check_mask = np.zeros(3).astype(bool)
     for i, arg in enumerate(array_labels):
-        if np.ma.is_masked(lime_object.__getattribute__(arg)):
+        if np.ma.isMaskedArray(lime_object.__getattribute__(arg)):
             check_mask[i] = True
 
     # TODO this one should go at the begining and review inputs
     if np.any(check_mask) and isinstance(lime_object, Spectrum):
-        lime_object._masked_inputs = True
         if ~np.all(check_mask):
             for i, arg in enumerate(array_labels):
                 if not check_mask[i]:
                     _logger.warning(f'Your {arg} array does not include a pixel mask this can caused issues on the fittings')
 
     # Check that the flux and wavelength normalization #
     # if not isinstance(lime_object, Cube):
@@ -329,15 +328,15 @@
         # First the table data
         air_columns = ['wavelength', 'w1', 'w2', 'w3', 'w4', 'w5', 'w6']
         mask_df[air_columns] = mask_df[air_columns].apply(air_to_vacuum_function, raw=True)
 
     # Convert to requested units
     units_wave = au.Unit(units_wave)
     if units_wave != 'Angstrom':
-        conversion_factor = unit_conversion('Angstrom', units_wave, wave_array=1, dispersion_units='dispersion axis')
+        conversion_factor = unit_conversion(au.Unit('Angstrom'), units_wave, wave_array=1, dispersion_units='dispersion axis')
         mask_df.loc[:, 'wavelength':'w6'] = mask_df.loc[:, 'wavelength':'w6'] * conversion_factor
 
     # Reconstruct the latex label
     n_bands = mask_df.index.size
     mask_df['latex_label'] = latex_from_label(None, mask_df['particle'], mask_df['wavelength'],
                                               np.array([units_wave] * n_bands), np.zeros(n_bands),
                                               mask_df['transition'], decimals=decimals)
@@ -449,36 +448,35 @@
 
     """
 
     # File manager for a Cube created from an observation file
     _fitsMgr = None
 
     def __init__(self, input_wave=None, input_flux=None, input_err=None, redshift=None, norm_flux=None, crop_waves=None,
-                 inst_FWHM=np.nan, units_wave='AA', units_flux='FLAM', pixel_mask=None, id_label=None, review_inputs=True):
+                 inst_FWHM=None, units_wave='AA', units_flux='FLAM', pixel_mask=None, id_label=None, review_inputs=True):
 
         # Load parent classes
         LineFinder.__init__(self)
 
         # Class attributes
         self.label = None
         self.wave = None
         self.wave_rest = None
         self.flux = None
         self.err_flux = None
         self.cont = None
         self.cont_std = None
 
-        self.log = None
+        self.frame = None
 
         self.redshift = None
         self.norm_flux = None
         self.inst_FWHM = None
         self.units_wave = None
         self.units_flux = None
-        self._masked_inputs = False # TODO quitar este
 
         # Treatments objects
         self.fit = SpecTreatment(self)
         self.infer = DetectionInference(self)
 
         # Plotting objects
         self.plot = SpectrumFigures(self)
@@ -501,23 +499,21 @@
         spec.label = label
         spec.wave = cube.wave
         spec.wave_rest = cube.wave_rest
         spec.flux = cube.flux[:, idx_j, idx_i]
         spec.err_flux = None if cube.err_flux is None else cube.err_flux[:, idx_j, idx_i]
         spec.norm_flux = cube.norm_flux
         spec.redshift = cube.redshift
-        spec.log = pd.DataFrame(np.empty(0, dtype=_LOG_EXPORT_RECARR))
+        spec.frame = pd.DataFrame(np.empty(0, dtype=_LOG_EXPORT_RECARR))
         spec.inst_FWHM = cube.inst_FWHM
         spec.units_wave = cube.units_wave
         spec.units_flux = cube.units_flux
 
         # Check if masked array
-        spec._masked_inputs = False
         if np.ma.isMaskedArray(spec.flux):
-            spec._masked_inputs = True
             spec.wave = np.ma.masked_array(spec.wave, cube.flux[:, idx_j, idx_i].mask)
             spec.wave_rest = np.ma.masked_array(cube.wave_rest, cube.flux[:, idx_j, idx_i].mask)
 
         return spec
 
     @classmethod
     def from_file(cls, file_address, instrument, mask_flux_entries=None, **kwargs):
@@ -605,15 +601,15 @@
         return cls(**fits_args)
 
     def _set_attributes(self, input_wave, input_flux, input_err, redshift, norm_flux, crop_waves, inst_FWHM, units_wave,
                         units_flux, pixel_mask, label):
 
         # Class attributes
         self.label = label
-        self.inst_FWHM = inst_FWHM
+        self.inst_FWHM = np.nan if inst_FWHM is None else inst_FWHM
 
         # Review the inputs
         check_inputs_arrays(input_wave, input_flux, input_err, self)
 
         # Checks units
         self.units_wave, self.units_flux = check_units(units_wave, units_flux)
 
@@ -629,15 +625,15 @@
                                                                                          input_err, pixel_mask,
                                                                                          self.redshift, self.norm_flux)
 
         # Check nan entries and mask quality
         check_spectrum_axes(self)
 
         # Generate empty dataframe to store measurement use cwd as default storing folder # TODO we are not using this
-        self.log = pd.DataFrame(np.empty(0, dtype=_LOG_EXPORT_RECARR))
+        self.frame = pd.DataFrame(np.empty(0, dtype=_LOG_EXPORT_RECARR))
 
         return
 
     def unit_conversion(self, wave_units_out=None, flux_units_out=None, norm_flux=None):
 
         """
 
@@ -717,26 +713,26 @@
             # Re-apply mask
             self.flux = flux_arr if input_mask is None else np.ma.masked_array(flux_arr, self.flux.mask)
             self.err_flux = err_arr if input_mask is None else np.ma.masked_array(err_arr, self.err_flux.mask)
             self.norm_flux = norm_flux
 
         return
 
-    def save_frame(self, fname, page='LINELOG', param_list='all', header=None, column_dtypes=None,
+    def save_frame(self, fname, page='FRAME', param_list='all', header=None, column_dtypes=None,
                    safe_version=True):
 
 
         """
 
         This function saves the spectrum measurements at the ``file_address`` provided by the user.
 
         The accepted extensions  are ".txt", ".pdf", ".fits", ".asdf" and ".xlsx".
 
         For ".fits" and ".xlsx" files the user can provide a page name for the HDU/sheet with the ``ext`` argument.
-        The default name is "LINELOG".
+        The default name is "LINESFRAME".
 
         The user can specify the ``parameters`` to be saved in the output file.
 
         For ".fits" files the user can provide a dictionary to add to the ``fits_header``. The user can provide a ``column_dtypes``
         string or dictionary for the output fits file record array. This overwrites LiMe deafult formatting and it must have the
         same columns as the file names.
 
@@ -767,20 +763,20 @@
         meta_params = {'LiMe':       __version__,
                        'u_wave':     self.units_wave.to_string(),
                        'u_flux':     self.units_flux.to_string(),
                        'redshift':   self.redshift,
                        'id':         self.label}
 
         # Save the file
-        save_frame(fname, self.log, page, param_list, header, column_dtypes=column_dtypes,
+        save_frame(fname, self.frame, page, param_list, header, column_dtypes=column_dtypes,
                    safe_version=safe_version, **meta_params)
 
         return
 
-    def load_frame(self, fname, page='LINELOG'):
+    def load_frame(self, fname, page='LINESFRAME'):
 
         """
 
         This function loads a lines measurements log as a lime.Spectrum.log variable.
 
         The appropriate variables are normalized by the current spectrum flux normalization.
 
@@ -810,25 +806,25 @@
             # Confirm all the log lines have the same units
             au_str = 'A' if line_0.units_wave[0] == 'Angstrom' else str(line_0.units_wave)
             same_units_check = np.flatnonzero(np.core.defchararray.find(line_list.astype(str), au_str) != -1).size == line_list.size
             if not same_units_check:
                 _logger.warning(f'The log has lines with different units')
 
             # Assign the log
-            self.log = log_df
+            self.frame = log_df
 
         else:
             _logger.info(f'Log file with 0 entries ({fname})')
 
         return
 
     def update_redshift(self, redshift):
 
         # Check if it is a masked array
-        if np.ma.is_masked(self.wave):
+        if np.ma.isMaskedArray(self.wave):
             input_wave = self.wave.data
             input_flux = self.flux.data
             input_err = self.err_flux.data
             pixel_mask = self.wave.mask
         else:
             input_wave = self.wave
             input_flux = self.flux
@@ -906,28 +902,27 @@
 
     """
 
     # File manager for a Cube created from an observation file
     _fitsMgr = None
 
     def __init__(self, input_wave=None, input_flux=None, input_err=None, redshift=None, norm_flux=None, crop_waves=None,
-                 inst_FWHM=np.nan, units_wave='AA', units_flux='FLAM', pixel_mask=None, id_label=None, wcs=None):
+                 inst_FWHM=None, units_wave='AA', units_flux='FLAM', pixel_mask=None, id_label=None, wcs=None):
 
         # Review the inputs
         check_inputs_arrays(input_wave, input_flux, input_err, self)
 
         # Class attributes
         self.obj_name = id_label
         self.wave = None
         self.wave_rest = None
         self.flux = None
         self.err_flux = None
         self.log = None
-        self.inst_FWHM = inst_FWHM
-        self._masked_inputs = False
+        self.inst_FWHM = np.nan if inst_FWHM is None else inst_FWHM
         self.wcs = wcs
 
         # Treatments objects
         self.fit = CubeTreatment(self)
 
         # Plotting objects
         self.plot = CubeFigures(self)
@@ -961,15 +956,15 @@
         This method creates a lime.Cube object from an observational (.fits) file.  The user needs to introduce the
         file address location and the name of the instrument of survey.
 
         Currently, this method supports MANGA and MUSE input instrument sources. This method will lower case the input
         instrument or survey name.
 
         The user can include list of pixel values to generate a mask from the input file flux entries. For example, if the
-        user introduces [np.nan, 'negative'] the output spectrum will mask np.nan entries and negative fluxes.
+        user introduces ["nan", "negative"] the output spectrum will mask np.nan entries and negative fluxes.
 
         This method procures the instrument observations units, normalization and wcs but the user should introduce the
         LiMe.Spectrum arguments (such as the observation redshift).
 
         :param file_address: Input file location address.
         :type file_address: Path, string
 
@@ -1055,16 +1050,18 @@
         if not param in ['flux', 'SN_line', 'SN_cont']:
             raise Error(f'The mask calculation parameter ({param}) is not recognised. Please use "flux", "SN_line", "SN_cont"')
 
         # Line for the background image
         line_bg = Line(line, bands)
 
         # Get the band indexes
-        idcsEmis, idcsCont = define_masks(self.wave, line_bg.mask * (1 + self.redshift), line_bg.pixel_mask)
+        idcsEmis, idcsCont = define_masks(self.wave, line_bg.mask * (1 + self.redshift), line_mask_entry=line_bg.pixel_mask,
+                                          line=line_bg.label)
         signal_slice = self.flux[idcsEmis, :, :]
+        signal_slice = signal_slice if not np.ma.isMaskedArray(signal_slice) else signal_slice.data
 
         # Get indeces all nan entries to exclude them from the analysis
         idcs_all_nan = np.all(np.isnan(signal_slice.data), axis=0)
 
         # If not mask parameter provided we use the flux percentiles
         if param == 'flux':
             param = self.units_flux
@@ -1074,14 +1071,16 @@
         elif param == 'SN_cont':
             param_image = np.nanmean(signal_slice, axis=0) / np.nanstd(signal_slice, axis=0)
 
         # S/N line
         elif param == 'SN_line':
             n_pixels = np.sum(idcsCont)
             cont_slice = self.flux[idcsCont, :, :]
+            cont_slice = cont_slice if not np.ma.isMaskedArray(cont_slice) else cont_slice.data
+
             Amp_image = np.nanmax(signal_slice, axis=0) - np.nanmean(cont_slice, axis=0)
             std_image = np.nanstd(cont_slice, axis=0)
             param_image = (np.sqrt(2 * n_pixels * np.pi) / 6) * (Amp_image / std_image)
 
         else:
             raise LiMe_Error(f'Parameter {param} is not recognized please use: "flux", "SN_line" or "SN_cont"')
 
@@ -1122,14 +1121,16 @@
         # Recover coordinates from the wcs to store in the headers:
         hdr_coords = extract_wcs_header(self.wcs, drop_axis='spectral')
 
         for idx_region, region_items in enumerate(mask_dict.items()):
             region_label, region_mask = region_items
 
             # Metadata for the fits page
+            signal_slice = signal_slice if not np.ma.isMaskedArray(signal_slice) else signal_slice.data
+
             hdr_i = fits.Header({'PARAM': param,
                                  'PARAMIDX': boundary_dict[region_label],
                                  'PARAMVAL': param_level[region_label],
                                  'NUMSPAXE': np.sum(region_mask)})
 
             # Add WCS information
             if hdr_coords is not None:
@@ -1188,34 +1189,34 @@
 
         """
 
         # Dispersion axes conversion
         if units_wave is not None:
 
             # Remove the masks for the conversion
-            input_wave = self.wave.data if np.ma.is_masked(self.wave) else self.wave
+            input_wave = self.wave.data if np.ma.isMaskedArray(self.wave) else self.wave
 
             output_wave = unit_conversion(self.units_wave, units_wave, wave_array=input_wave)
 
             # Reflect the new units
-            if np.ma.is_masked(self.wave):
+            if np.ma.isMaskedArray(self.wave):
                 self.wave = np.ma.masked_array(output_wave, self.wave.mask)
                 self.wave_rest = np.ma.masked_array(output_wave/(1+self.redshift), self.wave.mask)
             else:
                 self.wave = output_wave
                 self.wave_rest = output_wave/(1+self.redshift)
             self.units_wave = units_wave
 
         # Flux axis conversion
         if units_flux is not None:
 
             # Remove the masks for the conversion
-            input_wave = self.wave.data if np.ma.is_masked(self.wave) else self.wave
-            input_flux = self.flux.data if np.ma.is_masked(self.flux) else self.flux
-            input_err = self.err_flux.data if np.ma.is_masked(self.err_flux) else self.err_flux
+            input_wave = self.wave.data if np.ma.isMaskedArray(self.wave) else self.wave
+            input_flux = self.flux.data if np.ma.isMaskedArray(self.flux) else self.flux
+            input_err = self.err_flux.data if np.ma.isMaskedArray(self.err_flux) else self.err_flux
 
             # TODO this is slow
             flux_shape = input_flux.shape
             y_range, x_range = np.arange(flux_shape[1]), np.arange(flux_shape[2])
             if len(flux_shape) == 3:
                 output_flux = np.empty(flux_shape)
                 for j in y_range:
@@ -1227,26 +1228,26 @@
                                               flux_array=input_flux, dispersion_units=self.units_wave)
 
             if input_err is not None:
                 output_err = unit_conversion(self.units_flux, units_flux, wave_array=input_wave,
                                              flux_array=input_err, dispersion_units=self.units_wave)
 
             # Reflect the new units
-            if np.ma.is_masked(self.flux):
+            if np.ma.isMaskedArray(self.flux):
                 self.flux = np.ma.masked_array(output_flux, self.flux.mask)
             else:
                 self.flux = output_flux
             if input_err is not None:
-                self.err_flux = np.ma.masked_array(output_err, self.err_flux.mask) if np.ma.is_masked(self.err_flux) else output_err
+                self.err_flux = np.ma.masked_array(output_err, self.err_flux.mask) if np.ma.isMaskedArray(self.err_flux) else output_err
             self.units_flux = units_flux
 
         # Switch the normalization
         if norm_flux is not None:
-            # TODO isMaskedArray checks individually?
-            mask_check = np.ma.is_masked(self.flux)
+
+            mask_check = np.ma.isMaskedArray(self.flux)
 
             # Remove old
             if mask_check:
                 new_flux = self.flux.data * self.norm_flux / norm_flux
                 new_err = None if self.err_flux is None else self.err_flux.data * self.norm_flux / norm_flux
 
                 self.flux = np.ma.masked_array(new_flux, self.flux.mask)
@@ -1430,24 +1431,24 @@
 
         # Check the levels on combined labels target log
         check_sample_levels(self.levels)
 
         # Checks units
         self.units_wave, self.units_flux = check_units(units_wave, units_flux)
 
-        self.log = check_file_dataframe(sample_log, pd.DataFrame, sample_levels=self.levels)
+        self.frame = check_file_dataframe(sample_log, pd.DataFrame, sample_levels=self.levels)
         self._load_function = load_function
         self.load_params = kwargs
 
         # Functionality objects
         self.plot = SampleFigures(self)
         self.check = SampleCheck(self)
 
         # Check if there is not a log
-        if self.log is None:
+        if self.frame is None:
             _logger.warning(f'Sample was created with a null log')
 
         return
 
     @classmethod
     def from_file(cls, id_list, log_list=None, file_list=None, page_list=None, levels=('id', 'file', "line"),
                   load_function=None, instrument=None, folder_obs=None, **kwargs):
@@ -1517,15 +1518,15 @@
 
         # Loop through observations and combine the log
         df_list = []
         for i, id_spec in enumerate(id_list):
 
             # Page and spec index
             file_spec = None if file_list is None else file_list[i]
-            page_name = page_list[i] if page_list is not None else 'LINELOG'
+            page_name = page_list[i] if page_list is not None else 'LINESFRAME'
 
             # Load the log and check the levels
             if log_list is not None:
                 log_i = load_frame(log_list[i], page_name, levels)
                 df_list.append(review_sample_levels(log_i, id_spec, file_spec))
             else:
                 log_i = pd.DataFrame(columns=["id", "file"], data=(id_spec, file_spec))
@@ -1574,100 +1575,100 @@
         # Proceed to selection
         if valid_check:
 
             # Check if Pandas indeces, numpy boolean or scalar key
             if isinstance(id_key, pd.Index) or isinstance(id_key, pd.MultiIndex) or isinstance(id_key, pd.Series):
                 idcs = id_key
             elif isinstance(id_key, (np.ndarray, np.bool_)):
-                idcs = self.log.index[id_key]
+                idcs = self.frame.index[id_key]
             else:
-                idcs = self.log.index.get_level_values('id').isin([id_key])
+                idcs = self.frame.index.get_level_values('id').isin([id_key])
 
             # Not entry found
             if np.all(idcs is False):
                 raise KeyError(id_key)
 
             # Crop sample
-            output = Sample(self.log.loc[idcs], self.levels, self.load_function, self.source, self.file_address,
+            output = Sample(self.frame.loc[idcs], self.levels, self.load_function, self.source, self.file_address,
                             **self.load_params)
 
         return output
 
     def get_observation(self, input_index, default_none=False):
 
         output = None
         valid_check = self._review_df_indexes()
 
         if valid_check:
 
             # Case only ID string
             if isinstance(input_index, str):
-                idcs = self.log.index.get_level_values('id').isin(np.atleast_1d(input_index))
+                idcs = self.frame.index.get_level_values('id').isin(np.atleast_1d(input_index))
 
                 # Not entry found
                 if np.all(idcs is False):
                     raise KeyError(input_index)
 
                 # Check for logs without lines
-                if 'line' not in self.log.index.names:
-                    obj_idcs = self.log.loc[idcs].index.unique()
+                if 'line' not in self.frame.index.names:
+                    obj_idcs = self.frame.loc[idcs].index.unique()
                 else:
-                    obj_idcs = self.log.loc[idcs].iloc[0].name
+                    obj_idcs = self.frame.loc[idcs].iloc[0].name
             else:
                 obj_idcs = input_index
 
             # # Not entry found
             # if len(obj_idcs) > 1:
             #     raise LiMe_Error(f'Multiple observations match the input id: {obj_idcs}')
 
             # Load the LiMe object
-            output = self.load_function(self.log, obj_idcs, self.file_address, **self.load_params)
+            output = self.load_function(self.frame, obj_idcs, self.file_address, **self.load_params)
 
         return output
 
     def get_spectrum(self, idx):
 
         if isinstance(idx, pd.Series):
-            idx_true = self.log.loc[idx].index
+            idx_true = self.frame.loc[idx].index
 
             if idx_true.size > 1:
                 raise LiMe_Error(f'Input sample spectrum extraction has more than one existing entry')
 
-            idx_in = self.log.loc[idx_true].index.values[0]
+            idx_in = self.frame.loc[idx_true].index.values[0]
 
         else:
             idx_in = idx
 
-        return self.load_function(self.log, idx_in, self.file_address, **self.load_params)
+        return self.load_function(self.frame, idx_in, self.file_address, **self.load_params)
 
     @property
     def index(self):
-        return self.log.index
+        return self.frame.index
 
     @property
     def loc(self):
-        return self.log.loc
+        return self.frame.loc
 
     @property
     def ids(self):
-        return self.log.index.get_level_values('id')
+        return self.frame.index.get_level_values('id')
 
     @property
     def files(self):
-        return self.log.index.get_level_values('file')
+        return self.frame.index.get_level_values('file')
 
     @property
     def lines(self):
-        return self.log.index.get_level_values('line')
+        return self.frame.index.get_level_values('line')
 
     @property
     def size(self):
-        return self.log.index.size
+        return self.frame.index.size
 
-    def load_frame(self, dataframe, ext='LINELOG', sample_levels=['id', 'line']):
+    def load_frame(self, dataframe, ext='LINESFRAME', sample_levels=['id', 'line']):
 
         # Load the log file if it is a log file
         log_df = check_file_dataframe(dataframe, pd.DataFrame, ext=ext, sample_levels=sample_levels)
 
         # Security checks:
         if log_df.index.size > 0:
 
@@ -1688,52 +1689,52 @@
                 if not same_units_check:
                     _logger.warning(f'The log has lines with different units')
 
         else:
             _logger.info(f'Log file with 0 entries ({dataframe})')
 
         # Assign the log
-        self.log = log_df
+        self.frame = log_df
 
         return
 
-    def save_frame(self, fname, ext='LINELOG', param_list='all', fits_header=None):
+    def save_frame(self, fname, ext='LINESFRAME', param_list='all', fits_header=None):
 
         # Save the file
-        save_frame(fname, self.log, ext, param_list, fits_header)
+        save_frame(fname, self.frame, ext, param_list, fits_header)
 
         return
 
     def extract_fluxes(self, flux_type='mixture', sample_level='line', column_names='line_flux', column_positions=1):
 
-        return extract_fluxes(self.log, flux_type, sample_level, column_names, column_positions)
+        return extract_fluxes(self.frame, flux_type, sample_level, column_names, column_positions)
 
     def normalize_fluxes(self, normalization_line, flux_entries=['line_flux', 'line_flux_err'], column_names=None,
                          column_positions=[1, 2]):
 
-        return normalize_fluxes(self.log, normalization_line, flux_entries, column_names, column_positions)
+        return normalize_fluxes(self.frame, normalization_line, flux_entries, column_names, column_positions)
 
     def _review_df_indexes(self):
 
         # Check there is a log
         check = False
 
-        if self.log is None:
+        if self.frame is None:
             _logger.info(f'Sample does not contain observations')
 
         # Check there is load function
         elif self.load_function is None:
             _logger.info(f'The sample does not contain a load_function')
 
         # Check there is a 'file' index
-        elif 'id' not in self.log.index.names:
+        elif 'id' not in self.frame.index.names:
             _logger.info(f'The sample log does not contain an "id" index column the observation label')
 
         # Check there is a 'file' index
-        elif 'file' not in self.log.index.names:
+        elif 'file' not in self.frame.index.names:
             _logger.info(f'The sample log does not contain a "file" index column with the observation file')
 
         else:
             check = True
 
         return check
```

### Comparing `lime-stable-0.9.99.5/src/lime/plots.py` & `lime-stable-1.0.0/src/lime/plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         # Assign default
         self.conf = conf.copy()
         self.library = library
         self.set_style(style)
 
         return
 
-    def fig_defaults(self, user_fig, fig_type=None):
+    def fig_defaults(self, user_fig=None, fig_type=None):
 
         # Get plot configuration
         if fig_type is None:
             fig_conf = self.base_conf.copy()
         else:
             fig_conf = {** self.base_conf, **self.conf[self.library][fig_type]}
 
@@ -130,88 +130,49 @@
             ax_cfg = {}
 
             # Update with the user configuration
             ax_cfg = ax_cfg if user_ax is None else {**ax_cfg, **user_ax}
 
         return ax_cfg
 
-    def set_style(self, style, style_conf=None, colors_conf=None):
+    def set_style(self, style=None, fig_cfg=None, colors_conf=None):
 
         # Set the new style
-        self.style = np.atleast_1d(style)
-
-        # Add the new configuration
-        if style_conf is not None:
-            existing_set = {} if self.style not in self.conf[self.library] else self.conf[self.library][self.style]
-            self.conf[self.library][self.style] = {**existing_set, **style_conf}
+        if style is not None:
+            self.style = np.atleast_1d(style)
+        else:
+            self.style = np.atleast_1d('default')
 
         # Generate the default
         self.base_conf = self.conf[self.library]['default'].copy()
         for style in self.style:
             self.base_conf = {**self.base_conf, **self.conf[self.library][style]}
 
-        # Add the new colors
-        if colors_conf is not None:
-            existing_set = {} if self.style not in self.conf['lime_colors'] else self.conf['lime_colors'][self.style]
-            self.conf['lime_colors'][self.style] = {**existing_set, **colors_conf}
+        # Add the new configuration
+        if fig_cfg is not None:
+            self.base_conf = {**self.base_conf, **fig_cfg}
 
         # Set the colors
         for i_style in self.style:
-            if i_style in self.conf['lime_colors']:
-                self.colors = self.conf['lime_colors'][style].copy()
+            if i_style in self.conf['colors']:
+                self.colors = self.conf['colors'][style].copy()
+
+        # Add the new colors
+        if colors_conf is not None:
+            self.colors = {**self.colors, **colors_conf}
 
         if self.colors is None:
             _logger.warning(f'The input style {self.style} does not have a LiMe color database')
 
         return
 
 
 # LiMe figure labels and color formatter
 theme = Themer(_setup_cfg)
 
-# PLOT_SIZE_FONT = {'figure.figsize': (11, 6),
-#                   'axes.titlesize': 14,
-#                   'axes.labelsize': 14,
-#                   'legend.fontsize': 12,
-#                   'xtick.labelsize': 12,
-#                   'ytick.labelsize': 12}
-#
-# COLOR_DICT = {'bg': 'white', 'fg': 'black',
-#              'cont_band': '#8c564b', 'line_band': '#b5bd61',
-#              'color_cycle': ['#279e68', '#d62728', '#aa40fc', '#8c564b',
-#                              '#e377c2', '#7f7f7f', '#b5bd61', '#17becf', '#1f77b4', '#ff7f0e'],
-#              'matched_line': '#b5bd61',
-#              'peak': '#aa40fc',
-#              'trough': '#7f7f7f',
-#              'profile': '#1f77b4',
-#              'cont': '#ff7f0e',
-#              'error': 'red',
-#              'mask_map': 'viridis',
-#              'comps_map': 'Dark2',
-#              'mask_marker': 'red'}
-#
-# PLOT_COLORS = {'figure.facecolor': COLOR_DICT['bg'], 'axes.facecolor': COLOR_DICT['bg'],
-#                'axes.edgecolor': COLOR_DICT['fg'], 'axes.labelcolor': COLOR_DICT['fg'],
-#                'xtick.color': COLOR_DICT['fg'], 'ytick.color': COLOR_DICT['fg'],
-#                'text.color': COLOR_DICT['fg'], 'legend.edgecolor': 'inherit', 'legend.facecolor': 'inherit'}
-#
-# colorDictDark = {'bg': np.array((43, 43, 43))/255.0, 'fg': np.array((179, 199, 216))/255.0,
-#                  'red': np.array((43, 43, 43))/255.0, 'yellow': np.array((191, 144, 0))/255.0}
-#
-# PLOT_COLORS_DARK = {'figure.facecolor': colorDictDark['bg'], 'axes.facecolor': colorDictDark['bg'],
-#                     'axes.edgecolor': colorDictDark['fg'], 'axes.labelcolor': colorDictDark['fg'],
-#                     'xtick.color': colorDictDark['fg'],  'ytick.color': colorDictDark['fg'],
-#                     'text.color': colorDictDark['fg'], 'legend.edgecolor': 'inherit', 'legend.facecolor': 'inherit'}
-#
-# PLOT_COLORS = {}
-#
-# STANDARD_PLOT = {**PLOT_SIZE_FONT, **PLOT_COLORS}
-#
-# STANDARD_AXES = {'xlabel': r'Wavelength $(\AA)$', 'ylabel': r'Flux $(erg\,cm^{-2} s^{-1} \AA^{-1})$'}
-
 
 def mplcursors_legend(line, log, latex_label, norm_flux, units_wave, units_flux):
 
     legend_text = latex_label + '\n'
 
     units_line_flux = units_wave * units_flux
     line_flux_latex = f'{units_line_flux:latex}'
@@ -264,21 +225,21 @@
     # Return the figure for output plotting
     else:
         output_fig = fig_obj
 
     return output_fig
 
 
-def frame_mask_switch_2(wave_obs, flux_obs, redshift, rest_frame):
+def frame_mask_switch(wave_obs, flux_obs, redshift, rest_frame):
 
     # Doppler factor for rest _frame plots
     z_corr = (1 + redshift) if rest_frame else 1
 
     # Remove mask from plots and recover bad indexes
-    if np.ma.is_masked(wave_obs):
+    if np.ma.isMaskedArray(wave_obs):
         idcs_mask = wave_obs.mask
         wave_plot, flux_plot = wave_obs.data, flux_obs.data
 
     else:
         idcs_mask = np.zeros(wave_obs.size).astype(bool)
         wave_plot, flux_plot = wave_obs, flux_obs
 
@@ -351,17 +312,17 @@
 
 
 def check_line_for_bandplot(in_label, user_band, spec, log_ref=_PARENT_BANDS):
 
     # If no line provided, use the one from the last fitting
     label = None
     if in_label is None:
-        if spec.log.index.size > 0:
-            label = spec.log.iloc[-1].name
-            band = spec.log.loc[label, 'w1':'w6'].values
+        if spec.frame.index.size > 0:
+            label = spec.frame.iloc[-1].name
+            band = spec.frame.loc[label, 'w1':'w6'].values
         else:
             band = None
             _logger.info(f'The lines log is empty')
 
     # The user provides a line and a band
     elif (in_label is not None) and (user_band is not None):
         band = user_band
@@ -371,35 +332,35 @@
 
         # The line has not been measured before (just plot the region) # TODO I do not like this one
         if isinstance(in_label, str):
             if in_label.endswith('_b'):
                 in_label = in_label[:-2]
 
         # Case of a float entry
-        if in_label not in spec.log.index:
+        if in_label not in spec.frame.index:
 
             # First we try the user spec log
-            if spec.log.index.size > 0:
-                test_label = check_line_in_log(in_label, spec.log)
+            if spec.frame.index.size > 0:
+                test_label = check_line_in_log(in_label, spec.frame)
                 if test_label != in_label:
                     label = test_label
-                    band = spec.log.loc[label, 'w1':'w6'].values
+                    band = spec.frame.loc[label, 'w1':'w6'].values
 
             # We use the reference log
             if label is None:
                 label = check_line_in_log(in_label, log_ref)
                 if label in log_ref.index:
                     band = log_ref.loc[label, 'w1':'w6'].values
                 else:
                     band = None
 
         # The line has been plotted before
         else:
             label = in_label
-            band = spec.log.loc[in_label, 'w1':'w6'].values
+            band = spec.frame.loc[in_label, 'w1':'w6'].values
 
     return label, band
 
 
 def check_image_size(bg_image, fg_image, mask_dict):
 
     # Confirm that the background and foreground images have the same size
@@ -423,15 +384,16 @@
     # Generate line object
     if line is not None:
 
         # Determine the line of reference
         line = Line(line, band)
 
         # Compute the band map slice
-        idcsEmis, idcsCont = define_masks(cube.wave, line.mask * (1 + cube.redshift), line.pixel_mask)
+        idcsEmis, idcsCont = define_masks(cube.wave, line.mask * (1 + cube.redshift), line_mask_entry=line.pixel_mask,
+                                          line=line.label)
         image = cube.flux[idcsEmis, :, :].sum(axis=0)
 
         # If no scale provided compute a default one
         if color_scale is None:
 
             levels = np.nanpercentile(image, np.array(percentiles, ndmin=1))
 
@@ -452,15 +414,16 @@
 def image_plot(ax, image_bg, image_fg, fg_levels, fg_mesh, bg_scale, fg_scale, bg_color, fg_color, cursor_cords=None):
 
     # Background image plot
     im = ax.imshow(image_bg, cmap=bg_color, norm=bg_scale)
 
     # Foreground contours
     if image_fg is not None:
-        contours = ax.contour(fg_mesh[0], fg_mesh[1], image_fg, cmap=fg_color, levels=fg_levels, norm=fg_scale)
+        contours = ax.contour(fg_mesh[0], fg_mesh[1], image_fg, cmap=fg_color, levels=fg_levels, norm=fg_scale,
+                              linewidth=0.2)
     else:
         contours = None
 
     # Marker
     if cursor_cords is not None:
         marker, = ax.plot(cursor_cords[1], cursor_cords[0], '+', color='red')
     else:
@@ -511,22 +474,22 @@
 
             ax.imshow(inv_mask_array, cmap=cm_i, vmin=0, vmax=1, alpha=mask_alpha)
 
     return legend_list
 
 
 def spec_plot(ax, wave, flux, redshift, norm_flux, label='', rest_frame=False, log=None, include_fits=True,
-              units_wave='A', units_flux='Flam', log_scale=False, color_dict=theme.colors):
-
+              units_wave='A', units_flux='Flam', log_scale=False):
 
     # Reference frame for the plot
-    wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, redshift, rest_frame)
+    wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(wave, flux, redshift, rest_frame)
 
     # Plot the spectrum
-    ax.step(wave_plot / z_corr, flux_plot * z_corr, label=label, where='mid', color=color_dict['fg'])
+    ax.step(wave_plot / z_corr, flux_plot * z_corr, label=label, where='mid', color=theme.colors['fg'],
+            linewidth=theme.colors['spectrum_width'])
 
     # List of lines in the log
     line_list = []
     if log is not None:
         if log.index.size > 0 and include_fits:
             line_list = log.index.values
 
@@ -542,69 +505,55 @@
 
     # Plot the masked pixels
     _masks_plot(ax, line_list, wave_plot, flux_plot, z_corr, log, idcs_mask)
 
     return
 
 
-def _profile_plot(axis, x, y, label, idx_line=0, n_comps=1, observations_list='yes', color_dict=theme.colors):
+def _profile_plot(axis, x, y, label, idx_line=0, n_comps=1, observations_list='yes'):
 
     # Color and thickness
     if observations_list == 'no':
 
         # If only one component or combined
         if n_comps == 1:
-            width_i, style, color = 1.5, '-', color_dict['profile']
+            width_i, style, color = theme.colors['single_width'], '-', theme.colors['profile']
 
         # Component
         else:
-            cmap = cm.get_cmap(color_dict['comps_map'])
-
-            """  /home/usuario/PycharmProjects/lime/src/lime/plots.py:725: MatplotlibDeprecationWarning: 
-            The get_cmap function was deprecated in Matplotlib 3.7 and will be removed two minor releases later. 
-            Use ``matplotlib.colormaps[name]`` or ``matplotlib.colormaps.get_cmap(obj)`` instead.
-                cmap = cm.get_cmap(color_dict['comps_map'])
-            """
-
-            width_i, style, color = 2, ':', cmap(idx_line/n_comps)
+            cmap = cm.get_cmap(theme.colors['comps_map'])
+            width_i, style, color = theme.colors['comp_width'], ':', cmap(idx_line/n_comps)
 
     # Case where the line has an error
     else:
-        width_i, style, color = 3, '-', 'red'
+        width_i, style, color = theme.colors['err_width'], '-', theme.colors['error']
 
     # Plot the profile
     line_g = axis.plot(x, y, label=label, linewidth=width_i, linestyle=style, color=color)
 
     return line_g
 
 
 def color_selector(label, observations, idx_line, n_comps):
 
     # Color and thickness
     if observations == 'no':
 
         # If only one component or combined
         if n_comps == 1:
-            width_i, style, color = 1.5, '-', theme.colors['profile']
+            width_i, style, color = theme.colors['single_width'], '-', theme.colors['profile']
 
         # Component
         else:
             cmap = cm.get_cmap(theme.colors['comps_map'])
-
-            """  /home/usuario/PycharmProjects/lime/src/lime/plots.py:725: MatplotlibDeprecationWarning: 
-            The get_cmap function was deprecated in Matplotlib 3.7 and will be removed two minor releases later. 
-            Use ``matplotlib.colormaps[name]`` or ``matplotlib.colormaps.get_cmap(obj)`` instead.
-                cmap = cm.get_cmap(color_dict['comps_map'])
-            """
-
-            width_i, style, color = 2, ':', cmap(idx_line/n_comps)
+            width_i, style, color = theme.colors['comp_width'], ':', cmap(idx_line/n_comps)
 
     # Case where the line has an error
     else:
-        width_i, style, color = 3, '-', 'red'
+        width_i, style, color = theme.colors['err_width'], '-', 'red'
 
     # Make dictionary with the params
     cont_format = dict(label=label, color=color, linestyle=style, linewidth=width_i)
 
     return cont_format
 
 
@@ -685,20 +634,19 @@
             axis.plot(wave_i / z_corr, cont_i * z_corr / norm_flux, color=theme.colors['cont'], label=None,
                       linestyle='--', linewidth=0.5)
 
         # Plot combined gaussian profile if blended
         if idcs_comp is not None:
             gauss_comb = gaussian_array[:, idcs_comp].sum(axis=1) + cont_i
             _profile_plot(axis, wave_i/z_corr, gauss_comb*z_corr/norm_flux, None,
-                               idx_line=idx_line, n_comps=1, observations_list=observations[i], color_dict=theme.colors)
+                               idx_line=idx_line, n_comps=1, observations_list=observations[i])
 
         # Gaussian component plot
         line_g_list[i] = _profile_plot(axis, wave_i/z_corr, (gauss_i+cont_i)*z_corr/norm_flux, latex_label,
-                                       idx_line=idx_line, n_comps=n_comps, observations_list=observations[i],
-                                       color_dict=theme.colors)
+                                       idx_line=idx_line, n_comps=n_comps, observations_list=observations[i])
 
     return line_g_list
 
 
 def _masks_plot(axis, line_list, x, y, z_corr, log, spectrum_mask, color_dict={}):
 
     # Spectrum mask
@@ -845,15 +793,15 @@
         units_flux = self._spec.units_flux
         redshift = self._spec.redshift
 
         # Assign the default axis labels
         PLOT_CONF = theme.fig_defaults(None)
         AXES_CONF = theme.ax_defaults(None, units_wave, units_flux, norm_flux)
 
-        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, redshift, False)
+        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(wave, flux, redshift, False)
 
         with rc_context(PLOT_CONF):
 
             fig, ax = plt.subplots()
 
             # Object spectrum
             ax.step(wave_plot, flux_plot, label='Object spectrum', color=theme.colors['fg'], where='mid')
@@ -873,42 +821,42 @@
             ax.update(AXES_CONF)
             ax.legend()
             plt.tight_layout()
             plt.show()
 
         return
 
-    def _plot_peak_detection(self, peak_idcs, detect_limit, continuum=None, plot_title='', ml_mask=None):
+    def _plot_peak_detection(self, peak_idcs, detect_limit, continuum, match_bands):
 
 
         norm_flux = self._spec.norm_flux
         wave = self._spec.wave
         flux = self._spec.flux
         units_wave = self._spec.units_wave
         units_flux = self._spec.units_flux
         redshift = self._spec.redshift
 
         PLOT_CONF = theme.fig_defaults(None)
         AXES_CONF = theme.ax_defaults(None, units_wave, units_flux, norm_flux)
 
-        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, redshift, 'observed')
+        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(wave, flux, redshift, 'observed')
 
         continuum = continuum if continuum is not None else np.zeros(flux.size)
 
+        idcs_detect = match_bands['signal_peak'].to_numpy(dtype=int)
+
         with rc_context(PLOT_CONF):
 
             fig, ax = plt.subplots()
             ax.step(wave_plot, flux_plot, color=theme.colors['fg'], label='Object spectrum', where='mid')
 
-            if ml_mask is not None:
-                if np.any(ml_mask):
-                    ax.scatter(wave_plot[ml_mask], flux_plot[ml_mask], label='ML detection', color='palegreen')
-
-            ax.scatter(wave_plot[peak_idcs], flux_plot[peak_idcs], marker='o', label='Peaks', color=theme.colors['peak'], facecolors='none')
+            ax.scatter(wave_plot[peak_idcs], flux_plot[peak_idcs], marker='o', label='Peaks', color=theme.colors['fade_fg'], facecolors='none')
             ax.fill_between(wave_plot, continuum, detect_limit, facecolor=theme.colors['line_band'], label='Noise_region', alpha=0.5)
+            ax.scatter(wave_plot[idcs_detect], flux_plot[idcs_detect], marker='o', label='Matched lines',
+                       color=theme.colors['peak'], facecolors='none')
 
             if continuum is not None:
                 ax.plot(wave_plot, continuum, label='Continuum')
 
             ax.scatter(wave_plot[idcs_mask], flux_plot[idcs_mask], label='Masked pixels', marker='x',
                        color=theme.colors['mask_marker'])
 
@@ -932,15 +880,16 @@
 
         # Container for the matplotlib figures
         self._fig, self._ax = None, None
 
         return
 
     def spectrum(self, output_address=None, label=None, line_bands=None, rest_frame=False, log_scale=False,
-                 include_fits=True, include_cont=False, in_fig=None, fig_cfg={}, ax_cfg={}, maximize=False):
+                 include_fits=True, include_cont=False, in_fig=None, fig_cfg={}, ax_cfg={}, maximize=False,
+                 detection_band=None):
 
         """
 
         This function plots the spectrum flux versus wavelength.
 
         The user can include the line bands on the plot if added via the ``line_bands`` attribute.
 
@@ -1012,57 +961,101 @@
             if in_fig is None:
                 in_fig, in_ax = self._plot_container(in_fig, None, AXES_CONF)
             else:
                 in_ax = in_fig.add_subplot()
                 in_ax.set(**AXES_CONF)
 
             # Reference _frame for the plot
-            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
-                                                                          self._spec.redshift, rest_frame)
+            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(self._spec.wave, self._spec.flux,
+                                                                        self._spec.redshift, rest_frame)
 
             # Plot the spectrum
-            in_ax.step(wave_plot / z_corr, flux_plot * z_corr, label=label, where='mid', color=theme.colors['fg'])
+            in_ax.step(wave_plot / z_corr, flux_plot * z_corr, label=label, where='mid', color=theme.colors['fg'],
+                       linewidth=theme.colors['spectrum_width'])
 
             # Plot peaks and troughs if provided
             if line_bands is not None:
                 line_bands = check_file_dataframe(line_bands, pd.DataFrame)
                 self._line_matching_plot(in_ax, line_bands, wave_plot, flux_plot, z_corr, self._spec.redshift,
                                          self._spec.units_wave)
 
             # Plot the fittings
-            if include_fits and self._spec.log is not None:
+            if include_fits and self._spec.frame is not None:
 
                 # List of lines in the log
-                line_list = self._spec.log.index.values
+                line_list = self._spec.frame.index.values
 
-                # Do not include the legend as the labels are necessary for mplcursors
+                # Do not include the legend as the labels are necessary for mplcursors # TODO improve mechanics
                 legend_check = False
 
                 if line_list.size > 0:
 
                     # Loop through the lines and plot them
                     profile_list = [None] * line_list.size
                     for i, line_label in enumerate(line_list):
 
-                        line_i = Line.from_log(line_label, self._spec.log)
-                        profile_list[i] = _profile_plt(in_ax, line_i, z_corr, self._spec.log, self._spec.redshift,
+                        line_i = Line.from_log(line_label, self._spec.frame)
+                        profile_list[i] = _profile_plt(in_ax, line_i, z_corr, self._spec.frame, self._spec.redshift,
                                                        self._spec.norm_flux)
 
                     # Add the interactive pop-ups
-                    _mplcursor_parser(profile_list, line_list, self._spec.log, self._spec.norm_flux, self._spec.units_wave,
+                    _mplcursor_parser(profile_list, line_list, self._spec.frame, self._spec.norm_flux, self._spec.units_wave,
                                       self._spec.units_flux)
 
                 # Plot the masked pixels
-                _masks_plot(in_ax, line_list, wave_plot, flux_plot, z_corr, self._spec.log, idcs_mask, theme.colors)
+                _masks_plot(in_ax, line_list, wave_plot, flux_plot, z_corr, self._spec.frame, idcs_mask, theme.colors)
 
             # Plot the normalize continuum
             if include_cont and self._spec.cont is not None:
-                in_ax.plot(wave_plot/z_corr, self._spec.cont, label='Fitted continuum', linestyle='--')
+                in_ax.plot(wave_plot/z_corr, self._spec.cont*z_corr, label='Continuum', color=theme.colors['fade_fg'], linestyle='--')
+
+                low_limit, high_limit = self._spec.cont-self._spec.cont_std, self._spec.cont + self._spec.cont_std
+                in_ax.fill_between(wave_plot/z_corr, low_limit*z_corr, high_limit*z_corr, alpha=0.2,
+                                   color=theme.colors['fade_fg'])
+
+            # Include the detection bands
+            if detection_band is not None:
+
+                detec_obj = getattr(self._spec.infer, 'line_1d_pred')
 
-            # Switch y_axis to logarithmic scale if requested
+                if detec_obj.confidence is not None:
+
+                    # Boundaries array for confidence intervals
+                    bounds = np.array([0.0, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0])
+
+                    # Adjust color map to match lower detection limit to fg color
+                    cmap = cm.get_cmap(theme.colors['mask_map'])
+                    cmaplist = [cmap(i) for i in range(cmap.N)]
+                    cmaplist[0] = theme.colors['fg']
+                    cmap = colors.LinearSegmentedColormap.from_list('mcm', cmaplist, bounds.size-1)
+                    norm = colors.BoundaryNorm(bounds * 100, cmap.N)
+
+                    # Iterate through the confidence intervals and plot the step spectrum
+                    for i in range(1, len(bounds)):
+                        if i > 1:
+                            idcs = detec_obj(bounds[i-1]*100, confidence_max=bounds[i]*100)
+                            wave_nan, flux_nan = np.full(wave_plot.size, np.nan), np.full(flux_plot.size, np.nan)
+                            wave_nan[idcs], flux_nan[idcs] = wave_plot[idcs] / z_corr, flux_plot[idcs] * z_corr
+
+                            in_ax.step(wave_nan, flux_nan, label=label, where='mid', color=cmap(i-1))
+
+
+                    # Color bar
+                    sm = cm.ScalarMappable(cmap=cmap, norm=norm)
+                    sm.set_array([])
+                    cbar = plt.colorbar(sm, ax=in_ax)
+                    cbar.set_label('Detection confidence %', rotation=270, labelpad=35)
+
+
+                else:
+                    _logger.warning(f'The line detection bands confidence has not been calculated. They are not included'
+                                    f' on plot.')
+
+
+                # Switch y_axis to logarithmic scale if requested
             if log_scale:
                 in_ax.set_yscale('log')
 
             # Add or remove legend according to the plot type:
             if legend_check:
                 in_ax.legend()
 
@@ -1123,15 +1116,15 @@
 
         """
 
         # Display check for the user figures
         display_check = True if in_fig is None else False
 
         # Link to observation log
-        log = self._spec.log
+        log = self._spec.frame
 
         # Check that the log type and content
         if not isinstance(log, pd.DataFrame):
             _logger.critical('The bands log for the grid plot must be a pandas dataframe')
 
         # Proceed
         if len(log.index) > 0:
@@ -1171,40 +1164,40 @@
 
                         in_ax = plt.subplot(grid_spec[i])
 
                         # Check components
                         line_i = Line.from_log(lineList[i], log, self._spec.norm_flux)
 
                         # Reference _frame for the plot
-                        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
-                                                                                      self._spec.redshift, rest_frame)
+                        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(self._spec.wave, self._spec.flux,
+                                                                                    self._spec.redshift, rest_frame)
 
                         # Establish the limits for the line spectrum plot
                         idcs_m = np.searchsorted(wave_plot, line_i.mask * (1 + self._spec.redshift))
                         idx_blue = idcs_m[0] - 5 if idcs_m[0] > 5 else idcs_m[0]
                         idx_red = idcs_m[-1] + 5 if idcs_m[-1] < idcs_m[-1] + 5 else idcs_m[-1]
 
                         # Plot the spectrum
                         in_ax.step(wave_plot[idx_blue:idx_red] / z_corr, flux_plot[idx_blue:idx_red] * z_corr,
-                                   where='mid', color=theme.colors['fg'])
+                                   where='mid', color=theme.colors['fg'], linewidth=theme.colors['spectrum_width'])
 
                         # Continuum bands
                         self._bands_plot(in_ax, wave_plot, flux_plot, z_corr, idcs_m, line_i)
 
                         # Plot the masked pixels
                         _masks_plot(in_ax, [line_i], wave_plot[idx_blue:idx_red], flux_plot[idx_blue:idx_red],
                                     z_corr, log, idcs_mask[idx_blue:idx_red], theme.colors)
 
                         # Plot the fitting results
                         if include_fits:
 
                             line_list, profiles_list = [line_i.label], line_i._p_shape
                             wave_array, gaussian_array = profiles_computation([line_i.label], log,
                                                                               (1 + self._spec.redshift), profiles_list)
-                            wave_array, cont_array = linear_continuum_computation(line_list, self._spec.log,
+                            wave_array, cont_array = linear_continuum_computation(line_list, self._spec.frame,
                                                                                   (1 + self._spec.redshift))
 
                             # Single component lines
                             line_g_list = _gaussian_line_profiler(in_ax, line_list, wave_array, gaussian_array,
                                                                   cont_array, z_corr, log, self._spec.norm_flux)
 
                             # Add the interactive pop-ups
@@ -1276,30 +1269,28 @@
 
         :param maximize: Maximise plot window. The default value is False.
         :type maximize:  bool, optional
 
         :return:
         """
 
-
-
         # TODO check plot without fit
         # Unpack variables
-        log, norm_flux, redshift = self._spec.log, self._spec.norm_flux, self._spec.redshift
+        log, norm_flux, redshift = self._spec.frame, self._spec.norm_flux, self._spec.redshift
         units_wave, units_flux = self._spec.units_wave, self._spec.units_flux
 
         # Display check for the user figures
         display_check = True if in_fig is None else False
 
         # If not line is provided use the last one
         if line is None:
             if log.index.size > 0:
                 line = log.index[-1]
 
-        # Reconsand to user for the analysis
+        # Reconstruct the line for the analysis
         if line is not None:
             line = Line.from_log(line, log, norm_flux)
 
         # Proceed to plot
         if line is not None:
 
             # Guess whether we need both lines
@@ -1324,45 +1315,46 @@
                     in_ax = (spec_ax, resid_ax)
                 else:
                     in_ax = [in_fig.add_subplot()]
 
                 in_ax[0].set(**AXES_CONF)
 
                 # Reference _frame for the plot
-                wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
-                                                                              redshift, rest_frame)
+                wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(self._spec.wave, self._spec.flux,
+                                                                            redshift, rest_frame)
                 err_plot = self._spec.err_flux
 
                 # Establish the limits for the line spectrum plot
                 mask = line.mask * (1 + self._spec.redshift)
                 idcsM = np.searchsorted(wave_plot, mask) # TODO remove this one
 
                 pixel_mask = 'no' if line not in log.index else log.loc[line, 'pixel_mask']
-                idcsEmis, idcsCont = define_masks(self._spec.wave, line.mask * (1 + self._spec.redshift), line_mask_entry=line.pixel_mask)
+                idcsEmis, idcsCont = define_masks(self._spec.wave, line.mask * (1 + self._spec.redshift),
+                                                  line_mask_entry=line.pixel_mask, line=line.label)
                 idcs_line = idcsEmis + idcsCont
 
                 # Plot the spectrum
                 label = '' if include_fits else line
                 in_ax[0].step(wave_plot[idcsM[0]:idcsM[5]] / z_corr, flux_plot[idcsM[0]:idcsM[5]] * z_corr,
-                              where='mid', color=theme.colors['fg'], label=label)
+                              where='mid', color=theme.colors['fg'], label=label, linewidth=theme.colors['spectrum_width'])
 
                 # Add the fitting results
                 if include_fits:
 
                     # Check components
                     list_comps = line.group_label.split('+') if line.blended_check else [line.label]
 
                     wave_array, gaussian_array = profiles_computation(list_comps, log, (1 + redshift), line._p_shape)
                     wave_array, cont_array = linear_continuum_computation(list_comps, log, (1 + redshift))
 
                     # Continuum bands
                     self._bands_plot(in_ax[0], wave_plot, flux_plot, z_corr, idcsM, line)
 
                     # Gaussian profiles
-                    idcs_lines = self._spec.log.index.isin(list_comps)
+                    idcs_lines = self._spec.frame.index.isin(list_comps)
                     line_g_list = _gaussian_line_profiler(in_ax[0], list_comps, wave_array, gaussian_array, cont_array,
                                                           z_corr, log.loc[idcs_lines], norm_flux)
 
                     # Add the interactive text
                     _mplcursor_parser(line_g_list, list_comps, log, norm_flux, units_wave, units_flux)
 
 
@@ -1410,19 +1402,19 @@
 
         # Adjust the default theme
         PLT_CONF = theme.fig_defaults(fig_cfg)
         AXES_CONF = theme.ax_defaults(ax_cfg, self._spec.units_wave, self._spec.units_flux, self._spec.norm_flux,
                                       fig_type='velocity')
 
         # Recover the line data
-        line = Line.from_log(line, self._spec.log, self._spec.norm_flux)
+        line = Line.from_log(line, self._spec.frame, self._spec.norm_flux)
 
         # Line spectrum
-        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
-                                                                      self._spec.redshift, False)
+        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(self._spec.wave, self._spec.flux,
+                                                                    self._spec.redshift, False)
 
         # Establish the limits for the line spectrum plot
         mask = band * (1 + self._spec.redshift)
         idcsM = np.searchsorted(wave_plot, mask)
 
         # Velocity spectrum for the line region
         flux_plot = flux_plot[idcsM[0]:idcsM[5]]
@@ -1444,15 +1436,16 @@
                 self._fig = in_fig
                 self._ax = self._fig.add_subplot()
 
             self._ax.set(**AXES_CONF)
             trans = self._ax.get_xaxis_transform()
 
             # Plot the spectrum
-            self._ax.step(vel_plot, flux_plot, label=line.latex_label, where='mid', color=theme.colors['fg'])
+            self._ax.step(vel_plot, flux_plot, label=line.latex_label, where='mid', color=theme.colors['fg'],
+                          linewidth=theme.colors['spectrum_width'])
 
             # Velocity percentiles
             target_percen = ['v_1', 'v_5', 'v_10', 'v_50', 'v_90', 'v_95', 'v_99']
             for i_percentil, percentil in enumerate(target_percen):
 
                 vel_per = line.__getattribute__(percentil)
                 label_text = None if i_percentil > 0 else r'$v_{Pth}$'
@@ -1516,28 +1509,28 @@
             save_close_fig_swicth(output_address, 'tight', in_fig, maximize, display_check)
 
         return
 
     def _residual_line_plotter(self, axis, x, y, err, list_comps, z_corr, spec_mask, cont_std, profile_list):
 
         # Unpack properties
-        log, norm_flux, redshift = self._spec.log, self._spec.norm_flux, self._spec.redshift
+        log, norm_flux, redshift = self._spec.frame, self._spec.norm_flux, self._spec.redshift
 
         # Continuum level
         cont_level = log.loc[list_comps[0], 'cont']
 
         # Calculate the fluxes for the residual plot
         cont_i_resd = linear_continuum_computation(list_comps, log, z_corr=(1 + redshift), x_array=x)
         gaussian_i_resd = profiles_computation(list_comps, log, (1 + redshift), profile_list, x_array=x)
         total_resd = gaussian_i_resd.sum(axis=1) + cont_i_resd[:, 0]
 
         # Lower plot residual
         label_residual = r'$\frac{F_{obs} - F_{fit}}{F_{cont}}$'
         residual = ((y - total_resd / norm_flux) / (cont_level/norm_flux))
-        axis.step(x/z_corr, residual*z_corr, where='mid', color=theme.colors['fg'])
+        axis.step(x/z_corr, residual*z_corr, where='mid', color=theme.colors['fg'], linewidth=theme.colors['spectrum_width'])
 
         # Shade Continuum flux standard deviation # TODO revisit this calculation
         label = r'$\sigma_{Continuum}/\overline{F_{cont}}$'
         y_limit = cont_std / cont_level
         axis.fill_between(x/z_corr, -y_limit, +y_limit, facecolor='yellow', alpha=0.5, label=label)
 
         # Shade the pixel error spectrum if available:
@@ -1553,52 +1546,56 @@
         try:
             axis.set_ylim(-resd_limit, resd_limit)
         except ValueError:
             _logger.warning(f'Nan or inf entries in axis limit for {self.bands}')
 
         # Residual plot labeling
         axis.legend(loc='center right')
-        axis.set_ylabel(label_residual, fontsize=22)
+        axis.set_ylabel(label_residual)
 
         # Spectrum mask
         _masks_plot(axis, [list_comps[0]], x, y, z_corr, log, spec_mask, color_dict=theme.colors)
 
         return
 
-    def _continuum_iteration(self, wave, flux, continuum_fit, idcs_cont, low_lim, high_lim, threshold_factor,
-                             plot_title=''):
-
-        PLOT_CONF = STANDARD_PLOT.copy()
-        AXES_CONF = STANDARD_AXES.copy()
+    def _continuum_iteration(self, wave, flux, continuum_fit, smooth_flux, idcs_cont, low_lim, high_lim, threshold_factor,
+                             user_ax):
 
-        norm_label = r' $\,/\,{}$'.format(latex_science_float(self._spec.norm_flux)) if self._spec.norm_flux != 1.0 else ''
-        AXES_CONF['ylabel'] = f'Flux $({UNITS_LATEX_DICT[self._spec.units_flux]})$' + norm_label
-        AXES_CONF['xlabel'] = f'Wavelength $({UNITS_LATEX_DICT[self._spec.units_wave]})$'
-        AXES_CONF['title'] = plot_title
+        PLT_CONF = theme.fig_defaults(None)
+        AXES_CONF = theme.ax_defaults(user_ax, self._spec.units_wave, self._spec.units_flux, self._spec.norm_flux)
 
-        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, self._spec.redshift, False)
+        smooth_check = True if np.all(flux != smooth_flux) else False
+        # wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(wave, flux, self._spec.redshift, False)
 
-        with rc_context(PLOT_CONF):
+        with rc_context(PLT_CONF):
 
             fig, ax = plt.subplots()
 
             # Object spectrum
-            ax.step(wave_plot, flux_plot, label='Object spectrum', color=self._color_dict['fg'], where='mid')
+            label_spec = 'Smoothed spectrum' if smooth_check else 'Object spectrum'
+            ax.step(wave, smooth_flux, label=label_spec, color=theme.colors['fg'], where='mid', linewidth=theme.colors['spectrum_width'])
+
+            # Unsmooth
+            if smooth_check:
+                ax.step(wave, flux, label='Input spectrum', color=theme.colors['fade_fg'], where='mid', linestyle=':',
+                        linewidth=theme.colors['spectrum_width'])
 
             # Band limits
             label = r'$16^{{th}}/{} - 84^{{th}}\cdot{}$ flux percentiles band'.format(threshold_factor, threshold_factor)
-            ax.axhspan(low_lim, high_lim, alpha=0.2, label=label, color=self._color_dict['line_band'])
-            ax.axhline(np.median(flux_plot[idcs_cont]), label='Median flux', linestyle=':', color='black')
+            # ax.axhspan(low_lim, high_lim, alpha=0.2, label=label, color=theme.colors['line_band'])
+            ax.axhline(np.median(smooth_flux[idcs_cont]), label='Median flux', linestyle=':', color='black')
+
+            ax.fill_between(wave, low_lim, high_lim, alpha=0.2, color=theme.colors['inspection_negative'])
 
             # Masked and rectected pixels
-            ax.scatter(wave_plot[~idcs_cont], flux_plot[~idcs_cont], label='Rejected pixels', color=self._color_dict['peak'], facecolor='none')
-            ax.scatter(wave_plot[idcs_mask], flux_plot[idcs_mask], marker='x', label='Masked pixels', color=self._color_dict['mask_marker'])
+            ax.scatter(wave[~idcs_cont], smooth_flux[~idcs_cont], label='Rejected pixels', color=theme.colors['peak'],
+                       facecolor='none')
 
             # Output continuum
-            ax.plot(wave_plot, continuum_fit, label='Continuum')
+            ax.plot(wave, continuum_fit, label='Continuum')
 
             ax.update(AXES_CONF)
             ax.legend()
             plt.tight_layout()
             plt.show()
 
         return
@@ -1613,18 +1610,14 @@
 
         # Lime spectrum object with the scientific data
         self._cube = cube
 
         # Container for the matplotlib figures
         self._fig, self._ax = None, None
 
-        # self.param_conv = {'SN_line': r'$\frac{S}{N}_{line}$',
-        #                    'SN_cont': r'$\frac{S}{N}_{cont}$',
-        #                    self._cube.units_flux: None}
-
         return
 
     def cube(self, line, bands=None, line_fg=None, output_address=None, min_pctl_bg=60, cont_pctls_fg=(90, 95, 99),
              bg_cmap='gray', fg_cmap='viridis', bg_norm=None, fg_norm=None, masks_file=None, masks_cmap='viridis_r',
              masks_alpha=0.2, wcs=None, fig_cfg=None, ax_cfg=None, in_fig=None, maximise=False):
 
 
@@ -1733,18 +1726,18 @@
         # Use the input wcs or use the parent one
         wcs = self._cube.wcs if wcs is None else wcs
 
         # False for embed figures
         display_check = True if in_fig is None else False
 
         # Set the plot format where the user's overwrites the default
-        size_conf = {'figure.figsize': (8 if masks_file is None else 15, 8)}
+        size_conf = {'figure.figsize': (4 if masks_file is None else 5.5, 4)}
         size_conf = size_conf if fig_cfg is None else {**size_conf, **fig_cfg}
 
-        PLT_CONF = theme.fig_defaults(size_conf)
+        PLT_CONF = theme.fig_defaults(size_conf, fig_type='cube')
         AXES_CONF = theme.ax_defaults(ax_cfg, self._cube.units_wave, self._cube.units_flux, self._cube.norm_flux,
                                       fig_type='cube', line_bg=line_bg, line_fg=line_fg, masks_dict=masks_dict, wcs=wcs)
 
         # Create and fill the figure
         with rc_context(PLT_CONF):
 
             if in_fig is None:
@@ -1811,65 +1804,66 @@
             if obj_idcs is None:
                 sub_sample = self._sample
             else:
                 sub_sample = self._sample[obj_idcs]
 
             # Check for logs without lines # TODO we need common method for just providing the first entry
             if 'line' in sub_sample.index.names:
-                obj_idcs = sub_sample.log.droplevel('line').index.unique()
+                obj_idcs = sub_sample.frame.droplevel('line').index.unique()
             else:
                 obj_idcs = sub_sample.index.unique()
 
             if len(obj_idcs) > 0:
 
                 # Create and fill the figure
                 with rc_context(PLT_CONF):
 
                     # Generate the figure object and figures
                     self._fig, self._ax = self._plot_container(in_fig, in_axis, AXES_CONF)
 
                     # Loop through the SMACS_v2.0 in the sample
                     for sample_idx in obj_idcs:
 
-                        legend_label = label_generator(sample_idx, self._sample.log, legend_handle)
-                        spec = self._sample.load_function(self._sample.log, sample_idx, self._sample.file_address,
+                        legend_label = label_generator(sample_idx, self._sample.frame, legend_handle)
+                        spec = self._sample.load_function(self._sample.frame, sample_idx, self._sample.file_address,
                                                           **self._sample.load_params)
 
                         # Reference _frame for the plot
-                        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(spec.wave, spec.flux, spec.redshift,
-                                                                                      rest_frame)
+                        wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(spec.wave, spec.flux, spec.redshift,
+                                                                                    rest_frame)
 
                         # Plot the spectrum
-                        self._ax.step(wave_plot / z_corr, flux_plot * z_corr, label=legend_label, where='mid')
+                        self._ax.step(wave_plot / z_corr, flux_plot * z_corr, label=legend_label, where='mid',
+                                      linewidth=theme.colors['spectrum_width'])
 
                         # List of lines in the log
-                        line_list = spec.log.index.values
+                        line_list = spec.frame.index.values
 
                         # Plot the fittings
                         if include_fits:
 
                             # Do not include the legend as the labels are necessary for mplcursors
                             legend_check = False
 
                             if line_list.size > 0:
 
-                                wave_array, gaussian_array = profiles_computation(line_list, spec.log, (1 + spec.redshift))
-                                wave_array, cont_array = linear_continuum_computation(line_list, spec.log, (1 + spec.redshift))
+                                wave_array, gaussian_array = profiles_computation(line_list, spec.frame, (1 + spec.redshift))
+                                wave_array, cont_array = linear_continuum_computation(line_list, spec.frame, (1 + spec.redshift))
 
                                 # Single component lines
                                 line_g_list = self._gaussian_line_profiler(self._ax, line_list,
                                                                            wave_array, gaussian_array, cont_array,
-                                                                           z_corr, spec.log, spec.norm_flux,)
+                                                                           z_corr, spec.frame, spec.norm_flux, )
 
                                 # Add the interactive pop-ups
-                                self._mplcursor_parser(line_g_list, line_list, spec.log, spec.norm_flux, spec.units_wave,
+                                self._mplcursor_parser(line_g_list, line_list, spec.frame, spec.norm_flux, spec.units_wave,
                                                        spec.units_flux)
 
                         # Plot the masked pixels
-                        _masks_plot(self._ax, line_list, wave_plot, flux_plot, z_corr, spec.log, idcs_mask)
+                        _masks_plot(self._ax, line_list, wave_plot, flux_plot, z_corr, spec.frame, idcs_mask)
 
                     # Switch y_axis to logarithmic scale if requested
                     if log_scale:
                         self._ax.set_yscale('log')
 
                     # Add or remove legend according to the plot type:
                     # TODO we should be able to separate labels from sample objects from line fits
@@ -1890,19 +1884,19 @@
     def properties(self, x_param, y_param, observation_list=None, x_param_err=None, y_param_err=None, labels_list=None,
                    groups_variable=None, output_address=None, in_fig=None, in_axis=None, plt_cfg={}, ax_cfg={},
                    log_scale=False):
 
         # Check selected variables are located in the panel columns
         for param in [x_param, y_param, x_param_err, y_param_err, groups_variable]:
             if param is not None:
-                if param not in self._sample.log:
+                if param not in self._sample.frame:
                     raise LiMe_Error(f'Variable {param} is not found in the sample panel columns')
 
         # Panel slice
-        slice_df = self._sample.log.loc[observation_list]
+        slice_df = self._sample.frame.loc[observation_list]
 
         # Confirm selection has data
         if len(slice_df) > 0:
 
             # Get variables arrays
             data = {'x_param': slice_df[x_param].values, 'y_values': slice_df[y_param].values,
                     'x_err': slice_df[x_param_err].values if x_param_err in slice_df else None,
```

### Comparing `lime-stable-0.9.99.5/src/lime/plots_interactive.py` & `lime-stable-1.0.0/src/lime/plots_interactive.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from pathlib import Path
 from matplotlib import pyplot as plt, gridspec, rc_context
 from matplotlib.widgets import RadioButtons, SpanSelector, Slider
 from astropy.io import fits
 
 from .io import load_frame, save_frame, LiMe_Error, check_file_dataframe, _LINES_DATABASE_FILE
-from .plots import Plotter, frame_mask_switch_2, save_close_fig_swicth, _auto_flux_scale,\
+from .plots import Plotter, frame_mask_switch, save_close_fig_swicth, _auto_flux_scale,\
                     determine_cube_images, load_spatial_mask, check_image_size, \
                     image_plot, spec_plot, spatial_mask_plot, _masks_plot, theme
 
 
 from .tools import blended_label_from_log, define_masks
 from .transitions import label_decomposition, Line
 
@@ -385,25 +385,26 @@
             ax.set_facecolor(self._color_bg[active_check])
 
             # Check components
             blended_check, profile_label = blended_label_from_log(line, self.log)
             list_comps = profile_label.split('+') if blended_check else [line]
 
             # Reference _frame for the plot
-            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(self._spec.wave, self._spec.flux,
-                                                                          self._spec.redshift, frame)
+            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(self._spec.wave, self._spec.flux,
+                                                                        self._spec.redshift, frame)
 
             # Establish the limits for the line spectrum plot
             mask = self.log.loc[list_comps[0], 'w1':'w6'] * (1 + self._spec.redshift)
             idcsM = np.searchsorted(wave_plot, mask)
             idxL = idcsM[0] - 5 if idcsM[0] > 5 else idcsM[0]
             idxH = idcsM[-1] + 5 if idcsM[-1] < idcsM[-1] + 5 else idcsM[-1]
 
             # Plot the spectrum
-            ax.step(wave_plot[idxL:idxH]/z_corr, flux_plot[idxL:idxH]*z_corr, where='mid', color=theme.colors['fg'])
+            ax.step(wave_plot[idxL:idxH]/z_corr, flux_plot[idxL:idxH]*z_corr, where='mid', color=theme.colors['fg'],
+                    linewidth=theme.colors['spectrum_width'])
 
             # Continuum bands
             self._bands_plot(ax, wave_plot, flux_plot, z_corr, idcsM, line)
 
             # Plot the masked pixels
             _masks_plot(ax, [line], wave_plot[idxL:idxH], flux_plot[idxL:idxH], z_corr, self.log, idcs_mask[idxL:idxH],
                         color_dict=theme.colors)
@@ -684,35 +685,36 @@
 
     def _plot_spectrum_ZI(self, ax):
 
         # Loop through the objects
         for i, obj_idx in enumerate(self._obj_idcs):
 
             # Load the spectrum
-            spec = self._sample.load_function(self._sample.log, obj_idx, **self._sample.load_params)
+            spec = self._sample.load_function(self._sample.frame, obj_idx, **self._sample.load_params)
 
             # Plot on the observed frame with reshift = 0
-            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(spec.wave, spec.flux, 0, 'observed')
+            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(spec.wave, spec.flux, 0, 'observed')
 
             # Plot the spectrum
-            ax.step(wave_plot/z_corr, flux_plot*z_corr, label=self._label_generator(obj_idx), where='mid')
+            ax.step(wave_plot/z_corr, flux_plot*z_corr, label=self._label_generator(obj_idx), where='mid',
+                    linewidth=theme.colors['spectrum_width'])
 
             # Plot the masked pixels
-            _masks_plot(ax, None, wave_plot, flux_plot, z_corr, spec.log, idcs_mask, color_dict=self._color_dict)
+            _masks_plot(ax, None, wave_plot, flux_plot, z_corr, spec.frame, idcs_mask, color_dict=self._color_dict)
 
         return
 
     def _plot_line_labels_ZI(self, ax, click_coord, redshift_pred):
 
         if (redshift_pred != 0) and (not pd.isnull(redshift_pred)):
             wave_min, wave_max = None, None
             for obj_idx in self._obj_idcs:
 
                 # Load the spectrum
-                spec = self._sample.load_function(self._sample.log, obj_idx, **self._sample.load_params)
+                spec = self._sample.load_function(self._sample.frame, obj_idx, **self._sample.load_params)
 
                 wavelength = spec.wave.data if np.ma.isMaskedArray(spec.wave) else spec.wave
                 wavelength = wavelength[~np.isnan(wavelength)]
 
                 if wave_min is None:
                     wave_min = wavelength[0]
                 else:
@@ -815,16 +817,16 @@
 
         else:
 
             if self._legend_handle in self._sample.index.names:
                 idx_item = list(self._sample.index.names).index(self._legend_handle)
                 spec_label = idx_sample[idx_item]
 
-            elif self._legend_handle in self._sample.log.columns:
-                spec_label = self._sample.log.loc[idx_sample, self._legend_handle]
+            elif self._legend_handle in self._sample.frame.columns:
+                spec_label = self._sample.frame.loc[idx_sample, self._legend_handle]
 
             else:
                 raise LiMe_Error(f'The input handle "{self._legend_handle}" is not found on the sample log columns')
 
 
         return spec_label
 
@@ -879,15 +881,15 @@
 
         # Check all the object indeces are in the output indecs
         if np.sum(self._obj_idcs.isin(self._output_idcs)) < self._obj_idcs.size:
             _logger.warning(f'Some of the input "obj_idcs" are not present in output "output_idcs" this can cause issues'
                             f' on the displayed spectrum')
 
         # Check the redshift column exists
-        if self._column_log not in self._sample.log.columns:
+        if self._column_log not in self._sample.frame.columns:
             raise LiMe_Error(f'Redshift column "{redshift_column}" does not exist in the current sample log.')
 
         # Read initial value for the redshift
         redshift_pred = self._sample.loc[self._obj_idcs, self._column_log].to_numpy()
         redshift_pred = None if np.all(pd.isnull(redshift_pred)) else np.nanmean(redshift_pred)
 
         # Create initial entry
@@ -982,35 +984,36 @@
 
     def _plot_spectrum_ZI(self, ax):
 
         # Loop through the objects
         for i, obj_idx in enumerate(self._obj_idcs):
 
             # Load the spectrum
-            spec = self._sample.load_function(self._sample.log, obj_idx, **self._sample.load_params)
+            spec = self._sample.load_function(self._sample.frame, obj_idx, **self._sample.load_params)
 
             # Plot on the observed frame with reshift = 0
-            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch_2(spec.wave, spec.flux, 0, 'observed')
+            wave_plot, flux_plot, z_corr, idcs_mask = frame_mask_switch(spec.wave, spec.flux, 0, 'observed')
 
             # Plot the spectrum
-            ax.step(wave_plot/z_corr, flux_plot*z_corr, label=self._label_generator(obj_idx), where='mid')
+            ax.step(wave_plot/z_corr, flux_plot*z_corr, label=self._label_generator(obj_idx), where='mid',
+                    linewidth=theme.colors['spectrum_width'])
 
             # Plot the masked pixels
-            _masks_plot(ax, None, wave_plot, flux_plot, z_corr, spec.log, idcs_mask, color_dict=self._color_dict)
+            _masks_plot(ax, None, wave_plot, flux_plot, z_corr, spec.frame, idcs_mask, color_dict=self._color_dict)
 
         return
 
     def _plot_line_labels_ZI(self, ax, click_coord, redshift_pred):
 
         if (redshift_pred != 0) and (not pd.isnull(redshift_pred)):
             wave_min, wave_max = None, None
             for obj_idx in self._obj_idcs:
 
                 # Load the spectrum
-                spec = self._sample.load_function(self._sample.log, obj_idx, **self._sample.load_params)
+                spec = self._sample.load_function(self._sample.frame, obj_idx, **self._sample.load_params)
 
                 wavelength = spec.wave.data if np.ma.isMaskedArray(spec.wave) else spec.wave
                 wavelength = wavelength[~np.isnan(wavelength)]
 
                 if wave_min is None:
                     wave_min = wavelength[0]
                 else:
@@ -1077,15 +1080,15 @@
             _redshift_pred = redshift_output
 
         # Store the new redshift
         self._sample.loc[self._output_idcs, self._column_log] = _redshift_pred
 
         # Save to file if provided
         if self._log_address is not None:
-            save_frame(self._log_address, self._sample.log)
+            save_frame(self._log_address, self._sample.frame)
 
         return
 
     def _button_ZI(self, line_selection):
 
         # Button selection
         self._lineSelection = line_selection
@@ -1120,16 +1123,16 @@
 
         else:
 
             if self._legend_handle in self._sample.index.names:
                 idx_item = list(self._sample.index.names).index(self._legend_handle)
                 spec_label = idx_sample[idx_item]
 
-            elif self._legend_handle in self._sample.log.columns:
-                spec_label = self._sample.log.loc[idx_sample, self._legend_handle]
+            elif self._legend_handle in self._sample.frame.columns:
+                spec_label = self._sample.frame.loc[idx_sample, self._legend_handle]
 
             else:
                 raise LiMe_Error(f'The input handle "{self._legend_handle}" is not found on the sample log columns')
 
 
         return spec_label
 
@@ -1166,15 +1169,15 @@
         self.log_scale = None
 
         return
 
     def cube(self, line, bands=None, line_fg=None, min_pctl_bg=60, cont_pctls_fg=(90, 95, 99), bg_cmap='gray',
              fg_cmap='viridis', bg_norm=None, fg_norm=None, masks_file=None, masks_cmap='viridis_r', masks_alpha=0.2,
              rest_frame=False, log_scale=False, fig_cfg=None, ax_cfg_image=None, ax_cfg_spec=None, in_fig=None,
-             lines_log_file=None, ext_log='_LINELOG', wcs=None, maximize=False):
+             lines_file=None, ext_frame_suffix='_LINELOG', wcs=None, maximize=False):
 
         """
 
         This function opens an interactive plot to display and individual spaxel spectrum from the selection on the
         image map.
 
         The left-hand side plot displays an image map with the flux sum of a line band as described on the
@@ -1246,29 +1249,29 @@
 
         :param ax_cfg_image: Dictionary with the image band flux plot "xlabel", "ylabel" and "title" values.
         :type ax_cfg_image: dict, optional
 
         :param ax_cfg_spec: Dictionary with the spaxel spectrum plot "xlabel", "ylabel" and "title" values.
         :type ax_cfg_spec: dict, optional
 
-        :param lines_log_file: Address for the line measurements log ".fits" file.
-        :type lines_log_file: str, pathlib.Path, optional
+        :param lines_file: Address for the line measurements log ".fits" file.
+        :type lines_file: str, pathlib.Path, optional
 
-        :param ext_log: Suffix for the line measurements log spaxel page name
-        :type ext_log: str, optional
+        :param ext_frame_suffix: Suffix for the line measurements log spaxel page name
+        :type ext_frame_suffix: str, optional
 
         :param wcs: Observation `world coordinate system <https://docs.astropy.org/en/stable/wcs/index.html>`_.
         :type wcs: astropy WCS, optional
 
         :param maximize: Maximise plot window. The default value is False.
         :type maximize:  bool, optional
 
         """
 
-        self.ext_log = ext_log
+        self.ext_log = ext_frame_suffix
         self.mask_file = masks_file
 
         # Prepare the background image data
         line_bg, self.bg_image, self.bg_levels, self.bg_scale = determine_cube_images(self._cube, line, bands,
                                                                                       min_pctl_bg, bg_norm, contours_check=False)
 
         # Prepare the foreground image data
@@ -1307,38 +1310,38 @@
 
         if len(self.masks_dict) > 0:
             self.mask_ext = list(self.masks_dict.keys())[0]
         else:
             self.mask_ext = self.ext_log
 
         # Load the complete fits lines log if input
-        if lines_log_file is not None:
-            if Path(lines_log_file).is_file():
-                self.hdul_linelog = fits.open(lines_log_file, lazy_load_hdus=False)
+        if lines_file is not None:
+            if Path(lines_file).is_file():
+                self.hdul_linelog = fits.open(lines_file, lazy_load_hdus=False)
             else:
-                _logger.info(f'The lines log at {lines_log_file} was not found.')
+                _logger.info(f'The lines log at {lines_file} was not found.')
 
         # Get figure configuration configuration
         self.fig_conf = theme.fig_defaults(fig_cfg, fig_type='cube_interactive')
         ax_im = theme.ax_defaults(ax_cfg_image, self._cube.units_wave, self._cube.units_flux, self._cube.norm_flux,
                                 fig_type='cube', line_bg=line_bg, line_fg=line_fg, masks_dict=self.masks_dict, wcs=wcs)
         ax_spec = theme.ax_defaults(ax_cfg_spec, self._cube.units_wave, self._cube.units_flux, self._cube.norm_flux,
-                               g_type='default', line_bg=line_bg, line_fg=line_fg, masks_dict=self.masks_dict, wcs=wcs)
+                                g_type='default', line_bg=line_bg, line_fg=line_fg, masks_dict=self.masks_dict, wcs=wcs)
         self.axes_conf = {'image': ax_im, 'spectrum': ax_spec}
 
         # Create the figure
         with rc_context(self.fig_conf):
 
             # Figure structure
             self._fig = plt.figure() if in_fig is None else in_fig
             gs = gridspec.GridSpec(nrows=1, ncols=2, figure=self._fig, width_ratios=[1, 2], height_ratios=[1])
 
             # Create subgrid for buttons if mask file provided
             if len(self.masks_dict) > 0:
-                gs_image = gridspec.GridSpecFromSubplotSpec(nrows=2, ncols=1, subplot_spec=gs[0], height_ratios=[0.8, 0.2])
+                gs_image = gridspec.GridSpecFromSubplotSpec(nrows=2, ncols=1, subplot_spec=gs[0], height_ratios=[0.7, 0.3])
             else:
                 gs_image = gs
 
             # Image axes Astronomical coordinates if provided
             if wcs is None:
                 self._ax0 = self._fig.add_subplot(gs_image[0])
             else:
@@ -1350,19 +1353,19 @@
 
             # Buttons axis if provided
             if len(self.masks_dict) > 0:
                 self._ax2 = self._fig.add_subplot(gs_image[1])
                 radio = RadioButtons(self._ax2, list(self.masks_dict.keys()))
 
                 for r in radio.labels:
-                    r.set_fontsize(10)
+                    r.set_fontsize(5)
 
-                for circle in radio.circles:  # Make the buttons a bit rounder
-                    # circle.set_height(0.025)
-                    circle.set_width(0.04)
+                # for circle in radio.circles:  # Make the buttons a bit rounder
+                #     # circle.set_height(0.025)
+                #     circle.set_width(0.04)
 
             # Plot the data
             self.data_plots()
 
             # Connect the widgets
             self._fig.canvas.mpl_connect('button_press_event', self.on_click)
             self._fig.canvas.mpl_connect('axes_enter_event', self.on_enter_axes)
@@ -1409,15 +1412,15 @@
 
                 except KeyError:
                     _logger.info(f'Extension {ext_name} not found in the input file')
 
             # Plot spectrum
             spec_plot(self._ax1, self._cube.wave, flux_voxel, self._cube.redshift, self._cube.norm_flux,
                       rest_frame=self.rest_frame, log=log, units_wave=self._cube.units_wave,
-                      units_flux=self._cube.units_flux, color_dict=theme.colors)
+                      units_flux=self._cube.units_flux)
 
             if self.log_scale:
                 self._ax.set_yscale('log')
 
         # Update the axis
         self.axes_conf['spectrum']['title'] = f'Spaxel {idx_j} - {idx_i}'
         self._ax0.update(self.axes_conf['image'])
@@ -1537,15 +1540,16 @@
              fig_cfg={}, ax_cfg_image={}, ax_cfg_spec={}, in_fig=None, wcs=None, maximize=False):
 
         # --------------- Compute the cumilative signal to noise ---------------------------
         # TODO finish this one
         line_bg = Line(line, bands)
 
         # Get the band indexes
-        idcsEmis, idcsCont = define_masks(self._cube.wave, line_bg.mask * (1 + self._cube.redshift), line_bg.pixel_mask)
+        idcsEmis, idcsCont = define_masks(self._cube.wave, line_bg.mask * (1 + self._cube.redshift), line_mask_entry=line_bg.pixel_mask,
+                                          line=line.label)
         signal_slice = self._cube.flux[idcsEmis, :, :]
 
         # Compute the Signal to noise in the complete image
         n_pixels = np.sum(idcsCont)
         cont_slice = self._cube.flux[idcsCont, :, :]
         Amp_image = np.nanmax(signal_slice, axis=0) - np.nanmean(cont_slice, axis=0)
         std_image = np.nanstd(cont_slice, axis=0)
```

### Comparing `lime-stable-0.9.99.5/src/lime/read_fits.py` & `lime-stable-1.0.0/src/lime/read_fits.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,41 +15,56 @@
     requests_check = False
 
 
 _logger = logging.getLogger('LiMe')
 
 DESI_SPECTRA_BANDS = ('B', 'R', 'Z')
 
+SPECTRUM_FITS_PARAMS = {'nirspec': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None,
+                                    'units_wave': 'um', 'units_flux': 'MJy', 'pixel_mask': "nan", 'id_label': None},
 
-SPECTRUM_FITS_PARAMS = {'nirspec': {'redshift': None, 'norm_flux': None, 'inst_FWHM': np.nan,
-                                'units_wave': 'um', 'units_flux': 'mJy', 'pixel_mask': None, 'id_label': None},
+                        'isis': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None,
+                                 'units_wave': 'Angstrom', 'units_flux': 'FLAM', 'pixel_mask': "nan", 'id_label': None},
 
-                        'isis': {'redshift': None, 'norm_flux': None, 'inst_FWHM': np.nan,
-                                 'units_wave': 'FLAM', 'units_flux': 'mJy', 'pixel_mask': None, 'id_label': None},
+                        'osiris': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
+                                   'units_flux': 'FLAM', 'pixel_mask': "nan", 'id_label': None},
 
-                        'osiris': {'redshift': None, 'norm_flux': None, 'inst_FWHM': np.nan, 'units_wave': 'AA',
-                                   'units_flux': 'FLAM', 'pixel_mask': None, 'id_label': None},
+                        'sdss': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
+                                 'units_flux': '1e-17*FLAM', 'pixel_mask': None, 'id_label': None},
 
-                        'sdss': {'redshift': None, 'norm_flux': None, 'inst_FWHM': np.nan, 'units_wave': 'AA',
-                                 'units_flux': 'FLAM', 'pixel_mask': None, 'id_label': None},
+                        'desi': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
+                                 'units_flux': '1e-17*FLAM', 'pixel_mask': "nan", 'id_label': None}}
 
-                        'desi': {'redshift': None, 'norm_flux': None, 'inst_FWHM': np.nan, 'units_wave': 'AA',
-                                 'units_flux': '1e-17*FLAM', 'pixel_mask': None, 'id_label': None}
+CUBE_FITS_PARAMS = {'manga': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
+                              'units_flux': '1e-17*FLAM', 'pixel_mask': "nan", 'id_label': None},
 
-                        }
+                    'muse':  {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
+                              'units_flux': '1e-20*FLAM', 'pixel_mask': "nan", 'id_label': None},
 
-CUBE_FITS_PARAMS = {'manga': {'redshift': None, 'norm_flux': None, 'inst_FWHM': np.nan, 'units_wave': 'AA',
-                              'units_flux': 'FLAM', 'pixel_mask': None, 'id_label': None},
+                    'megara': {'redshift': None, 'norm_flux': None, 'inst_FWHM': None, 'units_wave': 'Angstrom',
+                               'units_flux': 'Jy', 'pixel_mask': "nan", 'id_label': None}}
 
-                    'muse':  {'redshift': None, 'norm_flux': None, 'inst_FWHM': np.nan, 'units_wave': 'AA',
-                              'units_flux': '1e-17*FLAM', 'pixel_mask': None, 'id_label': None},
 
-                    'megara': {'redshift': None, 'norm_flux': None, 'inst_FWHM': np.nan, 'units_wave': 'AA',
-                               'units_flux': 'Jy', 'pixel_mask': None, 'id_label': None}
-                    }
+def show_instrument_cfg():
+
+    print(f'\nSingle ".fits" spectra files configuration:')
+    for i, items in enumerate(SPECTRUM_FITS_PARAMS.items()):
+        key, value = items
+        print(f'{i} {key}) \t units_wave: {value["units_wave"]}, units_flux: {value["units_flux"]}, '
+              f'pixel_mask: {value["pixel_mask"]}, inst_FWHM: {value["inst_FWHM"]}')
+        # print(f'\t\t pixel mask: {value["pixel_mask"]}, instrumental FWHM: {value["inst_FWHM"]}')
+
+    print(f'\nCube ".fits" spectra files configuration:')
+    for i, items in enumerate(CUBE_FITS_PARAMS.items()):
+        key, value = items
+        print(f'{i} {key}) \t units_wave: {value["units_wave"]}, units_flux: {value["units_flux"]},'
+              f'pixel_mask: {value["pixel_mask"]}, inst_FWHM: {value["inst_FWHM"]}')
+        # print(f'\t\t pixel mask: {value["pixel_mask"]}, instrumental FWHM: {value["inst_FWHM"]}')
+
+    return
 
 
 def check_url_status(url):
 
     url_check = False
 
     if requests_check:
@@ -187,14 +202,15 @@
     return output
 
 
 def check_load_function():
 
     return
 
+
 def url_validator(url):
 
     valid_output = False
     message = None
     try:
         response = requests.options(url)
         if response.ok:  # alternatively you can use response.status_code == 200
@@ -315,32 +331,52 @@
 
         return
 
     def parse_data_from_file(self, file_address, pixel_mask=None):
 
         # Read the fits data
         wave_array, flux_array, err_array, header_list, fits_params = self.fits_reader(file_address)
+        pixel_mask = pixel_mask if pixel_mask is not None else fits_params['pixel_mask']
 
         # Mask requested entries
         if pixel_mask is not None:
             pixel_mask = np.atleast_1d(pixel_mask)
             mask_array = np.zeros(flux_array.shape).astype(bool)
-            for entry in pixel_mask:
-                if entry == 'negative':
-                    idcs = flux_array < 0
-                else:
-                    idcs = (flux_array == entry)
-                mask_array[idcs] = True
+
+            # String array:
+            if pixel_mask.dtype.kind in ['U', 'S']:
+                for entry in pixel_mask:
+                    if entry == 'negative':
+                        idcs = flux_array < 0
+                    elif entry == 'nan':
+                        idcs = np.isnan(flux_array) if err_array is None else np.isnan(flux_array) | np.isnan(err_array)
+                    elif entry == 'zero':
+                        idcs = (flux_array == entry) if err_array is None else (flux_array == entry) | (err_array == entry)
+                    else:
+                        raise LiMe_Error(f'Pixel entry "{entry}" is not recognized. Only boolean masks for the masked '
+                                         f'data or these strings are supported: "nan", "negative", "zero"')
+                    mask_array[idcs] = True
+
+            # Boolean mask
+            else:
+                assert flux_array.shape == pixel_mask.shape, LiMe_Error(f'- Input pixel mask shape {pixel_mask.shape}'
+                                                                        f'is different from data array shape {flux_array.shape}')
+                mask_array = pixel_mask
+
         else:
             mask_array = None
 
         # Construct attributes for LiMe object
-        fits_args = {'input_wave': wave_array, 'input_flux': flux_array, 'input_err': err_array, 'pixel_mask': mask_array}
+        fits_args = {'input_wave': wave_array, 'input_flux': flux_array, 'input_err': err_array}#'pixel_mask': mask_array}
         fits_args.update(fits_params)
 
+        # Add mask entry
+        if mask_array is not None:
+            fits_args['pixel_mask'] = mask_array
+
         return fits_args
 
     def parse_data_from_url(self, id_label, pixel_mask=None, **kwargs):
 
         # Read the fits data
         wave_array, flux_array, err_array, header_list, fits_params = self.fits_reader(id_label,  **kwargs)
 
@@ -525,15 +561,15 @@
         :return: wavelength array, flux array, uncertainty array, header list, observation parameter dict
 
         """
 
         # Get data table and header dict lists
         data_list, header_list = load_fits(fits_address, data_ext_list, hdr_ext_list, url_check=False)
 
-        # Re-construct spectrum arrays
+        # Re-construct spectrum arrays # TODO add error
         wave_array = 10.0 ** data_list[0]['loglam']
         flux_array = data_list[0]['flux']
         err_array = None
 
         # Spectrum properties
         params_dict = SPECTRUM_FITS_PARAMS['sdss']
 
@@ -568,22 +604,28 @@
         data_list, header_list = load_fits(fits_address, data_ext_list, hdr_ext_list, url_check=False)
 
         # Re-construct spectrum arrays
         wave_array = data_list[0]
         flux_cube = data_list[1]
         ivar_cube = data_list[1]
 
-        pixel_mask_cube = ivar_cube == 0
-        pixel_mask_cube = pixel_mask_cube.reshape(ivar_cube.shape)
-        err_cube = np.sqrt(1 / np.ma.masked_array(ivar_cube, pixel_mask_cube))
+        # Convert ivar = 0 to nan
+        ivar_cube[ivar_cube == 0] = np.nan
+
+        # Get standard deviation cube
+        err_cube = np.sqrt(1 / ivar_cube)
+
+        # Pixel mask
+        pixel_mask_cube = None
 
+        # WCS from hearder
         wcs = WCS(header_list[0])
 
         # Fits properties
-        fits_params = {**CUBE_FITS_PARAMS['manga'], 'pixel_mask': pixel_mask_cube, 'wcs': wcs}
+        fits_params = {**CUBE_FITS_PARAMS['manga'], 'wcs': wcs}
 
         return wave_array, flux_cube, err_cube, header_list, fits_params
 
     @staticmethod
     def muse(fits_address, data_ext_list=(1, 2), hdr_ext_list=1, pixel_mask=None):
 
         """
```

### Comparing `lime-stable-0.9.99.5/src/lime/recognition.py` & `lime-stable-1.0.0/src/lime/recognition.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 from scipy import signal
 from lmfit.models import PolynomialModel
 from inspect import signature
 from .io import LiMe_Error, check_file_dataframe
 from .transitions import label_decomposition
 import astropy.units as au
+from timeit import default_timer as timer
 
 try:
     import joblib
     joblib_check = True
 except ImportError:
     joblib_check = False
 
@@ -73,27 +74,85 @@
 
     else:
         raise KeyError(f'Input scaling "{transformation}" is not recognized.')
 
     return data_norm
 
 
+def enbox_spectrum(input_flux, box_size, range_box):
+
+    # Use only the true entries from the mask
+    flux_array = input_flux if not np.ma.isMaskedArray(input_flux) else input_flux.data[~input_flux.mask]
+
+    # Reshape to the detection interval
+    n_intervals = flux_array.size - box_size + 1
+    flux_array = flux_array[np.arange(n_intervals)[:, None] + range_box]
+
+    # # Remove nan entries
+    # idcs_nan_rows = np.isnan(input_flux).any(axis=1)
+    # flux_array = input_flux[~idcs_nan_rows, :]
+
+    return flux_array
+
+
+def flux_to_image(flux_array, approximation, model_2D):
+
+    if model_2D is not None:
+
+        img_flux_array = np.tile(flux_array[:, None, :, :], (1, approximation.size, 1, 1))
+        img_flux_array = img_flux_array > approximation[::-1, None, None]
+        img_flux_array = img_flux_array.astype(int)
+        img_flux_array = img_flux_array.reshape((flux_array.shape[0], 1, -1, flux_array.shape[-1]))
+        img_flux_array = img_flux_array.squeeze()
+
+        # Original
+        # flux_array_0 = flux_array[:, :, 0]
+        # Old_img = np.tile(flux_array_0[:, None, :], (1, approximation.size, 1))
+        # Old_img = Old_img > approximation[::-1, None]
+        # Old_img = Old_img.astype(int)
+        # Old_img = Old_img.reshape((flux_array_0.shape[0], 1, -1))
+        # Old_img = Old_img.squeeze()
+
+    else:
+      img_flux_array = None
+
+    return img_flux_array
+
+
+def prop_func(data_arr, box_width):
+
+    prop_arr = np.zeros(data_arr.shape, dtype=bool)
+    idcs_true = np.argwhere(data_arr) + np.arange(box_width)
+    idcs_true = idcs_true.flatten()
+    idcs_true = idcs_true[idcs_true < data_arr.size] # in case the error propagation gives a great
+    prop_arr[idcs_true] = True
+
+    # Original
+    # self.mask = np.zeros(n_pixels, dtype=bool)
+    # idcs_detect = np.argwhere(pred_array[:, 0]) + range_box
+    # idcs_detect = idcs_detect.flatten()
+    # idcs_detect = idcs_detect[idcs_detect < pred_array[:, 0].size]
+    # self.mask[idcs_detect] = True
+
+    return prop_arr
+
+
 class LineFinder:
 
     def __init__(self, machine_model_path=MACHINE_PATH):
 
         # self.ml_model = joblib.load(machine_model_path) # THIS CAN be warning at opening the file
 
         return
 
     def continuum_fitting(self, degree_list=[3, 7, 7, 7], threshold_list=[5, 3, 2, 2], plot_results=False,
                           return_std=False):
 
         # Check for a masked array
-        if np.ma.is_masked(self.flux):
+        if np.ma.isMaskedArray(self.flux):
             mask_cont = ~self.flux.mask
             input_wave, input_flux = self.wave.data, self.flux.data
         else:
             mask_cont = np.ones(self.flux.size).astype(bool)
             input_wave, input_flux = self.wave, self.flux
 
 
@@ -135,36 +194,21 @@
             std_spec = np.std((self.flux-continuum_fit)[mask_cont])
             output_params = (continuum_fit, std_spec)
         else:
             output_params = continuum_fit
 
         return output_params
 
-    def peak_detection(self, limit_threshold=None, continuum=None, distance=4, ml_mask=None, plot_results=False):
-
-        # No user imput provided compute the intensity threshold from the 84th percentil
-        limit_threshold = np.percentile(self.flux, 84) if limit_threshold is None else limit_threshold
-        limit_threshold = limit_threshold + continuum if continuum is not None else limit_threshold
-
-        peak_fp, _ = signal.find_peaks(self.flux, height=limit_threshold, distance=distance)
-
-        # Plot the results
-        if plot_results:
-            self.plot._plot_peak_detection(peak_fp, limit_threshold, continuum, ml_mask=ml_mask,
-                                      plot_title='Peak detection results ')
-
-        return peak_fp
-
     def ml_line_detection(self, continuum, box_width=11, model= None):
 
         if model is None:
             model = joblib.load(MACHINE_PATH)
 
         # Normalize the flux
-        input_flux = self.flux if not np.ma.is_masked(self.flux) else self.flux.data
+        input_flux = self.flux if not np.ma.isMaskedArray(self.flux) else self.flux.data
         input_flux = np.log10((input_flux/continuum - 1) + 10)
 
         # Reshape to the training dimensions
         input_flux = np.array(input_flux, ndmin=2)
 
         # Container for the true pixels
         detection_mask = np.zeros(self.flux.size).astype(bool)
@@ -176,111 +220,88 @@
                 y = input_flux[:, i:i + box_width]
                 if not np.any(np.isnan(y)):
                     detection_mask[i:i + box_width] = detection_mask[i:i + box_width] | model.predict(y)[0]
                     # print(f'y {i} ({np.sum(y)}): {self.ml_model.predict(y)[0]}')
 
         return detection_mask
 
-    def line_detection(self, bands=None, cont_fit_degree=(3, 7, 7, 7), cont_int_thres=(5, 3, 2, 2), noise_sigma_factor=3,
-                       line_type='emission', width_tol=5, band_modification=None, ml_detection=None, plot_cont_calc=False,
-                       plot_peak_calc=False):
+    def line_detection(self, bands, sigma_threshold=3, emission_type=True, width_tol=5, band_modification=None,
+                       continuum_array=None, continuum_std=None, plot_steps=False):
 
         """
 
         This function compares the input lines bands in the observation spectrum to confirm the presence of lines.
 
         The input bands can be specified as a pandas dataframe or the path to its file via the ``bands_df`` argument.
 
-        Prior to the line detection, the spectrum continuum is fit in an iterative process. The ``cont_fit_degree`` array
-        provides the order of the fitting polynomial, while the ``cont_int_thres`` array provides the threshold intensity
-        factor for the threshold flux above and below the continuum to exclude at each iteration.
+        The continuum needs to be fit a priori with the Spectrum.fit.continuum function or assigning a ``continuum_array``
+        and a ``continuum_std``.
+
+        The ``sigma_threshold`` establishes the standard deviation factor beyond which a positive line detection is assumed.
 
-        After the continuum has been normalized, the ``noise_sigma_factor`` establishes the standard deviation factor
-        beyond which a positive line detection is assumed.
+        By default the algorithm seeks for emission lines, set ``emission_type`` equal to False for absorption lines.
 
         The additional arguments provide additional tools to adjust the line detection and show the steps/results.
 
         :param bands: Input bands dataframe or the address to its file.
         :type bands: pandas.Dataframe, str, pathlib.Path
 
-        :param cont_fit_degree: Continuum polynomial fitting degree.
-        :type cont_fit_degree: tuple, optional
-
-        :param cont_int_thres: Continuum maximum intensity threshold to include pixels.
-        :type cont_int_thres: tuple, optional
+        :param sigma_threshold: Continuum standard deviation factor for line detection. The default value is 3.
+        :type sigma_threshold: float, optional
 
-        :param noise_sigma_factor: Continuum standard deviation factor for line detection. The default value is 3.
-        :type noise_sigma_factor: float, optional
-
-        :param line_type: Line type. The default value is "emission".
-        :type line_type: str, optional
+        :param emission_type: Line type. The default value is "True" for emission lines.
+        :type emission_type: str, optional
 
         :param width_tol: Minimum number of pixels between peaks/troughs. The default value is 5.
         :type width_tol: float, optional
 
         :param band_modification: Method to adjust the line band with. The default value is None.
         :type band_modification: str, optional
 
         :param ml_detection: Machine learning algorithm to detect lines. The default value is None.
         :type ml_detection: str, optional
 
-        :param plot_cont_calc: Plot the continuum fit at each iteration. The default value is False
-        :type plot_cont_calc: bool, optional
-
-        :param plot_peak_calc: Plot the detected peaks/troughs. The default value is False
-        :type plot_peak_calc: bool, optional
+        :param plot_steps: Plot the detected peaks/troughs. The default value is False
+        :type plot_steps: bool, optional
 
         """
 
-        # TODO input log should not be None... Maybe read database
-
-        # Fit the continuum
-        cont_flux, cond_Std = self.continuum_fitting(degree_list=cont_fit_degree, threshold_list=cont_int_thres,
-                                                     return_std=True, plot_results=plot_cont_calc)
-
-        # Check via machine learning algorithm
-        if ml_detection is not None:
-            if joblib_check:
-                self.ml_model = joblib.load(MACHINE_PATH)
-                ml_mask = self.ml_line_detection(cont_flux) if ml_detection else None
-            else:
-                raise ImportError(f'Need to install joblib library to use machine learning detection')
-        else:
-            ml_mask = None
-
         # Check for the peaks of the emission lines
-        detec_min = noise_sigma_factor * cond_Std
-        idcs_peaks = self.peak_detection(detec_min, cont_flux, plot_results=plot_peak_calc, ml_mask=ml_mask)
-
-        # Compare against the theoretical values
-        bands = check_file_dataframe(bands, pd.DataFrame)
-        if bands is not None:
+        continuum_array = self.cont if continuum_array is None else continuum_array
+        continuum_std = self.cont_std if continuum_std is None else continuum_std
 
-            # Match peaks with theoretical lines
-            matched_DF = self.label_peaks(idcs_peaks, bands, width_tol=width_tol, band_modification=band_modification,
-                                          line_type=line_type)
+        # Get indeces of peaks
+        limit_threshold = sigma_threshold * continuum_std
+        limit_threshold = continuum_array + limit_threshold if emission_type else continuum_array + limit_threshold
+        idcs_peaks, _ = signal.find_peaks(self.flux, height=limit_threshold, distance=width_tol)
 
-            return matched_DF
+        # Match peaks with theoretical lines
+        bands = check_file_dataframe(bands, pd.DataFrame)
+        matched_DF = self.label_peaks(idcs_peaks, bands, width_tol=width_tol, band_modification=band_modification,
+                                      line_type=emission_type)
 
-        else:
+        # Plot the results
+        if plot_steps:
+            self.plot._plot_peak_detection(idcs_peaks, limit_threshold, continuum_array, matched_DF)
 
-            return
+        return matched_DF
 
+    #
     def label_peaks(self, peak_table, mask_df, line_type='emission', width_tol=5, band_modification=None, detect_check=False):
 
         # TODO auto param should be changed to boolean
         # Establish the type of input values for the peak indexes, first numpy array
         if isinstance(peak_table, np.ndarray):
             idcsLinePeak = peak_table
 
         # Specutils table
         else:
             # Query the lines from the astropy finder tables #
             if len(peak_table) != 0:
-                idcsLineType = peak_table['line_type'] == line_type
+                idcsLineType = peak_table['emission_type'] == line_type
                 idcsLinePeak = np.array(peak_table[idcsLineType]['line_center_index'])
             else:
                 idcsLinePeak = np.array([])
 
         # Security check in case no lines detected
         if len(idcsLinePeak) == 0:
             return pd.DataFrame(columns=mask_df.columns)
@@ -297,26 +318,14 @@
         tolerance = np.diff(self.wave_rest).mean() * width_tol
         matched_DF['observation'] = 'not_detected'
         unidentifiedLine = dict.fromkeys(matched_DF.columns.values, np.nan)
 
         # Get the wavelength peaks
         wave_peaks = self.wave_rest[idcsLinePeak]
 
-        # from matplotlib import pyplot as plt
-        # fig, ax = plt.subplots()
-        # ax.step(self.wave_rest, self.flux, where='mid')
-        # ax.scatter(self.wave_rest[idcsLinePeak], self.flux[idcsLinePeak])
-        # plt.show()
-        # np.ma.isMaskedArray(wave_peaks)
-
-        # # Only treat pixels outisde the masks
-        # if np.ma.is_masked(wave_peaks):
-        #     idcsLinePeak = idcsLinePeak[~wave_peaks.mask]
-        #     wave_peaks = wave_peaks[~wave_peaks.mask].data
-
         for i in np.arange(wave_peaks.size):
 
             idx_array = np.where(np.isclose(a=waveTheory.astype(np.float64), b=wave_peaks[i], atol=tolerance))
 
             if len(idx_array[0]) == 0:
                 unknownLineLabel = 'xy_{:.0f}A'.format(np.round(wave_peaks[i]))
 
@@ -354,69 +363,154 @@
         # Sort by wavelength
         matched_DF.sort_values('wavelength', inplace=True)
         matched_DF.drop(columns=['wavelength', 'observation'], inplace=True)
 
         return matched_DF
 
 
+class FeatureClassifier:
+
+    def __init__(self, data_array, box_width, model, n_pixels):
+
+        # Attributes
+        self.pred_matrix = None
+        self.confidence = None
+        self.n_pixels = n_pixels
+
+        # Recover the models linear coefficients:
+        w, b = np.squeeze(model.coef_), np.squeeze(model.intercept_)
+
+        # Compute the prediction
+        self.pred_matrix = np.tensordot(data_array, w, axes=([1], [0])) + b
+        self.pred_matrix = self.pred_matrix > 0
+
+        # # Propagate the true detections for the box window # Convolution
+        # kernel = np.r_[np.zeros(box_width - 1), np.ones(box_width)][None]
+        # column_kernel = kernel.reshape(-1, 1)
+        # self.pred_matrix = signal.convolve2d(self.pred_matrix, column_kernel, mode='same').astype(bool)
+
+        # Propagate the true detections for the box window
+        self.pred_matrix = np.apply_along_axis(prop_func, 0, self.pred_matrix, box_width)
+
+        # Confidence array from Montecarlo
+        self.confidence = self.pred_matrix.sum(axis=1)
+
+        return
+
+    def __call__(self, confidence=None, entry=None, confidence_max=100):
+
+        mask = np.zeros(self.n_pixels).astype(bool)
+
+        if confidence is not None:
+
+            if (confidence < 0) or (confidence > 100):
+                raise LiMe_Error(f'Please define the detection confidence in an [0, 100] interval. '
+                                 f'The input value was "{confidence}".')
+            else:
+
+                mask[:self.confidence.shape[0]] = (self.confidence >= confidence) & (confidence_max >= self.confidence)
+
+        elif entry is not None:
+
+            if (entry < 0) or (entry > 100):
+                raise LiMe_Error(f'Please define the Monte Carlo entry in the [0, 100] interval. '
+                                 f'The input value was "{entry}".')
+
+            mask[:self.pred_matrix.shape[0]] = self.pred_matrix[:, entry]
+
+        else:
+            raise LiMe_Error(f'Please define a confidence interval or an Monte Carlo for the bands detection mask')
+
+        return mask
+
+
 class DetectionInference:
 
     def __init__(self, spectrum):
 
         self._spec = spectrum
         self.narrow_detect = None
+        self.box_width = None
+        self.range_box = None
+        self.n_mc = 100
+
+        self.line_1d_pred = None
+        self.line_2d_pred = None
+        self.line_pred = None
 
         return
 
-    def bands(self, box_width, approximation=None, scale_type='min-max', machine_path=None, log_base=10000):
+    def bands(self, box_width, approximation=None, scale_type='min-max', log_base=10000, model_1d_path=None,
+              model_2d_path=None):
 
         # Assign default values
+        self.box_width, self.range_box = box_width, np.arange(box_width)
         approximation = FLUX_PIXEL_CONV if approximation is None else approximation
-        machine_path = MACHINE_PATH if machine_path is None else machine_path
 
-        # Load the model
-        model = joblib.load(machine_path)
-        model_dim = model.n_features_in_
+        # Load the models
+        model1D = joblib.load(model_1d_path)
+        model2D = joblib.load(model_2d_path)
 
-        # Recover the flux (without mask?)
-        input_flux = self._spec.flux if not np.ma.is_masked(self._spec.flux) else self._spec.flux.data
+        # Reshape to the detection interval (n x box_size) matrix
+        input_flux = enbox_spectrum(self._spec.flux, self.box_width, self.range_box)
 
-        # Reshape to the detection interval
-        range_box = np.arange(box_width)
-        n_intervals = input_flux.size - box_width + 1
-        input_flux = input_flux[np.arange(n_intervals)[:, None] + range_box]
+        # Add random noise for Monte Carlo
+        input_flux = self.monte_carlo_expansion(input_flux)
 
-        # Remove nan entries
-        idcs_nan_rows = np.isnan(input_flux).any(axis=1)
-        input_flux = input_flux[~idcs_nan_rows, :]
+        # Normalize the flux
+        input_flux = feature_scaling(input_flux, transformation=scale_type, log_base=log_base)
 
-        # Add Monte Carlo columns (7858, 13) To (7858, 13, 100)
+        # Reshape for detection types
+        input_flux_2D = flux_to_image(input_flux, approximation, model2D)
 
+        # Perform and store the detections
+        self.feature_detection(input_flux, input_flux_2D, model1D, model2D, self._spec.flux.size)
 
-        # Normalize the flux
-        input_flux = feature_scaling(input_flux, transformation=scale_type, log_base=log_base)
+        return
 
-        # Perform the 1D detection
-        if box_width == model_dim:
-            detection_array = model.predict(input_flux)
+    def monte_carlo_expansion(self, flux_array, noise_scale=None):
+
+        # Get the noise scale for the selections
+        if noise_scale is None:
+            noise_scale = self._spec.err_flux if self._spec.err_flux is not None else self._spec.cont_std
+
+            if noise_scale is None:
+                _logger.warning(f"No flux uncertainty provided for the line detection. There won't be a confidence value"
+                                f" for the predictions.")
+                self.n_mc = 1
+
+        # Single flux uncertainty
+        noise_matrix_shape = (flux_array.shape[0], flux_array.shape[1], self.n_mc)
+        if isinstance(noise_scale, float):
+            noise_array = np.random.normal(0, noise_scale, size=noise_matrix_shape)
+
+        # Array of flux uncertainty
         else:
-            array_2D = np.tile(input_flux[:, None, :], (1, approximation.size, 1))
-            array_2D = array_2D > approximation[::-1, None]
-            array_2D = array_2D.astype(int)
-            array_2D = array_2D.reshape((input_flux.shape[0], 1, -1))
-            array_2D = array_2D.squeeze()
-            detection_array = model.predict(array_2D)
-
-        # Reshape array original shape and add with of positive entries # TODO this shape could cause issues with IFUs
-        mask = np.zeros(self._spec.flux.shape, dtype=bool)
-        idcs_detect = np.argwhere(detection_array) + range_box
-        idcs_detect = idcs_detect.flatten()
-        idcs_detect = idcs_detect[idcs_detect < detection_array.size]
-        mask[idcs_detect] = True
+            # Rescale to the box format
+            input_err = enbox_spectrum(noise_scale, self.box_width, self.range_box)
+            noise_array = np.random.normal(0, input_err[..., None], size=noise_matrix_shape)
 
-        return mask
+        # Add the noise
+        flux_array = flux_array[:, :, np.newaxis] + noise_array
+
+        # flux_0 = flux_array * 1
+        # fluxMC_0 = flux_mc[:, :, 0]
+        # noise_0 = noise_array[:, :, 0]
+        # np.all(np.isclose(fluxMC_0 - noise_0, flux_0, atol=0.0000000000001))
+
+        return flux_array
+
+    def feature_detection(self, flux_array_1d, flux_array_2d, model_1d, model_2d, n_pixels):
+
+        # Perform the line 1D detection
+        self.line_1d_pred = FeatureClassifier(flux_array_1d, self.box_width, model_1d, n_pixels)
+
+        # Perform the line 2d detection
+        self.line_2d_pred = FeatureClassifier(flux_array_2d, self.box_width, model_2d, n_pixels)
+
+        return
 
 
 # Line finder default parameters
 LINE_DETECT_PARAMS = signature(LineFinder.line_detection).parameters
 LINE_DETECT_PARAMS = {key: value.default for key, value in LINE_DETECT_PARAMS.items()}
 LINE_DETECT_PARAMS.pop('self')
```

### Comparing `lime-stable-0.9.99.5/src/lime/resources/parent_bands.txt` & `lime-stable-1.0.0/src/lime/resources/parent_bands_BackUp.txt`

 * *Files identical despite different names*

### Comparing `lime-stable-0.9.99.5/src/lime/resources/types_params.txt` & `lime-stable-1.0.0/src/lime/resources/types_params.txt`

 * *Files 6% similar despite different names*

```diff
@@ -70,8 +70,10 @@
 redchi                     0               1                   1          0           1    <f8      $\chi_{\nu}^{2}$       none
 aic                        0               1                   1          0           1    <f8                   AIC       none
 bic                        0               1                   1          0           1    <f8                   BIC       none
 observations               0               1                   0          0           1   <U50          Observations        str
 comments                   0               1                   0          0           1   <U50              Comments        str
 wave_vac                   0               0                   0          1           0    <f8       $\lambda_{vac}$       wave
 transition                 0               0                   0          1           0    <U5  Transition-component        str
-rel_int                    0               0                   0          1           0    <f8           $Int_{rel}$       none
+rel_int                    0               0                   0          1           0    <f8           $Int_{rel}$       none
+units_wave                 0               0                   0          1           0   <U50         $units\,wave$       none
+units_flux                 0               0                   0          1           0   <U50         $units\,wave$       none
```

### Comparing `lime-stable-0.9.99.5/src/lime/tables.py` & `lime-stable-1.0.0/src/lime/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 from functools import partial
 from collections.abc import Sequence
-from . import __version__
 
 try:
     import pylatex
     pylatex_check = True
 except ImportError:
     pylatex_check = False
```

### Comparing `lime-stable-0.9.99.5/src/lime/tools.py` & `lime-stable-1.0.0/src/lime/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,31 +20,37 @@
 _logger = logging.getLogger('LiMe')
 
 # Arrays for roman numerals conversion
 VAL_LIST = [1000, 900, 500, 400, 100, 90, 50, 40, 10, 9, 5, 4, 1]
 SYB_LIST = ["M", "CM", "D", "CD", "C", "XC", "L", "XL", "X", "IX", "V", "IV", "I"]
 
 
-flam = au.def_unit(['flam', 'FLAM'], au.erg/au.s/au.cm**2/au.AA,
-                    format={"latex": r"erg\,cm^{-2}s^{-1}\AA^{-1}",
-                            "generic": "FLAM", "console": "FLAM"})
-
-fnu = au.def_unit(['fnu', 'FNU'], au.erg/au.s/au.cm**2/au.Hz,
-                    format={"latex": r"erg\,cm^{-2}s^{-1}Hz^{-1}",
-                            "generic": "FNU", "console": "FNU"})
-
-photlam = au.def_unit(['photlam', 'PHOTLAM'], au.photon/au.s/au.cm**2/au.AA,
-                        format={"latex": r"photon\,cm^{-2}s^{-1}\AA^{-1}",
-                        "generic": "PHOTLAM", "console": "PHOTLAM"})
-
-photnu = au.def_unit(['photnu', 'PHOTNU'], au.photon/au.s/au.cm**2/au.Hz,
-                        format={"latex": r"photon\,cm^{-2}s^{-1}Hz^{-1}",
-                        "generic": "PHOTNU", "console": "PHOTNU"})
-
-au.add_enabled_units([flam, fnu, photlam, photnu])
+dict_units = {'flam': au.erg/au.s/au.cm**2/au.AA, 'FLAM': au.erg/au.s/au.cm**2/au.AA,
+              'fnu': au.erg/au.s/au.cm**2/au.Hz, 'FNU': au.erg/au.s/au.cm**2/au.Hz,
+              'photlam': au.photon/au.s/au.cm**2/au.AA, 'PHOTLAM': au.photon/au.s/au.cm**2/au.AA,
+              'photnu': au.photon/au.s/au.cm**2/au.Hz, 'PHOTNU': au.photon/au.s/au.cm**2/au.Hz}
+au.set_enabled_aliases(dict_units)
+
+# flam = au.def_unit(['flam', 'FLAM'], au.erg/au.s/au.cm**2/au.AA,
+#                     format={"latex": r"erg\,cm^{-2}s^{-1}\AA^{-1}",
+#                             "generic": "FLAM", "console": "FLAM"})
+#
+# fnu = au.def_unit(['fnu', 'FNU'], au.erg/au.s/au.cm**2/au.Hz,
+#                     format={"latex": r"erg\,cm^{-2}s^{-1}Hz^{-1}",
+#                             "generic": "FNU", "console": "FNU"})
+#
+# photlam = au.def_unit(['photlam', 'PHOTLAM'], au.photon/au.s/au.cm**2/au.AA,
+#                         format={"latex": r"photon\,cm^{-2}s^{-1}\AA^{-1}",
+#                         "generic": "PHOTLAM", "console": "PHOTLAM"})
+#
+# photnu = au.def_unit(['photnu', 'PHOTNU'], au.photon/au.s/au.cm**2/au.Hz,
+#                         format={"latex": r"photon\,cm^{-2}s^{-1}Hz^{-1}",
+#                         "generic": "PHOTNU", "console": "PHOTNU"})
+#
+# au.add_enabled_units([flam, fnu, photlam, photnu])
 
 
 PARAMETER_LATEX_DICT = {'Flam': r'$F_{\lambda}$',
                         'Fnu': r'$F_{\nu}$',
                         'SN_line': r'$\frac{S}{N}_{line}$',
                         'SN_cont': r'$\frac{S}{N}_{cont}$'}
 
@@ -76,14 +82,15 @@
 
     # Transform the value from the dataframe to the default if requested
     if transform is not None:
         cell = default if cell == transform else cell
 
     return cell
 
+
 # Favoured method to get line fluxes according to resolution
 def extract_fluxes(log, flux_type='mixture', sample_level='line', column_name='line_flux', column_positions=None):
 
     if flux_type not in ('mixture', 'intg', 'profile'):
         raise LiMe_Error(f'Flux type "{flux_type}" is not recognized please one of "intg", "profile", or "mixture" ')
 
     # Get indeces of blended lines
@@ -91,15 +98,15 @@
         idcs_blended = (log['group_label'] != 'none') & (~log.index.str.endswith('_m'))
     else:
         if sample_level not in log.index.names:
             raise LiMe_Error(f'Input log does not have a index level with column "{sample_level}"')
 
         idcs_blended = (log['group_label'] != 'none') & (~log.index.get_level_values('line').str.endswith('_m'))
 
-    # Mixture model: Integrated fluxes for all lines except blended
+    # Mixture models: Integrated fluxes for all lines except blended
     if flux_type == 'mixture' and np.any(idcs_blended):
         obsFlux = log['intg_flux'].to_numpy(copy=True)
         obsErr = log['intg_flux_err'].to_numpy(copy=True)
         obsFlux[idcs_blended.values] = log.loc[idcs_blended.values, 'profile_flux'].to_numpy(copy=True)
         obsErr[idcs_blended.values] = log.loc[idcs_blended.values, 'profile_flux_err'].to_numpy(copy=True)
 
     # Use the one requested by the user
@@ -201,71 +208,71 @@
     # Add new columns if necessary
     if column_name not in log.columns:
         log.insert(loc=column_position, column=f'{column_name}', value=np.nan)
         log.insert(loc=column_position+1, column=f'{column_name}_err', value=np.nan)
 
     # Add new line with normalization by default
     if column_normalization_name not in log.columns:
-        log.insert(loc=column_position+2, column=column_normalization_name, value=np.nan)
+        log.insert(loc=column_position+2, column=column_normalization_name, value='none')
 
     # Loop throught the lines to compute their normalization
     single_index = not isinstance(log.index, pd.MultiIndex)
     for i in np.arange(len(line_array)):
 
-            numer, denom = line_array[i], norm_array[i]
-            numer_flux, denom_flux = None, None
+        numer, denom = line_array[i], norm_array[i]
+        numer_flux, denom_flux = None, None
 
-            # Single-index dataframe
-            if single_index:
-                idcs_ratios = numer
-                if (numer in log.index) and (denom in log.index):
-                    numer_flux = log.loc[numer, flux_column]
-                    numer_err = log.loc[numer, f'{flux_column}_err']
+        # Single-index dataframe
+        if single_index:
+            idcs_ratios = numer
+            if (numer in log.index) and (denom in log.index):
+                numer_flux = log.loc[numer, flux_column]
+                numer_err = log.loc[numer, f'{flux_column}_err']
 
-                    denom_flux = log.loc[denom, flux_column]
-                    denom_err = log.loc[denom, f'{flux_column}_err']
+                denom_flux = log.loc[denom, flux_column]
+                denom_err = log.loc[denom, f'{flux_column}_err']
 
-            #Multi-index dataframe
-            else:
+        #Multi-index dataframe
+        else:
 
-                if numer == denom:  # Same line normalization
-                    idcs_slice = log.index.get_level_values(sample_levels[-1]) == numer
-                    df_slice = log.loc[idcs_slice]
-                else:  # Rest cases
-                    idcs_slice = log.index.get_level_values(sample_levels[-1]).isin([numer, denom])
-                    grouper = log.index.droplevel('line')
-                    idcs_slice = pd.Series(idcs_slice).groupby(grouper).transform('sum').ge(2).array
-                    df_slice = log.loc[idcs_slice]
-
-                # Get fluxes
-                if df_slice.size > 0:
-                    num_slice = df_slice.xs(numer, level=sample_levels[-1], drop_level=False)
-                    numer_flux = num_slice[flux_column].to_numpy()
-                    numer_err = num_slice[f'{flux_column}_err'].to_numpy()
-
-                    denom_slice = df_slice.xs(denom, level=sample_levels[-1], drop_level=False)
-                    denom_flux = denom_slice[flux_column].to_numpy()
-                    denom_err = denom_slice[f'{flux_column}_err'].to_numpy()
-
-                    idcs_ratios = num_slice.index
-
-            # Compute the ratios with error propagation
-            ratio_array, ratio_err = None, None
-            if (numer_flux is not None) and (denom_flux is not None):
-                ratio_array = numer_flux / denom_flux
-                ratio_err = ratio_array * np.sqrt(np.power(numer_err / numer_flux, 2) + np.power(denom_err / denom_flux, 2))
-
-            # Store in dataframe (with empty columns)
-            if (ratio_array is not None) and (ratio_err is not None):
-                log.loc[idcs_ratios, f'{column_name}'] = ratio_array
-                log.loc[idcs_ratios, f'{column_name}_err'] = ratio_err
-
-                # Store normalization line
-                if column_normalization_name is not None:
-                    log.loc[idcs_ratios, f'{column_normalization_name}'] = denom
+            if numer == denom:  # Same line normalization
+                idcs_slice = log.index.get_level_values(sample_levels[-1]) == numer
+                df_slice = log.loc[idcs_slice]
+            else:  # Rest cases
+                idcs_slice = log.index.get_level_values(sample_levels[-1]).isin([numer, denom])
+                grouper = log.index.droplevel('line')
+                idcs_slice = pd.Series(idcs_slice).groupby(grouper).transform('sum').ge(2).array
+                df_slice = log.loc[idcs_slice]
+
+            # Get fluxes
+            if df_slice.size > 0:
+                num_slice = df_slice.xs(numer, level=sample_levels[-1], drop_level=False)
+                numer_flux = num_slice[flux_column].to_numpy()
+                numer_err = num_slice[f'{flux_column}_err'].to_numpy()
+
+                denom_slice = df_slice.xs(denom, level=sample_levels[-1], drop_level=False)
+                denom_flux = denom_slice[flux_column].to_numpy()
+                denom_err = denom_slice[f'{flux_column}_err'].to_numpy()
+
+                idcs_ratios = num_slice.index
+
+        # Compute the ratios with error propagation
+        ratio_array, ratio_err = None, None
+        if (numer_flux is not None) and (denom_flux is not None):
+            ratio_array = numer_flux / denom_flux
+            ratio_err = ratio_array * np.sqrt(np.power(numer_err / numer_flux, 2) + np.power(denom_err / denom_flux, 2))
+
+        # Store in dataframe (with empty columns)
+        if (ratio_array is not None) and (ratio_err is not None):
+            log.loc[idcs_ratios, f'{column_name}'] = ratio_array
+            log.loc[idcs_ratios, f'{column_name}_err'] = ratio_err
+
+            # Store normalization line
+            if column_normalization_name is not None:
+                log.loc[idcs_ratios, f'{column_normalization_name}'] = denom
 
     return
 
 
 # Get Weighted redshift from lines
 def redshift_calculation(input_log, line_list=None, weight_parameter=None, obj_label='spec_0'):
 
@@ -342,88 +349,14 @@
 
         # Add to dataframe
         z_df.loc[idx, 'z_mean':'weight'] = z_mean, z_std, obsLineList, weight_parameter
 
     return z_df
 
 
-# def compute_line_ratios(log, line_ratios=None, flux_columns=['intg_flux', 'intg_flux_err'], sample_levels=['id', 'line'],
-#                         object_id='obj_0', keep_empty_columns=True):
-#
-#     # If normalization_line is not none
-#     if len(flux_columns) != np.sum(log.columns.isin(flux_columns)):
-#         raise LiMe_Error(f'Input log is missing {len(flux_columns)} "flux_entries" in the column headers')
-#
-#     # Check if single or multi-index
-#     sample_check = isinstance(log.index, pd.MultiIndex)
-#
-#     if sample_check:
-#         idcs = log.index.droplevel(sample_levels[-1]).unique()
-#     else:
-#         idcs = np.array([object_id])
-#
-#     ratio_df = pd.DataFrame(index=idcs)
-#
-#     # Loop through
-#     if line_ratios is not None:
-#
-#         # Loop through the ratios
-#         for ratio_str in line_ratios:
-#             numer, denom = ratio_str.split('/')
-#
-#             # Slice the dataframe to objects having both lines
-#             numer_flux, denom_flux = None, None
-#             if not isinstance(log.index, pd.MultiIndex):
-#                 if (numer in log.index) and (denom in log.index):
-#                     numer_flux = log.loc[numer, flux_columns[0]]
-#                     numer_err = log.loc[numer, flux_columns[1]]
-#
-#                     denom_flux = log.loc[denom, flux_columns[0]]
-#                     denom_err = log.loc[denom, flux_columns[1]]
-#                     idcs_slice = object_id
-#                 else:
-#                     idcs_slice = ratio_df.index
-#
-#             else:
-#
-#                 # Slice the dataframe to objects which have both lines
-#                 idcs_slice = log.index.get_level_values(sample_levels[-1]).isin([numer, denom])
-#                 grouper = log.index.droplevel('line')
-#                 idcs_slice = pd.Series(idcs_slice).groupby(grouper).transform('sum').ge(2).array
-#                 df_slice = log.loc[idcs_slice]
-#
-#                 # Get fluxes
-#                 if df_slice.size > 0:
-#                     numer_flux = df_slice.xs(numer, level=sample_levels[-1])[flux_columns[0]]
-#                     numer_err = df_slice.xs(numer, level=sample_levels[-1])[flux_columns[1]]
-#
-#                     denom_flux = df_slice.xs(denom, level=sample_levels[-1])[flux_columns[0]]
-#                     denom_err = df_slice.xs(denom, level=sample_levels[-1])[flux_columns[1]]
-#                     idcs_slice = numer_flux.index
-#                 else:
-#                     idcs_slice = ratio_df.index
-#
-#             # Check there have been measure
-#             if (numer_flux is not None) and (denom_flux is not None):
-#
-#                 # Compute the ratios with the error propagation
-#                 ratio_array = numer_flux/denom_flux
-#                 errRatio_array = ratio_array * np.sqrt(np.power(numer_err/numer_flux, 2) +
-#                                                        np.power(denom_err/denom_flux, 2))
-#             else:
-#                 ratio_array, errRatio_array = np.nan, np.nan
-#
-#             # Store in dataframe (with empty columns)
-#             if not ((numer_flux is None) and (denom_flux is None) and (keep_empty_columns is False)):
-#                 ratio_df.loc[idcs_slice, ratio_str] = ratio_array
-#                 ratio_df.loc[idcs_slice, f'{ratio_str}_err'] = errRatio_array
-#
-#     return ratio_df
-
-
 def compute_FWHM0(idx_peak, spec_flux, delta_wave, cont_flux, emission_check=True):
 
     """
 
     :param idx_peak:
     :param spec_flux:
     :param delta_wave:
@@ -559,22 +492,29 @@
             formatted_value[i] = [element-pix_width, element+pix_width]
 
     formatted_value = np.array(formatted_value).astype(float)
 
     return formatted_value
 
 
-def define_masks(wavelength_array, masks_array, merge_continua=True, line_mask_entry='no'):
+def define_masks(wavelength_array, masks_array, merge_continua=True, line_mask_entry='no', line=None):
 
     # Make sure it is a matrix
     # TODO warning for mask outside limimes
-    masks_array = np.array(masks_array, ndmin=2)
+    # masks_array = np.array(masks_array, ndmin=2)
+    masks_array = np.atleast_2d(masks_array)
+
+    if np.any(masks_array[:, 0] < wavelength_array[0]) or np.any(masks_array[:, 5] > wavelength_array[-1]):
+        warn_message = ('below', wavelength_array[:, 0] if np.any(masks_array[:, 0] < wavelength_array[0]) else
+                        'above', masks_array[:, 5])
+        _logger.warning(f'Bands for {line} are {warn_message[0]} the wavelength range {warn_message[1]}.')
+
 
     # Check if it is a masked array
-    if np.ma.is_masked(wavelength_array):
+    if np.ma.isMaskedArray(wavelength_array):
         wave_arr = wavelength_array.data
     else:
         wave_arr = wavelength_array
 
     # Remove masked pixels from this function wavelength array
     if line_mask_entry != 'no':
 
@@ -592,32 +532,32 @@
     idcsW = np.searchsorted(wave_arr, masks_array)
 
     # Emission region
     idcsLineRegion = ((wave_arr[idcsW[:, 2]] <= wave_arr[:, None]) & (wave_arr[:, None] <= wave_arr[idcsW[:, 3]]) & idcsValid).squeeze()
     
     # Return left and right continua merged in one array
     if merge_continua:
-
         idcsContRegion = (((wave_arr[idcsW[:, 0]] <= wave_arr[:, None]) &
                           (wave_arr[:, None] <= wave_arr[idcsW[:, 1]])) |
                           ((wave_arr[idcsW[:, 4]] <= wave_arr[:, None]) & (
                            wave_arr[:, None] <= wave_arr[idcsW[:, 5]])) & idcsValid).squeeze()
 
-        return idcsLineRegion, idcsContRegion
+        outputs = idcsLineRegion, idcsContRegion
 
     # Return left and right continua in separated arrays
     else:
-
         idcsContLeft = ((wave_arr[idcsW[:, 0]] <= wave_arr[:, None]) & (wave_arr[:, None] <= wave_arr[idcsW[:, 1]]) & idcsValid).squeeze()
         idcsContRight = ((wave_arr[idcsW[:, 4]] <= wave_arr[:, None]) & (wave_arr[:, None] <= wave_arr[idcsW[:, 5]]) & idcsValid).squeeze()
 
-        return idcsLineRegion, idcsContLeft, idcsContRight
+        outputs = idcsLineRegion, idcsContLeft, idcsContRight
+
+    return outputs
 
 
-def logs_into_fits(log_file_list, output_address, delete_after_join=False, levels=['id', 'line']):
+def join_fits_files(log_file_list, output_address, delete_after_join=False, levels=['id', 'line']):
 
     """
     This functions combines multiple log files into single *.fits* file. The user can request to the delete the individual
     logs after the individual logs have been combined.
 
     If the case of individual *.fits* the function loop through the individual HDU and add them to the output file. Currently,
     this is not available to other multi-page files (such as .xlsx or .asdf)
```

### Comparing `lime-stable-0.9.99.5/src/lime/transitions.py` & `lime-stable-1.0.0/src/lime/transitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -447,34 +447,56 @@
     _p_shape_list, _p_type_list = np.array(_p_shape_list), np.array(_p_type_list)
 
     return _p_shape_list, _p_type_list
 
 
 def label_mask_assigning(line_label, input_band, blend_check, merged_check, core_comp):
 
-    # TODO what about a "core" label
-
     if isinstance(input_band, DataFrame):
 
-        # Query for the input label # TODO put a try with .at and the other in the except
-        if line_label in input_band.index:
-            mask = input_band.loc[line_label, 'w1':'w6'].to_numpy().astype(float)
-
-        # Remove blended/merged suffix to check
-        elif (blend_check or merged_check) and (line_label[:-2] in input_band.index):
-            mask = input_band.loc[line_label[:-2], 'w1':'w6'].to_numpy().astype(float)
+        # Query for input label
+        if pd_get(input_band, line_label, 'w1') is not None:
+            ref_label = line_label
+
+        # Blended or merged line
+        elif pd_get(input_band, line_label[:-2], 'w1') is not None:
+            ref_label = line_label[:-2]
 
         # Case where we introduce a line with a different profile (H1_4861A_l)
-        elif core_comp in input_band.index:
-            mask = input_band.loc[core_comp, 'w1':'w6'].to_numpy().astype(float)
+        elif pd_get(input_band, core_comp, 'w1') is not None:
+            ref_label = core_comp
+
+        # Not found
+        else:
+            ref_label = None
 
-        # Could not find the mask
+        # Recover the mask
+        if ref_label is not None:
+            mask = np.array([input_band.at[ref_label, 'w1'], input_band.at[ref_label, 'w2'],
+                             input_band.at[ref_label, 'w3'], input_band.at[ref_label, 'w4'],
+                             input_band.at[ref_label, 'w5'], input_band.at[ref_label, 'w6']])
         else:
             mask = None
 
+        # # Query for the input label # TODO put a try with .at and the other in the except
+        # if line_label in input_band.index:
+        #     mask = input_band.loc[line_label, 'w1':'w6'].to_numpy().astype(float)
+        #
+        # # Remove blended/merged suffix to check
+        # elif (blend_check or merged_check) and (line_label[:-2] in input_band.index):
+        #     mask = input_band.loc[line_label[:-2], 'w1':'w6'].to_numpy().astype(float)
+        #
+        # # Case where we introduce a line with a different profile (H1_4861A_l)
+        # elif core_comp in input_band.index:
+        #     mask = input_band.loc[core_comp, 'w1':'w6'].to_numpy().astype(float)
+        #
+        # # Could not find the mask
+        # else:
+        #     mask = None
+
     # No band
     elif input_band is None:
         mask = None
 
     # Convert input to numpy array
     else:
         mask = np.atleast_1d(input_band)
@@ -637,33 +659,46 @@
         self._review_latex_label(band)
 
         return
 
     @classmethod
     def from_log(cls, label, log=None, norm_flux=1):
 
-        # Create the line object
-        inline = cls(label, band=log)
+        # Confirm we are not introducing a blended line which has been blended
 
-        # TODO loop through the log columns and match with line
         if label in log.index:
+            measured_check = True
+        elif (label[-2:] == '_b') and (label[:-2] in log.index):
+            _logger.warning(f'Blended line {label} not found in log, reading {label[:-2]}')
+            label = label[:-2]
+            measured_check = True
+        else:
+            _logger.warning(f'Input line {label} not found in log')
+            measured_check = False
+
+        # Reload the line
+        if measured_check:
+
+            # Create the line object
+            inline = cls(label, band=log)
 
             # Recover "simple" attributes
             for i, param in enumerate(_LOG_EXPORT):
 
                 param_value = log.at[label, param]
 
                 # Normalize
                 if _LOG_COLUMNS[param][0]:
                     param_value = param_value / norm_flux
 
                 inline.__setattr__(param, param_value)
 
         else:
-            _logger.warning(f'Input line {inline.label} not found in log')
+
+            inline = None
 
         return inline
 
     def _modularity_component(self, modularity_label, fit_conf=None, bands_log=None):
 
         # Not a single line
         if modularity_label is not None:
```

### Comparing `lime-stable-0.9.99.5/src/lime/workflow.py` & `lime-stable-1.0.0/src/lime/workflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,51 +2,54 @@
 import numpy as np
 import pandas as pd
 from pathlib import Path
 from astropy.io import fits
 from time import time
 
 from .model import LineFitting, signal_to_noise_rola
-from .tools import define_masks, ProgressBar, logs_into_fits, extract_wcs_header, pd_get
+from .tools import define_masks, ProgressBar, join_fits_files, extract_wcs_header, pd_get
 from .transitions import Line
 from .io import check_file_dataframe, check_file_array_mask, log_to_HDU, results_to_log, load_frame, LiMe_Error, check_fit_conf
 from lmfit.models import PolynomialModel
 
 _logger = logging.getLogger('LiMe')
 
 
-def review_bands(line, emis_wave, cont_wave, limit_narrow=7):
+def review_bands(line, emis_wave, cont_wave, emis_flux, cont_flux, limit_narrow=7):
 
     # Review the transition bands before
-    emis_band_lengh = emis_wave.size if not np.ma.is_masked(emis_wave) else np.sum(~emis_wave.mask)
-    cont_band_length = cont_wave.size if not np.ma.is_masked(cont_wave) else np.sum(~cont_wave.mask)
+    emis_band_lengh = emis_wave.size if not np.ma.isMaskedArray(emis_wave) else np.sum(~emis_wave.mask)
+    cont_band_length = cont_wave.size if not np.ma.isMaskedArray(cont_wave) else np.sum(~cont_wave.mask)
+
+    proceed = True
 
     if emis_band_lengh / emis_wave.size < 0.5:
         _logger.warning(f'The line band for {line.label} has very few valid pixels')
 
     if cont_band_length / cont_wave.size < 0.5:
         if cont_band_length > 0:
             _logger.warning(f'The continuum band for {line.label} has very few valid pixels)')
         else:
-            _logger.warning(f'The continuum bands for {line.label} have 0 pixels. The continuum will be approximated')
+            _logger.warning(f"The continuum bands for {line.label} have 0 pixels. It won't be measured")
+            proceed = False
 
     # Store error very small mask
     if emis_band_lengh <= 1:
         if line.observations == 'no':
             line.observations = 'Small_line_band'
         else:
             line.observations += '-Small_line_band'
 
-        if np.ma.is_masked(emis_wave):
+        if np.ma.isMaskedArray(emis_wave):
             length = np.sum(~emis_wave.mask)
         else:
             length = emis_band_lengh
         _logger.warning(f'The  {line.label} band is too small ({length} length array): {emis_wave}')
 
-    return
+    return proceed
 
 
 def import_line_kinematics(line, z_cor, log, units_wave, fit_conf):
 
     # Check if imported kinematics come from blended component
     if line.group_label is not None:
         childs_list = line.group_label.split('+')
@@ -189,14 +192,31 @@
         measure_check = False if line in comp_list else True
     else:
         measure_check = True
 
     return measure_check
 
 
+def continuum_model_fit(x_array, y_array, idcs, degree):
+
+
+    poly3Mod = PolynomialModel(prefix=f'poly_{degree}', degree=degree)
+    poly3Params = poly3Mod.guess(y_array[idcs], x=x_array[idcs])
+
+    try:
+        poly3Out = poly3Mod.fit(y_array[idcs], poly3Params, x=x_array[idcs])
+        cont_fit = poly3Out.eval(x=x_array)
+
+    except TypeError:
+        _logger.warning(f'- The continuum fitting polynomial has more degrees ({degree}) than data points')
+        cont_fit = np.full(x_array.size, np.nan)
+
+    return cont_fit
+
+
 class SpecTreatment(LineFitting):
 
     def __init__(self, spectrum):
 
         # Instantiate the dependencies
         LineFitting.__init__(self)
 
@@ -281,49 +301,51 @@
         # Check if the line location is provided
         bands_integrity = check_spectrum_bands(self.line, self._spec.wave_rest)
 
         if bands_integrity:
 
             # Get the bands regions
             idcsEmis, idcsCont = define_masks(self._spec.wave, self.line.mask * (1 + self._spec.redshift),
-                                              line_mask_entry=self.line.pixel_mask)
+                                              line_mask_entry=self.line.pixel_mask, line=self.line.label)
 
             emisWave, emisFlux = self._spec.wave[idcsEmis], self._spec.flux[idcsEmis]
             emisErr = None if self._spec.err_flux is None else self._spec.err_flux[idcsEmis]
 
             contWave, contFlux = self._spec.wave[idcsCont], self._spec.flux[idcsCont]
             contErr = None if self._spec.err_flux is None else self._spec.err_flux[idcsCont]
 
             # Check the bands size
-            review_bands(self.line, emisWave, contWave)
+            proceed = review_bands(self.line, emisWave, contWave, emisFlux, contFlux)
 
-            # Default line type is in emission unless all are absorption
-            emission_check = False if np.all(~self.line._p_type) else True
+            if proceed:
 
-            # Non-parametric measurements
-            self.integrated_properties(self.line, emisWave, emisFlux, emisErr, contWave, contFlux, contErr, emission_check)
+                # Default line type is in emission unless all are absorption
+                emission_check = False if np.all(~self.line._p_type) else True
 
-            # Import kinematics if requested
-            import_line_kinematics(self.line, 1 + self._spec.redshift, self._spec.log, self._spec.units_wave, input_conf)
+                # Non-parametric measurements
+                self.integrated_properties(self.line, emisWave, emisFlux, emisErr, contWave, contFlux, contErr, emission_check)
 
-            # Combine bands
-            idcsLine = idcsEmis + idcsCont
-            x_array, y_array = self._spec.wave[idcsLine], self._spec.flux[idcsLine]
-            emisErr = None if self._spec.err_flux is None else self._spec.err_flux[idcsLine]
+                # Import kinematics if requested
+                import_line_kinematics(self.line, 1 + self._spec.redshift, self._spec.frame, self._spec.units_wave, input_conf)
 
-            # Gaussian fitting
-            self.profile_fitting(self.line, x_array, y_array, emisErr, self._spec.redshift, input_conf, min_method, temp,
-                                 self._spec.inst_FWHM)
+                # Combine bands
+                idcsLine = idcsEmis + idcsCont
+                x_array, y_array = self._spec.wave[idcsLine], self._spec.flux[idcsLine]
+                emisErr = None if self._spec.err_flux is None else self._spec.err_flux[idcsLine]
 
-            # Recalculate the SNR with the gaussian parameters
-            err_cont = self.line.cont_err if self._spec.err_flux is None else np.mean(self._spec.err_flux[idcsEmis])
-            self.line.snr_line = signal_to_noise_rola(self.line.amp, err_cont, self.line.n_pixels)
+                # Gaussian fitting
+                self.profile_fitting(self.line, x_array, y_array, emisErr, self._spec.redshift, input_conf, min_method, temp,
+                                     self._spec.inst_FWHM)
 
-            # Save the line parameters to the dataframe
-            results_to_log(self.line, self._spec.log, self._spec.norm_flux)
+                # Recalculate the SNR with the gaussian parameters
+                err_cont = self.line.cont_err if self._spec.err_flux is None else np.mean(self._spec.err_flux[idcsEmis])
+                self.line.snr_line = signal_to_noise_rola(self.line.amp, err_cont, self.line.n_pixels)
+
+                # Save the line parameters to the dataframe
+                results_to_log(self.line, self._spec.frame, self._spec.norm_flux)
 
         return
 
     def frame(self, bands, fit_conf=None, min_method='least_squares', profile='g-emi', cont_from_bands=True,
               temp=10000.0, line_list=None, default_conf_prefix='default', id_conf_prefix=None, line_detection=False,
               plot_fit=False, progress_output='bar'):
 
@@ -414,14 +436,17 @@
                 bands = bands.loc[idcs]
 
             # Load configuration
             input_conf = check_fit_conf(fit_conf, default_conf_prefix, id_conf_prefix)
 
             # Line detection if requested
             if line_detection:
+                cont_fit_conf = input_conf.get('continuum_fit', {})
+                self._spec.fit.continuum(**cont_fit_conf)
+
                 detect_conf = input_conf.get('line_detection', {})
                 bands = self._spec.line_detection(bands, **detect_conf)
 
             # Define lines to treat through the lines
             label_list = bands.index.to_numpy()
             self._n_lines = label_list.size
 
@@ -449,22 +474,22 @@
                                    id_conf_prefix=None, default_conf_prefix=None)
 
                         if plot_fit:
                             self._spec.plot.bands()
 
             else:
                 msg = f'No lines were measured from the input dataframe:\n - line_list: {line_list}\n - line_detection: {line_detection}'
-                _logger.info(msg)
+                _logger.debug(msg)
 
         else:
             _logger.info(f'Not input dataframe. Lines were not measured')
 
         return
 
-    def continuum(self, degree_list, threshold_list, smooth_length=None, plot_steps=False):
+    def continuum(self, degree_list, emis_threshold, abs_threshold=None, smooth_length=None, plot_steps=False):
 
         """
 
         This function fits the spectrum continuum in an iterative process. The user specifies two parameters: the ``degree_list``
         for the fitted polynomial and the ``threshold_list``` for the multiplicative standard deviation factor. At each
         interation points beyond this flux threshold are excluded from the continuum current fittings. Consequently,
         the user should aim towards more constrictive parameter values at each iteration.
@@ -473,75 +498,77 @@
         the ``smooth_length`` parameter.
 
         The user can visually inspect the fitting output graphically setting the parameter ``plot_steps=True``.
 
         :param degree_list: Integer list with the degree of the continuum polynomial
         :type degree_list: list
 
-        :param threshold_list: Float list for the multiplicative continuum standard deviation flux factor
-        :type threshold_list: list
+        :param emis_threshold: Float list for the multiplicative continuum standard deviation flux factor
+        :type emis_threshold: list
 
         :param smooth_length: Size of the smoothing window to convolve the spectrum. The default value is None.
         :type smooth_length: integer, optional
 
         :param plot_steps: Set to "True" to plot the fitted continuum at each iteration.
         :type plot_steps: bool, optional
 
         :return:
 
         """
 
-        # Check for a masked array
-        if np.ma.is_masked(self._spec.flux):
+        # Create a pre-Mask based on the original mask if available # TODO np.ma.is_masked es malo quitalo
+        if np.ma.isMaskedArray(self._spec.flux):
             mask_cont = ~self._spec.flux.mask
             input_wave, input_flux = self._spec.wave.data, self._spec.flux.data
         else:
             mask_cont = np.ones(self._spec.flux.size).astype(bool)
             input_wave, input_flux = self._spec.wave, self._spec.flux
 
         # Smooth the spectrum
         if smooth_length is not None:
-            # Compute the Gaussian kernel
             smoothing_window = np.ones(smooth_length) / smooth_length
-            input_flux = np.convolve(input_flux, smoothing_window, mode='same')
+            input_flux_s = np.convolve(input_flux, smoothing_window, mode='same')
+        else:
+            input_flux_s = input_flux
 
         # Loop through the fitting degree
+        abs_threshold = emis_threshold if abs_threshold is None else abs_threshold
         for i, degree in enumerate(degree_list):
 
+            # First iteration use percentile limits for an initial fit
+            if i == 0:
+                low_lim, high_lim = np.percentile(input_flux_s[mask_cont], (16, 84))
+                mask_cont_0 = mask_cont & (input_flux_s >= low_lim) & (input_flux_s <= high_lim)
+                cont_fit = continuum_model_fit(input_wave, input_flux_s, mask_cont_0, degree)
+
             # Establishing the flux limits
-            low_lim, high_lim = np.percentile(input_flux[mask_cont], (16, 84))
-            low_lim, high_lim = low_lim / threshold_list[i], high_lim * threshold_list[i]
+            std_flux = np.std((input_flux_s - cont_fit)[mask_cont])
+            low_lim, high_lim = cont_fit - abs_threshold[i] * std_flux, cont_fit + emis_threshold[i] * std_flux
 
             # Add new entries to the mask
-            mask_cont = mask_cont & (input_flux >= low_lim) & (input_flux <= high_lim)
+            mask_cont = mask_cont & (input_flux_s >= low_lim) & (input_flux_s <= high_lim)
 
-            poly3Mod = PolynomialModel(prefix=f'poly_{degree}', degree=degree)
-            poly3Params = poly3Mod.guess(input_flux[mask_cont], x=input_wave[mask_cont])
-
-            try:
-                poly3Out = poly3Mod.fit(input_flux[mask_cont], poly3Params, x=input_wave[mask_cont])
-                self._spec.cont = poly3Out.eval(x=input_wave)
-
-            except TypeError:
-                _logger.warning(f'- The continuum fitting polynomial has more degrees ({degree}) than data points')
-                self._spec.cont = np.full(input_wave.size, np.nan)
+            # Fit continuum
+            cont_fit = continuum_model_fit(input_wave, input_flux_s, mask_cont, degree)
 
             # Compute the continuum and assign replace the value outside the bands the new continuum
             if plot_steps:
-                title = f'Continuum fitting, iteration ({i+1}/{len(degree_list)})'
-                continuum_full = poly3Out.eval(x=self._spec.wave.data)
-                self._spec.plot._continuum_iteration(self._spec.wave, input_flux, continuum_full, mask_cont, low_lim,
-                                                     high_lim, threshold_list[i], title)
+                ax_cfg = {'title':f'Continuum fitting, iteration ({i+1}/{len(degree_list)})'}
+                self._spec.plot._continuum_iteration(input_wave, input_flux, cont_fit, input_flux_s, mask_cont, low_lim,
+                                                     high_lim, emis_threshold[i], ax_cfg)
 
         # Include the standard deviation of the spectrum for the unmasked pixels
-        self._spec.cont_std = np.std((self._spec.flux - self._spec.cont)[mask_cont])
+        self._spec.cont = cont_fit if not np.ma.isMaskedArray(self._spec.flux) else np.ma.masked_array(cont_fit,
+                                                                                                       self._spec.flux.mask)
+        self._spec.cont_std = np.std((input_flux_s - cont_fit)[mask_cont])
 
         return
 
 
+
 class CubeTreatment(LineFitting):
 
     def __init__(self, cube):
 
         # Instantiate the dependencies
         LineFitting.__init__(self)
 
@@ -578,15 +605,15 @@
             In this multi-level configuration design, the higher level entries **update** the lower level entries:
             only shared entries are overwritten, the final configuration will include all the entries from the
             default mask and spaxel sections.
 
         If the ``line_detection`` is set to True the function proceeds to run the line detection algorithm prior to the
         fitting of the lines. The user provide the configuration parameters for the line_detection function in the
         ``fit_conf`` argument. At the default, mask or spaxel configuration the user needs to specify these entries with
-        the "function name" + "." + "function argument" (i.e. "line_detection.line_type='emission'"). The multi-level
+        the "function name" + "." + "function argument" (i.e. "line_detection.emission_type='emission'"). The multi-level
         configuration described above will be applied to this function parameters as well.
 
         .. note::
             The parameters for the ``line.detection`` can be found on the documentation. The user doesn't need to specify
             a "lime_detection.bands" parameter. The input bands from the corresponding mask will be used.
 
         :param mask_file: Address of binary spatial mask file
@@ -689,15 +716,14 @@
 
             # Mask progress indexing
             mask_name = mask_list[i]
             mask_hdr = mask_data_list[i][1]
             idcs_spaxels = spaxels_dict[i]
 
             # Recover the fitting configuration
-            # mask_conf = recover_level_conf(fit_conf, default_conf_prefix, mask_name)
             mask_conf = check_fit_conf(input_conf, default_conf_prefix, mask_name)
 
             # Load the mask log if provided
             if bands is None:
                 bands_file = mask_conf['bands']
                 bands_path = Path(bands_file).absolute() if bands_file[0] == '.' else Path(bands_file)
                 bands_in = load_frame(bands_path)
@@ -712,15 +738,15 @@
             pbar = ProgressBar(progress_output, f'mask')
             for j in np.arange(n_spaxels):
 
                 idx_j, idx_i = idcs_spaxels[j]
                 spaxel_label = f'{idx_j}-{idx_i}'
 
                 # Get the spaxel fitting configuration
-                spaxel_conf = fit_conf.get(f'{spaxel_label}_line_fitting')
+                spaxel_conf = input_conf.get(f'{spaxel_label}_line_fitting')
                 spaxel_conf = mask_conf if spaxel_conf is None else {**mask_conf, **spaxel_conf}
 
                 # Spaxel progress message
                 pbar.output_message(j, n_spaxels, pre_text="", post_text=f'(spaxel coordinate. {idx_j}-{idx_i})')
 
                 # Get spaxel data
                 spaxel = self._cube.get_spectrum(idx_j, idx_i, spaxel_label)
@@ -728,15 +754,15 @@
                 # Fit the lines
                 spaxel.fit.frame(bands_in, spaxel_conf, line_list=line_list, min_method=min_method,
                                  line_detection=line_detection, profile=profile, cont_from_bands=cont_from_bands,
                                  temp=temp, progress_output=None, plot_fit=None, id_conf_prefix=None,
                                  default_conf_prefix=None)
 
                 # Count the number of measurements
-                n_lines += spaxel.log.index.size
+                n_lines += spaxel.frame.index.size
 
                 # Create page header with the default data
                 hdr_i = fits.Header()
 
                 # Add WCS information
                 if hdr_coords is not None:
                     hdr_i.update(hdr_coords)
@@ -744,15 +770,15 @@
                 # Add user information
                 if header is not None:
                     page_hdr = header.get(f'{spaxel_label}{log_ext_suffix}', None)
                     page_hdr = header if page_hdr is None else page_hdr
                     hdr_i.update(page_hdr)
 
                 # Save to a fits file
-                linesHDU = log_to_HDU(spaxel.log, ext_name=f'{spaxel_label}{log_ext_suffix}', header_dict=hdr_i)
+                linesHDU = log_to_HDU(spaxel.frame, ext_name=f'{spaxel_label}{log_ext_suffix}', header_dict=hdr_i)
 
                 if linesHDU is not None:
                     hdul_log.append(linesHDU)
 
                 # Plot the fittings if requested:
                 if plot_fit:
                     spaxel.plot.spectrum(include_fits=True, rest_frame=True)
@@ -762,21 +788,29 @@
             hdul_log.close()
 
             # Computation time and message
             end_time = time()
             elapsed_time = end_time - start_time
             print(f'\n{n_lines} lines measured in {elapsed_time/60:0.2f} minutes.')
 
-        if join_output_files: # TODO If only one mask and join_output_files the output file has different name
+        if join_output_files:
             output_comb_file = f'{address_dir/address_stem}.fits'
 
             # In case of only one file just rename it
             if len(mask_list) == 1:
                 mask_0_path = Path(mask_log_files_list[0])
                 mask_0_path.rename(Path(output_comb_file))
             else:
                 print(f'\nJoining spatial log files ({",".join(mask_list)}) -> {output_comb_file}')
-                logs_into_fits(mask_log_files_list, output_comb_file, delete_after_join=join_output_files)
+                join_fits_files(mask_log_files_list, output_comb_file, delete_after_join=join_output_files)
+
+        # else:
+        #     # Just one mask and Join is False
+        #     if len(mask_list) == 1:
+        #         output_comb_file = f'{address_dir / address_stem}.fits'
+        #         mask_0_path = Path(mask_log_files_list[0])
+        #         mask_0_path.rename(Path(output_comb_file))
+
 
         return
```

### Comparing `lime-stable-0.9.99.5/src/lime_stable.egg-info/PKG-INFO` & `lime-stable-1.0.0/src/lime_stable.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 Metadata-Version: 2.1
 Name: lime-stable
-Version: 0.9.99.5
+Version: 1.0.0
 Summary: Line measuring algorithm for astronomical spectra
 Home-page: https://github.com/Vital-Fernandez/lime
 Author: Vital Fernandez
 Author-email: Vital Fernández <vgf@umich.edu>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
-Requires-Dist: joblib==1.3.1
-Requires-Dist: lmfit==1.2.2
-Requires-Dist: matplotlib==3.7.2
-Requires-Dist: mplcursors==0.5.2
-Requires-Dist: nbsphinx==0.9.2
-Requires-Dist: numpy==1.24.4
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: pandas==2.0.3
-Requires-Dist: PyLaTeX==1.4.1
-Requires-Dist: pytest==7.4.0
-Requires-Dist: pytest-cov==4.1.0
-Requires-Dist: pytest-mpl==0.16.1
-Requires-Dist: scipy==1.10.1
-Requires-Dist: toml==0.10.2
+Requires-Dist: asdf~=3.0
+Requires-Dist: astropy~=6.0
+Requires-Dist: joblib~=1.3
+Requires-Dist: lmfit~=1.2
+Requires-Dist: matplotlib~=3.7
+Requires-Dist: mplcursors~=0.5
+Requires-Dist: nbsphinx~=0.9
+Requires-Dist: numpy~=1.24
+Requires-Dist: openpyxl~=3.1
+Requires-Dist: pandas~=2.0
+Requires-Dist: PyLaTeX~=1.4
+Requires-Dist: pytest~=7.4
+Requires-Dist: pytest-cov~=4.1
+Requires-Dist: pytest-mpl~=0.16
+Requires-Dist: scipy~=1.10
+Requires-Dist: toml~=0.10
 Requires-Dist: tomli>=2.0.0; python_version < "3.11"
 
 
 .. image:: https://github.com/Vital-Fernandez/lime/blob/0afedb150b0169deec6c7f159def99750a3a30da/docs/source/_static/logo_transparent.png?raw=true
     :width: 50%
     :align: center
     :alt: Line Measurer (LiMe) library.
 
 |Repo status| |CI badge| |Documentation Status| |Code cov| |PyPI version| |PyPI downloads| |Code Size| |PyPI license|
 
 This library provides a set of tools to fit lines in astronomical spectra. Its design aims for a user-friendly workflow
-for both single lines and large data sets. The library provides tools for masking, detecting, profile fitting
-and storing the results. . The output measurements are focused on the gas chemical and kinematic analysis.
+for both single lines and large data sets. The functions can be used for masking data, detecting lines, fitting profiles
+and storing the results. The output measurements support the chemical and kinematic analysis of the observed transitions.
 
 Please check the `online documentation <https://lime-stable.readthedocs.io/>`_.
 
 Installation
 ============
 
 The library can be installed directly from its PyPi_ project page running the command:
 
 ``pip install lime-stable``
 
 Development
 ===========
 
-LiMe is currently in a beta release. Please check its github_ for the latest version news and tutorials.
-Any comment/issue/request can be added as an issue on the github_ page.
+LiMe is currently on its initial release. Any comment/issue/request can be added as an issue on the github_ page.
 
 .. _PyPi: https://pypi.org/project/lime-stable/
 .. _github: https://github.com/Vital-Fernandez/lime
 
 .. |Repo status| image:: http://www.repostatus.org/badges/latest/active.svg
     :target: http://www.repostatus.org/#active
     :alt: Project Status: Active – The project has reached a stable, usable state and is being actively developed.
```

### Comparing `lime-stable-0.9.99.5/tests/test_astro.py` & `lime-stable-1.0.0/tests/test_astro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import numpy as np
 import pandas as pd
 import lime
 
+
 def test_line_bands():
 
     log0 = lime.line_bands()
     parent_bands = lime.load_frame(lime._lines_database_path)
 
     # TODO rework on the master database
     # assert np.all(log0.index == parent_bands.index)
-    assert np.all(log0.columns == parent_bands.columns)
     # assert log0.equals(parent_bands)
+    assert np.all(log0.columns == parent_bands.columns)
 
     log1 = lime.line_bands(wave_intvl=(3000, 7000))
     assert np.all((3000 <= log1.wavelength.to_numpy()) & (log1.wavelength.to_numpy() <= 7000))
 
     log2 = lime.line_bands(wave_intvl=(3000, 7000), z_intvl=(0, 2))
     assert np.all((3000 * (1 + 0) <= log2.wavelength.to_numpy()) & (log2.wavelength.to_numpy() <= 7000 * (1 + 2)))
```

### Comparing `lime-stable-0.9.99.5/tests/test_cube.py` & `lime-stable-1.0.0/tests/test_cube.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         return fig
 
     @pytest.mark.mpl_image_compare(baseline_dir='baseline')
     def test_check_cube(self):
 
         fig = plt.figure()
-        cube.check.cube('H1_6563A', lines_log_file=spatial_log_address, masks_file=spatial_mask_address, in_fig=fig)
+        cube.check.cube('H1_6563A', lines_file=spatial_log_address, masks_file=spatial_mask_address, in_fig=fig)
 
         return fig
 
     def test_save_paramter_maps(self):
 
         ouput_folder = Path(__file__).parent/'outputs'
```

### Comparing `lime-stable-0.9.99.5/tests/test_io.py` & `lime-stable-1.0.0/tests/test_io.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,8 @@
         line = lime.Line.from_log(label, log_lines)
         if line.blended_check is False:
             param_exp_value = log_lines.loc[label, 'eqw']
             param_value = log_lines.loc[label, 'eqw_new']
             param_exp_err = log_lines.loc[label, f'eqw_new_err']
             assert np.allclose(param_value, param_exp_value, atol=np.abs(param_exp_err * 2), equal_nan=True)
 
-    return
+    return
```

### Comparing `lime-stable-0.9.99.5/tests/test_line.py` & `lime-stable-1.0.0/tests/test_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,29 +53,32 @@
 
         line = Line('O3_5007A_b', band=None, fit_conf=fit_conf)
         assert np.all(line.particle == [Particle.from_label('O3'), Particle.from_label('O3'), Particle.from_label('He1')])
         assert np.all(line.wavelength == np.array([5006.7664, 5006.7664, 5016.]))
         assert np.all(line.kinem == np.array([0, 1, 0]))
         assert np.all(line.transition_comp == np.array(['col', 'col', 'rec']))
         assert np.all(line.profile_comp == np.array(['g-emi', 'g-emi', 'g-emi']))
-        assert np.all(line.latex_label == np.array(['$[OIII]5007\mathring{A}$', '$[OIII]5007\mathring{A}-k_1$', '$HeI5016\mathring{A}$']))
+        assert np.all(line.latex_label == np.array(['$[OIII]5007\mathring{A}$',
+                                                    '$[OIII]5007\mathring{A}-k_1$',
+                                                    '$HeI5016\mathring{A}$']))
         assert np.all(line.list_comps == ['O3_5007A', 'O3_5007A_k-1', 'He1_5016A'])
 
         assert line.label == 'O3_5007A_b'
         assert line.group_label == 'O3_5007A+O3_5007A_k-1+He1_5016A'
         assert np.all(line.mask == O3_band)
 
         line = Line('O3_5007A_m', band=np.array([1, 2, 3, 4, 5, 6]), fit_conf=fit_conf)
         assert np.all(line.particle == [Particle('O3', symbol='O', ionization=3)])
         assert np.all(line.wavelength == np.array([5007]))
         assert np.all(line.kinem == np.array([0]))
         assert np.all(line.transition_comp == np.array(['col']))
         assert np.all(line.profile_comp == np.array(['g-emi', 'g-emi']))
         assert np.all(line.latex_label == np.array([r'$[OIII]5007\mathring{A}$+$[OIII]5007\mathring{A}-k_1$']))
         assert np.all(line.list_comps == ['O3_5007A_m'])
+        assert np.all(line.mask == np.array([1, 2, 3, 4, 5, 6]))
 
         assert line.label == 'O3_5007A_m'
         assert line.group_label == 'O3_5007A+O3_5007A_k-1'
         assert np.all(line.mask == np.array([1, 2, 3, 4, 5, 6]))
 
         return
```

### Comparing `lime-stable-0.9.99.5/tests/test_model.py` & `lime-stable-1.0.0/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,37 +22,35 @@
 gaussian_array = gaussian(x_array, amp * np.sqrt(2*np.pi) * sigma, mu, sigma)
 lorentzian_array = lorentzian(x_array, amp * np.pi * sigma, mu, sigma)
 pseudo_voigt_array = frac * gaussian_array + (1 - frac) * lorentzian_array
 
 
 def test_gaussian():
 
-
     y_array = gaussian_array + cont_array + noise_array
     spec = lime.Spectrum(x_array, y_array, redshift=0, norm_flux=1)
     spec.fit.bands('H1_4861A')
 
     assert np.allclose(spec.fit.line.amp, amp, rtol=0.01)
     assert np.allclose(spec.fit.line.center, mu, rtol=0.01)
     assert np.allclose(spec.fit.line.sigma, sigma, rtol=0.01)
     assert np.allclose(spec.fit.line.gamma, np.nan, equal_nan=True)
     assert np.allclose(spec.fit.line.frac, np.nan, equal_nan=True)
 
     assert np.allclose(spec.fit.line.m_cont, m_cont, rtol=0.05)
-    print(spec.fit.line.n_cont_err)
-    assert np.allclose(spec.fit.line.n_cont, n_cont, rtol=0.5) # TODO check why so big...
+    assert np.allclose(spec.fit.line.n_cont, n_cont, rtol=spec.fit.line.n_cont_err)
 
     p_shape = spec.fit.line._p_shape[0]
     g_fwhm = 2 * np.sqrt(2 * np.log(2)) * sigma
     g_area = amp * sigma * np.sqrt(2 * np.pi)
     assert p_shape == 'g'
     assert np.allclose(spec.fit.line.FWHM_p, g_fwhm, rtol=0.01)
-    # assert np.allclose(spec.fit.line.FWHM_i, g_fwhm, rtol=0.01)   # TODO correct this calculation
     assert np.allclose(spec.fit.line.intg_flux, g_area, rtol=0.01)
     assert np.allclose(spec.fit.line.profile_flux, g_area, rtol=0.01)
+    # assert np.allclose(spec.fit.line.FWHM_i, g_fwhm, rtol=0.01)   # TODO correct this calculation
 
     return
 
 
 def test_lorentzian():
 
     y_array = lorentzian_array + cont_array + noise_array
```

### Comparing `lime-stable-0.9.99.5/tests/test_sample.py` & `lime-stable-1.0.0/tests/test_sample.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 
         sample1 = lime.Sample.from_file(id_list=['spec1', 'spec2'],
                                         log_list=[lines_log_address, lines_log_address],
                                         file_list=['spec1.fits', 'spec2.fits'],
                                         instrument='isis')
         sample1.save_frame(outputs_folder / f'sample1_3indeces.txt')
 
-        assert list(sample1.log.index.names) == ['id', 'file', 'line']
+        assert list(sample1.frame.index.names) == ['id', 'file', 'line']
 
         sample2 = lime.Sample.from_file(id_list=['spec1', 'spec2'], log_list=[lines_log_address, lines_log_address],
                                         instrument='isis')
         sample2.save_frame(outputs_folder / f'sample1_2indeces.txt')
-        assert list(sample2.log.index.names) == ['id', 'line']
+        assert list(sample2.frame.index.names) == ['id', 'line']
 
         sample3 = lime.Sample(outputs_folder / f'sample1_3indeces.txt', instrument='isis')
         sample4 = lime.Sample(outputs_folder / f'sample1_2indeces.txt', levels=['id', 'line'], instrument='isis')
 
-        assert list(sample3.log.index.names) == ['id', 'file', 'line']
-        assert list(sample4.log.index.names) == ['id', 'line']
+        assert list(sample3.frame.index.names) == ['id', 'file', 'line']
+        assert list(sample4.frame.index.names) == ['id', 'line']
 
-        assert sample3.log.equals(sample1.log)
-        assert sample4.log.equals(sample2.log)
+        assert sample3.frame.equals(sample1.frame)
+        assert sample4.frame.equals(sample2.frame)
 
         return
 
     # def test_multindex_log(self):
     #
     #     # Default import
     #     assert isinstance(obs.log.index, pd.MultiIndex)
```

### Comparing `lime-stable-0.9.99.5/tests/test_spectrum.py` & `lime-stable-1.0.0/tests/test_spectrum.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
                      pixel_mask=pixel_mask)
 
 spec.fit.frame(bands_file_address, cfg, id_conf_prefix='38-35')
 
 
 def measurement_tolerance_test(input_spec, true_log, test_log, abs_factor=2, rel_tol=0.20):
 
-    for line in input_spec.log.index:
-        for param in input_spec.log.columns:
+    for line in input_spec.frame.index:
+        for param in input_spec.frame.columns:
 
             # String
             if _LOG_EXPORT_DICT[param].startswith('<U'):
                 if true_log.loc[line, param] is np.nan:
                     assert true_log.loc[line, param] is test_log.loc[line, param]
                 else:
                     assert true_log.loc[line, param] == test_log.loc[line, param]
@@ -122,15 +122,16 @@
         assert np.allclose(err_array, spec0.err_flux.data * norm_flux, equal_nan=True)
 
         return
 
     @pytest.mark.mpl_image_compare(tolerance=tolerance_rms)
     def test_line_detection_plot(self):
 
-        match_bands = spec.line_detection(bands_file_address, cont_fit_degree=[3, 7, 7, 7], cont_int_thres=[5, 3, 2, 1.5])
+        spec.fit.continuum(degree_list=[3, 6, 6], emis_threshold=[5, 3, 2])
+        match_bands = spec.line_detection(bands_file_address)
 
         fig = plt.figure()
         spec.plot.spectrum(in_fig=fig, line_bands=match_bands)
 
         return fig
 
     @pytest.mark.mpl_image_compare(tolerance=tolerance_rms)
@@ -254,15 +255,15 @@
                 remove(file_xlsx)
                 print(f"File '{file_xlsx}' has been deleted successfully.")
             except OSError as e:
                 print(f"Error: {e.strerror}")
 
         log_orig = lime.load_frame(lines_log_address)
 
-        for page in ['LINELOG', 'LINESLOG2', 'LINELOG']:
+        for page in ['FRAME', 'FRAME2', 'FRAME']:
             spec.save_frame(outputs_folder / file_xlsx, page=page)
             log_test = lime.load_frame(file_xlsx)
 
             measurement_tolerance_test(spec, log_orig, log_test)
 
         return
```

### Comparing `lime-stable-0.9.99.5/tests/test_tools.py` & `lime-stable-1.0.0/tests/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 import lime
 from pathlib import Path
-from lime.tools import int_to_roman, format_line_mask_option, refraction_index_air_vacuum, logs_into_fits
+from lime.tools import int_to_roman, format_line_mask_option, refraction_index_air_vacuum, join_fits_files
 from lime.io import _LOG_EXPORT_DICT, hdu_to_log_df
 from astropy.io import fits
 
 # Data for the tests
 baseline_folder = Path(__file__).parent / 'baseline'
 outputs_folder = Path(__file__).parent / 'outputs'
 
@@ -41,15 +41,15 @@
 
 
 def test_extract_fluxes():
 
     log1 = lines_log.copy()
     log2 = lines_log.copy()
     log3 = lines_log.copy()
-    log4 = obs.log.copy()
+    log4 = obs.frame.copy()
 
     lime.extract_fluxes(log1)
     lime.extract_fluxes(log2, flux_type='intg', column_name='integrated', column_positions=3)
     lime.extract_fluxes(log3, flux_type='profile', column_name='flux')
     lime.extract_fluxes(log4)
 
     # Mixture
@@ -130,21 +130,21 @@
     assert np.isnan(log3.loc['O3_4363A', 'line_flux'])
 
     return
 
 
 def test_extract_fluxes_multi_index():
 
-    idcs_remove = (obs.log.index.get_level_values('id') == 'obj_1') &\
-                  (~obs.log.index.get_level_values('line').isin(['H1_6563A', 'O3_4363A', 'H1_4861A']))
+    idcs_remove = (obs.frame.index.get_level_values('id') == 'obj_1') & \
+                  (~obs.frame.index.get_level_values('line').isin(['H1_6563A', 'O3_4363A', 'H1_4861A']))
 
-    log1 = obs.log.loc[~idcs_remove].copy()
-    log2 = obs.log.copy()
-    log3 = obs.log.copy()
-    log4 = obs.log.copy()
+    log1 = obs.frame.loc[~idcs_remove].copy()
+    log2 = obs.frame.copy()
+    log3 = obs.frame.copy()
+    log4 = obs.frame.copy()
 
     # One line normalization
     lime.normalize_fluxes(log1, norm_list='H1_4861A')
     ratio = log1.xs('O3_5007A', level='line')['profile_flux'] / log1.xs('H1_4861A', level='line')['profile_flux']
     assert log1.xs('O3_5007A', level='line')['line_flux']['obj_0'] == ratio['obj_0']
     assert log1.xs('O3_5007A', level='line')['line_flux']['obj_2'] == ratio['obj_2']
     assert np.isnan(ratio['obj_1'])
@@ -199,18 +199,18 @@
     assert z_df['weight'][0] is None
     assert z_df_eqw['weight'][0] == 'eqw'
     assert z_df_flux_gauss['weight'][0] == 'profile_flux'
     assert z_df_strong['weight'][0] is None
     assert z_df_strong['lines'][0] == 'O3_5007A,H1_6563A'
 
     # Multi-index
-    z_df = lime.redshift_calculation(obs.log)
-    z_df_eqw = lime.redshift_calculation(obs.log, weight_parameter='eqw')
-    z_df_flux_gauss = lime.redshift_calculation(obs.log, weight_parameter='profile_flux')
-    z_df_strong = lime.redshift_calculation(obs.log, line_list=['O3_5007A', 'H1_6563A'])
+    z_df = lime.redshift_calculation(obs.frame)
+    z_df_eqw = lime.redshift_calculation(obs.frame, weight_parameter='eqw')
+    z_df_flux_gauss = lime.redshift_calculation(obs.frame, weight_parameter='profile_flux')
+    z_df_strong = lime.redshift_calculation(obs.frame, line_list=['O3_5007A', 'H1_6563A'])
 
     assert np.allclose(z_df['z_mean'][0], 0.047526, atol=0.00024, equal_nan=True)
     assert np.allclose(z_df_eqw['z_mean'][0], 0.047526, atol=0.00024, equal_nan=True)
     assert np.allclose(z_df_flux_gauss['z_mean'][0], 0.047526, atol=0.00024, equal_nan=True)
     assert np.allclose(z_df_strong['z_mean'][0], 0.047498, atol=0.000018, equal_nan=True)
 
     assert np.all(z_df['weight'].to_numpy() == None)
@@ -268,15 +268,15 @@
     lime.save_frame(outputs_folder / f'log_1.txt', log_orig)
     lime.save_frame(outputs_folder / f'log_2.fits', log_orig, page='LOG2')
     lime.save_frame(outputs_folder / f'log_2.fits', log_orig, page='LOG3')
 
     file_list = [outputs_folder/f'log_1.txt', outputs_folder/f'log_2.fits']
     output_file = outputs_folder/'joined_log.fits'
 
-    logs_into_fits(file_list, output_file, delete_after_join=True)
+    join_fits_files(file_list, output_file, delete_after_join=True)
 
     # Check new and deteled files
     assert output_file.is_file()
     assert not file_list[0].is_file()
     assert not file_list[1].is_file()
 
     name_pages = ['LOG_1', 'LOG2', 'LOG3']
```

