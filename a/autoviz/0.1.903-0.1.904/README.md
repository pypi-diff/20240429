# Comparing `tmp/autoviz-0.1.903.tar.gz` & `tmp/autoviz-0.1.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoviz-0.1.903.tar", last modified: Sun Apr 28 16:05:47 2024, max compression
+gzip compressed data, was "autoviz-0.1.904.tar", last modified: Mon Apr 29 18:32:54 2024, max compression
```

## Comparing `autoviz-0.1.903.tar` & `autoviz-0.1.904.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 jupyter   (1002) jupyter   (1003)        0 2024-04-28 16:05:47.835416 autoviz-0.1.903/
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)    11558 2024-04-28 15:38:30.000000 autoviz-0.1.903/LICENSE
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)    14329 2024-04-28 16:05:47.835416 autoviz-0.1.903/PKG-INFO
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)    14195 2024-04-28 15:40:24.000000 autoviz-0.1.903/README.md
-drwxr-xr-x   0 jupyter   (1002) jupyter   (1003)        0 2024-04-28 16:05:47.831416 autoviz-0.1.903/autoviz/
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)    34934 2024-04-28 15:38:30.000000 autoviz-0.1.903/autoviz/AutoViz_Class.py
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)    64881 2024-04-28 15:38:30.000000 autoviz-0.1.903/autoviz/AutoViz_Holo.py
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)    24022 2024-04-28 15:38:30.000000 autoviz-0.1.903/autoviz/AutoViz_NLP.py
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)   117365 2024-04-28 15:38:30.000000 autoviz-0.1.903/autoviz/AutoViz_Utils.py
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)      875 2024-04-28 15:38:30.000000 autoviz-0.1.903/autoviz/__init__.py
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)      404 2024-04-28 15:38:30.000000 autoviz-0.1.903/autoviz/__version__.py
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)    18388 2024-04-28 15:38:30.000000 autoviz-0.1.903/autoviz/classify_method.py
-drwxr-xr-x   0 jupyter   (1002) jupyter   (1003)        0 2024-04-28 16:05:47.835416 autoviz-0.1.903/autoviz.egg-info/
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)    14329 2024-04-28 16:05:47.000000 autoviz-0.1.903/autoviz.egg-info/PKG-INFO
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)      366 2024-04-28 16:05:47.000000 autoviz-0.1.903/autoviz.egg-info/SOURCES.txt
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)        1 2024-04-28 16:05:47.000000 autoviz-0.1.903/autoviz.egg-info/dependency_links.txt
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)      243 2024-04-28 16:05:47.000000 autoviz-0.1.903/autoviz.egg-info/requires.txt
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)        8 2024-04-28 16:05:47.000000 autoviz-0.1.903/autoviz.egg-info/top_level.txt
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)       38 2024-04-28 16:05:47.835416 autoviz-0.1.903/setup.cfg
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)     1900 2024-04-28 15:38:30.000000 autoviz-0.1.903/setup.py
-drwxr-xr-x   0 jupyter   (1002) jupyter   (1003)        0 2024-04-28 16:05:47.835416 autoviz-0.1.903/tests/
--rw-r--r--   0 jupyter   (1002) jupyter   (1003)      231 2024-04-28 15:38:30.000000 autoviz-0.1.903/tests/test_deps.py
+drwxr-xr-x   0 rseshadri  (1000) rseshadri  (1000)        0 2024-04-29 18:32:54.113744 autoviz-0.1.904/
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)    11558 2022-09-30 17:57:06.000000 autoviz-0.1.904/LICENSE
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)    14348 2024-04-29 18:32:54.112743 autoviz-0.1.904/PKG-INFO
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)    14195 2024-04-29 14:29:12.000000 autoviz-0.1.904/README.md
+drwxr-xr-x   0 rseshadri  (1000) rseshadri  (1000)        0 2024-04-29 18:32:54.112743 autoviz-0.1.904/autoviz/
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)    34987 2024-04-29 18:22:03.000000 autoviz-0.1.904/autoviz/AutoViz_Class.py
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)    65361 2024-04-29 14:29:12.000000 autoviz-0.1.904/autoviz/AutoViz_Holo.py
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)    22978 2024-04-29 14:29:12.000000 autoviz-0.1.904/autoviz/AutoViz_NLP.py
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)   115272 2024-04-29 14:29:12.000000 autoviz-0.1.904/autoviz/AutoViz_Utils.py
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)      876 2024-04-29 14:29:12.000000 autoviz-0.1.904/autoviz/__init__.py
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)      404 2024-04-29 18:22:03.000000 autoviz-0.1.904/autoviz/__version__.py
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)    18857 2024-04-29 14:29:12.000000 autoviz-0.1.904/autoviz/classify_method.py
+drwxr-xr-x   0 rseshadri  (1000) rseshadri  (1000)        0 2024-04-29 18:32:54.112743 autoviz-0.1.904/autoviz/tests/
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)        0 2024-04-29 14:29:12.000000 autoviz-0.1.904/autoviz/tests/__init__.py
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)      134 2024-04-29 14:29:12.000000 autoviz-0.1.904/autoviz/tests/test_autoviz_class.py
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)      235 2024-04-29 14:29:12.000000 autoviz-0.1.904/autoviz/tests/test_deps.py
+drwxr-xr-x   0 rseshadri  (1000) rseshadri  (1000)        0 2024-04-29 18:32:54.112743 autoviz-0.1.904/autoviz.egg-info/
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)    14348 2024-04-29 18:32:53.000000 autoviz-0.1.904/autoviz.egg-info/PKG-INFO
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)      436 2024-04-29 18:32:54.000000 autoviz-0.1.904/autoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)        1 2024-04-29 18:32:53.000000 autoviz-0.1.904/autoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)      243 2024-04-29 18:32:53.000000 autoviz-0.1.904/autoviz.egg-info/requires.txt
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)        8 2024-04-29 18:32:53.000000 autoviz-0.1.904/autoviz.egg-info/top_level.txt
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)       38 2024-04-29 18:32:54.113744 autoviz-0.1.904/setup.cfg
+-rw-r--r--   0 rseshadri  (1000) rseshadri  (1000)     1900 2024-04-29 18:22:03.000000 autoviz-0.1.904/setup.py
```

### Comparing `autoviz-0.1.903/LICENSE` & `autoviz-0.1.904/LICENSE`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.903/PKG-INFO` & `autoviz-0.1.904/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.903
+Version: 0.1.904
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz.git
 Author: Ram Seshadri
 License: Apache License 2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AutoViz: The One-Line Automatic Data Visualization Library
 
@@ -267,7 +268,8 @@
   <li>Assumes the first row as the header in the file, but this can be changed.</li>
 </ul>
 
 - **By leveraging AutoViz's powerful and flexible features**, you can streamline your data visualization process and gain valuable insights more efficiently. Happy visualizing!
 
 ## DISCLAIMER
 This project is not an official Google project. It is not supported by Google, and Google specifically disclaims all warranties as to its quality, merchantability, or fitness for a particular purpose.
+
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.903 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.904 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz.git Author: Ram Seshadri License: Apache License
-2.0 Classifier: Programming Language :: Python :: 3 Classifier: Operating
-System :: OS Independent Description-Content-Type: text/markdown License-File:
-LICENSE # AutoViz: The One-Line Automatic Data Visualization Library ![logo]
-(images/logo.png) Unlock the power of **AutoViz** to visualize any dataset, any
-size, with just a single line of code! Plus, now you can get a quick assessment
-of your dataset's quality and fix DQ issues through the FixDQ() function. [!
-[Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/
-autoviz) [![Pepy Downloads per week](https://pepy.tech/badge/autoviz/week)]
-(https://pepy.tech/project/autoviz) [![Pepy Downloads per month](https://
-pepy.tech/badge/autoviz/month)](https://pepy.tech/project/autoviz) [![standard-
-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)]
-(https://github.com/RichardLitt/standard-readme) [![Python Versions](https://
-img.shields.io/pypi/pyversions/autoviz.svg)](https://pypi.org/project/autoviz)
-[![PyPI Version](https://img.shields.io/pypi/v/autoviz.svg)](https://pypi.org/
-project/autoviz) [![PyPI License](https://img.shields.io/pypi/l/autoviz.svg)]
-(https://github.com/AutoViML/AutoViz/blob/master/LICENSE) With AutoViz, you can
-easily and quickly generate insightful visualizations for your data. Whether
-you're a beginner or an expert in data analysis, AutoViz can help you explore
-your data and uncover valuable insights. Try it out and see the power of
-automated visualization for yourself! ## Table of Contents
+2.0 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE # AutoViz: The One-Line Automatic Data
+Visualization Library ![logo](images/logo.png) Unlock the power of **AutoViz**
+to visualize any dataset, any size, with just a single line of code! Plus, now
+you can get a quick assessment of your dataset's quality and fix DQ issues
+through the FixDQ() function. [![Pepy Downloads](https://pepy.tech/badge/
+autoviz)](https://pepy.tech/project/autoviz) [![Pepy Downloads per week](https:
+//pepy.tech/badge/autoviz/week)](https://pepy.tech/project/autoviz) [![Pepy
+Downloads per month](https://pepy.tech/badge/autoviz/month)](https://pepy.tech/
+project/autoviz) [![standard-readme compliant](https://img.shields.io/badge/
+standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
+[![Python Versions](https://img.shields.io/pypi/pyversions/autoviz.svg)](https:
+//pypi.org/project/autoviz) [![PyPI Version](https://img.shields.io/pypi/v/
+autoviz.svg)](https://pypi.org/project/autoviz) [![PyPI License](https://
+img.shields.io/pypi/l/autoviz.svg)](https://github.com/AutoViML/AutoViz/blob/
+master/LICENSE) With AutoViz, you can easily and quickly generate insightful
+visualizations for your data. Whether you're a beginner or an expert in data
+analysis, AutoViz can help you explore your data and uncover valuable insights.
+Try it out and see the power of automated visualization for yourself! ## Table
+of Contents
     * _L_a_t_e_s_t_ _U_p_d_a_t_e_s
     * _I_m_p_o_r_t_a_n_t_ _A_n_n_o_u_n_c_e_m_e_n_t
     * _C_i_t_a_t_i_o_n
     * _M_o_t_i_v_a_t_i_o_n_ _f_o_r_ _A_u_t_o_V_i_z
     * _H_o_w_ _t_o_ _u_s_e_ _A_u_t_o_V_i_z
     * _A_P_I_ _f_o_r_ _u_s_i_n_g_ _A_u_t_o_V_i_z
     * _E_x_a_m_p_l_e_s_ _o_f_ _u_s_i_n_g_ _A_u_t_o_V_i_z
```

### Comparing `autoviz-0.1.903/README.md` & `autoviz-0.1.904/README.md`

 * *Files identical despite different names*

### Comparing `autoviz-0.1.903/autoviz/AutoViz_Class.py` & `autoviz-0.1.904/autoviz/AutoViz_Class.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,79 +1,54 @@
 ############################################################################
-#Copyright 2019 Google LLC
+# Copyright 2019 Google LLC
 #
-#Licensed under the Apache License, Version 2.0 (the "License");
-#you may not use this file except in compliance with the License.
-#You may obtain a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
 #    https://www.apache.org/licenses/LICENSE-2.0
 #
-#Unless required by applicable law or agreed to in writing, software
-#distributed under the License is distributed on an "AS IS" BASIS,
-#WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#See the License for the specific language governing permissions and
-#limitations under the License.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 #################################################################################################
-import pandas as pd
-import numpy as np
-from pathlib import Path
 import os
-#### The warnings from Sklearn are so annoying that I have to shut it off ####
-import warnings
-warnings.filterwarnings("ignore")
-def warn(*args, **kwargs):
-    pass
-warnings.warn = warn
+import pandas as pd
 ########################################
 import warnings
-warnings.filterwarnings("ignore")
 from sklearn.exceptions import DataConversionWarning
-warnings.filterwarnings(action='ignore', category=DataConversionWarning)
 ####################################################################################
 import matplotlib
-matplotlib.use('agg')
-import matplotlib.pyplot as plt
-# from matplotlib import io
-import io
 import seaborn as sns
-sns.set(style="ticks", color_codes=True)
-import re
-import pprint
-import matplotlib
-from itertools import cycle, combinations
-from collections import defaultdict
 import copy
 import time
-import sys
-import random
-import xlrd
-import statsmodels
-from io import BytesIO
-import base64
-from functools import reduce
 import traceback
-import xgboost as xgb
-from xgboost.sklearn import XGBClassifier
-from xgboost.sklearn import XGBRegressor
-from sklearn.model_selection import train_test_split
-
+from pandas_dq import Fix_DQ, dq_report
 ##########################################################################################
 from autoviz.AutoViz_Holo import AutoViz_Holo
-from autoviz.AutoViz_Utils import save_image_data, analyze_problem_type, draw_pivot_tables, draw_scatters
-from autoviz.AutoViz_Utils import draw_pair_scatters, plot_fast_average_num_by_cat, draw_barplots, draw_heatmap
-from autoviz.AutoViz_Utils import draw_distplot, draw_violinplot, draw_date_vars, catscatter, draw_catscatterplots
-from autoviz.AutoViz_Utils import list_difference, search_for_word_in_list, analyze_ID_columns, start_classifying_vars
-from autoviz.AutoViz_Utils import analyze_columns_in_dataset, find_remove_duplicates, load_file_dataframe, classify_print_vars
-from autoviz.AutoViz_Utils import marthas_columns, EDA_find_remove_columns_with_infinity, return_dictionary_list
-from autoviz.AutoViz_Utils import remove_variables_using_fast_correlation, count_freq_in_list, find_corr_vars, left_subtract
-from autoviz.AutoViz_Utils import convert_train_test_cat_col_to_numeric, return_factorized_dict, convert_a_column_to_numeric
-from autoviz.AutoViz_Utils import convert_all_object_columns_to_numeric, find_top_features_xgb, convert_a_mixed_object_column_to_numeric
+from autoviz.AutoViz_Utils import draw_pivot_tables, draw_scatters
+from autoviz.AutoViz_Utils import draw_pair_scatters, draw_barplots, draw_heatmap
+from autoviz.AutoViz_Utils import draw_distplot, draw_violinplot, draw_date_vars, draw_catscatterplots
+from autoviz.AutoViz_Utils import list_difference
+from autoviz.AutoViz_Utils import find_remove_duplicates, classify_print_vars
+from autoviz.AutoViz_Utils import left_subtract
 from autoviz.AutoViz_NLP import draw_word_clouds
-#############################################################################################
-class AutoViz_Class():
+#######################################################################################
+sns.set(style="ticks", color_codes=True)
+matplotlib.use('agg')
+warnings.filterwarnings(action='ignore', category=DataConversionWarning)
+warnings.filterwarnings("ignore")
+#######################################################################################
+def warn(*args, **kwargs):
+    pass
+warnings.warn = warn
+#######################################################################################
+class AutoViz_Class:
     """
         ##############################################################################
         #############       This is not an Officially Supported Google Product! ######
         ##############################################################################
         #Copyright 2019 Google LLC                                              ######
         #                                                                       ######
         #Licensed under the Apache License, Version 2.0 (the "License");        ######
@@ -95,144 +70,144 @@
         ##############################################################################
         ##### AUTOVIZ PERFORMS AUTOMATIC VISUALIZATION OF ANY DATA SET WITH ONE CLICK.
         #####    Give it any input file (CSV, txt or json) and AV will visualize it.##
         ##### INPUTS:                                                            #####
         #####    A FILE NAME OR A DATA FRAME AS INPUT.                           #####
         ##### AutoViz will visualize any sized file using a statistically valid sample.
         #####  - COMMA is assumed as default separator in file. But u can change it.##
-        #####  - Assumes first row as header in file but you can change it.      #####
+        #####  - Assumes first row as header in file, but you can change it.      ####
         #####  - First instantiate an AutoViz class to  hold output of charts, plots.#
         #####  - Then call the Autoviz program with inputs as defined below.       ###
         ##############################################################################
     """
+
     def __init__(self):
         self.overall = {
-        'name': 'overall',
-        'plots': [],
-        'heading': [],
-        'subheading':[],  #"\n".join(subheading)
-        'desc': [],  #"\n".join(subheading)
-        'table1_title': "",
-        'table1': [],
-        'table2_title': "",
-        'table2': []
-            }  ### This is for overall description and comments about the data set
+            'name': 'overall',
+            'plots': [],
+            'heading': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': [],  # "\n".join(subheading)
+            'table1_title': "",
+            'table1': [],
+            'table2_title': "",
+            'table2': []
+        }  ### This is for overall description and comments about the data set
         self.scatter_plot = {
-        'name': 'scatter',
-        'heading': 'Scatter Plot of each Continuous Variable against Target Variable',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': [] #"\n".join(desc)
+            'name': 'scatter',
+            'heading': 'Scatter Plot of each Continuous Variable against Target Variable',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
         }  ##### This is for description and images for scatter plots ###
         self.pair_scatter = {
-        'name': 'pair-scatter',
-        'heading': 'Pairwise Scatter Plot of each Continuous Variable against other Continuous Variables',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': []  #"\n".join(desc)
-        }   ##### This is for description and images for pairs of scatter plots ###
+            'name': 'pair-scatter',
+            'heading': 'Pairwise Scatter Plot of each Continuous Variable against other Continuous Variables',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
+        }  ##### This is for description and images for pairs of scatter plots ###
         self.dist_plot = {
-        'name': 'distribution',
-        'heading': 'Distribution Plot of Target Variable',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': []  #"\n".join(desc)
-        } ##### This is for description and images for distribution plots ###
+            'name': 'distribution',
+            'heading': 'Distribution Plot of Target Variable',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
+        }  ##### This is for description and images for distribution plots ###
         self.pivot_plot = {
-        'name': 'pivot',
-        'heading': 'Pivot Plots of all Continuous Variable',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': [] #"\n".join(desc)
-        } ##### This is for description and images for pivot  plots ###
+            'name': 'pivot',
+            'heading': 'Pivot Plots of all Continuous Variable',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
+        }  ##### This is for description and images for pivot  plots ###
         self.violin_plot = {
-        'name': 'violin',
-        'heading': 'Violin Plots of all Continuous Variable',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': [] #"\n".join(desc)
+            'name': 'violin',
+            'heading': 'Violin Plots of all Continuous Variable',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
         }  ##### This is for description and images for violin plots ###
         self.heat_map = {
-        'name': 'heatmap',
-        'heading': 'Heatmap of all Continuous Variables for target Variable',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': [] #"\n".join(desc)
-        }   ##### This is for description and images for heatmaps ###
+            'name': 'heatmap',
+            'heading': 'Heatmap of all Continuous Variables for target Variable',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
+        }  ##### This is for description and images for heatmaps ###
         self.bar_plot = {
-        'name': 'bar',
-        'heading': 'Bar Plots of Average of each Continuous Variable by Target Variable',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': [] #"\n".join(desc)
+            'name': 'bar',
+            'heading': 'Bar Plots of Average of each Continuous Variable by Target Variable',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
         }  ##### This is for description and images for bar plots ###
         self.date_plot = {
-        'name': 'time-series',
-        'heading': 'Time Series Plots of Two Continuous Variables against a Date/Time Variable',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': [] #"\n".join(desc)
+            'name': 'time-series',
+            'heading': 'Time Series Plots of Two Continuous Variables against a Date/Time Variable',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
         }  ######## This is for description and images for date time plots ###
         self.wordcloud = {
-        'name': 'wordcloud',
-        'heading': 'Word Cloud Plots of NLP or String vars',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': [] #"\n".join(desc)
+            'name': 'wordcloud',
+            'heading': 'Word Cloud Plots of NLP or String vars',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
         }  ######## This is for description and images for date time plots ###
         self.catscatter_plot = {
-        'name': 'catscatter',
-        'heading': 'Cat-Scatter  Plots of categorical vars',
-        'plots': [],
-        'subheading':[],#"\n".join(subheading)
-        'desc': [] #"\n".join(desc)
+            'name': 'catscatter',
+            'heading': 'Cat-Scatter  Plots of categorical vars',
+            'plots': [],
+            'subheading': [],  # "\n".join(subheading)
+            'desc': []  # "\n".join(desc)
         }  ######## This is for description and images for catscatter plots ###
 
-
-    def add_plots(self,plotname,X):
+    def add_plots(self, plotname, X):
         """
         This is a simple program to append the input chart to the right variable named plotname
         which is an attribute of class AV. So make sure that the plotname var matches an exact
         variable name defined in class AV. Otherwise, this will give an error.
         """
         if X is None:
             ### If there is nothing to add, leave it as it is.
-            #print("Nothing to add Plot not being added")
+            # print("Nothing to add Plot not being added")
             pass
         else:
             getattr(self, plotname)["plots"].append(X)
 
-    def add_subheading(self,plotname,X):
+    def add_subheading(self, plotname, X):
         """
         This is a simple program to append the input chart to the right variable named plotname
         which is an attribute of class AV. So make sure that the plotname var matches an exact
         variable name defined in class AV. Otherwise, this will give an error.
         """
         if X is None:
             ### If there is nothing to add, leave it as it is.
             pass
         else:
-            getattr(self,plotname)["subheading"].append(X)
+            getattr(self, plotname)["subheading"].append(X)
 
-    def AutoViz(self, filename, sep=',', depVar='', dfte=None, header=0, verbose=1,
-                            lowess=False,chart_format='svg',max_rows_analyzed=150000,
-                                max_cols_analyzed=30, save_plot_dir=None):
+    def AutoViz(self, filename: (str or pd.DataFrame), sep=',', depVar='', dfte=None, header=0, verbose=1,
+                lowess=False, chart_format='svg', max_rows_analyzed=150000,
+                max_cols_analyzed=30, save_plot_dir=None):
         """
         ##############################################################################
         ##### AUTOVIZ PERFORMS AUTOMATIC VISUALIZATION OF ANY DATA SET WITH ONE CLICK.
         #####    Give it any input file (CSV, txt or json) and AV will visualize it.##
         ##### INPUTS:                                                            #####
         #####    A FILE NAME OR A DATA FRAME AS INPUT.                           #####
         ##### AutoViz will visualize any sized file using a statistically valid sample.
         #####  - max_rows_analyzed = 150000 ### this limits the max number of rows ###
         #####           that is used to display charts                             ###
         #####  - max_cols_analyzed = 30  ### This limits the number of continuous  ###
         #####           vars that can be analyzed                                 ####
         #####  - COMMA is assumed as default separator in file. But u can change it.##
-        #####  - Assumes first row as header in file but you can change it.      #####
+        #####  - Assumes first row as header in file, but you can change it.      ####
         #####  - First instantiate an AutoViz class to  hold output of charts, plots.#
         #####  - Then call the Autoviz program with inputs as defined below.       ###
         ##############################################################################
         ##### This is the main calling program in AV. It will call all the load, #####
         ####  display and save rograms that are currently outside AV. This program ###
         ####  will draw scatter and other plots for the input data set and then   ####
         ####  call the correct variable name with add_plots function and send in  ####
@@ -243,328 +218,336 @@
         ####  This is the default.                                               #####
         ####  If verbose=1, it will print messages on the terminal and also display###
         ####  charts on terminal                                                 #####
         ####  If verbose=2, it will print messages but will not display charts,  #####
         ####  it will simply save them.                                          #####
         ##############################################################################
         """
+        if isinstance(dfte, pd.DataFrame): ### if there is a dataframe, choose it
+            filename = dfte                
+
         if isinstance(depVar, list):
-            print('Since AutoViz cannot visualize multi-label targets, choosing first item in targets: %s' %depVar[0])
-            depVar = depVar[0]
-        
-        ####################################################################################
-        if chart_format.lower() in ['bokeh','server','bokeh_server','bokeh-server', 'html']:
-            dft = AutoViz_Holo(filename, sep, depVar, dfte, header, verbose,
-                        lowess,chart_format,max_rows_analyzed,
-                            max_cols_analyzed, save_plot_dir)
+            print('Since AutoViz cannot visualize multi-label targets, choosing first item in targets: %s' % depVar[0])
+            dep_var = depVar[0]
         else:
-            dft = self.AutoViz_Main(filename, sep, depVar, dfte, header, verbose,
-                        lowess,chart_format,max_rows_analyzed,
-                            max_cols_analyzed, save_plot_dir)
+            dep_var = copy.deepcopy(depVar)
+              ####################################################################################
+        if chart_format.lower() in ['bokeh', 'server', 'bokeh_server', 'bokeh-server', 'html']:
+            dft = AutoViz_Holo(filename, sep, dep_var, header, verbose,
+                               lowess, chart_format, max_rows_analyzed,
+                               max_cols_analyzed, save_plot_dir)
+        else:
+            dft = self.AutoViz_Main(filename, sep, dep_var, header, verbose,
+                                    lowess, chart_format, max_rows_analyzed,
+                                    max_cols_analyzed, save_plot_dir)
         return dft
-    
-    def AutoViz_Main(self, filename, sep=',', depVar='', dfte=None, header=0, verbose=0,
-                            lowess=False,chart_format='svg',max_rows_analyzed=150000,
-                                max_cols_analyzed=30, save_plot_dir=None):
+
+    def AutoViz_Main(self, filename: str or pd.DataFrame, sep=',', dep_var='', header=0, verbose=0,
+                     lowess=False, chart_format='svg', max_rows_analyzed=150000,
+                     max_cols_analyzed=30, save_plot_dir=None):
         """
         ##############################################################################
         ##### AUTOVIZ_MAIN PERFORMS AUTO VISUALIZATION OF ANY DATA USING MATPLOTLIB ##
         ##############################################################################
         """
-        corr_limit = 0.8  ### This is needed to remove variables correlated above this limit
         ######### create a directory to save all plots generated by autoviz ############
         ############    THis is where you save the figures in a target directory #######
-        
-        if not depVar is None:
-            if isinstance(depVar, list):
-                target_dir = depVar[0]
-            elif isinstance(depVar, str):
-                if depVar == '':
-                    target_dir = 'AutoViz'
-                else:
-                    target_dir = copy.deepcopy(depVar)
-        else:
-            target_dir = 'AutoViz'
+        target_dir = 'AutoViz'
+
+        if dep_var is not None:
+            if isinstance(dep_var, list):
+                target_dir = dep_var[0]
+            elif isinstance(dep_var, str):
+                if dep_var != '':
+                    target_dir = copy.deepcopy(dep_var)
         if save_plot_dir is None:
-            mk_dir = os.path.join(".","AutoViz_Plots")
+            mk_dir = os.path.join(".", "AutoViz_Plots")
         else:
             mk_dir = copy.deepcopy(save_plot_dir)
         if verbose == 2 and not os.path.isdir(mk_dir):
             os.mkdir(mk_dir)
-        mk_dir = os.path.join(mk_dir,target_dir)
+        mk_dir = os.path.join(mk_dir, target_dir)
         if verbose == 2 and not os.path.isdir(mk_dir):
             os.mkdir(mk_dir)
         ############   Start the clock here and classify variables in data set first ########
         start_time = time.time()
-        
-        try:
-            dft, depVar,IDcols,bool_vars,cats,continuous_vars,discrete_string_vars,date_vars,classes,problem_type,selected_cols = classify_print_vars(
-                                                filename,sep,max_rows_analyzed, max_cols_analyzed,
-                                                depVar,dfte,header,verbose)
-        except:
-            print('Not able to read or load file. Please check your inputs and try again...')
-            return None
+
+        (dft, dep_var, id_cols, bool_vars, cats, continuous_vars, discrete_string_vars, date_vars, classes,
+         problem_type, selected_cols) = classify_print_vars(filename, sep, max_rows_analyzed, max_cols_analyzed,
+                                                            dep_var, header, verbose)
+
         ###########  This is where perform data quality checks on data ################
         if verbose >= 1:
             print('To fix these data quality issues in the dataset, import FixDQ from autoviz...')
         ####   Run the Data Cleaning suggestions report now ############
 
-        if not depVar is None:
-            if isinstance(depVar, list):
-                remaining_vars = left_subtract(list(dft), depVar)
+        if dep_var is not None:
+            if isinstance(dep_var, list):
+                remaining_vars = left_subtract(list(dft), dep_var)
                 if len(remaining_vars) == len(list(dft)):
-                    print('depVar %s not found in given dataset. Please check your input and try again' %depVar)
+                    print('depVar %s not found in given dataset. Please check your input and try again' % dep_var)
                     return dft
                 ### run the data cleaning report with a multi-label list of targets ##
-                data_cleaning_suggestions(dft, target=depVar)
+                data_cleaning_suggestions(dft, target=dep_var)
             else:
                 ### run the data cleaning report with a single-label target ##
-                data_cleaning_suggestions(dft, target=depVar)
+                data_cleaning_suggestions(dft, target=dep_var)
         else:
             ### run data cleaning report with no target ####
             data_cleaning_suggestions(dft, target='')
 
         ##### This is where we start plotting different kinds of charts depending on dependent variables
-        if depVar == None or depVar == '':
-         ##### This is when No dependent Variable is given #######
+        if dep_var is None or dep_var == '':
+            ##### This is when No dependent Variable is given #######
             if len(continuous_vars) > 1:
                 try:
-                    svg_data = draw_pair_scatters(dft,continuous_vars,problem_type,verbose,chart_format,
-                                                    depVar,classes,lowess, mk_dir)
-                    self.add_plots('pair_scatter',svg_data)
+                    svg_data = draw_pair_scatters(dft, continuous_vars, problem_type, verbose, chart_format,
+                                                  dep_var, classes, lowess, mk_dir)
+                    self.add_plots('pair_scatter', svg_data)
                 except Exception as e:
                     print(e)
                     print('Could not draw Pair Scatter Plots')
             try:
-                svg_data = draw_distplot(dft, bool_vars+cats, continuous_vars,verbose,chart_format,problem_type,
-                                    depVar,classes, mk_dir)
-                self.add_plots('dist_plot',svg_data)
-            except:
-                print('Could not draw Distribution Plot')
+                svg_data = draw_distplot(dft, bool_vars + cats, continuous_vars, verbose, chart_format, problem_type,
+                                         dep_var, classes, mk_dir)
+                self.add_plots('dist_plot', svg_data)
+            except Exception as e:
+                print(f'Could not draw Distribution Plot. {e}')
             try:
                 if len(continuous_vars) > 0:
-                    svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                    self.add_plots('violin_plot',svg_data)
+                    svg_data = draw_violinplot(dft, dep_var, continuous_vars, verbose, chart_format, problem_type,
+                                               mk_dir)
+                    self.add_plots('violin_plot', svg_data)
                 else:
                     svg_data = draw_pivot_tables(dft, problem_type, verbose,
-                        chart_format,depVar,classes, mk_dir)
-                    self.add_plots('pivot_plot',svg_data)
-            except:
-                print('Could not draw Distribution Plots')
+                                                 chart_format, dep_var, mk_dir)
+                    self.add_plots('pivot_plot', svg_data)
+            except Exception as e:
+                print(f'Could not draw Distribution Plots {e}')
             try:
-                #### Since there is no depependent variable in this dataset, you can leave it as-is
+                #### Since there is no dependent variable in this dataset, you can leave it as-is
                 numeric_cols = dft.select_dtypes(include='number').columns.tolist()
                 numeric_cols = list_difference(numeric_cols, date_vars)
-                svg_data = draw_heatmap(dft, numeric_cols, verbose,chart_format, date_vars, depVar,
-                                    problem_type,classes, mk_dir)
-                self.add_plots('heat_map',svg_data)
-            except:
-                print('Could not draw Heat Map')
+                svg_data = draw_heatmap(dft, numeric_cols, verbose, chart_format, date_vars, dep_var,
+                                        problem_type, mk_dir)
+                self.add_plots('heat_map', svg_data)
+            except Exception as e:
+                print(f'Could not draw Heat Map {e}')
             if date_vars != [] and len(continuous_vars) > 0:
                 try:
-                    svg_data = draw_date_vars(dft,depVar,date_vars,
-                                              continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                    self.add_plots('date_plot',svg_data)
-                except:
-                    print('Could not draw Date Vars')
+                    svg_data = draw_date_vars(dft, dep_var, date_vars,
+                                              continuous_vars, verbose, chart_format, problem_type, mk_dir)
+                    self.add_plots('date_plot', svg_data)
+                except Exception as e:
+                    print(f'Could not draw Date Vars {e}')
             if len(continuous_vars) > 0 and len(cats) > 0:
                 try:
-                    svg_data = draw_barplots(dft,cats,continuous_vars, problem_type,
-                                    verbose,chart_format,depVar,classes, mk_dir)
-                    self.add_plots('bar_plot',svg_data)
-                except:
-                    print('Could not draw Bar Plots')
+                    svg_data = draw_barplots(dft, cats, continuous_vars, problem_type,
+                                             verbose, chart_format, dep_var, mk_dir)
+                    self.add_plots('bar_plot', svg_data)
+                except Exception as e:
+                    print(f'Could not draw Bar Plots {e}')
             else:
                 if len(cats) > 1:
                     try:
-                        svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
-                                    chart_format, mk_dir=None)
-                        self.add_plots('catscatter_plot',svg_data)
-                    except:
-                        print ('Could not draw catscatter plots...')
+                        svg_data = draw_catscatterplots(dft, cats, verbose,
+                                                        chart_format, mk_dir=None)
+                        self.add_plots('catscatter_plot', svg_data)
+                    except Exception as e:
+                        print(f'Could not draw catscatter plots. {e}')
         else:
-            if problem_type=='Regression':
+            if problem_type == 'Regression':
                 ############## This is a Regression Problem #################
                 if len(continuous_vars) > 0:
                     try:
                         svg_data = draw_scatters(dft,
-                                        continuous_vars,verbose,chart_format,problem_type,depVar,classes,lowess, mk_dir)
-                        self.add_plots('scatter_plot',svg_data)
+                                                 continuous_vars, verbose, chart_format, problem_type, dep_var, classes,
+                                                 lowess, mk_dir)
+                        self.add_plots('scatter_plot', svg_data)
                     except Exception as e:
                         print("Exception Drawing Scatter Plots")
                         print(e)
                         traceback.print_exc()
                         print('Could not draw Scatter Plots')
                 if len(continuous_vars) > 1:
                     try:
-                        svg_data = draw_pair_scatters(dft,continuous_vars,problem_type,verbose,chart_format,
-                                                        depVar,classes,lowess, mk_dir)
-                        self.add_plots('pair_scatter',svg_data)
-                    except:
-                        print('Could not draw Pair Scatter Plots')
+                        svg_data = draw_pair_scatters(dft, continuous_vars, problem_type, verbose, chart_format,
+                                                      dep_var, classes, lowess, mk_dir)
+                        self.add_plots('pair_scatter', svg_data)
+                    except Exception as e:
+                        print(f'Could not draw Pair Scatter Plots {e}')
                 try:
-                    if type(depVar) == str:
-                        othernums = [x for x in continuous_vars if x not in [depVar]]
+                    if type(dep_var) == str:
+                        othernums = [x for x in continuous_vars if x not in [dep_var]]
                     else:
-                        othernums = [x for x in continuous_vars if x not in depVar]
+                        othernums = [x for x in continuous_vars if x not in dep_var]
                     if len(othernums) >= 1:
-                        svg_data = draw_distplot(dft, bool_vars+cats, continuous_vars,verbose,chart_format,
-                                            problem_type, depVar, classes, mk_dir)
-                        self.add_plots('dist_plot',svg_data)
-                except:
-                    print('Could not draw some Distribution Plots')
+                        svg_data = draw_distplot(dft, bool_vars + cats, continuous_vars, verbose, chart_format,
+                                                 problem_type, dep_var, classes, mk_dir)
+                        self.add_plots('dist_plot', svg_data)
+                except Exception as e:
+                    print(f'Could not draw some Distribution Plots {e}')
                 try:
                     if len(continuous_vars) > 0:
-                        svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                        self.add_plots('violin_plot',svg_data)
-                except:
-                    print('Could not draw Violin Plots')
+                        svg_data = draw_violinplot(dft, dep_var, continuous_vars, verbose, chart_format, problem_type,
+                                                   mk_dir)
+                        self.add_plots('violin_plot', svg_data)
+                except Exception as e:
+                    print(f'Could not draw Violin Plots {e}')
                 try:
-                    numeric_cols = [x for x in dft.select_dtypes(include='number').columns.tolist() if x not in [depVar]]
+                    numeric_cols = [x for x in dft.select_dtypes(include='number').columns.tolist() if
+                                    x not in [dep_var]]
                     numeric_cols = list_difference(numeric_cols, date_vars)
                     svg_data = draw_heatmap(dft,
-                                        numeric_cols, verbose,chart_format, date_vars, depVar,
-                                            problem_type, classes, mk_dir)
-                    self.add_plots('heat_map',svg_data)
-                except:
-                    print('Could not draw some Heat Maps')
+                                            numeric_cols, verbose, chart_format, date_vars, dep_var,
+                                            problem_type, mk_dir)
+                    self.add_plots('heat_map', svg_data)
+                except Exception as e:
+                    print(f'Could not draw some Heat Maps {e}')
                 if date_vars != [] and len(continuous_vars) > 0:
                     try:
                         svg_data = draw_date_vars(
-                            dft,depVar,date_vars,continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                        self.add_plots('date_plot',svg_data)
-                    except:
-                        print('Could not draw some Time Series plots')
+                            dft, dep_var, date_vars, continuous_vars, verbose, chart_format, problem_type, mk_dir)
+                        self.add_plots('date_plot', svg_data)
+                    except Exception as e:
+                        print(f'Could not draw some Time Series plots. {e}')
                 if len(cats) > 0 and len(continuous_vars) == 0:
                     ### This is somewhat duplicative with distplot (above) - hence do it only minimally!
                     try:
                         svg_data = draw_pivot_tables(dft, problem_type, verbose,
-                            chart_format,depVar,classes, mk_dir)
-                        self.add_plots('pivot_plot',svg_data)
-                    except:
-                        print('Could not draw some Pivot Charts against Dependent Variable')
+                                                     chart_format, dep_var, mk_dir)
+                        self.add_plots('pivot_plot', svg_data)
+                    except Exception as e:
+                        print(f'Could not draw some Pivot Charts against Dependent Variable {e}')
                 if len(continuous_vars) > 0 and len(cats) > 0:
                     try:
-                        svg_data = draw_barplots(dft, find_remove_duplicates(cats+bool_vars),continuous_vars,
-                                                    problem_type, verbose,chart_format,depVar,classes, mk_dir)
-                        self.add_plots('bar_plot',svg_data)
-                        #self.add_plots('bar_plot',None)
-                    except:
-                        print('Could not draw some Bar Charts')
+                        svg_data = draw_barplots(dft, find_remove_duplicates(cats + bool_vars), continuous_vars,
+                                                 problem_type, verbose, chart_format, dep_var, mk_dir)
+                        self.add_plots('bar_plot', svg_data)
+                        # self.add_plots('bar_plot',None)
+                    except Exception as e:
+                        print(f'Could not draw some Bar Charts {e}')
                 else:
                     if len(cats) > 1:
                         try:
-                            svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
-                                        chart_format, mk_dir=None)
-                            self.add_plots('catscatter_plot',svg_data)
-                        except:
-                            print ('Could not draw catscatter plots...')
-            else :
+                            svg_data = draw_catscatterplots(dft, cats, verbose,
+                                                            chart_format, mk_dir=None)
+                            self.add_plots('catscatter_plot', svg_data)
+                        except Exception as e:
+                            print(f'Could not draw catscatter plots... {e}')
+            else:
                 ############ This is a Classification Problem ##################
                 if len(continuous_vars) > 0:
                     try:
-                        svg_data = draw_scatters(dft,continuous_vars,
-                                                 verbose,chart_format,problem_type,depVar, classes,lowess, mk_dir)
-                        self.add_plots('scatter_plot',svg_data)
+                        svg_data = draw_scatters(dft, continuous_vars,
+                                                 verbose, chart_format, problem_type, dep_var, classes, lowess, mk_dir)
+                        self.add_plots('scatter_plot', svg_data)
                     except Exception as e:
                         print(e)
                         traceback.print_exc()
                         print('Could not draw some Scatter Plots')
                 if len(continuous_vars) > 1:
                     try:
-                        svg_data = draw_pair_scatters(dft,continuous_vars,
-                                                      problem_type,verbose,chart_format,depVar,classes,lowess, mk_dir)
-                        self.add_plots('pair_scatter',svg_data)
-                    except:
-                        print('Could not draw some Pair Scatter Plots')
+                        svg_data = draw_pair_scatters(dft, continuous_vars,
+                                                      problem_type, verbose, chart_format, dep_var, classes, lowess,
+                                                      mk_dir)
+                        self.add_plots('pair_scatter', svg_data)
+                    except Exception as e:
+                        print(f'Could not draw some Pair Scatter Plots {e}')
                 try:
-                    if type(depVar) == str:
-                        othernums = [x for x in continuous_vars if x not in [depVar]]
+                    if type(dep_var) == str:
+                        othernums = [x for x in continuous_vars if x not in [dep_var]]
                     else:
-                        othernums = [x for x in continuous_vars if x not in depVar]
+                        othernums = [x for x in continuous_vars if x not in dep_var]
 
                     if len(othernums) >= 1:
-                        svg_data = draw_distplot(dft, bool_vars+cats, continuous_vars,verbose,chart_format,
-                                                problem_type,depVar,classes, mk_dir)
-                        self.add_plots('dist_plot',svg_data)
+                        svg_data = draw_distplot(dft, bool_vars + cats, continuous_vars, verbose, chart_format,
+                                                 problem_type, dep_var, classes, mk_dir)
+                        self.add_plots('dist_plot', svg_data)
                     else:
                         print('No continuous var in data set: drawing categorical distribution plots')
-                except:
-                    print('Could not draw some Distribution Plots')
+                except Exception as e:
+                    print(f'Could not draw some Distribution Plots {e}')
                 try:
                     if len(continuous_vars) > 0:
-                        svg_data = draw_violinplot(dft,depVar,continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                        self.add_plots('violin_plot',svg_data)
-                except:
-                    print('Could not draw some Violin Plots')
+                        svg_data = draw_violinplot(dft, dep_var, continuous_vars, verbose, chart_format, problem_type,
+                                                   mk_dir)
+                        self.add_plots('violin_plot', svg_data)
+                except Exception as e:
+                    print(f'Could not draw some Violin Plots {e}')
                 try:
-                    numeric_cols = [x for x in dft.select_dtypes(include='number').columns.tolist() if x not in [depVar]]
+                    numeric_cols = [x for x in dft.select_dtypes(include='number').columns.tolist() if
+                                    x not in [dep_var]]
                     numeric_cols = list_difference(numeric_cols, date_vars)
                     svg_data = draw_heatmap(dft, numeric_cols,
-                                            verbose,chart_format, date_vars, depVar,problem_type,
-                                            classes, mk_dir)
-                    self.add_plots('heat_map',svg_data)
-                except:
-                    print('Could not draw some Heat Maps')
+                                            verbose, chart_format, date_vars, dep_var, problem_type,
+                                            mk_dir)
+                    self.add_plots('heat_map', svg_data)
+                except Exception as e:
+                    print(f'Could not draw some Heat Maps {e}')
                 if date_vars != [] and len(continuous_vars) > 0:
                     try:
-                        svg_data = draw_date_vars(dft,depVar,date_vars,
-                                                  continuous_vars,verbose,chart_format,problem_type, mk_dir)
-                        self.add_plots('date_plot',svg_data)
-                    except:
-                        print('Could not draw some Time Series plots')
+                        svg_data = draw_date_vars(dft, dep_var, date_vars,
+                                                  continuous_vars, verbose, chart_format, problem_type, mk_dir)
+                        self.add_plots('date_plot', svg_data)
+                    except Exception as e:
+                        print(f'Could not draw some Time Series plots. {e}')
                 if len(cats) > 0 and len(continuous_vars) == 0:
                     ### This is somewhat duplicative with distplot (above) - hence do it only minimally!
                     try:
                         svg_data = draw_pivot_tables(dft, problem_type, verbose,
-                                        chart_format,depVar,classes, mk_dir)
-                        self.add_plots('pivot_plot',svg_data)
-                    except:
-                        print('Could not draw some Pivot Charts against Dependent Variable')
+                                                     chart_format, dep_var, mk_dir)
+                        self.add_plots('pivot_plot', svg_data)
+                    except Exception as e:
+                        print(f'Could not draw some Pivot Charts against Dependent Variable {e}')
                 if len(continuous_vars) > 0 and len(cats) > 0:
                     try:
-                        svg_data = draw_barplots(dft,find_remove_duplicates(cats+bool_vars),continuous_vars,problem_type,
-                                        verbose,chart_format, depVar, classes, mk_dir)
-                        self.add_plots('bar_plot',svg_data)
+                        svg_data = draw_barplots(dft, find_remove_duplicates(cats + bool_vars), continuous_vars,
+                                                 problem_type,
+                                                 verbose, chart_format, dep_var, mk_dir)
+                        self.add_plots('bar_plot', svg_data)
                         pass
-                    except:
+                    except Exception as e:
                         if verbose <= 1:
-                            print('Could not draw some Bar Charts')
+                            print(f'Could not draw some Bar Charts {e}')
                         pass
                 else:
                     if len(cats) > 1:
                         try:
-                            svg_data = draw_catscatterplots(dft,cats, problem_type, verbose, 
-                                        chart_format, mk_dir=None)
-                            self.add_plots('catscatter_plot',svg_data)
-                        except:
-                            print ('Could not draw catscatter plots...')
+                            svg_data = draw_catscatterplots(dft, cats, verbose,
+                                                            chart_format, mk_dir=None)
+                            self.add_plots('catscatter_plot', svg_data)
+                        except Exception as e:
+                            print(f'Could not draw catscatter plots. {e}')
         ###### Now you can check for NLP vars or discrete_string_vars to do wordcloud #######
         if len(discrete_string_vars) > 0:
             plotname = 'wordcloud'
             import nltk
             nltk.download('popular')
             for each_string_var in discrete_string_vars:
                 try:
-                    svg_data = draw_word_clouds(dft, each_string_var, chart_format, plotname, 
-                                    depVar, problem_type, classes, mk_dir, verbose=0)
-                    self.add_plots(plotname,svg_data)
-                except:
-                    print('Could not draw wordcloud plot for %s' %each_string_var)
+                    svg_data = draw_word_clouds(dft, each_string_var, chart_format, plotname,
+                                                dep_var, problem_type, classes, mk_dir, verbose=0)
+                    self.add_plots(plotname, svg_data)
+                except Exception as e:
+                    print(f'Could not draw wordcloud plot for {each_string_var}. {e}')
         ### Now print the time taken to run charts for AutoViz #############
         if verbose <= 1:
             print('All Plots done')
         else:
-            print('All Plots are saved in %s' %mk_dir)
-        print('Time to run AutoViz = %0.0f seconds ' %(time.time()-start_time))
+            print('All Plots are saved in %s' % mk_dir)
+        print('Time to run AutoViz = %0.0f seconds ' % (time.time() - start_time))
         if verbose <= 1:
-            print ('\n ###################### AUTO VISUALIZATION Completed ########################')
+            print('\n ###################### AUTO VISUALIZATION Completed ########################')
         return dft
+
+
 #############################################################################################
-from pandas_dq import Fix_DQ
+
+
 # Create a new class FixDQ by inheriting from Fix_DQ
 class FixDQ(Fix_DQ):
     """
     FixDQ is a great way to clean an entire train data set and apply the same steps in 
     an MLOps pipeline to a test dataset. FixDQ can be used to detect most issues in 
     your data (similar to data_cleaning_suggestions but without the `target` 
     related issues) in one step. Then it fixes those issues it finds during the 
@@ -585,32 +568,35 @@
         It detects high cardinality features but leaves them as it is.
         It detects highly correlated features and drops one of them (whichever 
                     comes first in the column sequence)
         It detects duplicate rows and drops one of them or keeps only one copy 
                     of duplicate rows
         It detects duplicate columns and drops one of them or keeps only one copy
         It detects skewed distributions and applies log or box-cox 
-                    transformations on them
+                    transformations on them.
         It detects imbalanced classes and leaves them as it is
         It detects feature leakage and drops one of those features if 
                     they are highly correlated to target
     """
-    def __init__(self, quantile=0.87, cat_fill_value = 'missing', 
-                num_fill_value = 9999, rare_threshold = 0.01, 
-                correlation_threshold = 0.9):
+
+    def __init__(self, quantile=0.87, cat_fill_value='missing',
+                 num_fill_value=9999, rare_threshold=0.01,
+                 correlation_threshold=0.9):
         super().__init__()  # Call the parent class constructor
         # Additional initialization code here
         self.quantile = quantile
         self.cat_fill_value = cat_fill_value
         self.num_fill_value = num_fill_value
         self.rare_threshold = rare_threshold
         self.correlation_threshold = correlation_threshold
 
+
 ###################################################################################
-from pandas_dq import dq_report
+
+
 def data_cleaning_suggestions(df, target=None):
     """
     This is a simple program to give data cleaning and improvement suggestions in class AV.
     Make sure you send in a dataframe. Otherwise, this will give an error.
     """
     if isinstance(df, pd.DataFrame):
         dqr = dq_report(data=df, target=target, html=False, csv_engine="pandas", verbose=1)
```

### Comparing `autoviz-0.1.903/autoviz/AutoViz_Holo.py` & `autoviz-0.1.904/autoviz/AutoViz_Holo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,148 +1,152 @@
-######################### AutoViz New with HoloViews ############################
+from holoviews.ipython import display
+
+from autoviz.AutoViz_Utils import classify_print_vars, find_remove_duplicates
 import numpy as np
 import pandas as pd
-############# Import from autoviz.AutoViz_Class the following libraries #######
-from autoviz.AutoViz_Utils import *
-##############   make sure you use: conda install -c pyviz hvplot ###############
-import copy
-####################################################################################
-#### The warnings from Sklearn are so annoying that I have to shut it off ####
 import warnings
+
 warnings.filterwarnings("ignore")
+
+
 def warn(*args, **kwargs):
     pass
+
+
 warnings.warn = warn
 ########################################
 import logging
+
 logging.getLogger("param").setLevel(logging.ERROR)
-import warnings 
+import warnings
 from sklearn.exceptions import DataConversionWarning
+
 warnings.filterwarnings("ignore")
 ### These Bokeh warnings are useless => leave them alone for now!
 ### from bokeh.util.warnings import BokehUserWarning
 ## warnings.simplefilter(action='ignore', category=BokehUserWarning) 
 warnings.filterwarnings(action='ignore', category=DataConversionWarning)
 ####################################################################################
 import matplotlib
+
 matplotlib.use('agg')
-import matplotlib.pyplot as plt
 # from matplotlib import io
 import io
 import seaborn as sns
+
 sns.set(style="whitegrid", color_codes=True)
-import re
-import pdb
-import pprint
-import matplotlib
-#matplotlib.style.use('fivethirtyeight')
-from itertools import cycle, combinations
-from collections import defaultdict
+# matplotlib.style.use('fivethirtyeight')
+from itertools import cycle
 import copy
 import time
-import sys
-import random
-import xlrd
-import statsmodels
 from io import BytesIO
 import base64
-from functools import reduce
-import traceback
-import xgboost as xgb
-from xgboost.sklearn import XGBClassifier
-from xgboost.sklearn import XGBRegressor
 import os
 # If specific functions/classes are needed from your own modules
-from .classify_method import classify_columns
+
+
 ##########################################################################################
 def ensure_hvplot_imported():
     global hv, opts, pn, pnw, INLINE
     try:
         # Import main modules
         import hvplot.pandas
         import holoviews as hv
         import panel as pn
         from bokeh.resources import INLINE
-        from bokeh.util.warnings import BokehUserWarning 
+        from bokeh.util.warnings import BokehUserWarning
 
         # Import submodules and specific components
         from holoviews import opts
         import panel.widgets as pnw
         import holoviews.plotting.bokeh
 
         # Set the extension
         hv.extension('bokeh', 'matplotlib')
 
     except ImportError as e:
         raise ImportError(f"An error occurred while importing: {str(e)}")
+
+
 ######################################################################################
 ##### Now you can use hv, opts, pn, etc. in your modules 
 ######################################################################################
 ######## This is where we store the image data in a dictionary with a list of images #########
-def save_image_data_hv(fig, chart_count, chart_format):
+def save_image_data_hv(fig, chart_format):
     if chart_format == 'svg':
         ###### You have to add these lines to each function that creates charts currently ##
         imgdata = io.StringIO()
         fig.savefig(imgdata, format=chart_format)
         imgdata.seek(0)
         svg_data = imgdata.getvalue()
         return svg_data
-    elif chart_format in ['png','jpg']:
+    elif chart_format in ['png', 'jpg']:
         ### You have to do it slightly differently for PNG and JPEG formats
         imgdata = BytesIO()
         fig.savefig(imgdata, format=chart_format, bbox_inches='tight', pad_inches=0.0)
         imgdata.seek(0)
         figdata_png = base64.b64encode(imgdata.getvalue())
         return figdata_png
+
+
 ##############  This is where we save panels that we create to HTML ############
 def save_html_data(hv_all, chart_format, plot_name, mk_dir, additional=''):
     ensure_hvplot_imported()
-    print('Saving %s in HTML format' %(plot_name+additional))
+    print('Saving %s in HTML format' % (plot_name + additional))
     if not os.path.isdir(mk_dir):
         os.mkdir(mk_dir)
     if additional == '':
-        filename = os.path.join(mk_dir,plot_name+"."+chart_format)
+        filename = os.path.join(mk_dir, plot_name + "." + chart_format)
     else:
-        filename = os.path.join(mk_dir,plot_name+additional+"."+chart_format)
+        filename = os.path.join(mk_dir, plot_name + additional + "." + chart_format)
     ## it is amazing you can save interactive plots ##
     ## You don't need the resources = INLINE since it would consume too much space in HTML plots
-    #pn.panel(hv_all).save(filename, embed=True, resources=INLINE) 
+    # pn.panel(hv_all).save(filename, embed=True, resources=INLINE)
     pn.panel(hv_all).save(filename, embed=True)
 
+
 ##############  This is where we append panels that we create ############
 def append_panels(hv_panel, imgdata_list, chart_format):
     imgdata_list.append(hv.output(hv_panel, backend='bokeh', fig=chart_format))
     return imgdata_list
+
+
 ###### Display on Jupyter Notebook or on the Server ########
 def display_dmap(dmap):
     ensure_hvplot_imported()
     renderer = hv.renderer('bokeh')
     #### You must have a Dynamic Map dmap to render these Bokeh objects on Servers
-    app = renderer.app(dmap)
+    renderer.app(dmap)
     server = renderer.app(dmap, show=True, new_window=True)
     return server
+
+
 ####################################################################################
 def display_obj(dmap_in):
     ensure_hvplot_imported()
     ### This is to render the chart in a web server to display as a dashboard!!
     renderer = hv.renderer('bokeh')
     #### You must have a Dynamic Map dmap to render these Bokeh objects on Servers
-    app = renderer.app(dmap_in)
+    renderer.app(dmap_in)
     server = renderer.app(dmap_in, show=True, new_window=True)
     display(server)
+
+
 ####################################################################################
 def display_server(dmap):
     ensure_hvplot_imported()
     #### You must have a Dynamic Map dmap to render these Bokeh objects on Servers
     server = pn.serve(dmap, start=True, show=False)
     return server
+
+
 ##############################  This is the beginning of the new AutoViz_Holo ###################
-def AutoViz_Holo(filename, sep=',', depVar='', dfte=None, header=0, verbose=0,
-                        lowess=False,chart_format='svg',max_rows_analyzed=150000,
-                            max_cols_analyzed=30, save_plot_dir=None):
+def AutoViz_Holo(filename, sep=',', depVar='', header=0, verbose=0,
+                 lowess=False, chart_format='svg', max_rows_analyzed=150000,
+                 max_cols_analyzed=30, save_plot_dir=None):
     """
     ##############################################################################
     ##### AUTOVIZ_HOLO PERFORMS AUTO VISUALIZATION OF ANY DATA SET USING BOKEH. ##
     #####    Give it any input file (CSV, txt or json) and AV will visualize it.##
     ##### INPUTS:                                                            #####
     #####    A FILE NAME OR A DATA FRAME AS INPUT.                           #####
     ##### AutoViz will visualize any sized file using a statistically valid sample.
@@ -164,54 +168,54 @@
     ##############################################################################
     """
     ####################################################################################
     corr_limit = 0.7  ### This is needed to remove variables correlated above this limit
     ######### create a directory to save all plots generated by autoviz ############
     ############    THis is where you save the figures in a target directory #######
     target_dir = 'AutoViz'
-    if not depVar is None:
+    if depVar is not None:
         if depVar != '':
             target_dir = copy.deepcopy(depVar)
     if save_plot_dir is None:
-        mk_dir = os.path.join(".","AutoViz_Plots")
+        mk_dir = os.path.join(".", "AutoViz_Plots")
     else:
         mk_dir = copy.deepcopy(save_plot_dir)
     if chart_format == 'html' and not os.path.isdir(mk_dir):
         os.mkdir(mk_dir)
-    mk_dir = os.path.join(mk_dir,target_dir)
+    mk_dir = os.path.join(mk_dir, target_dir)
     if chart_format == 'html' and not os.path.isdir(mk_dir):
         os.mkdir(mk_dir)
     ############   Start the clock here and classify variables in data set first ########
     start_time = time.time()
     try:
-        dfin, dep,IDcols,bool_vars,cats,nums,discrete_string_vars,date_vars,classes,problem_type,selected_cols = classify_print_vars(
-                                            filename,sep,max_rows_analyzed, max_cols_analyzed,
-                                            depVar,dfte,header,verbose)
-    except:
-        print('Not able to read or load file. Please check your inputs and try again...')
+        (dfin, dep, IDcols, bool_vars, cats, nums, discrete_string_vars, date_vars, classes, problem_type,
+         selected_cols) = classify_print_vars(filename, sep, max_rows_analyzed, max_cols_analyzed,
+                                              depVar, header, verbose)
+    except Exception as e:
+        print(f'Not able to read or load file. Please check your inputs and try again... {e}')
         return None
     #################   This is where the differentiated HoloViews code begins ####
     ls_objects = []
     imgdata_list = list()
     height_size = 400
     width_size = 500
-    
+
     ##########    Now start drawing the Bokeh Plots ###############################
     if len(nums) > 0:
         if problem_type == 'Clustering':
             #### There is no need to do a scatter plot with a dep variable when no dependent variable is given
             print('No scatter plots with depVar when no depVar is given.')
         else:
-            drawobj1 = draw_scatters_hv(dfin,nums,chart_format,problem_type,
-                          dep, classes, lowess, mk_dir, verbose)
+            drawobj1 = draw_scatters_hv(dfin, nums, chart_format, problem_type,
+                                        dep, classes, lowess, mk_dir, verbose)
             ls_objects.append(drawobj1)
         ### You can draw pair scatters only if there are 2 or more numeric variables ####
         if len(nums) >= 2:
             drawobj2 = draw_pair_scatters_hv(dfin, nums, problem_type, chart_format, dep,
-                           classes, lowess, mk_dir, verbose)
+                                             classes, lowess, mk_dir, verbose)
             ls_objects.append(drawobj2)
     drawobj3 = draw_distplot_hv(dfin, cats, nums, chart_format, problem_type, dep, classes, mk_dir, verbose)
     ls_objects.append(drawobj3)
     ### kdeplot is the only time you send in ls_objects since it has to be returned with 2 objects ###
     try:
         #### This KDE draws only the distribution of the target variable!
         drawobj4 = draw_kdeplot_hv(dfin, cats, nums, chart_format, problem_type, dep, ls_objects, mk_dir, verbose)
@@ -226,24 +230,26 @@
         ls_objects.append(drawobj5)
     if len(nums) > 0:
         #### Adding int vars to nums since pandas has changed the df.corr() to error when cats are included ###
         if len(cats) > 0:
             nums_in = nums + dfin[cats].select_dtypes(include="number").columns.tolist()
         else:
             nums_in = nums[:]
-        drawobj6 = draw_heatmap_hv(dfin, nums_in, chart_format, date_vars, dep, problem_type, classes, 
-                            mk_dir, verbose)
+        drawobj6 = draw_heatmap_hv(dfin, nums_in, chart_format, date_vars, dep, problem_type, classes,
+                                   mk_dir, verbose)
         ls_objects.append(drawobj6)
     if len(date_vars) > 0:
-        drawobj7 = draw_date_vars_hv(dfin,dep,date_vars, nums, chart_format, problem_type, mk_dir, verbose)
+        drawobj7 = draw_date_vars_hv(dfin, dep, date_vars, nums, chart_format, problem_type, mk_dir, verbose)
         ls_objects.append(drawobj7)
     if len(nums) > 0 and len(cats) > 0:
         drawobj8 = draw_cat_vars_hv(dfin, dep, nums, cats, chart_format, problem_type, mk_dir, verbose)
-    print('Time to run AutoViz (in seconds) = %0.0f' %(time.time()-start_time))
+    print('Time to run AutoViz (in seconds) = %0.0f' % (time.time() - start_time))
     return dfin
+
+
 ####################################################################################
 def draw_cat_vars_hv(dfin, dep, nums, cats, chart_format, problem_type, mk_dir, verbose=0):
     ensure_hvplot_imported()
     ######## SCATTER PLOTS ARE USEFUL FOR COMPARING NUMERIC VARIABLES
     ##### we are going to modify dfin and classes, so we are making copies to make changes
     dft = copy.deepcopy(dfin)
     image_count = 0
@@ -278,116 +284,124 @@
         else:
             cats += dep
             cats = find_remove_duplicates(cats)
     ### This is where you draw the widgets #####################
     quantileable = [x for x in nums if len(dft[x].unique()) > 20]
     if len(quantileable) <= 1:
         quantileable = [x for x in nums if len(dft[x].unique()) > 2]
-    cmap_list = ['Blues','rainbow', 'viridis', 'plasma', 'inferno', 'magma', 'cividis']
+    cmap_list = ['Blues', 'rainbow', 'viridis', 'plasma', 'inferno', 'magma', 'cividis']
     ### The X axis should be cat vars and the Y axis should be numeric vars ######
     x = pnw.Select(name='X-Axis', value=cats[0], options=cats)
     y = pnw.Select(name='Y-Axis', value=quantileable[0], options=quantileable)
-    ## you need to decorate this function with depends to make the widgets change axes real time ##
-    @pn.depends(x.param.value, y.param.value) 
-    def create_figure(x, y):
-        #opts = dict(cmap=cmap_list[0], line_color='black')
+
+    # you need to decorate this function with depends to make the widgets change axes real time ##
+    @pn.depends(x.param.value, y.param.value)
+    def create_figure(x, figure_y):
+        # opts = dict(cmap=cmap_list[0], line_color='black')
         opts = dict(width=width_size, height=height_size, line_color='black',
-                xrotation=70, title='Average of each numeric var by categorical var')
+                    xrotation=70, title='Average of each numeric var by categorical var')
         ### If it is None, don't stack it
         opts['color'] = next(colors)
         opts['alpha'] = alpha
         opts['tools'] = ['hover']
         opts['toolbar'] = 'above'
         opts['colorbar'] = True
-        conti_df = dft[[x,y]].groupby(x).mean().reset_index()
+        conti_df = dft[[x, figure_y]].groupby(x).mean().reset_index()
         return hv.Bars(conti_df).opts(**opts)
 
     widgets = pn.WidgetBox(x, y)
 
-    hv_panel = pn.Row(widgets, create_figure).servable('Cross-selector')    
+    hv_panel = pn.Row(widgets, create_figure).servable('Cross-selector')
     #####################################################
     ##### Save all the chart objects here ##############
     if verbose == 2:
         imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
         image_count += 1
     if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-        #server = pn.serve(hv_panel, start=True, show=True)
-        print('%s can be found in URL below:' %plot_name)
+        # server = pn.serve(hv_panel, start=True, show=True)
+        print('%s can be found in URL below:' % plot_name)
         hv_panel.show()
     elif chart_format == 'html':
         save_html_data(hv_panel, chart_format, plot_name, mk_dir)
     else:
-        display(hv_panel)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
+        display(
+            hv_panel)  ## This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
     return hv_panel
+
+
 #####################################################################################################
 def draw_kdeplot_hv(dfin, cats, nums, chart_format, problem_type, dep, ls_objects, mk_dir, verbose=0):
     ensure_hvplot_imported()
     dft = copy.deepcopy(dfin)
     image_count = 0
     imgdata_list = list()
     N = len(nums)
     cols = 2
     plot_name = 'kde_plots'
     width_size = 600
     height_size = 400
     hv_all = None
     transparent = 0.5
-    color='lightblue'
+    color = 'lightblue'
+
     ########################################################################################
     def return_dynamic_objects(dfout, dep, title='Distribution of Target variable'):
         width_size = 600
         height_size = 400
         pdf1 = pd.DataFrame(dfout[dep].value_counts().reset_index())
         pdf2 = pd.DataFrame(dfout[dep].value_counts(1).reset_index())
         drawobj41 = pdf1.hvplot(kind='bar', color='lightblue', title=title).opts(
-                        height=height_size, width=width_size,xrotation=70)
+            height=height_size, width=width_size, xrotation=70)
         drawobj42 = pdf2.hvplot(kind='bar', color='lightgreen', title=title)
-        return (drawobj41+drawobj42)
-    
+        return drawobj41 + drawobj42
+
     if problem_type.endswith('Classification'):
         colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
         dmap = hv.DynamicMap(return_dynamic_objects(dfin, dep, title='Percent Distribution of Target variable'
-                        ).opts(shared_axes=False).opts(title='Histogram and KDE of Target = %s' %dep)).opts(
-                            height=height_size, width=width_size)
-        dmap.opts(framewise=True,axiswise=True) ## both must be True for your charts to have dynamically varying axes!
-        hv_all = pn.pane.HoloViews(dmap)#, sizing_mode="stretch_both")
-        #ls_objects.append(drawobj41)
-        #ls_objects.append(drawobj42)
+                                                    ).opts(shared_axes=False).opts(
+            title='Histogram and KDE of Target = %s' % dep)).opts(
+            height=height_size, width=width_size)
+        dmap.opts(framewise=True, axiswise=True)  ## both must be True for your charts to have dynamically varying axes!
+        hv_all = pn.pane.HoloViews(dmap)  # , sizing_mode="stretch_both")
+        # ls_objects.append(drawobj41)
+        # ls_objects.append(drawobj42)
     else:
         if not isinstance(dep, list):
             ### it means dep is a string ###
             if dep == '':
                 ### there is no target variable to draw ######
                 return ls_objects
             else:
                 dmap = hv.Distribution(dfin[dep]).opts(color=color,
-                                        height=height_size, width=width_size, alpha=transparent,
-                                    title='KDE (Distribution) Plot of Target Variable')
+                                                       height=height_size, width=width_size, alpha=transparent,
+                                                       title='KDE (Distribution) Plot of Target Variable')
                 hv_all = pn.pane.HoloViews(dmap)
-                #ls_objects.append(drawobj41)
-                #ls_objects.append(drawobj42)
+                # ls_objects.append(drawobj41)
+                # ls_objects.append(drawobj42)
     #### In this case we are using multiple objects in panel ###
     ##### Save all the chart objects here ##############
     if verbose == 2:
         imgdata_list = append_panels(hv_all, imgdata_list, chart_format)
         image_count += 1
     if chart_format.lower() in ['server', 'bokeh_server', 'bokeh-server']:
         ### If you want it on a server, you use drawobj.show()
-        #(drawobj41+drawobj42).show()
-        print('%s can be found in URL below:' %plot_name)
+        # (drawobj41+drawobj42).show()
+        print('%s can be found in URL below:' % plot_name)
         server = pn.serve(hv_all, start=True, show=True)
     elif chart_format == 'html':
         save_html_data(hv_all, chart_format, plot_name, mk_dir)
     else:
         ### This will display it in a Jupyter Notebook.
         display(hv_all)
     return ls_objects
+
+
 #####################################################################################################
 def draw_scatters_hv(dft, nums, chart_format, problem_type,
-                  dep=None, classes=None, lowess=False, mk_dir='AutoViz_Plots', verbose=0):
+                     dep=None, classes=None, lowess=False, mk_dir='AutoViz_Plots', verbose=0):
     ensure_hvplot_imported()
     ######## SCATTER PLOTS ARE USEFUL FOR COMPARING NUMERIC VARIABLES
     ##### we are going to modify dfin and classes, so we are making copies to make changes
     dft = copy.deepcopy(dft)
     image_count = 0
     imgdata_list = list()
     classes = copy.deepcopy(classes)
@@ -406,113 +420,87 @@
     hv_panel = None
     #####################################################
     if problem_type == 'Regression':
         ####### This is a Regression Problem #### You need to plot a Scatter plot ####
         ####### First, Plot each Continuous variable against the Target Variable ###
         ######   This is a Very Simple Way to build an Scatter Chart with One Variable as a Select Variable #######
         alpha = 0.5
+
         def load_symbol(symbol, **kwargs):
             color = next(colors)
-            return hv.Scatter((dft[symbol].values,dft[dep].values)).opts(framewise=True).opts(size=bubble_size,
-                    color=color, alpha=alpha, height=height_size, width=width_size).opts(
-                    xlabel='%s' %symbol).opts(ylabel='%s' %dep).opts(
-                   title='Scatter Plot of %s against %s variable' %(symbol,dep))
+            return hv.Scatter((dft[symbol].values, dft[dep].values)).opts(framewise=True).opts(size=bubble_size,
+                                                                                               color=color, alpha=alpha,
+                                                                                               height=height_size,
+                                                                                               width=width_size).opts(
+                xlabel='%s' % symbol).opts(ylabel='%s' % dep).opts(
+                title='Scatter Plot of %s against %s variable' % (symbol, dep))
+
         ### This is where you create the dynamic map and pass it the variable to load the chart!
-        dmap = hv.DynamicMap(load_symbol, kdims='Select_Variable').redim.values(Select_Variable=nums).opts(framewise=True)
+        dmap = hv.DynamicMap(load_symbol, kdims='Select_Variable').redim.values(Select_Variable=nums).opts(
+            framewise=True)
         ###########  This is where you put the Panel Together ############
         hv_panel = pn.panel(dmap)
         widgets = hv_panel[0]
         hv_all = pn.Column(pn.Row(*widgets))
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
     else:
-        ##################################################################################################################
-        ####### This is a Classification Problem #### You need to plot a Scatter plot ####
-        #######   This widget based code works well except it does not add jitter. But it changes y-axis so that's good!
-        ##################################################################################################################
+        ###############################################################################################################
+        # This is a Classification Problem #### You need to plot a Scatter plot ####
+        # This widget based code works well except it does not add jitter. But it changes y-axis so that's good!
+        ###############################################################################################################
         x = pn.widgets.Select(name='x', options=[dep])
         y = pn.widgets.Select(name='y', options=nums)
-        @pn.depends(x.param.value, y.param.value) 
-        def create_figure(x, y):
+
+        @pn.depends(x.param.value, y.param.value)
+        def create_figure(figure_x, figure_y):
             opts = dict(cmap=cmap_list[0], width=width_size, height=height_size, line_color='black')
             opts['color'] = next(colors)
             opts['size'] = bubble_size
             opts['alpha'] = alpha
             opts['tools'] = ['hover']
             opts['toolbar'] = 'above'
             opts['colorbar'] = True
-            opts['title'] ='Scatter Plot of each numeric variable against target variable'
-            return hv.Scatter(dft, [x, y], label="%s vs %s" % (x.title(), y.title()),
-                ).opts(**opts)
+            opts['title'] = 'Scatter Plot of each numeric variable against target variable'
+            return hv.Scatter(dft, [figure_x, figure_y], label="%s vs %s" % (figure_x.title(), figure_y.title()),
+                              ).opts(**opts)
 
         widgets = pn.WidgetBox(x, y)
 
         hv_all = pn.Row(widgets, create_figure).servable('Cross-selector')
         #############  This is the old way of doing it - but it wasn't pretty ################
-        #target_vars = dft[dep].unique()
-        #x = pn.widgets.Select(name='x', options=nums)
+        # target_vars = dft[dep].unique()
+        # x = pn.widgets.Select(name='x', options=nums)
         y = pn.widgets.Select(name='y', options=nums)
         kind = pn.widgets.Select(name='kind', value='scatter', options=['scatter'])
-        #######  This is where you call the widget and pass it the hv_plotto draw a Chart #######
-        #hv_plot = dft.hvplot(x=dep, y=y, kind=kind, height=height_size, width=width_size, size=bubble_size,color = next(colors),
-        #                title='Scatter Plot of each independent numeric variable against target variable')
-        #hv_panel = pn.panel(hv_plot)
-        #hv_all = pn.Row(pn.WidgetBox(y), hv_plot)
-        ##
-        ##################################################################################################################
-        #############   This works well except that the y-axis does not change when you switch y-variable ################
-        ##################################################################################################################
-        #target_vars = dft[dep].unique().tolist()
-        #color_list = list(colortext[:len(target_vars)])
-        #def select_widget(Select_numeric_variable):
-        #    """
-        #    This program must take in a variable passed from the widget and turn it into a chart.
-        #    The input is known as select_variable and it is the variable you must use to get the data and build a chart.
-        #    The output must return a HoloViews Chart.
-        #    """
-        #    hv_string = ''
-        #    target_list = np.unique(dfin[dep].values)
-        #    lowerbound = dfin[Select_numeric_variable].min()
-        #    upperbound = dfin[Select_numeric_variable].max()
-        #    for each_t in target_list:
-        #        if not isinstance(each_t, str):
-        #            each_ts = str(each_t) 
-        #        else:
-        #            each_ts = copy.deepcopy(each_t)
-        #        next_color = next(colors)
-        #        #add_string = "hv.Scatter((dfin[dfin['"+dep+"']=="+each_ts+"]['"+dep+"'].values,dfin[dfin['"+dep+"']=="+each_ts+"]['"+Select_numeric_variable+"'].values)).opts(color='"+next_color+"',jitter=eval('"+str(jitter)+"'),alpha=eval('"+str(alpha)+"'),size=eval('"+str(bubble_size)+"'),height=eval('"+str(height_size)+"'),width=eval('"+str(width_size)+"'))"
-        #        add_string = "hv.Scatter((dfin[dfin['"+dep+"']=="+each_ts+"]['"+dep+"'].values,dfin[dfin['"+dep+"']=="+each_ts+"]['"+Select_numeric_variable+"'].values)).opts(color='"+next_color+"',jitter=eval('"+str(jitter)+"'),alpha=eval('"+str(alpha)+"'),ylim=(eval('"+str(lowerbound)+"'),eval('"+str(upperbound)+"')),height=eval('"+str(height_size)+"'),width=eval('"+str(width_size)+"'))"
-        #        hv_string += add_string + " * "
-        #    return eval(hv_string[:-2]).opts(
-        #            legend_position='top_left',title='Scatter Plot of each Numeric Variable against Target variable')
-        #######  This is where you call the widget and pass it the select_variable to draw a Chart #######
-        #########   This is for bokeh server only ##############
-        #dmap = hv.DynamicMap(select_widget,  kdims=['Select_numeric_variable']).redim.values(Select_numeric_variable=nums).opts(framewise=True)
-        ###########  This is where you put the Panel Together ############
-        #hv_panel = pn.panel(dmap)
-        #widgets = hv_panel[0]
-        #hv_all = pn.Column(pn.Row(*widgets))
-        ###########  E N D    O F     Y- A X I S    C O D E    ############
+        # ######  This is where you call the widget and pass it the hv_plotto draw a Chart ####### hv_plot =
+        # dft.hvplot(x=dep, y=y, kind=kind, height=height_size, width=width_size, size=bubble_size,color = next(
+        # colors), title='Scatter Plot of each independent numeric variable against target variable') hv_panel =
+        # pn.panel(hv_plot) hv_all = pn.Row(pn.WidgetBox(y), hv_plot) #
+        # ################################################################################################################# ############   This works well except that the y-axis does not change when you switch y-variable ################ ################################################################################################################# target_vars = dft[dep].unique().tolist() color_list = list(colortext[:len(target_vars)]) def select_widget(Select_numeric_variable): """ This program must take in a variable passed from the widget and turn it into a chart. The input is known as select_variable and it is the variable you must use to get the data and build a chart. The output must return a HoloViews Chart. """ hv_string = '' target_list = np.unique(dfin[dep].values) lowerbound = dfin[Select_numeric_variable].min() upperbound = dfin[Select_numeric_variable].max() for each_t in target_list: if not isinstance(each_t, str): each_ts = str(each_t) else: each_ts = copy.deepcopy(each_t) next_color = next(colors) #add_string = "hv.Scatter((dfin[dfin['"+dep+"']=="+each_ts+"]['"+dep+"'].values,dfin[dfin['"+dep+"']=="+each_ts+"]['"+Select_numeric_variable+"'].values)).opts(color='"+next_color+"',jitter=eval('"+str(jitter)+"'),alpha=eval('"+str(alpha)+"'),size=eval('"+str(bubble_size)+"'),height=eval('"+str(height_size)+"'),width=eval('"+str(width_size)+"'))" add_string = "hv.Scatter((dfin[dfin['"+dep+"']=="+each_ts+"]['"+dep+"'].values,dfin[dfin['"+dep+"']=="+each_ts+"]['"+Select_numeric_variable+"'].values)).opts(color='"+next_color+"',jitter=eval('"+str(jitter)+"'),alpha=eval('"+str(alpha)+"'),ylim=(eval('"+str(lowerbound)+"'),eval('"+str(upperbound)+"')),height=eval('"+str(height_size)+"'),width=eval('"+str(width_size)+"'))" hv_string += add_string + " * " return eval(hv_string[:-2]).opts( legend_position='top_left',title='Scatter Plot of each Numeric Variable against Target variable') ######  This is where you call the widget and pass it the select_variable to draw a Chart ####### ########   This is for bokeh server only ############## dmap = hv.DynamicMap(select_widget,  kdims=['Select_numeric_variable']).redim.values(Select_numeric_variable=nums).opts(framewise=True) ##########  This is where you put the Panel Together ############ hv_panel = pn.panel(dmap) widgets = hv_panel[0] hv_all = pn.Column(pn.Row(*widgets)) ##########  E N D    O F     Y- A X I S    C O D E    ############
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
     ####### End of Scatter Plots ######
     if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-        #server = pn.serve(hv_all, start=True, show=True)
-        print('%s can be found in URL below:' %plot_name)
+        # server = pn.serve(hv_all, start=True, show=True)
+        print('%s can be found in URL below:' % plot_name)
         hv_all.show()
     elif chart_format == 'html':
         save_html_data(hv_all, chart_format, plot_name, mk_dir)
     else:
-        display(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
+        display(
+            hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
     return hv_all
+
+
 #######################################################################################
-def draw_pair_scatters_hv(dfin,nums,problem_type,chart_format, dep=None,
-                       classes=None, lowess=False, mk_dir='AutoViz_Plots', verbose=0):
+def draw_pair_scatters_hv(dfin, nums, problem_type, chart_format, dep=None,
+                          classes=None, lowess=False, mk_dir='AutoViz_Plots', verbose=0):
     """
     #### PAIR SCATTER PLOTS ARE NEEDED ONLY FOR CLASSIFICATION PROBLEMS IN NUMERIC VARIABLES
     ### This is where you plot a pair-wise scatter plot of Independent Variables against each other####
     """
     ensure_hvplot_imported()
     dft = dfin[:]
     image_count = 0
@@ -532,339 +520,370 @@
     if problem_type in ['Regression', 'Clustering']:
         ########## This is for Regression problems ##########
         #########  Here we plot a pair-wise scatter plot of Independent Variables ####
         ### Only 1 color is needed since only 2 vars are plotted against each other ##
         ################################################################################################
         #####  This widgetbox code works but it doesn't change the x- and y-axis when you change variables
         ################################################################################################
-        #x = pn.widgets.Select(name='x', options=nums)
-        #y = pn.widgets.Select(name='y', options=nums)
-        #kind = pn.widgets.Select(name='kind', value='scatter', options=['bivariate', 'scatter'])
+        # x = pn.widgets.Select(name='x', options=nums)
+        # y = pn.widgets.Select(name='y', options=nums)
+        # kind = pn.widgets.Select(name='kind', value='scatter', options=['bivariate', 'scatter'])
         ### Let us say you want to change the range of the x axis 
         ## - Then you can explicitly set the limits and it works!
-        #xlimi = (dft[x.value].min(), dft[x.value].max())
-        #ylimi = (dft[y.value].min(), dft[y.value].max())
-        #plot = dft.hvplot(x=x, y=y, kind=kind,  color=next(colors), alpha=0.5, xlim=xlimi, ylim=ylimi,
+        # xlimi = (dft[x.value].min(), dft[x.value].max())
+        # ylimi = (dft[y.value].min(), dft[y.value].max())
+        # plot = dft.hvplot(x=x, y=y, kind=kind,  color=next(colors), alpha=0.5, xlim=xlimi, ylim=ylimi,
         #            title='Pair-wise Scatter Plot of two Independent Numeric variables')
-        #hv_panel = pn.Row(pn.WidgetBox(x, y, kind),plot)
+        # hv_panel = pn.Row(pn.WidgetBox(x, y, kind),plot)
         ########################   This is the new way of drawing scatter   ###############################
-        
+
         quantileable = [x for x in nums if len(dft[x].unique()) > 20]
         if len(quantileable) <= 1:
             quantileable = [x for x in nums if len(dft[x].unique()) > 2]
-        
+
         x = pnw.Select(name='X-Axis', value=quantileable[0], options=quantileable)
         y = pnw.Select(name='Y-Axis', value=quantileable[1], options=quantileable)
         size = pnw.Select(name='Size', value='None', options=['None'] + quantileable)
         if problem_type == 'Clustering':
             ### There is no depVar in clustering, so no need to add it to None
             color = pnw.Select(name='Color', value='None', options=['None'])
         else:
             color = pnw.Select(name='Color', value='None', options=['None', dep])
+
         ## you need to decorate this function with depends to make the widgets change axes real time ##
-        @pn.depends(x.param.value, y.param.value, color.param.value) 
-        def create_figure(x, y, color):
-            opts = dict(cmap=cmap_list[0], width=width_size, height=height_size, line_color='black')
-            if color != 'None':
-                opts['color'] = color 
-            opts['size'] = bubble_size
-            opts['alpha'] = alpha
-            opts['tools'] = ['hover']
-            opts['toolbar'] = 'above'
-            opts['colorbar'] = True
-            opts['title'] ='Pair-wise Scatter Plot of two Independent Numeric variables'
-            return hv.Points(dft, [x, y], label="%s vs %s" % (x.title(), y.title()),
-                ).opts(**opts)
+        @pn.depends(x.param.value, y.param.value, color.param.value)
+        def create_figure(x, figure_y, figure_color):
+            figure_opts = dict(cmap=cmap_list[0], width=width_size, height=height_size, line_color='black')
+            if figure_color != 'None':
+                figure_opts['color'] = figure_color
+            figure_opts['size'] = bubble_size
+            figure_opts['alpha'] = alpha
+            figure_opts['tools'] = ['hover']
+            figure_opts['toolbar'] = 'above'
+            figure_opts['colorbar'] = True
+            figure_opts['title'] = 'Pair-wise Scatter Plot of two Independent Numeric variables'
+            return hv.Points(dft, [x, figure_y], label="%s vs %s" % (x.title(), figure_y.title()),
+                             ).opts(**figure_opts)
 
         widgets = pn.WidgetBox(x, y, color)
 
         hv_panel = pn.Row(widgets, create_figure).servable('Cross-selector')
         ########################   This is the old way of drawing scatter  ################################
-        #colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
-        #def load_symbol(symbol, variable, **kwargs):
+        # colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
+        # def load_symbol(symbol, variable, **kwargs):
         #    color = next(colors)
         #    return hv.Scatter((dft[symbol].values,dft[variable].values)).opts(framewise=True).opts(size=5,
         #            color=color, alpha=alpha, height=height_size, width=width_size).opts(
         #            xlabel='%s' %symbol).opts(ylabel='%s' %variable).opts(
         #           title='Scatter Plot of %s against %s variable' %(symbol,variable))
         ### This is where you create the dynamic map and pass it the variable to load the chart!
-        #dmap = hv.DynamicMap(load_symbol, kdims=['Select_X','Select_Y']).redim.values(Select_X=nums, Select_Y=nums).opts(framewise=True)
+        # dmap = hv.DynamicMap(load_symbol, kdims=['Select_X','Select_Y']).redim.values(Select_X=nums, Select_Y=nums).opts(framewise=True)
         ###########  This is where you put the Panel Together ############
-        #hv_panel = pn.panel(dmap)
-        #widgets = hv_panel[0]
-        #hv_panel = pn.Column(pn.Row(*widgets))
+        # hv_panel = pn.panel(dmap)
+        # widgets = hv_panel[0]
+        # hv_panel = pn.Column(pn.Row(*widgets))
         ########################   End of the old way of drawing scatter  ################################
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
     else:
         ########## This is for Classification problems ##########
         #########  This is the new way to plot a pair-wise scatter plot ####
         quantileable = [x for x in nums if len(dft[x].unique()) > 20]
         if len(quantileable) <= 1:
             quantileable = [x for x in nums if len(dft[x].unique()) > 2]
 
         x = pnw.Select(name='X-Axis', value=quantileable[0], options=quantileable)
         y = pnw.Select(name='Y-Axis', value=quantileable[1], options=quantileable)
         size = pnw.Select(name='Size', value='None', options=['None'] + quantileable)
-        color = pnw.Select(name='Color', value='None', options=['None',dep])
+        color = pnw.Select(name='Color', value='None', options=['None', dep])
 
-        @pn.depends(x.param.value, y.param.value, color.param.value) 
-        def create_figure(x, y, color):
-            opts = dict(cmap=cmap_list[0], width=width_size, height=height_size, line_color='black')
-            if color != 'None':
-                opts['color'] = color
+        @pn.depends(x.param.value, y.param.value, color.param.value)
+        def create_figure(x, figure_y, figure_color):
+            figure_opts = dict(cmap=cmap_list[0], width=width_size, height=height_size, line_color='black')
+            if figure_color != 'None':
+                figure_opts['color'] = figure_color
             else:
-                opts['color'] = next(colors)
-            opts['size'] = bubble_size
-            opts['alpha'] = alpha
-            opts['tools'] = ['hover']
-            opts['toolbar'] = 'above'
-            opts['colorbar'] = True
-            opts['title'] ='Pair-wise Scatter Plot of two Independent Numeric variables'
-            return hv.Points(dft, [x, y], label="%s vs %s" % (x.title(), y.title()),
-                ).opts(**opts)
+                figure_opts['color'] = next(colors)
+            figure_opts['size'] = bubble_size
+            figure_opts['alpha'] = alpha
+            figure_opts['tools'] = ['hover']
+            figure_opts['toolbar'] = 'above'
+            figure_opts['colorbar'] = True
+            figure_opts['title'] = 'Pair-wise Scatter Plot of two Independent Numeric variables'
+            return hv.Points(dft, [x, figure_y], label="%s vs %s" % (x.title(), figure_y.title()),
+                             ).opts(**figure_opts)
 
         widgets = pn.WidgetBox(x, y, color)
 
         hv_panel = pn.Row(widgets, create_figure).servable('Cross-selector')
         #########  This is an old way to plot a pair-wise scatter plot ####
-        #target_vars = dft[dep].unique()
-        #x = pn.widgets.Select(name='x', options=nums)
-        #y = pn.widgets.Select(name='y', options=nums)
-        #kind = pn.widgets.Select(name='kind', value='scatter', options=['bivariate', 'scatter'])
+        # target_vars = dft[dep].unique()
+        # x = pn.widgets.Select(name='x', options=nums)
+        # y = pn.widgets.Select(name='y', options=nums)
+        # kind = pn.widgets.Select(name='kind', value='scatter', options=['bivariate', 'scatter'])
 
-        #plot = dft.hvplot(x=x, y=y, kind=kind, by=dep, height=height_size, alpha=0.5,
+        # plot = dft.hvplot(x=x, y=y, kind=kind, by=dep, height=height_size, alpha=0.5,
         #                title='Pair-wise Scatter Plot of two Independent Numeric variables')
-        #hv_panel = pn.Row(pn.WidgetBox(x, y, kind), plot)
+        # hv_panel = pn.Row(pn.WidgetBox(x, y, kind), plot)
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
     ####### End of Pair Scatter Plots ######
     if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-        #server = pn.serve(hv_panel, start=True, show=True)
-        print('%s can be found in URL below:' %plot_name)
+        # server = pn.serve(hv_panel, start=True, show=True)
+        print('%s can be found in URL below:' % plot_name)
         hv_panel.show()
     elif chart_format == 'html':
         save_html_data(hv_panel, chart_format, plot_name, mk_dir)
     else:
-        display(hv_panel)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
+        display(
+            hv_panel)  # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
     return hv_panel
+
+
 ##################################################################################
 ##### Draw the Distribution of each variable using Distplot
 ##### Must do this only for Continuous Variables
-def draw_distplot_hv(dft, cats, conti, chart_format,problem_type,dep=None, 
-                    classes=None, mk_dir='AutoViz_Plots', verbose=0):
+def draw_distplot_hv(dft, cats, conti, chart_format, problem_type, dep=None,
+                     classes=None, mk_dir='AutoViz_Plots', verbose=0):
     ensure_hvplot_imported()
     dft = copy.deepcopy(dft)
     image_count = 0
     imgdata_list = list()
     #### Since we are making changes to dft and classes, we will be making copies of it here
     conti = list(set(conti))
     nums = copy.deepcopy(conti)
     classes = copy.deepcopy(classes)
     colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
     imgdata_list = list()
     width_size = 600  #### this is to control the width of chart as well as number of categories to display
     height_size = 400
-    gap = 0.4 #### This controls the space between rows  ######
+    gap = 0.4  #### This controls the space between rows  ######
     plot_name = 'distplots'
     hv_all = None
     ###################################################################################
-    if dep==None or dep=='' or problem_type == 'Regression':
+    if dep is None or dep == '' or problem_type == 'Regression':
         ######### This is for Regression problems only ########
         transparent = 0.7
         binsize = 30
         ### Be very careful with the next 2 lines: we want to fill NA with 0 in numeric vars
-        for each_conti,k in zip(conti,range(len(conti))):
+        for each_conti, k in zip(conti, range(len(conti))):
             if dft[each_conti].isnull().sum() > 0:
                 ### Remember that fillna only works at dataframe level! ###
                 dft[[each_conti]] = dft[[each_conti]].fillna(0)
         ## In this case, we perform this only if we have Cat variables
         if not isinstance(dep, list):
             ### it means dep is a string ###
             if dep == '':
                 pass
             elif len(cats) > 0:
                 colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
+
                 def select_widget(each_cat):
                     """
                     This program must take in a variable passed from the widget and turn it into a chart.
-                    The input is known as each_cat and it is the variable you must use to get the data and build a chart.
+                    The input is known as each_cat and is the variable you must use to get the data and build a chart.
                     The output must return a HoloViews Chart.
                     """
-                    width_size=15
+                    width_size = 15
                     #######  This is where you plot the histogram of categorical variable input as each_cat ####
-                    conti_df = dft[[dep,each_cat]].groupby(each_cat).mean().reset_index()
+                    conti_df = dft[[dep, each_cat]].groupby(each_cat).mean().reset_index()
                     row_ticks = dft[dep].unique().tolist()
                     color_list = next(colors)
                     pivotdf = pd.DataFrame(conti_df.to_records()).set_index(each_cat)
-                    plot = pivotdf.hvplot(kind='bar',stacked=False,use_index=False, color=color_list,
-                                          title='Mean Target = %s by each Categorical Variable' %dep).opts(xrotation=70)
+                    plot = pivotdf.hvplot(kind='bar', stacked=False, use_index=False, color=color_list,
+                                          title='Mean Target = %s by each Categorical Variable' % dep).opts(
+                        xrotation=70)
                     return plot
+
                 #######  This is where you call the widget and pass it the select_variable to draw a Chart #######
-                dmap = hv.DynamicMap(select_widget,  kdims=['Select_Cat_Variable']).redim.values(Select_Cat_Variable=cats)
-                dmap.opts(framewise=True,axiswise=True) ## both must be True for your charts to have dynamically varying axes!
+                dmap = hv.DynamicMap(select_widget, kdims=['Select_Cat_Variable']).redim.values(
+                    Select_Cat_Variable=cats)
+                dmap.opts(framewise=True,
+                          axiswise=True)  ## both must be True for your charts to have dynamically varying axes!
                 ###########  This is where you put the Panel Together ############
                 hv_panel = pn.panel(dmap)
                 widgets = hv_panel[0]
                 hv_all = pn.Column(pn.Row(*widgets))
                 if verbose == 2:
                     imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
                     image_count += 1
                 if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-                    #server = pn.serve(hv_all, start=True, show=True)
-                    print('%s can be found in URL below:' %plot_name)
+                    # server = pn.serve(hv_all, start=True, show=True)
+                    print('%s can be found in URL below:' % plot_name)
                     hv_all.show()
                 elif chart_format == 'html':
                     save_html_data(hv_all, chart_format, plot_name, mk_dir, additional="_cats")
                 else:
-                    display(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
-                    #display_obj(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+                    display(
+                        hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+                    # display_obj(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
         if len(conti) > 0:
             try:
-                ######   This is a Very Complex Way to build an ND Overlay Chart with One Variable as a Select Variable #######
+                # This is a Very Complex Way to build an ND Overlay Chart with One Variable as a Select Variable
                 jitter = 0.5
                 colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
                 transparent = 0.5
+
                 def select_variable_to_plot(num_var):
                     """
                     This program must take in a variable passed from the widget and turn it into a chart.
                     The input is known as num_var and it is the variable you must use to get the data and build a chart.
                     The output must return a HoloViews Chart.
                     """
                     color = next(colors)
                     xlimi = (dft[num_var].min(), dft[num_var].max())
                     hv_look = hv.Distribution(np.histogram(dft[num_var]), num_var).opts(color=color,
-                                        height=height_size, width=width_size, alpha=transparent,
-                                    title='KDE (Distribution) Plot of Numeric Variables').redim.range(num_var=xlimi)
+                                                                                        height=height_size,
+                                                                                        width=width_size,
+                                                                                        alpha=transparent,
+                                                                                        title='KDE (Distribution) Plot of Numeric Variables').redim.range(
+                        num_var=xlimi)
                     return hv_look
+
                 #######  This is where you call the widget and pass it the select_variable to draw a Chart #######
-                dmap = hv.DynamicMap(select_variable_to_plot,  kdims=['Select_Variable']).redim.values(Select_Variable=nums)
-                dmap.opts(framewise=True,axiswise=True) ## both must be True for your charts to have dynamically varying axes!
+                dmap = hv.DynamicMap(select_variable_to_plot, kdims=['Select_Variable']).redim.values(
+                    Select_Variable=nums)
+                dmap.opts(framewise=True,
+                          axiswise=True)  ## both must be True for your charts to have dynamically varying axes!
                 ###########  This is where you put the Panel Together ############
                 hv_panel = pn.panel(dmap)
                 widgets = hv_panel[0]
                 hv_all = pn.Column(pn.Row(*widgets))
             except:
                 print('Error in Distribution Plot')
                 hv_panel = []
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
         if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-            #server = pn.serve(hv_all, start=True, show=True)
-            print('%s can be found in URL below:' %plot_name)
+            # server = pn.serve(hv_all, start=True, show=True)
+            print('%s can be found in URL below:' % plot_name)
             hv_all.show()
         elif chart_format == 'html':
             save_html_data(hv_all, chart_format, plot_name, mk_dir, additional="_nums")
         else:
-            display(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
-            #display_obj(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+            display(hv_all)
+            # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+            # display_obj(hv_all)
+            # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
     else:
         ######### This is for Classification problems only ########
         transparent = 0.7
         binsize = 30
         alpha = 0.5
         height_size = 400
         width_size = 600
         ### Be very careful with the next 2 lines: we want to fill NA with 0 in numeric vars
         target_vars = dft[dep].unique().tolist()
-        if type(classes[0])==int:
+        if type(classes[0]) == int:
             classes = [str(x) for x in classes]
-        for each_conti,k in zip(conti,range(len(conti))):
+        for each_conti, k in zip(conti, range(len(conti))):
             if dft[each_conti].isnull().sum() > 0:
                 ## fillna only works on a dataframe level - it also doesnt do inplace! ###
                 dft[[each_conti]] = dft[[each_conti]].fillna(0)
         if len(cats) > 0:
             def select_widget(Select_categorical_var):
                 """
                 This program must take in a variable passed from the widget and turn it into a chart.
                 The input is known as num_var and it is the variable you must use to get the data and build a chart.
                 The output must return a HoloViews Chart.
                 """
                 colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
                 #######  This is where you plot the histogram of categorical variable input as each_cat ####
-                conti_df = dft[[dep,Select_categorical_var]].groupby([dep,Select_categorical_var]).size().nlargest(
-                                    width_size).reset_index(name='Values')
+                conti_df = dft[[dep, Select_categorical_var]].groupby([dep, Select_categorical_var]).size().nlargest(
+                    width_size).reset_index(name='Values')
                 pivot_df = conti_df.pivot(index=Select_categorical_var, columns=dep, values='Values').fillna(0)
                 row_ticks = dft[dep].unique().tolist()
                 color_list = []
                 for i in range(len(row_ticks)):
                     color_list.append(next(colors))
                 pivotdf = pd.DataFrame(pivot_df.to_records()).set_index(Select_categorical_var)
-                plot = pivotdf.hvplot(kind='bar',stacked=True,use_index=True,
-                            title='Target = %s Histogram by each Categorical Variable' %dep).opts(
-                                height=height_size,width=width_size, xrotation=70)
+                plot = pivotdf.hvplot(kind='bar', stacked=True, use_index=True,
+                                      title='Target = %s Histogram by each Categorical Variable' % dep).opts(
+                    height=height_size, width=width_size, xrotation=70)
                 return plot
+
             #######  This is where you call the widget and pass it the select_variable to draw a Chart #######
-            dmap = hv.DynamicMap(select_widget,  kdims=['Select_categorical_var']).redim.values(
-                                                Select_categorical_var=cats)
+            dmap = hv.DynamicMap(select_widget, kdims=['Select_categorical_var']).redim.values(
+                Select_categorical_var=cats)
             ###########  This is where you put the Panel Together ############
             hv_panel = pn.panel(dmap)
             widgets = hv_panel[0]
             hv_all = pn.Column(pn.Row(*widgets))
             if verbose == 2:
                 imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
                 image_count += 1
             if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-                #server = pn.serve(hv_all, start=True, show=True)
-                print('%s can be found in URL below:' %plot_name)
+                # server = pn.serve(hv_all, start=True, show=True)
+                print('%s can be found in URL below:' % plot_name)
                 hv_all.show()
             elif chart_format == 'html':
                 save_html_data(hv_all, chart_format, plot_name, mk_dir, additional="_cats")
             else:
-                display(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
-                #display_obj(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+                display(hv_all)
+                # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+                # display_obj(hv_all)
+                # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
         if len(conti) > 0:
             try:
                 ######   This is a Very Complex Way to build an ND Overlay Chart with One Variable as a Select Variable #######
                 colortext = 'brycgkbyrcmgkbyrcmgkbyrcmgkbyr'
                 target_vars = dft[dep].unique().tolist()
                 color_list = list(colortext[:len(target_vars)])
                 jitter = 0.5
                 colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
                 transparent = 0.5
+
                 def select_widget(Select_numeric_variable):
                     """
                     This program must take in a variable passed from the widget and turn it into a chart.
                     The input is known as num_var and it is the variable you must use to get the data and build a chart.
                     The output must return a HoloViews Chart.
                     """
                     color = next(colors)
-                    overlay = hv.NdOverlay({group: hv.Distribution(np.histogram(dft[dft[dep]==group][Select_numeric_variable].values)) for i,group in enumerate(target_vars)})
+                    overlay = hv.NdOverlay(
+                        {group: hv.Distribution(np.histogram(dft[dft[dep] == group][Select_numeric_variable].values))
+                         for i, group in enumerate(target_vars)})
                     hv_look = overlay.opts(opts.Distribution(alpha=0.5, height=height_size, width=width_size)).opts(
                         title='KDE (Distribution) Plots of all Numeric Variables by Classes').opts(
-                        xlabel='%s' %dep).opts(ylabel='%s' %Select_numeric_variable)
+                        xlabel='%s' % dep).opts(ylabel='%s' % Select_numeric_variable)
                     return hv_look
+
                 #######  This is where you call the widget and pass it the select_variable to draw a Chart #######
-                dmap = hv.DynamicMap(select_widget,  kdims=['Select_numeric_variable']).redim.values(Select_numeric_variable=nums)
+                dmap = hv.DynamicMap(select_widget, kdims=['Select_numeric_variable']).redim.values(
+                    Select_numeric_variable=nums)
                 ###########  This is where you put the Panel Together ############
                 hv_panel = pn.panel(dmap)
                 widgets = hv_panel[0]
                 hv_all = pn.Column(pn.Row(*widgets))
             except:
                 print('Error in Distribution Plot')
             if verbose == 2:
                 imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
                 image_count += 1
             if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-                #server = pn.serve(hv_all, start=True, show=True)
-                print('%s can be found in URL below:' %plot_name)
+                # server = pn.serve(hv_all, start=True, show=True)
+                print('%s can be found in URL below:' % plot_name)
                 hv_all.show()
             elif chart_format == 'html':
                 save_html_data(hv_all, chart_format, plot_name, mk_dir, additional="_nums")
             else:
-                display(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
-                #display_obj(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+                display(hv_all)
+                # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+                # display_obj(hv_all)
+                # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
     ####### End of Distplots ###########
     return hv_all
+
+
 ##################################################################################
-def draw_violinplot_hv(dft, dep, nums,chart_format, modeltype='Regression', 
-                    mk_dir='AutoViz_Plots', verbose=0):
+def draw_violinplot_hv(dft, dep, nums, chart_format, modeltype='Regression',
+                       mk_dir='AutoViz_Plots', verbose=0):
     ensure_hvplot_imported()
     dft = copy.deepcopy(dft)
     image_count = 0
     imgdata_list = list()
     width_size = 800
     height_size = 500
     if type(dep) == str:
@@ -880,122 +899,127 @@
         number_in_each_row = 30
         cmap_list = ["#75968f", "#a5bab7", "#c9d9d3", "#e2e2e2", "#dfccce", "#ddb7b1", "#cc7878", "#933b41", "#550b1d"]
         ###### This is for looping over variables 10 at a time only ##########################
         df_p = dft[nums]
         if df_p.shape[1] < number_in_each_row:
             iter_limit = number_in_each_row
         else:
-            iter_limit = max(number_in_each_row, int(df_p.shape[1]/5+0.5))
-        #print('Current number of Numeric Variables = %d ' %(df_p.shape[1],))
+            iter_limit = max(number_in_each_row, int(df_p.shape[1] / 5 + 0.5))
+        # print('Current number of Numeric Variables = %d ' %(df_p.shape[1],))
         ###### This is for looping over variables 10 at a time only ##########################
-        drawobjv_list = [] ## this keeps track of the actual values
-        drawobj_list = [] ## this keeps track of the names
+        drawobjv_list = []  ## this keeps track of the actual values
+        drawobj_list = []  ## this keeps track of the names
         counter = 0
         string_size = 10
-        for i in range(0,df_p.shape[1],iter_limit):
-            new_end = i+iter_limit
-            #print('i = ',i,"new end = ", new_end)
+        for i in range(0, df_p.shape[1], iter_limit):
+            new_end = i + iter_limit
+            # print('i = ',i,"new end = ", new_end)
             if i == 0:
-                title_string = 'using first %d variables...' %(iter_limit)
-                #print(title_string )
+                title_string = 'using first %d variables...' % iter_limit
+                # print(title_string )
             else:
-                title_string = 'using next %d variables...' %(iter_limit)
-                #print(title_string )
+                title_string = 'using next %d variables...' % iter_limit
+                # print(title_string )
             conti = nums[i:new_end]
             ######################### Add Standard Scaling here ##################################
             short_conti = [x[:string_size] for x in conti]
             from sklearn.preprocessing import StandardScaler
             SS = StandardScaler()
-            data = pd.DataFrame(SS.fit_transform(dft[conti]),columns=short_conti)
-            var_name = 'drawobjv_list['+str(counter)+']'
+            data = pd.DataFrame(SS.fit_transform(dft[conti]), columns=short_conti)
+            var_name = 'drawobjv_list[' + str(counter) + ']'
             drawobj_list.append(var_name)
             drawobjv_list.append(var_name)
-            drawobj = data.hvplot(kind='violin', label='Violin Plot %s (Standard Scaled)' %title_string,
-                                   rot=70  #height=height_size,width=width_size
-                                 )
+            drawobj = data.hvplot(kind='violin', label='Violin Plot %s (Standard Scaled)' % title_string,
+                                  rot=70  # height=height_size,width=width_size
+                                  )
             drawobjv_list[counter] = drawobj
             counter += 1
         ######### After collecting all the drawobjv's put them in a dynamic map and display them ###
-        combined_charts = "("+"".join([x+'+' for x in drawobj_list])[:-1]+")"
-        hv_all = pn.panel(eval(combined_charts))        #### This is where we add them to the list ######        
+        combined_charts = "(" + "".join([x + '+' for x in drawobj_list])[:-1] + ")"
+        hv_all = pn.panel(eval(combined_charts))  #### This is where we add them to the list ######
         if verbose == 2:
             imgdata_list = append_panels(hv_all, imgdata_list, chart_format)
             image_count += 1
         #### In the case of violin plots, you have to create multiple tabs or plots ###
         if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-            print('%s can be found in URL below:' %plot_name)
+            print('%s can be found in URL below:' % plot_name)
             server = pn.serve(hv_all, start=True, show=True)
-            #hv_all.show()  ### for some reason .show errors in violin plots
+            # hv_all.show()  ### for some reason .show errors in violin plots
         elif chart_format == 'html':
             save_html_data(hv_all, chart_format, plot_name, mk_dir)
         else:
-            display(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
-            #display_obj(hv_all)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+            display(hv_all)
+            # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+            # display_obj(hv_all)
+            # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
     else:
         #### This is for Classification problems ###################
         number_in_each_row = 30
         df_p = dft[nums]
         if df_p.shape[1] < number_in_each_row:
             iter_limit = number_in_each_row
         else:
-            iter_limit = max(number_in_each_row, int(df_p.shape[1]/5+0.5))
+            iter_limit = max(number_in_each_row, int(df_p.shape[1] / 5 + 0.5))
         ###### This is for looping over variables 10 at a time only ##########################
         target_vars = np.unique(dft[dep])
         dmaps = []
         combined_charts = ''
         counter = 0
-        drawobjv_list = [] ## this keeps track of the actual values
-        drawobj_list = [] ## this keeps track of the names
+        drawobjv_list = []  ## this keeps track of the actual values
+        drawobj_list = []  ## this keeps track of the names
         for symbol in target_vars:
             color = next(colors)
-            sup_title = 'Violin Plot for %s = %s' %(dep,symbol)
-            for i in range(0,df_p.shape[1],iter_limit):
-                new_end = i+iter_limit
+            sup_title = 'Violin Plot for %s = %s' % (dep, symbol)
+            for i in range(0, df_p.shape[1], iter_limit):
+                new_end = i + iter_limit
                 if i == 0:
-                    title_string = 'first %d variables' %(df_p.shape[1])
+                    title_string = 'first %d variables' % (df_p.shape[1])
                 else:
-                    title_string = 'next %d variables' %(df_p.shape[1])
+                    title_string = 'next %d variables' % (df_p.shape[1])
                 conti = nums[i:new_end]
                 ######################### Add Standard Scaling here ##################################
                 from sklearn.preprocessing import StandardScaler
                 SS = StandardScaler()
-                data = pd.DataFrame(SS.fit_transform(dft[conti]),columns=conti)
+                data = pd.DataFrame(SS.fit_transform(dft[conti]), columns=conti)
                 data[dep] = dft[dep].values
                 dft_sym = data[data[dep] == symbol][conti]
-                var_name = 'drawobjv_list['+str(counter)+']'
+                var_name = 'drawobjv_list[' + str(counter) + ']'
                 drawobj_list.append(var_name)
                 drawobjv_list.append(var_name)
-                drawobj =  dft_sym.hvplot(kind='violin',title='%s: %s' %(sup_title, title_string)).opts(framewise=True).opts(
-                        box_color=color, height=height_size, width=width_size)
+                drawobj = dft_sym.hvplot(kind='violin', title='%s: %s' % (sup_title, title_string)).opts(
+                    framewise=True).opts(
+                    box_color=color, height=height_size, width=width_size)
                 drawobjv_list[counter] = drawobj
                 counter += 1
         ######### After collecting all the drawobjv's put them in a panel and display them ###
-        combined_charts = "".join([x+'+' for x in drawobj_list])[:-1]
+        combined_charts = "".join([x + '+' for x in drawobj_list])[:-1]
         ###########  This is where you put the Panel Together ############
         hv_all = pn.panel(eval(combined_charts))
         if chart_format.lower() in ['server', 'bokeh_server', 'bokeh-server']:
             ### If you want it on a server, you use drawobj.show()
-            print('%s can be found in URL below:' %plot_name)
+            print('%s can be found in URL below:' % plot_name)
             server = pn.serve(hv_all, start=True, show=True)
         elif chart_format == 'html':
             save_html_data(hv_all, chart_format, plot_name, mk_dir)
         else:
             ### This will display it in a Jupyter Notebook.
             display(hv_all)
         #### This is where we add them to the list ######        
         if verbose == 2:
             imgdata_list = append_panels(hv_all, imgdata_list, chart_format)
             image_count += 1
     ########## End of Violin Plots #########
     return hv_all
+
+
 ###########################################################################################
 ##########     Draw date time series variables                    #########################
 ###########################################################################################
-def draw_date_vars_hv(df,dep,datevars, nums, chart_format, modeltype='Regression',
-                        mk_dir='AutoViz_Plots', verbose=0):
+def draw_date_vars_hv(df, dep, datevars, nums, chart_format, modeltype='Regression',
+                      mk_dir='AutoViz_Plots', verbose=0):
     ensure_hvplot_imported()
     #### Now you want to display 2 variables at a time to see how they change over time
     ### Don't change the number of cols since you will have to change rows formula as well
     df = copy.deepcopy(df)
     imgdata_list = list()
     image_count = 0
     N = len(nums)
@@ -1017,60 +1041,62 @@
         if isinstance(dep, str):
             if dep not in nums:
                 nums.append(dep)
         else:
             nums += dep
             nums = find_remove_duplicates(nums)
     else:
-            nums = find_remove_duplicates(nums)
+        nums = find_remove_duplicates(nums)
     ### This is where you draw the widgets #####################
     quantileable = nums[:]
-    cmap_list = ['Blues','rainbow', 'viridis', 'plasma', 'inferno', 'magma', 'cividis']
+    cmap_list = ['Blues', 'rainbow', 'viridis', 'plasma', 'inferno', 'magma', 'cividis']
 
     x = pnw.Select(name='X-Axis', value=datevars[0], options=datevars)
     y = pnw.Select(name='Y-Axis', value=quantileable[0], options=quantileable)
 
     ## you need to decorate this function with depends to make the widgets change axes real time ##
-    @pn.depends(x.param.value, y.param.value) 
-    def create_figure(x, y):
-        #opts = dict(cmap=cmap_list[0], line_color='black')
-        opts = dict(width=width_size, height=height_size, 
-            line_color='black',
-            line_width=1, line_dash='dotted', line_alpha=0.5)
-        #opts['size'] = bubble_size
+    @pn.depends(x.param.value, y.param.value)
+    def create_figure(figure_x, figure_y):
+        # opts = dict(cmap=cmap_list[0], line_color='black')
+        opts = dict(width=width_size, height=height_size,
+                    line_color='black',
+                    line_width=1, line_dash='dotted', line_alpha=0.5)
+        # opts['size'] = bubble_size
         opts['alpha'] = alpha
         opts['tools'] = ['hover']
         opts['toolbar'] = 'above'
-        #opts['colorbar'] = True
-        #opts['color'] = next(colors)
-        opts['title'] = title='Time Series plots of Numeric vars'
-        dft = df.set_index(df[x])
-        conti_df = df[[x,y]].set_index(df[x]).drop(x, axis=1)
+        # opts['colorbar'] = True
+        # opts['color'] = next(colors)
+        opts['title'] = title = 'Time Series plots of Numeric vars'
+        dft = df.set_index(df[figure_x])
+        conti_df = df[[figure_x, figure_y]].set_index(df[figure_x]).drop(figure_x, axis=1)
         return hv.Curve(conti_df).opts(**opts)
 
     widgets = pn.WidgetBox(x, y)
 
-    hv_panel = pn.Row(widgets, create_figure).servable('Cross-selector')    
+    hv_panel = pn.Row(widgets, create_figure).servable('Cross-selector')
     #####################################################
     ##### Save all the chart objects here ##############
     if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-        #server = pn.serve(hv_panel, start=True, show=True)
-        print('%s can be found in URL below:' %plot_name)
+        # server = pn.serve(hv_panel, start=True, show=True)
+        print('%s can be found in URL below:' % plot_name)
         hv_panel.show()
     elif chart_format == 'html':
         save_html_data(hv_panel, chart_format, plot_name, mk_dir)
     else:
         ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
-        display(hv_panel)  
+        display(hv_panel)
     return hv_panel
+
+
 ################################################################################################
 ############# Draw a Heatmap using Pearson Correlation #########################################
 ################################################################################################
-def draw_heatmap_hv(dft, conti, chart_format, datevars=[], dep=None,
-                            modeltype='Regression',classes=None, mk_dir='AutoViz_Plots', verbose=0):
+def draw_heatmap_hv(dft, conti, chart_format, datevars:list, dep=None,
+                    modeltype='Regression', classes=None, mk_dir='AutoViz_Plots', verbose=0):
     ensure_hvplot_imported()
     dft = copy.deepcopy(dft)
     ### Test if this is a time series data set, then differene the continuous vars to find
     ###  if they have true correlation to Dependent Var. Otherwise, leave them as is
     width_size = 600
     height_size = 400
     cmap_list = ["#75968f", "#a5bab7", "#c9d9d3", "#e2e2e2", "#dfccce", "#ddb7b1", "#cc7878", "#933b41", "#550b1d"]
@@ -1081,59 +1107,60 @@
         width_size = 600
     else:
         height_size = 800
         width_size = 1200
     plot_name = 'heatmaps'
     hv_panel = None
     #####  If it is a datetime index we need to calculate heat map on differenced data ###
-    if isinstance(dft.index, pd.DatetimeIndex) :
+    if isinstance(dft.index, pd.DatetimeIndex):
         dft = dft[:]
         timeseries_flag = True
         pass
     else:
         dft = dft[:]
         try:
-            dft.index = pd.to_datetime(dft.pop(datevars[0]),infer_datetime_format=True)
+            dft.index = pd.to_datetime(dft.pop(datevars[0]), infer_datetime_format=True)
             timeseries_flag = True
         except:
             if verbose == 1 and len(datevars) > 0:
-                print('No date vars could be found or %s could not be indexed.' %datevars)
+                print('No date vars could be found or %s could not be indexed.' % datevars)
             elif verbose == 1 and len(datevars) == 0:
                 print('No date vars could be found in data set')
             timeseries_flag = False
     # Add a column: the color depends on target variable but you can use whatever function
     imgdata_list = list()
     ##########    This is where we plot the charts #########################
-    if not modeltype in ['Regression','Clustering']:
+    if modeltype not in ['Regression', 'Clustering']:
         ########## This is for Classification problems only ###########
         if dft[dep].dtype == object or dft[dep].dtype == np.int64:
             dft[dep] = dft[dep].factorize()[0]
         image_count = 0
         N = len(conti)
         target_vars = dft[dep].unique()
         plotc = 1
-        #rows = len(target_vars)
+        # rows = len(target_vars)
         rows = 1
         cols = 1
         if timeseries_flag:
-            dft_target = dft[[dep]+conti].diff()
+            dft_target = dft[[dep] + conti].diff()
         else:
             dft_target = dft[conti]
             dft_target[dep] = dft[dep].values
         corre = dft_target.corr()
         corre = corre.round(2)
         if timeseries_flag:
-            heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True, 
-                    cmap=cmap_list, rot=70,
-            title='Time Series: Heatmap of all Differenced Numeric vars for target = %s' %dep)
+            heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True,
+                                           cmap=cmap_list, rot=70,
+                                           title=f'Time Series: Heatmap of all Differenced '
+                                                 f'Numeric vars for target = {dep}')
         else:
-            heatmap = corre.hvplot.heatmap(height=height_size, width=width_size,  colorbar=True,
-                    cmap=cmap_list,
-                    rot=70,
-            title='Heatmap of all Numeric Variables including target');
+            heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True,
+                                           cmap=cmap_list,
+                                           rot=70,
+                                           title='Heatmap of all Numeric Variables including target')
         hv_plot = heatmap * hv.Labels(heatmap).opts(opts.Labels(text_font_size='7pt'))
         hv_panel = pn.panel(hv_plot)
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
     else:
         ### This is for Regression and None Dep variable problems only ##
@@ -1147,35 +1174,36 @@
             dft_target = dft_target.diff().dropna()
         else:
             dft_target = dft_target[:]
         N = len(conti)
         corre = dft_target.corr()
         corre = corre.round(2)
         if timeseries_flag:
-            heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True, 
-                    cmap=cmap_list,
+            heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True,
+                                           cmap=cmap_list,
                                            rot=70,
-                title='Time Series Data: Heatmap of Differenced Numeric vars including target').opts(
-                        opts.HeatMap(tools=['hover'], toolbar='above'))
+                                           title='Time Series Data: Heatmap of Differenced Numeric vars including target').opts(
+                opts.HeatMap(tools=['hover'], toolbar='above'))
         else:
-            heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True, 
-                    cmap=cmap_list,
+            heatmap = corre.hvplot.heatmap(height=height_size, width=width_size, colorbar=True,
+                                           cmap=cmap_list,
                                            rot=70,
-            title='Heatmap of all Numeric Variables including target').opts(
-                                    opts.HeatMap(tools=['hover'],  toolbar='above'))
+                                           title='Heatmap of all Numeric Variables including target').opts(
+                opts.HeatMap(tools=['hover'], toolbar='above'))
         hv_plot = heatmap * hv.Labels(heatmap).opts(opts.Labels(text_font_size='7pt'))
         hv_panel = pn.panel(hv_plot)
         if verbose == 2:
             imgdata_list = append_panels(hv_panel, imgdata_list, chart_format)
             image_count += 1
     ############# End of Heat Maps ##############
     if chart_format in ['server', 'bokeh_server', 'bokeh-server']:
-        print('%s can be found in URL below:' %plot_name)
+        print('%s can be found in URL below:' % plot_name)
         server = pn.serve(hv_panel, start=True, show=True)
-        #hv_panel.show() ### dont use show for just heatmap there is some problem with it
+        # hv_panel.show() ### dont use show for just heatmap there is some problem with it
     elif chart_format == 'html':
         save_html_data(hv_panel, chart_format, plot_name, mk_dir)
     else:
-        display(hv_panel)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()        
-        #display_obj(hv_panel)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+        display(
+            hv_panel)  # This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
+        # display_obj(hv_panel)  ### This will display it in a Jupyter Notebook. If you want it on a server, you use drawobj.show()
     return hv_panel
 #######################################################################################
```

### Comparing `autoviz-0.1.903/autoviz/AutoViz_NLP.py` & `autoviz-0.1.904/autoviz/AutoViz_NLP.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,686 +1,687 @@
 """
 Copyright 2020 Google LLC. This software is provided as-is, without warranty or
 representation for any use or purpose. Your use of it is subject to your
 agreement with Google.
 """
-# --------------------------------------------------------------------------------
-import pandas as pd, numpy as np
-import pdb
-import nltk
-pd.set_option('display.max_colwidth',5000)
-# --------------------------------------------------------------------------------
-from nltk.sentiment.vader import SentimentIntensityAnalyzer
-from operator import itemgetter
-import copy
-from nltk import word_tokenize, pos_tag
+import pandas as pd
+import string
+
 from collections import Counter
-from nltk.stem.wordnet import WordNetLemmatizer
 
-#Contraction map
+from .AutoViz_Utils import save_image_data
+
+pd.set_option('display.max_colwidth', 5000)
+
+# Contraction map
 c_dict = {
-  "ain't": "am not",
-  "aren't": "are not",
-  "cant":"cannot",
-  "can't": "cannot",
-  "can't've": "cannot have",
-  "'cause": "because",
-  "b": "be",
-  "bc": "because",
-  "becos":"because",
-  "bs": "Expletive",
-  "cause": "because",
-  "could've": "could have",
-  "couldn't": "could not",
-  "couldn't've": "could not have",
-  "corp": "corporation",
-  "cud":"could",
-  "didn't": "did not",
-  "doesn't": "does not",
-  "don't": "do not",
-  "execs": "executives",
-  "fck": "fuck",
-  "fcking": "fucking",
-  "gon na": "going to",
-  "hadn't": "had not",
-  "hadn't've": "had not have",
-  "hasn't": "has not",
-  "haven't": "have not",
-  "he'd": "he would",
-  "he'd've": "he would have",
-  "he'll": "he will",
-  "he'll've": "he will have",
-  "he's": "he is",
-  "how'd": "how did",
-  "how'd'y": "how do you",
-  "how'll": "how will",
-  "how's": "how is",
-  "im": "i am",
-  "iam": "i am",
-  "i'd": "I would",
-  "i'd've": "I would have",
-  "i'll": "I will",
-  "i'll've": "I will have",
-  "i'm": "I am",
-  "i've": "I have",
-  "isn't": "is not",
-  "it'd": "it had",
-  "it'd've": "it would have",
-  "it'll": "it will",
-  "it'll've": "it will have",
-  "it's": "it is",
-  "let's": "let us",
-  "ma'am": "madam",
-  "mayn't": "may not",
-  "mgr": "manager",
-  "might've": "might have",
-  "mightn't": "might not",
-  "mightn't've": "might not have",
-  "must've": "must have",
-  "mustn't": "must not",
-  "mustn't've": "must not have",
-  "needn't": "need not",
-  "needn't've": "need not have",
-  "o'clock": "of the clock",
-  "ofc": "office",
-  "oughtn't": "ought not",
-  "oughtn't've": "ought not have",
-  "pics": "pictures",
-  "shan't": "shall not",
-  "sha'n't": "shall not",
-  "shan't've": "shall not have",
-  "she'd": "she would",
-  "she'd've": "she would have",
-  "she'll": "she will",
-  "she'll've": "she will have",
-  "she's": "she is",
-  "should've": "should have",
-  "shouldn't": "should not",
-  "shouldn't've": "should not have",
-  "so've": "so have",
-  "so's": "so is",
-  "svc":"service",
-  "that'd": "that would",
-  "that'd've": "that would have",
-  "that's": "that is",
-  "there'd": "there had",
-  "there'd've": "there would have",
-  "there's": "there is",
-  "they'd": "they would",
-  "they'd've": "they would have",
-  "they'll": "they will",
-  "they'll've": "they will have",
-  "they're": "they are",
-  "they've": "they have",
-  "tho":"though",
-  "to've": "to have",
-  "wan na": "want to",
-  "wasn't": "was not",
-  "we'd": "we had",
-  "we'd've": "we would have",
-  "we'll": "we will",
-  "we'll've": "we will have",
-  "we're": "we are",
-  "we've": "we have",
-  "weren't": "were not",
-  "what'll": "what will",
-  "what'll've": "what will have",
-  "what're": "what are",
-  "what's": "what is",
-  "what've": "what have",
-  "when's": "when is",
-  "when've": "when have",
-  "where'd": "where did",
-  "where's": "where is",
-  "where've": "where have",
-  "who'll": "who will",
-  "who'll've": "who will have",
-  "who's": "who is",
-  "who've": "who have",
-  "why's": "why is",
-  "why've": "why have",
-  "will've": "will have",
-  "won't": "will not",
-  "won't've": "will not have",
-  "would've": "would have",
-  "wouldn't": "would not",
-  "wouldn't've": "would not have",
-  "y'all": "you all",
-  "y'alls": "you alls",
-  "y'all'd": "you all would",
-  "y'all'd've": "you all would have",
-  "y'all're": "you all are",
-  "y'all've": "you all have",
-  "you'd": "you had",
-  "you'd've": "you would have",
-  "you'll": "you you will",
-  "you'll've": "you you will have",
-  "you're": "you are",
-  "you've": "you have"
+    "ain't": "am not",
+    "aren't": "are not",
+    "cant": "cannot",
+    "can't": "cannot",
+    "can't've": "cannot have",
+    "'cause": "because",
+    "b": "be",
+    "bc": "because",
+    "becos": "because",
+    "bs": "Expletive",
+    "cause": "because",
+    "could've": "could have",
+    "couldn't": "could not",
+    "couldn't've": "could not have",
+    "corp": "corporation",
+    "cud": "could",
+    "didn't": "did not",
+    "doesn't": "does not",
+    "don't": "do not",
+    "execs": "executives",
+    "fck": "fuck",
+    "fcking": "fucking",
+    "gon na": "going to",
+    "hadn't": "had not",
+    "hadn't've": "had not have",
+    "hasn't": "has not",
+    "haven't": "have not",
+    "he'd": "he would",
+    "he'd've": "he would have",
+    "he'll": "he will",
+    "he'll've": "he will have",
+    "he's": "he is",
+    "how'd": "how did",
+    "how'd'y": "how do you",
+    "how'll": "how will",
+    "how's": "how is",
+    "im": "i am",
+    "iam": "i am",
+    "i'd": "I would",
+    "i'd've": "I would have",
+    "i'll": "I will",
+    "i'll've": "I will have",
+    "i'm": "I am",
+    "i've": "I have",
+    "isn't": "is not",
+    "it'd": "it had",
+    "it'd've": "it would have",
+    "it'll": "it will",
+    "it'll've": "it will have",
+    "it's": "it is",
+    "let's": "let us",
+    "ma'am": "madam",
+    "mayn't": "may not",
+    "mgr": "manager",
+    "might've": "might have",
+    "mightn't": "might not",
+    "mightn't've": "might not have",
+    "must've": "must have",
+    "mustn't": "must not",
+    "mustn't've": "must not have",
+    "needn't": "need not",
+    "needn't've": "need not have",
+    "o'clock": "of the clock",
+    "ofc": "office",
+    "oughtn't": "ought not",
+    "oughtn't've": "ought not have",
+    "pics": "pictures",
+    "shan't": "shall not",
+    "sha'n't": "shall not",
+    "shan't've": "shall not have",
+    "she'd": "she would",
+    "she'd've": "she would have",
+    "she'll": "she will",
+    "she'll've": "she will have",
+    "she's": "she is",
+    "should've": "should have",
+    "shouldn't": "should not",
+    "shouldn't've": "should not have",
+    "so've": "so have",
+    "so's": "so is",
+    "svc": "service",
+    "that'd": "that would",
+    "that'd've": "that would have",
+    "that's": "that is",
+    "there'd": "there had",
+    "there'd've": "there would have",
+    "there's": "there is",
+    "they'd": "they would",
+    "they'd've": "they would have",
+    "they'll": "they will",
+    "they'll've": "they will have",
+    "they're": "they are",
+    "they've": "they have",
+    "tho": "though",
+    "to've": "to have",
+    "wan na": "want to",
+    "wasn't": "was not",
+    "we'd": "we had",
+    "we'd've": "we would have",
+    "we'll": "we will",
+    "we'll've": "we will have",
+    "we're": "we are",
+    "we've": "we have",
+    "weren't": "were not",
+    "what'll": "what will",
+    "what'll've": "what will have",
+    "what're": "what are",
+    "what's": "what is",
+    "what've": "what have",
+    "when's": "when is",
+    "when've": "when have",
+    "where'd": "where did",
+    "where's": "where is",
+    "where've": "where have",
+    "who'll": "who will",
+    "who'll've": "who will have",
+    "who's": "who is",
+    "who've": "who have",
+    "why's": "why is",
+    "why've": "why have",
+    "will've": "will have",
+    "won't": "will not",
+    "won't've": "will not have",
+    "would've": "would have",
+    "wouldn't": "would not",
+    "wouldn't've": "would not have",
+    "y'all": "you all",
+    "y'alls": "you alls",
+    "y'all'd": "you all would",
+    "y'all'd've": "you all would have",
+    "y'all're": "you all are",
+    "y'all've": "you all have",
+    "you'd": "you had",
+    "you'd've": "you would have",
+    "you'll": "you you will",
+    "you'll've": "you you will have",
+    "you're": "you are",
+    "you've": "you have"
 }
 
+
 ##################################################################################
-def left_subtract(l1,l2):
+def left_subtract(l1, l2):
     lst = []
     for i in l1:
         if i not in l2:
             lst.append(i)
     return lst
+
+
 ################################################################################
 def return_stop_words():
-    from nltk.corpus import stopwords
     STOP_WORDS = ['it', "this", "that", "to", 'its', 'am', 'is', 'are', 'was', 'were', 'a',
-                'an', 'the', 'and', 'or', 'of', 'at', 'by', 'for', 'with', 'about', 'between',
-                 'into','above', 'below', 'from', 'up', 'down', 'in', 'out', 'on', 'over','will','shall','could',
-                  'under', 'again', 'further', 'then', 'once', 'all', 'any', 'both', 'each','would',
-                   'few', 'more', 'most', 'other', 'some', 'such', 'only', 'own', 'same', 'so',
-                    'than', 'too', 'very', 's', 't', 'can', 'just', 'd', 'll', 'm', 'o', 're',
-                    've', 'y', 'ain', 'ma','them','themselves','they','he','she','ex','become','their']
-    add_words = ["s", "m",'you', 'not',  'get', 'no', 'via', 'one', 'still', 'us', 'u','hey','hi','oh','jeez',
-                'the', 'a', 'in', 'to', 'of', 'i', 'and', 'is', 'for', 'on', 'it', 'got','aww','awww',
-                'not', 'my', 'that', 'by', 'with', 'are', 'at', 'this', 'from', 'be', 'have', 'was',
-                '', ' ', 'say', 's', 'u', 'ap', 'afp', '...', 'n', '\\']
-    #stopWords = text.ENGLISH_STOP_WORDS.union(add_words)
-    stop_words = list(set(STOP_WORDS+add_words))
-    excl =['will',"i'll",'shall',"you'll",'may',"don't","hadn't","hasn't","haven't",
-           "don't","isn't",'if',"mightn't","mustn'","mightn't",'mightn',"needn't",
-           'needn',"needn't",'no','not','shan',"shan't",'shouldn',"shouldn't","wasn't",
-          'wasn','weren',"weren't",'won',"won't",'wouldn',"wouldn't","you'd",
-          "you'd","you'll","you're",'yourself','yourselves']
-    stopWords = left_subtract(stop_words,excl)
+                  'an', 'the', 'and', 'or', 'of', 'at', 'by', 'for', 'with', 'about', 'between',
+                  'into', 'above', 'below', 'from', 'up', 'down', 'in', 'out', 'on', 'over', 'will', 'shall', 'could',
+                  'under', 'again', 'further', 'then', 'once', 'all', 'any', 'both', 'each', 'would',
+                  'few', 'more', 'most', 'other', 'some', 'such', 'only', 'own', 'same', 'so',
+                  'than', 'too', 'very', 's', 't', 'can', 'just', 'd', 'll', 'm', 'o', 're',
+                  've', 'y', 'ain', 'ma', 'them', 'themselves', 'they', 'he', 'she', 'ex', 'become', 'their']
+    add_words = ["s", "m", 'you', 'not', 'get', 'no', 'via', 'one', 'still', 'us', 'u', 'hey', 'hi', 'oh', 'jeez',
+                 'the', 'a', 'in', 'to', 'of', 'i', 'and', 'is', 'for', 'on', 'it', 'got', 'aww', 'awww',
+                 'not', 'my', 'that', 'by', 'with', 'are', 'at', 'this', 'from', 'be', 'have', 'was',
+                 '', ' ', 'say', 's', 'u', 'ap', 'afp', '...', 'n', '\\']
+    # stopWords = text.ENGLISH_STOP_WORDS.union(add_words)
+    stop_words = list(set(STOP_WORDS + add_words))
+    excl = ['will', "i'll", 'shall', "you'll", 'may', "don't", "hadn't", "hasn't", "haven't",
+            "don't", "isn't", 'if', "mightn't", "mustn'", "mightn't", 'mightn', "needn't",
+            'needn', "needn't", 'no', 'not', 'shan', "shan't", 'shouldn', "shouldn't", "wasn't",
+            'wasn', 'weren', "weren't", 'won', "won't", 'wouldn', "wouldn't", "you'd",
+            "you'd", "you'll", "you're", 'yourself', 'yourselves']
+    stopWords = left_subtract(stop_words, excl)
     return sorted(stopWords)
+
+
 ##################################################################################
 def expandContractions(text):
     """
     Takes in a sentence, splits it into list of strings and returns sentence back with
     items sibstituted by expanded abbreviations or abbreviated words that are expanded.
     """
     text_list = text.split(" ")
     return " ".join([c_dict.get(item, item) for item in text_list])
+
+
 #
 # remove entire URL
 def remove_URL(text):
     url = re.compile(r'https?://\S+|www\.\S+')
-    return url.sub(r'',text)
+    return url.sub(r'', text)
+
 
 # Remove just HTML markup language
 def remove_html(text):
-    html=re.compile(r'<.*?>')
-    return html.sub(r'',text)
+    html = re.compile(r'<.*?>')
+    return html.sub(r'', text)
 
-from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 
 # Convert Emojis to Text
 import emoji
+
+
 def convert_emojis(text):
-    try:
-        return emoji.demojize(text)
-    except:
-        return "Errorintext"
+    return emoji.demojize(text)
+
 
-import string
 def remove_punct(text):
-    table=str.maketrans('','',string.punctuation)
+    table = str.maketrans('', '', string.punctuation)
     return text.translate(table)
 
+
 # Clean even further removing non-printable text
 # Thanks to https://www.kaggle.com/rftexas/text-only-kfold-bert
-import string
+
+
 def remove_stopwords(tweet):
     """Removes STOP_WORDS characters"""
     stop_words = return_stop_words()
     tweet = tweet.lower()
     tweet = ' '.join([x for x in tweet.split(" ") if x not in stop_words])
     tweet = ''.join([x for x in tweet if x in string.printable])
     return tweet
 
+
 # define a function that accepts text and returns a list of lemmas
 def split_into_lemmas(text):
     words = TextBlob(text).words
     text = ' '.join([word.lemmatize() for word in words])
     return text
 
+
 # Expand Slangs
 # Thanks to https://www.kaggle.com/rftexas/text-only-kfold-bert
 slangs = {
-    "IG" : "Instagram",
+    "IG": "Instagram",
     "FB": "Facebook",
-    "MOFO" : "Expletive",
-    "OMG" : "Oh my God",
-    "ROFL" : "roll on the floor laughing",
-    "ROFLOL" : "roll on the floor laughing out loud",
-    "ROTFLMAO" : "roll on the floor laughing my ass off",
+    "MOFO": "Expletive",
+    "OMG": "Oh my God",
+    "ROFL": "roll on the floor laughing",
+    "ROFLOL": "roll on the floor laughing out loud",
+    "ROTFLMAO": "roll on the floor laughing my ass off",
     "FCK": "Expletive",
     "LMAO": "Laugh my Ass off",
-    "LOL" : "laugh out loud",
+    "LOL": "laugh out loud",
 }
 
 abbreviations = {
-    "$" : " dollar ",
-    "€" : " euro ",
-    "4ao" : "for adults only",
-    "a.m" : "before midday",
-    "a3" : "anytime anywhere anyplace",
-    "aamof" : "as a matter of fact",
-    "acct" : "account",
-    "adih" : "another day in hell",
-    "afaic" : "as far as i am concerned",
-    "afaict" : "as far as i can tell",
-    "afaik" : "as far as i know",
-    "afair" : "as far as i remember",
-    "afk" : "away from keyboard",
-    "app" : "application",
-    "approx" : "approximately",
-    "apps" : "applications",
-    "asap" : "as soon as possible",
-    "asl" : "age, sex, location",
-    "atk" : "at the keyboard",
-    "ave." : "avenue",
-    "aymm" : "are you my mother",
-    "ayor" : "at your own risk",
-    "b&b" : "bed and breakfast",
-    "b+b" : "bed and breakfast",
-    "b.c" : "before christ",
-    "b2b" : "business to business",
-    "b2c" : "business to customer",
-    "b4" : "before",
-    "b4n" : "bye for now",
-    "b@u" : "back at you",
-    "bae" : "before anyone else",
-    "bak" : "back at keyboard",
-    "bbbg" : "bye bye be good",
-    "bbc" : "british broadcasting corporation",
-    "bbias" : "be back in a second",
-    "bbl" : "be back later",
-    "bbs" : "be back soon",
-    "be4" : "before",
-    "bfn" : "bye for now",
-    "blvd" : "boulevard",
-    "bout" : "about",
-    "brb" : "be right back",
-    "bros" : "brothers",
-    "brt" : "be right there",
-    "bsaaw" : "big smile and a wink",
+    "$": " dollar ",
+    "€": " euro ",
+    "4ao": "for adults only",
+    "a.m": "before midday",
+    "a3": "anytime anywhere anyplace",
+    "aamof": "as a matter of fact",
+    "acct": "account",
+    "adih": "another day in hell",
+    "afaic": "as far as i am concerned",
+    "afaict": "as far as i can tell",
+    "afaik": "as far as i know",
+    "afair": "as far as i remember",
+    "afk": "away from keyboard",
+    "app": "application",
+    "approx": "approximately",
+    "apps": "applications",
+    "asap": "as soon as possible",
+    "asl": "age, sex, location",
+    "atk": "at the keyboard",
+    "ave.": "avenue",
+    "aymm": "are you my mother",
+    "ayor": "at your own risk",
+    "b&b": "bed and breakfast",
+    "b+b": "bed and breakfast",
+    "b.c": "before christ",
+    "b2b": "business to business",
+    "b2c": "business to customer",
+    "b4": "before",
+    "b4n": "bye for now",
+    "b@u": "back at you",
+    "bae": "before anyone else",
+    "bak": "back at keyboard",
+    "bbbg": "bye bye be good",
+    "bbc": "british broadcasting corporation",
+    "bbias": "be back in a second",
+    "bbl": "be back later",
+    "bbs": "be back soon",
+    "be4": "before",
+    "bfn": "bye for now",
+    "blvd": "boulevard",
+    "bout": "about",
+    "brb": "be right back",
+    "bros": "brothers",
+    "brt": "be right there",
+    "bsaaw": "big smile and a wink",
     "btch": "bitch",
-    "btw" : "by the way",
+    "btw": "by the way",
     "btfd": "buy the Expletive dip",
-    "bwl" : "bursting with laughter",
-    "c/o" : "care of",
-    "cet" : "central european time",
-    "cf" : "compare",
-    "cia" : "central intelligence agency",
-    "csl" : "can not stop laughing",
-    "cu" : "see you",
-    "cul8r" : "see you later",
-    "cv" : "curriculum vitae",
-    "cwot" : "complete waste of time",
-    "cya" : "see you",
-    "cyt" : "see you tomorrow",
-    "dae" : "does anyone else",
-    "dbmib" : "do not bother me i am busy",
-    "diy" : "do it yourself",
-    "dm" : "direct message",
-    "dwh" : "during work hours",
-    "e123" : "easy as one two three",
-    "eet" : "eastern european time",
-    "eg" : "example",
-    "embm" : "early morning business meeting",
-    "encl" : "enclosed",
-    "encl." : "enclosed",
-    "etc" : "and so on",
-    "faq" : "frequently asked questions",
-    "fawc" : "for anyone who cares",
-    "fb" : "facebook",
-    "fc" : "fingers crossed",
-    "fig" : "figure",
-    "fimh" : "forever in my heart",
-    "ft." : "feet",
-    "ft" : "featuring",
-    "ftl" : "for the loss",
-    "ftw" : "for the win",
-    "fwiw" : "for what it is worth",
-    "fyi" : "for your information",
-    "g9" : "genius",
-    "gahoy" : "get a hold of yourself",
-    "gal" : "get a life",
-    "gcse" : "general certificate of secondary education",
-    "gfn" : "gone for now",
-    "gg" : "good game",
-    "gl" : "good luck",
-    "glhf" : "good luck have fun",
-    "gmt" : "greenwich mean time",
-    "gmta" : "great minds think alike",
-    "gn" : "good night",
-    "g.o.a.t" : "greatest of all time",
-    "goat" : "greatest of all time",
-    "goi" : "get over it",
-    "gps" : "global positioning system",
-    "gr8" : "great",
-    "gratz" : "congratulations",
-    "gyal" : "girl",
-    "h&c" : "hot and cold",
-    "hp" : "horsepower",
-    "hr" : "hour",
-    "hrh" : "his royal highness",
-    "ht" : "height",
-    "ibrb" : "i will be right back",
-    "ic" : "i see",
-    "icq" : "i seek you",
-    "icymi" : "in case you missed it",
-    "idc" : "i do not care",
-    "idgadf" : "i do not give a damn Expletive",
-    "idgaf" : "i do not give a Expletive",
-    "idk" : "i do not know",
-    "ie" : "that is",
-    "i.e" : "that is",
-    "ifyp" : "i feel your pain",
-    "iirc" : "if i remember correctly",
-    "ilu" : "i love you",
-    "ily" : "i love you",
-    "imho" : "in my humble opinion",
-    "imo" : "in my opinion",
-    "imu" : "i miss you",
-    "iow" : "in other words",
-    "irl" : "in real life",
-    "j4f" : "just for fun",
-    "jic" : "just in case",
-    "jk" : "just kidding",
-    "jsyk" : "just so you know",
-    "l8r" : "later",
-    "lb" : "pound",
-    "lbs" : "pounds",
-    "ldr" : "long distance relationship",
-    "lmao" : "laugh my ass off",
-    "lmfao" : "laugh my Expletive ass off",
-    "lol" : "laugh out loud",
-    "ltd" : "limited",
-    "ltns" : "long time no see",
-    "m8" : "mate",
-    "mf" : "Expletive",
+    "bwl": "bursting with laughter",
+    "c/o": "care of",
+    "cet": "central european time",
+    "cf": "compare",
+    "cia": "central intelligence agency",
+    "csl": "can not stop laughing",
+    "cu": "see you",
+    "cul8r": "see you later",
+    "cv": "curriculum vitae",
+    "cwot": "complete waste of time",
+    "cya": "see you",
+    "cyt": "see you tomorrow",
+    "dae": "does anyone else",
+    "dbmib": "do not bother me i am busy",
+    "diy": "do it yourself",
+    "dm": "direct message",
+    "dwh": "during work hours",
+    "e123": "easy as one two three",
+    "eet": "eastern european time",
+    "eg": "example",
+    "embm": "early morning business meeting",
+    "encl": "enclosed",
+    "encl.": "enclosed",
+    "etc": "and so on",
+    "faq": "frequently asked questions",
+    "fawc": "for anyone who cares",
+    "fb": "facebook",
+    "fc": "fingers crossed",
+    "fig": "figure",
+    "fimh": "forever in my heart",
+    "ft.": "feet",
+    "ft": "featuring",
+    "ftl": "for the loss",
+    "ftw": "for the win",
+    "fwiw": "for what it is worth",
+    "fyi": "for your information",
+    "g9": "genius",
+    "gahoy": "get a hold of yourself",
+    "gal": "get a life",
+    "gcse": "general certificate of secondary education",
+    "gfn": "gone for now",
+    "gg": "good game",
+    "gl": "good luck",
+    "glhf": "good luck have fun",
+    "gmt": "greenwich mean time",
+    "gmta": "great minds think alike",
+    "gn": "good night",
+    "g.o.a.t": "greatest of all time",
+    "goat": "greatest of all time",
+    "goi": "get over it",
+    "gps": "global positioning system",
+    "gr8": "great",
+    "gratz": "congratulations",
+    "gyal": "girl",
+    "h&c": "hot and cold",
+    "hp": "horsepower",
+    "hr": "hour",
+    "hrh": "his royal highness",
+    "ht": "height",
+    "ibrb": "i will be right back",
+    "ic": "i see",
+    "icq": "i seek you",
+    "icymi": "in case you missed it",
+    "idc": "i do not care",
+    "idgadf": "i do not give a damn Expletive",
+    "idgaf": "i do not give a Expletive",
+    "idk": "i do not know",
+    "ie": "that is",
+    "i.e": "that is",
+    "ifyp": "i feel your pain",
+    "iirc": "if i remember correctly",
+    "ilu": "i love you",
+    "ily": "i love you",
+    "imho": "in my humble opinion",
+    "imo": "in my opinion",
+    "imu": "i miss you",
+    "iow": "in other words",
+    "irl": "in real life",
+    "j4f": "just for fun",
+    "jic": "just in case",
+    "jk": "just kidding",
+    "jsyk": "just so you know",
+    "l8r": "later",
+    "lb": "pound",
+    "lbs": "pounds",
+    "ldr": "long distance relationship",
+    "lmao": "laugh my ass off",
+    "lmfao": "laugh my Expletive ass off",
+    "lol": "laugh out loud",
+    "ltd": "limited",
+    "ltns": "long time no see",
+    "m8": "mate",
+    "mf": "Expletive",
     "mfing": "Expletive",
-    "mfs" : "Expletive",
-    "mfw" : "my face when",
-    "mofo" : "Expletive",
-    "mph" : "miles per hour",
-    "mr" : "mister",
-    "mrw" : "my reaction when",
-    "ms" : "miss",
-    "mte" : "my thoughts exactly",
-    "nagi" : "not a good idea",
-    "nbc" : "national broadcasting company",
-    "nbd" : "not big deal",
-    "nfs" : "not for sale",
-    "ngl" : "not going to lie",
-    "nhs" : "national health service",
-    "nrn" : "no reply necessary",
-    "nsfl" : "not safe for life",
-    "nsfw" : "not safe for work",
-    "nth" : "nice to have",
-    "nvr" : "never",
-    "nyc" : "new york city",
-    "oc" : "original content",
-    "og" : "original",
-    "ohp" : "overhead projector",
-    "oic" : "oh i see",
-    "omdb" : "over my dead body",
-    "omg" : "oh my god",
-    "omw" : "on my way",
-    "p.a" : "per annum",
-    "p.m" : "after midday",
-    "pm" : "prime minister",
-    "poc" : "people of color",
-    "pov" : "point of view",
-    "pp" : "pages",
-    "ppl" : "people",
-    "prw" : "parents are watching",
-    "ps" : "postscript",
-    "pt" : "point",
-    "ptb" : "please text back",
-    "pto" : "please turn over",
-    "qpsa" : "what happens", #"que pasa",
-    "ratchet" : "rude",
-    "rbtl" : "read between the lines",
-    "rlrt" : "real life retweet",
-    "rofl" : "rolling on the floor laughing",
-    "roflol" : "rolling on the floor laughing out loud",
-    "rotflmao" : "rolling on the floor laughing my ass off",
-    "rt" : "retweet",
-    "ruok" : "are you ok",
-    "sfw" : "safe for work",
-    "sk8" : "skate",
-    "smh" : "shake my head",
-    "sq" : "square",
-    "srsly" : "seriously",
-    "ssdd" : "same stuff different day",
-    "tbh" : "to be honest",
-    "tbs" : "tablespooful",
-    "tbsp" : "tablespooful",
-    "tfw" : "that feeling when",
-    "thks" : "thank you",
-    "tho" : "though",
-    "thx" : "thank you",
-    "tia" : "thanks in advance",
-    "til" : "today i learned",
-    "tl;dr" : "too long i did not read",
-    "tldr" : "too long i did not read",
-    "tmb" : "tweet me back",
-    "tntl" : "trying not to laugh",
-    "ttyl" : "talk to you later",
-    "u" : "you",
-    "u2" : "you too",
-    "u4e" : "yours for ever",
-    "utc" : "coordinated universal time",
-    "w/" : "with",
-    "w/o" : "without",
-    "w8" : "wait",
-    "wassup" : "what is up",
-    "wb" : "welcome back",
-    "wtf" : "what the Expletive",
-    "WTF" : "what the Expletive",
-    "wtg" : "way to go",
-    "wtpa" : "where the party at",
-    "wuf" : "where are you from",
-    "wuzup" : "what is up",
-    "wywh" : "wish you were here",
-    "yd" : "yard",
-    "ygtr" : "you got that right",
-    "ynk" : "you never know",
-    "zzz" : "sleeping bored and tired"
+    "mfs": "Expletive",
+    "mfw": "my face when",
+    "mofo": "Expletive",
+    "mph": "miles per hour",
+    "mr": "mister",
+    "mrw": "my reaction when",
+    "ms": "miss",
+    "mte": "my thoughts exactly",
+    "nagi": "not a good idea",
+    "nbc": "national broadcasting company",
+    "nbd": "not big deal",
+    "nfs": "not for sale",
+    "ngl": "not going to lie",
+    "nhs": "national health service",
+    "nrn": "no reply necessary",
+    "nsfl": "not safe for life",
+    "nsfw": "not safe for work",
+    "nth": "nice to have",
+    "nvr": "never",
+    "nyc": "new york city",
+    "oc": "original content",
+    "og": "original",
+    "ohp": "overhead projector",
+    "oic": "oh i see",
+    "omdb": "over my dead body",
+    "omg": "oh my god",
+    "omw": "on my way",
+    "p.a": "per annum",
+    "p.m": "after midday",
+    "pm": "prime minister",
+    "poc": "people of color",
+    "pov": "point of view",
+    "pp": "pages",
+    "ppl": "people",
+    "prw": "parents are watching",
+    "ps": "postscript",
+    "pt": "point",
+    "ptb": "please text back",
+    "pto": "please turn over",
+    "qpsa": "what happens",  # "que pasa",
+    "ratchet": "rude",
+    "rbtl": "read between the lines",
+    "rlrt": "real life retweet",
+    "rofl": "rolling on the floor laughing",
+    "roflol": "rolling on the floor laughing out loud",
+    "rotflmao": "rolling on the floor laughing my ass off",
+    "rt": "retweet",
+    "ruok": "are you ok",
+    "sfw": "safe for work",
+    "sk8": "skate",
+    "smh": "shake my head",
+    "sq": "square",
+    "srsly": "seriously",
+    "ssdd": "same stuff different day",
+    "tbh": "to be honest",
+    "tbs": "tablespooful",
+    "tbsp": "tablespooful",
+    "tfw": "that feeling when",
+    "thks": "thank you",
+    "tho": "though",
+    "thx": "thank you",
+    "tia": "thanks in advance",
+    "til": "today i learned",
+    "tl;dr": "too long i did not read",
+    "tldr": "too long i did not read",
+    "tmb": "tweet me back",
+    "tntl": "trying not to laugh",
+    "ttyl": "talk to you later",
+    "u": "you",
+    "u2": "you too",
+    "u4e": "yours for ever",
+    "utc": "coordinated universal time",
+    "w/": "with",
+    "w/o": "without",
+    "w8": "wait",
+    "wassup": "what is up",
+    "wb": "welcome back",
+    "wtf": "what the Expletive",
+    "WTF": "what the Expletive",
+    "wtg": "way to go",
+    "wtpa": "where the party at",
+    "wuf": "where are you from",
+    "wuzup": "what is up",
+    "wywh": "wish you were here",
+    "yd": "yard",
+    "ygtr": "you got that right",
+    "ynk": "you never know",
+    "zzz": "sleeping bored and tired"
 }
 
+
 # Thanks to https://www.kaggle.com/rftexas/text-only-kfold-bert
-from nltk.tokenize import word_tokenize
+
 
 # Thanks to https://www.kaggle.com/rftexas/text-only-kfold-bert
 def expandAbbreviations(sentence):
     text = sentence.split(" ")
     return " ".join([abbreviations.get(item, item) for item in text])
 
+
 # Thanks to https://www.kaggle.com/rftexas/text-only-kfold-bert
 def expandSlangs(sentence):
     text = sentence.split(" ")
     return " ".join([slangs.get(item, item) for item in text])
 
+
 def join_words(text):
     return " ".join(text)
 
-def remove_punctuations(text):
-    try:
-        remove_puncs = re.sub(r'[?|!|~|@|$|%|^|&|#]', r'', text)
-    except:
-        return "error"
-    return re.sub(r'[.|,\'|,|)|(|\|/|+|-|{|}|:|]', r' ', remove_puncs)
 
-import re
+def remove_punctuations(text: str):
+    return re.sub(r'[^\w\s]', '', text)
+
+
 def remove_emoji(text):
     emoji_pattern = re.compile("["
-                           u"\U0001F600-\U0001F64F"  # emoticons
-                           u"\U0001F300-\U0001F5FF"  # symbols & pictographs
-                           u"\U0001F680-\U0001F6FF"  # transport & map symbols
-                           u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
-                           u"\U00002702-\U000027B0"
-                           u"\U000024C2-\U0001F251"
-                           "]+", flags=re.UNICODE)
+                               u"\U0001F600-\U0001F64F"  # emoticons
+                               u"\U0001F300-\U0001F5FF"  # symbols & pictographs
+                               u"\U0001F680-\U0001F6FF"  # transport & map symbols
+                               u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
+                               u"\U00002702-\U000027B0"
+                               u"\U000024C2-\U0001F251"
+                               "]+", flags=re.UNICODE)
     return emoji_pattern.sub(r'', text)
 
-# Remove punctuation marks
-import string
-def remove_punct(text):
-    table=str.maketrans('','',string.punctuation)
-    return text.translate(table)
 
 #### This counts emojis in a sentence which is very helpful to gauge sentiment
 def count_emojis(sentence):
     import regex
     import emoji
     emoji_counter = 0
     data = regex.findall(r'\X', sentence)
     for word in data:
         if any(char in emoji.UNICODE_EMOJI for char in word):
             emoji_counter += 1
     return emoji_counter
+
+
 ################################################################################
 import re
 from wordcloud import WordCloud, STOPWORDS
 import matplotlib.pyplot as plt
-from textblob import TextBlob, Word
+from textblob import TextBlob
 from itertools import chain
 
 replace_spaces = re.compile('[/(){}\[\]\|@,;]')
 remove_special_chars = re.compile('[^0-9a-z #+_]')
 STOPWORDS = return_stop_words()
 remove_ip_addr = re.compile(r'\b(?:[0-9]{1,3}\.){3}[0-9]{1,3}\b')
 
+
 def clean_steps(text):
-    text = text.replace('\n', ' ').lower()#
+    text = text.replace('\n', ' ').lower()  #
     text = remove_ip_addr.sub('', text)
-    text = replace_spaces.sub(' ',text)
-    text = remove_special_chars.sub('',text)
-    text = ' '.join([w for w in text.split() if not w in STOPWORDS])
+    text = replace_spaces.sub(' ', text)
+    text = remove_special_chars.sub('', text)
+    text = ' '.join([w for w in text.split() if w not in STOPWORDS])
     return text
 
+
 def clean_text(x):
     """
     ###############################################################################
     ## This cleans text string. Use it only as a Series.map(clean_text) function  #
     ###############################################################################
     Input must be one text string only. Don't send arrays or dataframes.
     Clean steps cleans one tweet at a time using following steps:
     1. removes URL
     2. Removes a very small list of stop words - about 65
     """
-    x = expandSlangs(x) ### do this before lowering case since case is important for sentiment
-    x = expandAbbreviations(x) ### this is before lowering case since case is important in sentiment
+    x = expandSlangs(x)  ### do this before lowering case since case is important for sentiment
+    x = expandAbbreviations(x)  ### this is before lowering case since case is important in sentiment
     x = expandContractions(x)  ### this is after lowering case - just to double check
-    x = remove_stopwords(x) ## this works well to remove a small number of stop words
-    x = remove_punctuations(x) # this works well to remove punctuations and add spaces correctly
-    x = split_into_lemmas(x) ## this lemmatizes text and gets it ready for wordclouds ###
+    x = remove_stopwords(x)  ## this works well to remove a small number of stop words
+    x = remove_punctuations(x)  # this works well to remove punctuations and add spaces correctly
+    x = split_into_lemmas(x)  ## this lemmatizes text and gets it ready for wordclouds ###
     return x
 
-def draw_wordcloud_from_dataframe(dataframe, column, chart_format, 
-                                depVar, mk_dir, verbose=0):
+
+def draw_wordcloud_from_dataframe(dataframe, column):
     """
     This handy function draws a dataframe column using Wordcloud library and nltk.
     """
-    imgdata_list = []
-    
+
     ### Remember that fillna only works at dataframe level! ##
     X_train = dataframe[[column]].fillna("missing")
     ### Map function only works on Series, so you should use this ###
     X_train = X_train[column].map(clean_steps)
     ### next time, you get back a series, so just use it as is ###
     X_train = X_train.map(clean_text)
-    
+
     # Dictionary of all words from train corpus with their counts.
 
     ### Fantastic way to count words using one line of code #############
     ###  Thanks to : https://stackoverflow.com/questions/35857519/efficiently-count-word-frequencies-in-python
     words_counts = Counter(chain.from_iterable(map(str.split, X_train)))
     vocab_size = 50000
     top_words = sorted(words_counts, key=words_counts.get, reverse=True)[:vocab_size]
     text_join = ' '.join(top_words)
 
-    #picture_mask = plt.imread('test.png')
+    # picture_mask = plt.imread('test.png')
 
     wordcloud1 = WordCloud(
-                          stopwords=STOPWORDS,
-                          background_color='white',
-                          width=1800,
-                          height=1400,
-                          #mask=picture_mask
-                ).generate(text_join)
+        stopwords=STOPWORDS,
+        background_color='white',
+        width=1800,
+        height=1400,
+        # mask=picture_mask
+    ).generate(text_join)
     return wordcloud1
+
+
 ################################################################################
 # Removes duplicates from a list to return unique values - USED ONLYONCE
 def find_remove_duplicates(values):
     output = []
     seen = set()
     for value in values:
         if value not in seen:
             output.append(value)
             seen.add(value)
     return output
 
-def draw_word_clouds(dft, each_string_var, chart_format, plotname, 
-                        dep, problem_type, classes, mk_dir, verbose=0):
+
+def draw_word_clouds(dft, each_string_var, chart_format, plotname,
+                     dep, problem_type, classes, mk_dir, verbose=0):
     dft = dft[:]
     width_size = 20
     height_size = 10
-    image_count = 0
     imgdata_list = []
 
     if problem_type == 'Regression' or problem_type == 'Clustering':
         ########## This is for Regression and Clustering problems only #####
         num_plots = 1
-        fig = plt.figure(figsize=(min(num_plots*width_size,20),min(num_plots*height_size,20)))
+        fig = plt.figure(figsize=(min(num_plots * width_size, 20), min(num_plots * height_size, 20)))
         cols = 2
-        rows = int(num_plots/cols + 0.5)
+        rows = int(num_plots / cols + 0.5)
         plotc = 1
         while plotc <= num_plots:
             plt.subplot(rows, cols, plotc)
             ax1 = plt.gca()
-            wc1 = draw_wordcloud_from_dataframe(dft, each_string_var, chart_format,
-                    dep, mk_dir, verbose)
+            wc1 = draw_wordcloud_from_dataframe(dft, each_string_var)
             plotc += 1
             ax1.axis("off")
             ax1.imshow(wc1)
-            ax1.set_title('Wordcloud for %s' %each_string_var)
+            ax1.set_title('Wordcloud for %s' % each_string_var)
         image_count = 0
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                                plotname, depVar, mk_dir))
+                                                plotname, mk_dir))
             image_count += 1
         if verbose <= 1:
-            plt.show();
+            plt.show()
     else:
         ########## This is for Classification problems only ###########
         num_plots = len(classes)
         target_vars = dft[dep].unique()
-        fig = plt.figure(figsize=(min(num_plots*width_size,20),min(num_plots*height_size,20)))
+        fig = plt.figure(figsize=(min(num_plots * width_size, 20), min(num_plots * height_size, 20)))
         cols = 2
-        rows = int(num_plots/cols + 0.5)
+        rows = int(num_plots / cols + 0.5)
         plotc = 1
         while plotc <= num_plots:
             plt.subplot(rows, cols, plotc)
             ax1 = plt.gca()
             ax1.axis("off")
-            dft_target = dft.loc[(dft[dep] == target_vars[plotc-1])][each_string_var]
-            if isinstance(dft_target,pd.Series):
-                wc1 = draw_wordcloud_from_dataframe(pd.DataFrame(dft_target), each_string_var, chart_format,
-                        dep, mk_dir, verbose)
+            dft_target = dft.loc[(dft[dep] == target_vars[plotc - 1])][each_string_var]
+            if isinstance(dft_target, pd.Series):
+                wc1 = draw_wordcloud_from_dataframe(pd.DataFrame(dft_target), each_string_var)
             else:
-                wc1 = draw_wordcloud_from_dataframe(dft_target, each_string_var, chart_format,
-                        dep, mk_dir, verbose)
+                wc1 = draw_wordcloud_from_dataframe(dft_target, each_string_var)
             ax1.imshow(wc1)
-            ax1.set_title('Wordcloud for %s, target=%s' %(each_string_var, target_vars[plotc-1]), fontsize=20)
+            ax1.set_title('Wordcloud for %s, target=%s' % (each_string_var, target_vars[plotc - 1]), fontsize=20)
             plotc += 1
-        fig.tight_layout();
+        fig.tight_layout()
         ### This is where you save the fig or show the fig ######
         image_count = 0
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                                plotname, depVar, mk_dir))
+                                                plotname, mk_dir))
             image_count += 1
         if verbose <= 1:
-            plt.show();
+            plt.show()
     ####### End of Word Clouds #############################
-
```

### Comparing `autoviz-0.1.903/autoviz/AutoViz_Utils.py` & `autoviz-0.1.904/autoviz/AutoViz_Utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,1227 +1,1179 @@
 ############################################################################
-#Copyright 2019 Google LLC
+# Copyright 2019 Google LLC
 #
-#Licensed under the Apache License, Version 2.0 (the "License");
-#you may not use this file except in compliance with the License.
-#You may obtain a copy of the License at
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
 #
 #    https://www.apache.org/licenses/LICENSE-2.0
 #
-#Unless required by applicable law or agreed to in writing, software
-#distributed under the License is distributed on an "AS IS" BASIS,
-#WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#See the License for the specific language governing permissions and
-#limitations under the License.
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 #################################################################################################
-import pandas as pd
-import numpy as np
-from pathlib import Path
 import os
 #### The warnings from Sklearn are so annoying that I have to shut it off ####
 import warnings
+
+import numpy as np
+import pandas as pd
+
 warnings.filterwarnings("ignore")
-def warn(*args, **kwargs):
+
+
+def warn():
     pass
+
+
 warnings.warn = warn
 ########################################
 import warnings
+
 warnings.filterwarnings("ignore")
 from sklearn.exceptions import DataConversionWarning
+
 warnings.filterwarnings(action='ignore', category=DataConversionWarning)
 ####################################################################################
 import matplotlib
+
 matplotlib.use('agg')
 import matplotlib.pyplot as plt
 # from matplotlib import io
 import io
 import seaborn as sns
-sns.set(style="whitegrid", color_codes=True)
+
+# sns.set(style="whitegrid", color_codes=True)
 import re
 import pprint
-import matplotlib
-#matplotlib.style.use('seaborn')
+# matplotlib.style.use('seaborn')
 from itertools import cycle, combinations
-from collections import defaultdict
-import copy
-import time
 import sys
-import random
-import xlrd
-import statsmodels
 from io import BytesIO
 import base64
-from functools import reduce
-import traceback
-import xgboost as xgb
-from xgboost.sklearn import XGBClassifier
-from xgboost.sklearn import XGBRegressor
 from sklearn.model_selection import train_test_split
 from .classify_method import classify_columns
+
+
 ######## This is where we store the image data in a dictionary with a list of images #########
-def save_image_data(fig, chart_format, plot_name, depVar, mk_dir, additional=''):
+def save_image_data(fig, chart_format, plot_name, mk_dir, additional=''):
     if not os.path.isdir(mk_dir):
         os.mkdir(mk_dir)
     if additional == '':
-        filename = os.path.join(mk_dir,plot_name+"."+chart_format)
+        filename = os.path.join(mk_dir, plot_name + "." + chart_format)
     else:
-        filename = os.path.join(mk_dir,plot_name+additional+"."+chart_format)
+        filename = os.path.join(mk_dir, plot_name + additional + "." + chart_format)
     ##################################################################################
     if chart_format == 'svg':
         ###### You have to add these lines to each function that creates charts currently ##
         imgdata = io.StringIO()
         fig.savefig(filename, dpi='figure', format=chart_format)
         imgdata.seek(0)
         svg_data = imgdata.getvalue()
         return svg_data
     else:
         ### You have to do it slightly differently for PNG and JPEG formats
         imgdata = BytesIO()
-        fig.savefig(filename,format=chart_format, dpi='figure')
-        #fig.savefig(imgdata, format=chart_format, bbox_inches='tight', pad_inches=0.0)
+        fig.savefig(filename, format=chart_format, dpi='figure')
+        # fig.savefig(imgdata, format=chart_format, bbox_inches='tight', pad_inches=0.0)
         imgdata.seek(0)
         figdata_png = base64.b64encode(imgdata.getvalue())
         return figdata_png
 
+
 #### This module analyzes a dependent Variable and finds out whether it is a
 #### Regression or Classification type problem
-def analyze_problem_type(train, target, verbose=0) : 
+def analyze_problem_type(train, target, verbose=0):
     train = copy.deepcopy(train)
     target = copy.deepcopy(target)
-    cat_limit = 30 ### this determines the number of categories to name integers as classification ##
-    float_limit = 15 ### this limits the number of float variable categories for it to become cat var
-    
+    cat_limit = 30  ### this determines the number of categories to name integers as classification ##
+    float_limit = 15  ### this limits the number of float variable categories for it to become cat var
+
     if isinstance(target, str):
         target = [target]
     ### we can analyze only the first target in a multi-label to detect problem type ##
     targ = target[0]
     ####  This is where you detect what kind of problem it is #################
-    if  train[targ].dtype in [np.int64,np.int32,np.int16,np.int8]:
+    if train[targ].dtype in [np.int64, np.int32, np.int16, np.int8]:
         if len(train[targ].unique()) <= 2:
             model_class = 'Binary_Classification'
-        elif len(train[targ].unique().tolist()) > 2 and len(train[targ].unique().tolist()) <= cat_limit:
+        elif 2 < len(train[targ].unique().tolist()) <= cat_limit:
             model_class = 'Multi_Classification'
         else:
             model_class = 'Regression'
-    elif  train[targ].dtype in ['float16','float32','float64']:
+    elif train[targ].dtype in ['float16', 'float32', 'float64']:
         if len(train[targ].unique()) <= 2:
             model_class = 'Binary_Classification'
-        elif len(train[targ].unique().tolist()) > 2 and len(train[targ].unique().tolist()) <= float_limit:
+        elif 2 < len(train[targ].unique().tolist()) <= float_limit:
             model_class = 'Multi_Classification'
         else:
             model_class = 'Regression'
     elif train[targ].dtype == bool:
         model_class = 'Binary_Classification'
     else:
         if len(train[targ].unique().tolist()) <= 2:
             model_class = 'Binary_Classification'
         else:
             model_class = 'Multi_Classification'
     ########### print this for the start of next step ###########
     if verbose <= 2:
-        print('''\n################ %s problem #####################''' %model_class)
+        print('''\n################ %s problem #####################''' % model_class)
     return model_class
+
+
 #################################################################################
 # Pivot Tables are generally meant for Categorical Variables on the axes
 # and a Numeric Column (typically the Dep Var) as the "Value" aggregated by Sum.
 # Let's do some pivot tables to capture some meaningful insights
-import random
-def draw_pivot_tables(dft, problem_type, verbose, chart_format, depVar='', classes=None, mk_dir=None):
+def draw_pivot_tables(dft, problem_type, verbose, chart_format, depVar='', mk_dir=None):
     #### Finally I have fixed the bugs in pivot tables due to "category" dtypes in data ##############
     plot_name = 'Bar_Plots_Cats'
     imgdata_list = []
-    cats = [i for i in dft.loc[:,dft.nunique()<=15]]
+    cats = [i for i in dft.loc[:, dft.nunique() <= 15]]
     if isinstance(depVar, str):
         cats = [x for x in cats if x not in [depVar]]
     else:
         cats = [x for x in cats if x not in depVar]
     dft = copy.deepcopy(dft)
-    cols = 2
     cmap = plt.get_cmap('jet')
     #### For some reason, the cmap colors are not working #########################
-    colors = cmap(np.linspace(0, 1, len(cats)))
-    colors = cycle('byrcmgkbyrcmgkbyrcmgkbyrcmgkbyr')
-    #colormaps = ['summer', 'rainbow','viridis','inferno','magma','jet','plasma']
-    colormaps = ['Greys','Blues','Greens','GnBu','PuBu',
-                    'YlGnBu','PuBuGn','BuGn','YlGn']
-    #colormaps = ['Purples','Oranges','Reds','YlOrBr',
+    # colormaps = ['summer', 'rainbow','viridis','inferno','magma','jet','plasma']
+    # colormaps = ['Purples','Oranges','Reds','YlOrBr',
     #                'YlOrRd','OrRd','PuRd','RdPu','BuPu',]
     N = len(cats)
     combos = copy.deepcopy(cats)
-    if N==0:
+    if N == 0:
         print('No categorical or boolean vars in data set. Hence no pivot plots...')
         return None
-    noplots = copy.deepcopy(N)
     #### You can set the number of subplots per row and the number of categories to display here cols = 2
-    displaylimit = 20
     categorylimit = 5
-    width_size = 15
     height_size = 5
-    stringlimit = 20
     N = len(cats)
     sns.set_palette("Set1")
     ###########  This works equally well for classification as well as Regression ###
-    lst=[]
-    noplots=int(len(cats))
+    noplots = int(len(cats))
     dicti = {}
     counter = 1
     cols = 2
     ### first make sure there are enough plots to plot #####
     ######  we want to now figure out rows and columns ####
-    if noplots%cols <= 2:
+    if noplots % cols <= 2:
         if noplots == 0:
             rows = 1
         else:
-            rows = int((noplots/cols)+0.5)
+            rows = int((noplots / cols) + 0.5)
     else:
-        rows = int((noplots/cols)+0.5)
-    countplots  = len(cats)
+        rows = int((noplots / cols) + 0.5)
     if N > 0:
         fig = plt.figure()
         if cols < 2:
-            fig.set_size_inches(min(15,8),rows*height_size)
-            fig.subplots_adjust(hspace=0.5) ### This controls the space betwen rows
-            fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
-        else:
-            fig.set_size_inches(min(cols*10,20),rows*height_size)
-            fig.subplots_adjust(hspace=0.5) ### This controls the space betwen rows
-            fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
+            fig.set_size_inches(min(15, 8), rows * height_size)
+            fig.subplots_adjust(hspace=0.5)  ### This controls the space between rows
+            fig.subplots_adjust(wspace=0.3)  ### This controls the space between columns
+        else:
+            fig.set_size_inches(min(cols * 10, 20), rows * height_size)
+            fig.subplots_adjust(hspace=0.5)  ### This controls the space between rows
+            fig.subplots_adjust(wspace=0.3)  ### This controls the space between columns
         ### we start to draw the pivot tables here #########
         for var1 in combos:
-            #color1 = random.choice(colormaps)
-            color1 = "Set1"
-            data = pd.DataFrame(dicti)
-            x=dft[var1]
-            ax1 = fig.add_subplot(rows,cols,counter)
-            nocats = min(categorylimit,dft[var1].nunique())
-            data = dft[var1].value_counts()
+            # color1 = random.choice(colormaps)
+            ax1 = fig.add_subplot(rows, cols, counter)
             if problem_type in ['Binary_Classification', 'Multi_Classification']:
                 if dft[depVar].nunique() > 15:
                     sns.countplot(x=var1,
-                                    data=dft,
-                                    ax=ax1,
-                                    order=dft[var1].value_counts().index,)
-                    ax1.set_title('Distribution of %s' %var1,fontsize=12)
+                                  data=dft,
+                                  ax=ax1,
+                                  order=dft[var1].value_counts().index, )
+                    ax1.set_title('Distribution of %s' % var1, fontsize=12)
                 else:
                     sns.countplot(x=var1,
-                                    data=dft,
-                                    ax=ax1,
-                                    order=dft[var1].value_counts().index,
-                                    hue = depVar)
-                    ax1.set_title('Distribution of %s by %s' %(var1, depVar),fontsize=12)
+                                  data=dft,
+                                  ax=ax1,
+                                  order=dft[var1].value_counts().index,
+                                  hue=depVar)
+                    ax1.set_title('Distribution of %s by %s' % (var1, depVar), fontsize=12)
             else:
                 sns.countplot(x=var1,
-                                data=dft,
-                                ax=ax1,
-                                order=dft[var1].value_counts().index,)
-                ax1.set_title('Distribution of %s' %var1,fontsize=12)
+                              data=dft,
+                              ax=ax1,
+                              order=dft[var1].value_counts().index, )
+                ax1.set_title('Distribution of %s' % var1, fontsize=12)
             ax1.set_xlabel(var1)
             ax1.set_xticklabels(dft[var1].value_counts().index, rotation=30, ha='right', fontsize=9)
             counter += 1
         fig.tight_layout()
-        fig.suptitle('Distribution of Variables (with <=15 categories)', fontsize=15,y=1.01);
+        fig.suptitle('Distribution of Variables (with <=15 categories)', fontsize=15, y=1.01)
     image_count = 0
     if verbose == 2:
         imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name, depVar, mk_dir))
+                                            plot_name, mk_dir))
         image_count += 1
     if verbose <= 1:
-        plt.show();
+        plt.show()
     ####### End of Pivot Plotting #############################
     return imgdata_list
 
-def draw_pivot_tables_old(dft,problem_type,verbose,chart_format,depVar='', classes=None, mk_dir=None):
+
+def draw_pivot_tables_old(dft, verbose, chart_format, depVar='', mk_dir=None):
     #### Finally I have fixed the bugs in pivot tables due to "category" dtypes in data ##############
     plot_name = 'Bar_Plots_Pivots'
+    cats = [i for i in dft.loc[:, dft.nunique() <= 15]]
     cats = copy.deepcopy(cats)
     cats = list(set(cats))
     dft = copy.deepcopy(dft)
-    cols = 2
     cmap = plt.get_cmap('jet')
     #### For some reason, the cmap colors are not working #########################
-    colors = cmap(np.linspace(0, 1, len(cats)))
-    colors = cycle('byrcmgkbyrcmgkbyrcmgkbyrcmgkbyr')
-    #colormaps = ['summer', 'rainbow','viridis','inferno','magma','jet','plasma']
-    colormaps = ['Greys','Blues','Greens','GnBu','PuBu',
-                    'YlGnBu','PuBuGn','BuGn','YlGn']
-    #colormaps = ['Purples','Oranges','Reds','YlOrBr',
+    # colormaps = ['summer', 'rainbow','viridis','inferno','magma','jet','plasma']
+    # colormaps = ['Purples','Oranges','Reds','YlOrBr',
     #                'YlOrRd','OrRd','PuRd','RdPu','BuPu',]
-    N = len(cats)
-    if N==0:
+    len_cats = len(cats)
+    if len_cats == 0:
         print('No categorical or boolean vars in data set. Hence no pivot plots...')
         return None
-    noplots = copy.deepcopy(N)
     #### You can set the number of subplots per row and the number of categories to display here cols = 2
-    displaylimit = 20
     categorylimit = 5
     imgdata_list = []
-    width_size = 15
     height_size = 5
     stringlimit = 20
     combos = combinations(cats, 2)
-    N = len(cats)
+    len_cats = len(cats)
     sns.set_palette("Set1")
-    if N <= 1:
+    if len_cats <= 1:
         ### if there are not many categorical variables, there is nothing to plot
         return imgdata_list
-    if len(nums) == 0:
+    if len(cats) == 0:
         ### if there are no numeric variables, there is nothing to plot
         return imgdata_list
-    if not depVar is None or not depVar=='' or not depVar==[] :
+    if depVar is not None or not depVar == '' or not depVar == []:
         ###########  This works equally well for classification as well as Regression ###
-        lst=[]
-        noplots=int((N**2-N)/2)
+        noplots = int((len_cats ** 2 - len_cats) / 2)
         dicti = {}
         counter = 1
         cols = 2
         ### first make sure there are enough plots to plot #####
         copy_combos = copy.deepcopy(combos)
         countplots = 0
         for var1, var2 in copy_combos:
             if dft[depVar].dtype == object:
-                data = pd.pivot_table(dft,values=depVar,index=var1, columns=var2, aggfunc='count',fill_value=0)
+                data = pd.pivot_table(dft, values=depVar, index=var1, columns=var2, aggfunc='count', fill_value=0)
             elif str(dft[depVar].dtype) in ['category']:
-                data = pd.pivot_table(dft,values=depVar,index=var1, columns=var2, aggfunc='count',fill_value=0)
-            else:                
-                data = pd.pivot_table(dft,values=depVar,index=var1, columns=var2)
+                data = pd.pivot_table(dft, values=depVar, index=var1, columns=var2, aggfunc='count', fill_value=0)
+            else:
+                data = pd.pivot_table(dft, values=depVar, index=var1, columns=var2)
             if data.shape[1] > 0:
                 countplots += 1
         if countplots != noplots:
             noplots = copy.deepcopy(countplots)
         ######  we want to now figure out rows and columns ####
-        if noplots%cols == 0:
+        if noplots % cols == 0:
             if noplots == 0:
                 rows = 1
             else:
-                rows = int((noplots/cols)+0.5)
+                rows = int((noplots / cols) + 0.5)
         else:
-            rows = int((noplots/cols)+0.5)
+            rows = int((noplots / cols) + 0.5)
         ### Now let us draw the pivot charts ############
         if countplots > 0:
             fig = plt.figure()
             if cols < 2:
-                fig.set_size_inches(min(15,8),rows*height_size)
-                fig.subplots_adjust(hspace=0.5) ### This controls the space betwen rows
-                fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
+                fig.set_size_inches(min(15, 8), rows * height_size)
+                fig.subplots_adjust(hspace=0.5)  ### This controls the space between rows
+                fig.subplots_adjust(wspace=0.3)  ### This controls the space between columns
             else:
-                fig.set_size_inches(min(cols*10,20),rows*height_size)
-                fig.subplots_adjust(hspace=0.5) ### This controls the space betwen rows
-                fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
+                fig.set_size_inches(min(cols * 10, 20), rows * height_size)
+                fig.subplots_adjust(hspace=0.5)  ### This controls the space between rows
+                fig.subplots_adjust(wspace=0.3)  ### This controls the space between columns
             ### we start to draw the pivot tables here #########
             for (var1, var2) in combos:
-                #color1 = random.choice(colormaps)
+                # color1 = random.choice(colormaps)
                 color1 = "Set1"
-                data = pd.DataFrame(dicti)
-                x=dft[var1]
-                y=dft[var2]
-                ax1 = fig.add_subplot(rows,cols,counter)
-                nocats = min(categorylimit,dft[var1].nunique())
-                nocats1 = min(categorylimit,dft[var2].nunique())
-                if dft[depVar].dtype==object or dft[depVar].dtype==bool:
+                ax1 = fig.add_subplot(rows, cols, counter)
+                nocats = min(categorylimit, dft[var1].nunique())
+                nocats1 = min(categorylimit, dft[var2].nunique())
+                if dft[depVar].dtype == object or dft[depVar].dtype == bool:
                     dft[depVar] = dft[depVar].factorize()[0]
                 if dft[depVar].dtype == object:
-                    data = pd.pivot_table(dft,values=depVar,index=var1, columns=var2, aggfunc='count',fill_value=0).head(nocats)
+                    data = pd.pivot_table(dft, values=depVar, index=var1, columns=var2, aggfunc='count',
+                                          fill_value=0).head(nocats)
                 elif str(dft[depVar].dtype) in ['category']:
-                    data = pd.pivot_table(dft,values=depVar,index=var1, columns=var2, aggfunc='count',fill_value=0).head(nocats)
-                else:                
-                    data = pd.pivot_table(dft,values=depVar,index=var1, columns=var2).head(nocats)
-                data = data[data.columns[:nocats1]] #### make sure you don't print more than 10 rows of data
-                data.plot(kind='bar',ax=ax1,colormap=color1)
+                    data = pd.pivot_table(dft, values=depVar, index=var1, columns=var2, aggfunc='count',
+                                          fill_value=0).head(nocats)
+                else:
+                    data = pd.pivot_table(dft, values=depVar, index=var1, columns=var2).head(nocats)
+                data = data[data.columns[:nocats1]]  #### make sure you don't print more than 10 rows of data
+                data.plot(kind='bar', ax=ax1, colormap=color1)
                 ax1.set_xlabel(var1)
                 ax1.set_ylabel(depVar)
                 if dft[var1].dtype == object or str(dft[depVar].dtype) in ['category']:
                     labels = data.index.str[:stringlimit].tolist()
                 else:
                     labels = data.index.tolist()
-                ax1.set_xticklabels(labels,fontdict={'fontsize':10}, rotation = 45, ha="right")
+                ax1.set_xticklabels(labels, fontdict={'fontsize': 10}, rotation=45, ha="right")
                 ax1.legend(fontsize="medium")
-                ax1.set_title('%s (Mean) by %s and %s' %(depVar,var1,var2),fontsize=12)
+                ax1.set_title('%s (Mean) by %s and %s' % (depVar, var1, var2), fontsize=12)
                 counter += 1
             fig.tight_layout()
-            fig.suptitle('Target (average) by two Categorical vars (top 5 categories)', fontsize=15,y=1.01);
+            fig.suptitle('Target (average) by two Categorical vars (top 5 categories)', fontsize=15, y=1.01)
     image_count = 0
     if verbose == 2:
         imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name, depVar, mk_dir))
+                                            plot_name, mk_dir))
         image_count += 1
     if verbose <= 1:
-        plt.show();
+        plt.show()
     ####### End of Pivot Plotting #############################
     return imgdata_list
 
+
 # In[ ]:
 # SCATTER PLOTS ARE USEFUL FOR COMPARING NUMERIC VARIABLES
-def draw_scatters(dfin,nums,verbose,chart_format,problem_type,dep=None, classes=None, lowess=False, mk_dir=None):
+def draw_scatters(dfin, nums, verbose, chart_format, problem_type, dep=None, classes=None, lowess=False, mk_dir=None):
     plot_name = 'Scatter_Plots'
     dft = dfin[:]
     ##### we are going to modify dfin and classes, so we are making copies to make changes
     classes = copy.deepcopy(classes)
     colortext = 'brymcgkbyrcmgkbyrcmgkbyrcmgkbyr'
     if len(classes) == 0:
         leng = len(nums)
     else:
         leng = len(classes)
     colors = cycle(colortext[:leng])
-    #imgdata_list = defaultdict(list)
+    # imgdata_list = defaultdict(list)
     imgdata_list = []
-    if dfin.shape[0] >= 10000 or lowess == False:
+    if dfin.shape[0] >= 10000 or lowess is False:
         lowess = False
-        x_est = None
-        transparent = 0.6
-        bubble_size = 80
     else:
         if verbose <= 1:
             print('Using Lowess Smoothing. This might take a few minutes for large data sets...')
         lowess = True
-        x_est = None
-        transparent = 0.6
-        bubble_size = 100
     if verbose <= 1:
-        x_est = np.mean
-    N = len(nums)
+        pass
     cols = 2
     width_size = 15
     height_size = 4
     sns.set_palette("Set1")
-    if dep == None or dep == '':
+    if dep is None or dep == '':
         ### when there is no dependent variable, you can't plot anything in scatters here ###
         return None
     elif problem_type == 'Regression':
         image_count = 0
         ####### This is a Regression Problem so it requires 2 steps ####
         ####### First, plot every Independent variable against the Dependent Variable ###
         noplots = len(nums)
-        rows = int((noplots/cols)+0.99)
-        fig = plt.figure(figsize=(width_size,rows*height_size))
-        for num, plotcounter, color_val in zip(nums, range(1,noplots+1), colors):
+        rows = int((noplots / cols) + 0.99)
+        fig = plt.figure(figsize=(width_size, rows * height_size))
+        for num, plotcounter, color_val in zip(nums, range(1, noplots + 1), colors):
             ### Be very careful with the next line. It should be singular "subplot" ##
             ##### Otherwise, if you use the plural version "subplots" it has a different meaning!
-            plt.subplot(rows,cols,plotcounter)
+            plt.subplot(rows, cols, plotcounter)
             if lowess:
-                sns.regplot(x=dft[num], y = dft[dep], lowess=lowess, color=color_val, ax=plt.gca())
+                sns.regplot(x=dft[num], y=dft[dep], lowess=lowess, color=color_val, ax=plt.gca())
             else:
-                sns.scatterplot(x=dft[num], y=dft[dep], ax=plt.gca(), palette='dark',color=color_val)
+                sns.scatterplot(x=dft[num], y=dft[dep], ax=plt.gca(), palette='dark', color=color_val)
             plt.xlabel(num)
             plt.ylabel(dep)
-        fig.suptitle('Scatter Plot of each Continuous Variable vs Target',fontsize=15,y=1.01)
-        fig.tight_layout();
+        fig.suptitle('Scatter Plot of each Continuous Variable vs Target', fontsize=15, y=1.01)
+        fig.tight_layout()
         if verbose <= 1:
-            plt.show();
+            plt.show()
         #### Keep it at the figure level###
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name, dep, mk_dir))
+                                                plot_name, mk_dir))
             image_count += 1
     else:
         ####### This is a Classification Problem #### You need to plot a strip plot ####
         ####### First, Plot each Continuous variable against the Target Variable ###
         if len(dft) < 1000:
             jitter = 0.05
         else:
             jitter = 0.5
         image_count = 0
         noplots = len(nums)
-        rows = int((noplots/cols)+0.99)
+        rows = int((noplots / cols) + 0.99)
         ### Be very careful with the next line. we have used the singular "subplot" ##
-        fig = plt.figure(figsize=(width_size,rows*height_size))
+        fig = plt.figure(figsize=(width_size, rows * height_size))
         sns.set_palette("Set1")
-        for num, plotc, color_val in zip(nums, range(1,noplots+1),colors):
+        for num, plotc, color_val in zip(nums, range(1, noplots + 1), colors):
             ####Strip plots are meant for categorical plots so x axis must always be depVar ##
-            plt.subplot(rows,cols,plotc)
+            plt.subplot(rows, cols, plotc)
             ### Don't change this line - it works properly now Dec 20, 2023 ####
             sns.stripplot(data=dft, x=dep, y=num, hue=dep, ax=plt.gca(), jitter=jitter)
             plt.xticks(rotation=30, ha='right', fontsize=9)
             plt.ylabel(num)
             plt.xlabel(dep)
-        plt.suptitle('Scatter Plot of Continuous Variable vs Target (jitter=%0.2f)' %jitter, fontsize=15,y=1.01)
-        fig.tight_layout();
+        plt.suptitle('Scatter Plot of Continuous Variable vs Target (jitter=%0.2f)' % jitter, fontsize=15, y=1.01)
+        fig.tight_layout()
         if verbose <= 1:
-            plt.show();
+            plt.show()
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name, dep, mk_dir))
+                                                plot_name, mk_dir))
             image_count += 1
     ####### End of Scatter Plots ######
     return imgdata_list
 
+
 # PAIR SCATTER PLOTS ARE NEEDED ONLY FOR CLASSIFICATION PROBLEMS IN NUMERIC VARIABLES
-def draw_pair_scatters(dfin,nums,problem_type, verbose,chart_format, dep=None, classes=None, lowess=False, mk_dir=None):
+def draw_pair_scatters(dfin, nums, problem_type, verbose, chart_format, dep=None, classes=None, lowess=False,
+                       mk_dir=None):
     """
     ### This is where you plot a pair-wise scatter plot of Independent Variables against each other####
     """
     plot_name = 'Pair_Scatter_Plots'
     dft = dfin[:]
     classes = copy.deepcopy(classes)
     cols = 2
     colortext = 'brymcgkbyrcmgkbyrcmgkbyrcmgkbyr'
     colors = cycle(colortext)
     imgdata_list = list()
     width_size = 15
     height_size = 4
     N = len(nums)
-    if dfin.shape[0] >= 10000 or lowess == False:
-        x_est = None
-        transparent =0.7
-        bubble_size = 80
+    if dfin.shape[0] >= 10000 or lowess is False:
+        transparent = 0.7
     elif lowess:
         print('Using Lowess Smoothing. This might take a few minutes for large data sets...')
-        x_est = None
-        transparent =0.7
-        bubble_size = 100
-    else:
-        x_est = None
-        transparent =0.7
-        bubble_size = 100
+        transparent = 0.7
+    else:
+        transparent = 0.7
     if verbose <= 1:
-        x_est = np.mean
+        pass
     if problem_type == 'Regression' or problem_type == 'Clustering':
         image_count = 0
         ### Second, plot a pair-wise scatter plot of Independent Variables against each other####
         combos = combinations(nums, 2)
-        noplots = int((N**2-N)/2)
-        print('Number of All Scatter Plots = %d' %(noplots+N))
-        rows = int((noplots/cols)+0.99)
-        fig = plt.figure(figsize=(width_size,rows*height_size))
-        for (var1,var2), plotcounter,color_val in zip(combos, range(1,noplots+1),colors):
+        noplots = int((N ** 2 - N) / 2)
+        print('Number of All Scatter Plots = %d' % (noplots + N))
+        rows = int((noplots / cols) + 0.99)
+        fig = plt.figure(figsize=(width_size, rows * height_size))
+        for (var1, var2), plotcounter, color_val in zip(combos, range(1, noplots + 1), colors):
             ### Be very careful with the next line. It should be singular "subplot" ##
             ##### Otherwise, if you use the plural version "subplots" it has a different meaning!
-            plt.subplot(rows,cols,plotcounter)
+            plt.subplot(rows, cols, plotcounter)
             if lowess:
                 sns.regplot(x=dft[var1], y=dft[var2], lowess=lowess, color=color_val, ax=plt.gca())
             else:
-                sns.scatterplot(x=dft[var1], y=dft[var2], ax=plt.gca(), palette='dark',color=color_val)
+                sns.scatterplot(x=dft[var1], y=dft[var2], ax=plt.gca(), palette='dark', color=color_val)
             plt.xlabel(var1)
             plt.ylabel(var2)
-        fig.suptitle('Pair-wise Scatter Plot of all Continuous Variables', fontsize=15,y=1.01)
-        fig.tight_layout();
+        fig.suptitle('Pair-wise Scatter Plot of all Continuous Variables', fontsize=15, y=1.01)
+        fig.tight_layout()
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name, dep, mk_dir))
+                                                plot_name, mk_dir))
             image_count += 1
         if verbose <= 1:
-            plt.show();
+            plt.show()
     else:
         ########## This is for Classification problems ##########
         if len(classes) <= 1:
             leng = 1
         else:
             leng = len(classes)
         colors = cycle(colortext[:leng])
         image_count = 0
-        #cmap = plt.get_cmap('gnuplot')
-        #cmap = plt.get_cmap('Set1')
-        cmap = plt.get_cmap('Paired')
+        # cmap = plt.get_cmap('gnuplot')
+        # cmap = plt.get_cmap('Set1')
         combos = combinations(nums, 2)
-        combos_cycle = cycle(combos)
-        noplots = int((N**2-N)/2)
-        print('Total Number of Scatter Plots = %d' %(noplots+N))
-        rows = int((noplots/cols)+0.99)
-        fig = plt.figure(figsize=(width_size,rows*height_size))
+        noplots = int((N ** 2 - N) / 2)
+        print('Total Number of Scatter Plots = %d' % (noplots + N))
+        rows = int((noplots / cols) + 0.99)
+        fig = plt.figure(figsize=(width_size, rows * height_size))
         ### Be very careful with the next line. we have used the plural "subplots" ##
         ## In this case, you have ax as an array and you have to use (row,col) to get each ax!
         target_vars = dft[dep].unique()
-        number = len(target_vars)
-        #colors = [cmap(i) for i in np.linspace(0, 1, number)]
-        for (var1,var2), plotc in zip(combos, range(1,noplots+1)):
+        # colors = [cmap(i) for i in np.linspace(0, 1, number)]
+        for (var1, var2), plotc in zip(combos, range(1, noplots + 1)):
             for target_var, color_val, class_label in zip(target_vars, colors, classes):
-                #Fix color in all scatter plots for each class the same using this trick
+                # Fix color in all scatter plots for each class the same using this trick
                 color_array = np.empty(0)
-                value = dft[dep]==target_var
-                dft['color'] = np.where(value==True, color_val, 'r')
-                color_array = np.hstack((color_array, dft[dft['color']==color_val]['color'].values))
+                value = dft[dep] == target_var
+                dft['color'] = np.where(value is True, color_val, 'r')
                 plt.subplot(rows, cols, plotc)
-                plt.scatter(x=dft.loc[dft[dep]==target_var][var1], y=dft.loc[dft[dep]==target_var][var2],
-                             label=class_label, color=color_val, alpha=transparent)
+                plt.scatter(x=dft.loc[dft[dep] == target_var][var1], y=dft.loc[dft[dep] == target_var][var2],
+                            label=class_label, color=color_val, alpha=transparent)
                 plt.xlabel(var1)
                 plt.ylabel(var2)
                 plt.legend()
-        fig.suptitle('Pair-wise Scatter Plot of all Continuous Variables',fontsize=15,y=1.01)
-        #fig.tight_layout();
+        fig.suptitle('Pair-wise Scatter Plot of all Continuous Variables', fontsize=15, y=1.01)
+        # fig.tight_layout();
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name, dep, mk_dir))
+                                                plot_name, mk_dir))
             image_count += 1
         if verbose <= 1:
-            plt.show();
+            plt.show()
     ####### End of Pair Scatter Plots ######
     return imgdata_list
 
-#Bar Plots are for 2 Categoricals and One Numeric (usually Dep Var)
-def plot_fast_average_num_by_cat(dft, cats, num_vars, verbose=0,kind="bar"):
+
+# Bar Plots are for 2 Categoricals and One Numeric (usually Dep Var)
+def plot_fast_average_num_by_cat(dft, cats, num_vars, verbose=0, kind="bar"):
     """
     Great way to plot continuous variables fast grouped by a categorical variable. Just sent them in and it will take care of the rest!
     """
     chunksize = 20
     stringlimit = 20
     col = 2
-    width_size = 15
-    height_size = 4
-    N = int(len(num_vars)*len(cats))
+    N = int(len(num_vars) * len(cats))
     colors = cycle('byrcmgkbyrcmgkbyrcmgkbyrcmgk')
     if N % 2 == 0:
-        row = N//col
+        row = N // col
     else:
-        row = int(N//col + 1)
+        row = int(N // col + 1)
     fig = plt.figure()
     if kind == 'bar':
-        fig.suptitle('Bar plots for each Continuous by each Categorical variable', fontsize=15,y=1.01)
+        fig.suptitle('Bar plots for each Continuous by each Categorical variable', fontsize=15, y=1.01)
     else:
-        fig.suptitle('Time Series plots for all date-time vars %s' %cats, fontsize=15,y=1.01)
+        fig.suptitle('Time Series plots for all date-time vars %s' % cats, fontsize=15, y=1.01)
     if col < 2:
-        fig.set_size_inches(min(15,8),row*5)
-        fig.subplots_adjust(hspace=0.5) ### This controls the space betwen rows
-        fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
-    else:
-        fig.set_size_inches(min(col*10,20),row*5)
-        fig.subplots_adjust(hspace=0.5) ### This controls the space betwen rows
-        fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
+        fig.set_size_inches(min(15, 8), row * 5)
+        fig.subplots_adjust(hspace=0.5)  ### This controls the space between rows
+        fig.subplots_adjust(wspace=0.3)  ### This controls the space between columns
+    else:
+        fig.set_size_inches(min(col * 10, 20), row * 5)
+        fig.subplots_adjust(hspace=0.5)  ### This controls the space between rows
+        fig.subplots_adjust(wspace=0.3)  ### This controls the space between columns
     counter = 1
     for cat in cats:
         for each_conti in num_vars:
             color3 = next(colors)
             try:
                 ax1 = plt.subplot(row, col, counter)
                 if kind == "bar":
                     data = dft.groupby(cat)[each_conti].mean().sort_values(
-                            ascending=False).head(chunksize)
-                    data.plot(kind=kind,ax=ax1,color=color3)
+                        ascending=False).head(chunksize)
+                    data.plot(kind=kind, ax=ax1, color=color3)
                 elif kind == "line":
                     data = dft.groupby(cat)[each_conti].mean().sort_index(
-                            ascending=True).head(chunksize)
-                    data.plot(kind=kind,ax=ax1,color=color3)
+                        ascending=True).head(chunksize)
+                    data.plot(kind=kind, ax=ax1, color=color3)
                 if dft[cat].dtype == object or str(dft[cat].dtype) in ['category']:
                     labels = data.index.str[:stringlimit].tolist()
                 else:
                     labels = data.index.tolist()
                 ax1.set_xlabel("")
-                ax1.set_xticklabels(labels,fontdict={'fontsize':9}, rotation = 45, ha="right")
-                ax1.set_title('Average %s by %s (Top %d)' %(each_conti,cat,chunksize))
+                ax1.set_xticklabels(labels, fontdict={'fontsize': 9}, rotation=45, ha="right")
+                ax1.set_title('Average %s by %s (Top %d)' % (each_conti, cat, chunksize))
                 counter += 1
             except:
-                ax1.set_title('No plot as %s is not numeric' %each_conti)
+                ax1.set_title('No plot as %s is not numeric' % each_conti)
                 counter += 1
     if verbose <= 1:
         plt.show()
     if verbose == 2:
         return fig
-################# The barplots module below calls the plot_fast_average_num_by_cat module above ###
-def draw_barplots(dft,cats,conti,problem_type,verbose,chart_format,dep='', classes=None, mk_dir=None):
 
+
+################# The barplots module below calls the plot_fast_average_num_by_cat module above ###
+def draw_barplots(dft, cats, conti, problem_type, verbose, chart_format, dep='', mk_dir=None):
     cats = cats[:]
     conti = conti[:]
     plot_name = 'Bar_Plots'
     #### Category limit within a variable ###
     #### Remove Floating Point Categorical Vars from this list since they Error when Bar Plots are drawn
     cats = [x for x in cats if dft[x].dtype != float]
     dft = dft[:]
-    N = len(cats)
     if len(cats) == 0 or len(conti) == 0:
         print('No categorical or numeric vars in data set. Hence no bar charts.')
         return None
     cmap = plt.get_cmap('jet')
     ### Not sure why the cmap doesn't work and gives an error in some cases #################
-    colors = cmap(np.linspace(0, 1, len(conti)))
-    colors = cycle('gkbyrcmgkbyrcmgkbyrcmgkbyr')
-    colormaps = ['plasma','viridis','inferno','magma']
     imgdata_list = list()
-    cat_limit = 10
-    conti = list_difference(conti,dep)
+    conti = list_difference(conti, dep)
     #### Make sure that you plot charts for the depVar as well by including it #######
     if problem_type == 'Regression':
         conti.append(dep)
     elif problem_type.endswith('Classification'):
         cats.append(dep)
     else:
         ### Since there is no dependent variable in clustering there is nothing to add dep to.
         pass
-    chunksize = 20
     ########## This is for Regression Problems only ######
     image_count = 0
     figx = plot_fast_average_num_by_cat(dft, cats, conti, verbose)
     if verbose == 2:
         imgdata_list.append(save_image_data(figx, chart_format,
-                            plot_name, dep, mk_dir))
+                                            plot_name, mk_dir))
         image_count += 1
     return imgdata_list
+
+
 ############## End of Bar Plotting ##########################################
 ##### Draw a Heatmap using Pearson Correlation #########################################
-def draw_heatmap(dft, conti, verbose,chart_format,datevars=[], dep=None,
-                                    modeltype='Regression',classes=None, mk_dir=None):
+def draw_heatmap(dft, conti, verbose, chart_format, datevars: list, dep=None,
+                 modeltype='Regression', mk_dir=None):
     ### Test if this is a time series data set, then differene the continuous vars to find
     ###  if they have true correlation to Dependent Var. Otherwise, leave them as is
     plot_name = 'Heat_Maps'
     width_size = 3
     height_size = 2
     timeseries_flag = False
     if len(conti) <= 1:
         return
-    if isinstance(dft.index, pd.DatetimeIndex) :
+    if isinstance(dft.index, pd.DatetimeIndex):
         dft = dft[:]
         timeseries_flag = True
         pass
     elif len(datevars) > 0:
         dft = dft[:]
         try:
-            dft.index = pd.to_datetime(dft.pop(datevars[0]),infer_datetime_format=True)
+            dft.index = pd.to_datetime(dft.pop(datevars[0]), infer_datetime_format=True)
             timeseries_flag = True
         except:
             if verbose >= 1 and len(datevars) > 0:
-                print('No date vars could be found or %s could not be indexed.' %datevars)
+                print('No date vars could be found or %s could not be indexed.' % datevars)
             timeseries_flag = False
     # Add a column: the color depends on target variable but you can use whatever function
     imgdata_list = list()
     if modeltype.endswith('Classification'):
         ########## This is for Classification problems only ###########
         if dft[dep].dtype == object or dft[dep].dtype == np.int64:
             dft[dep] = dft[dep].factorize()[0]
         image_count = 0
         N = len(conti)
-        target_vars = dft[dep].unique()
-        fig = plt.figure(figsize=(min(N*width_size,20),min(N*height_size,20)))
+        fig = plt.figure(figsize=(min(N * width_size, 20), min(N * height_size, 20)))
         if timeseries_flag:
-            fig.suptitle('Time Series: Heatmap of all Differenced Continuous vars for target = %s' %dep, fontsize=15,y=1.01)
+            fig.suptitle('Time Series: Heatmap of all Differenced Continuous vars for target = %s' % dep, fontsize=15,
+                         y=1.01)
         else:
-            fig.suptitle('Heatmap of all Numeric Variables with target: %s' %dep, fontsize=15,y=1.01)
+            fig.suptitle('Heatmap of all Numeric Variables with target: %s' % dep, fontsize=15, y=1.01)
         plotc = 1
-        #rows = len(target_vars)
+        # rows = len(target_vars)
         rows = 1
         cols = 1
         if timeseries_flag:
-            dft_target = dft[[dep]+conti].diff()
+            dft_target = dft[[dep] + conti].diff()
         else:
             dft_target = dft[conti]
             dft_target[dep] = dft[dep].values
         corr = dft_target.corr()
         plt.subplot(rows, cols, plotc)
         ax1 = plt.gca()
-        sns.heatmap(corr, annot=True,ax=ax1)
+        sns.heatmap(corr, annot=True, ax=ax1)
         plotc += 1
-        fig.tight_layout();
+        fig.tight_layout()
         if verbose <= 1:
-            plt.show();
+            plt.show()
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name, dep, mk_dir))
+                                                plot_name, mk_dir))
             image_count += 1
     else:
         ### This is for Regression and None Dep variable problems only ##
         image_count = 0
-        if dep == None or dep == '':
+        if dep is None or dep == '':
             pass
         else:
             conti += [dep]
         dft_target = dft[conti]
         if timeseries_flag:
             dft_target = dft_target.diff().dropna()
         else:
             dft_target = dft_target[:]
         N = len(conti)
-        fig = plt.figure(figsize=(min(20,N*width_size),min(20,N*height_size)))
+        fig = plt.figure(figsize=(min(20, N * width_size), min(20, N * height_size)))
         corr = dft_target.corr()
         sns.heatmap(corr, annot=True)
         if timeseries_flag:
-            fig.suptitle('Time Series Data: Heatmap of Differenced Continuous vars including target = %s' %dep, fontsize=15,y=1.01)
+            fig.suptitle('Time Series Data: Heatmap of Differenced Continuous vars including target = %s' % dep,
+                         fontsize=15, y=1.01)
         else:
-            fig.suptitle('Heatmap of all Numeric Variables including target: %s' %dep,fontsize=15,y=1.01)
-        fig.tight_layout();
+            fig.suptitle('Heatmap of all Numeric Variables including target: %s' % dep, fontsize=15, y=1.01)
+        fig.tight_layout()
         if verbose <= 1:
-            plt.show();
+            plt.show()
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name, dep, mk_dir))
+                                                plot_name, mk_dir))
             image_count += 1
     return imgdata_list
     ############# End of Heat Maps ##############
 
+
 ##### Draw the Distribution of each variable using Distplot
 ##### Must do this only for Continuous Variables
-from scipy.stats import probplot,skew
-def draw_distplot(dft, cat_bools, conti, verbose,chart_format,problem_type,dep=None, classes=None, mk_dir=None):
-    cats = find_remove_duplicates(cat_bools) ### first make sure there are no duplicates in this ###
+from scipy.stats import probplot
+
+
+def draw_distplot(dft, cat_bools, conti, verbose, chart_format, problem_type, dep=None, classes=None, mk_dir=None):
+    cats = find_remove_duplicates(cat_bools)  ### first make sure there are no duplicates in this ###
     copy_cats = copy.deepcopy(cats)
     conti = copy.deepcopy(conti)
     plot_name = 'Dist_Plots'
     #### Since we are making changes to dft and classes, we will be making copies of it here
     conti = list(set(conti))
     dft = dft[:]
     classes = copy.deepcopy(classes)
     colors = cycle('brycgkbyrcmgkbyrcmgkbyrcmgkbyr')
     imgdata_list = list()
     width_size = 15  #### this is to control the width of chart as well as number of categories to display
     height_size = 5
-    gap = 0.4 #### This controls the space between rows  ######
-    
-    if dep is None or dep=='' or problem_type == 'Regression':
+    gap = 0.4  #### This controls the space between rows  ######
+
+    if dep is None or dep == '' or problem_type == 'Regression':
         image_count = 0
-        transparent = 0.7
         ######### This is for cases where there is No Target or Dependent Variable ########
         if problem_type == 'Regression':
-            if isinstance(dep,list):
+            if isinstance(dep, list):
                 conti += dep
             else:
                 conti += [dep]
         ### Be very careful with the next line. we have used the plural "subplots" ##
         ## In this case, you have ax as an array and you have to use (row,col) to get each ax!
         ########## This is where you insert the logic for distplots ##############
-        #sns.color_palette("Set1")
+        # sns.color_palette("Set1")
         sns.set_palette("Set1")
         ##### First draw all the numeric variables in row after row #############
         if len(conti) > 0:
             cols = 3
             rows = len(conti)
-            fig, axes = plt.subplots(rows, cols, figsize=(width_size,rows*height_size))
-            fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows            
+            fig, axes = plt.subplots(rows, cols, figsize=(width_size, rows * height_size))
+            fig.subplots_adjust(hspace=gap)  ### This controls the space between rows
             k = 1
             binsize = 30
             for each_conti in conti:
                 color1 = next(colors)
                 ax1 = plt.subplot(rows, cols, k)
                 dft[each_conti].hist(
-                    bins=binsize, 
-                #sns.histplot(dft[each_conti],
-                    #kde=False,
-                #    kde=True, stat="density", linewidth=0,
+                    bins=binsize,
+                    # sns.histplot(dft[each_conti],
+                    # kde=False,
+                    #    kde=True, stat="density", linewidth=0,
                     ax=ax1, color=color1)
                 k += 1
                 ax2 = plt.subplot(rows, cols, k)
                 sns.boxplot(dft[each_conti], ax=ax2, color=color1)
                 k += 1
                 ax3 = plt.subplot(rows, cols, k)
                 probplot(dft[each_conti], plot=ax3)
                 k += 1
-                skew_val=round(dft[each_conti].skew(), 1)
+                skew_val = round(dft[each_conti].skew(), 1)
                 ax2.set_yticklabels([])
                 ax2.set_yticks([])
                 ax1.set_title(each_conti + " | Distplot", fontsize=9)
                 ax2.set_title(each_conti + " | Boxplot", fontsize=9)
-                ax3.set_title(each_conti + " | Probability Plot - Skew: "+str(skew_val), fontsize=9)
+                ax3.set_title(each_conti + " | Probability Plot - Skew: " + str(skew_val), fontsize=9)
             ###### Save the plots to disk if verbose = 2 ############
             if verbose == 2:
                 imgdata_list.append(save_image_data(fig, chart_format,
-                                plot_name+'_Numeric', dep, mk_dir))
+                                                    plot_name + '_Numeric', mk_dir))
                 image_count += 1
         #####  Now draw each of the categorical variable distributions in each subplot ####
         if len(cats) > 0:
             cols = 2
             noplots = len(cats)
-            rows = int((noplots/cols)+0.99 )
+            rows = int((noplots / cols) + 0.99)
             k = 0
-            fig = plt.figure(figsize=(width_size,rows*height_size))
-            fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows            
+            fig = plt.figure(figsize=(width_size, rows * height_size))
+            fig.subplots_adjust(hspace=gap)  ### This controls the space between rows
             for each_cat in copy_cats:
                 color2 = next(colors)
-                ax1 = plt.subplot(rows, cols, k+1)
-                kwds = {"rotation": 45, "ha":"right"}
+                ax1 = plt.subplot(rows, cols, k + 1)
+                kwds = {"rotation": 45, "ha": "right"}
                 ### In some small datasets, we get floats as categories since there are so few categories.
-                if dft[each_cat].dtype in ['float16','float32','float64']:
+                if dft[each_cat].dtype in ['float16', 'float32', 'float64']:
                     ### In those cases, we must remove the width_size since it thinks they are an index and errors.
-                    dft[each_cat].value_counts(normalize=True, dropna=False).plot(kind='bar', 
-                                            color=color2,
-                                            ax=ax1,label='%s' %each_cat)
+                    dft[each_cat].value_counts(normalize=True, dropna=False).plot(kind='bar',
+                                                                                  color=color2,
+                                                                                  ax=ax1, label='%s' % each_cat)
                     labels = dft[each_cat].value_counts(dropna=False).index.tolist()
                 else:
-                    dft[each_cat].value_counts(normalize=True, dropna=False)[:width_size].plot(kind='bar', 
-                                            color=color2,
-                                            ax=ax1,label='%s' %each_cat)
+                    dft[each_cat].value_counts(normalize=True, dropna=False)[:width_size].plot(kind='bar',
+                                                                                               color=color2,
+                                                                                               ax=ax1,
+                                                                                               label='%s' % each_cat)
                     labels = dft[each_cat].value_counts(dropna=False)[:width_size].index.tolist()
                 k += 1
-                ax1.set_xticklabels(labels,**kwds);
-                ax1.set_title('Norm. disti.of %s (top %d categories only)' %(each_cat,width_size), fontsize=9)
-            fig.tight_layout();
-            
+                ax1.set_xticklabels(labels, **kwds)
+                ax1.set_title('Norm. disti.of %s (top %d categories only)' % (each_cat, width_size), fontsize=9)
+            fig.tight_layout()
+
             ########## This is where you end the logic for distplots ################
             if verbose == 2:
                 imgdata_list.append(save_image_data(fig, chart_format,
-                                plot_name+'_Cats', dep, mk_dir))
+                                                    plot_name + '_Cats', mk_dir))
                 image_count += 1
             fig.suptitle('Histograms and Normalized distribitions of all variables', fontsize=12, y=1.01)
             if verbose <= 1:
-                plt.show();
+                plt.show()
     else:
         ######### This is for Classification problems only ########
         #### Now you can draw both object and numeric variables using same conti variable
-        #sns.color_palette("Set1")
+        # sns.color_palette("Set1")
         sns.set_palette("Set1")
         conti = conti + cats
         cols = 2
         image_count = 0
-        transparent = 0.7
         noplots = len(conti)
-        binsize = 30
-        k = 0
-        rows = int((noplots/cols)+0.99 )
+        rows = int((noplots / cols) + 0.99)
         ### Be very careful with the next line. we have used the plural "subplots" ##
         ## In this case, you have ax as an array and you have to use (row,col) to get each ax!
-        fig = plt.figure(figsize=(width_size,rows*height_size))
+        fig = plt.figure(figsize=(width_size, rows * height_size))
         target_vars = dft[dep].unique()
-        if type(classes[0])==int:
+        if type(classes[0]) == int:
             classes = [str(x) for x in classes]
         label_limit = len(target_vars)
         legend_flag = 1
         row_ticks = dft[dep].unique().tolist()
         ######## This is where each of the distribution plots for all kinds of vars is plotted ##       
         color_list = []
         for i in range(len(row_ticks)):
             color_list.append(next(colors))
-        for each_conti,k in zip(conti,range(len(conti))):
+        for each_conti, k in zip(conti, range(len(conti))):
             if dft[each_conti].isnull().sum() > 0:
                 if str(dft[each_conti].dtype) in ['category']:
                     ls = dft[each_conti].unique().astype(str)
                     dft[each_conti] = dft[each_conti].astype(pd.CategoricalDtype(ls))
                     ### Remember that fillna only works at dataframe level! ###
                     dft[[each_conti]] = dft[[each_conti]].fillna("nan").astype('category')
                 elif dft[each_conti].dtype == 'object':
                     ### Remember that fillna only works at dataframe level! ###
                     dft[[each_conti]] = dft[[each_conti]].fillna("nan")
                 else:
                     dft[[each_conti]] = dft[[each_conti]].fillna(0)
-            plt.subplot(rows, cols, k+1)
+            plt.subplot(rows, cols, k + 1)
             ax1 = plt.gca()
-            
-            if dft[each_conti].dtype==object:
-                kwds = {"rotation": 45, "ha":"right"}
-                labels = dft[each_conti].value_counts()[:width_size].index.tolist()
-                conti_df = dft[[dep,each_conti]].groupby([dep,each_conti]).size().nlargest(width_size).reset_index(name='Values')
+
+            if dft[each_conti].dtype == object:
+                conti_df = dft[[dep, each_conti]].groupby([dep, each_conti]).size().nlargest(width_size).reset_index(
+                    name='Values')
                 pivot_df = conti_df.pivot(index=each_conti, columns=dep, values='Values')
                 ### row_ticks must be modified since some values of dep are missing in conti_df
                 row_ticks = conti_df[dep].unique().tolist()
-                pivot_df.loc[:,row_ticks].plot.bar(stacked=True, 
-                    color=color_list, 
-                    ax=ax1)
-                #dft[each_conti].value_counts()[:width_size].plot(kind='bar',ax=ax1,
+                pivot_df.loc[:, row_ticks].plot.bar(stacked=True,
+                                                    color=color_list,
+                                                    ax=ax1)
+                # dft[each_conti].value_counts()[:width_size].plot(kind='bar',ax=ax1,
                 #                    label=class_label)
-                #ax1.set_xticklabels(labels,**kwds);
-                ax1.set_title('Distribution of %s (top %d categories only)' %(each_conti,width_size))
+                # ax1.set_xticklabels(labels,**kwds);
+                ax1.set_title('Distribution of %s (top %d categories only)' % (each_conti, width_size))
             elif str(dft[each_conti].dtype) in ['category']:
-                kwds = {"rotation": 45, "ha":"right"}
-                labels = dft[each_conti].value_counts()[:width_size].index.tolist()
-                conti_df = dft[[dep,each_conti]].groupby([dep,each_conti]).size().nlargest(width_size).reset_index(name='Values')
+                conti_df = dft[[dep, each_conti]].groupby([dep, each_conti]).size().nlargest(width_size).reset_index(
+                    name='Values')
                 pivot_df = conti_df.pivot(index=each_conti, columns=dep, values='Values')
                 ### row_ticks must be modified since some values of dep are missing in conti_df
                 row_ticks = conti_df[dep].unique().tolist()
-                pivot_df.loc[:,row_ticks].plot.bar(stacked=True, 
-                    color=color_list,
-                    ax=ax1)
-                #dft[each_conti].value_counts()[:width_size].plot(kind='bar',ax=ax1,
+                pivot_df.loc[:, row_ticks].plot.bar(stacked=True,
+                                                    color=color_list,
+                                                    ax=ax1)
+                # dft[each_conti].value_counts()[:width_size].plot(kind='bar',ax=ax1,
                 #                    label=class_label)
-                #ax1.set_xticklabels(labels,**kwds);
-                ax1.set_title('Distribution of %s (top %d categories only)' %(each_conti,width_size))
+                # ax1.set_xticklabels(labels,**kwds);
+                ax1.set_title('Distribution of %s (top %d categories only)' % (each_conti, width_size))
             else:
-                
-                for target_var, color2, class_label in zip(target_vars,color_list,classes):
+
+                for target_var, color2, class_label in zip(target_vars, color_list, classes):
                     try:
                         if legend_flag <= label_limit:
-                            sns.histplot(dft.loc[dft[dep]==target_var][each_conti],
-                                #hist=False, 
-                                kde=True, stat="density",
-                            #dft.loc[dft[dep]==target_var][each_conti].hist(
-                            #    bins=binsize, ax= ax1,
-                                label=target_var, 
-                                color=color2,
-                                )
-                            ax1.set_title('Distribution of %s' %each_conti)
+                            sns.histplot(dft.loc[dft[dep] == target_var][each_conti],
+                                         # hist=False,
+                                         kde=True, stat="density",
+                                         # dft.loc[dft[dep]==target_var][each_conti].hist(
+                                         #    bins=binsize, ax= ax1,
+                                         label=target_var,
+                                         color=color2,
+                                         )
+                            ax1.set_title('Distribution of %s' % each_conti)
                             legend_flag += 1
                         else:
-                            sns.kdeplot(dft.loc[dft[dep]==target_var][each_conti],
-                                #hist=False, 
-                                #kde=True, stat="density",
-                            #dft.loc[dft[dep]==target_var][each_conti].hist(
-                                #kde=True, stat="density", linewidth=0,
-                            #    bins=binsize, ax= ax1,
-                                label=target_var, 
-                                color=color2,
-                                )
+                            sns.kdeplot(dft.loc[dft[dep] == target_var][each_conti],
+                                        # hist=False,
+                                        # kde=True, stat="density",
+                                        # dft.loc[dft[dep]==target_var][each_conti].hist(
+                                        # kde=True, stat="density", linewidth=0,
+                                        #    bins=binsize, ax= ax1,
+                                        label=target_var,
+                                        color=color2,
+                                        )
                             legend_flag += 1
-                            ax1.set_title('Normed Histogram of %s' %each_conti)
+                            ax1.set_title('Normed Histogram of %s' % each_conti)
                     except:
                         pass
             ax1.legend(loc='best')
             k += 1
-        fig.tight_layout();
+        fig.tight_layout()
         if verbose <= 1:
-            plt.show();
+            plt.show()
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name+'_Numerics', dep, mk_dir))
+                                                plot_name + '_Numerics', mk_dir))
             image_count += 1
-        fig.suptitle('Histograms (KDE plots) of all Continuous Variables', fontsize=12,y=1.01)
+        fig.suptitle('Histograms (KDE plots) of all Continuous Variables', fontsize=12, y=1.01)
         ###### Now draw the distribution of the target variable in Classification only ####
         #####  Now draw each of the categorical variable distributions in each subplot ####
         ############################################################################
         if problem_type.endswith('Classification'):
             col = 2
             row = 1
-            fig, (ax1,ax2) = plt.subplots(row, col)
+            fig, (ax1, ax2) = plt.subplots(row, col)
             fig.set_figheight(5)
             fig.set_figwidth(15)
-            fig.suptitle('%s : Distribution of Target Variable' %dep, fontsize=12)
-            #fig.subplots_adjust(hspace=0.3) ### This controls the space betwen rows
-            #fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
+            fig.suptitle('%s : Distribution of Target Variable' % dep, fontsize=12)
+            # fig.subplots_adjust(hspace=0.3) ### This controls the space between rows
+            # fig.subplots_adjust(wspace=0.3) ### This controls the space between columns
             ###### Precentage Distribution is first #################
-            dft[dep].value_counts(1).plot(ax=ax1,kind='bar', color=color_list)
+            dft[dep].value_counts(1).plot(ax=ax1, kind='bar', color=color_list)
             if dft[dep].dtype == object:
                 dft[dep] = dft[dep].factorize()[0]
             for p in ax1.patches:
-                ax1.annotate(str(round(p.get_height(),2)), (round(p.get_x()*1.01,2), round(p.get_height()*1.01,2)))
-            #### Do not change the next 2 lines even though they may appear redundant. Otherwise it will error!
+                ax1.annotate(str(round(p.get_height(), 2)),
+                             (round(p.get_x() * 1.01, 2), round(p.get_height() * 1.01, 2)))
+            #### Do not change the next 2 lines even though they may appear redundant. Otherwise, it will error!
             if not str(dft[dep].dtype) in ['category']:
                 if dft[dep].dtype != object:
                     ax1.set_xticks(dft[dep].unique().tolist())
-            ax1.set_xticklabels(classes, rotation = 45, ha="right", fontsize=9)
-            ax1.set_title('Percentage Distribution of Target = %s' %dep, fontsize=10, y=1.05)
+            ax1.set_xticklabels(classes, rotation=45, ha="right", fontsize=9)
+            ax1.set_title('Percentage Distribution of Target = %s' % dep, fontsize=10, y=1.05)
             #### Freq Distribution is next ###########################
-            dft[dep].value_counts().plot(ax=ax2,kind='bar', color=color_list)
+            dft[dep].value_counts().plot(ax=ax2, kind='bar', color=color_list)
             for p in ax2.patches:
-                ax2.annotate(str(round(p.get_height(),2)), (round(p.get_x()*1.01,2), round(p.get_height()*1.01,2)))
-            #### Do not change the next 2 lines even though they may appear redundant. Otherwise it will error!
+                ax2.annotate(str(round(p.get_height(), 2)),
+                             (round(p.get_x() * 1.01, 2), round(p.get_height() * 1.01, 2)))
+            #### Do not change the next 2 lines even though they may appear redundant. Otherwise, it will error!
             if not str(dft[dep].dtype) in ['category']:
                 if dft[dep].dtype != object:
                     ax2.set_xticks(dft[dep].unique().tolist())
-            ax2.set_xticklabels(classes, rotation = 45, ha="right", fontsize=9)
-            ax2.set_title('Freq Distribution of Target Variable = %s' %dep,  fontsize=12)
+            ax2.set_xticklabels(classes, rotation=45, ha="right", fontsize=9)
+            ax2.set_title('Freq Distribution of Target Variable = %s' % dep, fontsize=12)
         elif problem_type == 'Regression':
             ############################################################################
             width_size = 5
             height_size = 5
-            fig = plt.figure(figsize=(width_size,height_size))
+            fig = plt.figure(figsize=(width_size, height_size))
             dft[dep].plot(kind='hist')
-            fig.suptitle('%s : Distribution of Target Variable' %dep, fontsize=12)
-            fig.tight_layout();
+            fig.suptitle('%s : Distribution of Target Variable' % dep, fontsize=12)
+            fig.tight_layout()
         else:
             return imgdata_list
         if verbose <= 1:
-            plt.show();
+            plt.show()
         if verbose == 2:
             imgdata_list.append(save_image_data(fig, chart_format,
-                            plot_name+'_target', dep, mk_dir))
+                                                plot_name + '_target', mk_dir))
             image_count += 1
     ####### End of Distplots ###########
     return imgdata_list
 
+
 ##### Standardize all the variables in One step. But be careful !
 #### All the variables must be numeric for this to work !!
-def draw_violinplot(df, dep, nums,verbose,chart_format, modeltype='Regression', mk_dir=None):
+def draw_violinplot(df, dep, nums, verbose, chart_format, modeltype='Regression', mk_dir=None):
     plot_name = 'Violin_Plots'
     df = df[:]
     number_in_each_row = 8
     imgdata_list = list()
     width_size = 15
     height_size = 4
     if type(dep) == str:
         othernums = [x for x in nums if x not in [dep]]
     else:
         othernums = [x for x in nums if x not in dep]
-    #sns.color_palette("Set1")
-    
+    # sns.color_palette("Set1")
+
     sns.set_palette("Set1")
-    if modeltype == 'Regression' or dep == None or dep == '':
+    if modeltype == 'Regression' or dep is None or dep == '':
         image_count = 0
         if modeltype == 'Regression':
             nums = nums + [dep]
         numb = len(nums)
         if numb > number_in_each_row:
-            rows = int((numb/number_in_each_row)+.99)
+            rows = int((numb / number_in_each_row) + .99)
         else:
             rows = 1
         plot_index = 0
         for row in range(rows):
             plot_index += 1
-            first_10 = number_in_each_row*row
+            first_10 = number_in_each_row * row
             next_10 = first_10 + number_in_each_row
             num_10 = nums[first_10:next_10]
             df10 = df[num_10]
-            df_norm = (df10 - df10.mean())/df10.std()
+            df_norm = (df10 - df10.mean()) / df10.std()
             if numb <= 5:
-                fig = plt.figure(figsize=(min(width_size*len(num_10),width_size),min(height_size,height_size*len(num_10))))
+                fig = plt.figure(
+                    figsize=(min(width_size * len(num_10), width_size), min(height_size, height_size * len(num_10))))
             else:
-                fig = plt.figure(figsize=(min(width_size*len(num_10),width_size),min(height_size,height_size*len(num_10))))
+                fig = plt.figure(
+                    figsize=(min(width_size * len(num_10), width_size), min(height_size, height_size * len(num_10))))
             ax = fig.gca()
-            #ax.set_xticklabels (df.columns, tolist(), size=10)
+            # ax.set_xticklabels (df.columns, tolist(), size=10)
             #### Don't change this line since it works to best now Dec 20, 2023 #####
             sns.violinplot(data=df_norm, orient='v', scale='width',
-                linewidth=3, ax=ax, inner='box')
+                           linewidth=3, ax=ax, inner='box')
             fig.suptitle('Violin Plot of all Continuous Variables', fontsize=15)
-            fig.tight_layout();
+            fig.tight_layout()
             if verbose <= 1:
-                plt.show();
+                plt.show()
             if verbose == 2:
-                additional = '_'+str(plot_index)+'_'
+                additional = '_' + str(plot_index) + '_'
                 imgdata_list.append(save_image_data(fig, chart_format,
-                                plot_name, dep, mk_dir, additional))
+                                                    plot_name, mk_dir, additional))
                 image_count += 1
-    else :
+    else:
         plot_name = "Box_Plots"
         ###### This is for Classification problems only ##########################
         image_count = 0
-        classes = df[dep].factorize()[1].tolist()
         ######################### Add Box plots here ##################################
         # Styling...
-        numb = len(nums)
-        target_vars = df[dep].unique()
-        target_len = df[dep].nunique()
         if len(othernums) >= 1:
             width_size = 15
             height_size = 7
             count = 0
-            data = pd.DataFrame(index=df.index)
             cols = 2
             noplots = len(nums)
-            rows = int((noplots/cols)+0.99 )
-            fig = plt.figure(figsize=(width_size,rows*height_size))
+            rows = int((noplots / cols) + 0.99)
+            fig = plt.figure(figsize=(width_size, rows * height_size))
             for col in nums:
-                ax = plt.subplot(rows,cols,count+1)
+                ax = plt.subplot(rows, cols, count + 1)
                 sns.boxplot(x=dep,
-                    y=col,
-                    data=df,
-                    ax=ax,
-                    linewidth=3, notch=False, saturation=0.5, showfliers=False)
-                ax.set_title('%s for each %s' %(col,dep))
+                            y=col,
+                            data=df,
+                            ax=ax,
+                            linewidth=3, notch=False, saturation=0.5, showfliers=False)
+                ax.set_title('%s for each %s' % (col, dep))
                 ax.set_xticklabels(df[dep].value_counts().index, rotation=30, ha='right', fontsize=9)
                 count += 1
-            fig.suptitle('Box Plots without Outliers shown',  fontsize=15)
-            fig.tight_layout();
+            fig.suptitle('Box Plots without Outliers shown', fontsize=15)
+            fig.tight_layout()
             if verbose <= 1:
-                plt.show();
+                plt.show()
             if verbose == 2:
                 imgdata_list.append(save_image_data(fig, chart_format,
-                                plot_name, dep, mk_dir))
+                                                    plot_name, mk_dir))
                 image_count += 1
         #########################################
     return imgdata_list
     ########## End of Violin Plots #########
 
+
 #### Drawing Date Variables is very important in Time Series data
-import copy
-def draw_date_vars(dfx,dep,datevars, num_vars,verbose, chart_format, modeltype='Regression', mk_dir=None):
-    
-    dfx = copy.deepcopy(dfx) ## use this to preserve the original dataframe
-    df =  copy.deepcopy(dfx) #### use this for making it into a datetime index etc...
+def draw_date_vars(dfx, dep, datevars, num_vars, verbose, chart_format, modeltype='Regression', mk_dir=None):
+    dfx = copy.deepcopy(dfx)  ## use this to preserve the original dataframe
+    df = copy.deepcopy(dfx)  #### use this for making it into a datetime index etc...
     ##### Fixed problems with number of plots no_plots. It now works well for regressions!
     plot_name = 'Time_Series_Plots'
     #### Now you want to display 2 variables at a time to see how they change over time
     ### Don't change the number of cols since you will have to change rows formula as well
-    gap = 0.3 ### adjusts the gap between rows in multiple rows of charts
+    gap = 0.3  ### adjusts the gap between rows in multiple rows of charts
     imgdata_list = list()
     image_count = 0
     N = len(num_vars)
-    chunksize = 20
     if N < 1 or len(datevars) == 0:
         #### If there are no numeric variables, nothing to plot here ######
         return imgdata_list
     else:
-        width_size = 15
-        height_size = 5
-    
-    if isinstance(df.index, pd.DatetimeIndex) :
+        pass
+
+    if isinstance(df.index, pd.DatetimeIndex):
         pass
     elif len(datevars) > 0:
         try:
             ts_column = datevars[0]
-            ### if we have already found that it was a date time var, then leave it as it is. Thats good enough!
+            ### if we have already found that it was a date time var, then leave it as it is. That's good enough!
             date_items = df[ts_column].apply(str).apply(len)
             try:
-                date_4_digit = (date_items==4).all() | (date_items==6).all()
+                date_4_digit = (date_items == 4).all() | (date_items == 6).all()
             except:
                 date_4_digit = False
             ### remove the next line it is not working well for non-4 digit dates
-            #date_4_digit = all(date_items[0] == item for item in date_items) ### this checks for 4 digits date
+            # date_4_digit = all(date_items[0] == item for item in date_items) ### this checks for 4 digits date
             #### In some cases, date time variable is a year like 1999 (4-digit), this must be translated correctly
             if date_4_digit:
                 if date_items[0] == 4:
                     ### If it is just a year variable alone, you should leave it as just a year!
-                    df[ts_column] = df[ts_column].map(lambda x: pd.to_datetime(x,format='%Y', errors='coerce')).values
+                    df[ts_column] = df[ts_column].map(lambda x: pd.to_datetime(x, format='%Y', errors='coerce')).values
                 else:
                     ### if it is not a year alone, then convert it into a date time variable
                     if df[ts_column].min() > 1900 or df[ts_column].max() < 2100:
-                        df[ts_column] = df[ts_column].map(lambda x: '0101'+str(x) if len(str(x)) == 4 else x)
+                        df[ts_column] = df[ts_column].map(lambda x: '0101' + str(x) if len(str(x)) == 4 else x)
                         df[ts_column] = pd.to_datetime(df[ts_column], format='%m%d%Y', errors='coerce')
                     else:
-                        print('%s could not be indexed. Could not draw date_vars.' %col)
+                        print(f'{ts_column} could not be indexed. Could not draw date_vars.')
                         return imgdata_list
             else:
                 df[ts_column] = pd.to_datetime(df[ts_column], infer_datetime_format=True, errors='coerce')
             ##### Now set the column to be the date - time index
-            df.index = df.pop(ts_column) #### This is where we set the date time column as the index ######
+            df.index = df.pop(ts_column)  #### This is where we set the date time column as the index ######
         except:
-            print('%s could not be indexed. Could not draw date_vars.' %col)
+            print(f'{ts_column} could not be indexed. Could not draw date_vars.')
             return imgdata_list
     ####### Draw the time series for Regression and DepVar
-    
+
     width_size = 15
     height_size = 4
     cols = 2
     if modeltype == 'Regression':
-        gap=0.5
+        gap = 0.5
         no_plots = df.groupby(ts_column).mean().shape[1]
-        rows = int((no_plots/cols)+0.99)
-        fig,ax = plt.subplots(figsize=(width_size,rows*height_size))
-        fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows
-        df.groupby(ts_column).mean().plot(subplots=True,ax=ax,layout=(rows,cols))
-        fig.suptitle('Time Series Plot for each Continuous Variable by %s' %ts_column, fontsize=15,y=1.01)
+        rows = int((no_plots / cols) + 0.99)
+        fig, ax = plt.subplots(figsize=(width_size, rows * height_size))
+        fig.subplots_adjust(hspace=gap)  ### This controls the space between rows
+        df.groupby(ts_column).mean().plot(subplots=True, ax=ax, layout=(rows, cols))
+        fig.suptitle('Time Series Plot for each Continuous Variable by %s' % ts_column, fontsize=15, y=1.01)
     elif modeltype == 'Clustering':
-        kind = 'line' #### you can change this to plot any kind of time series plot you want
+        kind = 'line'  #### you can change this to plot any kind of time series plot you want
         image_count = 0
         combos = combinations(num_vars, 2)
-        combs = copy.deepcopy(combos)
-        noplots = int((N**2-N)/2)
-        rows = int((noplots/cols)+0.99)
+        noplots = int((N ** 2 - N) / 2)
+        rows = int((noplots / cols) + 0.99)
         counter = 1
-        fig = plt.figure(figsize=(width_size,rows*height_size))
-        fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows
+        fig = plt.figure(figsize=(width_size, rows * height_size))
+        fig.subplots_adjust(hspace=gap)  ### This controls the space between rows
         try:
-            for (var1,var2) in combos:
-                plt.subplot(rows,cols,counter)
+            for (var1, var2) in combos:
+                plt.subplot(rows, cols, counter)
                 ax1 = plt.gca()
                 df[var1].plot(kind=kind, secondary_y=True, label=var1, ax=ax1)
-                df[var2].plot(kind=kind, title=var2 +' (left_axis) vs. ' + var1+' (right_axis)', ax=ax1)
+                df[var2].plot(kind=kind, title=var2 + ' (left_axis) vs. ' + var1 + ' (right_axis)', ax=ax1)
                 plt.legend(loc='best')
                 counter += 1
-                fig.suptitle('Time Series Plot by %s: Pairwise Continuous Variables' %ts_column, fontsize=15,y=1.01)
+                fig.suptitle('Time Series Plot by %s: Pairwise Continuous Variables' % ts_column, fontsize=15, y=1.01)
         except:
             plt.close('all')
-            fig = plot_fast_average_num_by_cat(dfx, datevars, num_vars, verbose,kind="line")
+            fig = plot_fast_average_num_by_cat(dfx, datevars, num_vars, verbose, kind="line")
     else:
         ######## This is for Classification problems only ####
-        kind = 'line' ### you can decide what kind of plots you want to show here ####
         image_count = 0
         target_vars = df[dep].factorize()[1].tolist()
-        #classes = copy.deepcopy(classes)
+        # classes = copy.deepcopy(classes)
         ##### Now separate out the drawing of time series data by the number of classes ###
-        colors = cycle('gkbyrcmgkbyrcmgkbyrcmgkbyr')
         classes = df[dep].unique()
-        if type(classes[0])==int or type(classes[0])==float:
-            classes = [str(x) for x in classes]
+        if type(classes[0]) == int or type(classes[0]) == float:
+            pass
         cols = 2
-        count = 0
         combos = combinations(num_vars, 2)
-        combs = copy.deepcopy(combos)
         noplots = len(target_vars)
-        rows = int((noplots/cols)+0.99)
-        fig = plt.figure(figsize=(width_size,rows*height_size))
-        fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows
+        rows = int((noplots / cols) + 0.99)
+        fig = plt.figure(figsize=(width_size, rows * height_size))
+        fig.subplots_adjust(hspace=gap)  ### This controls the space between rows
         counter = 1
         copy_target_vars = copy.deepcopy(target_vars)
         try:
             for target_var in copy_target_vars:
-                df_target = df[df[dep]==target_var]
-                ax1 = plt.subplot(rows,cols,counter)
-                df_target.groupby(ts_column).mean().plot(subplots=False,ax=ax1)
-                ax1.set_title('Time Series plots for '+dep + ' value = '+target_var)
+                df_target = df[df[dep] == target_var]
+                ax1 = plt.subplot(rows, cols, counter)
+                df_target.groupby(ts_column).mean().plot(subplots=False, ax=ax1)
+                ax1.set_title('Time Series plots for ' + dep + ' value = ' + target_var)
                 counter += 1
         except:
             plt.close('all')
-            fig = plot_fast_average_num_by_cat(df_target, datevars, num_vars, verbose,kind="line")
-        fig.suptitle('Time Series Plot by %s: Continuous Variables Pair' %ts_column, fontsize=15, y=1.01)
+            fig = plot_fast_average_num_by_cat(df_target, datevars, num_vars, verbose, kind="line")
+        fig.suptitle('Time Series Plot by %s: Continuous Variables Pair' % ts_column, fontsize=15, y=1.01)
     if verbose == 2:
         imgdata_list.append(save_image_data(fig, chart_format,
-                        plot_name, dep, mk_dir))
+                                            plot_name, mk_dir))
         image_count += 1
     return imgdata_list
+
+
 ############# End of Date vars plotting #########################
-def catscatter(data,colx,coly, ax, ratio=10,save=False,save_name='Default'):
+def catscatter(data, colx, coly, ax, ratio=10):
     """
     ####################################################################################
     # The catscatter idea was conceived by: Myr Barnés in 2020 
     # This idea is reused and modified here in AutoViz with sincere thanks to Myr Barnés.
     ####################################################################################
     The function draws catscatter plots for pairs of categorical variables in a data frame. 
     A catscatter plot is a type of scatter plot that shows the frequency of each combination 
@@ -1232,189 +1184,190 @@
     # aggregate record counts by different labels of cat_x and cat_y
     df = data.groupby([colx, coly]).size().reset_index(name='record_count')
     top_xticks = df[colx].value_counts().index[:length]
     top_yticks = df[coly].value_counts().index[:length]
     df = df[(df[colx].isin(top_xticks)) & (df[coly].isin(top_yticks))].reset_index(drop=True)
     cols = 'record_count'
     # define the color map
-    color=['red', 'green', 'grey']
-    font_size = 7
-    font='Helvetica'
-    # Create a dict to encode the categeories into numbers (sorted)
+    color = ['red', 'green', 'grey']
+    font = 'Helvetica'
+    # Create a dict to encode the categories into numbers (sorted)
     xticks = df[colx].sort_values().unique().tolist()
     yticks = df[coly].sort_values().unique().tolist()
-    
-    colx_codes=dict(zip(xticks,range(len(xticks))))
-    coly_codes=dict(zip(yticks,range(len(yticks))))
-    
+
+    colx_codes = dict(zip(xticks, range(len(xticks))))
+    coly_codes = dict(zip(yticks, range(len(yticks))))
+
     # Apply the encoding
-    df[colx]=df[colx].apply(lambda x: colx_codes[x])
-    df[coly]=df[coly].apply(lambda x: coly_codes[x])
-    
+    df[colx] = df[colx].apply(lambda x: colx_codes[x])
+    df[coly] = df[coly].apply(lambda x: coly_codes[x])
+
     # Prepare the aspect of the plot
-    #plt.rcParams['xtick.bottom'] = plt.rcParams['xtick.labelbottom'] = False
-    #plt.rcParams['xtick.top'] = plt.rcParams['xtick.labeltop'] = True
+    # plt.rcParams['xtick.bottom'] = plt.rcParams['xtick.labelbottom'] = False
+    # plt.rcParams['xtick.top'] = plt.rcParams['xtick.labeltop'] = True
     plt.rcParams['font.family'] = 'sans-serif'
     plt.rcParams['font.sans-serif'] = [font] + plt.rcParams['font.sans-serif']
-    plt.rcParams['xtick.color']=color[-1]
-    plt.rcParams['ytick.color']=color[-1]
+    plt.rcParams['xtick.color'] = color[-1]
+    plt.rcParams['ytick.color'] = color[-1]
     plt.box(False)
 
     plt.tick_params(
-        axis='x',          # changes apply to the x-axis
-        which='both',      # both major and minor ticks are affected
-        bottom=True,      # ticks along the bottom edge are off
-        top=False,         # ticks along the top edge are off
-        labelbottom=True) # labels along the bottom edge are off
+        axis='x',  # changes apply to the x-axis
+        which='both',  # both major and minor ticks are affected
+        bottom=True,  # ticks along the bottom edge are off
+        top=False,  # ticks along the top edge are off
+        labelbottom=True)  # labels along the bottom edge are off
 
     plt.tick_params(
-        axis='y',          # changes apply to the y-axis
-        which='major',      # both major and minor ticks are affected
-        left=False,      # ticks along the bottom edge are off
-        right=False,         # ticks along the top edge are off
-        ) # labels along the bottom edge are off
+        axis='y',  # changes apply to the y-axis
+        which='major',  # both major and minor ticks are affected
+        left=False,  # ticks along the bottom edge are off
+        right=False,  # ticks along the top edge are off
+    )  # labels along the bottom edge are off
 
     # Plot all the lines for the background
     for num in range(len(top_yticks)):
-        ax.hlines(num,-1,len(top_xticks),linestyle='dashed',linewidth=1,color=color[num%2],alpha=0.5)
+        ax.hlines(num, -1, len(top_xticks), linestyle='dashed', linewidth=1, color=color[num % 2], alpha=0.5)
     for num in range(len(top_xticks)):
-        ax.vlines(num,-1,len(top_yticks),linestyle='dashed',linewidth=1,color=color[num%2],alpha=0.5)
-        
-    
-    ax.set_xticklabels(['']+xticks[:length], rotation=15, ha='right', color=color[-1])
-    ax.set_xticks(range(-1,len(xticks)))
-    ax.set_yticklabels(['']+yticks[:length], rotation=15, ha='left', color=color[-1])
-    ax.set_yticks(range(-1,len(yticks)+1))
+        ax.vlines(num, -1, len(top_yticks), linestyle='dashed', linewidth=1, color=color[num % 2], alpha=0.5)
+
+    ax.set_xticklabels([''] + xticks[:length], rotation=15, ha='right', color=color[-1])
+    ax.set_xticks(range(-1, len(xticks)))
+    ax.set_yticklabels([''] + yticks[:length], rotation=15, ha='left', color=color[-1])
+    ax.set_yticks(range(-1, len(yticks) + 1))
 
     # Plot the scatter plot with the numbers
     ax.scatter(df[colx],
                df[coly],
-               s=df[cols]*ratio,
+               s=df[cols] * ratio,
                zorder=1,
                color=color[-1],
                )
-    ax.set_xlim(xmin=-1,xmax=len(colx_codes))
-    ax.set_ylim(ymin=-1,ymax=len(coly_codes))
+    ax.set_xlim(xmin=-1, xmax=len(colx_codes))
+    ax.set_ylim(ymin=-1, ymax=len(coly_codes))
     return ax
+
+
 ############################################################################
-def draw_catscatterplots(dft,cats, problem_type, verbose, 
-                chart_format, mk_dir=None):
+def draw_catscatterplots(dft, cats, verbose, chart_format, mk_dir=None):
     """
     The function draws catscatter plots for pairs of categorical variables in a data frame. 
     A catscatter plot is a type of scatter plot that shows the frequency of each combination 
     of categories in two variables. It can be useful for exploring the relationship between 
     categorical variables and identifying patterns or outliers.
     Args:
         dft (pandas.DataFrame): The data frame containing the categorical variables.
         cats (list): A list of column names of the categorical variables in dft.
-        problem_type (str): The type of problem to be solved, either 'classification' or 'regression'.
         verbose (int): The level of verbosity for displaying the plots. 0 means no plots, 1 means show plots, 2 means save plots as image files.
         chart_format (str): The format of the image files to be saved. Can be 'png', 'jpg', 'svg', etc.
         mk_dir (str, optional): The directory where the image files will be saved. Defaults to None.
 
     Returns:
         list: A list of image data objects for each catscatter plot if verbose == 2, otherwise an empty list.
     """
     imgdata_list = list()
-    image_count = 0
-    N = len(cats)
-    chunksize = 20
+    cat_len = len(cats)
+    plot_name = "catscatter plot"
     if len(cats) == 0:
         #### If there are no categorical variables, nothing to plot here ######
         return imgdata_list
     else:
         width_size = 15
         height_size = 5
     #### start drawing the catscatter here ###
     cols = 2
-    gap=0.5
+    gap = 0.5
     image_count = 0
     combos = combinations(cats, 2)
     combs = copy.deepcopy(combos)
-    noplots = int((N**2-N)/2)
-    rows = int((noplots/cols)+0.99)
+    noplots = int((cat_len ** 2 - cat_len) / 2)
+    rows = int((noplots / cols) + 0.99)
     counter = 1
-    fig = plt.figure(figsize=(width_size,rows*height_size))
-    fig.subplots_adjust(hspace=gap) ### This controls the space betwen rows
-    for (var1,var2) in combs:
+    fig = plt.figure(figsize=(width_size, rows * height_size))
+    fig.subplots_adjust(hspace=gap)  ### This controls the space between rows
+    for (var1, var2) in combs:
         try:
-            plt.subplot(rows,cols,counter)
+            plt.subplot(rows, cols, counter)
             ax1 = plt.gca()
             catscatter(dft, var1, var2, ax1, ratio=10)
-            ax1.set_title('Catscatter plot for '+var1 + '(X axis) vs. '+var2, fontsize=10)
+            ax1.set_title('Catscatter plot for ' + var1 + '(X axis) vs. ' + var2, fontsize=10)
             counter += 1
         except:
             plt.close('all')
     fig.suptitle('Catscatter plot of Pairs of Categorical Variables', fontsize=15, y=1.01)
     if verbose == 2:
-        imgdata_list.append(save_image_data(fig, chart_format,
-                        plot_name, dep, mk_dir))
+        imgdata_list.append(save_image_data(fig, chart_format, plot_name, mk_dir))
         image_count += 1
     return imgdata_list
 
+
 ######################################################################################
 # This little function classifies columns into 4 types: categorical, continuous, boolean and
 # certain columns that have only one value repeated that they are useless and must be removed from dataset
-#Subtract RIGHT_LIST from LEFT_LIST to produce a new list
+# Subtract RIGHT_LIST from LEFT_LIST to produce a new list
 ### This program is USED VERY HEAVILY so be careful about changing it
-def list_difference(l1,l2):
+def list_difference(l1, l2):
     lst = []
     for i in l1:
         if i not in l2:
             lst.append(i)
     return lst
 
+
 ######## Find ANY word in columns to identify ANY TYPE OF columns
 ####### search_for_list = ["Date","DATE", "date"], any words you want to search for it
 ####### columns__list and word refer to columns in the dataset that is the target dataset
 ####### Both columns_list and search_for_list must be lists - otherwise it won't work
 def search_for_word_in_list(columns_list, search_for_list):
     columns_list = columns_list[:]
     search_for_list = search_for_list[:]
-    lst=[]
+    lst = []
     for src in search_for_list:
         for word in columns_list:
-            result = re.findall (src, word)
-            if len(result)>0:
-                if word.endswith(src) and not word in lst:
+            result = re.findall(src, word)
+            if len(result) > 0:
+                if word.endswith(src) and word not in lst:
                     lst.append(word)
-            elif (word == 'id' or word == 'ID') and not word in lst:
+            elif (word == 'id' or word == 'ID') and word not in lst:
                 lst.append(word)
             else:
                 continue
     return lst
 
+
 ### This is a small program to look for keywords such as "id" in a dataset to see if they are ID variables
 ### If that doesn't work, it then compares the len of the dataframe to the variable's unique values. If
 ###	they match, it means that the variable could be an ID variable. If not, it goes with the name of
 ###	of the ID variable through a keyword match with "id" or some such keyword in dataset's columns.
 ###  This is a small program to look for keywords such as "id" in a dataset to see if they are ID variables
 ###    If that doesn't work, it then compares the len of the dataframe to the variable's unique values. If
 ###     they match, it means that the variable could be an ID variable. If not, it goes with the name of
 ###     of the ID variable through a keyword match with "id" or some such keyword in dataset's columns.
 
-def analyze_ID_columns(dfin,columns_list):
+def analyze_ID_columns(dfin, columns_list):
     columns_list = columns_list[:]
     dfin = dfin[:]
     IDcols_final = []
     IDcols = search_for_word_in_list(columns_list,
-        ['ID','Identifier','NUMBER','No','Id','Num','num','_no','.no','Number','number','_id','.id'])
-    if IDcols == []:
+                                     ['ID', 'Identifier', 'NUMBER', 'No', 'Id', 'Num', 'num', '_no', '.no', 'Number',
+                                      'number', '_id', '.id'])
+    if not IDcols:
         for eachcol in columns_list:
             if len(dfin) == len(dfin[eachcol].unique()) and dfin[eachcol].dtype != float:
                 IDcols_final.append(eachcol)
     else:
         for each_col in IDcols:
             if len(dfin) == len(dfin[each_col].unique()) and dfin[each_col].dtype != float:
                 IDcols_final.append(each_col)
     if IDcols_final == [] and IDcols != []:
         IDcols_final = IDcols
     return IDcols_final
 
-# THESE FUNCTIONS ASSUME A DIRTY DATASET" IN A PANDAS DATAFRAME AS Inum_j}lotsUT
+
+# THESE FUNCTIONS ASSUME A DIRTY DATASET IN A PANDAS DATAFRAME AS Inum_j}lotsUT
 # AND CONVERT THEM INTO A DATASET FIT FOR ANALYSIS IN THE END
 # In [ ]:
 # this function starts with dividing columns into 4 types: categorical, continuous, boolean and to_delete
 # The To_Delete columns have only one unique value and can be removed from the dataset
 def start_classifying_vars(dfin, verbose):
     dfin = dfin[:]
     cols_to_delete = []
@@ -1427,31 +1380,31 @@
         print('Error: No rows in dataset. Check your input again...')
         return cols_to_delete, boolean_vars, categorical_vars, continuous_vars, discrete_vars, dfin
     for col in dfin.columns:
         if col == 'source':
             continue
         elif len(dfin[col].value_counts()) <= 1:
             cols_to_delete.append(dfin[col].name)
-            print('    Column %s has only one value hence it will be dropped' %dfin[col].name)
-        elif dfin[col].dtype==object:
-            if (dfin[col].str.len()).any()>50:
+            print('    Column %s has only one value hence it will be dropped' % dfin[col].name)
+        elif dfin[col].dtype == object:
+            if (dfin[col].str.len()).any() > 50:
                 cols_to_delete.append(dfin[col].name)
                 continue
-            elif search_for_word_in_list([col],['DESCRIPTION','DESC','desc','Text','text']):
+            elif search_for_word_in_list([col], ['DESCRIPTION', 'DESC', 'desc', 'Text', 'text']):
                 cols_to_delete.append(dfin[col].name)
                 continue
             elif len(dfin.groupby(col)) == 1:
                 cols_to_delete.append(dfin[col].name)
                 continue
             elif dfin[col].isnull().sum() > 0:
-                missing_rows=dfin[col].isnull().sum()
-                pct_missing = float(missing_rows)/float(totrows)
+                missing_rows = dfin[col].isnull().sum()
+                pct_missing = float(missing_rows) / float(totrows)
                 if pct_missing > 0.90:
                     if verbose <= 1:
-                        print('Pct of Missing Values in %s exceed 90 pct, hence will be dropped...' %col)
+                        print('Pct of Missing Values in %s exceed 90 pct, hence will be dropped...' % col)
                     cols_to_delete.append(dfin[col].name)
                     continue
                 elif len(dfin.groupby(col)) == 2:
                     boolean_vars.append(dfin[col].name)
                     py_version = sys.version_info[0]
                     if py_version < 3:
                         # This is the Python 2 Version
@@ -1466,38 +1419,38 @@
 
                             item_mode = dfin[col].mode()[0]
                         except:
                             print('''Statistics package not installed in your Python3. Get it installed''')
                     ### Remember that fillna only works at dataframe level! ###
                     dfin[[col]] = dfin[[col]].fillna(item_mode)
                     continue
-                elif len(dfin.groupby(col)) < 20 and len(dfin.groupby(col)) > 1:
+                elif 20 > len(dfin.groupby(col)) > 1:
                     categorical_vars.append(dfin[col].name)
                     continue
                 else:
                     discrete_vars.append(dfin[col].name)
                     continue
             elif len(dfin.groupby(col)) == 2:
                 boolean_vars.append(dfin[col].name)
                 continue
-            elif len(dfin.groupby(col)) < 20 and len(dfin.groupby(col)) > 1:
+            elif 20 > len(dfin.groupby(col)) > 1:
                 categorical_vars.append(dfin[col].name)
                 continue
             else:
                 discrete_vars.append(dfin[col].name)
-        elif dfin[col].dtype=='int64' or dfin[col].dtype=='int32':
+        elif dfin[col].dtype == 'int64' or dfin[col].dtype == 'int32':
             if len(dfin[col].value_counts()) <= 15:
                 categorical_vars.append(dfin[col].name)
         else:
             if dfin[col].isnull().sum() > 0:
-                missing_rows=dfin[col].isnull().sum()
-                pct_missing = float(missing_rows)/float(totrows)
+                missing_rows = dfin[col].isnull().sum()
+                pct_missing = float(missing_rows) / float(totrows)
                 if pct_missing > 0.90:
                     if verbose <= 1:
-                        print('Pct of Missing Values in %s exceed 90 pct, hence will be dropped...' %col)
+                        print('Pct of Missing Values in %s exceed 90 pct, hence will be dropped...' % col)
                     cols_to_delete.append(dfin[col].name)
                     continue
                 elif len(dfin.groupby(col)) == 2:
                     boolean_vars.append(dfin[col].name)
                     py_version = sys.version_info[0]
                     if py_version < 3:
                         # This is the Python 2 Version
@@ -1527,769 +1480,786 @@
             else:
                 if len(dfin[col].value_counts()) <= 25 and len(dfin) >= 250:
                     categorical_vars.append(dfin[col].name)
                 else:
                     continuous_vars.append(dfin[col].name)
     return cols_to_delete, boolean_vars, categorical_vars, continuous_vars, discrete_vars, dfin
 
+
 #### this is the MAIN ANALYSIS function that calls the start_classifying_vars and then
 #### takes that result and divides categorical vars into 2 additional types: discrete vars and bool vars
-def analyze_columns_in_dataset(dfx,IDcolse,verbose):
+def analyze_columns_in_dataset(dfx, IDcolse, verbose):
     dfx = dfx[:]
     IDcolse = IDcolse[:]
-    cols_delete, bool_vars, cats, nums, discrete_string_vars, dft = start_classifying_vars(dfx,verbose)
+    cols_delete, bool_vars, cats, nums, discrete_string_vars, dft = start_classifying_vars(dfx, verbose)
     continuous_vars = nums
-    if nums != []:
+    if nums:
         for k in nums:
-            if len(dft[k].unique())==2:
+            if len(dft[k].unique()) == 2:
                 bool_vars.append(k)
-            elif len(dft[k].unique())<=20:
+            elif len(dft[k].unique()) <= 20:
                 cats.append(k)
-            elif (np.array(dft[k]).dtype=='float64' or np.array(dft[k]).dtype=='int64') and (k not in continuous_vars):
+            elif (np.array(dft[k]).dtype == 'float64' or np.array(dft[k]).dtype == 'int64') and (
+                    k not in continuous_vars):
                 if len(dft[k].value_counts()) <= 25:
                     cats.append(k)
                 else:
                     continuous_vars.append(k)
-            elif dft[k].dtype==object:
+            elif dft[k].dtype == object:
                 discrete_string_vars.append(k)
             elif k in continuous_vars:
                 continue
             else:
                 print('The %s variable could not be classified into any known type' % k)
-    #print(cols_delete, bool_vars, cats, continuous_vars, discrete_string_vars)
-    date_vars = search_for_word_in_list(dfx.columns.tolist(),['Date','DATE','date','TIME','time',
-                                                   'Time','Year','Yr','year','yr','timestamp',
-                                                   'TimeStamp','TIMESTAMP','Timestamp','Time Stamp'])
-    date_vars = [x for x in date_vars if x not in find_remove_duplicates(cats+bool_vars) ]
-    if date_vars == []:
+    # print(cols_delete, bool_vars, cats, continuous_vars, discrete_string_vars)
+    date_vars = search_for_word_in_list(dfx.columns.tolist(), ['Date', 'DATE', 'date', 'TIME', 'time',
+                                                               'Time', 'Year', 'Yr', 'year', 'yr', 'timestamp',
+                                                               'TimeStamp', 'TIMESTAMP', 'Timestamp', 'Time Stamp'])
+    date_vars = [x for x in date_vars if x not in find_remove_duplicates(cats + bool_vars)]
+    if not date_vars:
         for col in continuous_vars:
-            if dfx[col].dtype==int:
+            if dfx[col].dtype == int:
                 if dfx[col].min() > 1900 or dfx[col].max() < 2100:
                     date_vars.append(col)
         for col in discrete_string_vars:
             try:
                 dfx.index = pd.to_datetime(dfx.pop(col), infer_datetime_format=True)
             except:
                 continue
     if isinstance(dfx.index, pd.DatetimeIndex):
         date_vars = [dfx.index.name]
-    continuous_vars=list_difference(list_difference(continuous_vars,date_vars),IDcolse)
-    #cats =  list_difference(continuous_vars, cats)
-    cats=list_difference(cats,date_vars)
-    discrete_string_vars=list_difference(list_difference(discrete_string_vars,date_vars),IDcolse)
-    return cols_delete, bool_vars, cats, continuous_vars, discrete_string_vars,date_vars, dft
+    continuous_vars = list_difference(list_difference(continuous_vars, date_vars), IDcolse)
+    # cats =  list_difference(continuous_vars, cats)
+    cats = list_difference(cats, date_vars)
+    discrete_string_vars = list_difference(list_difference(discrete_string_vars, date_vars), IDcolse)
+    return cols_delete, bool_vars, cats, continuous_vars, discrete_string_vars, date_vars, dft
+
 
 # Removes duplicates from a list to return unique values - USED ONLYONCE
 def find_remove_duplicates(values):
     output = []
     seen = set()
     for value in values:
         if value not in seen:
             output.append(value)
             seen.add(value)
     return output
-#################################################################################
-def load_file_dataframe(dataname, sep=",", header=0, verbose=0, nrows=None,parse_dates=False):
 
-    start_time = time.time()
+
+#################################################################################
+def load_file_dataframe(dataname, sep=",", header=0, nrows=None, parse_dates=False):
     ###########################  This is where we load file or data frame ###############
-    if isinstance(dataname,str):
+    if isinstance(dataname, str):
         #### this means they have given file name as a string to load the file #####
         codex_flag = False
         codex = ['ascii', 'utf-8', 'iso-8859-1', 'cp1252', 'latin1']
-        
-        if dataname != '' and dataname.endswith(('csv')):
+
+        if dataname != '' and dataname.endswith('csv'):
             try:
                 dfte = pd.read_csv(dataname, sep=sep, header=header, encoding=None,
-                                parse_dates=parse_dates)
-                if not nrows is None:
+                                   parse_dates=parse_dates)
+                if nrows is not None:
                     if nrows < dfte.shape[0]:
-                        print('    max_rows_analyzed is smaller than dataset shape %d...' %dfte.shape[0])
+                        print('    max_rows_analyzed is smaller than dataset shape %d...' % dfte.shape[0])
                         dfte = dfte.sample(nrows, replace=False, random_state=99)
-                        print('        randomly sampled %d rows from read CSV file' %nrows)
-                print('Shape of your Data Set loaded: %s' %(dfte.shape,))
+                        print('        randomly sampled %d rows from read CSV file' % nrows)
+                print('Shape of your Data Set loaded: %s' % (dfte.shape,))
                 if len(np.array(list(dfte))[dfte.columns.duplicated()]) > 0:
                     print('You have duplicate column names in your data set. Removing duplicate columns now...')
                     dfte = dfte[list(dfte.columns[~dfte.columns.duplicated(keep='first')])]
                 return dfte
             except:
                 codex_flag = True
         if codex_flag:
             for code in codex:
                 try:
-                    dfte = pd.read_csv(dataname, sep=sep, header=header, encoding=code, nrows=nrows,
-                                    skiprows=skip_function, parse_dates=parse_dates)
+                    pass
                 except:
-                    print('    pandas %s encoder does not work for this file. Continuing...' %code)
+                    print('    pandas %s encoder does not work for this file. Continuing...' % code)
                     continue
-        elif dataname.endswith(('xlsx','xls','txt')):
+        elif dataname.endswith(('xlsx', 'xls', 'txt')):
             #### It's very important to get header rows in Excel since people put headers anywhere in Excel#
             if nrows is None:
-                dfte = pd.read_excel(dataname,header=header, parse_dates=parse_dates)
+                dfte = pd.read_excel(dataname, header=header, parse_dates=parse_dates)
             else:
-                dfte = pd.read_excel(dataname,header=header, nrows=nrows, parse_dates=parse_dates)
-            print('Shape of your Data Set loaded: %s' %(dfte.shape,))
+                dfte = pd.read_excel(dataname, header=header, nrows=nrows, parse_dates=parse_dates)
+            print('Shape of your Data Set loaded: %s' % (dfte.shape,))
             return dfte
         else:
             print('    Filename is an empty string or file not able to be loaded')
             return None
-    elif isinstance(dataname,pd.DataFrame):
+    elif isinstance(dataname, pd.DataFrame):
         #### this means they have given a dataframe name to use directly in processing #####
         if nrows is None:
             dfte = copy.deepcopy(dataname)
         else:
             if nrows < dataname.shape[0]:
-                print('    Since nrows is smaller than dataset, loading random sample of %d rows into pandas...' %nrows)
+                print(
+                    '    Since nrows is smaller than dataset, loading random sample of %d rows into pandas...' % nrows)
                 dfte = dataname.sample(n=nrows, replace=False, random_state=99)
             else:
                 dfte = copy.deepcopy(dataname)
-        print('Shape of your Data Set loaded: %s' %(dfte.shape,))
+        print('Shape of your Data Set loaded: %s' % (dfte.shape,))
         if len(np.array(list(dfte))[dfte.columns.duplicated()]) > 0:
             print('You have duplicate column names in your data set. Removing duplicate columns now...')
             dfte = dfte[list(dfte.columns[~dfte.columns.duplicated(keep='first')])]
         return dfte
     else:
         print('Dataname input must be a filename with path to that file or a Dataframe')
         return None
+
+
 ##########################################################################################
-import copy
-import pdb
-def classify_print_vars(filename,sep, max_rows_analyzed, max_cols_analyzed,
-                        depVar='',dfte=None, header=0,verbose=0):
+def classify_print_vars(filename: str or pd.DataFrame, sep, max_rows_analyzed, max_cols_analyzed,
+                        depVar='', header=0, verbose=0):
     corr_limit = 0.7  ### This limit represents correlation above this, vars will be removed
-    
-    start_time=time.time()
-    
-    if filename:
+
+    if isinstance(filename, str):
         dataname = copy.deepcopy(filename)
         parse_dates = True
-    else:
-        dataname = copy.deepcopy(dfte)
+    elif isinstance(filename, pd.DataFrame):
+        dataname = copy.deepcopy(filename)
         parse_dates = False
-    
-    dfte = load_file_dataframe(dataname, sep=sep, header=header, verbose=verbose, 
-                    nrows=max_rows_analyzed, parse_dates=parse_dates)
-    
+
+    dfte = load_file_dataframe(dataname, sep=sep, header=header, nrows=max_rows_analyzed, parse_dates=parse_dates)
+
     orig_preds = [x for x in list(dfte) if x not in [depVar]]
     #################    CLASSIFY  COLUMNS   HERE    ######################
     if len(dfte) >= 100000:
         dfte_small = dfte.sample(n=10000, random_state=99)
     else:
         dfte_small = copy.deepcopy(dfte)
     var_df = classify_columns(dfte_small[orig_preds], verbose)
     #####       Classify Columns   ################
-    IDcols = var_df['id_vars']
-    discrete_string_vars = var_df['nlp_vars']+var_df['discrete_string_vars']
+    id_cols = var_df['id_vars']
+    discrete_string_vars = var_df['nlp_vars'] + var_df['discrete_string_vars']
     cols_delete = var_df['cols_delete']
     bool_vars = var_df['string_bool_vars'] + var_df['num_bool_vars']
     int_vars = var_df['int_vars']
     categorical_vars = var_df['cat_vars'] + var_df['factor_vars'] + int_vars + bool_vars
     date_vars = var_df['date_vars']
-    
-    
-    if len(var_df['continuous_vars'])==0 and len(int_vars)>0:
+
+    if len(var_df['continuous_vars']) == 0 and len(int_vars) > 0:
         continuous_vars = var_df['int_vars']
         categorical_vars = list_difference(categorical_vars, int_vars)
-        int_vars = []
-    #elif len(var_df['continuous_vars'])==0 and len(int_vars)==0:
+    # elif len(var_df['continuous_vars'])==0 and len(int_vars)==0:
     #    print('Cannot visualize this dataset since no numeric or integer vars in data...returning')
     #    return dataname
     else:
         continuous_vars = var_df['continuous_vars']
     #### from now you can use wordclouds on discrete_string_vars ######################
-    preds = [x for x in orig_preds if x not in IDcols+cols_delete]
-    if len(IDcols+cols_delete) == 0:
+    preds = [x for x in orig_preds if x not in id_cols + cols_delete]
+    if len(id_cols + cols_delete) == 0:
         print('        No variables removed since no ID or low-information variables found in data set')
     else:
         print('        %d variable(s) removed since they were ID or low-information variables'
-                                %len(IDcols+cols_delete))
+              % len(id_cols + cols_delete))
         if verbose >= 1:
-            print('        List of variables removed: %s' %(IDcols+cols_delete))
+            print('        List of variables removed: %s' % (id_cols + cols_delete))
     #############    Sample data if too big and find problem type   #############################
-    if dfte.shape[0]>= max_rows_analyzed:
-        print('Since Number of Rows in data %d exceeds maximum, randomly sampling %d rows for EDA...' %(len(dfte),max_rows_analyzed))
+    if dfte.shape[0] >= max_rows_analyzed:
+        print('Since Number of Rows in data %d exceeds maximum, randomly sampling %d rows for EDA...' % (
+            len(dfte), max_rows_analyzed))
         dft = dfte.sample(max_rows_analyzed, random_state=0)
     else:
         dft = copy.deepcopy(dfte)
     ###### This is where you find what type the dependent variable is ########
     if isinstance(depVar, list):
         # If depVar is a list, just select the first one in the list to visualize!
         depVar = depVar[0]
-        print('Since AutoViz cannot visualize multi-label targets, selecting %s from target list' %depVar[0])
-    
+        print('Since AutoViz cannot visualize multi-label targets, selecting %s from target list' % depVar[0])
+
     ### Now we analyze depVar as usual - Do not change the next line to elif! ###
     if type(depVar) == str:
         if depVar == '':
             cols_list = list(dft)
             problem_type = 'Clustering'
             classes = []
         else:
             try:
-                problem_type = analyze_problem_type(dft, depVar,verbose)
+                problem_type = analyze_problem_type(dft, depVar, verbose)
             except:
                 print('Could not find given target var in data set. Please check input')
                 ### return the data frame as is ############
-                return dfte,depVar,IDcols,bool_vars,categorical_vars,continuous_vars,discrete_string_vars,date_vars,classes,problem_type, cols_list
-            cols_list = list_difference(list(dft),depVar)
+                return (dfte, depVar, id_cols, bool_vars, categorical_vars, continuous_vars, discrete_string_vars,
+                        date_vars)
+            cols_list = list_difference(list(dft), depVar)
             if dft[depVar].dtype == object:
                 classes = dft[depVar].unique().tolist()
-                #### You dont have to convert it since most charts can take string vars as target ####
-                #dft[depVar] = dft[depVar].factorize()[0]
+                #### You don't have to convert it since most charts can take string vars as target ####
+                # dft[depVar] = dft[depVar].factorize()[0]
             elif str(dft[depVar].dtype) in ['category']:
-                #### You dont have to convert it since most charts can take string vars as target ####
+                #### You don't have to convert it since most charts can take string vars as target ####
                 classes = dft[depVar].unique().tolist()
             elif dft[depVar].dtype in [np.int64, np.int32, np.int16, np.int8]:
                 classes = dft[depVar].unique().tolist()
             elif dft[depVar].dtype == bool:
                 dft[depVar] = dft[depVar].astype(int)
-                classes =  dft[depVar].unique().astype(int).tolist()
+                classes = dft[depVar].unique().astype(int).tolist()
             elif dft[depVar].dtype == float and problem_type.endswith('Classification'):
                 classes = dft[depVar].factorize()[1].tolist()
             else:
                 classes = dft[depVar].factorize()[1].tolist()
-    elif depVar == None:
-            cols_list = list(dft)
-            problem_type = 'Clustering'
-            classes = []
+    elif depVar is None:
+        cols_list = list(dft)
+        problem_type = 'Clustering'
+        classes = []
     else:
         print('Cannot find target variable to visualize. Returning...')
         return dft
     #############  Check if there are too many columns to visualize  ################
     if len(preds) >= max_cols_analyzed:
         #########     In that case, SELECT IMPORTANT FEATURES HERE   ######################
         if problem_type.endswith('Classification') or problem_type == 'Regression':
-            print('Number of variables = %d exceeds limit, finding top %d variables through XGBoost' %(len(
-                                            preds), max_cols_analyzed))
-            important_features,num_vars, _ = find_top_features_xgb(dft,preds,continuous_vars,
-                                                         depVar,problem_type,corr_limit,verbose)
+            print('Number of variables = %d exceeds limit, finding top %d variables through XGBoost' % (len(
+                preds), max_cols_analyzed))
+            important_features, num_vars, _ = find_top_features_xgb(dft, preds, continuous_vars,
+                                                                    depVar, problem_type, corr_limit, verbose)
             if len(important_features) >= max_cols_analyzed:
-                print('    Since number of features selected is greater than max columns analyzed, limiting to %d variables' %max_cols_analyzed)
+                print(
+                    '    Since number of features selected is greater than max columns analyzed, limiting to %d variables' % max_cols_analyzed)
                 important_features = important_features[:max_cols_analyzed]
-            dft = dft[important_features+[depVar]]
+            dft = dft[important_features + [depVar]]
             #### Time to  classify the important columns again. Set verbose to zero so you don't print it again ###
             var_df = classify_columns(dft[important_features], verbose=0)
-            IDcols = var_df['id_vars']
-            discrete_string_vars = var_df['nlp_vars']+var_df['discrete_string_vars']
+            id_cols = var_df['id_vars']
+            discrete_string_vars = var_df['nlp_vars'] + var_df['discrete_string_vars']
             cols_delete = var_df['cols_delete']
             bool_vars = var_df['string_bool_vars'] + var_df['num_bool_vars']
             int_vars = var_df['int_vars']
             categorical_vars = var_df['cat_vars'] + var_df['factor_vars'] + int_vars + bool_vars
-            if len(var_df['continuous_vars'])==0 and len(int_vars)>0:
+            if len(var_df['continuous_vars']) == 0 and len(int_vars) > 0:
                 continuous_vars = var_df['int_vars']
                 categorical_vars = list_difference(categorical_vars, int_vars)
-                int_vars = []
             else:
                 continuous_vars = var_df['continuous_vars']
             date_vars = var_df['date_vars']
-            preds = [x for x in important_features if x not in IDcols+cols_delete+discrete_string_vars]
-            if len(IDcols+cols_delete+discrete_string_vars) == 0:
+            preds = [x for x in important_features if x not in id_cols + cols_delete + discrete_string_vars]
+            if len(id_cols + cols_delete + discrete_string_vars) == 0:
                 print('    No variables removed since no ID or low-information variables found in data')
             else:
                 print('    %d variable(s) removed since they were ID or low-information variables'
-                                        %len(IDcols+cols_delete+discrete_string_vars))
+                      % len(id_cols + cols_delete + discrete_string_vars))
             if verbose >= 1:
-                print('    List of variables removed: %s' %(IDcols+cols_delete+discrete_string_vars))
-            dft = dft[preds+[depVar]]
+                print('    List of variables removed: %s' % (id_cols + cols_delete + discrete_string_vars))
+            dft = dft[preds + [depVar]]
         else:
             continuous_vars = continuous_vars[:max_cols_analyzed]
-            print('%d numeric variables in data exceeds limit, taking top %d variables' %(len(
-                                            continuous_vars), max_cols_analyzed))
+            print('%d numeric variables in data exceeds limit, taking top %d variables' % (len(
+                continuous_vars), max_cols_analyzed))
             if verbose >= 1:
-                print('    List of variables selected: %s' %(continuous_vars[:max_cols_analyzed]))
-    #elif len(continuous_vars) < 1:
+                print('    List of variables selected: %s' % (continuous_vars[:max_cols_analyzed]))
+    # elif len(continuous_vars) < 1:
     #    print('No continuous variables in this data set. No visualization can be performed')
     #    ### Return data frame as is #####
     #    return dfte
     else:
         #########     If above 1 but below limit, leave features as it is   ######################
         if not isinstance(depVar, list):
             if depVar != '':
-                dft = dft[preds+[depVar]]
+                dft = dft[preds + [depVar]]
         else:
-            dft = dft[preds+depVar]
+            dft = dft[preds + depVar]
     ###################   Time to reduce cat vars which have more than 30 categories #############
-    #discrete_string_vars += np.array(categorical_vars)[dft[categorical_vars].nunique()>30].tolist()
-    #categorical_vars = left_subtract(categorical_vars,np.array(
+    # discrete_string_vars += np.array(categorical_vars)[dft[categorical_vars].nunique()>30].tolist()
+    # categorical_vars = left_subtract(categorical_vars,np.array(
     #    categorical_vars)[dft[categorical_vars].nunique()>30].tolist())
     #############   Next you can print them if verbose is set to print #########
-    
+
     ppt = pprint.PrettyPrinter(indent=4)
-    if verbose>=2 and len(cols_list) <= max_cols_analyzed:
-        #marthas_columns(dft,verbose)
+    if verbose >= 2 and len(cols_list) <= max_cols_analyzed:
+        # marthas_columns(dft,verbose)
         print("   Columns to delete:")
-        ppt.pprint('   %s' %cols_delete)
+        ppt.pprint('   %s' % cols_delete)
         print("   Boolean variables %s ")
-        ppt.pprint('   %s' %bool_vars)
+        ppt.pprint('   %s' % bool_vars)
         print("   Categorical variables %s ")
-        ppt.pprint('   %s' %categorical_vars)
-        print("   Continuous variables %s " )
-        ppt.pprint('   %s' %continuous_vars)
-        print("   Discrete string variables %s " )
-        ppt.pprint('   %s' %discrete_string_vars)
-        print("   Date and time variables %s " )
-        ppt.pprint('   %s' %date_vars)
+        ppt.pprint('   %s' % categorical_vars)
+        print("   Continuous variables %s ")
+        ppt.pprint('   %s' % continuous_vars)
+        print("   Discrete string variables %s ")
+        ppt.pprint('   %s' % discrete_string_vars)
+        print("   Date and time variables %s ")
+        ppt.pprint('   %s' % date_vars)
         print("   ID variables %s ")
-        ppt.pprint('   %s' %IDcols)
+        ppt.pprint('   %s' % id_cols)
         print("   Target variable %s ")
-        ppt.pprint('   %s' %depVar)
-    elif verbose==1 and len(cols_list) > 30:
+        ppt.pprint('   %s' % depVar)
+    elif verbose == 1 and len(cols_list) > 30:
         print('   Total columns > 30, too numerous to print.')
-    return dft,depVar,IDcols,bool_vars,categorical_vars,continuous_vars,discrete_string_vars,date_vars,classes,problem_type, cols_list
+    return dft, depVar, id_cols, bool_vars, categorical_vars, continuous_vars, discrete_string_vars, date_vars, classes, problem_type, cols_list
+
+
 ####################################################################
-def marthas_columns(data,verbose=0):
+def marthas_columns(data, verbose=0):
     """
     This program is named  in honor of my one of students who came up with the idea for it.
     It's a neat way of printing data types and information compared to the boring describe() function in Pandas.
     """
     data = data[:]
     print('Data Set Shape: %d rows, %d cols' % data.shape)
     if data.shape[1] > 30:
         print('Too many columns to print')
     else:
-        if verbose>=3:
+        if verbose >= 3:
             print('Data Set columns info:')
             for col in data.columns:
                 print('* %s: %d nulls, %d unique vals, most common: %s' % (
-                        col,
-                        data[col].isnull().sum(),
-                        data[col].nunique(),
-                        data[col].value_counts().head(2).to_dict()
-                    ))
+                    col,
+                    data[col].isnull().sum(),
+                    data[col].nunique(),
+                    data[col].value_counts().head(2).to_dict()
+                ))
             print('--------------------------------------------------------------------')
 
+
 #################################################################################
-import copy
 def EDA_find_remove_columns_with_infinity(df, remove=False):
     """
     This function finds all columns in a dataframe that have inifinite values (np.inf or -np.inf)
     It returns a list of column names. If the list is empty, it means no columns were found.
     If remove flag is set, then it returns a smaller dataframe with inf columns removed.
     """
     nums = df.select_dtypes(include='number').columns.tolist()
     dfx = df[nums]
     sum_rows = np.isinf(dfx).values.sum()
-    add_cols =  list(dfx.columns.to_series()[np.isinf(dfx).any()])
+    add_cols = list(dfx.columns.to_series()[np.isinf(dfx).any()])
     if sum_rows > 0:
-        print('    there are %d rows and %d columns with infinity in them...' %(sum_rows,len(add_cols)))
+        print('    there are %d rows and %d columns with infinity in them...' % (sum_rows, len(add_cols)))
         if remove:
             ### here you need to use df since the whole dataset is involved ###
             nocols = [x for x in df.columns if x not in add_cols]
-            print("    Shape of dataset before %s and after %s removing columns with infinity" %(df.shape,(df[nocols].shape,)))
+            print("    Shape of dataset before %s and after %s removing columns with infinity" % (
+                df.shape, (df[nocols].shape,)))
             return df[nocols]
         else:
             ## this will be a list of columns with infinity ####
             return add_cols
     else:
         ## this will be an empty list if there are no columns with infinity
         return add_cols
+
+
 #######################################################################################
-from collections import Counter
-import time
-from sklearn.feature_selection import chi2, mutual_info_regression, mutual_info_classif
+from sklearn.feature_selection import mutual_info_regression, mutual_info_classif
 from sklearn.feature_selection import SelectKBest
 ################################################################################
 from collections import defaultdict
-from collections import OrderedDict
-import time
+
+
 def return_dictionary_list(lst_of_tuples):
     """ Returns a dictionary of lists if you send in a list of Tuples"""
     orDict = defaultdict(list)
     # iterating over list of tuples
     for key, val in lst_of_tuples:
         orDict[key].append(val)
     return orDict
+
+
 ##################################################################################
 def remove_variables_using_fast_correlation(df, numvars, modeltype, target,
-                                corr_limit = 0.70,verbose=0):
+                                            corr_limit=0.70, verbose=0):
     """
     #### THIS METHOD IS KNOWN AS SULO METHOD in HONOR OF my mother SULOCHANA SESHADRI #######
     This highly efficient method removes variables that are highly correlated using a series of
     pair-wise correlation knockout rounds. It is extremely fast and hence can work on thousands
     of variables in less than a minute, even on a laptop. You need to send in a list of numeric
     variables and that's all! The method defines high Correlation as anything over 0.70 (absolute)
     but this can be changed. If two variables have absolute correlation higher than this, they
     will be marked, and using a process of elimination, one of them will get knocked out:
-    To decide order of variables to keep, we use mutuail information score to select. MIS returns
-    a ranked list of these correlated variables: when we select one, we knock out others
-    that it is correlated to. Then we select next var. This way we knock out correlated variables.
-    Finally we are left with uncorrelated variables that are also highly important (mutual score).
+    To decide order of variables to keep, we use mutual information score to select. MIS returns
+    a ranked list of these correlated variables: when we select one, we knock out other variables
+    it is correlated to. Then we select next var. This way we remove correlated variables.
+    Finally, we are left with uncorrelated variables that are also highly important (mutual score).
     ##############  YOU MUST INCLUDE THE ABOVE MESSAGE IF YOU COPY THIS CODE IN YOUR LIBRARY #####
     """
-    print('    Removing correlated variables from %d numerics using SULO method' %len(numvars))
+    print('    Removing correlated variables from %d numerics using SULO method' % len(numvars))
     correlation_dataframe = df[numvars].corr()
     a = correlation_dataframe.values
     col_index = correlation_dataframe.columns.tolist()
-    index_triupper = list(zip(np.triu_indices_from(a,k=1)[0],np.triu_indices_from(a,k=1)[1]))
-    high_corr_index_list = [x for x in np.argwhere(abs(a[np.triu_indices(len(a), k = 1)])>=corr_limit)]
-    low_corr_index_list =  [x for x in np.argwhere(abs(a[np.triu_indices(len(a), k = 1)])<corr_limit)]
+    index_triupper = list(zip(np.triu_indices_from(a, k=1)[0], np.triu_indices_from(a, k=1)[1]))
+    high_corr_index_list = [x for x in np.argwhere(abs(a[np.triu_indices(len(a), k=1)]) >= corr_limit)]
     tuple_list = [y for y in [index_triupper[x[0]] for x in high_corr_index_list]]
-    correlated_pair = [(col_index[tuple[0]],col_index[tuple[1]]) for tuple in tuple_list]
+    correlated_pair = [(col_index[local_tuple[0]], col_index[local_tuple[1]]) for local_tuple in tuple_list]
     corr_pair_dict = dict(return_dictionary_list(correlated_pair))
     keys_in_dict = list(corr_pair_dict.keys())
-    reverse_correlated_pair = [(y,x) for (x,y) in correlated_pair]
+    reverse_correlated_pair = [(y, x) for (x, y) in correlated_pair]
     reverse_corr_pair_dict = dict(return_dictionary_list(reverse_correlated_pair))
     for key, val in reverse_corr_pair_dict.items():
         if key in keys_in_dict:
             if len(key) > 1:
                 corr_pair_dict[key] += val
         else:
             corr_pair_dict[key] = val
     flat_corr_pair_list = [item for sublist in correlated_pair for item in sublist]
     #### You can make it a dictionary or a tuple of lists. We have chosen the latter here to keep order intact.
     corr_pair_count_dict = count_freq_in_list(flat_corr_pair_list)
-    corr_list = [k for (k,v) in corr_pair_count_dict]
-    ###### This is for ordering the variables in the highest to lowest importance to target ###
+    corr_list = [k for (k, v) in corr_pair_count_dict]
+    ###### This is for ordering the variables from highest to lowest importance by target ###
     if len(corr_list) == 0:
-        final_list = list(correlation_dataframe)
-        print('Selecting all (%d) variables since none of them are highly correlated...' %len(numvars))
+        print('Selecting all (%d) variables since none of them are highly correlated...' % len(numvars))
         return numvars
     else:
         max_feats = len(corr_list)
         if modeltype == 'Regression':
             sel_function = mutual_info_regression
             fs = SelectKBest(score_func=sel_function, k=max_feats)
             fs.fit(df[corr_list], df[target])
-            mutual_info = dict(zip(corr_list,fs.scores_))
+            mutual_info = dict(zip(corr_list, fs.scores_))
         else:
             sel_function = mutual_info_classif
             fs = SelectKBest(score_func=sel_function, k=max_feats)
             fs.fit(df[corr_list], df[target])
-            mutual_info = dict(zip(corr_list,fs.scores_))
+            mutual_info = dict(zip(corr_list, fs.scores_))
         #### The first variable in list has the highest correlation to the target variable ###
-        sorted_by_mutual_info =[key for (key,val) in sorted(mutual_info.items(), key=lambda kv: kv[1],reverse=True)]
+        sorted_by_mutual_info = [key for (key, val) in sorted(mutual_info.items(), key=lambda kv: kv[1], reverse=True)]
         #####   Now we select the final list of correlated variables ###########
         selected_corr_list = []
         #### select each variable by the highest mutual info and see what vars are correlated to it
         for each_corr_name in sorted_by_mutual_info:
             ### add the selected var to the selected_corr_list
             selected_corr_list.append(each_corr_name)
             for each_remove in corr_pair_dict[each_corr_name]:
                 #### Now remove each variable that is highly correlated to the selected variable
                 if each_remove in sorted_by_mutual_info:
                     sorted_by_mutual_info.remove(each_remove)
         ##### Now we combine the uncorrelated list to the selected correlated list above
-        rem_col_list = left_subtract(list(correlation_dataframe),corr_list)
+        rem_col_list = left_subtract(list(correlation_dataframe), corr_list)
         final_list = rem_col_list + selected_corr_list
         if verbose >= 1:
-            print('\nAfter removing highly correlated variables, following %d numeric vars selected: %s' %(len(final_list),final_list))
+            print('\nAfter removing highly correlated variables, following %d numeric vars selected: %s' % (
+                len(final_list), final_list))
         return final_list
+
+
 ###############################################################################################
 def count_freq_in_list(lst):
     """
     This counts the frequency of items in a list but MAINTAINS the order of appearance of items.
-    This order is very important when you are doing certain functions. Hence this function!
+    This order is very important when you are doing certain functions. Hence, this function!
     """
-    temp=np.unique(lst)
+    temp = np.unique(lst)
     result = []
     for i in temp:
-        result.append((i,lst.count(i)))
+        result.append((i, lst.count(i)))
     return result
 
-def find_corr_vars(correlation_dataframe,corr_limit = 0.70):
+
+def find_corr_vars(correlation_dataframe, corr_limit=0.70):
     """
     This returns a dictionary of counts of each variable and how many vars it is correlated to in the dataframe
     """
     flatten = lambda l: [item for sublist in l for item in sublist]
     flatten_items = lambda dic: [x for x in dic.items()]
     a = correlation_dataframe.values
     col_index = correlation_dataframe.columns.tolist()
-    index_triupper = list(zip(np.triu_indices_from(a,k=1)[0],np.triu_indices_from(a,k=1)[1]))
-    high_corr_index_list = [x for x in np.argwhere(abs(a[np.triu_indices(len(a), k = 1)])>=corr_limit)]
-    low_corr_index_list =  [x for x in np.argwhere(abs(a[np.triu_indices(len(a), k = 1)])<corr_limit)]
+    index_triupper = list(zip(np.triu_indices_from(a, k=1)[0], np.triu_indices_from(a, k=1)[1]))
+    high_corr_index_list = [x for x in np.argwhere(abs(a[np.triu_indices(len(a), k=1)]) >= corr_limit)]
     tuple_list = [y for y in [index_triupper[x[0]] for x in high_corr_index_list]]
-    correlated_pair = [(col_index[tuple[0]],col_index[tuple[1]]) for tuple in tuple_list]
+    correlated_pair = [(col_index[tup[0]], col_index[tup[1]]) for tup in tuple_list]
     correlated_pair_dict = dict(correlated_pair)
     flat_corr_pair_list = [item for sublist in correlated_pair for item in sublist]
     #### You can make it a dictionary or a tuple of lists. We have chosen the latter here to keep order intact.
-    #corr_pair_count_dict = Counter(flat_corr_pair_list)
+    # corr_pair_count_dict = Counter(flat_corr_pair_list)
     corr_pair_count_dict = count_freq_in_list(flat_corr_pair_list)
     corr_list = list(set(flatten(flatten_items(correlated_pair_dict))))
-    rem_col_list = left_subtract(list(correlation_dataframe),list(OrderedDict.fromkeys(flat_corr_pair_list)))
+    rem_col_list = left_subtract(list(correlation_dataframe), list(OrderedDict.fromkeys(flat_corr_pair_list)))
     return corr_pair_count_dict, rem_col_list, corr_list, correlated_pair_dict
+
+
 #################################################################################
-def left_subtract(l1,l2):
+def left_subtract(l1, l2):
     lst = []
     for i in l1:
         if i not in l2:
             lst.append(i)
     return lst
+
+
 #######
 def convert_train_test_cat_col_to_numeric(start_train, start_test, col):
     """
     ####  This is the easiest way to label encode object variables in both train and test
     #### This takes care of some categories that are present in train and not in test
     ###     and vice versa
     """
     start_train = copy.deepcopy(start_train)
     start_test = copy.deepcopy(start_test)
     if start_train[col].isnull().sum() > 0:
         ### Remember that fillna only works at dataframe level! ###
         start_train[[col]] = start_train[[col]].fillna("NA")
     train_categs = list(pd.unique(start_train[col].values))
-    if not isinstance(start_test,str) :
+    if not isinstance(start_test, str):
         test_categs = list(pd.unique(start_test[col].values))
-        categs_all = train_categs+test_categs
-        dict_all =  return_factorized_dict(categs_all)
+        categs_all = train_categs + test_categs
+        dict_all = return_factorized_dict(categs_all)
     else:
         dict_all = return_factorized_dict(train_categs)
     start_train[col] = start_train[col].map(dict_all)
-    if not isinstance(start_test,str) :
+    if not isinstance(start_test, str):
         if start_test[col].isnull().sum() > 0:
             start_test[[col]] = start_test[[col]].fillna("NA")
         start_test[col] = start_test[col].map(dict_all)
     return start_train, start_test
+
+
 ###############################################################################
 def return_factorized_dict(ls):
     """
     ######  Factorize any list of values in a data frame using this neat function
     if your data has any NaN's it automatically marks it as -1 and returns that for NaN's
     Returns a dictionary mapping previous values with new values.
     """
     factos = pd.unique(pd.factorize(ls)[0])
     categs = pd.unique(pd.factorize(ls)[1])
     if -1 in factos:
-        categs = np.insert(categs,np.where(factos==-1)[0][0],np.nan)
-    return dict(zip(categs,factos))
+        categs = np.insert(categs, np.where(factos == -1)[0][0], np.nan)
+    return dict(zip(categs, factos))
+
+
 #################################################################################
 ################      Find top features using XGB     ###################
 #################################################################################
-from sklearn.model_selection import KFold
-from sklearn.model_selection import GridSearchCV
-from sklearn.multioutput import MultiOutputClassifier
-import copy
-from sklearn.multiclass import OneVsRestClassifier
 from collections import OrderedDict
 ################################################################################
 ###########################################################################################
 ############## CONVERSION OF STRING COLUMNS TO NUMERIC WITHOUT LABEL ENCODER #########
 #######################################################################################
 import copy
-def convert_a_column_to_numeric(x, col_dict=""):
-    '''Function converts any pandas series (or column) consisting of string chars,
+
+
+def convert_a_column_to_numeric(x, col_dict):
+    """Function converts any pandas series (or column) consisting of string chars,
        into numeric values. It converts an all-string column to an all-number column.
        This is an amazing function which performs exactly like a Label Encoding
-       except that it is simpler and faster'''
+       except that it is simpler and faster"""
     if isinstance(col_dict, str):
         values = np.unique(x)
-        values2nums = dict(zip(values,range(len(values))))
-        convert_dict = dict(zip(range(len(values)),values))
+        values2nums = dict(zip(values, range(len(values))))
+        convert_dict = dict(zip(range(len(values)), values))
         return x.replace(values2nums), convert_dict
-    else:
+    elif isinstance(col_dict, dict):
         convert_dict = copy.deepcopy(col_dict)
-        keys  = col_dict.keys()
+        keys = col_dict.keys()
         newkeys = np.unique(x)
         rem_keys = left_subtract(newkeys, keys)
         max_val = max(col_dict.values()) + 1
         for eachkey in rem_keys:
-            convert_dict.update({eachkey:max_val})
+            convert_dict.update({eachkey: max_val})
             max_val += 1
         return x.replace(convert_dict)
+
+
 #######################################################################################
 def convert_a_mixed_object_column_to_numeric(x, col_dict=''):
     """
     This is the main utility that converts any string column to numeric.
-    It does not need Label Encoder since it picks up an string that may not be in test data.
+    It does not need Label Encoder since it picks up a string that may not be in test data.
     """
     x = x.astype(str)
     if isinstance(col_dict, str):
-        x, convert_dict = convert_a_column_to_numeric(x)
-        convert_dict = dict([(v,k) for (k,v) in convert_dict.items()])
+        x, convert_dict = convert_a_column_to_numeric(x, col_dict)
+        convert_dict = dict([(v, k) for (k, v) in convert_dict.items()])
         return x, convert_dict
     else:
         x = convert_a_column_to_numeric(x, col_dict)
     return x
+
+
 ######################################################################################
 def convert_all_object_columns_to_numeric(train, test):
     """
     #######################################################################################
     This is a utility that converts string columns to numeric WITHOUT LABEL ENCODER.
     The beauty of this utility is that it does not blow up when it finds strings in test not in train.
     #######################################################################################
     """
     train = copy.deepcopy(train)
-    if train.dtypes.any()==object:
-        lis=[]
-        for row,column in train.dtypes.iteritems():
+    if train.dtypes.any() == object:
+        lis = []
+        for row, column in train.dtypes.iteritems():
             if column == object:
                 lis.append(row)
-        #print('%d string variables identified' %len(lis))
+        # print('%d string variables identified' %len(lis))
         for everycol in lis:
-            #print('    Converting %s to numeric' %everycol)
+            # print('    Converting %s to numeric' %everycol)
             try:
                 train[everycol], train_dict = convert_a_mixed_object_column_to_numeric(train[everycol])
                 if not isinstance(test, str):
                     test[everycol] = convert_a_mixed_object_column_to_numeric(test[everycol], train_dict)
             except:
-                #print('Error converting %s column from string to numeric. Continuing...' %everycol)
+                # print('Error converting %s column from string to numeric. Continuing...' %everycol)
                 continue
     return train, test
+
+
 ###################################################################################
 ################      Find top features using XGB     ###################
 ################################################################################
 from xgboost import XGBClassifier, XGBRegressor
-def find_top_features_xgb(train,preds,numvars,target,modeltype,corr_limit=0.7,verbose=0):
+
+
+def find_top_features_xgb(train, preds, numvars, target, modeltype, corr_limit=0.7, verbose=0):
     """
-    This is a fast utility that uses XGB to find top features. You
+    This is a fast utility that uses XGB to find top features.
     It returns a list of important features.
-    Since it is XGB, you dont have to restrict the input to just numeric vars.
+    Since it is XGB, you don't have to restrict the input to just numeric vars.
     You can send in all kinds of vars and it will take care of transforming it. Sweet!
     """
     train = copy.deepcopy(train)
     preds = copy.deepcopy(preds)
     numvars = copy.deepcopy(numvars)
     ######################   I M P O R T A N T ##############################################
     ###### This top_num decides how many top_n features XGB selects in each iteration.
-    ####  There a total of 5 iterations. Hence 5x10 means maximum 50 features will be selected.
+    ####  There a total of 5 iterations. Hence, 5x10 means maximum 50 features will be selected.
     #####  If there are more than 50 variables, then maximum 25% of its variables will be selected
     if len(preds) <= 50:
         top_num = 10
     else:
         ### the maximum number of variables will 25% of preds which means we divide by 5 and get 5% here
-        ### The five iterations result in 5% being chosen in each iteration. Hence max 25% of variables!
-        top_num = int(len(preds)*0.05)
+        ### The five iterations result in 5% being chosen in each iteration. Hence, max 25% of variables!
+        top_num = int(len(preds) * 0.05)
     ######################   I M P O R T A N T ##############################################
     #### If there are more than 30 categorical variables in a data set, it is worth reducing features.
     ####  Otherwise. XGBoost is pretty good at finding the best features whether cat or numeric !
     n_splits = 5
     max_depth = 8
-    max_cats = 5
     ######################   I M P O R T A N T ##############################################
-    subsample =  0.7
+    subsample = 0.7
     col_sub_sample = 0.7
     train = copy.deepcopy(train)
-    start_time = time.time()
     test_size = 0.2
     seed = 1
     early_stopping = 5
     ####### All the default parameters are set up now #########
-    kf = KFold(n_splits=n_splits)
-    rem_vars = left_subtract(preds,numvars)
+    rem_vars = left_subtract(preds, numvars)
     catvars = copy.deepcopy(rem_vars)
     ############   I  M P O R T A N T ! I M P O R T A N T ! ######################
     ##### Removing the Cat Vars selection using Linear Methods since they fail so often.
     ##### Linear methods such as Chi2 or Mutual Information Score are not great
     ####  for feature selection since they can't handle large data and provide
-    ####  misleading results for large data sets. Hence I am using XGBoost alone.
+    ####  misleading results for large data sets. Hence, I am using XGBoost alone.
     ####  Also, another method of using Spearman Correlation for CatVars with 100's
     ####  of variables is very slow. Also, is not very clear is effective: only 3-4 vars
     ####   are removed. Hence for now, I am not going to use Spearman method. Perhaps later.
     ##############################################################################
-    #if len(catvars) > max_cats:
+    # if len(catvars) > max_cats:
     #    start_time = time.time()
     #    important_cats = remove_variables_using_fast_correlation(train,catvars,'spearman',
     #                         corr_limit,verbose)
     #    if verbose >= 1:
     #        print('Time taken for reducing highly correlated Categorical vars was %0.0f seconds' %(time.time()-start_time))
-    #else:
+    # else:
     important_cats = copy.deepcopy(catvars)
-    print('    No categorical feature reduction done. All %d Categorical vars selected ' %(len(catvars)))
+    print('    No categorical feature reduction done. All %d Categorical vars selected ' % (len(catvars)))
     ########    Drop Missing value rows since XGB for some reason  #########
     ########    can't handle missing values in early stopping rounds #######
-    train.dropna(axis=0,subset=preds+[target],inplace=True)
+    train.dropna(axis=0, subset=preds + [target], inplace=True)
     if len(numvars) > 1:
-        final_list = remove_variables_using_fast_correlation(train,numvars,modeltype,target,
-                             corr_limit,verbose)
+        final_list = remove_variables_using_fast_correlation(train, numvars, modeltype, target,
+                                                             corr_limit, verbose)
     else:
         final_list = copy.deepcopy(numvars)
-    print('    Adding %s categorical variables to reduced numeric variables  of %d' %(
-                            len(important_cats),len(final_list)))
-    if  isinstance(final_list,np.ndarray):
+    print('    Adding %s categorical variables to reduced numeric variables  of %d' % (
+        len(important_cats), len(final_list)))
+    if isinstance(final_list, np.ndarray):
         final_list = final_list.tolist()
-    preds = final_list+important_cats
+    preds = final_list + important_cats
     #######You must convert category variables into integers ###############
     if len(important_cats) > 0:
         train, _ = convert_all_object_columns_to_numeric(train, "")
     ########   Dont move this train and y definition anywhere else ########
     y = train[target]
     print('############## F E A T U R E   S E L E C T I O N  ####################')
     important_features = []
     if modeltype == 'Regression':
         objective = 'reg:squarederror'
-        model_xgb = XGBRegressor( n_estimators=100,subsample=subsample,objective=objective,
-                                colsample_bytree=col_sub_sample,reg_alpha=0.5, reg_lambda=0.5,
-                                 seed=1,n_jobs=-1,random_state=1)
+        model_xgb = XGBRegressor(n_estimators=100, subsample=subsample, objective=objective,
+                                 colsample_bytree=col_sub_sample, reg_alpha=0.5, reg_lambda=0.5,
+                                 seed=1, n_jobs=-1, random_state=1)
         eval_metric = 'rmse'
     else:
         #### This is for Classifiers only
         classes = np.unique(train[target].values)
         if len(classes) == 2:
             model_xgb = XGBClassifier(base_score=0.5, booster='gbtree', subsample=subsample,
-                colsample_bytree=col_sub_sample,gamma=1, learning_rate=0.1, max_delta_step=0,
-                max_depth=max_depth, min_child_weight=1, missing=-999, n_estimators=100,
-                n_jobs=-1, nthread=None, objective='binary:logistic',
-                random_state=1, reg_alpha=0.5, reg_lambda=0.5,
-                seed=1)
+                                      colsample_bytree=col_sub_sample, gamma=1, learning_rate=0.1, max_delta_step=0,
+                                      max_depth=max_depth, min_child_weight=1, missing=-999, n_estimators=100,
+                                      n_jobs=-1, nthread=None, objective='binary:logistic',
+                                      random_state=1, reg_alpha=0.5, reg_lambda=0.5,
+                                      seed=1)
             eval_metric = 'logloss'
         else:
             model_xgb = XGBClassifier(base_score=0.5, booster='gbtree', subsample=subsample,
-                        colsample_bytree=col_sub_sample, gamma=1, learning_rate=0.1, max_delta_step=0,
-                max_depth=max_depth, min_child_weight=1, missing=-999, n_estimators=100,
-                n_jobs=-1, nthread=None, objective='multi:softmax',
-                random_state=1, reg_alpha=0.5, reg_lambda=0.5,
-                seed=1)
+                                      colsample_bytree=col_sub_sample, gamma=1, learning_rate=0.1, max_delta_step=0,
+                                      max_depth=max_depth, min_child_weight=1, missing=-999, n_estimators=100,
+                                      n_jobs=-1, nthread=None, objective='multi:softmax',
+                                      random_state=1, reg_alpha=0.5, reg_lambda=0.5,
+                                      seed=1)
             eval_metric = 'mlogloss'
     ####   This is where you start to Iterate on Finding Important Features ################
     save_xgb = copy.deepcopy(model_xgb)
     train_p = train[preds]
     if train_p.shape[1] < 10:
         iter_limit = 2
     else:
-        iter_limit = int(train_p.shape[1]/5+0.5)
-    print('Current number of predictors = %d ' %(train_p.shape[1],))
+        iter_limit = int(train_p.shape[1] / 5 + 0.5)
+    print('Current number of predictors = %d ' % (train_p.shape[1],))
     print('    Finding Important Features using Boosted Trees algorithm...')
     try:
-        for i in range(0,train_p.shape[1],iter_limit):
+        for i in range(0, train_p.shape[1], iter_limit):
             new_xgb = copy.deepcopy(save_xgb)
-            print('        using %d variables...' %(train_p.shape[1]-i))
-            if train_p.shape[1]-i < iter_limit:
-                X = train_p.iloc[:,i:]
+            print('        using %d variables...' % (train_p.shape[1] - i))
+            if train_p.shape[1] - i < iter_limit:
+                X = train_p.iloc[:, i:]
                 if modeltype == 'Regression':
-                    train_part = int((1-test_size)*X.shape[0])
-                    X_train, X_cv, y_train, y_cv = X[:train_part],X[train_part:],y[:train_part],y[train_part:]
+                    train_part = int((1 - test_size) * X.shape[0])
+                    X_train, X_cv, y_train, y_cv = X[:train_part], X[train_part:], y[:train_part], y[train_part:]
                 else:
                     X_train, X_cv, y_train, y_cv = train_test_split(X, y,
-                                                                test_size=test_size, random_state=seed)
+                                                                    test_size=test_size, random_state=seed)
                 try:
-                    eval_set = [(X_train,y_train),(X_cv,y_cv)]
-                    model_xgb.fit(X_train,y_train,early_stopping_rounds=early_stopping,eval_set=eval_set,
-                                        eval_metric=eval_metric,verbose=False)
+                    eval_set = [(X_train, y_train), (X_cv, y_cv)]
+                    model_xgb.fit(X_train, y_train, early_stopping_rounds=early_stopping, eval_set=eval_set,
+                                  eval_metric=eval_metric, verbose=False)
                     important_features += pd.Series(model_xgb.get_booster().get_score(
-                                importance_type='gain')).sort_values(ascending=False)[:top_num].index.tolist()
+                        importance_type='gain')).sort_values(ascending=False)[:top_num].index.tolist()
                 except:
-                    new_xgb.fit(X_train,y_train,early_stopping_rounds=early_stopping,eval_set=eval_set,
-                                        eval_metric=eval_metric,verbose=False)
-                    print('XGB has a bug in version xgboost 1.02 for feature importances. Try to install version 0.90 or 1.10 - continuing...')
+                    new_xgb.fit(X_train, y_train, early_stopping_rounds=early_stopping, eval_set=eval_set,
+                                eval_metric=eval_metric, verbose=False)
+                    print(
+                        'XGB has a bug in version xgboost 1.02 for feature importances. Try to install version 0.90 or 1.10 - continuing...')
                     important_features += pd.Series(new_xgb.get_booster().get_score(
-                                importance_type='gain')).sort_values(ascending=False)[:top_num].index.tolist()
+                        importance_type='gain')).sort_values(ascending=False)[:top_num].index.tolist()
                 important_features = list(OrderedDict.fromkeys(important_features))
             else:
                 X = train_p[list(train_p.columns.values)[i:train_p.shape[1]]]
                 #### Split here into train and test #####
                 if modeltype == 'Regression':
-                    train_part = int((1-test_size)*X.shape[0])
-                    X_train, X_cv, y_train, y_cv = X[:train_part],X[train_part:],y[:train_part],y[train_part:]
+                    train_part = int((1 - test_size) * X.shape[0])
+                    X_train, X_cv, y_train, y_cv = X[:train_part], X[train_part:], y[:train_part], y[train_part:]
                 else:
                     X_train, X_cv, y_train, y_cv = train_test_split(X, y,
-                                                                test_size=test_size, random_state=seed)
-                eval_set = [(X_train,y_train),(X_cv,y_cv)]
+                                                                    test_size=test_size, random_state=seed)
+                eval_set = [(X_train, y_train), (X_cv, y_cv)]
                 try:
-                    model_xgb.fit(X_train,y_train,early_stopping_rounds=early_stopping,
-                                  eval_set=eval_set,eval_metric=eval_metric,verbose=False)
+                    model_xgb.fit(X_train, y_train, early_stopping_rounds=early_stopping,
+                                  eval_set=eval_set, eval_metric=eval_metric, verbose=False)
                     important_features += pd.Series(model_xgb.get_booster().get_score(
-                                importance_type='gain')).sort_values(ascending=False)[:top_num].index.tolist()
+                        importance_type='gain')).sort_values(ascending=False)[:top_num].index.tolist()
                 except:
-                    new_xgb.fit(X_train,y_train,early_stopping_rounds=early_stopping,
-                                  eval_set=eval_set,eval_metric=eval_metric,verbose=False)
+                    new_xgb.fit(X_train, y_train, early_stopping_rounds=early_stopping,
+                                eval_set=eval_set, eval_metric=eval_metric, verbose=False)
                     important_features += pd.Series(model_xgb.get_booster().get_score(
-                                importance_type='gain')).sort_values(ascending=False)[:top_num].index.tolist()
+                        importance_type='gain')).sort_values(ascending=False)[:top_num].index.tolist()
                 important_features = list(OrderedDict.fromkeys(important_features))
     except:
         print('Finding top features using XGB is crashing. Continuing with all predictors...')
         important_features = copy.deepcopy(preds)
         return important_features, [], []
     important_features = list(OrderedDict.fromkeys(important_features))
-    print('Found %d important features' %len(important_features))
-    #print('    Time taken (in seconds) = %0.0f' %(time.time()-start_time))
+    print('Found %d important features' % len(important_features))
+    # print('    Time taken (in seconds) = %0.0f' %(time.time()-start_time))
     numvars = [x for x in numvars if x in important_features]
     important_cats = [x for x in important_cats if x in important_features]
     return important_features, numvars, important_cats
 ######################################################################################
```

### Comparing `autoviz-0.1.903/autoviz/__init__.py` & `autoviz-0.1.904/autoviz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 else:
     module_type = 'Imported'
 version_number = __version__
 print("""%s v%s. Please call AutoViz in this sequence:
     AV = AutoViz_Class()
     %%matplotlib inline
     dfte = AV.AutoViz(filename, sep=',', depVar='', dfte=None, header=0, verbose=1, lowess=False,
-               chart_format='svg',max_rows_analyzed=150000,max_cols_analyzed=30, save_plot_dir=None)""" %(
+               chart_format='svg',max_rows_analyzed=150000,max_cols_analyzed=30, save_plot_dir=None)""" % (
                module_type, version_number))
 ###########################################################################################
```

### Comparing `autoviz-0.1.903/autoviz/classify_method.py` & `autoviz-0.1.904/autoviz/classify_method.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,73 @@
+import random
+
 import numpy as np
 import pandas as pd
-import random
+
 np.random.seed(99)
 random.seed(42)
 ################################################################################
 #### The warnings from Sklearn are so annoying that I have to shut it off #######
 import warnings
+
 warnings.filterwarnings("ignore")
 from sklearn.exceptions import DataConversionWarning
+
 warnings.filterwarnings(action='ignore', category=DataConversionWarning)
+
+
 def warn(*args, **kwargs):
     pass
+
+
 warnings.warn = warn
-import logging
 ####################################################################################
 from functools import reduce
-import copy
-import time
-def left_subtract(l1,l2):
+
+
+def left_subtract(l1, l2):
     lst = []
     for i in l1:
         if i not in l2:
             lst.append(i)
     return lst
+
+
 #################################################################################
 import copy
+
+
 def EDA_find_remove_columns_with_infinity(df, remove=False, verbose=0):
     """
-    This function finds all columns in a dataframe that have inifinite values (np.inf or -np.inf)
+    This function finds all columns in a dataframe that have infinite values (np.inf or -np.inf)
     It returns a list of column names. If the list is empty, it means no columns were found.
     If remove flag is set, then it returns a smaller dataframe with inf columns removed.
     """
     nums = df.select_dtypes(include='number').columns.tolist()
     dfx = df[nums]
     sum_rows = np.isinf(dfx).values.sum()
-    add_cols =  list(dfx.columns.to_series()[np.isinf(dfx).any()])
+    add_cols = list(dfx.columns.to_series()[np.isinf(dfx).any()])
     if sum_rows > 0:
         if verbose > 0:
-            print('    there are %d rows and %d columns with infinity in them...' %(sum_rows,len(add_cols)))
+            print('    there are %d rows and %d columns with infinity in them...' % (sum_rows, len(add_cols)))
         if remove:
             ### here you need to use df since the whole dataset is involved ###
             nocols = [x for x in df.columns if x not in add_cols]
             if verbose > 0:
-                print("    Shape of dataset before %s and after %s removing columns with infinity" %(df.shape,(df[nocols].shape,)))
+                print("    Shape of dataset before %s and after %s removing columns with infinity" %
+                      (df.shape, (df[nocols].shape,)))
             return df[nocols]
         else:
             ## this will be a list of columns with infinity ####
             return add_cols
     else:
         ## this will be an empty list if there are no columns with infinity
         return add_cols
+
+
 ####################################################################################
 def classify_columns(df_preds, verbose=0):
     """
     This actually does Exploratory data analysis - it means this function performs EDA
     ######################################################################################
     Takes a dataframe containing only predictors to be classified into various types.
     DO NOT SEND IN A TARGET COLUMN since it will try to include that into various columns.
@@ -68,213 +82,216 @@
     max_cols_to_print = 30
     print('#######################################################################################')
     print('######################## C L A S S I F Y I N G  V A R I A B L E S  ####################')
     print('#######################################################################################')
     print('Classifying variables in data set...')
     #### Cat_Limit defines the max number of categories a column can have to be called a categorical colum
     cat_limit = 35
-    float_limit = 15 #### Make this limit low so that float variables below this limit become cat vars ###
-    def add(a,b):
-        return a+b
+    float_limit = 15  #### Make this limit low so that float variables below this limit become cat vars ###
+
+    def add(a, b):
+        return a + b
+
     sum_all_cols = dict()
     orig_cols_total = train.shape[1]
-    #Types of columns
+    # Types of columns
     cols_delete = []
-    cols_delete = [col for col in list(train) if (len(train[col].value_counts()) == 1
-                                       ) | (train[col].isnull().sum()/len(train) >= 0.90)]
+    cols_delete = [col for col in list(train) if (len(train[col].value_counts()) == 1)
+                   | (train[col].isnull().sum() / len(train) >= 0.90)]
     inf_cols = EDA_find_remove_columns_with_infinity(train, remove=False, verbose=verbose)
     mixed_cols = [x for x in list(train) if len(train[x].dropna().apply(type).value_counts()) > 1]
     if len(mixed_cols) > 0:
-        print('    Removing %s column(s) due to mixed data type detected...' %mixed_cols)
+        print('    Removing %s column(s) due to mixed data type detected...' % mixed_cols)
     cols_delete += mixed_cols
     cols_delete += inf_cols
-    train = train[left_subtract(list(train),cols_delete)]
+    train = train[left_subtract(list(train), cols_delete)]
     var_df = pd.Series(dict(train.dtypes)).reset_index(drop=False).rename(
-                        columns={0:'type_of_column'})
+        columns={0: 'type_of_column'})
     sum_all_cols['cols_delete'] = cols_delete
 
-    var_df['bool'] = var_df.apply(lambda x: 1 if x['type_of_column'] in ['bool','object']
-                        and len(train[x['index']].value_counts()) == 2 else 0, axis=1)
-    string_bool_vars = list(var_df[(var_df['bool'] ==1)]['index'])
+    var_df['bool'] = var_df.apply(
+        lambda x: 1 if x['type_of_column'] in ['bool', 'object'] and len(train[x['index']].value_counts()) == 2 else 0,
+        axis=1)
+    string_bool_vars = list(var_df[(var_df['bool'] == 1)]['index'])
     sum_all_cols['string_bool_vars'] = string_bool_vars
     var_df['num_bool'] = var_df.apply(lambda x: 1 if x['type_of_column'] in [np.uint8,
-                            np.uint16, np.uint32, np.uint64,
-                            'int8','int16','int32','int64',
-                            'float16','float32','float64'] and len(
-                        train[x['index']].value_counts()) == 2 else 0, axis=1)
-    num_bool_vars = list(var_df[(var_df['num_bool'] ==1)]['index'])
+                                                                             np.uint16, np.uint32, np.uint64,
+                                                                             'int8', 'int16', 'int32', 'int64',
+                                                                             'float16', 'float32', 'float64'] and len(
+        train[x['index']].value_counts()) == 2 else 0, axis=1)
+    num_bool_vars = list(var_df[(var_df['num_bool'] == 1)]['index'])
     sum_all_cols['num_bool_vars'] = num_bool_vars
     ######   This is where we take all Object vars and split them into diff kinds ###
-    discrete_or_nlp = var_df.apply(lambda x: 1 if x['type_of_column'] in ['object']  and x[
-        'index'] not in string_bool_vars+cols_delete else 0,axis=1)
+    discrete_or_nlp = var_df.apply(lambda x: 1 if x['type_of_column'] in ['object'] and x[
+        'index'] not in string_bool_vars + cols_delete else 0, axis=1)
     ######### This is where we figure out whether a string var is nlp or discrete_string var ###
     var_df['nlp_strings'] = 0
     var_df['discrete_strings'] = 0
     var_df['cat'] = 0
     var_df['id_col'] = 0
-    discrete_or_nlp_vars = var_df.loc[discrete_or_nlp==1]['index'].values.tolist()
+    discrete_or_nlp_vars = var_df.loc[discrete_or_nlp == 1]['index'].values.tolist()
     copy_discrete_or_nlp_vars = copy.deepcopy(discrete_or_nlp_vars)
     if len(discrete_or_nlp_vars) > 0:
         for col in copy_discrete_or_nlp_vars:
             #### first fill empty or missing vals since it will blowup ###
             ### Remember that fillna only works at the dataframe level!
             train[[col]] = train[[col]].fillna('  ')
-            if train[col].map(lambda x: len(x) if type(x)==str else 0).max(
-                ) >= 50 and len(train[col].value_counts()
-                        ) >= int(0.9*len(train)) and col not in string_bool_vars:
-                var_df.loc[var_df['index']==col,'nlp_strings'] = 1
-            elif train[col].map(lambda x: len(x) if type(x)==str else 0).mean(
-                ) >= max_nlp_char_size and train[col].map(lambda x: len(x) if type(x)==str else 0).max(
-                ) < 50 and len(train[col].value_counts()
-                        ) <= int(0.9*len(train)) and col not in string_bool_vars:
-                var_df.loc[var_df['index']==col,'discrete_strings'] = 1
+            if train[col].map(lambda x: len(x) if type(x) == str else 0).max(
+            ) >= 50 and len(train[col].value_counts()) >= int(0.9 * len(train)) and col not in string_bool_vars:
+                var_df.loc[var_df['index'] == col, 'nlp_strings'] = 1
+            elif train[col].map(lambda x: len(x) if type(x) == str else 0).mean(
+            ) >= max_nlp_char_size and train[col].map(lambda x: len(x) if type(x) == str else 0).max(
+            ) < 50 and len(train[col].value_counts()
+                           ) <= int(0.9 * len(train)) and col not in string_bool_vars:
+                var_df.loc[var_df['index'] == col, 'discrete_strings'] = 1
+            elif len(train[col].value_counts()) > cat_limit and len(
+                    train[col].value_counts()) <= int(0.9 * len(train)) and col not in string_bool_vars:
+                var_df.loc[var_df['index'] == col, 'discrete_strings'] = 1
             elif len(train[col].value_counts()) > cat_limit and len(train[col].value_counts()
-                        ) <= int(0.9*len(train)) and col not in string_bool_vars:
-                var_df.loc[var_df['index']==col,'discrete_strings'] = 1
-            elif len(train[col].value_counts()) > cat_limit and len(train[col].value_counts()
-                        ) == len(train) and col not in string_bool_vars:
-                var_df.loc[var_df['index']==col,'id_col'] = 1
+                                                                    ) == len(train) and col not in string_bool_vars:
+                var_df.loc[var_df['index'] == col, 'id_col'] = 1
             else:
-                var_df.loc[var_df['index']==col,'cat'] = 1
-    nlp_vars = list(var_df[(var_df['nlp_strings'] ==1)]['index'])
+                var_df.loc[var_df['index'] == col, 'cat'] = 1
+    nlp_vars = list(var_df[(var_df['nlp_strings'] == 1)]['index'])
     sum_all_cols['nlp_vars'] = nlp_vars
-    discrete_string_vars = list(var_df[(var_df['discrete_strings'] ==1) ]['index'])
+    discrete_string_vars = list(var_df[(var_df['discrete_strings'] == 1)]['index'])
     sum_all_cols['discrete_string_vars'] = discrete_string_vars
     ###### This happens only if a string column happens to be an ID column #######
-    #### DO NOT Add this to ID_VARS yet. It will be done later.. Dont change it easily...
+    #### DO NOT Add this to ID_VARS yet. It will be done later. Don't change it easily...
     #### Category DTYPE vars are very special = they can be left as is and not disturbed in Python. ###
-    var_df['dcat'] = var_df.apply(lambda x: 1 if str(x['type_of_column'])=='category' else 0,
-                            axis=1)
-    factor_vars = list(var_df[(var_df['dcat'] ==1)]['index'])
+    var_df['dcat'] = var_df.apply(lambda x: 1 if str(x['type_of_column']) == 'category' else 0,
+                                  axis=1)
+    factor_vars = list(var_df[(var_df['dcat'] == 1)]['index'])
     sum_all_cols['factor_vars'] = factor_vars
     ########################################################################
     date_or_id = var_df.apply(lambda x: 1 if x['type_of_column'] in [np.uint8,
-                         np.uint16, np.uint32, np.uint64,
-                         'int8','int16',
-                        'int32','int64']  and x[
-        'index'] not in string_bool_vars+num_bool_vars+discrete_string_vars+nlp_vars else 0,
-                                        axis=1)
+                                                                     np.uint16, np.uint32, np.uint64,
+                                                                     'int8', 'int16',
+                                                                     'int32', 'int64'] and x[
+                                                 'index'] not in (string_bool_vars + num_bool_vars +
+                                                                  discrete_string_vars + nlp_vars) else 0,
+                              axis=1)
     ######### This is where we figure out whether a numeric col is date or id variable ###
     var_df['int'] = 0
     var_df['date_time'] = 0
     ### if a particular column is date-time type, now set it as a date time variable ##
-    var_df['date_time'] = var_df.apply(lambda x: 1 if x['type_of_column'] in ['<M8[ns]','datetime64[ns]']  and x[
-        'index'] not in string_bool_vars+num_bool_vars+discrete_string_vars+nlp_vars else 0,
-                                        axis=1)
+    var_df['date_time'] = var_df.apply(lambda x: 1 if x['type_of_column'] in ['<M8[ns]', 'datetime64[ns]'] and x[
+        'index'] not in string_bool_vars + num_bool_vars + discrete_string_vars + nlp_vars else 0,
+                                       axis=1)
     ### this is where we save them as date time variables ###
-    if len(var_df.loc[date_or_id==1]) != 0:
-        for col in var_df.loc[date_or_id==1]['index'].values.tolist():
+    if len(var_df.loc[date_or_id == 1]) != 0:
+        for col in var_df.loc[date_or_id == 1]['index'].values.tolist():
             if len(train[col].value_counts()) == len(train):
                 if train[col].min() < 1900 or train[col].max() > 2050:
-                    var_df.loc[var_df['index']==col,'id_col'] = 1
+                    var_df.loc[var_df['index'] == col, 'id_col'] = 1
                 else:
                     try:
-                        pd.to_datetime(train[col],infer_datetime_format=True)
-                        var_df.loc[var_df['index']==col,'date_time'] = 1
+                        pd.to_datetime(train[col], infer_datetime_format=True)
+                        var_df.loc[var_df['index'] == col, 'date_time'] = 1
                     except:
-                        var_df.loc[var_df['index']==col,'id_col'] = 1
+                        var_df.loc[var_df['index'] == col, 'id_col'] = 1
             else:
                 if train[col].min() < 1900 or train[col].max() > 2050:
                     if col not in num_bool_vars:
-                        var_df.loc[var_df['index']==col,'int'] = 1
+                        var_df.loc[var_df['index'] == col, 'int'] = 1
                 else:
                     try:
-                        pd.to_datetime(train[col],infer_datetime_format=True)
-                        var_df.loc[var_df['index']==col,'date_time'] = 1
+                        pd.to_datetime(train[col], infer_datetime_format=True)
+                        var_df.loc[var_df['index'] == col, 'date_time'] = 1
                     except:
                         if col not in num_bool_vars:
-                            var_df.loc[var_df['index']==col,'int'] = 1
+                            var_df.loc[var_df['index'] == col, 'int'] = 1
     else:
         pass
-    int_vars = list(var_df[(var_df['int'] ==1)]['index'])
+    int_vars = list(var_df[(var_df['int'] == 1)]['index'])
     date_vars = list(var_df[(var_df['date_time'] == 1)]['index'])
     id_vars = list(var_df[(var_df['id_col'] == 1)]['index'])
     sum_all_cols['int_vars'] = int_vars
     copy_date_vars = copy.deepcopy(date_vars)
     for date_var in copy_date_vars:
-        #### This test is to make sure sure date vars are actually date vars
+        #### This test is to make sure date vars are actually date vars
         try:
-            pd.to_datetime(train[date_var],infer_datetime_format=True)
+            pd.to_datetime(train[date_var], infer_datetime_format=True)
         except:
             ##### if not a date var, then just add it to delete it from processing
             cols_delete.append(date_var)
             date_vars.remove(date_var)
     sum_all_cols['date_vars'] = date_vars
     sum_all_cols['id_vars'] = id_vars
     sum_all_cols['cols_delete'] = cols_delete
     ## This is an EXTREMELY complicated logic for cat vars. Don't change it unless you test it many times!
     var_df['numeric'] = 0
     float_or_cat = var_df.apply(lambda x: 1 if x['type_of_column'] in ['float16',
-                            'float32','float64'] else 0,
-                                        axis=1)
+                                                                       'float32', 'float64'] else 0,
+                                axis=1)
     #######  We need to make sure there are no categorical vars in float #######
     if len(var_df.loc[float_or_cat == 1]) > 0:
         for col in var_df.loc[float_or_cat == 1]['index'].values.tolist():
-            if len(train[col].value_counts()) > 2 and len(train[col].value_counts()
-                ) <= float_limit and len(train[col].value_counts()) <= len(train):
-                var_df.loc[var_df['index']==col,'cat'] = 1
+            if 2 < len(train[col].value_counts()) <= float_limit and len(
+                    train[col].value_counts()) <= len(train):
+                var_df.loc[var_df['index'] == col, 'cat'] = 1
             else:
                 if col not in (num_bool_vars + factor_vars):
-                    var_df.loc[var_df['index']==col,'numeric'] = 1
-    cat_vars = list(var_df[(var_df['cat'] ==1)]['index'])
-    continuous_vars = list(var_df[(var_df['numeric'] ==1)]['index'])
+                    var_df.loc[var_df['index'] == col, 'numeric'] = 1
+    cat_vars = list(var_df[(var_df['cat'] == 1)]['index'])
+    continuous_vars = list(var_df[(var_df['numeric'] == 1)]['index'])
 
     ########  V E R Y    I M P O R T A N T   ###################################################
     cat_vars_copy = copy.deepcopy(factor_vars)
     for cat in cat_vars_copy:
-        if df_preds[cat].dtype==float:
+        if df_preds[cat].dtype == float:
             continuous_vars.append(cat)
             factor_vars.remove(cat)
-            var_df.loc[var_df['index']==cat,'dcat'] = 0
-            var_df.loc[var_df['index']==cat,'numeric'] = 1
+            var_df.loc[var_df['index'] == cat, 'dcat'] = 0
+            var_df.loc[var_df['index'] == cat, 'numeric'] = 1
         elif len(df_preds[cat].value_counts()) == df_preds.shape[0]:
             id_vars.append(cat)
             factor_vars.remove(cat)
-            var_df.loc[var_df['index']==cat,'dcat'] = 0
-            var_df.loc[var_df['index']==cat,'id_col'] = 1
+            var_df.loc[var_df['index'] == cat, 'dcat'] = 0
+            var_df.loc[var_df['index'] == cat, 'id_col'] = 1
 
     sum_all_cols['factor_vars'] = factor_vars
     ##### There are a couple of extra tests you need to do to remove abberations in cat_vars ###
     cat_vars_copy = copy.deepcopy(cat_vars)
     for cat in cat_vars_copy:
-        if df_preds[cat].dtype==float:
+        if df_preds[cat].dtype == float:
             continuous_vars.append(cat)
             cat_vars.remove(cat)
-            var_df.loc[var_df['index']==cat,'cat'] = 0
-            var_df.loc[var_df['index']==cat,'numeric'] = 1
+            var_df.loc[var_df['index'] == cat, 'cat'] = 0
+            var_df.loc[var_df['index'] == cat, 'numeric'] = 1
         elif len(df_preds[cat].value_counts()) == df_preds.shape[0]:
             id_vars.append(cat)
             cat_vars.remove(cat)
-            var_df.loc[var_df['index']==cat,'cat'] = 0
-            var_df.loc[var_df['index']==cat,'id_col'] = 1
+            var_df.loc[var_df['index'] == cat, 'cat'] = 0
+            var_df.loc[var_df['index'] == cat, 'id_col'] = 1
     sum_all_cols['cat_vars'] = cat_vars
     sum_all_cols['continuous_vars'] = continuous_vars
     sum_all_cols['id_vars'] = id_vars
-    ###### This is where you consoldate the numbers ###########
-    var_dict_sum = dict(zip(var_df.values[:,0], var_df.values[:,2:].sum(1)))
+    ###### This is where you consolidate the numbers ###########
+    var_dict_sum = dict(zip(var_df.values[:, 0], var_df.values[:, 2:].sum(1)))
     for col, sumval in var_dict_sum.items():
         if sumval == 0:
-            print('%s of type=%s is not classified' %(col,train[col].dtype))
+            print('%s of type=%s is not classified' % (col, train[col].dtype))
         elif sumval > 1:
-            print('%s of type=%s is classified into more then one type' %(col,train[col].dtype))
+            print('%s of type=%s is classified into more then one type' % (col, train[col].dtype))
         else:
             pass
     ##### If there are more than 1000 unique values, then add it to NLP vars ###
-    copy_discretes = copy.deepcopy(discrete_string_vars)
-    for each_discrete in copy_discretes:
+    copy_discrete_vals = copy.deepcopy(discrete_string_vars)
+    for each_discrete in copy_discrete_vals:
         if train[each_discrete].nunique() >= 1000:
             nlp_vars.append(each_discrete)
             discrete_string_vars.remove(each_discrete)
-        elif train[each_discrete].nunique() > 100 and train[each_discrete].nunique() < 1000:
+        elif 100 < train[each_discrete].nunique() < 1000:
             pass
         else:
             ### If it is less than 100 unique values, then make it categorical var
             cat_vars.append(each_discrete)
             discrete_string_vars.remove(each_discrete)
-    sum_all_cols['discrete_string_vars'] =  discrete_string_vars
+    sum_all_cols['discrete_string_vars'] = discrete_string_vars
     sum_all_cols['cat_vars'] = cat_vars
     sum_all_cols['nlp_vars'] = nlp_vars
     ###############  This is where you print all the types of variables ##############
     ####### Returns 8 vars in the following order: continuous_vars,int_vars,cat_vars,
     ###  string_bool_vars,discrete_string_vars,nlp_vars,date_or_id_vars,cols_delete
     if verbose == 1:
         print("    Number of Numeric Columns = ", len(continuous_vars))
@@ -285,37 +302,36 @@
         print("    Number of Numeric-Boolean Columns = ", len(num_bool_vars))
         print("    Number of Discrete String Columns = ", len(discrete_string_vars))
         print("    Number of NLP String Columns = ", len(nlp_vars))
         print("    Number of Date Time Columns = ", len(date_vars))
         print("    Number of ID Columns = ", len(id_vars))
         print("    Number of Columns to Delete = ", len(cols_delete))
     if verbose >= 2:
-        print('  Printing upto %d columns (max) in each category:' %max_cols_to_print)
-        print("    Numeric Columns : %s" %continuous_vars[:max_cols_to_print])
-        print("    Integer-Categorical Columns: %s" %int_vars[:max_cols_to_print])
-        print("    String-Categorical Columns: %s" %cat_vars[:max_cols_to_print])
-        print("    Factor-Categorical Columns: %s" %factor_vars[:max_cols_to_print])
-        print("    String-Boolean Columns: %s" %string_bool_vars[:max_cols_to_print])
-        print("    Numeric-Boolean Columns: %s" %num_bool_vars[:max_cols_to_print])
-        print("    Discrete String Columns: %s" %discrete_string_vars[:max_cols_to_print])
-        print("    NLP text Columns: %s" %nlp_vars[:max_cols_to_print])
-        print("    Date Time Columns: %s" %date_vars[:max_cols_to_print])
-        print("    ID Columns: %s" %id_vars[:max_cols_to_print])
-        print("    Columns that will not be considered in modeling: %s" %cols_delete[:max_cols_to_print])
+        print('  Printing up to %d columns (max) in each category:' % max_cols_to_print)
+        print("    Numeric Columns : %s" % continuous_vars[:max_cols_to_print])
+        print("    Integer-Categorical Columns: %s" % int_vars[:max_cols_to_print])
+        print("    String-Categorical Columns: %s" % cat_vars[:max_cols_to_print])
+        print("    Factor-Categorical Columns: %s" % factor_vars[:max_cols_to_print])
+        print("    String-Boolean Columns: %s" % string_bool_vars[:max_cols_to_print])
+        print("    Numeric-Boolean Columns: %s" % num_bool_vars[:max_cols_to_print])
+        print("    Discrete String Columns: %s" % discrete_string_vars[:max_cols_to_print])
+        print("    NLP text Columns: %s" % nlp_vars[:max_cols_to_print])
+        print("    Date Time Columns: %s" % date_vars[:max_cols_to_print])
+        print("    ID Columns: %s" % id_vars[:max_cols_to_print])
+        print("    Columns that will not be considered in modeling: %s" % cols_delete[:max_cols_to_print])
     ##### now collect all the column types and column names into a single dictionary to return!
 
-    len_sum_all_cols = reduce(add,[len(v) for v in sum_all_cols.values()])
+    len_sum_all_cols = reduce(add, [len(v) for v in sum_all_cols.values()])
     if len_sum_all_cols == orig_cols_total:
-        print('    %d Predictors classified...' %orig_cols_total)
-        #print('        This does not include the Target column(s)')
+        print('    %d Predictors classified...' % orig_cols_total)
+        # print('        This does not include the Target column(s)')
     else:
-        print('No of columns classified %d does not match %d total cols. Continuing...' %(
-                   len_sum_all_cols, orig_cols_total))
+        print('No of columns classified %d does not match %d total cols. Continuing...' % (
+            len_sum_all_cols, orig_cols_total))
         ls = sum_all_cols.values()
         flat_list = [item for sublist in ls for item in sublist]
-        if len(left_subtract(list(train),flat_list)) == 0:
+        if len(left_subtract(list(train), flat_list)) == 0:
             print(' Missing columns = None')
         else:
-            print(' Missing columns = %s' %left_subtract(list(train),flat_list))
+            print(' Missing columns = %s' % left_subtract(list(train), flat_list))
     return sum_all_cols
 ####################################################################################
-
```

### Comparing `autoviz-0.1.903/autoviz.egg-info/PKG-INFO` & `autoviz-0.1.904/autoviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: autoviz
-Version: 0.1.903
+Version: 0.1.904
 Summary: Automatically Visualize any dataset, any size with a single line of code
 Home-page: https://github.com/AutoViML/AutoViz.git
 Author: Ram Seshadri
 License: Apache License 2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # AutoViz: The One-Line Automatic Data Visualization Library
 
@@ -267,7 +268,8 @@
   <li>Assumes the first row as the header in the file, but this can be changed.</li>
 </ul>
 
 - **By leveraging AutoViz's powerful and flexible features**, you can streamline your data visualization process and gain valuable insights more efficiently. Happy visualizing!
 
 ## DISCLAIMER
 This project is not an official Google project. It is not supported by Google, and Google specifically disclaims all warranties as to its quality, merchantability, or fitness for a particular purpose.
+
```

#### html2text {}

```diff
@@ -1,30 +1,31 @@
-Metadata-Version: 2.1 Name: autoviz Version: 0.1.903 Summary: Automatically
+Metadata-Version: 2.1 Name: autoviz Version: 0.1.904 Summary: Automatically
 Visualize any dataset, any size with a single line of code Home-page: https://
 github.com/AutoViML/AutoViz.git Author: Ram Seshadri License: Apache License
-2.0 Classifier: Programming Language :: Python :: 3 Classifier: Operating
-System :: OS Independent Description-Content-Type: text/markdown License-File:
-LICENSE # AutoViz: The One-Line Automatic Data Visualization Library ![logo]
-(images/logo.png) Unlock the power of **AutoViz** to visualize any dataset, any
-size, with just a single line of code! Plus, now you can get a quick assessment
-of your dataset's quality and fix DQ issues through the FixDQ() function. [!
-[Pepy Downloads](https://pepy.tech/badge/autoviz)](https://pepy.tech/project/
-autoviz) [![Pepy Downloads per week](https://pepy.tech/badge/autoviz/week)]
-(https://pepy.tech/project/autoviz) [![Pepy Downloads per month](https://
-pepy.tech/badge/autoviz/month)](https://pepy.tech/project/autoviz) [![standard-
-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg)]
-(https://github.com/RichardLitt/standard-readme) [![Python Versions](https://
-img.shields.io/pypi/pyversions/autoviz.svg)](https://pypi.org/project/autoviz)
-[![PyPI Version](https://img.shields.io/pypi/v/autoviz.svg)](https://pypi.org/
-project/autoviz) [![PyPI License](https://img.shields.io/pypi/l/autoviz.svg)]
-(https://github.com/AutoViML/AutoViz/blob/master/LICENSE) With AutoViz, you can
-easily and quickly generate insightful visualizations for your data. Whether
-you're a beginner or an expert in data analysis, AutoViz can help you explore
-your data and uncover valuable insights. Try it out and see the power of
-automated visualization for yourself! ## Table of Contents
+2.0 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent Description-Content-Type: text/
+markdown License-File: LICENSE # AutoViz: The One-Line Automatic Data
+Visualization Library ![logo](images/logo.png) Unlock the power of **AutoViz**
+to visualize any dataset, any size, with just a single line of code! Plus, now
+you can get a quick assessment of your dataset's quality and fix DQ issues
+through the FixDQ() function. [![Pepy Downloads](https://pepy.tech/badge/
+autoviz)](https://pepy.tech/project/autoviz) [![Pepy Downloads per week](https:
+//pepy.tech/badge/autoviz/week)](https://pepy.tech/project/autoviz) [![Pepy
+Downloads per month](https://pepy.tech/badge/autoviz/month)](https://pepy.tech/
+project/autoviz) [![standard-readme compliant](https://img.shields.io/badge/
+standard--readme-OK-green.svg)](https://github.com/RichardLitt/standard-readme)
+[![Python Versions](https://img.shields.io/pypi/pyversions/autoviz.svg)](https:
+//pypi.org/project/autoviz) [![PyPI Version](https://img.shields.io/pypi/v/
+autoviz.svg)](https://pypi.org/project/autoviz) [![PyPI License](https://
+img.shields.io/pypi/l/autoviz.svg)](https://github.com/AutoViML/AutoViz/blob/
+master/LICENSE) With AutoViz, you can easily and quickly generate insightful
+visualizations for your data. Whether you're a beginner or an expert in data
+analysis, AutoViz can help you explore your data and uncover valuable insights.
+Try it out and see the power of automated visualization for yourself! ## Table
+of Contents
     * _L_a_t_e_s_t_ _U_p_d_a_t_e_s
     * _I_m_p_o_r_t_a_n_t_ _A_n_n_o_u_n_c_e_m_e_n_t
     * _C_i_t_a_t_i_o_n
     * _M_o_t_i_v_a_t_i_o_n_ _f_o_r_ _A_u_t_o_V_i_z
     * _H_o_w_ _t_o_ _u_s_e_ _A_u_t_o_V_i_z
     * _A_P_I_ _f_o_r_ _u_s_i_n_g_ _A_u_t_o_V_i_z
     * _E_x_a_m_p_l_e_s_ _o_f_ _u_s_i_n_g_ _A_u_t_o_V_i_z
```

### Comparing `autoviz-0.1.903/setup.py` & `autoviz-0.1.904/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "pandas>=2.0", ## pandas must be below 2.0 version
     "matplotlib>3.7.4", ## newer version of matplotlib
     "seaborn>0.12.2", ## newer version of seaborn ##
 ]
 
 setuptools.setup(
     name="autoviz",
-    version="0.1.903",
+    version="0.1.904",
     author="Ram Seshadri",
     description="Automatically Visualize any dataset, any size with a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/AutoViz.git",
     packages=setuptools.find_packages(exclude=("tests",)),
```

