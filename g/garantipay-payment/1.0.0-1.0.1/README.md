# Comparing `tmp/garantipay_payment-1.0.0.tar.gz` & `tmp/garantipay_payment-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garantipay_payment-1.0.0.tar", last modified: Fri Apr 26 10:01:34 2024, max compression
+gzip compressed data, was "garantipay_payment-1.0.1.tar", last modified: Mon Apr 29 07:53:52 2024, max compression
```

## Comparing `garantipay_payment-1.0.0.tar` & `garantipay_payment-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-26 10:01:34.576254 garantipay_payment-1.0.0/
--rw-r--r--   0 ismailbayram   (501) staff       (20)     1299 2024-04-26 10:01:34.576056 garantipay_payment-1.0.0/PKG-INFO
--rw-r--r--   0 ismailbayram   (501) staff       (20)      861 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/README.md
-drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-26 10:01:34.573948 garantipay_payment-1.0.0/garantipay_payment/
--rw-r--r--   0 ismailbayram   (501) staff       (20)        0 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/__init__.py
-drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-26 10:01:34.575084 garantipay_payment-1.0.0/garantipay_payment/commerce/
--rw-r--r--   0 ismailbayram   (501) staff       (20)        0 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/commerce/__init__.py
--rw-r--r--   0 ismailbayram   (501) staff       (20)     1915 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/commerce/checkout.py
--rw-r--r--   0 ismailbayram   (501) staff       (20)     1389 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/commerce/dummy.py
--rw-r--r--   0 ismailbayram   (501) staff       (20)      441 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/forms.py
-drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-26 10:01:34.575677 garantipay_payment-1.0.0/garantipay_payment/tests/
--rw-r--r--   0 ismailbayram   (501) staff       (20)        0 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/tests/__init__.py
--rw-r--r--   0 ismailbayram   (501) staff       (20)      716 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/tests/mixins.py
--rw-r--r--   0 ismailbayram   (501) staff       (20)     3751 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/tests/test_service.py
--rw-r--r--   0 ismailbayram   (501) staff       (20)     2065 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/tests/test_views.py
--rw-r--r--   0 ismailbayram   (501) staff       (20)      174 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/urls.py
--rw-r--r--   0 ismailbayram   (501) staff       (20)     1167 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/garantipay_payment/views.py
-drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-26 10:01:34.575844 garantipay_payment-1.0.0/garantipay_payment.egg-info/
--rw-r--r--   0 ismailbayram   (501) staff       (20)     1299 2024-04-26 10:01:34.000000 garantipay_payment-1.0.0/garantipay_payment.egg-info/PKG-INFO
--rw-r--r--   0 ismailbayram   (501) staff       (20)      651 2024-04-26 10:01:34.000000 garantipay_payment-1.0.0/garantipay_payment.egg-info/SOURCES.txt
--rw-r--r--   0 ismailbayram   (501) staff       (20)        1 2024-04-26 10:01:34.000000 garantipay_payment-1.0.0/garantipay_payment.egg-info/dependency_links.txt
--rw-r--r--   0 ismailbayram   (501) staff       (20)        1 2024-04-26 10:01:34.000000 garantipay_payment-1.0.0/garantipay_payment.egg-info/not-zip-safe
--rw-r--r--   0 ismailbayram   (501) staff       (20)       88 2024-04-26 10:01:34.000000 garantipay_payment-1.0.0/garantipay_payment.egg-info/requires.txt
--rw-r--r--   0 ismailbayram   (501) staff       (20)       19 2024-04-26 10:01:34.000000 garantipay_payment-1.0.0/garantipay_payment.egg-info/top_level.txt
--rw-r--r--   0 ismailbayram   (501) staff       (20)       38 2024-04-26 10:01:34.576307 garantipay_payment-1.0.0/setup.cfg
--rw-r--r--   0 ismailbayram   (501) staff       (20)      750 2024-04-26 09:56:06.000000 garantipay_payment-1.0.0/setup.py
+drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-29 07:53:52.481503 garantipay_payment-1.0.1/
+-rw-r--r--   0 ismailbayram   (501) staff       (20)     1299 2024-04-29 07:53:52.481297 garantipay_payment-1.0.1/PKG-INFO
+-rw-r--r--   0 ismailbayram   (501) staff       (20)      861 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/README.md
+drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-29 07:53:52.478105 garantipay_payment-1.0.1/garantipay_payment/
+-rw-r--r--   0 ismailbayram   (501) staff       (20)        0 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/__init__.py
+drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-29 07:53:52.480027 garantipay_payment-1.0.1/garantipay_payment/commerce/
+-rw-r--r--   0 ismailbayram   (501) staff       (20)        0 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/commerce/__init__.py
+-rw-r--r--   0 ismailbayram   (501) staff       (20)     1915 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/commerce/checkout.py
+-rw-r--r--   0 ismailbayram   (501) staff       (20)     1389 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/commerce/dummy.py
+-rw-r--r--   0 ismailbayram   (501) staff       (20)      441 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/forms.py
+drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-29 07:53:52.480179 garantipay_payment-1.0.1/garantipay_payment/templates/
+-rw-r--r--   0 ismailbayram   (501) staff       (20)      621 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/templates/garantipay.html
+drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-29 07:53:52.480802 garantipay_payment-1.0.1/garantipay_payment/tests/
+-rw-r--r--   0 ismailbayram   (501) staff       (20)        0 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/tests/__init__.py
+-rw-r--r--   0 ismailbayram   (501) staff       (20)      716 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/tests/mixins.py
+-rw-r--r--   0 ismailbayram   (501) staff       (20)     3751 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/tests/test_service.py
+-rw-r--r--   0 ismailbayram   (501) staff       (20)     2065 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/tests/test_views.py
+-rw-r--r--   0 ismailbayram   (501) staff       (20)      174 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/urls.py
+-rw-r--r--   0 ismailbayram   (501) staff       (20)     1167 2024-04-26 09:56:06.000000 garantipay_payment-1.0.1/garantipay_payment/views.py
+drwxr-xr-x   0 ismailbayram   (501) staff       (20)        0 2024-04-29 07:53:52.481067 garantipay_payment-1.0.1/garantipay_payment.egg-info/
+-rw-r--r--   0 ismailbayram   (501) staff       (20)     1299 2024-04-29 07:53:52.000000 garantipay_payment-1.0.1/garantipay_payment.egg-info/PKG-INFO
+-rw-r--r--   0 ismailbayram   (501) staff       (20)      696 2024-04-29 07:53:52.000000 garantipay_payment-1.0.1/garantipay_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 ismailbayram   (501) staff       (20)        1 2024-04-29 07:53:52.000000 garantipay_payment-1.0.1/garantipay_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 ismailbayram   (501) staff       (20)        1 2024-04-26 10:01:34.000000 garantipay_payment-1.0.1/garantipay_payment.egg-info/not-zip-safe
+-rw-r--r--   0 ismailbayram   (501) staff       (20)       88 2024-04-29 07:53:52.000000 garantipay_payment-1.0.1/garantipay_payment.egg-info/requires.txt
+-rw-r--r--   0 ismailbayram   (501) staff       (20)       19 2024-04-29 07:53:52.000000 garantipay_payment-1.0.1/garantipay_payment.egg-info/top_level.txt
+-rw-r--r--   0 ismailbayram   (501) staff       (20)       38 2024-04-29 07:53:52.481551 garantipay_payment-1.0.1/setup.cfg
+-rw-r--r--   0 ismailbayram   (501) staff       (20)      808 2024-04-29 07:52:24.000000 garantipay_payment-1.0.1/setup.py
```

### Comparing `garantipay_payment-1.0.0/PKG-INFO` & `garantipay_payment-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garantipay-payment
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library to provide payment gateway for GarantiPay 2.0
 Home-page: https://bitbucket.org/akinonteam/garantipay-payment
 Author: Akinon
 Author-email: dev@akinon.com
 Description-Content-Type: text/markdown
 Requires-Dist: Django<4.0,>=2.2.9
 Requires-Dist: requests
