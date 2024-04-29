# Comparing `tmp/passive_honeypot-0.1.1.tar.gz` & `tmp/passive_honeypot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passive_honeypot-0.1.1.tar", max compression
+gzip compressed data, was "passive_honeypot-0.1.2.tar", max compression
```

## Comparing `passive_honeypot-0.1.1.tar` & `passive_honeypot-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35821 2024-04-28 21:46:17.779240 passive_honeypot-0.1.1/LICENSE
--rw-r--r--   0        0        0      452 2024-04-28 23:48:06.726627 passive_honeypot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6035 2024-04-28 23:44:01.645996 passive_honeypot-0.1.1/src/passive_honeypot/__init__.py
--rw-r--r--   0        0        0     1733 2024-04-28 21:36:51.904821 passive_honeypot-0.1.1/src/passive_honeypot/config.py
--rw-r--r--   0        0        0     4555 2024-04-28 21:36:51.905822 passive_honeypot-0.1.1/src/passive_honeypot/database.py
--rw-r--r--   0        0        0    23461 2024-04-28 16:21:07.363515 passive_honeypot-0.1.1/src/passive_honeypot/favicon.ico
--rw-r--r--   0        0        0     1508 2024-04-28 21:36:51.907822 passive_honeypot-0.1.1/src/passive_honeypot/templates/home.html
--rw-r--r--   0        0        0      749 2024-04-28 21:36:51.908825 passive_honeypot-0.1.1/src/passive_honeypot/templates/navbar.html
--rw-r--r--   0        0        0     2224 2024-04-28 21:36:51.909823 passive_honeypot-0.1.1/src/passive_honeypot/templates/view_hosts.html
--rw-r--r--   0        0        0     4217 2024-04-28 21:36:51.910823 passive_honeypot-0.1.1/src/passive_honeypot/templates/view_requests.html
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 passive_honeypot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-28 21:46:17.779240 passive_honeypot-0.1.2/LICENSE
+-rw-r--r--   0        0        0      452 2024-04-29 00:05:51.118133 passive_honeypot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6069 2024-04-29 00:05:39.309513 passive_honeypot-0.1.2/src/passive_honeypot/__init__.py
+-rw-r--r--   0        0        0     1733 2024-04-28 21:36:51.904821 passive_honeypot-0.1.2/src/passive_honeypot/config.py
+-rw-r--r--   0        0        0     4555 2024-04-28 21:36:51.905822 passive_honeypot-0.1.2/src/passive_honeypot/database.py
+-rw-r--r--   0        0        0    23461 2024-04-28 16:21:07.363515 passive_honeypot-0.1.2/src/passive_honeypot/favicon.ico
+-rw-r--r--   0        0        0     1508 2024-04-28 21:36:51.907822 passive_honeypot-0.1.2/src/passive_honeypot/templates/home.html
+-rw-r--r--   0        0        0      749 2024-04-28 21:36:51.908825 passive_honeypot-0.1.2/src/passive_honeypot/templates/navbar.html
+-rw-r--r--   0        0        0     2224 2024-04-28 21:36:51.909823 passive_honeypot-0.1.2/src/passive_honeypot/templates/view_hosts.html
+-rw-r--r--   0        0        0     4217 2024-04-28 21:36:51.910823 passive_honeypot-0.1.2/src/passive_honeypot/templates/view_requests.html
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 passive_honeypot-0.1.2/PKG-INFO
```

### Comparing `passive_honeypot-0.1.1/LICENSE` & `passive_honeypot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.1/src/passive_honeypot/__init__.py` & `passive_honeypot-0.1.2/src/passive_honeypot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from json import dumps
 from sys import argv
 from typing import Tuple, Dict, List, Generator, Any, Union
 
 from flask import Flask, request, render_template, redirect
 
-from config import Config
-from database import DbHandler
+from passive_honeypot.config import Config
+from passive_honeypot.database import DbHandler
 
 
 class Listener:
     _config: Config
     _flask_app: Flask
     _authorized_addresses: List[str]
     _yield_forever: bool
```

### Comparing `passive_honeypot-0.1.1/src/passive_honeypot/config.py` & `passive_honeypot-0.1.2/src/passive_honeypot/config.py`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.1/src/passive_honeypot/database.py` & `passive_honeypot-0.1.2/src/passive_honeypot/database.py`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.1/src/passive_honeypot/favicon.ico` & `passive_honeypot-0.1.2/src/passive_honeypot/favicon.ico`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.1/src/passive_honeypot/templates/home.html` & `passive_honeypot-0.1.2/src/passive_honeypot/templates/home.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.1/src/passive_honeypot/templates/navbar.html` & `passive_honeypot-0.1.2/src/passive_honeypot/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.1/src/passive_honeypot/templates/view_hosts.html` & `passive_honeypot-0.1.2/src/passive_honeypot/templates/view_hosts.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.1/src/passive_honeypot/templates/view_requests.html` & `passive_honeypot-0.1.2/src/passive_honeypot/templates/view_requests.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.1/PKG-INFO` & `passive_honeypot-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passive_honeypot
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple passive honeypot written in Python with Flask and psycopg2.
 Author: ottodanp
 Author-email: ottodanp@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

