# Comparing `tmp/conect2py-0.1.2.tar.gz` & `tmp/conect2py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conect2py-0.1.2.tar", last modified: Thu Oct 26 14:41:44 2023, max compression
+gzip compressed data, was "conect2py-0.1.3.tar", last modified: Mon Apr 29 16:51:24 2024, max compression
```

## Comparing `conect2py-0.1.2.tar` & `conect2py-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-10-26 14:41:44.206942 conect2py-0.1.2/
--rw-rw-rw-   0        0        0     1071 2023-10-23 17:30:14.000000 conect2py-0.1.2/LICENSE
--rw-rw-rw-   0        0        0    10061 2023-10-26 14:41:44.206942 conect2py-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     9567 2023-10-26 14:37:36.000000 conect2py-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-10-26 14:41:44.175084 conect2py-0.1.2/conect2py/
--rw-rw-rw-   0        0        0       40 2023-10-25 18:02:57.000000 conect2py-0.1.2/conect2py/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-26 14:41:44.191074 conect2py-0.1.2/conect2py/models/
--rw-rw-rw-   0        0        0     6552 2023-10-25 19:00:00.000000 conect2py-0.1.2/conect2py/models/AutoTAC.py
--rw-rw-rw-   0        0        0     5278 2023-10-25 18:57:11.000000 conect2py-0.1.2/conect2py/models/TAC.py
--rw-rw-rw-   0        0        0       82 2023-10-25 18:05:02.000000 conect2py-0.1.2/conect2py/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-26 14:41:44.191074 conect2py-0.1.2/conect2py/run/
--rw-rw-rw-   0        0        0       42 2023-10-25 18:05:22.000000 conect2py-0.1.2/conect2py/run/__init__.py
--rw-rw-rw-   0        0        0     9603 2023-10-26 14:39:17.000000 conect2py-0.1.2/conect2py/run/multiple.py
--rw-rw-rw-   0        0        0     5778 2023-09-18 13:21:24.000000 conect2py-0.1.2/conect2py/run/single.py
-drwxrwxrwx   0        0        0        0 2023-10-26 14:41:44.200406 conect2py-0.1.2/conect2py/utils/
--rw-rw-rw-   0        0        0       55 2023-10-25 18:03:48.000000 conect2py-0.1.2/conect2py/utils/__init__.py
--rw-rw-rw-   0        0        0     7617 2023-09-18 13:24:17.000000 conect2py-0.1.2/conect2py/utils/format_save.py
--rw-rw-rw-   0        0        0    16112 2023-09-18 13:24:32.000000 conect2py-0.1.2/conect2py/utils/metrics.py
--rw-rw-rw-   0        0        0     9576 2023-10-20 19:46:04.000000 conect2py-0.1.2/conect2py/utils/plots.py
-drwxrwxrwx   0        0        0        0 2023-10-26 14:41:44.183073 conect2py-0.1.2/conect2py.egg-info/
--rw-rw-rw-   0        0        0    10061 2023-10-26 14:41:43.000000 conect2py-0.1.2/conect2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-10-26 14:41:43.000000 conect2py-0.1.2/conect2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-26 14:41:43.000000 conect2py-0.1.2/conect2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-10-26 14:41:43.000000 conect2py-0.1.2/conect2py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-10-26 14:41:43.000000 conect2py-0.1.2/conect2py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-26 14:41:44.206942 conect2py-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1277 2023-10-26 14:40:48.000000 conect2py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:51:24.807556 conect2py-0.1.3/
+-rw-rw-rw-   0        0        0     1071 2023-10-23 17:30:14.000000 conect2py-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-29 16:30:36.000000 conect2py-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    10588 2024-04-29 16:51:24.804777 conect2py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10092 2024-04-29 16:00:45.000000 conect2py-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 16:51:24.777047 conect2py-0.1.3/conect2py/
+-rw-rw-rw-   0        0        0       40 2023-10-25 18:02:57.000000 conect2py-0.1.3/conect2py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:51:24.793393 conect2py-0.1.3/conect2py/models/
+-rw-rw-rw-   0        0        0    20786 2023-12-28 07:09:01.000000 conect2py-0.1.3/conect2py/models/AutoCloud.py
+-rw-rw-rw-   0        0        0     6552 2023-10-25 19:00:00.000000 conect2py-0.1.3/conect2py/models/AutoTAC.py
+-rw-rw-rw-   0        0        0     5278 2023-10-25 18:57:11.000000 conect2py-0.1.3/conect2py/models/TAC.py
+-rw-rw-rw-   0        0        0     5797 2023-12-28 06:24:09.000000 conect2py-0.1.3/conect2py/models/TEDA.py
+-rw-rw-rw-   0        0        0       82 2023-10-25 18:05:02.000000 conect2py-0.1.3/conect2py/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:51:24.797573 conect2py-0.1.3/conect2py/run/
+-rw-rw-rw-   0        0        0       42 2023-10-25 18:05:22.000000 conect2py-0.1.3/conect2py/run/__init__.py
+-rw-rw-rw-   0        0        0     9603 2023-10-26 14:39:17.000000 conect2py-0.1.3/conect2py/run/multiple.py
+-rw-rw-rw-   0        0        0     5778 2023-09-18 13:21:24.000000 conect2py-0.1.3/conect2py/run/single.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:51:24.804777 conect2py-0.1.3/conect2py/utils/
+-rw-rw-rw-   0        0        0       55 2023-10-25 18:03:48.000000 conect2py-0.1.3/conect2py/utils/__init__.py
+-rw-rw-rw-   0        0        0     7617 2023-09-18 13:24:17.000000 conect2py-0.1.3/conect2py/utils/format_save.py
+-rw-rw-rw-   0        0        0    16112 2023-09-18 13:24:32.000000 conect2py-0.1.3/conect2py/utils/metrics.py
+-rw-rw-rw-   0        0        0     9576 2023-10-20 19:46:04.000000 conect2py-0.1.3/conect2py/utils/plots.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:51:24.783312 conect2py-0.1.3/conect2py.egg-info/
+-rw-rw-rw-   0        0        0    10588 2024-04-29 16:51:24.000000 conect2py-0.1.3/conect2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2024-04-29 16:51:24.000000 conect2py-0.1.3/conect2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:51:24.000000 conect2py-0.1.3/conect2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2024-04-29 16:51:24.000000 conect2py-0.1.3/conect2py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 16:51:24.000000 conect2py-0.1.3/conect2py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:51:24.807556 conect2py-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1277 2024-04-29 16:50:13.000000 conect2py-0.1.3/setup.py
```

### Comparing `conect2py-0.1.2/LICENSE` & `conect2py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `conect2py-0.1.2/PKG-INFO` & `conect2py-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conect2py
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python library for data compression using TAC (Tiny Anomaly Compression)
 Home-page: https://github.com/conect2ai/Conect2Py-Package
 Author: Conect2ai
 Author-email: conect2ai@gmail.com
 Keywords: TEDA,TAC,Annomaly Detection,Data Compression,IoT,Eccentricity
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,24 @@
 &nbsp;
 
 
 # Conect2Ai - TAC python package
 
 Conect2Py-Package is the name given for the Conect2ai Python software package. The package contains the implementation of TAC, an algorithm for data compression using TAC (Tiny Anomaly Compression). The TAC algorithm is based on the concept the data eccentricity and does not require previously established mathematical models or any assumptions about the underlying data distribution.  Additionally, it uses recursive equations, which enables an efficient computation with low computational cost, using little memory and processing power.
 
-Currente version:  ![version](https://img.shields.io/badge/version-0.1.1-blue)
+<p align="right">
+  <img alt="version" src="https://img.shields.io/badge/version-0.1.1-blue">
+</p>
+
+
+
+- [Installation](#installation)
+- [Usage](#usage-example)
+- [References](#literature-reference)
+- [License](#license)
 
 ---
 #### Dependencies
 
 ```bash
 Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn, Ipython
 ```
@@ -48,38 +57,38 @@
 
 ```bash
 pip install conect2py-0.1.1-py3-none-any.whl
 ```
 
 ---
 
-## Example of Use
+## Usage Example
 
-To begin you can import TACpy using
+To begin you can import `conect2py` using
 
 ```Python
 # FULL PACKAGE
