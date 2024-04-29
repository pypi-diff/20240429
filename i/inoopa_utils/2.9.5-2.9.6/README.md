# Comparing `tmp/inoopa_utils-2.9.5.tar.gz` & `tmp/inoopa_utils-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inoopa_utils-2.9.5.tar", max compression
+gzip compressed data, was "inoopa_utils-2.9.6.tar", max compression
```

## Comparing `inoopa_utils-2.9.5.tar` & `inoopa_utils-2.9.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      953 2024-03-11 12:17:35.204315 inoopa_utils-2.9.5/README.md
--rw-r--r--   0        0        0        0 2024-04-22 08:46:46.594963 inoopa_utils-2.9.5/inoopa_utils/__init__.py
--rw-r--r--   0        0        0     1781 2024-03-08 11:42:35.645264 inoopa_utils-2.9.5/inoopa_utils/address_parser.py
--rw-r--r--   0        0        0     6238 2024-03-08 11:42:34.540729 inoopa_utils-2.9.5/inoopa_utils/batch_processing.py
--rw-r--r--   0        0        0        0 2024-03-08 11:43:03.997156 inoopa_utils-2.9.5/inoopa_utils/custom_types/__init__.py
--rw-r--r--   0        0        0     9136 2024-03-08 11:43:05.631896 inoopa_utils-2.9.5/inoopa_utils/custom_types/companies.py
--rw-r--r--   0        0        0      801 2024-03-08 11:43:06.928124 inoopa_utils-2.9.5/inoopa_utils/custom_types/decision_makers.py
--rw-r--r--   0        0        0      117 2024-03-08 11:43:11.918631 inoopa_utils-2.9.5/inoopa_utils/custom_types/exceptions.py
--rw-r--r--   0        0        0     2352 2024-04-26 10:34:01.198648 inoopa_utils-2.9.5/inoopa_utils/custom_types/typesense_schemas.py
--rw-r--r--   0        0        0      358 2024-03-08 11:43:09.416778 inoopa_utils-2.9.5/inoopa_utils/custom_types/websites.py
--rw-r--r--   0        0        0     1720 2024-03-08 11:42:33.437130 inoopa_utils-2.9.5/inoopa_utils/inoopa_logging.py
--rw-r--r--   0        0        0    16195 2024-03-08 11:42:26.507548 inoopa_utils-2.9.5/inoopa_utils/mongodb_helpers.py
--rw-r--r--   0        0        0     3207 2024-03-27 14:28:43.391739 inoopa_utils-2.9.5/inoopa_utils/openai_helpers.py
--rw-r--r--   0        0        0     4243 2024-03-08 11:42:32.029627 inoopa_utils-2.9.5/inoopa_utils/rabbitmq_helpers.py
--rw-r--r--   0        0        0     4871 2024-03-08 11:42:30.821464 inoopa_utils-2.9.5/inoopa_utils/sql_helpers.py
--rw-r--r--   0        0        0      427 2023-11-06 09:54:38.711474 inoopa_utils-2.9.5/inoopa_utils/tests/test_logging.py
--rw-r--r--   0        0        0      627 2023-11-06 12:56:31.343962 inoopa_utils-2.9.5/inoopa_utils/tests/test_rabbitmq.py
--rw-r--r--   0        0        0    11383 2024-04-26 10:43:04.588471 inoopa_utils-2.9.5/inoopa_utils/typesense_helpers.py
--rw-r--r--   0        0        0        0 2023-11-06 00:28:42.240779 inoopa_utils-2.9.5/inoopa_utils/utils/__init__.py
--rw-r--r--   0        0        0      368 2024-03-08 11:43:44.438533 inoopa_utils-2.9.5/inoopa_utils/utils/env_variables_helper.py
--rw-r--r--   0        0        0      144 2024-03-08 11:43:22.052184 inoopa_utils-2.9.5/inoopa_utils/utils/exceptions.py
--rw-r--r--   0        0        0      662 2024-04-26 10:43:18.043402 inoopa_utils-2.9.5/pyproject.toml
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 inoopa_utils-2.9.5/PKG-INFO
+-rw-r--r--   0        0        0      953 2024-03-11 12:17:35.204315 inoopa_utils-2.9.6/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 08:46:46.594963 inoopa_utils-2.9.6/inoopa_utils/__init__.py
+-rw-r--r--   0        0        0     1781 2024-03-08 11:42:35.645264 inoopa_utils-2.9.6/inoopa_utils/address_parser.py
+-rw-r--r--   0        0        0     6238 2024-03-08 11:42:34.540729 inoopa_utils-2.9.6/inoopa_utils/batch_processing.py
+-rw-r--r--   0        0        0        0 2024-03-08 11:43:03.997156 inoopa_utils-2.9.6/inoopa_utils/custom_types/__init__.py
+-rw-r--r--   0        0        0     9103 2024-04-29 14:08:17.458618 inoopa_utils-2.9.6/inoopa_utils/custom_types/companies.py
+-rw-r--r--   0        0        0      801 2024-03-08 11:43:06.928124 inoopa_utils-2.9.6/inoopa_utils/custom_types/decision_makers.py
+-rw-r--r--   0        0        0      117 2024-03-08 11:43:11.918631 inoopa_utils-2.9.6/inoopa_utils/custom_types/exceptions.py
+-rw-r--r--   0        0        0     2352 2024-04-26 10:34:01.198648 inoopa_utils-2.9.6/inoopa_utils/custom_types/typesense_schemas.py
+-rw-r--r--   0        0        0      358 2024-03-08 11:43:09.416778 inoopa_utils-2.9.6/inoopa_utils/custom_types/websites.py
+-rw-r--r--   0        0        0     1720 2024-03-08 11:42:33.437130 inoopa_utils-2.9.6/inoopa_utils/inoopa_logging.py
+-rw-r--r--   0        0        0    16195 2024-03-08 11:42:26.507548 inoopa_utils-2.9.6/inoopa_utils/mongodb_helpers.py
+-rw-r--r--   0        0        0     3207 2024-03-27 14:28:43.391739 inoopa_utils-2.9.6/inoopa_utils/openai_helpers.py
+-rw-r--r--   0        0        0     4243 2024-03-08 11:42:32.029627 inoopa_utils-2.9.6/inoopa_utils/rabbitmq_helpers.py
+-rw-r--r--   0        0        0     4871 2024-03-08 11:42:30.821464 inoopa_utils-2.9.6/inoopa_utils/sql_helpers.py
+-rw-r--r--   0        0        0      427 2023-11-06 09:54:38.711474 inoopa_utils-2.9.6/inoopa_utils/tests/test_logging.py
+-rw-r--r--   0        0        0      627 2023-11-06 12:56:31.343962 inoopa_utils-2.9.6/inoopa_utils/tests/test_rabbitmq.py
+-rw-r--r--   0        0        0    11383 2024-04-26 10:43:04.588471 inoopa_utils-2.9.6/inoopa_utils/typesense_helpers.py
+-rw-r--r--   0        0        0        0 2023-11-06 00:28:42.240779 inoopa_utils-2.9.6/inoopa_utils/utils/__init__.py
+-rw-r--r--   0        0        0      368 2024-03-08 11:43:44.438533 inoopa_utils-2.9.6/inoopa_utils/utils/env_variables_helper.py
+-rw-r--r--   0        0        0      144 2024-03-08 11:43:22.052184 inoopa_utils-2.9.6/inoopa_utils/utils/exceptions.py
+-rw-r--r--   0        0        0      662 2024-04-29 14:09:05.836007 inoopa_utils-2.9.6/pyproject.toml
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 inoopa_utils-2.9.6/PKG-INFO
```

### Comparing `inoopa_utils-2.9.5/README.md` & `inoopa_utils-2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/address_parser.py` & `inoopa_utils-2.9.6/inoopa_utils/address_parser.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/batch_processing.py` & `inoopa_utils-2.9.6/inoopa_utils/batch_processing.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/custom_types/companies.py` & `inoopa_utils-2.9.6/inoopa_utils/custom_types/companies.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         status=company_dict.get('status'),
         start_date=company_dict.get('start_date'),
         entity_type=company_dict.get('entity_type'),
         legal_form=company_dict.get('legal_form'),
         legal_form_last_update=company_dict.get('legal_form_last_update'),
         legal_situation=company_dict.get('legal_situation'),
         legal_situation_last_update=company_dict.get('legal_situation_last_update'),
