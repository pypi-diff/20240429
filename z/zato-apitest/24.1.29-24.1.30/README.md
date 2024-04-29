# Comparing `tmp/zato_apitest-24.1.29.tar.gz` & `tmp/zato_apitest-24.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zato_apitest-24.1.29.tar", last modified: Mon Apr 29 11:05:43 2024, max compression
+gzip compressed data, was "zato_apitest-24.1.30.tar", last modified: Mon Apr 29 13:16:48 2024, max compression
```

## Comparing `zato_apitest-24.1.29.tar` & `zato_apitest-24.1.30.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.233910 zato_apitest-24.1.29/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.29/LICENSE.txt
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.29/MANIFEST.in
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 11:05:43.233910 zato_apitest-24.1.29/PKG-INFO
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.29/README.md
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.29/requirements.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-29 11:05:43.233910 zato_apitest-24.1.29/setup.cfg
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2663 2024-04-29 11:05:16.000000 zato_apitest-24.1.29/setup.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/zato/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.29/src/zato/__init__.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/zato/apitest/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.29/src/zato/apitest/__init__.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4482 2024-04-28 09:17:32.000000 zato_apitest-24.1.29/src/zato/apitest/cli.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/zato/apitest/console/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.29/src/zato/apitest/console/apitest
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     6434 2024-04-29 09:17:00.000000 zato_apitest-24.1.29/src/zato/apitest/init.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     3116 2024-04-28 13:16:28.000000 zato_apitest-24.1.29/src/zato/apitest/run.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.229910 zato_apitest-24.1.29/src/zato/apitest/steps/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.29/src/zato/apitest/steps/__init__.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    46107 2024-04-29 11:05:12.000000 zato_apitest-24.1.29/src/zato/apitest/steps/common.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.29/src/zato/apitest/steps/json.py
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.29/src/zato/apitest/typing_.py
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)    14680 2024-04-29 09:23:45.000000 zato_apitest-24.1.29/src/zato/apitest/util.py
-drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 11:05:43.233910 zato_apitest-24.1.29/src/zato_apitest.egg-info/
--rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/PKG-INFO
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/SOURCES.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/dependency_links.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/namespace_packages.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 11:05:41.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/not-zip-safe
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/requires.txt
--rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 11:05:43.000000 zato_apitest-24.1.29/src/zato_apitest.egg-info/top_level.txt
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    29450 2024-04-28 07:49:48.000000 zato_apitest-24.1.30/LICENSE.txt
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       24 2019-06-24 21:01:23.000000 zato_apitest-24.1.30/MANIFEST.in
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/PKG-INFO
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)       64 2021-01-13 02:20:20.000000 zato_apitest-24.1.30/README.md
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      375 2024-03-12 11:30:46.000000 zato_apitest-24.1.30/requirements.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)       38 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/setup.cfg
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     2663 2024-04-29 13:16:24.000000 zato_apitest-24.1.30/setup.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.976788 zato_apitest-24.1.30/src/
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      211 2024-04-28 07:50:38.000000 zato_apitest-24.1.30/src/zato/__init__.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato/apitest/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     1800 2024-04-28 07:51:00.000000 zato_apitest-24.1.30/src/zato/apitest/__init__.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     4482 2024-04-28 09:17:32.000000 zato_apitest-24.1.30/src/zato/apitest/cli.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato/apitest/console/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      210 2024-04-28 07:50:47.000000 zato_apitest-24.1.30/src/zato/apitest/console/apitest
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     6434 2024-04-29 09:17:00.000000 zato_apitest-24.1.30/src/zato/apitest/init.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     3116 2024-04-28 13:16:28.000000 zato_apitest-24.1.30/src/zato/apitest/run.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato/apitest/steps/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)      156 2024-04-28 07:50:55.000000 zato_apitest-24.1.30/src/zato/apitest/steps/__init__.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)    48533 2024-04-29 13:13:57.000000 zato_apitest-24.1.30/src/zato/apitest/steps/common.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    22517 2024-04-28 07:50:58.000000 zato_apitest-24.1.30/src/zato/apitest/steps/json.py
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)     7325 2024-04-28 07:50:53.000000 zato_apitest-24.1.30/src/zato/apitest/typing_.py
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)    14680 2024-04-29 09:23:45.000000 zato_apitest-24.1.30/src/zato/apitest/util.py
+drwxrwxr-x   0 dsuch     (1000) dsuch     (1000)        0 2024-04-29 13:16:48.980788 zato_apitest-24.1.30/src/zato_apitest.egg-info/
+-rw-r--r--   0 dsuch     (1000) dsuch     (1000)     2393 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/PKG-INFO
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      654 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/SOURCES.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/dependency_links.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/namespace_packages.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        1 2024-04-29 13:16:46.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/not-zip-safe
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)      356 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/requires.txt
+-rw-rw-r--   0 dsuch     (1000) dsuch     (1000)        5 2024-04-29 13:16:48.000000 zato_apitest-24.1.30/src/zato_apitest.egg-info/top_level.txt
```

### Comparing `zato_apitest-24.1.29/LICENSE.txt` & `zato_apitest-24.1.30/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.29/PKG-INFO` & `zato_apitest-24.1.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.29
+Version: 24.1.30
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
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.29 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.30 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.29/setup.py` & `zato_apitest-24.1.30/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under SSPL 1.0, see LICENSE.txt for terms and conditions.
 """
 
 # stdlib
 import os
 from setuptools import setup, find_packages
 
-version = '24.1.29'
+version = '24.1.30'
 
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
-'24.1.29' LONG_DESCRIPTION = """ Write API tests for your [API integrations]
+'24.1.30' LONG_DESCRIPTION = """ Write API tests for your [API integrations]
 (https://zato.io) in plain English, with no programming needed. Here is how it
 looks like: _!_[_A_P_I_ _t_e_s_t_i_n_g_ _i_n_ _P_y_t_h_o_n_]_(_h_t_t_p_s_:_/_/_u_p_c_d_n_._i_o_/_k_W_1_5_b_q_q_/_r_a_w_/_r_o_o_t_/_e_n_/_d_o_c_s_/
 _3_._2_/_g_f_x_/_a_p_i_-_t_e_s_t_i_n_g_/_d_e_m_o_._w_e_b_p_) More information about API testing: https://
 zato.io/en/docs/3.2/api-testing/index.html """ def parse_requirements
 (requirements): # type: ignore ignored = ['#', 'setuptools', '-e'] with open
 (requirements) as f: return [line for line in f if line.strip() and not any
 (line.startswith(prefix) for prefix in ignored)] setup( name = 'zato-apitest',
```

### Comparing `zato_apitest-24.1.29/src/zato/apitest/__init__.py` & `zato_apitest-24.1.30/src/zato/apitest/__init__.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.29/src/zato/apitest/cli.py` & `zato_apitest-24.1.30/src/zato/apitest/cli.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.29/src/zato/apitest/init.py` & `zato_apitest-24.1.30/src/zato/apitest/init.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.29/src/zato/apitest/run.py` & `zato_apitest-24.1.30/src/zato/apitest/run.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.29/src/zato/apitest/steps/common.py` & `zato_apitest-24.1.30/src/zato/apitest/steps/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     username: 'str'
     password: 'str'
     scopes:   'str'
     grant_type: 'str'
     extra_fields: 'anydict'
     client_id_field: 'str'
     client_secret_field: 'str'
+    request_format: 'str'
     is_json:  'bool'
 
 # ################################################################################################################################
 # ################################################################################################################################
 
 def _get_bearer_token_config(ctx:'Context', is_json:'bool') -> 'BearerTokenConfig':
 
@@ -92,15 +93,15 @@
     config.username = ctx.zato.user_ctx['zato_oauth2_username']
     config.password = ctx.zato.user_ctx['zato_oauth2_password']
     config.scopes = ctx.zato.user_ctx.get('zato_oauth2_scopes', '')
     config.grant_type = ctx.zato.user_ctx.get('zato_oauth2_grant_type', 'password')
     config.extra_fields = _extra_fields
     config.client_id_field = ctx.zato.user_ctx.get('zato_oauth2_client_id_field', 'username')
     config.client_secret_field = ctx.zato.user_ctx.get('zato_oauth2_client_secret_field', 'password')
-    config.is_json = is_json
+    config.is_json = ctx.zato.user_ctx.get('zato_oauth2_request_format', '').lower() == 'json'
 
     # .. and return it to our caller.
     return config
 
 # ################################################################################################################################
 # ################################################################################################################################
 
@@ -239,21 +240,28 @@
             data = json.dumps(ctx.zato.request.data_impl, indent=2)
             ctx.zato.request.headers['Content-Type'] = 'application/json'
 
     ctx.zato.request.method = method
     ctx.zato.request.data = data
     ctx.zato.full_address = '{}{}{}'.format(address, url_path, qs)
 
+    #
+    # Basic Auth
+    #
     auth = None
-
-    # New in 1.1 hence optional
     if ctx.zato.get('auth'):
         if ctx.zato.auth['type'] == Auth.Basic_Auth:
             auth = HTTPBasicAuth(ctx.zato.auth['username'], ctx.zato.auth['password'])
 
+    #
+    # OAuth2 bearer tokens
+    #
+    if current_token := ctx.zato.user_ctx.get('zato_oauth2_current_token'):
+        ctx.zato.request.headers['Authorization'] = f'Bearer {current_token}'
+
     ctx.zato.response = Bunch()
 
     session = req_api.sessions.Session() # type: ignore
 
     for adapter in adapters:
         session.mount('http://', adapter)
         session.mount('https://', adapter)
@@ -558,27 +566,47 @@
 
     # Store for later use
     ctx.zato.user_ctx['zato_oauth2_client_secret_field'] = client_secret_field
 
 # ################################################################################################################################
 # ################################################################################################################################
 
-@given('I store an OAuth2 form bearer token under "{name}"')
+@given('OAuth2 request format "{request_format}"')
+@util.obtain_values
+def oauth2_client_request_format(ctx:'Context', request_format:'str') -> 'None':
+
+    # Store for later use
+    ctx.zato.user_ctx['zato_oauth2_request_format'] = request_format
+
+# ################################################################################################################################
+# ################################################################################################################################
+
+@given('I store an OAuth2 bearer token under "{name}"')
 @util.obtain_values
 def i_store_an_oauth2_form_bearer_token_under(ctx:'Context', name:'str') -> 'None':
 
     # Build the configuration ..
     config = _get_bearer_token_config(ctx, False)
 
     # .. and store the token for later use
     _set_bearer_token_impl(ctx, config, name)
 
 # ################################################################################################################################
 # ################################################################################################################################
 
+@given('OAuth2 bearer token "{token}"')
+@util.obtain_values
+def oauth2_bearer_token(ctx:'Context', token:'str') -> 'None':
+
+    # Indicate that this token will be used in subsequent calls
+    ctx.zato.user_ctx['zato_oauth2_current_token'] = token
+
+# ################################################################################################################################
+# ################################################################################################################################
+
 @given('I store an OAuth2 JSON bearer token under "{name}"')
 @util.obtain_values
 def i_store_an_oauth2_json_bearer_token_under(ctx:'Context', name:'str') -> 'None':
 
     # Build the configuration ..
     config = _get_bearer_token_config(ctx, True)
 
@@ -944,7 +972,35 @@
 @then('variable "{variable}" is any Boolean')
 @util.obtain_values
 def and_variable_is_any_boolean(ctx:'Context', variable:'any_') -> 'None':
     assert isinstance(variable, bool), 'Value `{}` is not a Boolean'.format(variable)
 
 # ################################################################################################################################
 # ################################################################################################################################
+
+@then('context is logged')
+@util.obtain_values
+def and_context_is_logged(ctx:'Context') -> 'None':
+    logger.info('Context: %s' % ctx.zato.user_ctx)
+    logger.info('')
+
+# ################################################################################################################################
+# ################################################################################################################################
+
+@then('OAuth2 context is cleaned up')
+@util.obtain_values
+def then_oauth2_context_is_cleaned_up(ctx:'Context') -> 'None':
+
+    # All the keys we're going to delete
+    to_delete = []
+
+    # .. collect the keys ..
+    for key in ctx.zato.user_ctx:
+        if key.startswith('zato_oauth2_'):
+            to_delete.append(key)
+
+    # .. and delete them all.
+    for item in to_delete:
+        _ = ctx.zato.user_ctx.pop(item, None)
+
+# ################################################################################################################################
+# ################################################################################################################################
```

### Comparing `zato_apitest-24.1.29/src/zato/apitest/steps/json.py` & `zato_apitest-24.1.30/src/zato/apitest/steps/json.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.29/src/zato/apitest/typing_.py` & `zato_apitest-24.1.30/src/zato/apitest/typing_.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.29/src/zato/apitest/util.py` & `zato_apitest-24.1.30/src/zato/apitest/util.py`

 * *Files identical despite different names*

### Comparing `zato_apitest-24.1.29/src/zato_apitest.egg-info/PKG-INFO` & `zato_apitest-24.1.30/src/zato_apitest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zato-apitest
-Version: 24.1.29
+Version: 24.1.30
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
-Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.29 Summary: API Testing
+Metadata-Version: 2.1 Name: zato-apitest Version: 24.1.30 Summary: API Testing
 for Humans. Write API tests in pure English, without any programming needed.
 Home-page: https://zato.io Author: Zato Source s.r.o. Author-email:
 info@zato.io License: Proprietary Platform: OS Independent Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Other Audience Classifier: License :: Other/Proprietary
```

### Comparing `zato_apitest-24.1.29/src/zato_apitest.egg-info/SOURCES.txt` & `zato_apitest-24.1.30/src/zato_apitest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