```

### Comparing `garantipay_payment-1.0.0/README.md` & `garantipay_payment-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `garantipay_payment-1.0.0/garantipay_payment/commerce/checkout.py` & `garantipay_payment-1.0.1/garantipay_payment/commerce/checkout.py`

 * *Files identical despite different names*

### Comparing `garantipay_payment-1.0.0/garantipay_payment/commerce/dummy.py` & `garantipay_payment-1.0.1/garantipay_payment/commerce/dummy.py`

 * *Files identical despite different names*

### Comparing `garantipay_payment-1.0.0/garantipay_payment/tests/mixins.py` & `garantipay_payment-1.0.1/garantipay_payment/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `garantipay_payment-1.0.0/garantipay_payment/tests/test_service.py` & `garantipay_payment-1.0.1/garantipay_payment/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `garantipay_payment-1.0.0/garantipay_payment/tests/test_views.py` & `garantipay_payment-1.0.1/garantipay_payment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `garantipay_payment-1.0.0/garantipay_payment/views.py` & `garantipay_payment-1.0.1/garantipay_payment/views.py`

 * *Files identical despite different names*

### Comparing `garantipay_payment-1.0.0/garantipay_payment.egg-info/PKG-INFO` & `garantipay_payment-1.0.1/garantipay_payment.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garantipay-payment
-Version: 1.0.0
+Version: 1.0.1
 Summary: A library to provide payment gateway for GarantiPay 2.0
 Home-page: https://bitbucket.org/akinonteam/garantipay-payment
 Author: Akinon
 Author-email: dev@akinon.com
 Description-Content-Type: text/markdown
 Requires-Dist: Django<4.0,>=2.2.9
 Requires-Dist: requests
```

### Comparing `garantipay_payment-1.0.0/garantipay_payment.egg-info/SOURCES.txt` & `garantipay_payment-1.0.1/garantipay_payment.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,11 +9,12 @@
 garantipay_payment.egg-info/dependency_links.txt
 garantipay_payment.egg-info/not-zip-safe
 garantipay_payment.egg-info/requires.txt
 garantipay_payment.egg-info/top_level.txt
 garantipay_payment/commerce/__init__.py
 garantipay_payment/commerce/checkout.py
 garantipay_payment/commerce/dummy.py
+garantipay_payment/templates/garantipay.html
 garantipay_payment/tests/__init__.py
 garantipay_payment/tests/mixins.py
 garantipay_payment/tests/test_service.py
 garantipay_payment/tests/test_views.py
```

### Comparing `garantipay_payment-1.0.0/setup.py` & `garantipay_payment-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("readme.md", "r") as f:
         return f.read()
 
 
 setuptools.setup(
     name="garantipay-payment",
-    version="1.0.0",
+    version="1.0.1",
     author="Akinon",
     author_email="dev@akinon.com",
     description="A library to provide payment gateway for GarantiPay 2.0",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/akinonteam/garantipay-payment",
     packages=setuptools.find_packages(exclude=["tests", "tests.*", "dummy.*"]),
@@ -21,8 +21,9 @@
         "Django>=2.2.9,<4.0",
         "requests",
         "djangorestframework>=3.11.0,<3.15",
         "orjson==3.7.2",
         "mock==4.0.3",
     ],
     include_package_data=True,
+    package_data={"garantipay_payment": ["templates/*"]},
 )
```