-        address=Address(**company_dict['address']) if company_dict and "source" in company_dict.get('address', {}) else None,
+        address=Address(**company_dict['address']) if company_dict.get("address") else None,
         best_email=company_dict.get('best_email'),
         emails=[Email(**email) for email in company_dict.get('emails', []) or []],
         best_phone=company_dict.get('best_phone'),
         phones=[Phone(**phone) for phone in company_dict.get('phones', []) or []],
         best_website=company_dict.get('best_website'),
         websites=[Website(**website)for website in company_dict.get('websites', []) or []],
         last_website_finding_date=company_dict.get('best_website'),
```

### Comparing `inoopa_utils-2.9.5/inoopa_utils/custom_types/decision_makers.py` & `inoopa_utils-2.9.6/inoopa_utils/custom_types/decision_makers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/custom_types/typesense_schemas.py` & `inoopa_utils-2.9.6/inoopa_utils/custom_types/typesense_schemas.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/inoopa_logging.py` & `inoopa_utils-2.9.6/inoopa_utils/inoopa_logging.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/mongodb_helpers.py` & `inoopa_utils-2.9.6/inoopa_utils/mongodb_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/openai_helpers.py` & `inoopa_utils-2.9.6/inoopa_utils/openai_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/rabbitmq_helpers.py` & `inoopa_utils-2.9.6/inoopa_utils/rabbitmq_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/sql_helpers.py` & `inoopa_utils-2.9.6/inoopa_utils/sql_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/tests/test_rabbitmq.py` & `inoopa_utils-2.9.6/inoopa_utils/tests/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/inoopa_utils/typesense_helpers.py` & `inoopa_utils-2.9.6/inoopa_utils/typesense_helpers.py`

 * *Files identical despite different names*

### Comparing `inoopa_utils-2.9.5/pyproject.toml` & `inoopa_utils-2.9.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "inoopa_utils"
 description = "Collection of utils used at Inoopa."
-version = "2.9.5"
+version = "2.9.6"
 authors = ["Dev Inoopa <dev@inoopa.com>"]
 packages = [{ include = "inoopa_utils" }]
 repository = "https://bitbucket.org/inoopa/inoopa_utils/"
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `inoopa_utils-2.9.5/PKG-INFO` & `inoopa_utils-2.9.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inoopa_utils
-Version: 2.9.5
+Version: 2.9.6
 Summary: Collection of utils used at Inoopa.
 Home-page: https://bitbucket.org/inoopa/inoopa_utils/
 Author: Dev Inoopa
 Author-email: dev@inoopa.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

