# Comparing `tmp/xerosdk-0.8.3.tar.gz` & `tmp/xerosdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xerosdk-0.8.3.tar", last modified: Tue Sep 28 08:16:44 2021, max compression
+gzip compressed data, was "xerosdk-0.9.0.tar", last modified: Tue Nov 16 10:25:59 2021, max compression
```

## Comparing `xerosdk-0.8.3.tar` & `xerosdk-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:44.510978 xerosdk-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-09-28 08:16:35.000000 xerosdk-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-09-28 08:16:44.510978 xerosdk-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2021-09-28 08:16:35.000000 xerosdk-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-28 08:16:44.510978 xerosdk-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      798 2021-09-28 08:16:35.000000 xerosdk-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:44.506978 xerosdk-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:35.000000 xerosdk-0.8.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:44.506978 xerosdk-0.8.3/tests/common/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:35.000000 xerosdk-0.8.3/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1603 2021-09-28 08:16:35.000000 xerosdk-0.8.3/tests/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:44.506978 xerosdk-0.8.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:35.000000 xerosdk-0.8.3/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-09-28 08:16:35.000000 xerosdk-0.8.3/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2021-09-28 08:16:35.000000 xerosdk-0.8.3/tests/integration/test_xero.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:44.506978 xerosdk-0.8.3/xerosdk/
--rw-r--r--   0 runner    (1001) docker     (121)      518 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:44.510978 xerosdk-0.8.3/xerosdk/apis/
--rw-r--r--   0 runner    (1001) docker     (121)      580 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     8233 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/api_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/attachments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1238 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/bank_transactions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/contacts.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/invoices.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/items.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/organisations.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/payments.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/tenants.py
--rw-r--r--   0 runner    (1001) docker     (121)      446 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/apis/tracking_categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5487 2021-09-28 08:16:35.000000 xerosdk-0.8.3/xerosdk/xerosdk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-28 08:16:44.506978 xerosdk-0.8.3/xerosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2265 2021-09-28 08:16:44.000000 xerosdk-0.8.3/xerosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      721 2021-09-28 08:16:44.000000 xerosdk-0.8.3/xerosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-28 08:16:44.000000 xerosdk-0.8.3/xerosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-09-28 08:16:44.000000 xerosdk-0.8.3/xerosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-09-28 08:16:44.000000 xerosdk-0.8.3/xerosdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:59.303167 xerosdk-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2021-11-16 10:25:48.000000 xerosdk-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2377 2021-11-16 10:25:59.303167 xerosdk-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1831 2021-11-16 10:25:48.000000 xerosdk-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-16 10:25:59.303167 xerosdk-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2021-11-16 10:25:48.000000 xerosdk-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:59.299167 xerosdk-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:48.000000 xerosdk-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:59.299167 xerosdk-0.9.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:48.000000 xerosdk-0.9.0/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1603 2021-11-16 10:25:48.000000 xerosdk-0.9.0/tests/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:59.299167 xerosdk-0.9.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:48.000000 xerosdk-0.9.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-11-16 10:25:48.000000 xerosdk-0.9.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1874 2021-11-16 10:25:48.000000 xerosdk-0.9.0/tests/integration/test_xero.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:59.299167 xerosdk-0.9.0/xerosdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:59.303167 xerosdk-0.9.0/xerosdk/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)      636 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11762 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/api_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1268 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/bank_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/connections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1221 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/items.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/organisations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/payments.py
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (121)      446 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/apis/tracking_categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5655 2021-11-16 10:25:48.000000 xerosdk-0.9.0/xerosdk/xerosdk.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-16 10:25:59.299167 xerosdk-0.9.0/xerosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2377 2021-11-16 10:25:59.000000 xerosdk-0.9.0/xerosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2021-11-16 10:25:59.000000 xerosdk-0.9.0/xerosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-16 10:25:59.000000 xerosdk-0.9.0/xerosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-16 10:25:59.000000 xerosdk-0.9.0/xerosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-16 10:25:59.000000 xerosdk-0.9.0/xerosdk.egg-info/top_level.txt
```

### Comparing `xerosdk-0.8.3/LICENSE` & `xerosdk-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xerosdk-0.8.3/PKG-INFO` & `xerosdk-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerosdk
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python SDK to access Xero APIs
 Home-page: https://github.com/fylein/xero-sdk-py
 Author: Ashwin T
 Author-email: ashwin.t@fyle.in
 License: MIT
 Keywords: xero,api,python,sdk
 Platform: UNKNOWN
