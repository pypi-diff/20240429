# Comparing `tmp/pop_cli-4.3.1.tar.gz` & `tmp/pop_cli-5.1.0.tar.gz`

## Comparing `pop_cli-4.3.1.tar` & `pop_cli-5.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-4.3.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     1087 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/__main__.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/config.yaml
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/cli.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/config.py
--rw-r--r--   0        0        0     6863 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/console.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/init.py
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/ref.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-4.3.1/src/hub/state.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_init.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_ref.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-4.3.1/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-4.3.1/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-4.3.1/README.rst
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pop_cli-4.3.1/pyproject.toml
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 pop_cli-5.1.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      881 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/__main__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/config.yaml
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/hub/cli.py
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/hub/completer.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/hub/config.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/hub/console.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/hub/init.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/hub/ref.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 pop_cli-5.1.0/src/hub/state.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-5.1.0/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-5.1.0/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-5.1.0/README.rst
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 pop_cli-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 pop_cli-5.1.0/PKG-INFO
```

### Comparing `pop_cli-4.3.1/.pre-commit-config.yaml` & `pop_cli-5.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/src/__main__.py` & `pop_cli-5.1.0/src/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,13 @@
 import asyncio
 
 import cpop.hub
 
-try:
-    import uvloop
-
-    HAS_UVLOOP = True
-except ImportError:
-    HAS_UVLOOP = False
-
 
 def main():
-    # Initialize the event loop
-    if HAS_UVLOOP:
-        asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
-
     # Set the event loop
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
 
     # Start the async code
     try:
         asyncio.run(amain(loop))
```

### Comparing `pop_cli-4.3.1/src/config.yaml` & `pop_cli-5.1.0/src/config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -40,18 +40,21 @@
 dyne:
   cli:
     - hub
 
 # python imports to put on the hub for this plugin
 import:
   - aioconsole
+  - aioconsole.console
+  - aioconsole.server
   - aiopath
   - asyncio
   - ast
   - builtins
+  - functools
   - pdb
   - pickle
   - pprint
   - prompt_toolkit
   - readline
   - rlcompleter
   - sys
```

### Comparing `pop_cli-4.3.1/src/hub/cli.py` & `pop_cli-5.1.0/src/hub/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/src/hub/config.py` & `pop_cli-5.1.0/src/hub/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/src/hub/init.py` & `pop_cli-5.1.0/src/hub/init.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,17 +53,17 @@
         if isinstance(finder, hub.lib.cpop.contract.Contracted):
             finder = finder.func
         ret = help(finder)
     else:
         # Call or retrieve the object at the given ref
         ret = await hub.cli.ref.resolve(finder, *args, **kwargs)
 
-        # output the results of finder to the console
-        await hub.cli.ref.output(ret)
-
     if opt.cli.interactive:
         # Start an asynchronous interactive console
-        await hub.cli.console.run(opt=opt, ref=finder)
+        await hub.cli.console.run(opt=opt, ref=finder, ret=ret)
+    else:
+        # output the results of finder to the console
+        await hub.cli.ref.output(ret)
 
     if hub_state_file:
         # Write the serialized hub to a file
         hub_state_file = await hub.cli.state.save(hub_state_file)
```

### Comparing `pop_cli-4.3.1/src/hub/ref.py` & `pop_cli-5.1.0/src/hub/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/src/hub/state.py` & `pop_cli-5.1.0/src/hub/state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/tests/conftest.py` & `pop_cli-5.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/tests/integration/test_cli.py` & `pop_cli-5.1.0/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/tests/integration/test_config.py` & `pop_cli-5.1.0/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/tests/integration/test_console.py` & `pop_cli-5.1.0/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/tests/integration/test_init.py` & `pop_cli-5.1.0/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/tests/integration/test_ref.py` & `pop_cli-5.1.0/tests/integration/test_ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/tests/integration/test_state.py` & `pop_cli-5.1.0/tests/integration/test_state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/.gitignore` & `pop_cli-5.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/README.rst` & `pop_cli-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-4.3.1/pyproject.toml` & `pop_cli-5.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "4.3.1"
+version = "5.1.0"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `pop_cli-4.3.1/PKG-INFO` & `pop_cli-5.1.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 4.3.1
+Version: 5.1.0
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

