# Comparing `tmp/clipkit-2.2.6.tar.gz` & `tmp/clipkit-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipkit-2.2.6.tar", last modified: Fri Apr 12 23:23:04 2024, max compression
+gzip compressed data, was "clipkit-2.3.0.tar", last modified: Mon Apr 29 19:13:27 2024, max compression
```

## Comparing `clipkit-2.2.6.tar` & `clipkit-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-12 23:23:04.708958 clipkit-2.2.6/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2020-10-28 23:29:32.000000 clipkit-2.2.6/LICENSE.md
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-04-12 23:23:04.708525 clipkit-2.2.6/PKG-INFO
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4564 2024-02-07 15:51:48.000000 clipkit-2.2.6/README.md
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-12 23:23:04.703202 clipkit-2.2.6/clipkit/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       25 2023-07-21 16:57:06.000000 clipkit-2.2.6/clipkit/__init__.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      124 2020-10-04 18:34:57.000000 clipkit-2.2.6/clipkit/__main__.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2129 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/api.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1849 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/args_processing.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5517 2024-04-12 23:22:01.000000 clipkit-2.2.6/clipkit/clipkit.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      103 2023-07-21 16:57:06.000000 clipkit-2.2.6/clipkit/exceptions.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2198 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/files.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2330 2024-03-04 23:25:45.000000 clipkit-2.2.6/clipkit/helpers.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      193 2023-07-21 16:57:06.000000 clipkit-2.2.6/clipkit/logger.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      563 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/modes.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)    10486 2024-04-04 03:22:22.000000 clipkit-2.2.6/clipkit/msa.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     9703 2024-04-02 18:24:46.000000 clipkit-2.2.6/clipkit/parser.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      108 2024-03-18 22:22:33.000000 clipkit-2.2.6/clipkit/settings.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1538 2023-09-24 21:24:47.000000 clipkit-2.2.6/clipkit/site_classification.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2267 2024-02-18 20:23:57.000000 clipkit-2.2.6/clipkit/smart_gap_helper.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      912 2023-09-24 21:24:47.000000 clipkit-2.2.6/clipkit/stats.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       22 2024-04-12 23:22:08.000000 clipkit-2.2.6/clipkit/version.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      648 2023-09-24 21:24:47.000000 clipkit-2.2.6/clipkit/warnings.py
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2388 2024-02-13 00:05:53.000000 clipkit-2.2.6/clipkit/write.py
-drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-12 23:23:04.707066 clipkit-2.2.6/clipkit.egg-info/
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5214 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/PKG-INFO
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      596 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/SOURCES.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/dependency_links.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       49 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/entry_points.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       37 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/requires.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        8 2024-04-12 23:23:04.000000 clipkit-2.2.6/clipkit.egg-info/top_level.txt
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2024-04-12 23:23:04.709199 clipkit-2.2.6/setup.cfg
--rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1211 2024-02-18 20:19:59.000000 clipkit-2.2.6/setup.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-29 19:13:27.939252 clipkit-2.3.0/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1078 2020-10-28 23:29:32.000000 clipkit-2.3.0/LICENSE.md
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5265 2024-04-29 19:13:27.939040 clipkit-2.3.0/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     4564 2024-02-07 15:51:48.000000 clipkit-2.3.0/README.md
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-29 19:13:27.937081 clipkit-2.3.0/clipkit/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       25 2023-07-21 16:57:06.000000 clipkit-2.3.0/clipkit/__init__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      124 2020-10-04 18:34:57.000000 clipkit-2.3.0/clipkit/__main__.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2129 2024-04-02 18:24:46.000000 clipkit-2.3.0/clipkit/api.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1849 2024-04-02 18:24:46.000000 clipkit-2.3.0/clipkit/args_processing.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5517 2024-04-12 23:22:01.000000 clipkit-2.3.0/clipkit/clipkit.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      103 2023-07-21 16:57:06.000000 clipkit-2.3.0/clipkit/exceptions.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2198 2024-04-02 18:24:46.000000 clipkit-2.3.0/clipkit/files.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2330 2024-03-04 23:25:45.000000 clipkit-2.3.0/clipkit/helpers.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      193 2023-07-21 16:57:06.000000 clipkit-2.3.0/clipkit/logger.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      563 2024-04-02 18:24:46.000000 clipkit-2.3.0/clipkit/modes.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)    10486 2024-04-04 03:22:22.000000 clipkit-2.3.0/clipkit/msa.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     9703 2024-04-02 18:24:46.000000 clipkit-2.3.0/clipkit/parser.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      108 2024-03-18 22:22:33.000000 clipkit-2.3.0/clipkit/settings.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1538 2023-09-24 21:24:47.000000 clipkit-2.3.0/clipkit/site_classification.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2267 2024-02-18 20:23:57.000000 clipkit-2.3.0/clipkit/smart_gap_helper.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      912 2023-09-24 21:24:47.000000 clipkit-2.3.0/clipkit/stats.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       22 2024-04-22 22:26:30.000000 clipkit-2.3.0/clipkit/version.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      648 2023-09-24 21:24:47.000000 clipkit-2.3.0/clipkit/warnings.py
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     2388 2024-02-13 00:05:53.000000 clipkit-2.3.0/clipkit/write.py
+drwxr-xr-x   0 jacoblsteenwyk   (501) staff       (20)        0 2024-04-29 19:13:27.938760 clipkit-2.3.0/clipkit.egg-info/
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     5265 2024-04-29 19:13:27.000000 clipkit-2.3.0/clipkit.egg-info/PKG-INFO
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)      596 2024-04-29 19:13:27.000000 clipkit-2.3.0/clipkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        1 2024-04-29 19:13:27.000000 clipkit-2.3.0/clipkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       49 2024-04-29 19:13:27.000000 clipkit-2.3.0/clipkit.egg-info/entry_points.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       37 2024-04-29 19:13:27.000000 clipkit-2.3.0/clipkit.egg-info/requires.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)        8 2024-04-29 19:13:27.000000 clipkit-2.3.0/clipkit.egg-info/top_level.txt
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)       38 2024-04-29 19:13:27.939304 clipkit-2.3.0/setup.cfg
+-rw-r--r--   0 jacoblsteenwyk   (501) staff       (20)     1257 2024-04-29 19:09:19.000000 clipkit-2.3.0/setup.py
```

### Comparing `clipkit-2.2.6/LICENSE.md` & `clipkit-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/PKG-INFO` & `clipkit-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: clipkit
-Version: 2.2.6
+Version: 2.3.0
 Summary: Alignment trimming software for phylogenetics.
 Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: biopython>=1.81
