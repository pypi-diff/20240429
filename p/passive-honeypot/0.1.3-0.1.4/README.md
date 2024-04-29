# Comparing `tmp/passive_honeypot-0.1.3.tar.gz` & `tmp/passive_honeypot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passive_honeypot-0.1.3.tar", max compression
+gzip compressed data, was "passive_honeypot-0.1.4.tar", max compression
```

## Comparing `passive_honeypot-0.1.3.tar` & `passive_honeypot-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35821 2024-04-28 21:46:17.779240 passive_honeypot-0.1.3/LICENSE
--rw-r--r--   0        0        0      452 2024-04-29 00:08:42.420352 passive_honeypot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6099 2024-04-29 00:08:35.935202 passive_honeypot-0.1.3/src/passive_honeypot/__init__.py
--rw-r--r--   0        0        0     1733 2024-04-28 21:36:51.904821 passive_honeypot-0.1.3/src/passive_honeypot/config.py
--rw-r--r--   0        0        0     4555 2024-04-28 21:36:51.905822 passive_honeypot-0.1.3/src/passive_honeypot/database.py
--rw-r--r--   0        0        0    23461 2024-04-28 16:21:07.363515 passive_honeypot-0.1.3/src/passive_honeypot/favicon.ico
--rw-r--r--   0        0        0     1508 2024-04-28 21:36:51.907822 passive_honeypot-0.1.3/src/passive_honeypot/templates/home.html
--rw-r--r--   0        0        0      749 2024-04-28 21:36:51.908825 passive_honeypot-0.1.3/src/passive_honeypot/templates/navbar.html
--rw-r--r--   0        0        0     2224 2024-04-28 21:36:51.909823 passive_honeypot-0.1.3/src/passive_honeypot/templates/view_hosts.html
--rw-r--r--   0        0        0     4217 2024-04-28 21:36:51.910823 passive_honeypot-0.1.3/src/passive_honeypot/templates/view_requests.html
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 passive_honeypot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-28 21:46:17.779240 passive_honeypot-0.1.4/LICENSE
+-rw-r--r--   0        0        0      452 2024-04-29 00:10:46.463844 passive_honeypot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6150 2024-04-29 00:10:42.085056 passive_honeypot-0.1.4/src/passive_honeypot/__init__.py
+-rw-r--r--   0        0        0     1733 2024-04-28 21:36:51.904821 passive_honeypot-0.1.4/src/passive_honeypot/config.py
+-rw-r--r--   0        0        0     4555 2024-04-28 21:36:51.905822 passive_honeypot-0.1.4/src/passive_honeypot/database.py
+-rw-r--r--   0        0        0    23461 2024-04-28 16:21:07.363515 passive_honeypot-0.1.4/src/passive_honeypot/favicon.ico
+-rw-r--r--   0        0        0     1508 2024-04-28 21:36:51.907822 passive_honeypot-0.1.4/src/passive_honeypot/templates/home.html
+-rw-r--r--   0        0        0      749 2024-04-28 21:36:51.908825 passive_honeypot-0.1.4/src/passive_honeypot/templates/navbar.html
+-rw-r--r--   0        0        0     2224 2024-04-28 21:36:51.909823 passive_honeypot-0.1.4/src/passive_honeypot/templates/view_hosts.html
+-rw-r--r--   0        0        0     4217 2024-04-28 21:36:51.910823 passive_honeypot-0.1.4/src/passive_honeypot/templates/view_requests.html
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 passive_honeypot-0.1.4/PKG-INFO
```

### Comparing `passive_honeypot-0.1.3/LICENSE` & `passive_honeypot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.3/src/passive_honeypot/__init__.py` & `passive_honeypot-0.1.4/src/passive_honeypot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,34 +42,34 @@
         self.handle_request(*self.unpack_request_values(request))
         return "User-agent: *\nDisallow: /", 200
 
     def admin_index(self) -> Tuple[str, int]:
         if not self._database_handler.host_is_authorized(request.remote_addr):
             return "Unauthorized", 403
 
-        return render_template("templates/home.html"), 200
+        return render_template("passive_honeypot/templates/home.html"), 200
 
     def view_hosts(self) -> Union[Tuple[List[Dict[str, Any]], int], Tuple[str, int]]:
         if not self._database_handler.host_is_authorized(request.remote_addr):
             return "Unauthorized", 403
 
         hosts = self._database_handler.get_remote_hosts()
-        return render_template("templates/view_hosts.html", hosts=hosts), 200
+        return render_template("passive_honeypot/templates/view_hosts.html", hosts=hosts), 200
 
     def view_requests(self) -> Union[Tuple[List[Dict[str, Any]], int], Tuple[str, int]]:
         if not self._database_handler.host_is_authorized(request.remote_addr):
             return "Unauthorized", 403
 
         host = request.args.get("host")
         request_type = request.args.get("type")
         request_type = "all" if (request_type is None or not request_type) else request_type
         if host is None:
             return "Missing host parameter", 400
         requests = self._database_handler.get_requests(host)
-        return render_template("templates/view_requests.html", requests=requests, host=host), 200
+        return render_template("passive_honeypot/templates/view_requests.html", requests=requests, host=host), 200
 
     def add_authorized_host(self):
         if not self._database_handler.host_is_authorized(request.remote_addr):
             return "Unauthorized", 403
 
         host = request.args.get("host") or request.form.get("host")
         if host is None:
```

### Comparing `passive_honeypot-0.1.3/src/passive_honeypot/config.py` & `passive_honeypot-0.1.4/src/passive_honeypot/config.py`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.3/src/passive_honeypot/database.py` & `passive_honeypot-0.1.4/src/passive_honeypot/database.py`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.3/src/passive_honeypot/favicon.ico` & `passive_honeypot-0.1.4/src/passive_honeypot/favicon.ico`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.3/src/passive_honeypot/templates/home.html` & `passive_honeypot-0.1.4/src/passive_honeypot/templates/home.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.3/src/passive_honeypot/templates/navbar.html` & `passive_honeypot-0.1.4/src/passive_honeypot/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.3/src/passive_honeypot/templates/view_hosts.html` & `passive_honeypot-0.1.4/src/passive_honeypot/templates/view_hosts.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.3/src/passive_honeypot/templates/view_requests.html` & `passive_honeypot-0.1.4/src/passive_honeypot/templates/view_requests.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.3/PKG-INFO` & `passive_honeypot-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passive_honeypot
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple passive honeypot written in Python with Flask and psycopg2.
 Author: ottodanp
 Author-email: ottodanp@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```
