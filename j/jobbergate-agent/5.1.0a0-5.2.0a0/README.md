# Comparing `tmp/jobbergate_agent-5.1.0a0.tar.gz` & `tmp/jobbergate_agent-5.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_agent-5.1.0a0.tar", max compression
+gzip compressed data, was "jobbergate_agent-5.2.0a0.tar", max compression
```

## Comparing `jobbergate_agent-5.1.0a0.tar` & `jobbergate_agent-5.2.0a0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1077 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/LICENSE
--rw-r--r--   0        0        0     1346 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/README.md
--rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/clients/__init__.py
--rw-r--r--   0        0        0     3597 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/clients/cluster_api.py
--rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/internals/__init__.py
--rw-r--r--   0        0        0     4305 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/internals/update.py
--rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/__init__.py
--rw-r--r--   0        0        0      150 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/constants.py
--rw-r--r--   0        0        0      636 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/report_health.py
--rw-r--r--   0        0        0     2805 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/schemas.py
--rw-r--r--   0        0        0    11828 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/submit.py
--rw-r--r--   0        0        0     3676 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/update.py
--rw-r--r--   0        0        0      491 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/main.py
--rw-r--r--   0        0        0     2759 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/settings.py
--rw-r--r--   0        0        0     3035 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/tasks.py
--rw-r--r--   0        0        0        0 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/__init__.py
--rw-r--r--   0        0        0     4663 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/exception.py
--rw-r--r--   0        0        0     1440 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/logging.py
--rw-r--r--   0        0        0     1414 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/plugin.py
--rw-r--r--   0        0        0     2153 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/scheduler.py
--rw-r--r--   0        0        0      730 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/sentry.py
--rw-r--r--   0        0        0     2500 2024-04-19 17:22:06.550111 jobbergate_agent-5.1.0a0/jobbergate_agent/utils/user_mapper.py
--rw-r--r--   0        0        0     3295 2024-04-19 17:22:06.554111 jobbergate_agent-5.1.0a0/pyproject.toml
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/LICENSE
+-rw-r--r--   0        0        0     1346 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/clients/__init__.py
+-rw-r--r--   0        0        0     3597 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/clients/cluster_api.py
+-rw-r--r--   0        0        0        0 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/internals/__init__.py
+-rw-r--r--   0        0        0     4305 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/internals/update.py
+-rw-r--r--   0        0        0        0 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/constants.py
+-rw-r--r--   0        0        0      636 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/report_health.py
+-rw-r--r--   0        0        0     2805 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/schemas.py
+-rw-r--r--   0        0        0    11828 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/submit.py
+-rw-r--r--   0        0        0     3676 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/update.py
+-rw-r--r--   0        0        0      491 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/main.py
+-rw-r--r--   0        0        0     2759 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/settings.py
+-rw-r--r--   0        0        0     3035 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/tasks.py
+-rw-r--r--   0        0        0        0 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/utils/__init__.py
+-rw-r--r--   0        0        0     4663 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/utils/exception.py
+-rw-r--r--   0        0        0     1440 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/utils/logging.py
+-rw-r--r--   0        0        0     1414 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/utils/plugin.py
+-rw-r--r--   0        0        0     2153 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/utils/scheduler.py
+-rw-r--r--   0        0        0      730 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/utils/sentry.py
+-rw-r--r--   0        0        0     2500 2024-04-29 20:17:26.782340 jobbergate_agent-5.2.0a0/jobbergate_agent/utils/user_mapper.py
+-rw-r--r--   0        0        0     3295 2024-04-29 20:17:26.786340 jobbergate_agent-5.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 jobbergate_agent-5.2.0a0/PKG-INFO
```

### Comparing `jobbergate_agent-5.1.0a0/LICENSE` & `jobbergate_agent-5.2.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/README.md` & `jobbergate_agent-5.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/clients/cluster_api.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/clients/cluster_api.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/internals/update.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/internals/update.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/report_health.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/report_health.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/schemas.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/submit.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/submit.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/jobbergate/update.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/jobbergate/update.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/settings.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/settings.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/tasks.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/tasks.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/exception.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/utils/exception.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/logging.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/utils/logging.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/plugin.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/utils/plugin.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/scheduler.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/sentry.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/utils/sentry.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/jobbergate_agent/utils/user_mapper.py` & `jobbergate_agent-5.2.0a0/jobbergate_agent/utils/user_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_agent-5.1.0a0/pyproject.toml` & `jobbergate_agent-5.2.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-agent"
-version = "5.1.0a0"
+version = "5.2.0a0"
 description = "Jobbergate Agent"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_agent-5.1.0a0/PKG-INFO` & `jobbergate_agent-5.2.0a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-agent
-Version: 5.1.0a0
+Version: 5.2.0a0
 Summary: Jobbergate Agent
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: apscheduler (==3.10.3)
 Requires-Dist: auto-name-enum (>=2.0.0,<3.0.0)
 Requires-Dist: httpx (==0.24.1)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0) ; python_version < "3.10"
-Requires-Dist: jobbergate-core (==5.1.0a0)
+Requires-Dist: jobbergate-core (==5.2.0a0)
 Requires-Dist: loguru (==0.6.0)
 Requires-Dist: py-buzz (>=4.0.0,<5.0.0)
 Requires-Dist: pydantic (==1.10.12)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-jose (==3.3.0)
 Requires-Dist: sentry-sdk (>=1.1.0,<2.0.0)
```