+Requires-Dist: biopython>=1.82
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: cython
 
 <p align="center">
   <a href="https://github.com/jlsteenwyk/clipkit">
     <img src="https://raw.githubusercontent.com/JLSteenwyk/ClipKIT/master/docs/_static/img/logo.jpg" alt="Logo" width="400">
   </a>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: clipkit Version: 2.2.6 Summary: Alignment trimming
+Metadata-Version: 2.1 Name: clipkit Version: 2.3.0 Summary: Alignment trimming
 software for phylogenetics. Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk Author-email: jlsteenwyk@gmail.com Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Science/
 Research Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
-markdown License-File: LICENSE.md Requires-Dist: biopython>=1.81 Requires-Dist:
-numpy>=1.24.0 Requires-Dist: cython
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering Description-Content-Type: text/markdown License-File:
+LICENSE.md Requires-Dist: biopython>=1.82 Requires-Dist: numpy>=1.24.0
+Requires-Dist: cython
                                     _[_L_o_g_o_]
                      _D_o_c_s Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_J_L_S_t_e_e_n_w_y_k_/_C_l_i_p_K_I_T_/
  _c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_j_l_s_t_e_e_n_w_y_k_/_c_l_i_p_k_i_t_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/
  _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_0_J_4_9_I_6_4_4_1_V_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_n_t_r_i_b_u_t_o_r_s_/
                     _j_l_s_t_e_e_n_w_y_k_/_c_l_i_p_k_i_t_]_[_f_o_l_l_o_w_ _o_n_ _T_w_i_t_t_e_r_]
                  _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
