# Comparing `tmp/passive_honeypot-0.1.8.tar.gz` & `tmp/passive_honeypot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passive_honeypot-0.1.8.tar", max compression
+gzip compressed data, was "passive_honeypot-0.1.9.tar", max compression
```

## Comparing `passive_honeypot-0.1.8.tar` & `passive_honeypot-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35821 2024-04-28 21:46:17.779240 passive_honeypot-0.1.8/LICENSE
--rw-r--r--   0        0        0      452 2024-04-29 01:00:38.967905 passive_honeypot-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     6069 2024-04-29 00:30:07.525801 passive_honeypot-0.1.8/src/passive_honeypot/__init__.py
--rw-r--r--   0        0        0     1733 2024-04-28 21:36:51.904821 passive_honeypot-0.1.8/src/passive_honeypot/config.py
--rw-r--r--   0        0        0     4684 2024-04-29 01:00:33.384762 passive_honeypot-0.1.8/src/passive_honeypot/database.py
--rw-r--r--   0        0        0    23461 2024-04-28 16:21:07.363515 passive_honeypot-0.1.8/src/passive_honeypot/favicon.ico
--rw-r--r--   0        0        0     1508 2024-04-28 21:36:51.907822 passive_honeypot-0.1.8/src/passive_honeypot/templates/home.html
--rw-r--r--   0        0        0      749 2024-04-28 21:36:51.908825 passive_honeypot-0.1.8/src/passive_honeypot/templates/navbar.html
--rw-r--r--   0        0        0     2224 2024-04-28 21:36:51.909823 passive_honeypot-0.1.8/src/passive_honeypot/templates/view_hosts.html
--rw-r--r--   0        0        0     4217 2024-04-28 21:36:51.910823 passive_honeypot-0.1.8/src/passive_honeypot/templates/view_requests.html
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 passive_honeypot-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35821 2024-04-28 21:46:17.779240 passive_honeypot-0.1.9/LICENSE
+-rw-r--r--   0        0        0      452 2024-04-29 01:05:23.577847 passive_honeypot-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     6069 2024-04-29 00:30:07.525801 passive_honeypot-0.1.9/src/passive_honeypot/__init__.py
+-rw-r--r--   0        0        0     1733 2024-04-28 21:36:51.904821 passive_honeypot-0.1.9/src/passive_honeypot/config.py
+-rw-r--r--   0        0        0     4863 2024-04-29 01:04:43.704260 passive_honeypot-0.1.9/src/passive_honeypot/database.py
+-rw-r--r--   0        0        0    23461 2024-04-28 16:21:07.363515 passive_honeypot-0.1.9/src/passive_honeypot/favicon.ico
+-rw-r--r--   0        0        0     1508 2024-04-28 21:36:51.907822 passive_honeypot-0.1.9/src/passive_honeypot/templates/home.html
+-rw-r--r--   0        0        0      749 2024-04-28 21:36:51.908825 passive_honeypot-0.1.9/src/passive_honeypot/templates/navbar.html
+-rw-r--r--   0        0        0     2224 2024-04-28 21:36:51.909823 passive_honeypot-0.1.9/src/passive_honeypot/templates/view_hosts.html
+-rw-r--r--   0        0        0     4217 2024-04-28 21:36:51.910823 passive_honeypot-0.1.9/src/passive_honeypot/templates/view_requests.html
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 passive_honeypot-0.1.9/PKG-INFO
```

### Comparing `passive_honeypot-0.1.8/LICENSE` & `passive_honeypot-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.8/src/passive_honeypot/__init__.py` & `passive_honeypot-0.1.9/src/passive_honeypot/__init__.py`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.8/src/passive_honeypot/config.py` & `passive_honeypot-0.1.9/src/passive_honeypot/config.py`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.8/src/passive_honeypot/database.py` & `passive_honeypot-0.1.9/src/passive_honeypot/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,17 @@
     def get_remote_hosts(self) -> List[Dict[str, Any]]:
         # return all hosts except for authorized hosts
         self.execute("SELECT remote_host FROM remote_hosts")
         hosts = self.fetchall()
         r = []
         for row in hosts:
             host = row[0]
+            print(host)
             if self.host_is_authorized(host):
+                print("host is authorized")
                 continue
             valid, invalid = self.count_requests(host)
             r.append({
                 "host": host,
                 "valid_requests": valid,
                 "invalid_requests": invalid,
                 "total_requests": valid + invalid
@@ -95,15 +97,17 @@
                 "timestamp": timestamp,
                 "port": port
             })
 
         return r
 
     def host_is_authorized(self, host: str) -> bool:
-        self.execute("SELECT EXISTS(SELECT 1 FROM remote_hosts WHERE remote_host = %s)", (host,))
+        self.execute(
+            "SELECT EXISTS(SELECT remote_host_id FROM authorized_hosts WHERE remote_host_id = (SELECT remote_host_id FROM remote_hosts WHERE remote_host = %s))",
+            (host,))
         return self.fetchone()[0]
 
     def add_authorized_host(self, host: str):
         if not self.remote_host_exists(host):
             self.insert_remote_host(host)
             self._conn.commit()
```

### Comparing `passive_honeypot-0.1.8/src/passive_honeypot/favicon.ico` & `passive_honeypot-0.1.9/src/passive_honeypot/favicon.ico`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.8/src/passive_honeypot/templates/home.html` & `passive_honeypot-0.1.9/src/passive_honeypot/templates/home.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.8/src/passive_honeypot/templates/navbar.html` & `passive_honeypot-0.1.9/src/passive_honeypot/templates/navbar.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.8/src/passive_honeypot/templates/view_hosts.html` & `passive_honeypot-0.1.9/src/passive_honeypot/templates/view_hosts.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.8/src/passive_honeypot/templates/view_requests.html` & `passive_honeypot-0.1.9/src/passive_honeypot/templates/view_requests.html`

 * *Files identical despite different names*

### Comparing `passive_honeypot-0.1.8/PKG-INFO` & `passive_honeypot-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passive_honeypot
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple passive honeypot written in Python with Flask and psycopg2.
 Author: ottodanp
 Author-email: ottodanp@example.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

