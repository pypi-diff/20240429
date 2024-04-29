# Comparing `tmp/close_dot_io-0.0.913.tar.gz` & `tmp/close_dot_io-0.0.914.tar.gz`

## Comparing `close_dot_io-0.0.913.tar` & `close_dot_io-0.0.914.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/.pre-commit-config.yaml
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/requirements-dev.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/__about__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/__init__.py
--rw-r--r--   0        0        0    13491 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/client.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/dict_util.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/enums.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/security.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/__init__.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/activity.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/base.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/connected_account.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/contact.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/event.py
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/lead.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/opportunity.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/sequence.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/smart_view.py
--rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/src/close_dot_io/resources/webhook.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/tests/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/.gitignore
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/LICENSE.txt
--rw-r--r--   0        0        0    16966 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/README.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/pyproject.toml
--rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 close_dot_io-0.0.913/PKG-INFO
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/requirements-dev.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/__about__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/__init__.py
+-rw-r--r--   0        0        0    13491 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/client.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/dict_util.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/enums.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/security.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/__init__.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/activity.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/base.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/connected_account.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/contact.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/event.py
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/lead.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/opportunity.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/sequence.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/smart_view.py
+-rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/src/close_dot_io/resources/webhook.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/tests/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/.gitignore
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/LICENSE.txt
+-rw-r--r--   0        0        0    16966 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/README.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/pyproject.toml
+-rw-r--r--   0        0        0    18047 2020-02-02 00:00:00.000000 close_dot_io-0.0.914/PKG-INFO
```

### Comparing `close_dot_io-0.0.913/.pre-commit-config.yaml` & `close_dot_io-0.0.914/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/client.py` & `close_dot_io-0.0.914/src/close_dot_io/client.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/enums.py` & `close_dot_io-0.0.914/src/close_dot_io/enums.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/__init__.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/activity.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/activity.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/base.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/base.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/contact.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/contact.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class ContactPhoneNumber(BaseModel):
     country: CountryAlpha2 | None = "US"
     phone: str
     type: ContactEmailOrPhoneTypeEnum = ContactEmailOrPhoneTypeEnum.OFFICE
 
 
 class Contact(BaseResourceModel):
+    lead_id: str | None = None
     name: str | None = None
     title: str | None = None
     phones: list[ContactPhoneNumber] = []
     emails: list[ContactEmailAddress] = []
 
     @classmethod
     def create_from_email(cls, email, **other_contact_data):
```

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/event.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/event.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/lead.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/lead.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/opportunity.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/opportunity.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from ..enums import OpportunityPeriod, OpportunityStatus
 from .base import BaseResourceModel
 
 
 class Opportunity(BaseResourceModel):
     status_type: OpportunityStatus = OpportunityStatus.ACTIVE
     lead_id: str
-    lead_name: str
+    lead_name: str | None = None
     contact_id: str | None = None
 
     confidence: int | None = None
-    status_label: str
-    pipeline_id: str
-    pipeline_name: str
+    status_label: str | None = None
+    pipeline_id: str | None = None
+    pipeline_name: str | None = None
 
     value: int | float | None = None
     value_period: OpportunityPeriod = OpportunityPeriod.ONE_TIME
     value_formatted: str | None = None
     value_currency: str | None = None
     expected_value: int | float | None = None
     annualized_value: int | float | None = None
```

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/sequence.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/sequence.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/smart_view.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/smart_view.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/src/close_dot_io/resources/webhook.py` & `close_dot_io-0.0.914/src/close_dot_io/resources/webhook.py`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/LICENSE.txt` & `close_dot_io-0.0.914/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/README.md` & `close_dot_io-0.0.914/README.md`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/pyproject.toml` & `close_dot_io-0.0.914/pyproject.toml`

 * *Files identical despite different names*

### Comparing `close_dot_io-0.0.913/PKG-INFO` & `close_dot_io-0.0.914/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: close-dot-io
-Version: 0.0.913
+Version: 0.0.914
 Summary: Easy interface to work with the Close.io API.
 Project-URL: Documentation, https://github.com/unknown/close_dot_io#readme
 Project-URL: Issues, https://github.com/unknown/close_dot_io/issues
 Project-URL: Source, https://github.com/unknown/close_dot_io
 Author-email: Copyfactory <dev@copyfactory.io>
 License-Expression: MIT
 License-File: LICENSE.txt
```

