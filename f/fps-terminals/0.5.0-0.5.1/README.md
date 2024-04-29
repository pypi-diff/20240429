# Comparing `tmp/fps_terminals-0.5.0.tar.gz` & `tmp/fps_terminals-0.5.1.tar.gz`

## Comparing `fps_terminals-0.5.0.tar` & `fps_terminals-0.5.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/fps_terminals/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/fps_terminals/main.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/fps_terminals/routes.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/fps_terminals/server.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/fps_terminals/win_server.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fps_terminals-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/fps_terminals/main.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/fps_terminals/server.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fps_terminals-0.5.1/PKG-INFO
```

### Comparing `fps_terminals-0.5.0/fps_terminals/main.py` & `fps_terminals-0.5.1/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.0/fps_terminals/routes.py` & `fps_terminals-0.5.1/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.0/fps_terminals/server.py` & `fps_terminals-0.5.1/fps_terminals/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,11 @@
             if self.data_or_disconnect is None:
                 await self.websocket.send_json(["disconnect", 1])
             else:
                 for websocket in self.websockets:
                     await websocket.send_json(["stdout", self.data_or_disconnect])
 
     def quit(self, websocket):
-        self.websockets.remove(websocket)
+        if websocket in self.weksockets:
+            self.websockets.remove(websocket)
         if not self.websockets:
             os.close(self.fd)
```

### Comparing `fps_terminals-0.5.0/fps_terminals/win_server.py` & `fps_terminals-0.5.1/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.0/.gitignore` & `fps_terminals-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.0/COPYING.md` & `fps_terminals-0.5.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.0/pyproject.toml` & `fps_terminals-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.0/PKG-INFO` & `fps_terminals-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_terminals
-Version: 0.5.0
+Version: 0.5.1
 Summary: An FPS plugin for the terminals API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

