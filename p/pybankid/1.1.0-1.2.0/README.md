# Comparing `tmp/pybankid-1.1.0.tar.gz` & `tmp/pybankid-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybankid-1.1.0.tar", last modified: Wed Apr 24 20:34:12 2024, max compression
+gzip compressed data, was "pybankid-1.2.0.tar", last modified: Mon Apr 29 08:08:43 2024, max compression
```

## Comparing `pybankid-1.1.0.tar` & `pybankid-1.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.146315 pybankid-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-24 20:34:08.000000 pybankid-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 20:34:08.000000 pybankid-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-24 20:34:12.146315 pybankid-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-24 20:34:08.000000 pybankid-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.138315 pybankid-1.1.0/bankid/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/asyncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/baseclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/bankid/certs/
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20220818.p12
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20220818_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20220818_key.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20230629.p12
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20230629_cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/FPTestcert4_20230629_key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/appapi.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/appapi.test.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/appapi2.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certs/appapi2.test.bankid.com.pem
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/certutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/bankid/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/experimental/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/experimental/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/qr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-24 20:34:08.000000 pybankid-1.1.0/bankid/syncclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.138315 pybankid-1.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/examples/qrdemo/
--rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/examples/qrdemo/qrdemo/
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/qrdemo/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.142315 pybankid-1.1.0/examples/qrdemo/qrdemo/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/qrdemo/templates/auth_complete.html
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/qrdemo/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/qrdemo/templates/qr.html
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 20:34:08.000000 pybankid-1.1.0/examples/qrdemo/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.146315 pybankid-1.1.0/pybankid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 20:34:12.000000 pybankid-1.1.0/pybankid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-24 20:34:08.000000 pybankid-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-24 20:34:12.146315 pybankid-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-24 20:34:08.000000 pybankid-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:12.146315 pybankid-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/test_asyncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/test_certutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-24 20:34:08.000000 pybankid-1.1.0/tests/test_syncclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.739759 pybankid-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 08:08:37.000000 pybankid-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-29 08:08:37.000000 pybankid-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-04-29 08:08:43.739759 pybankid-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-04-29 08:08:37.000000 pybankid-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.731758 pybankid-1.2.0/bankid/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/asyncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/baseclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.735758 pybankid-1.2.0/bankid/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/FPTestcert4_20220818.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/FPTestcert4_20220818_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/FPTestcert4_20220818_key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/FPTestcert4_20230629.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/FPTestcert4_20230629_cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/FPTestcert4_20230629_key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/appapi.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/appapi.test.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/appapi2.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certs/appapi2.test.bankid.com.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/certutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.735758 pybankid-1.2.0/bankid/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/experimental/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/experimental/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/qr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-04-29 08:08:37.000000 pybankid-1.2.0/bankid/syncclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.731758 pybankid-1.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.735758 pybankid-1.2.0/examples/qrdemo/
+-rw-r--r--   0 runner    (1001) docker     (127)    11296 2024-04-29 08:08:37.000000 pybankid-1.2.0/examples/qrdemo/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-29 08:08:37.000000 pybankid-1.2.0/examples/qrdemo/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.735758 pybankid-1.2.0/examples/qrdemo/qrdemo/
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-29 08:08:37.000000 pybankid-1.2.0/examples/qrdemo/qrdemo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.735758 pybankid-1.2.0/examples/qrdemo/qrdemo/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-29 08:08:37.000000 pybankid-1.2.0/examples/qrdemo/qrdemo/templates/auth_complete.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-29 08:08:37.000000 pybankid-1.2.0/examples/qrdemo/qrdemo/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-29 08:08:37.000000 pybankid-1.2.0/examples/qrdemo/qrdemo/templates/qr.html
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 08:08:37.000000 pybankid-1.2.0/examples/qrdemo/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.739759 pybankid-1.2.0/pybankid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8324 2024-04-29 08:08:43.000000 pybankid-1.2.0/pybankid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-29 08:08:43.000000 pybankid-1.2.0/pybankid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:08:43.000000 pybankid-1.2.0/pybankid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 08:08:43.000000 pybankid-1.2.0/pybankid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 08:08:43.000000 pybankid-1.2.0/pybankid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-29 08:08:37.000000 pybankid-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 08:08:43.739759 pybankid-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-29 08:08:37.000000 pybankid-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:43.739759 pybankid-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:08:37.000000 pybankid-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-29 08:08:37.000000 pybankid-1.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-04-29 08:08:37.000000 pybankid-1.2.0/tests/test_asyncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-29 08:08:37.000000 pybankid-1.2.0/tests/test_certutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-29 08:08:37.000000 pybankid-1.2.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-04-29 08:08:37.000000 pybankid-1.2.0/tests/test_syncclient.py
```

### Comparing `pybankid-1.1.0/LICENSE` & `pybankid-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/PKG-INFO` & `pybankid-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybankid
-Version: 1.1.0
+Version: 1.2.0
 Summary: BankID Relying Party client for Python
 Home-page: https://github.com/hbldh/pybankid
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,18 +15,19 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
+Requires-Dist: importlib_resources; python_version < "3.9"
 Provides-Extra: signature-verification
