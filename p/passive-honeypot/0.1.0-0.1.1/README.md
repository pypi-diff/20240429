# Comparing `tmp/passive_honeypot-0.1.0.tar.gz` & `tmp/passive_honeypot-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passive_honeypot-0.1.0.tar", max compression
+gzip compressed data, was "passive_honeypot-0.1.1.tar", max compression
```

## Comparing `passive_honeypot-0.1.0.tar` & `passive_honeypot-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0    35821 2024-04-28 21:46:17.779240 passive_honeypot-0.1.0/LICENSE
--rw-r--r--   0        0        0      452 2024-04-28 23:39:21.614372 passive_honeypot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-28 21:40:41.657502 passive_honeypot-0.1.0/src/passive_honeypot/__init__.py
--rw-r--r--   0        0        0     1733 2024-04-28 21:36:51.904821 passive_honeypot-0.1.0/src/passive_honeypot/config.py
--rw-r--r--   0        0        0     4555 2024-04-28 21:36:51.905822 passive_honeypot-0.1.0/src/passive_honeypot/database.py
--rw-r--r--   0        0        0    23461 2024-04-28 16:21:07.363515 passive_honeypot-0.1.0/src/passive_honeypot/favicon.ico
--rw-r--r--   0        0        0     6035 2024-04-28 21:36:51.906821 passive_honeypot-0.1.0/src/passive_honeypot/honeypot.py
--rw-r--r--   0        0        0     1508 2024-04-28 21:36:51.907822 passive_honeypot-0.1.0/src/passive_honeypot/templates/home.html
--rw-r--r--   0        0        0      749 2024-04-28 21:36:51.908825 passive_honeypot-0.1.0/src/passive_honeypot/templates/navbar.html
--rw-r--r--   0        0        0     2224 2024-04-28 21:36:51.909823 passive_honeypot-0.1.0/src/passive_honeypot/templates/view_hosts.html
--rw-r--r--   0        0        0     4217 2024-04-28 21:36:51.910823 passive_honeypot-0.1.0/src/passive_honeypot/templates/view_requests.html
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 passive_honeypot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-28 21:46:17.779240 passive_honeypot-0.1.1/LICENSE
+-rw-r--r--   0        0        0      452 2024-04-28 23:48:06.726627 passive_honeypot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6035 2024-04-28 23:44:01.645996 passive_honeypot-0.1.1/src/passive_honeypot/__init__.py
+-rw-r--r--   0        0        0     1733 2024-04-28 21:36:51.904821 passive_honeypot-0.1.1/src/passive_honeypot/config.py
+-rw-r--r--   0        0        0     4555 2024-04-28 21:36:51.905822 passive_honeypot-0.1.1/src/passive_honeypot/database.py
+-rw-r--r--   0        0        0    23461 2024-04-28 16:21:07.363515 passive_honeypot-0.1.1/src/passive_honeypot/favicon.ico
+-rw-r--r--   0        0        0     1508 2024-04-28 21:36:51.907822 passive_honeypot-0.1.1/src/passive_honeypot/templates/home.html
+-rw-r--r--   0        0        0      749 2024-04-28 21:36:51.908825 passive_honeypot-0.1.1/src/passive_honeypot/templates/navbar.html
+-rw-r--r--   0        0        0     2224 2024-04-28 21:36:51.909823 passive_honeypot-0.1.1/src/passive_honeypot/templates/view_hosts.html
+-rw-r--r--   0        0        0     4217 2024-04-28 21:36:51.910823 passive_honeypot-0.1.1/src/passive_honeypot/templates/view_requests.html
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 passive_honeypot-0.1.1/PKG-INFO
```

### Comparing `passive_honeypot-0.1.0/LICENSE` & `passive_honeypot-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.0/src/passive_honeypot/config.py` & `passive_honeypot-0.1.1/src/passive_honeypot/config.py`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.0/src/passive_honeypot/database.py` & `passive_honeypot-0.1.1/src/passive_honeypot/database.py`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.0/src/passive_honeypot/favicon.ico` & `passive_honeypot-0.1.1/src/passive_honeypot/favicon.ico`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.0/src/passive_honeypot/honeypot.py` & `passive_honeypot-0.1.1/src/passive_honeypot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,9 +134,9 @@
             flask_app=app,
             yield_forever=argv[1] == "yield",
             run_with_ssl=argv[2] == "ssl",
             authorized_hosts=["127.0.0.1"],
             port=listen_port,
         ).run()
     except IndexError:
-        print("Usage: python3 honeypot.py [yield|noyield] [ssl|nossl] <port>")
+        print("Usage: python3 __init__.py [yield|noyield] [ssl|nossl] <port>")
         exit(1)
```

### Comparing `passive_honeypot-0.1.0/src/passive_honeypot/templates/home.html` & `passive_honeypot-0.1.1/src/passive_honeypot/templates/home.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.0/src/passive_honeypot/templates/navbar.html` & `passive_honeypot-0.1.1/src/passive_honeypot/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.0/src/passive_honeypot/templates/view_hosts.html` & `passive_honeypot-0.1.1/src/passive_honeypot/templates/view_hosts.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.0/src/passive_honeypot/templates/view_requests.html` & `passive_honeypot-0.1.1/src/passive_honeypot/templates/view_requests.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.0/PKG-INFO` & `passive_honeypot-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passive_honeypot
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple passive honeypot written in Python with Flask and psycopg2.
 Author: ottodanp
 Author-email: ottodanp@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

