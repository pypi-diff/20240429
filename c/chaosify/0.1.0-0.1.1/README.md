# Comparing `tmp/chaosify-0.1.0.tar.gz` & `tmp/chaosify-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chaosify-0.1.0.tar", max compression
+gzip compressed data, was "chaosify-0.1.1.tar", max compression
```

## Comparing `chaosify-0.1.0.tar` & `chaosify-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0    11357 2024-04-26 14:28:53.111011 chaosify-0.1.0/LICENSE
--rw-r--r--   0        0        0     1281 2024-04-26 15:00:33.835363 chaosify-0.1.0/README.md
--rw-r--r--   0        0        0       32 2024-04-26 17:06:47.603117 chaosify-0.1.0/chaosify/__init__.py
--rw-r--r--   0        0        0      295 2024-04-26 15:52:46.407655 chaosify-0.1.0/chaosify/main.py
--rw-r--r--   0        0        0      274 2024-04-26 15:47:43.415368 chaosify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 chaosify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-26 14:28:53.111011 chaosify-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1749 2024-04-29 12:39:46.010400 chaosify-0.1.1/README.md
+-rw-r--r--   0        0        0       60 2024-04-26 21:42:47.116324 chaosify-0.1.1/chaosify/__init__.py
+-rw-r--r--   0        0        0      722 2024-04-26 21:42:47.117137 chaosify-0.1.1/chaosify/check.py
+-rw-r--r--   0        0        0      598 2024-04-26 21:42:47.118198 chaosify-0.1.1/chaosify/main.py
+-rw-r--r--   0        0        0      326 2024-04-29 13:14:44.727274 chaosify-0.1.1/chaosify/wreck.py
+-rw-r--r--   0        0        0      460 2024-04-29 13:00:02.982989 chaosify-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 chaosify-0.1.1/PKG-INFO
```

### Comparing `chaosify-0.1.0/LICENSE` & `chaosify-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chaosify-0.1.0/PKG-INFO` & `chaosify-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: chaosify
-Version: 0.1.0
-Summary: 
-Author: Yuriy Sannikov
-Author-email: yury.sannikov@gmail.com
-Requires-Python: >=3.12,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-
 <p align="center">
   <a href=""><img src="https://github.com/yury-sannikov/chaosify/blob/main/resources/chaos-lib.png?raw=true" alt="Chaosify"></a>
 </p>
 
 <p align="center">
     <em>“In all chaos there is a cosmos, in all disorder a secret order.”</em><br/>
     ― Carl Gustav Jung
@@ -22,16 +11,16 @@
 <p align="center">
     <em>Chaos Testing library to build better, resilient Python applications.</em>
 </p>
 
 
 
 <p align="center">
-<a href="https://github.com/yury-sannikov/chaosify/actions?query=workflow%3ATest+event%3Apush+branch%3Amaster" target="_blank">
-    <img src="https://github.com/yury-sannikov/chaosify/workflows/Test/badge.svg?event=push&branch=master" alt="Test">
+<a href="https://github.com/yury-sannikov/chaosify/actions/workflows/run_coverage.yml" target="_blank">
+    <img src="https://github.com/yury-sannikov/chaosify/actions/workflows/run_coverage.yml/badge.svg" alt="Test">
 </a>
 <a href="https://pypi.org/project/chaosify" target="_blank">
     <img src="https://img.shields.io/pypi/v/chaosify?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://pypi.org/project/chaosify" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/chaosify.svg?color=%2334D058" alt="Supported Python versions">
 </a>
@@ -41,12 +30,17 @@
 
 **Documentation**: <a href="" target="_blank"></a>
 
 **Source Code**: <a href="https://github.com/yury-sannikov/chaosify" target="_blank">https://github.com/yury-sannikov/chaosify</a>
 
 ---
 
-# chaosify
-Chaos Testing library for pyhon
+Chaosify, is a powerful chaos testing library for Python applications. Designed to inject controlled chaos into your code.
 
+Chaosify empowers developers to uncover weaknesses and improve the resilience of their software. Whether you're building microservices, distributed systems, or monolithic applications
 
+Key features are:
+* introduce latency injection
+* emulate resource exhaustion
+* mimic service disruptions
 
+Chaosify is highly configurable, allowing you to fine-tune chaos parameters and observe how your system behaves under stress.
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
-Metadata-Version: 2.1 Name: chaosify Version: 0.1.0 Summary: Author: Yuriy
-Sannikov Author-email: yury.sannikov@gmail.com Requires-Python: >=3.12,<4.0
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.12 Description-Content-Type: text/markdown
                                   [Chaosify]
      ?â??IInn aallll cchhaaooss tthheerree iiss aa ccoossmmooss,, iinn aallll ddiissoorrddeerr aa sseeccrreett oorrddeerr..?â??
                              â Carl Gustav Jung
      CChhaaooss TTeessttiinngg lliibbrraarryy ttoo bbuuiilldd bbeetttteerr,, rreessiilliieenntt PPyytthhoonn aapppplliiccaattiioonnss..
               _[_T_e_s_t_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
 --- **Documentation**: **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_y_u_r_y_-_s_a_n_n_i_k_o_v_/
-_c_h_a_o_s_i_f_y --- # chaosify Chaos Testing library for pyhon
+_c_h_a_o_s_i_f_y --- Chaosify, is a powerful chaos testing library for Python
+applications. Designed to inject controlled chaos into your code. Chaosify
+empowers developers to uncover weaknesses and improve the resilience of their
+software. Whether you're building microservices, distributed systems, or
+monolithic applications Key features are: * introduce latency injection *
+emulate resource exhaustion * mimic service disruptions Chaosify is highly
+configurable, allowing you to fine-tune chaos parameters and observe how your
+system behaves under stress.
```

