# Comparing `tmp/ain-py-1.2.0.tar.gz` & `tmp/ain_py-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ain-py-1.2.0.tar", last modified: Fri Apr  5 02:13:19 2024, max compression
+gzip compressed data, was "ain_py-1.2.1.tar", last modified: Mon Apr 29 06:42:07 2024, max compression
```

## Comparing `ain-py-1.2.0.tar` & `ain_py-1.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.407527 ain-py-1.2.0/
--rw-r--r--   0 dongilseo   (501) staff       (20)     1778 2024-04-05 02:13:19.404497 ain-py-1.2.0/PKG-INFO
--rw-r--r--   0 dongilseo   (501) staff       (20)      707 2024-03-13 06:12:07.000000 ain-py-1.2.0/README.md
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.388115 ain-py-1.2.0/ain/
--rw-r--r--   0 dongilseo   (501) staff       (20)        0 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/__init__.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     2154 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/account.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    14690 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/ain.py
--rw-r--r--   0 dongilseo   (501) staff       (20)       38 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/constants.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.390369 ain-py-1.2.0/ain/db/
--rw-r--r--   0 dongilseo   (501) staff       (20)      844 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/db/__init__.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     2312 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/db/push_id.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    20683 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/db/ref.py
--rw-r--r--   0 dongilseo   (501) staff       (20)      420 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/errors.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     2436 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/net.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     2601 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/provider.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.392189 ain-py-1.2.0/ain/signer/
--rw-r--r--   0 dongilseo   (501) staff       (20)     2283 2024-03-13 06:12:07.000000 ain-py-1.2.0/ain/signer/__init__.py
--rw-r--r--   0 dongilseo   (501) staff       (20)     6728 2024-03-13 06:12:07.000000 ain-py-1.2.0/ain/signer/default_signer.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    14237 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/types.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.394374 ain-py-1.2.0/ain/utils/
--rw-r--r--   0 dongilseo   (501) staff       (20)    20474 2024-03-25 00:42:04.000000 ain-py-1.2.0/ain/utils/__init__.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    10552 2023-08-31 04:32:09.000000 ain-py-1.2.0/ain/utils/v3keystore.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    16311 2024-04-05 01:51:54.000000 ain-py-1.2.0/ain/wallet.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.401980 ain-py-1.2.0/ain_py.egg-info/
--rw-r--r--   0 dongilseo   (501) staff       (20)     1778 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/PKG-INFO
--rw-r--r--   0 dongilseo   (501) staff       (20)      562 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/SOURCES.txt
--rw-r--r--   0 dongilseo   (501) staff       (20)        1 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/dependency_links.txt
--rw-r--r--   0 dongilseo   (501) staff       (20)        1 2024-03-13 01:46:49.000000 ain-py-1.2.0/ain_py.egg-info/not-zip-safe
--rw-r--r--   0 dongilseo   (501) staff       (20)      136 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/requires.txt
--rw-r--r--   0 dongilseo   (501) staff       (20)        4 2024-04-05 02:13:19.000000 ain-py-1.2.0/ain_py.egg-info/top_level.txt
--rw-r--r--   0 dongilseo   (501) staff       (20)       38 2024-04-05 02:13:19.407763 ain-py-1.2.0/setup.cfg
--rw-r--r--   0 dongilseo   (501) staff       (20)     1546 2024-04-05 02:04:58.000000 ain-py-1.2.0/setup.py
-drwxr-xr-x   0 dongilseo   (501) staff       (20)        0 2024-04-05 02:13:19.400479 ain-py-1.2.0/tests/
--rw-r--r--   0 dongilseo   (501) staff       (20)    41295 2024-04-05 01:51:54.000000 ain-py-1.2.0/tests/test_ain.py
--rw-r--r--   0 dongilseo   (501) staff       (20)      950 2023-08-31 04:32:09.000000 ain-py-1.2.0/tests/test_ain_account.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    11096 2023-08-31 04:32:09.000000 ain-py-1.2.0/tests/test_ain_raw.py
--rw-r--r--   0 dongilseo   (501) staff       (20)    23247 2024-03-25 00:42:04.000000 ain-py-1.2.0/tests/test_ain_utils.py
+drwxr-xr-x   0 comcom     (501) staff       (20)        0 2024-04-29 06:42:07.272568 ain_py-1.2.1/
+-rw-r--r--   0 comcom     (501) staff       (20)     1771 2024-04-29 06:42:07.272342 ain_py-1.2.1/PKG-INFO
+-rw-r--r--   0 comcom     (501) staff       (20)      707 2024-04-29 04:39:56.000000 ain_py-1.2.1/README.md
+drwxr-xr-x   0 comcom     (501) staff       (20)        0 2024-04-29 06:42:07.268359 ain_py-1.2.1/ain/
+-rw-r--r--   0 comcom     (501) staff       (20)        0 2023-08-29 06:11:13.000000 ain_py-1.2.1/ain/__init__.py
+-rw-r--r--   0 comcom     (501) staff       (20)     2154 2023-08-29 06:11:13.000000 ain_py-1.2.1/ain/account.py
+-rw-r--r--   0 comcom     (501) staff       (20)    14690 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/ain.py
+-rw-r--r--   0 comcom     (501) staff       (20)       38 2023-08-29 06:11:13.000000 ain_py-1.2.1/ain/constants.py
+drwxr-xr-x   0 comcom     (501) staff       (20)        0 2024-04-29 06:42:07.268975 ain_py-1.2.1/ain/db/
+-rw-r--r--   0 comcom     (501) staff       (20)      844 2023-08-29 06:11:13.000000 ain_py-1.2.1/ain/db/__init__.py
+-rw-r--r--   0 comcom     (501) staff       (20)     2312 2023-08-29 06:11:13.000000 ain_py-1.2.1/ain/db/push_id.py
+-rw-r--r--   0 comcom     (501) staff       (20)    20683 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/db/ref.py
+-rw-r--r--   0 comcom     (501) staff       (20)      420 2023-08-29 06:11:13.000000 ain_py-1.2.1/ain/errors.py
+-rw-r--r--   0 comcom     (501) staff       (20)     2436 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/net.py
+-rw-r--r--   0 comcom     (501) staff       (20)     2601 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/provider.py
+drwxr-xr-x   0 comcom     (501) staff       (20)        0 2024-04-29 06:42:07.269745 ain_py-1.2.1/ain/signer/
+-rw-r--r--   0 comcom     (501) staff       (20)     2283 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/signer/__init__.py
+-rw-r--r--   0 comcom     (501) staff       (20)     6728 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/signer/default_signer.py
+-rw-r--r--   0 comcom     (501) staff       (20)    14237 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/types.py
+drwxr-xr-x   0 comcom     (501) staff       (20)        0 2024-04-29 06:42:07.270310 ain_py-1.2.1/ain/utils/
+-rw-r--r--   0 comcom     (501) staff       (20)    20474 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/utils/__init__.py
+-rw-r--r--   0 comcom     (501) staff       (20)    10552 2023-08-29 06:11:13.000000 ain_py-1.2.1/ain/utils/v3keystore.py
+-rw-r--r--   0 comcom     (501) staff       (20)    16311 2024-04-29 04:39:56.000000 ain_py-1.2.1/ain/wallet.py
+drwxr-xr-x   0 comcom     (501) staff       (20)        0 2024-04-29 06:42:07.272078 ain_py-1.2.1/ain_py.egg-info/
+-rw-r--r--   0 comcom     (501) staff       (20)     1771 2024-04-29 06:42:07.000000 ain_py-1.2.1/ain_py.egg-info/PKG-INFO
+-rw-r--r--   0 comcom     (501) staff       (20)      562 2024-04-29 06:42:07.000000 ain_py-1.2.1/ain_py.egg-info/SOURCES.txt
+-rw-r--r--   0 comcom     (501) staff       (20)        1 2024-04-29 06:42:07.000000 ain_py-1.2.1/ain_py.egg-info/dependency_links.txt
+-rw-r--r--   0 comcom     (501) staff       (20)        1 2024-04-29 06:42:07.000000 ain_py-1.2.1/ain_py.egg-info/not-zip-safe
+-rw-r--r--   0 comcom     (501) staff       (20)      129 2024-04-29 06:42:07.000000 ain_py-1.2.1/ain_py.egg-info/requires.txt
+-rw-r--r--   0 comcom     (501) staff       (20)        4 2024-04-29 06:42:07.000000 ain_py-1.2.1/ain_py.egg-info/top_level.txt
+-rw-r--r--   0 comcom     (501) staff       (20)       38 2024-04-29 06:42:07.272606 ain_py-1.2.1/setup.cfg
+-rw-r--r--   0 comcom     (501) staff       (20)     1539 2024-04-29 05:50:56.000000 ain_py-1.2.1/setup.py
+drwxr-xr-x   0 comcom     (501) staff       (20)        0 2024-04-29 06:42:07.271792 ain_py-1.2.1/tests/
+-rw-r--r--   0 comcom     (501) staff       (20)    41295 2024-04-29 04:39:56.000000 ain_py-1.2.1/tests/test_ain.py
+-rw-r--r--   0 comcom     (501) staff       (20)      950 2023-08-29 06:11:13.000000 ain_py-1.2.1/tests/test_ain_account.py
+-rw-r--r--   0 comcom     (501) staff       (20)    11096 2023-08-29 06:11:13.000000 ain_py-1.2.1/tests/test_ain_raw.py
+-rw-r--r--   0 comcom     (501) staff       (20)    23247 2024-04-29 04:39:56.000000 ain_py-1.2.1/tests/test_ain_utils.py
```

### Comparing `ain-py-1.2.0/PKG-INFO` & `ain_py-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ain-py
-Version: 1.2.0
+Version: 1.2.1
 Summary: AI Network Client Library for Python3
 Home-page: https://github.com/ainblockchain/ain-py
 Author: AIN Dev Team
 Author-email: dev@ainetwork.ai
 License: MPL license
 Keywords: ain,ainetwork,ainblockchain,API
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: typing-extensions==4.7.1
+Requires-Dist: typing-extensions
 Requires-Dist: pycryptodome==3.18.0
 Requires-Dist: coincurve==18.0.0
 Requires-Dist: aiohttp[speedups]==3.8.5
 Requires-Dist: jsonrpcclient==4.0.3
 Requires-Dist: mnemonic==0.20
 Requires-Dist: bip32==3.4