```

### Comparing `clipkit-2.2.6/README.md` & `clipkit-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/api.py` & `clipkit-2.3.0/clipkit/api.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/args_processing.py` & `clipkit-2.3.0/clipkit/args_processing.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/clipkit.py` & `clipkit-2.3.0/clipkit/clipkit.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/files.py` & `clipkit-2.3.0/clipkit/files.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/helpers.py` & `clipkit-2.3.0/clipkit/helpers.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/modes.py` & `clipkit-2.3.0/clipkit/modes.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/msa.py` & `clipkit-2.3.0/clipkit/msa.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/parser.py` & `clipkit-2.3.0/clipkit/parser.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/site_classification.py` & `clipkit-2.3.0/clipkit/site_classification.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/smart_gap_helper.py` & `clipkit-2.3.0/clipkit/smart_gap_helper.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/stats.py` & `clipkit-2.3.0/clipkit/stats.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/warnings.py` & `clipkit-2.3.0/clipkit/warnings.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit/write.py` & `clipkit-2.3.0/clipkit/write.py`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/clipkit.egg-info/PKG-INFO` & `clipkit-2.3.0/clipkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: clipkit
-Version: 2.2.6
+Version: 2.3.0
 Summary: Alignment trimming software for phylogenetics.
 Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk
 Author-email: jlsteenwyk@gmail.com
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: biopython>=1.81
+Requires-Dist: biopython>=1.82
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: cython
 
 <p align="center">
   <a href="https://github.com/jlsteenwyk/clipkit">
     <img src="https://raw.githubusercontent.com/JLSteenwyk/ClipKIT/master/docs/_static/img/logo.jpg" alt="Logo" width="400">
   </a>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: clipkit Version: 2.2.6 Summary: Alignment trimming
+Metadata-Version: 2.1 Name: clipkit Version: 2.3.0 Summary: Alignment trimming
 software for phylogenetics. Home-page: https://github.com/jlsteenwyk/clipkit
 Author: Jacob L. Steenwyk Author-email: jlsteenwyk@gmail.com Classifier:
 Operating System :: OS Independent Classifier: Intended Audience :: Science/
 Research Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering Description-Content-Type: text/
-markdown License-File: LICENSE.md Requires-Dist: biopython>=1.81 Requires-Dist:
-numpy>=1.24.0 Requires-Dist: cython
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering Description-Content-Type: text/markdown License-File:
+LICENSE.md Requires-Dist: biopython>=1.82 Requires-Dist: numpy>=1.24.0
+Requires-Dist: cython
                                     _[_L_o_g_o_]
                      _D_o_c_s Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_J_L_S_t_e_e_n_w_y_k_/_C_l_i_p_K_I_T_/
  _c_i_._y_m_l_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_h_/_j_l_s_t_e_e_n_w_y_k_/_c_l_i_p_k_i_t_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/
  _g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_0_J_4_9_I_6_4_4_1_V_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_c_o_n_t_r_i_b_u_t_o_r_s_/
                     _j_l_s_t_e_e_n_w_y_k_/_c_l_i_p_k_i_t_]_[_f_o_l_l_o_w_ _o_n_ _T_w_i_t_t_e_r_]
                  _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_p_e_r_s_o_n_a_l_i_z_e_d_-_b_a_d_g_e_/
```

### Comparing `clipkit-2.2.6/clipkit.egg-info/SOURCES.txt` & `clipkit-2.3.0/clipkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clipkit-2.2.6/setup.py` & `clipkit-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 
 CLASSIFIERS = [
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
 ]
 
-REQUIRES = ["biopython>=1.81", "numpy>=1.24.0", "cython"]
+REQUIRES = ["biopython>=1.82", "numpy>=1.24.0", "cython"]
 
 setup(
     name="clipkit",
     description="Alignment trimming software for phylogenetics.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Jacob L. Steenwyk",
```

