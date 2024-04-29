# Comparing `tmp/comfy_script-0.5.0a1.tar.gz` & `tmp/comfy_script-0.5.0a2.tar.gz`

## Comparing `comfy_script-0.5.0a1.tar` & `comfy_script-0.5.0a2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/__init__.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/requirements.txt
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/.vscode/launch.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/README.md
--rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/Runtime.md
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/Transpiler.md
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/Image/README.md
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/Latent/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/Models/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/Nodes/README.md
--rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/README/auto-queue.png
--rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/README/diff.png
--rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/README/plot.png
--rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/README/select.png
--rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/README/type-stubs.png
--rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/README/type-stubs2.png
--rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/README/workflow.png
--rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/README/workflow2.png
--rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/docs/images/Runtime/load-api-format.png
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/__init__.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/astutil.py
--rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/client/__init__.py
--rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/nodes/__init__.py
--rw-r--r--   0        0        0    45421 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/runtime/__init__.py
--rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/runtime/factory.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/runtime/nodes.py
--rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/runtime/data/Images.py
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/runtime/data/__init__.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/runtime/real/__init__.py
--rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/runtime/real/nodes.py
--rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/transpile/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/transpile/__main__.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/transpile/prompt.py
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/transpile/passes/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/ui/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/ui/solara/__init__.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/src/comfy_script/ui/solara/metadata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/tests/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/tests/test_astutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/tests/transpile/__init__.py
--rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/tests/transpile/bypass.json
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/tests/transpile/default.json
--rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/tests/transpile/test_transpiler.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/LICENSE.txt
--rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/README.md
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/pyproject.toml
--rw-r--r--   0        0        0    16183 2020-02-02 00:00:00.000000 comfy_script-0.5.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/__init__.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/requirements.txt
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/.vscode/launch.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/README.md
+-rw-r--r--   0        0        0    18293 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Runtime.md
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Transpiler.md
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Image/README.md
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Latent/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Models/README.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/Nodes/README.md
+-rw-r--r--   0        0        0   839054 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/auto-queue.png
+-rw-r--r--   0        0        0    41490 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/diff.png
+-rw-r--r--   0        0        0   908632 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/plot.png
+-rw-r--r--   0        0        0  2677075 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/select.png
+-rw-r--r--   0        0        0    74672 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/type-stubs.png
+-rw-r--r--   0        0        0    51995 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/type-stubs2.png
+-rw-r--r--   0        0        0    89265 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/workflow.png
+-rw-r--r--   0        0        0   170300 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/README/workflow2.png
+-rw-r--r--   0        0        0   199246 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/docs/images/Runtime/load-api-format.png
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/__init__.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/astutil.py
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/client/__init__.py
+-rw-r--r--   0        0        0     8029 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/nodes/__init__.py
+-rw-r--r--   0        0        0    45421 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/__init__.py
+-rw-r--r--   0        0        0    20573 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/factory.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/nodes.py
+-rw-r--r--   0        0        0     4442 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/data/Images.py
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/data/__init__.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/real/__init__.py
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/runtime/real/nodes.py
+-rw-r--r--   0        0        0    14763 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/transpile/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/transpile/__main__.py
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/transpile/prompt.py
+-rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/transpile/passes/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/ui/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/ui/solara/__init__.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/src/comfy_script/ui/solara/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/test_astutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/transpile/__init__.py
+-rw-r--r--   0        0        0    23060 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/transpile/bypass.json
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/transpile/default.json
+-rw-r--r--   0        0        0     2239 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/tests/transpile/test_transpiler.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/LICENSE.txt
+-rw-r--r--   0        0        0    14501 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/README.md
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/pyproject.toml
+-rw-r--r--   0        0        0    16183 2020-02-02 00:00:00.000000 comfy_script-0.5.0a2/PKG-INFO
```

### Comparing `comfy_script-0.5.0a1/__init__.py` & `comfy_script-0.5.0a2/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/README.md` & `comfy_script-0.5.0a2/docs/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/Runtime.md` & `comfy_script-0.5.0a2/docs/Runtime.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/Image/README.md` & `comfy_script-0.5.0a2/docs/Image/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/Latent/README.md` & `comfy_script-0.5.0a2/docs/Latent/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/Nodes/README.md` & `comfy_script-0.5.0a2/docs/Nodes/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/README/auto-queue.png` & `comfy_script-0.5.0a2/docs/images/README/auto-queue.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/README/diff.png` & `comfy_script-0.5.0a2/docs/images/README/diff.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/README/plot.png` & `comfy_script-0.5.0a2/docs/images/README/plot.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/README/select.png` & `comfy_script-0.5.0a2/docs/images/README/select.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/README/type-stubs.png` & `comfy_script-0.5.0a2/docs/images/README/type-stubs.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/README/type-stubs2.png` & `comfy_script-0.5.0a2/docs/images/README/type-stubs2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/README/workflow.png` & `comfy_script-0.5.0a2/docs/images/README/workflow.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/README/workflow2.png` & `comfy_script-0.5.0a2/docs/images/README/workflow2.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/docs/images/Runtime/load-api-format.png` & `comfy_script-0.5.0a2/docs/images/Runtime/load-api-format.png`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/astutil.py` & `comfy_script-0.5.0a2/src/comfy_script/astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/client/__init__.py` & `comfy_script-0.5.0a2/src/comfy_script/client/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,27 +31,29 @@
 
           e.g. `'http://127.0.0.1:8188/'`
 
         - `session_factory`: A callable factory that returns a new [`aiohttp.ClientSession`](https://docs.aiohttp.org/en/latest/client_reference.html#aiohttp.ClientSession) object. 
 
           e.g. `lambda: aiohttp.ClientSession(auth=aiohttp.BasicAuth('Aladdin', 'open sesame'))`
         '''
+        self.base_url = self._normalize_base_url(base_url)
+
+        # Do not pass base_url to ClientSession, as it only supports absolute URLs without path part
+        self._session_factory = session_factory
+        
+    def _normalize_base_url(self, base_url: str | URL):
         if base_url is None:
             base_url = 'http://127.0.0.1:8188/'
-        elif not isinstance(base_url, str):
+        if not isinstance(base_url, str):
             base_url = str(base_url)
-        
-        if not base_url.startswith('http://'):
+        if not base_url.startswith(('http://', 'https://')):
             base_url = 'http://' + base_url
         if not base_url.endswith('/'):
             base_url += '/'
-        self.base_url = base_url
-
-        # Do not pass base_url to ClientSession, as it only supports absolute URLs without path part
-        self._session_factory = session_factory
+        return base_url
     
     def session(self) -> aiohttp.ClientSession:
         '''Because `aiohttp.ClientSession` is not event-loop-safe (thread-safe), a new session should be created for each request to avoid potential issues. Also, `aiohttp.ClientSession` cannot be closed in a sync manner.'''
         return self._session_factory()
 
 client: Client = Client()
 '''The global client object.'''
```