@@ -60,14 +60,18 @@
 """
 USAGE: <XeroSDK INSTANCE>.<API_NAME>.<API_METHOD>(<PARAMETERS>)
 """
 
 # Get a list of all Invoices
 response = connection.invoices.get_all()
 
+# Get a list of all Invoices using generator
+for response in invoices.list_all_generator():
+   print(response)
+
 # Get an Invoice by id
 response = connection.invoices.get_by_id(<invoice_id>)
 ```
 
 **NOTE**: Only Tenants, Invoices, Accounts, Contacts, Items and TrackingCategories 
 API classes are defined in this SDK.
```

### Comparing `xerosdk-0.8.3/README.md` & `xerosdk-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,18 @@
 """
 USAGE: <XeroSDK INSTANCE>.<API_NAME>.<API_METHOD>(<PARAMETERS>)
 """
 
 # Get a list of all Invoices
 response = connection.invoices.get_all()
 
+# Get a list of all Invoices using generator
+for response in invoices.list_all_generator():
+   print(response)
+
 # Get an Invoice by id
 response = connection.invoices.get_by_id(<invoice_id>)
 ```
 
 **NOTE**: Only Tenants, Invoices, Accounts, Contacts, Items and TrackingCategories 
 API classes are defined in this SDK.
```

### Comparing `xerosdk-0.8.3/setup.py` & `xerosdk-0.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
 setuptools.setup(
     name='xerosdk',
-    version='0.8.3',
+    version='0.9.0',
     author='Ashwin T',
     author_email='ashwin.t@fyle.in',
     description='Python SDK to access Xero APIs',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['xero', 'api', 'python', 'sdk'],
```

### Comparing `xerosdk-0.8.3/tests/common/utils.py` & `xerosdk-0.9.0/tests/common/utils.py`

 * *Files identical despite different names*

### Comparing `xerosdk-0.8.3/tests/integration/test_xero.py` & `xerosdk-0.9.0/tests/integration/test_xero.py`

 * *Files identical despite different names*

### Comparing `xerosdk-0.8.3/xerosdk/__init__.py` & `xerosdk-0.9.0/xerosdk/__init__.py`

 * *Files identical despite different names*

### Comparing `xerosdk-0.8.3/xerosdk/apis/__init__.py` & `xerosdk-0.9.0/xerosdk/apis/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 from .tracking_categories import TrackingCategories
 from .payments import Payments
 from .items import Items
 from .tenants import Tenants
 from .bank_transactions import BankTransactions
 from .attachments import Attachments
 from .organisations import Organisations
+from .connections import Connections
 
 __all__ = [
     'Invoices',
     'Accounts',
     'Contacts',
     'TrackingCategories',
     'Payments',
     'Items',
     'Tenants',
     'BankTransactions',
     'Attachments',
-    'Organisations'
+    'Organisations',
+    'Connections'
 ]
```

### Comparing `xerosdk-0.8.3/xerosdk/apis/api_base.py` & `xerosdk-0.9.0/xerosdk/apis/api_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -42,28 +42,72 @@
         Set tenant id while creating connection
         Parameters:
             tenant_id (str): Xero tenant ID
         """
 
         self.__tenant_id = tenant_id
 
-    def _get_request(self, api_url):
+    def _search_request(self, api_url, parameter: str, value: str):
         """
         HTTP get request to a given Xero API URL
 
         Parameters:
             api_url (str): URL of Xero API
+            additional_headers (dict): HTTP Additional headers for the wanted API.
         """
 
         api_headers = {
             'authorization': 'Bearer ' + self.__access_token,
             'xero-tenant-id': self.__tenant_id,
             'accept': 'application/json'
         }
 
+        api_url = '{0}?where={1}="{2}"'.format(api_url, parameter, value)
+
+        response = requests.get(
+            self.__server_url+api_url,
+            headers=api_headers
+        )
+
+        if response.status_code == 200:
+            result = json.loads(response.text)
+            return result
+
+        if response.status_code == 403:
+            raise UnsuccessfulAuthentication(
+                'Invalid xero tenant ID or xero-tenant-id header missing'
+            )
+
+        if response.status_code == 500:
+            raise InternalServerError(
+                'Internal server error'
+            )
+
+        raise XeroSDKError(
+            'Status code {0}'.format(response.status_code), response.text
+        )
+
+    def _get_request(self, api_url, page = None, additional_headers: dict = {}):
+        """
+        HTTP get request to a given Xero API URL
+
+        Parameters:
+            api_url (str): URL of Xero API
+            page (int): Page number
+            additional_headers (dict): HTTP Additional headers for the wanted API.
+        """
+
+        api_headers = {
+            'authorization': 'Bearer ' + self.__access_token,
+            'xero-tenant-id': self.__tenant_id,
+            'accept': 'application/json',
+            **additional_headers
+        }
+
+        api_url = '{0}?page={1}'.format(api_url, page)
         response = requests.get(
             self.__server_url+api_url,
             headers=api_headers
         )
 
         if response.status_code == 200:
             result = json.loads(response.text)
@@ -79,14 +123,33 @@
                 'Internal server error'
             )
 
         raise XeroSDKError(
             'Status code {0}'.format(response.status_code), response.text
         )
 
+    def _get_all_generator(self, api_url: str, attribute_type: str, additional_headers: dict = {}):
+        """
+        HTTP get request to a given Xero API URL
+
+        Parameters:
+            api_url (str): URL of Xero API
+            attribute_type: API calling Attribute
+        """
+        page = 1
+        has_more = True
+
+        while has_more:
+            response = self._get_request(api_url, page, additional_headers)
+            page += 1
+            yield response
+
+            if not response[attribute_type]:
+                has_more = False
+
     def _update_request(self, data, api_url):
         """
         HTTP put method to send data to Xero API URL
 
         Parameters:
             data (dict): Data to be sent to Xero API
             api_url (str): URL of Xero API
@@ -159,14 +222,59 @@
 
         if response.status_code == 400:
             error_msg = json.loads(response.text)
             raise WrongParamsError(error_msg, response.status_code)
 
         if response.status_code == 401:
             error_msg = json.loads(response.text)
+            raise InvalidTokenError('Invalid token, try to refresh it', error_msg)
+
+        if response.status_code == 403:
+            error_msg = json.loads(response.text)
+            raise NoPrivilegeError('Forbidden, the user has insufficient privilege', error_msg)
+
+        if response.status_code == 404:
+            error_msg = json.loads(response.text)
+            raise NotFoundItemError('Not found item with ID', error_msg)
+
+        if response.status_code == 500:
+            error_msg = json.loads(response.text)
+            raise InternalServerError('Internal server error', error_msg)
+
+        raise XeroSDKError(
+            'Status code {0}'.format(response.status_code), response.text
+        )
+
+    def _delete_request(self, api_url: str):
+        """
+        HTTP delete method to send data to Xero API URL
+
+        Parameters:
+            api_url (str): URL of Xero API
+        """
+        api_headers = {
+            'authorization': 'Bearer ' + self.__access_token,
+        }
+        response = requests.delete(
+            self.__server_url + api_url,
+            headers=api_headers
+        )
+
+        if response.status_code == 200:
+            return json.loads(response.text)
+
+        if response.status_code == 204:
+            return None
+
+        if response.status_code == 400:
+            error_msg = json.loads(response.text)
+            raise WrongParamsError(error_msg, response.status_code)
+
+        if response.status_code == 401:
+            error_msg = json.loads(response.text)
             raise InvalidTokenError('Invalid token, try to refresh it', error_msg)
 
         if response.status_code == 403:
             error_msg = json.loads(response.text)
             raise NoPrivilegeError('Forbidden, the user has insufficient privilege', error_msg)
 
         if response.status_code == 404:
```

### Comparing `xerosdk-0.8.3/xerosdk/apis/attachments.py` & `xerosdk-0.9.0/xerosdk/apis/attachments.py`

 * *Files identical despite different names*

### Comparing `xerosdk-0.8.3/xerosdk/apis/bank_transactions.py` & `xerosdk-0.9.0/xerosdk/apis/bank_transactions.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,24 @@
 
         Returns:
             List of all Bank Transactions
         """
 
         return self._get_request(BankTransactions.GET_BANK_TRANSACTIONS)
 
+    def list_all_generator(self):
+        """
+        Get all Bank Transactions
+
+        Returns:
+            List of all transactions with pagination and generator
+        """
+
+        return list(self._get_all_generator(BankTransactions.GET_BANK_TRANSACTIONS, 'BankTransactions'))
+
     def get_by_id(self, bank_transaction_id):
         """
         Get bank transaction by bank_transaction_id
 
         Parameters:
             bank_transaction_id (str): Bank Transaction ID
```

### Comparing `xerosdk-0.8.3/xerosdk/apis/payments.py` & `xerosdk-0.9.0/xerosdk/apis/payments.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,46 +6,56 @@
 
 
 class Payments(ApiBase):
     """
     Class for Payments API
     """
 
-    GET_INVOICES = '/api.xro/2.0/payments'
-    GET_INVOICE_BY_ID = '/api.xro/2.0/payments/{0}'
-    POST_INVOICE = '/api.xro/2.0/payments'
+    GET_PAYMENTS = '/api.xro/2.0/payments'
+    GET_PAYMENT_BY_ID = '/api.xro/2.0/payments/{0}'
+    POST_PAYMENT = '/api.xro/2.0/payments'
 
     def get_all(self):
         """
         Get all payments
 
         Returns:
             List of all payments
         """
 
-        return self._get_request(Payments.GET_INVOICES)
+        return self._get_request(Payments.GET_PAYMENTS)
+
+    def list_all_generator(self):
+        """
+        Get all payments
+
+        Returns:
+            List of all payments with pagination
+        """
+
+        return list(self._get_all_generator(Payments.GET_PAYMENTS, 'Payments'))
 
     def get_by_id(self, payment_id):
         """
         Get payment by payment_id
 
         Parameters:
             payment_id (str): Payment ID
 
         Returns:
             Payment dict
         """
 
-        return self._get_request(Payments.GET_INVOICE_BY_ID.format(payment_id))
+        return self._get_request(Payments.GET_PAYMENT_BY_ID.format(payment_id))
 
     def post(self, data):
         """
         Create new payment
 
         Parameters:
             data (dict): Data to create payment
 
         Returns:
              Response from API
         """
 
-        return self._update_request(data, Payments.POST_INVOICE)
+        return self._update_request(data, Payments.POST_PAYMENT)
```

### Comparing `xerosdk-0.8.3/xerosdk/exceptions.py` & `xerosdk-0.9.0/xerosdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `xerosdk-0.8.3/xerosdk/xerosdk.py` & `xerosdk-0.9.0/xerosdk/xerosdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,27 @@
 
     def __init__(self, base_url, client_id, client_secret, refresh_token):
         # Store the input parameters
         self.__base_url = base_url
         self.__client_id = client_id
         self.__client_secret = client_secret
         self._refresh_token = refresh_token  # Fix: refresh token expiry
-        self.__tenant_id = None
 
         # Create an object for each API
         self.invoices = Invoices()
         self.accounts = Accounts()
         self.contacts = Contacts()
         self.tracking_categories = TrackingCategories()
         self.payments = Payments()
         self.items = Items()
         self.tenants = Tenants()
         self.bank_transactions = BankTransactions()
         self.attachments = Attachments()
         self.organisations = Organisations()
+        self.connections = Connections()
 
         # Set the server url
         self.set_server_url()
 
         # Refresh access token
         self.refresh_access_token()
 
@@ -64,14 +64,15 @@
         self.tracking_categories.set_server_url(base_url)
         self.items.set_server_url(base_url)
         self.tenants.set_server_url(base_url)
         self.payments.set_server_url(base_url)
         self.bank_transactions.set_server_url(base_url)
         self.attachments.set_server_url(base_url)
         self.organisations.set_server_url(base_url)
+        self.connections.set_server_url(base_url)
 
     def set_tenant_id(self, tenant_id):
         """
         Set tenant id for all API objects
 
         Parameters:
             tenant_id (str): Xero tenant ID
@@ -83,14 +84,15 @@
         self.tracking_categories.set_tenant_id(tenant_id)
         self.items.set_tenant_id(tenant_id)
         self.payments.set_tenant_id(tenant_id)
         self.tenants.set_tenant_id(tenant_id)
         self.bank_transactions.set_tenant_id(tenant_id)
         self.attachments.set_tenant_id(tenant_id)
         self.organisations.set_tenant_id(tenant_id)
+        self.connections.set_tenant_id(tenant_id)
 
     def refresh_access_token(self):
         """
         Refresh access token for each API objects
         """
 
         access_token = self.__get_access_token()
@@ -101,14 +103,15 @@
         self.tracking_categories.change_access_token(access_token)
         self.items.change_access_token(access_token)
         self.payments.change_access_token(access_token)
         self.tenants.change_access_token(access_token)
         self.bank_transactions.change_access_token(access_token)
         self.attachments.change_access_token(access_token)
         self.organisations.change_access_token(access_token)
+        self.connections.change_access_token(access_token)
 
     def __get_access_token(self):
         """
         Get access token from Xero TOKEN_URL
 
         Returns:
             A new access token
```

### Comparing `xerosdk-0.8.3/xerosdk.egg-info/PKG-INFO` & `xerosdk-0.9.0/xerosdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xerosdk
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python SDK to access Xero APIs
 Home-page: https://github.com/fylein/xero-sdk-py
 Author: Ashwin T
 Author-email: ashwin.t@fyle.in
 License: MIT
 Keywords: xero,api,python,sdk
 Platform: UNKNOWN
@@ -60,14 +60,18 @@
 """
 USAGE: <XeroSDK INSTANCE>.<API_NAME>.<API_METHOD>(<PARAMETERS>)
 """
 
 # Get a list of all Invoices
 response = connection.invoices.get_all()
 
+# Get a list of all Invoices using generator
+for response in invoices.list_all_generator():
+   print(response)
+
 # Get an Invoice by id
 response = connection.invoices.get_by_id(<invoice_id>)
 ```
 
 **NOTE**: Only Tenants, Invoices, Accounts, Contacts, Items and TrackingCategories 
 API classes are defined in this SDK.
```

### Comparing `xerosdk-0.8.3/xerosdk.egg-info/SOURCES.txt` & `xerosdk-0.9.0/xerosdk.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 xerosdk.egg-info/requires.txt
 xerosdk.egg-info/top_level.txt
 xerosdk/apis/__init__.py
 xerosdk/apis/accounts.py
 xerosdk/apis/api_base.py
 xerosdk/apis/attachments.py
 xerosdk/apis/bank_transactions.py
+xerosdk/apis/connections.py
 xerosdk/apis/contacts.py
 xerosdk/apis/invoices.py
 xerosdk/apis/items.py
 xerosdk/apis/organisations.py
 xerosdk/apis/payments.py
 xerosdk/apis/tenants.py
 xerosdk/apis/tracking_categories.py
```

