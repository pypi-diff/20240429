# Comparing `tmp/edgegap_settings-0.1.0.tar.gz` & `tmp/edgegap_settings-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_settings-0.1.0.tar", max compression
+gzip compressed data, was "edgegap_settings-1.0.0.tar", max compression
```

## Comparing `edgegap_settings-0.1.0.tar` & `edgegap_settings-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1993 2024-04-29 14:01:56.389766 edgegap_settings-0.1.0/LICENSE
--rw-r--r--   0        0        0     2182 2024-04-29 14:44:44.642105 edgegap_settings-0.1.0/README.md
--rw-r--r--   0        0        0      358 2024-04-25 13:10:38.957084 edgegap_settings-0.1.0/edgegap_settings/__init__.py
--rw-r--r--   0        0        0      531 2024-04-25 13:10:38.957169 edgegap_settings-0.1.0/edgegap_settings/_apm.py
--rw-r--r--   0        0        0      872 2024-04-25 13:10:38.957258 edgegap_settings-0.1.0/edgegap_settings/_base.py
--rw-r--r--   0        0        0      119 2024-04-25 13:10:38.957346 edgegap_settings-0.1.0/edgegap_settings/_configuration.py
--rw-r--r--   0        0        0     3016 2024-04-29 14:58:02.095530 edgegap_settings-0.1.0/edgegap_settings/_factory.py
--rw-r--r--   0        0        0      963 2024-04-25 13:10:38.957514 edgegap_settings-0.1.0/edgegap_settings/_fields.py
--rw-r--r--   0        0        0      427 2024-04-25 13:10:38.957717 edgegap_settings-0.1.0/edgegap_settings/_logstash.py
--rw-r--r--   0        0        0      567 2024-04-29 14:57:48.337022 edgegap_settings-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2976 1970-01-01 00:00:00.000000 edgegap_settings-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2182 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/README.md
+-rw-r--r--   0        0        0      358 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/edgegap_settings/__init__.py
+-rw-r--r--   0        0        0      531 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/edgegap_settings/_apm.py
+-rw-r--r--   0        0        0      872 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/edgegap_settings/_base.py
+-rw-r--r--   0        0        0      119 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/edgegap_settings/_configuration.py
+-rw-r--r--   0        0        0     3016 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/edgegap_settings/_factory.py
+-rw-r--r--   0        0        0      963 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/edgegap_settings/_fields.py
+-rw-r--r--   0        0        0      427 2024-04-29 18:13:42.714660 edgegap_settings-1.0.0/edgegap_settings/_logstash.py
+-rw-r--r--   0        0        0      567 2024-04-29 18:13:54.930725 edgegap_settings-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2925 1970-01-01 00:00:00.000000 edgegap_settings-1.0.0/PKG-INFO
```

### Comparing `edgegap_settings-0.1.0/LICENSE` & `edgegap_settings-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_settings-0.1.0/README.md` & `edgegap_settings-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_settings-0.1.0/edgegap_settings/_apm.py` & `edgegap_settings-1.0.0/edgegap_settings/_apm.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-0.1.0/edgegap_settings/_base.py` & `edgegap_settings-1.0.0/edgegap_settings/_base.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-0.1.0/edgegap_settings/_factory.py` & `edgegap_settings-1.0.0/edgegap_settings/_factory.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-0.1.0/edgegap_settings/_fields.py` & `edgegap_settings-1.0.0/edgegap_settings/_fields.py`

 * *Files identical despite different names*

### Comparing `edgegap_settings-0.1.0/pyproject.toml` & `edgegap_settings-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-settings"
-version = "0.1.0"
+version = "1.0.0"
 description = "The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic-settings = "^2.2.1"
```

### Comparing `edgegap_settings-0.1.0/PKG-INFO` & `edgegap_settings-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: edgegap-settings
-Version: 0.1.0
+Version: 1.0.0
 Summary: The Edgegap Settings library includes various tools and helpers for interacting with Explicit Settings Models. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: edgegap-consul (>=0.1.0,<0.2.0)
 Requires-Dist: edgegap-logging (>=0.1.0,<0.2.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
```

