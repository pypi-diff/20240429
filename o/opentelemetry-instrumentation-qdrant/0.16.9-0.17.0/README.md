# Comparing `tmp/opentelemetry_instrumentation_qdrant-0.16.9.tar.gz` & `tmp/opentelemetry_instrumentation_qdrant-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.16.9.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_qdrant-0.17.0.tar", max compression
```

## Comparing `opentelemetry_instrumentation_qdrant-0.16.9.tar` & `opentelemetry_instrumentation_qdrant-0.17.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      572 2024-04-26 20:44:31.814903 opentelemetry_instrumentation_qdrant-0.16.9/README.md
--rw-r--r--   0        0        0     2114 2024-04-26 20:44:31.814903 opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     2943 2024-04-26 20:44:31.814903 opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
--rw-r--r--   0        0        0       42 2024-04-26 20:44:31.814903 opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/config.py
--rw-r--r--   0        0        0     2828 2024-04-26 20:44:31.814903 opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
--rw-r--r--   0        0        0      699 2024-04-26 20:44:31.814903 opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/utils.py
--rw-r--r--   0        0        0       23 2024-04-26 20:44:31.814903 opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/version.py
--rw-r--r--   0        0        0     3783 2024-04-26 20:44:31.814903 opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/wrapper.py
--rw-r--r--   0        0        0     1352 2024-04-26 20:44:56.439022 opentelemetry_instrumentation_qdrant-0.16.9/pyproject.toml
--rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.16.9/PKG-INFO
+-rw-r--r--   0        0        0      572 2024-04-29 13:32:45.474768 opentelemetry_instrumentation_qdrant-0.17.0/README.md
+-rw-r--r--   0        0        0     2114 2024-04-29 13:32:45.474768 opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     2943 2024-04-29 13:32:45.474768 opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json
+-rw-r--r--   0        0        0       42 2024-04-29 13:32:45.474768 opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/config.py
+-rw-r--r--   0        0        0     2828 2024-04-29 13:32:45.474768 opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json
+-rw-r--r--   0        0        0      699 2024-04-29 13:32:45.474768 opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/utils.py
+-rw-r--r--   0        0        0       23 2024-04-29 13:32:45.474768 opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/version.py
+-rw-r--r--   0        0        0     3783 2024-04-29 13:32:45.474768 opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/wrapper.py
+-rw-r--r--   0        0        0     1352 2024-04-29 13:33:10.286658 opentelemetry_instrumentation_qdrant-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     1655 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_qdrant-0.17.0/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_qdrant-0.16.9/README.md` & `opentelemetry_instrumentation_qdrant-0.17.0/README.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/__init__.py` & `opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/async_qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json` & `opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/qdrant_client_methods.json`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/utils.py` & `opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/utils.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.9/opentelemetry/instrumentation/qdrant/wrapper.py` & `opentelemetry_instrumentation_qdrant-0.17.0/opentelemetry/instrumentation/qdrant/wrapper.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrumentation_qdrant-0.16.9/pyproject.toml` & `opentelemetry_instrumentation_qdrant-0.17.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.coverage.report]
 exclude_lines = [ "if TYPE_CHECKING:" ]
 show_missing = true
 
 [tool.poetry]
 name = "opentelemetry-instrumentation-qdrant"
-version = "0.16.9"
+version = "0.17.0"
 description = "OpenTelemetry Qdrant instrumentation"
 authors = [
   "Gal Kleinman <gal@traceloop.com>",
   "Nir Gazit <nir@traceloop.com>",
   "Tomer Friedman <tomer@traceloop.com>"
 ]
 repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant"
@@ -23,15 +23,15 @@
 include = "opentelemetry/instrumentation/qdrant"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 opentelemetry-api = "^1.24.0"
 opentelemetry-instrumentation = "^0.45b0"
 opentelemetry-semantic-conventions = "^0.45b0"
-opentelemetry-semantic-conventions-ai = "0.1.1"
+opentelemetry-semantic-conventions-ai = "0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "2.1.0"
 flake8 = "7.0.0"
 
 [tool.poetry.group.test.dependencies]
 qdrant-client = "^1.7.3"
```

### Comparing `opentelemetry_instrumentation_qdrant-0.16.9/PKG-INFO` & `opentelemetry_instrumentation_qdrant-0.17.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-qdrant
-Version: 0.16.9
+Version: 0.17.0
 Summary: OpenTelemetry Qdrant instrumentation
 Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant
 License: Apache-2.0
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: instruments
 Requires-Dist: opentelemetry-api (>=1.24.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation (>=0.45b0,<0.46)
 Requires-Dist: opentelemetry-semantic-conventions (>=0.45b0,<0.46)
-Requires-Dist: opentelemetry-semantic-conventions-ai (==0.1.1)
+Requires-Dist: opentelemetry-semantic-conventions-ai (==0.2.0)
 Project-URL: Repository, https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant
 Description-Content-Type: text/markdown
 
 # OpenTelemetry Qdrant Instrumentation
 
 <a href="https://pypi.org/project/opentelemetry-instrumentation-qdrant/">
     <img src="https://badge.fury.io/py/opentelemetry-instrumentation-qdrant.svg">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1 Name: opentelemetry-instrumentation-qdrant Version:
-0.16.9 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
+0.17.0 Summary: OpenTelemetry Qdrant instrumentation Home-page: https://
 github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-
 instrumentation-qdrant License: Apache-2.0 Author: Gal Kleinman Author-email:
 gal@traceloop.com Requires-Python: >=3.9,<4 Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: instruments
 Requires-Dist: opentelemetry-api (>=1.24.0,<2.0.0) Requires-Dist:
 opentelemetry-instrumentation (>=0.45b0,<0.46) Requires-Dist: opentelemetry-
 semantic-conventions (>=0.45b0,<0.46) Requires-Dist: opentelemetry-semantic-
-conventions-ai (==0.1.1) Project-URL: Repository, https://github.com/traceloop/
+conventions-ai (==0.2.0) Project-URL: Repository, https://github.com/traceloop/
 openllmetry/tree/main/packages/opentelemetry-instrumentation-qdrant
 Description-Content-Type: text/markdown # OpenTelemetry Qdrant Instrumentation
 _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_o_p_e_n_t_e_l_e_m_e_t_r_y_-_i_n_s_t_r_u_m_e_n_t_a_t_i_o_n_-_q_d_r_a_n_t_._s_v_g_]This library
 allows tracing client-side calls to Qdrant vector DB sent with the official
 [Qdrant client library](https://github.com/qdrant/qdrant-client). ##
 Installation ```bash pip install opentelemetry-instrumentation-qdrant ``` ##
 Example usage ```python from opentelemetry.instrumentation.qdrant import
```