-import tac
+import conect2py
 ```
 
 Or try each of our implemented functionalities
 
 ```Python
 # MODEL FUNCTIONS
-from conect2ai.models.TAC import TAC
-from conect2ai.models.AutoTAC import AutoTAC
+from conect2py.models import TAC
+from conect2py.models import AutoTAC
 
 # RUN FUNCTIONS
-from conect2ai.run.single import (print_run_details)
-from conect2ai.run.multiple import (run_multiple_instances, get_optimal_params, display_multirun_optimal_values, run_optimal_combination)
+from conect2py.run.single import print_run_details, run_single_online, run_single_offline
+from conect2py.run.multiple import run_multiple_instances, get_optimal_params, display_multirun_optimal_values, run_optimal_combination
 
 # UTILS FUNCTIONS
-from conect2ai.utils.format_save import (create_param_combinations, create_compressor_list, create_eval_df) 
-from conect2ai.utils.metrics import (get_compression_report, print_compression_report, calc_statistics)
-from conect2ai.utils.plots import (plot_curve_comparison, plot_dist_comparison, plot_multirun_metric_results)
+from conect2py.utils.format_save import create_param_combinations, create_compressor_list, create_eval_df 
+from conect2py.utils.metrics import get_compression_report, print_compression_report, calc_statistics
+from conect2py.utils.plots import plot_curve_comparison, plot_dist_comparison, plot_multirun_metric_results 
 
 ```
 
 ### *Running Multiple tests with TAC*
 - Setting up the initial variables
 
 ```Python
