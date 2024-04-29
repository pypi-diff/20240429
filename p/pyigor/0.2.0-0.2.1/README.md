# Comparing `tmp/pyigor-0.2.0.tar.gz` & `tmp/pyigor-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyigor-0.2.0.tar", last modified: Thu Apr  4 13:20:19 2024, max compression
+gzip compressed data, was "pyigor-0.2.1.tar", last modified: Mon Apr 29 06:48:55 2024, max compression
```

## Comparing `pyigor-0.2.0.tar` & `pyigor-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-04 13:20:19.484627 pyigor-0.2.0/
--rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 pyigor-0.2.0/LICENSE.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       26 2023-01-22 05:57:41.000000 pyigor-0.2.0/MANIFEST.in
--rw-r--r--   0 shuntaro   (501) staff       (20)     2360 2024-04-04 13:20:19.484569 pyigor-0.2.0/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)     1553 2024-04-04 10:54:26.000000 pyigor-0.2.0/README.md
--rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 pyigor-0.2.0/pyproject.toml
--rw-r--r--   0 shuntaro   (501) staff       (20)      899 2024-04-04 13:20:19.484875 pyigor-0.2.0/setup.cfg
--rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 pyigor-0.2.0/setup.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-04 13:20:19.481792 pyigor-0.2.0/src/
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-04 13:20:19.483451 pyigor-0.2.0/src/pyigor/
--rw-r--r--   0 shuntaro   (501) staff       (20)       36 2023-01-22 05:51:31.000000 pyigor-0.2.0/src/pyigor/__init__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)      276 2023-10-31 01:21:18.000000 pyigor-0.2.0/src/pyigor/__main__.py
--rw-r--r--   0 shuntaro   (501) staff       (20)     7148 2024-04-04 11:01:30.000000 pyigor-0.2.0/src/pyigor/pyigor.py
-drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-04 13:20:19.484365 pyigor-0.2.0/src/pyigor.egg-info/
--rw-r--r--   0 shuntaro   (501) staff       (20)     2360 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/PKG-INFO
--rw-r--r--   0 shuntaro   (501) staff       (20)      303 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/SOURCES.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/dependency_links.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)       21 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/requires.txt
--rw-r--r--   0 shuntaro   (501) staff       (20)        7 2024-04-04 13:20:19.000000 pyigor-0.2.0/src/pyigor.egg-info/top_level.txt
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-29 06:48:55.017196 pyigor-0.2.1/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     1075 2023-01-22 05:52:37.000000 pyigor-0.2.1/LICENSE.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       26 2023-01-22 05:57:41.000000 pyigor-0.2.1/MANIFEST.in
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2936 2024-04-29 06:48:55.017129 pyigor-0.2.1/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2055 2024-04-29 06:42:41.000000 pyigor-0.2.1/README.md
+-rw-r--r--   0 shuntaro   (501) staff       (20)       94 2023-01-22 06:54:48.000000 pyigor-0.2.1/pyproject.toml
+-rw-r--r--   0 shuntaro   (501) staff       (20)      961 2024-04-29 06:48:55.017702 pyigor-0.2.1/setup.cfg
+-rw-r--r--   0 shuntaro   (501) staff       (20)       37 2022-12-09 19:04:39.000000 pyigor-0.2.1/setup.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-29 06:48:55.013812 pyigor-0.2.1/src/
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-29 06:48:55.015697 pyigor-0.2.1/src/pyigor/
+-rw-r--r--   0 shuntaro   (501) staff       (20)       36 2023-01-22 05:51:31.000000 pyigor-0.2.1/src/pyigor/__init__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)      276 2023-10-31 01:21:18.000000 pyigor-0.2.1/src/pyigor/__main__.py
+-rw-r--r--   0 shuntaro   (501) staff       (20)     8195 2024-04-29 06:37:02.000000 pyigor-0.2.1/src/pyigor/pyigor.py
+drwxr-xr-x   0 shuntaro   (501) staff       (20)        0 2024-04-29 06:48:55.016870 pyigor-0.2.1/src/pyigor.egg-info/
+-rw-r--r--   0 shuntaro   (501) staff       (20)     2936 2024-04-29 06:48:55.000000 pyigor-0.2.1/src/pyigor.egg-info/PKG-INFO
+-rw-r--r--   0 shuntaro   (501) staff       (20)      303 2024-04-29 06:48:55.000000 pyigor-0.2.1/src/pyigor.egg-info/SOURCES.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        1 2024-04-29 06:48:55.000000 pyigor-0.2.1/src/pyigor.egg-info/dependency_links.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)       32 2024-04-29 06:48:55.000000 pyigor-0.2.1/src/pyigor.egg-info/requires.txt
+-rw-r--r--   0 shuntaro   (501) staff       (20)        7 2024-04-29 06:48:55.000000 pyigor-0.2.1/src/pyigor.egg-info/top_level.txt
```

### Comparing `pyigor-0.2.0/LICENSE.txt` & `pyigor-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyigor-0.2.0/PKG-INFO` & `pyigor-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyigor
-Version: 0.2.0
-Summary: Bridging between Python and Igor Pro
+Version: 0.2.1
+Summary: Seamlessly integrate Python with WaveMetrics Igor Pro for data and command exchange.
 Home-page: https://github.com/chocolate-icecream/pyigor
 Author: chocolate-icecream
 Project-URL: Bug Tracker, https://github.com/chocolate-icecream/pyigor/issues
 Keywords: Igor
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
@@ -15,74 +15,84 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: flask>=2.1
 Requires-Dist: h5py>=3.0