```

### Comparing `ain-py-1.2.0/README.md` & `ain_py-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/account.py` & `ain_py-1.2.1/ain/account.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/ain.py` & `ain_py-1.2.1/ain/ain.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/db/__init__.py` & `ain_py-1.2.1/ain/db/__init__.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/db/push_id.py` & `ain_py-1.2.1/ain/db/push_id.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/db/ref.py` & `ain_py-1.2.1/ain/db/ref.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/net.py` & `ain_py-1.2.1/ain/net.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/provider.py` & `ain_py-1.2.1/ain/provider.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/signer/__init__.py` & `ain_py-1.2.1/ain/signer/__init__.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/signer/default_signer.py` & `ain_py-1.2.1/ain/signer/default_signer.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/types.py` & `ain_py-1.2.1/ain/types.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/utils/__init__.py` & `ain_py-1.2.1/ain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/utils/v3keystore.py` & `ain_py-1.2.1/ain/utils/v3keystore.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain/wallet.py` & `ain_py-1.2.1/ain/wallet.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/ain_py.egg-info/PKG-INFO` & `ain_py-1.2.1/ain_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ain-py
-Version: 1.2.0
+Version: 1.2.1
 Summary: AI Network Client Library for Python3
 Home-page: https://github.com/ainblockchain/ain-py
 Author: AIN Dev Team
 Author-email: dev@ainetwork.ai
 License: MPL license
 Keywords: ain,ainetwork,ainblockchain,API
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: typing-extensions==4.7.1
+Requires-Dist: typing-extensions
 Requires-Dist: pycryptodome==3.18.0
 Requires-Dist: coincurve==18.0.0
 Requires-Dist: aiohttp[speedups]==3.8.5
 Requires-Dist: jsonrpcclient==4.0.3
 Requires-Dist: mnemonic==0.20
 Requires-Dist: bip32==3.4