+Requires-Dist: pytz; extra == "signature-verification"
 Requires-Dist: pyOpenSSL; extra == "signature-verification"
 Requires-Dist: asn1crypto; extra == "signature-verification"
-Requires-Dist: pytz; extra == "signature-verification"
 
 
 # PyBankID
 
 ![Build and Test](https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg)
 ![Documentation Status](https://readthedocs.org/projects/pybankid/badge/?version=latest)
 ![PyPI Version](https://img.shields.io/pypi/v/pybankid)
```

### Comparing `pybankid-1.1.0/README.md` & `pybankid-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/__init__.py` & `pybankid-1.2.0/bankid/__init__.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/asyncclient.py` & `pybankid-1.2.0/bankid/asyncclient.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/baseclient.py` & `pybankid-1.2.0/bankid/baseclient.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/FPTestcert4_20220818.p12` & `pybankid-1.2.0/bankid/certs/FPTestcert4_20220818.p12`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/FPTestcert4_20220818_cert.pem` & `pybankid-1.2.0/bankid/certs/FPTestcert4_20220818_cert.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/FPTestcert4_20220818_key.pem` & `pybankid-1.2.0/bankid/certs/FPTestcert4_20220818_key.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/FPTestcert4_20230629.p12` & `pybankid-1.2.0/bankid/certs/FPTestcert4_20230629.p12`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/FPTestcert4_20230629_cert.pem` & `pybankid-1.2.0/bankid/certs/FPTestcert4_20230629_cert.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/FPTestcert4_20230629_key.pem` & `pybankid-1.2.0/bankid/certs/FPTestcert4_20230629_key.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/appapi.bankid.com.pem` & `pybankid-1.2.0/bankid/certs/appapi.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/appapi.test.bankid.com.pem` & `pybankid-1.2.0/bankid/certs/appapi.test.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/appapi2.bankid.com.pem` & `pybankid-1.2.0/bankid/certs/appapi2.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certs/appapi2.test.bankid.com.pem` & `pybankid-1.2.0/bankid/certs/appapi2.test.bankid.com.pem`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/certutils.py` & `pybankid-1.2.0/bankid/certutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 """
 :mod:`bankid.certutils` -- Certificate Utilities
 ================================================
 .. moduleauthor:: hbldh <henrik.blidh@nedomkull.com>
 """
 
 import os
+import sys
 import subprocess
 from typing import Tuple, Union
 
 import pathlib
-import importlib.resources
+if sys.version_info < (3, 9):
+    import importlib_resources as impres
+else:
+    import importlib.resources as impres
 
 from bankid.certs import get_test_cert_p12
 from bankid.exceptions import BankIDError
 
 _TEST_CERT_PASSWORD = "qwerty123"
 
 
 def resolve_cert_path(file: str) -> pathlib.Path:
-    path = importlib.resources.files("bankid.certs").joinpath(file)
+    path = impres.files("bankid.certs").joinpath(file)
     assert isinstance(path, pathlib.Path)
     return path
 
 
 def create_bankid_test_server_cert_and_key(destination_path: str = ".") -> Tuple[str, str]:
     """Split the bundled test certificate into certificate and key parts and save them
     as separate files, stored in PEM format.
@@ -33,15 +37,16 @@
 
     :param destination_path: The directory to save certificate and key files to. Default is the current directory.
     :type destination_path: str
     :returns: The path tuple ``(cert_path, key_path)``.
     :rtype: tuple
 
     """
-    if test_cert_file := os.getenv("TEST_CERT_FILE"):
+    test_cert_file = os.getenv("TEST_CERT_FILE")
+    if test_cert_file is not None:
         certificate, key = split_certificate(
             test_cert_file, destination_path, password=_TEST_CERT_PASSWORD
         )
 
     else:
         # Fetch testP12 certificate path
         certificate, key = split_certificate(str(get_test_cert_p12()), destination_path, password=_TEST_CERT_PASSWORD)
```

### Comparing `pybankid-1.1.0/bankid/exceptions.py` & `pybankid-1.2.0/bankid/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/experimental/helper.py` & `pybankid-1.2.0/bankid/experimental/helper.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/experimental/verify.py` & `pybankid-1.2.0/bankid/experimental/verify.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/qr.py` & `pybankid-1.2.0/bankid/qr.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/bankid/syncclient.py` & `pybankid-1.2.0/bankid/syncclient.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/examples/qrdemo/.gitignore` & `pybankid-1.2.0/examples/qrdemo/.gitignore`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/examples/qrdemo/README.md` & `pybankid-1.2.0/examples/qrdemo/README.md`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/examples/qrdemo/qrdemo/app.py` & `pybankid-1.2.0/examples/qrdemo/qrdemo/app.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/examples/qrdemo/qrdemo/templates/auth_complete.html` & `pybankid-1.2.0/examples/qrdemo/qrdemo/templates/auth_complete.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/examples/qrdemo/qrdemo/templates/index.html` & `pybankid-1.2.0/examples/qrdemo/qrdemo/templates/index.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/examples/qrdemo/qrdemo/templates/qr.html` & `pybankid-1.2.0/examples/qrdemo/qrdemo/templates/qr.html`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/pybankid.egg-info/PKG-INFO` & `pybankid-1.2.0/pybankid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybankid
-Version: 1.1.0
+Version: 1.2.0
 Summary: BankID Relying Party client for Python
 Home-page: https://github.com/hbldh/pybankid
 Author: Henrik Blidh
 Author-email: henrik.blidh@nedomkull.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -15,18 +15,19 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: httpx
+Requires-Dist: importlib_resources; python_version < "3.9"
 Provides-Extra: signature-verification
+Requires-Dist: pytz; extra == "signature-verification"
 Requires-Dist: pyOpenSSL; extra == "signature-verification"
 Requires-Dist: asn1crypto; extra == "signature-verification"
-Requires-Dist: pytz; extra == "signature-verification"
 
 
 # PyBankID
 
 ![Build and Test](https://github.com/hbldh/pybankid/workflows/Build%20and%20Test/badge.svg)
 ![Documentation Status](https://readthedocs.org/projects/pybankid/badge/?version=latest)
 ![PyPI Version](https://img.shields.io/pypi/v/pybankid)
```

### Comparing `pybankid-1.1.0/pybankid.egg-info/SOURCES.txt` & `pybankid-1.2.0/pybankid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/setup.py` & `pybankid-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/tests/conftest.py` & `pybankid-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/tests/test_asyncclient.py` & `pybankid-1.2.0/tests/test_asyncclient.py`

 * *Files identical despite different names*

### Comparing `pybankid-1.1.0/tests/test_exceptions.py` & `pybankid-1.2.0/tests/test_exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from collections import namedtuple
+import sys
 from typing import Union
 
 import pytest
 
 import bankid
 
+if sys.version_info >= (3, 9):
+    from builtins import type as Type
+else:
+    # Remove once PyBankID no longer support Python 3.8 or lower
+    from typing import Type
+
 
 @pytest.mark.parametrize(
     "exception_class,rfa",
     [
         (bankid.exceptions.AlreadyInProgressError, 4),
         (bankid.exceptions.InvalidParametersError, None),
         (bankid.exceptions.UnauthorizedError, None),
         (bankid.exceptions.NotFoundError, None),
         (bankid.exceptions.RequestTimeoutError, 5),
         (bankid.exceptions.InternalError, 5),
         (bankid.exceptions.MaintenanceError, 5),
         (bankid.exceptions.BankIDError, None),
     ],
 )
-def test_exceptions(exception_class: type[Exception], rfa: Union[int, None]) -> None:
+def test_exceptions(exception_class: Type[Exception], rfa: Union[int, None]) -> None:
     e = exception_class()
     assert isinstance(e, bankid.exceptions.BankIDError)
     assert e.rfa == rfa
 
 
 @pytest.mark.parametrize(
     "exception_class,error_code",
@@ -34,13 +41,13 @@
         (bankid.exceptions.NotFoundError, "notFound"),
         (bankid.exceptions.RequestTimeoutError, "requestTimeout"),
         (bankid.exceptions.InternalError, "internalError"),
         (bankid.exceptions.MaintenanceError, "maintenance"),
         (bankid.exceptions.BankIDError, "Unknown error code"),
     ],
 )
-def test_error_class_factory(exception_class: type[Exception], error_code: str) -> None:
+def test_error_class_factory(exception_class: Type[Exception], error_code: str) -> None:
     MockResponse = namedtuple("MockResponse", ["json"])
     response = MockResponse(json=lambda: {"errorCode": error_code})
     # error: Argument 1 to "get_json_error_class" has incompatible type "MockResponse@41"; expected "Response"  [arg-type]
     e_class = bankid.exceptions.get_json_error_class(response)  # type: ignore[arg-type]
     assert isinstance(e_class, exception_class)
```

### Comparing `pybankid-1.1.0/tests/test_syncclient.py` & `pybankid-1.2.0/tests/test_syncclient.py`

 * *Files identical despite different names*