### Comparing `comfy_script-0.5.0a1/src/comfy_script/nodes/__init__.py` & `comfy_script-0.5.0a2/src/comfy_script/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/runtime/__init__.py` & `comfy_script-0.5.0a2/src/comfy_script/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/runtime/factory.py` & `comfy_script-0.5.0a2/src/comfy_script/runtime/factory.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/runtime/nodes.py` & `comfy_script-0.5.0a2/src/comfy_script/runtime/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/runtime/data/Images.py` & `comfy_script-0.5.0a2/src/comfy_script/runtime/data/Images.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/runtime/data/__init__.py` & `comfy_script-0.5.0a2/src/comfy_script/runtime/data/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/runtime/real/__init__.py` & `comfy_script-0.5.0a2/src/comfy_script/runtime/real/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/runtime/real/nodes.py` & `comfy_script-0.5.0a2/src/comfy_script/runtime/real/nodes.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/transpile/__init__.py` & `comfy_script-0.5.0a2/src/comfy_script/transpile/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/transpile/prompt.py` & `comfy_script-0.5.0a2/src/comfy_script/transpile/prompt.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/transpile/passes/__init__.py` & `comfy_script-0.5.0a2/src/comfy_script/transpile/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/src/comfy_script/ui/solara/metadata.py` & `comfy_script-0.5.0a2/src/comfy_script/ui/solara/metadata.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/tests/test_astutil.py` & `comfy_script-0.5.0a2/tests/test_astutil.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/tests/transpile/bypass.json` & `comfy_script-0.5.0a2/tests/transpile/bypass.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/tests/transpile/default.json` & `comfy_script-0.5.0a2/tests/transpile/default.json`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/tests/transpile/test_transpiler.py` & `comfy_script-0.5.0a2/tests/transpile/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/.gitignore` & `comfy_script-0.5.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/LICENSE.txt` & `comfy_script-0.5.0a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/README.md` & `comfy_script-0.5.0a2/README.md`

 * *Files identical despite different names*

### Comparing `comfy_script-0.5.0a1/pyproject.toml` & `comfy_script-0.5.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "comfy-script"
-version = "0.5.0a1"
+version = "0.5.0a2"
 description = "A Python front end and library for ComfyUI"
 readme = "README.md"
 # ComfyUI: >=3.8
 # comfyui: >=3.9
 # >=3.6 is required to preserve insertion order of input types
 requires-python = ">=3.9"
 authors = [
```

### Comparing `comfy_script-0.5.0a1/PKG-INFO` & `comfy_script-0.5.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comfy-script
-Version: 0.5.0a1
+Version: 0.5.0a2
 Summary: A Python front end and library for ComfyUI
 Project-URL: Homepage, https://github.com/Chaoses-Ib/ComfyScript
 Project-URL: Issues, https://github.com/Chaoses-Ib/ComfyScript/issues
 Author-email: Chaoses-Ib <Chaos-es@outlook.com>
 License-File: LICENSE.txt
 Keywords: comfyui
 Classifier: License :: OSI Approved :: MIT License
```