+Requires-Dist: numpy>=1.0
 
 # PyIgor
 
-PyIgor bridges between Python and WaveMetrics Igor Pro.
+PyIgor facilitates communication between Python and WaveMetrics Igor Pro, enabling seamless data and command exchange.
 
-## Preparation
+## Requirements
 
-- Igor Pro 7.0 or later
-- HDF5 XOP installation (See HDF5 installation in Igor Pro's help topics for the detail).
-- Load pyigor.ipf (https://github.com/chocolate-icecream/pyigor/blob/master/pyigor.ipf).
+- **Igor Pro 7.0 or later:** Ensure you have Igor Pro 7.0 or a newer version installed.
+- **HDF5 XOP:** Install the HDF5 XOP module. Detailed installation instructions are available in the "HDF5 installation" section under Igor Pro's help topics.
+- **PyIgor Procedure File:** Download the `pyigor.ipf` file from [GitHub](https://github.com/chocolate-icecream/pyigor/blob/master/pyigor.ipf) and place it in the Igor Procedures folder for convenience.
 
-  Putting it in the Igor Procedures folder is very convenient.
+## Installation
+
+To install PyIgor, use the following pip command:
+
+```bash
+pip install pyigor
+```
 
 ## Usage
 
-#### Accessing Igor Pro from Python
+### Accessing Igor Pro from Python
+
+Here’s how you can interact with Igor Pro using PyIgor:
 
 ```python
 from pyigor import Connection
 import numpy as np
 
+# Establish a connection with Igor Pro
 igor = Connection()
 
-### Sending an array to Igor Pro
+# Send a numpy array to Igor Pro
 array = np.sin(np.linspace(0, 10, 100))
 igor.put(array, "sinwave")
 
-### Executing a command in Igor Pro
+# Execute a command in Igor Pro
 igor("sinwave += 1")
 
-### Getting a wave from Igor Pro
+# Retrieve a wave from Igor Pro
 wv = igor.get("sinwave")
 print(wv.array)
 ```
 
-#### Accessing Python from Igor Pro
+### Accessing Python from Igor Pro
 
-###### Preparation in Python
+#### Preparing Python
 
 ```python
 from pyigor import Connection
 
+# Establish a connection
 igor = Connection()
 
-### @igor.function decorator makes the function callable from Igor Pro.
+# Register a function callable from Igor Pro
 @igor.function 
 def myfunc(a):
-	return a*a
+    return a * a
 
-igor.wait_done() # Just to prevent the program quit. You don't need it in the interactive mode.
+# Keep the connection open; not required in interactive mode
+igor.wait_done()
 ```
 
-By using Connection(security_hole=True), you can call any Python code. Meanwhile, this option makes it possible to execute any Python code by HTTP requests: http://localhost/code -> `eval(code)`. Do not use unless you are sure of it.
+Use the `Connection(security_hole=True)` to call any Python code from Igor Pro. This setting allows executing Python code through HTTP requests to `http://localhost/code` using `eval(code)`. **Important:** Use this option only if you understand the security implications.
 
-###### Calling registered functions from Igor Pro
+#### Calling Python Functions from Igor Pro
+
+Execute Python functions registered via PyIgor from Igor Pro:
 
 ```
 print PyIgorCall("myfunc(10)")
 ```
 
+## Security Note
 
-
-## Contributors
-
-A special thanks to the people who have contributed to this project:
-\- [@nlyamada](https://github.com/nlyamada) - Made compatible with Windows
-
+When enabling `security_hole=True`, ensure your environment is secure and understand the risks associated with executing arbitrary code.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyigor-0.2.0/README.md` & `pyigor-0.2.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,75 @@
 # PyIgor
 
-PyIgor bridges between Python and WaveMetrics Igor Pro.
+PyIgor facilitates communication between Python and WaveMetrics Igor Pro, enabling seamless data and command exchange.
 
-## Preparation
+## Requirements
 
-- Igor Pro 7.0 or later
-- HDF5 XOP installation (See HDF5 installation in Igor Pro's help topics for the detail).
-- Load pyigor.ipf (https://github.com/chocolate-icecream/pyigor/blob/master/pyigor.ipf).
+- **Igor Pro 7.0 or later:** Ensure you have Igor Pro 7.0 or a newer version installed.
+- **HDF5 XOP:** Install the HDF5 XOP module. Detailed installation instructions are available in the "HDF5 installation" section under Igor Pro's help topics.
+- **PyIgor Procedure File:** Download the `pyigor.ipf` file from [GitHub](https://github.com/chocolate-icecream/pyigor/blob/master/pyigor.ipf) and place it in the Igor Procedures folder for convenience.
 
-  Putting it in the Igor Procedures folder is very convenient.
+## Installation
+
+To install PyIgor, use the following pip command:
+
+```bash
+pip install pyigor
+```
 
 ## Usage
 
-#### Accessing Igor Pro from Python
+### Accessing Igor Pro from Python
+
+Here’s how you can interact with Igor Pro using PyIgor:
 
 ```python
 from pyigor import Connection
 import numpy as np
 
+# Establish a connection with Igor Pro
 igor = Connection()
 
-### Sending an array to Igor Pro
+# Send a numpy array to Igor Pro
 array = np.sin(np.linspace(0, 10, 100))
 igor.put(array, "sinwave")
 
-### Executing a command in Igor Pro
+# Execute a command in Igor Pro
 igor("sinwave += 1")
 
-### Getting a wave from Igor Pro
+# Retrieve a wave from Igor Pro
 wv = igor.get("sinwave")
 print(wv.array)
 ```
 
-#### Accessing Python from Igor Pro
+### Accessing Python from Igor Pro
 
-###### Preparation in Python
+#### Preparing Python
 
 ```python
 from pyigor import Connection
 
+# Establish a connection
 igor = Connection()
 
-### @igor.function decorator makes the function callable from Igor Pro.
+# Register a function callable from Igor Pro
 @igor.function 
 def myfunc(a):
-	return a*a
+    return a * a
 
-igor.wait_done() # Just to prevent the program quit. You don't need it in the interactive mode.
+# Keep the connection open; not required in interactive mode
+igor.wait_done()
 ```
 
-By using Connection(security_hole=True), you can call any Python code. Meanwhile, this option makes it possible to execute any Python code by HTTP requests: http://localhost/code -> `eval(code)`. Do not use unless you are sure of it.
+Use the `Connection(security_hole=True)` to call any Python code from Igor Pro. This setting allows executing Python code through HTTP requests to `http://localhost/code` using `eval(code)`. **Important:** Use this option only if you understand the security implications.
 
-###### Calling registered functions from Igor Pro
+#### Calling Python Functions from Igor Pro
+
+Execute Python functions registered via PyIgor from Igor Pro:
 
 ```
 print PyIgorCall("myfunc(10)")
 ```
 
+## Security Note
 
-
-## Contributors
-
-A special thanks to the people who have contributed to this project:
-\- [@nlyamada](https://github.com/nlyamada) - Made compatible with Windows
-
+When enabling `security_hole=True`, ensure your environment is secure and understand the risks associated with executing arbitrary code.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyigor-0.2.0/setup.cfg` & `pyigor-0.2.1/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = pyigor
-version = 0.2.0
+version = 0.2.1
 author = chocolate-icecream
-description = Bridging between Python and Igor Pro
+description = Seamlessly integrate Python with WaveMetrics Igor Pro for data and command exchange.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chocolate-icecream/pyigor
 project_urls = 
 	Bug Tracker = https://github.com/chocolate-icecream/pyigor/issues
 classifiers = 
 	Programming Language :: Python :: 3
@@ -25,14 +25,15 @@
 	= src
 packages = find:
 include_package_data = True
 python_requires = >=3.6
 install_requires = 
 	flask >= 2.1
 	h5py >= 3.0
+	numpy >= 1.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyigor-0.2.0/src/pyigor/pyigor.py` & `pyigor-0.2.1/src/pyigor/pyigor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import os
 import logging
 import threading
 import queue
 import uuid
 import subprocess
 import re, ast, json, glob, platform
+from typing import List
 
 import flask
 from flask import Flask
 import h5py
+import numpy as np
 
 my_platform = "mac" if platform.platform(terse=True).startswith("macOS") else ("windows" if platform.platform(terse=True).startswith("Windows") else None)
 
 def alphanumeric_sort(l):
     convert = lambda text: int(text) if text.isdigit() else text.lower()
     alphanum_key = lambda key: [convert(c) for c in re.split('([0-9]+)', key)]
     return sorted(l, key=alphanum_key, reverse=True)
 
 ##### OS dependent codes #####
 def find_executable_path():
-    exe_path_dict = {   "mac": "/Applications/Igor Pro * Folder/Igor64.app/Contents/MacOS/Igor64",
-                        "windows": "C:\Program Files\WaveMetrics\Igor Pro * Folder\IgorBinaries_x64\Igor64.exe"}
+    exe_path_dict = {"mac": os.path.join("/Applications", "Igor Pro * Folder", "Igor64.app", "Contents", "MacOS", "Igor64"),
+                    "windows": os.path.join("C:", "Program Files", "WaveMetrics", "Igor Pro * Folder", "IgorBinaries_x64", "Igor64.exe")}
 
     path_candidates = glob.glob(exe_path_dict[my_platform])
     assert len(path_candidates) > 0, "Cannot find Igor Pro"
 
     exe_path = alphanumeric_sort(path_candidates)[0] # get the newest version
     return exe_path
 
@@ -41,29 +43,29 @@
 
 
 class Connection:
     TIMEOUT = 3
     ### security_hole options makes it possible to execute any Python code by HTTP requests. Do not use unless you are sure of it.
     def __init__(self, port=15556, security_hole=False, timeout=3):
         self._app = Flask(__name__)
-        self._task_queue = queue.Queue(maxsize=1)
-        self._queue = queue.Queue(maxsize=1)
+        self._task_queue = queue.Queue(maxsize=1) # set of (command, uid)
+        self._queue = queue.Queue(maxsize=1) # set of (status, uid, data_dict or None)
         self._port = port
         self._registered_functions = {"get": self.get, "put": self.put, "print": print}
         self._basepath = os.getcwd()
         self._executable_path = find_executable_path()
         self._security_hole = security_hole
         self.TIMEOUT = timeout
         
         self._register_route()
         threading.Thread(target=self._run_server, daemon=True).start()
 
     def reset(self):
         try:
-            self._queue.put_nowait(("error", 0))
+            self._queue.put_nowait(("error", 0, None))
         except:
             pass
         try:
             self._queue.get_nowait()
         except:
             pass
         try:
@@ -127,17 +129,17 @@
 
         @self._app.route("/msg/<string:msg>/<string:uid>")
         def got_message(msg, uid):
             if msg == "get":
                 result = self._process_get(uid)
                 self._queue.put_nowait(result)
             if msg == "put":
-                self._queue.put_nowait(("ok", uid))
+                self._queue.put_nowait(("ok", uid, None))
             if msg == "error":
-                self._queue.put_nowait(("error", uid))
+                self._queue.put_nowait(("error", uid, None))
             return "<p>Bridging Igor and Python</p>"
 
         @self._app.route("/call/<string:commands>")
         def call_command(commands):
             result_list = []
             p = re.compile(r"([\w]+)\(([^\)]*)\)")
             for command in commands.split(";"):
@@ -156,14 +158,21 @@
                     print(e)
                     result_list.append(f"error:{command}")
             return ";".join([str(x) for x in result_list if x is not None])
 
     def _process_get(self, uid):
         with h5py.File(self._temp_path(), mode="r") as f:
             result_dict = {"array": f[uid][...]}
+            attrs = f[uid].attrs
+            if "IGORWaveScaling" in attrs:
+                result_dict["offsets"] = list(attrs["IGORWaveScaling"][1:, 1])
+                result_dict["deltas"] = list(attrs["IGORWaveScaling"][1:, 0])
+            else: # IGORWaveScaling is omitted for default parameters
+                result_dict["offsets"] = [0.0] * len(result_dict["array"].shape)
+                result_dict["deltas"] = [1.0] * len(result_dict["array"].shape)
         return ("ok", uid, result_dict)
     
     def _temp_path(self, for_igor=False):
         path = os.path.join(self._basepath, f"temp_pyigor_{self._port}.h5")
         if for_igor:
             path = convert_to_igor_path(path)
         return path
@@ -184,21 +193,39 @@
     def function(self, f):
         def wrapper(*args, **kwargs):
             return f(*args, **kwargs)
         self._registered_functions[f.__name__] == f
         return wrapper
 
 class Wave:
-    def __init__(self, array):
+    def __init__(self, array, offsets: List[float], deltas: List[float], units: str=""):
+        if isinstance(array, list):
+            array = np.array(list)
         self.array = array
-        self.offset = [0]
-        self.delta = [1]
-        self.units = [None]
+        self.offsets = offsets
+        self.deltas = deltas
+        self.units = units
     
     @classmethod
     def from_dict(cls, d):
-        wave = Wave(d["array"])
+        wave = Wave(**d)
         return wave
-    
-    def __str__(self):
-        return f"<Wave shape:{self.array.shape}, data_type:{self.array.dtype}>"
+
+    @property
+    def shape(self):
+        return self.array.shape
+
+    @property
+    def numpnts(self):
+        return self.array.size
+    
+    @property
+    def deltax(self):
+        return self.deltas[0]
+
+    @property
+    def leftx(self):
+        return self.offsets[0]
+
+    def __repr__(self):
+        return f"<pyigor.Wave shape: {self.shape}, data_type: {self.array.dtype}>"
```

### Comparing `pyigor-0.2.0/src/pyigor.egg-info/PKG-INFO` & `pyigor-0.2.1/src/pyigor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyigor
-Version: 0.2.0
-Summary: Bridging between Python and Igor Pro
+Version: 0.2.1
+Summary: Seamlessly integrate Python with WaveMetrics Igor Pro for data and command exchange.
 Home-page: https://github.com/chocolate-icecream/pyigor
 Author: chocolate-icecream
 Project-URL: Bug Tracker, https://github.com/chocolate-icecream/pyigor/issues
 Keywords: Igor
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
@@ -15,74 +15,84 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: flask>=2.1
 Requires-Dist: h5py>=3.0
+Requires-Dist: numpy>=1.0
 
 # PyIgor
 
-PyIgor bridges between Python and WaveMetrics Igor Pro.
+PyIgor facilitates communication between Python and WaveMetrics Igor Pro, enabling seamless data and command exchange.
 
-## Preparation
+## Requirements
 
-- Igor Pro 7.0 or later
-- HDF5 XOP installation (See HDF5 installation in Igor Pro's help topics for the detail).
-- Load pyigor.ipf (https://github.com/chocolate-icecream/pyigor/blob/master/pyigor.ipf).
+- **Igor Pro 7.0 or later:** Ensure you have Igor Pro 7.0 or a newer version installed.
+- **HDF5 XOP:** Install the HDF5 XOP module. Detailed installation instructions are available in the "HDF5 installation" section under Igor Pro's help topics.
+- **PyIgor Procedure File:** Download the `pyigor.ipf` file from [GitHub](https://github.com/chocolate-icecream/pyigor/blob/master/pyigor.ipf) and place it in the Igor Procedures folder for convenience.
 
-  Putting it in the Igor Procedures folder is very convenient.
+## Installation
+
+To install PyIgor, use the following pip command:
+
+```bash
+pip install pyigor
+```
 
 ## Usage
 
-#### Accessing Igor Pro from Python
+### Accessing Igor Pro from Python
+
+Here’s how you can interact with Igor Pro using PyIgor:
 
 ```python
 from pyigor import Connection
 import numpy as np
 
+# Establish a connection with Igor Pro
 igor = Connection()
 
-### Sending an array to Igor Pro
+# Send a numpy array to Igor Pro
 array = np.sin(np.linspace(0, 10, 100))
 igor.put(array, "sinwave")
 
-### Executing a command in Igor Pro
+# Execute a command in Igor Pro
 igor("sinwave += 1")
 
-### Getting a wave from Igor Pro
+# Retrieve a wave from Igor Pro
 wv = igor.get("sinwave")
 print(wv.array)
 ```
 
-#### Accessing Python from Igor Pro
+### Accessing Python from Igor Pro
 
-###### Preparation in Python
+#### Preparing Python
 
 ```python
 from pyigor import Connection
 
+# Establish a connection
 igor = Connection()
 
-### @igor.function decorator makes the function callable from Igor Pro.
+# Register a function callable from Igor Pro
 @igor.function 
 def myfunc(a):
-	return a*a
+    return a * a
 
-igor.wait_done() # Just to prevent the program quit. You don't need it in the interactive mode.
+# Keep the connection open; not required in interactive mode
+igor.wait_done()
 ```
 
-By using Connection(security_hole=True), you can call any Python code. Meanwhile, this option makes it possible to execute any Python code by HTTP requests: http://localhost/code -> `eval(code)`. Do not use unless you are sure of it.
+Use the `Connection(security_hole=True)` to call any Python code from Igor Pro. This setting allows executing Python code through HTTP requests to `http://localhost/code` using `eval(code)`. **Important:** Use this option only if you understand the security implications.
 
-###### Calling registered functions from Igor Pro
+#### Calling Python Functions from Igor Pro
+
+Execute Python functions registered via PyIgor from Igor Pro:
 
 ```
 print PyIgorCall("myfunc(10)")
 ```
 
+## Security Note
 
-
-## Contributors
-
-A special thanks to the people who have contributed to this project:
-\- [@nlyamada](https://github.com/nlyamada) - Made compatible with Windows
-
+When enabling `security_hole=True`, ensure your environment is secure and understand the risks associated with executing arbitrary code.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

