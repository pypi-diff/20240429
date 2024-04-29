# Comparing `tmp/vonage_messages-1.1.0.tar.gz` & `tmp/vonage_messages-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_messages-1.1.0.tar", last modified: Tue Apr 23 14:16:53 2024, max compression
+gzip compressed data, was "vonage_messages-1.1.1.tar", last modified: Mon Apr 29 01:52:07 2024, max compression
```

## Comparing `vonage_messages-1.1.0.tar` & `vonage_messages-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.251484 vonage_messages-1.1.0/
--rw-r--r--   0 mkahan     (503) staff       (20)     3289 2024-04-23 14:16:53.250993 vonage_messages-1.1.0/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)     2510 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      836 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-23 14:16:53.251541 vonage_messages-1.1.0/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.228661 vonage_messages-1.1.0/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.233991 vonage_messages-1.1.0/src/vonage_messages/
--rw-r--r--   0 mkahan     (503) staff       (20)      152 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1616 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/messages.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.249880 vonage_messages-1.1.0/src/vonage_messages/models/
--rw-r--r--   0 mkahan     (503) staff       (20)     2136 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      348 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/base_message.py
--rw-r--r--   0 mkahan     (503) staff       (20)      548 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/enums.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1490 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/messenger.py
--rw-r--r--   0 mkahan     (503) staff       (20)      942 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/mms.py
--rw-r--r--   0 mkahan     (503) staff       (20)      672 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/sms.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2485 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/viber.py
--rw-r--r--   0 mkahan     (503) staff       (20)     2387 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/models/whatsapp.py
--rw-r--r--   0 mkahan     (503) staff       (20)      221 2024-04-23 14:16:51.000000 vonage_messages-1.1.0/src/vonage_messages/responses.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-23 14:16:53.250434 vonage_messages-1.1.0/src/vonage_messages.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     3289 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      652 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       16 2024-04-23 14:16:53.000000 vonage_messages-1.1.0/src/vonage_messages.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.760351 vonage_messages-1.1.1/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3289 2024-04-29 01:52:07.759537 vonage_messages-1.1.1/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)     2510 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      836 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:07.760422 vonage_messages-1.1.1/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.742471 vonage_messages-1.1.1/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.744738 vonage_messages-1.1.1/src/vonage_messages/
+-rw-r--r--   0 mkahan     (503) staff       (20)      152 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1616 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/messages.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.758166 vonage_messages-1.1.1/src/vonage_messages/models/
+-rw-r--r--   0 mkahan     (503) staff       (20)     2136 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/models/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      348 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/models/base_message.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      548 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/models/enums.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1490 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/models/messenger.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      942 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/models/mms.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      672 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/models/sms.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2485 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/models/viber.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     2387 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/models/whatsapp.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      221 2024-04-29 01:52:06.000000 vonage_messages-1.1.1/src/vonage_messages/responses.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.758865 vonage_messages-1.1.1/src/vonage_messages.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     3289 2024-04-29 01:52:07.000000 vonage_messages-1.1.1/src/vonage_messages.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      652 2024-04-29 01:52:07.000000 vonage_messages-1.1.1/src/vonage_messages.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:07.000000 vonage_messages-1.1.1/src/vonage_messages.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       62 2024-04-29 01:52:07.000000 vonage_messages-1.1.1/src/vonage_messages.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       16 2024-04-29 01:52:07.000000 vonage_messages-1.1.1/src/vonage_messages.egg-info/top_level.txt
```

### Comparing `vonage_messages-1.1.0/PKG-INFO` & `vonage_messages-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-messages
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vonage messages package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-http-client>=1.3.0
-Requires-Dist: vonage-utils>=1.1.0
-Requires-Dist: pydantic>=2.6.1
+Requires-Dist: vonage-http-client>=1.3.1
+Requires-Dist: vonage-utils>=1.1.1
+Requires-Dist: pydantic>=2.7.1
 
 # Vonage Messages Package
 
 This package contains the code to use [Vonage's Messages API](https://developer.vonage.com/en/messages/overview) in Python.
 
 ## Usage
```

### Comparing `vonage_messages-1.1.0/README.md` & `vonage_messages-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/backend_shim.py` & `vonage_messages-1.1.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/pyproject.toml` & `vonage_messages-1.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = 'vonage-messages'
-version = '1.1.0'
+version = '1.1.1'
 description = 'Vonage messages package'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 requires-python = ">=3.8"
 dependencies = [
-  "vonage-http-client>=1.3.0",
-  "vonage-utils>=1.1.0",
-  "pydantic>=2.6.1",
+  "vonage-http-client>=1.3.1",
+  "vonage-utils>=1.1.1",
+  "pydantic>=2.7.1",
 ]
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `vonage_messages-1.1.0/src/vonage_messages/messages.py` & `vonage_messages-1.1.1/src/vonage_messages/messages.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/src/vonage_messages/models/__init__.py` & `vonage_messages-1.1.1/src/vonage_messages/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/src/vonage_messages/models/enums.py` & `vonage_messages-1.1.1/src/vonage_messages/models/enums.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/src/vonage_messages/models/messenger.py` & `vonage_messages-1.1.1/src/vonage_messages/models/messenger.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/src/vonage_messages/models/mms.py` & `vonage_messages-1.1.1/src/vonage_messages/models/mms.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/src/vonage_messages/models/sms.py` & `vonage_messages-1.1.1/src/vonage_messages/models/sms.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/src/vonage_messages/models/viber.py` & `vonage_messages-1.1.1/src/vonage_messages/models/viber.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/src/vonage_messages/models/whatsapp.py` & `vonage_messages-1.1.1/src/vonage_messages/models/whatsapp.py`

 * *Files identical despite different names*

### Comparing `vonage_messages-1.1.0/src/vonage_messages.egg-info/PKG-INFO` & `vonage_messages-1.1.1/src/vonage_messages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vonage-messages
-Version: 1.1.0
+Version: 1.1.1
 Summary: Vonage messages package
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: vonage-http-client>=1.3.0
-Requires-Dist: vonage-utils>=1.1.0
-Requires-Dist: pydantic>=2.6.1
+Requires-Dist: vonage-http-client>=1.3.1
+Requires-Dist: vonage-utils>=1.1.1
+Requires-Dist: pydantic>=2.7.1
 
 # Vonage Messages Package
 
 This package contains the code to use [Vonage's Messages API](https://developer.vonage.com/en/messages/overview) in Python.
 
 ## Usage
```

### Comparing `vonage_messages-1.1.0/src/vonage_messages.egg-info/SOURCES.txt` & `vonage_messages-1.1.1/src/vonage_messages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