@@ -275,21 +284,22 @@
 And finally here is a example of the result:
 
 ![image](https://github.com/conect2ai/Conect2Py-Package/assets/56210040/978fdeaa-688c-4c8a-90c7-7726eab96302)
 
 
 
 
+## Other Models
 
-
-
-
-
-
-
+Please check the [informations](https://github.com/conect2ai/Conect2Py-Package/blob/main/Info/AutoCloud.md) for more information about the other models been implemented in this package.
 
 
 # Literature reference
 
+
 1. Signoretti, G.; Silva, M.; Andrade, P.; Silva, I.; Sisinni, E.; Ferrari, P. "An Evolving TinyML Compression Algorithm for IoT Environments Based on Data Eccentricity". Sensors 2021, 21, 4153. https://doi.org/10.3390/s21124153
 
 2. Medeiros, T.; Amaral, M.; Targino, M; Silva, M.; Silva, I.; Sisinni, E.; Ferrari, P.; "TinyML Custom AI Algorithms for Low-Power IoT Data Compression: A Bridge Monitoring Case Study" - 2023 IEEE International Workshop on Metrology for Industry 4.0 & IoT (MetroInd4.0&IoT), 2023. [10.1109/MetroInd4.0IoT57462.2023.10180152](https://ieeexplore.ieee.org/document/10180152])
+
+# License
+
+This package is licensed under the [MIT License](https://github.com/conect2ai/Conect2Py-Package/blob/main/LICENSE) - Â© 2023 Conect2ai.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `conect2py-0.1.2/README.md` & `conect2py-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,24 @@
 &nbsp;
 
 
 # Conect2Ai - TAC python package
 
 Conect2Py-Package is the name given for the Conect2ai Python software package. The package contains the implementation of TAC, an algorithm for data compression using TAC (Tiny Anomaly Compression). The TAC algorithm is based on the concept the data eccentricity and does not require previously established mathematical models or any assumptions about the underlying data distribution.  Additionally, it uses recursive equations, which enables an efficient computation with low computational cost, using little memory and processing power.
 
-Currente version:  ![version](https://img.shields.io/badge/version-0.1.1-blue)
+<p align="right">
+  <img alt="version" src="https://img.shields.io/badge/version-0.1.1-blue">
+</p>
+
+
+
+- [Installation](#installation)
+- [Usage](#usage-example)
+- [References](#literature-reference)
+- [License](#license)
 
 ---
 #### Dependencies
 
 ```bash
 Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn, Ipython
 ```
@@ -35,38 +44,38 @@
 
 ```bash
 pip install conect2py-0.1.1-py3-none-any.whl
 ```
 
 ---
 
-## Example of Use
+## Usage Example
 
-To begin you can import TACpy using
+To begin you can import `conect2py` using
 
 ```Python
 # FULL PACKAGE
-import tac
+import conect2py
 ```
 
 Or try each of our implemented functionalities
 
 ```Python
 # MODEL FUNCTIONS
-from conect2ai.models.TAC import TAC
-from conect2ai.models.AutoTAC import AutoTAC
+from conect2py.models import TAC
+from conect2py.models import AutoTAC
 
 # RUN FUNCTIONS
-from conect2ai.run.single import (print_run_details)
-from conect2ai.run.multiple import (run_multiple_instances, get_optimal_params, display_multirun_optimal_values, run_optimal_combination)
+from conect2py.run.single import print_run_details, run_single_online, run_single_offline
+from conect2py.run.multiple import run_multiple_instances, get_optimal_params, display_multirun_optimal_values, run_optimal_combination
 
 # UTILS FUNCTIONS
-from conect2ai.utils.format_save import (create_param_combinations, create_compressor_list, create_eval_df) 
-from conect2ai.utils.metrics import (get_compression_report, print_compression_report, calc_statistics)
-from conect2ai.utils.plots import (plot_curve_comparison, plot_dist_comparison, plot_multirun_metric_results)
+from conect2py.utils.format_save import create_param_combinations, create_compressor_list, create_eval_df 
+from conect2py.utils.metrics import get_compression_report, print_compression_report, calc_statistics
+from conect2py.utils.plots import plot_curve_comparison, plot_dist_comparison, plot_multirun_metric_results 
 
 ```
 
 ### *Running Multiple tests with TAC*
 - Setting up the initial variables
 
 ```Python
@@ -262,21 +271,22 @@
 And finally here is a example of the result:
 
 ![image](https://github.com/conect2ai/Conect2Py-Package/assets/56210040/978fdeaa-688c-4c8a-90c7-7726eab96302)
 
 
 
 
+## Other Models
 
-
-
-
-
-
-
+Please check the [informations](https://github.com/conect2ai/Conect2Py-Package/blob/main/Info/AutoCloud.md) for more information about the other models been implemented in this package.
 
 
 # Literature reference
 
+
 1. Signoretti, G.; Silva, M.; Andrade, P.; Silva, I.; Sisinni, E.; Ferrari, P. "An Evolving TinyML Compression Algorithm for IoT Environments Based on Data Eccentricity". Sensors 2021, 21, 4153. https://doi.org/10.3390/s21124153
 
 2. Medeiros, T.; Amaral, M.; Targino, M; Silva, M.; Silva, I.; Sisinni, E.; Ferrari, P.; "TinyML Custom AI Algorithms for Low-Power IoT Data Compression: A Bridge Monitoring Case Study" - 2023 IEEE International Workshop on Metrology for Industry 4.0 & IoT (MetroInd4.0&IoT), 2023. [10.1109/MetroInd4.0IoT57462.2023.10180152](https://ieeexplore.ieee.org/document/10180152])
+
+# License
+
+This package is licensed under the [MIT License](https://github.com/conect2ai/Conect2Py-Package/blob/main/LICENSE) - © 2023 Conect2ai.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `conect2py-0.1.2/conect2py/models/AutoTAC.py` & `conect2py-0.1.3/conect2py/models/AutoTAC.py`

 * *Files identical despite different names*

### Comparing `conect2py-0.1.2/conect2py/models/TAC.py` & `conect2py-0.1.3/conect2py/models/TAC.py`

 * *Files identical despite different names*

### Comparing `conect2py-0.1.2/conect2py/run/multiple.py` & `conect2py-0.1.3/conect2py/run/multiple.py`

 * *Files identical despite different names*

### Comparing `conect2py-0.1.2/conect2py/run/single.py` & `conect2py-0.1.3/conect2py/run/single.py`

 * *Files identical despite different names*

### Comparing `conect2py-0.1.2/conect2py/utils/format_save.py` & `conect2py-0.1.3/conect2py/utils/format_save.py`

 * *Files identical despite different names*

### Comparing `conect2py-0.1.2/conect2py/utils/metrics.py` & `conect2py-0.1.3/conect2py/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `conect2py-0.1.2/conect2py/utils/plots.py` & `conect2py-0.1.3/conect2py/utils/plots.py`

 * *Files identical despite different names*

### Comparing `conect2py-0.1.2/conect2py.egg-info/PKG-INFO` & `conect2py-0.1.3/conect2py.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conect2py
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python library for data compression using TAC (Tiny Anomaly Compression)
 Home-page: https://github.com/conect2ai/Conect2Py-Package
 Author: Conect2ai
 Author-email: conect2ai@gmail.com
 Keywords: TEDA,TAC,Annomaly Detection,Data Compression,IoT,Eccentricity
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,24 @@
 &nbsp;
 
 
 # Conect2Ai - TAC python package
 
 Conect2Py-Package is the name given for the Conect2ai Python software package. The package contains the implementation of TAC, an algorithm for data compression using TAC (Tiny Anomaly Compression). The TAC algorithm is based on the concept the data eccentricity and does not require previously established mathematical models or any assumptions about the underlying data distribution.  Additionally, it uses recursive equations, which enables an efficient computation with low computational cost, using little memory and processing power.
 
-Currente version:  ![version](https://img.shields.io/badge/version-0.1.1-blue)
+<p align="right">
+  <img alt="version" src="https://img.shields.io/badge/version-0.1.1-blue">
+</p>
+
+
+
+- [Installation](#installation)
+- [Usage](#usage-example)
+- [References](#literature-reference)
+- [License](#license)
 
 ---
 #### Dependencies
 
 ```bash
 Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn, Ipython
 ```
@@ -48,38 +57,38 @@
 
 ```bash
 pip install conect2py-0.1.1-py3-none-any.whl
 ```
 
 ---
 
-## Example of Use
+## Usage Example
 
-To begin you can import TACpy using
+To begin you can import `conect2py` using
 
 ```Python
 # FULL PACKAGE
-import tac
+import conect2py
 ```
 
 Or try each of our implemented functionalities
 
 ```Python
 # MODEL FUNCTIONS
-from conect2ai.models.TAC import TAC
-from conect2ai.models.AutoTAC import AutoTAC
+from conect2py.models import TAC
+from conect2py.models import AutoTAC
 
 # RUN FUNCTIONS
-from conect2ai.run.single import (print_run_details)
-from conect2ai.run.multiple import (run_multiple_instances, get_optimal_params, display_multirun_optimal_values, run_optimal_combination)
+from conect2py.run.single import print_run_details, run_single_online, run_single_offline
+from conect2py.run.multiple import run_multiple_instances, get_optimal_params, display_multirun_optimal_values, run_optimal_combination
 
 # UTILS FUNCTIONS
-from conect2ai.utils.format_save import (create_param_combinations, create_compressor_list, create_eval_df) 
-from conect2ai.utils.metrics import (get_compression_report, print_compression_report, calc_statistics)
-from conect2ai.utils.plots import (plot_curve_comparison, plot_dist_comparison, plot_multirun_metric_results)
+from conect2py.utils.format_save import create_param_combinations, create_compressor_list, create_eval_df 
+from conect2py.utils.metrics import get_compression_report, print_compression_report, calc_statistics
+from conect2py.utils.plots import plot_curve_comparison, plot_dist_comparison, plot_multirun_metric_results 
 
 ```
 
 ### *Running Multiple tests with TAC*
 - Setting up the initial variables
 
 ```Python
@@ -275,21 +284,22 @@
 And finally here is a example of the result:
 
 ![image](https://github.com/conect2ai/Conect2Py-Package/assets/56210040/978fdeaa-688c-4c8a-90c7-7726eab96302)
 
 
 
 
+## Other Models
 
-
-
-
-
-
-
+Please check the [informations](https://github.com/conect2ai/Conect2Py-Package/blob/main/Info/AutoCloud.md) for more information about the other models been implemented in this package.
 
 
 # Literature reference
 
+
 1. Signoretti, G.; Silva, M.; Andrade, P.; Silva, I.; Sisinni, E.; Ferrari, P. "An Evolving TinyML Compression Algorithm for IoT Environments Based on Data Eccentricity". Sensors 2021, 21, 4153. https://doi.org/10.3390/s21124153
 
 2. Medeiros, T.; Amaral, M.; Targino, M; Silva, M.; Silva, I.; Sisinni, E.; Ferrari, P.; "TinyML Custom AI Algorithms for Low-Power IoT Data Compression: A Bridge Monitoring Case Study" - 2023 IEEE International Workshop on Metrology for Industry 4.0 & IoT (MetroInd4.0&IoT), 2023. [10.1109/MetroInd4.0IoT57462.2023.10180152](https://ieeexplore.ieee.org/document/10180152])
+
+# License
+
+This package is licensed under the [MIT License](https://github.com/conect2ai/Conect2Py-Package/blob/main/LICENSE) - Â© 2023 Conect2ai.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `conect2py-0.1.2/setup.py` & `conect2py-0.1.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 README_MD = open(join(dirname(abspath(__file__)), "README.md")).read()
 
 setup(
     # Name 
     name="conect2py",
 
     # Version
-    version="0.1.2",
+    version="0.1.3",
 
     # Packages
     packages=find_packages(include=['conect2py', 'conect2py.*']),
 
     # Description
     description="A python library for data compression using TAC (Tiny Anomaly Compression)",
 
@@ -33,9 +33,9 @@
         "Programming Language :: Python :: 3"
     ],
 
     # Keywords are tags that identify your project and help searching for it
     # This field is OPTIONAL
     keywords="TEDA, TAC, Annomaly Detection, Data Compression, IoT, Eccentricity",
 
-    install_requires=['numpy>=1.26', 'pandas>=2.1', 'matplotlib>=3.8', 'seaborn>=0.13', 'ipython>=8.16', 'scikit-learn>=1.3']
+    install_requires=['numpy>=1.26', 'pandas>=2.0', 'matplotlib>=3.8', 'seaborn>=0.13', 'ipython>=7.34', 'scikit-learn>=1.3']
 )
```