```

### Comparing `ain-py-1.2.0/ain_py.egg-info/SOURCES.txt` & `ain_py-1.2.1/ain_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/setup.py` & `ain_py-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 requirements = [
-    "typing-extensions==4.7.1",
+    "typing-extensions",
     "pycryptodome==3.18.0",
     "coincurve==18.0.0",
     "aiohttp[speedups]==3.8.5",
     "jsonrpcclient==4.0.3",
     "mnemonic==0.20",
     "bip32==3.4",
 ]
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords=["ain", "ainetwork", "ainblockchain", "API"],
     name="ain-py",
     packages=find_packages(include=["ain", "ain.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/ainblockchain/ain-py",
-    version="1.2.0",
+    version="1.2.1",
     zip_safe=False,
 )
```

### Comparing `ain-py-1.2.0/tests/test_ain.py` & `ain_py-1.2.1/tests/test_ain.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/tests/test_ain_account.py` & `ain_py-1.2.1/tests/test_ain_account.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/tests/test_ain_raw.py` & `ain_py-1.2.1/tests/test_ain_raw.py`

 * *Files identical despite different names*

### Comparing `ain-py-1.2.0/tests/test_ain_utils.py` & `ain_py-1.2.1/tests/test_ain_utils.py`

 * *Files identical despite different names*

