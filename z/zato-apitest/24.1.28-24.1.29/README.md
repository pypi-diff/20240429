# Comparing `tmp/zato_apitest-24.1.28.tar.gz` & `tmp/zato_apitest-24.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zato_apitest-24.1.28.tar", last modified: Mon Apr 29 11:00:40 2024, max compression
+gzip compressed data, was "zato_apitest-24.1.29.tar", last modified: Mon Apr 29 11:05:43 2024, max compression
```

## Comparing `zato_apitest-24.1.28.tar` & `zato_apitest-24.1.29.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:00:40.980832 zato_apitest-24.1.28/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.28/LICENSE.txt
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.28/MANIFEST.in
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 11:00:40.980832 zato_apitest-24.1.28/PKG-INFO
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.28/README.md
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.28/requirements.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-29 11:00:40.980832 zato_apitest-24.1.28/setup.cfg
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2663 2024-04-29 11:00:15.000000 zato_apitest-24.1.28/setup.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:00:40.972832 zato_apitest-24.1.28/src/
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:00:40.976832 zato_apitest-24.1.28/src/zato/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.28/src/zato/__init__.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:00:40.976832 zato_apitest-24.1.28/src/zato/apitest/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.28/src/zato/apitest/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4482 2024-04-28 09:17:32.000000 zato_apitest-24.1.28/src/zato/apitest/cli.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:00:40.976832 zato_apitest-24.1.28/src/zato/apitest/console/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.28/src/zato/apitest/console/apitest
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     6434 2024-04-29 09:17:00.000000 zato_apitest-24.1.28/src/zato/apitest/init.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     3116 2024-04-28 13:16:28.000000 zato_apitest-24.1.28/src/zato/apitest/run.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:00:40.976832 zato_apitest-24.1.28/src/zato/apitest/steps/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.28/src/zato/apitest/steps/__init__.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    46074 2024-04-29 10:59:48.000000 zato_apitest-24.1.28/src/zato/apitest/steps/common.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.28/src/zato/apitest/steps/json.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.28/src/zato/apitest/typing_.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    14680 2024-04-29 09:23:45.000000 zato_apitest-24.1.28/src/zato/apitest/util.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:00:40.976832 zato_apitest-24.1.28/src/zato_apitest.egg-info/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 11:00:40.000000 zato_apitest-24.1.28/src/zato_apitest.egg-info/PKG-INFO
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-29 11:00:40.000000 zato_apitest-24.1.28/src/zato_apitest.egg-info/SOURCES.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 11:00:40.000000 zato_apitest-24.1.28/src/zato_apitest.egg-info/dependency_links.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 11:00:40.000000 zato_apitest-24.1.28/src/zato_apitest.egg-info/namespace_packages.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 11:00:38.000000 zato_apitest-24.1.28/src/zato_apitest.egg-info/not-zip-safe
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-29 11:00:40.000000 zato_apitest-24.1.28/src/zato_apitest.egg-info/requires.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 11:00:40.000000 zato_apitest-24.1.28/src/zato_apitest.egg-info/top_level.txt
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.233910 zato_apitest-24.1.29/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.29/LICENSE.txt
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.29/MANIFEST.in
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 11:05:43.233910 zato_apitest-24.1.29/PKG-INFO
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.29/README.md
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.29/requirements.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-29 11:05:43.233910 zato_apitest-24.1.29/setup.cfg
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2663 2024-04-29 11:05:16.000000 zato_apitest-24.1.29/setup.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/zato/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.29/src/zato/__init__.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/zato/apitest/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.29/src/zato/apitest/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4482 2024-04-28 09:17:32.000000 zato_apitest-24.1.29/src/zato/apitest/cli.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/zato/apitest/console/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.29/src/zato/apitest/console/apitest
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     6434 2024-04-29 09:17:00.000000 zato_apitest-24.1.29/src/zato/apitest/init.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     3116 2024-04-28 13:16:28.000000 zato_apitest-24.1.29/src/zato/apitest/run.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/zato/apitest/steps/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.29/src/zato/apitest/steps/__init__.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    46107 2024-04-29 11:05:12.000000 zato_apitest-24.1.29/src/zato/apitest/steps/common.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.29/src/zato/apitest/steps/json.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.29/src/zato/apitest/typing_.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    14680 2024-04-29 09:23:45.000000 zato_apitest-24.1.29/src/zato/apitest/util.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.233910 zato_apitest-24.1.29/src/zato_apitest.egg-info/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/PKG-INFO
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/namespace_packages.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 11:05:41.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/not-zip-safe
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/requires.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/top_level.txt
```

### Comparing `zato_apitest-24.1.28/LICENSE.txt` & `zato_apitest-24.1.29/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.28/PKG-INFO` & `zato_apitest-24.1.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.28
+Version: 24.1.29
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
 License: Proprietary
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.28 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.29 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.28/setup.py` & `zato_apitest-24.1.29/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
 """
 
 # stdlib
 import os
 from setuptools import setup, find_packages
 
-version = '24.1.28'
+version = '24.1.29'
 
 LONG_DESCRIPTION = """
 
 Write API tests for your [API integrations](https://zato.io) in plain English, with no programming needed.
 
 Here is how it looks like:
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- """ Copyright (C) 2024, Zato Source s.r.o. https://
 zato.io Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions. """
 # stdlib import os from setuptools import setup, find_packages version =
-'24.1.28' LONG_DESCRIPTION = """ Write API tests for your [API integrations]
+'24.1.29' LONG_DESCRIPTION = """ Write API tests for your [API integrations]
 (https://zato.io) in plain English, with no programming needed. Here is how it
 looks like: _!_[_A_P_I_ _t_e_s_t_i_n_g_ _i_n_ _P_y_t_h_o_n_]_(_h_t_t_p_s_:_/_/_u_p_c_d_n_._i_o_/_k_W_1_5_b_q_q_/_r_a_w_/_r_o_o_t_/_e_n_/_d_o_c_s_/
 _3_._2_/_g_f_x_/_a_p_i_-_t_e_s_t_i_n_g_/_d_e_m_o_._w_e_b_p_) More information about API testing: https://
 zato.io/en/docs/3.2/api-testing/index.html """ def parse_requirements
 (requirements): # type: ignore ignored = ['#', 'setuptools', '-e'] with open
 (requirements) as f: return [line for line in f if line.strip() and not any
 (line.startswith(prefix) for prefix in ignored)] setup( name = 'zato-apitest',
```

### Comparing `zato_apitest-24.1.28/src/zato/apitest/__init__.py` & `zato_apitest-24.1.29/src/zato/apitest/__init__.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.28/src/zato/apitest/cli.py` & `zato_apitest-24.1.29/src/zato/apitest/cli.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.28/src/zato/apitest/init.py` & `zato_apitest-24.1.29/src/zato/apitest/init.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.28/src/zato/apitest/run.py` & `zato_apitest-24.1.29/src/zato/apitest/run.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.28/src/zato/apitest/steps/common.py` & `zato_apitest-24.1.29/src/zato/apitest/steps/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,18 +76,19 @@
 
     # Extract extra fields
     _extra_fields = {}
     extra_fields = ctx.zato.user_ctx.get('zato_oauth2_extra_fields', '')
     extra_fields = [elem.strip() for elem in extra_fields.split(',')]
 
     for elem in extra_fields:
-        key, value = elem.split('=')
-        key = key.strip()
-        value = value.strip()
-        _extra_fields[key] = value
+        if elem:
+            key, value = elem.split('=')
+            key = key.strip()
+            value = value.strip()
+            _extra_fields[key] = value
 
     # .. build the configuration ..
     config = BearerTokenConfig()
     config.address = ctx.zato.user_ctx['zato_oauth2_address']
     config.username = ctx.zato.user_ctx['zato_oauth2_username']
     config.password = ctx.zato.user_ctx['zato_oauth2_password']
     config.scopes = ctx.zato.user_ctx.get('zato_oauth2_scopes', '')
```

### Comparing `zato_apitest-24.1.28/src/zato/apitest/steps/json.py` & `zato_apitest-24.1.29/src/zato/apitest/steps/json.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.28/src/zato/apitest/typing_.py` & `zato_apitest-24.1.29/src/zato/apitest/typing_.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.28/src/zato/apitest/util.py` & `zato_apitest-24.1.29/src/zato/apitest/util.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.28/src/zato_apitest.egg-info/PKG-INFO` & `zato_apitest-24.1.29/src/zato_apitest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.28
+Version: 24.1.29
 Summary: API Testing for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io
 Author: Zato Source s.r.o.
 Author-email: info@zato.io
 License: Proprietary
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.28 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.29 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.28/src/zato_apitest.egg-info/SOURCES.txt` & `zato_apitest-24.1.29/src/zato_apitest.egg-info/SOURCES.txt`

 * *Files identical despite different names*
