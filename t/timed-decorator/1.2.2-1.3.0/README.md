# Comparing `tmp/timed_decorator-1.2.2.tar.gz` & `tmp/timed_decorator-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timed_decorator-1.2.2.tar", last modified: Sat Apr 27 18:24:58 2024, max compression
+gzip compressed data, was "timed_decorator-1.3.0.tar", last modified: Mon Apr 29 10:43:09 2024, max compression
```

## Comparing `timed_decorator-1.2.2.tar` & `timed_decorator-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:58.305111 timed_decorator-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-27 18:24:58.305111 timed_decorator-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9868 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:24:58.305111 timed_decorator-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:58.305111 timed_decorator-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/tests/test_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:58.305111 timed_decorator-1.2.2/timed_decorator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/timed_decorator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/timed_decorator/nested_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/timed_decorator/simple_timed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-27 18:24:53.000000 timed_decorator-1.2.2/timed_decorator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:24:58.305111 timed_decorator-1.2.2/timed_decorator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-04-27 18:24:58.000000 timed_decorator-1.2.2/timed_decorator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-27 18:24:58.000000 timed_decorator-1.2.2/timed_decorator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:24:58.000000 timed_decorator-1.2.2/timed_decorator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-27 18:24:58.000000 timed_decorator-1.2.2/timed_decorator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-27 18:24:58.000000 timed_decorator-1.2.2/timed_decorator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:09.254914 timed_decorator-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-29 10:43:09.254914 timed_decorator-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:43:09.254914 timed_decorator-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:09.250914 timed_decorator-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/tests/test_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:09.250914 timed_decorator-1.3.0/timed_decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/timed_decorator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/timed_decorator/nested_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/timed_decorator/simple_timed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-29 10:43:04.000000 timed_decorator-1.3.0/timed_decorator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:43:09.254914 timed_decorator-1.3.0/timed_decorator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 10:43:09.000000 timed_decorator-1.3.0/timed_decorator.egg-info/top_level.txt
```

### Comparing `timed_decorator-1.2.2/LICENSE` & `timed_decorator-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timed_decorator-1.2.2/PKG-INFO` & `timed_decorator-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.2.2
+Version: 1.3.0
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2024 George Stoica
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -25,28 +25,30 @@
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: repository, https://github.com/ancestor-mithril/timed-decorator
 Keywords: timing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 
 # timed-decorator
 
 ## Installation
 
 ```
-pip install timed-decorator
+pip install --upgrade timed-decorator
 ```
 
 ## Usage
 
 Attach it to the function you want to time and run the application. 
 
 ```py
@@ -63,17 +65,19 @@
     y_squared = (b ** 2).sum(dim=1)
     return x_squared.unsqueeze(-1) + y_squared.unsqueeze(0) - 2 * diff
 
 
 a = torch.rand((10000, 800))
 b = torch.rand((12000, 800))
 batched_euclidean_distance(a, b)
-a = a.cuda()
-b = b.cuda()
-batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
+
+if torch.cuda.is_available():
+    a = a.cuda()
+    b = b.cuda()
+    batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
 ```
 Prints:
 ```
 batched_euclidean_distance(CpuTensor[10000, 800], CpuTensor[12000, 800]) -> total time: 685659400ns
 batched_euclidean_distance(CudaTensor[10000, 800], CudaTensor[12000, 800]) -> total time: 260411900ns
 ```
 
@@ -84,19 +88,21 @@
     * `disable_gc` (`bool`): If `True`, disabled garbage collection during function execution. Default: `False`.
     * `use_seconds` (`bool`): If `True`, displays the elapsed time in seconds. Default: `False`.
     * `precision` (`int`): Used in conjunction with `use_seconds`, represents the decimal points used for printing seconds. Default: `9`.
     * `show_args` (`bool`): If `True`, displays the function arguments according to `display_level`. Useful when timing function calls with arguments of different magnitude. Default: `False`.
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
-    * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Can't be used in conjunction with `logger_name`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
-    * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`. See [Using a logger](#using-a-logger).
-    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as key. If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict)
+    * `stdout` (`bool`): If `True`, writes the elapsed time to stdout. Default: `True`.
+    * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Default: `None`.
+    * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
+    * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
+    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as key. If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
 
-2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after substracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
+2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 ### Examples
 
 Simple usage.
 ```py
 from timed_decorator.simple_timed import timed
 
@@ -107,15 +113,35 @@
     a, b = 0, 1
     for _ in range(n):
         a, b = b, a + b
     return a
 
 
 fibonacci(10000)
-# fibonacci() -> total time: 2114100ns
+# fibonacci() -> total time: 1114100ns
+```
+
+Getting both the function's return value and the elapsed time.
+```py
+from timed_decorator.simple_timed import timed
+
+
+@timed(return_time=True)
+def fibonacci(n: int) -> int:
+    assert n > 0
+    a, b = 0, 1
+    for _ in range(n):
+        a, b = b, a + b
+    return a
+
+
+value, elapsed = fibonacci(10000)
+print(f'10000th fibonacci number has {len(str(value))} digits. Calculating it took {elapsed}ns.')
+# fibonacci() -> total time: 1001200ns
+# 10000th fibonacci number has 2090 digits. Calculating it took 1001200ns.
 ```
 
 Set `collect_gc=False` to disable pre-collection of garbage.
 
 ```py
 from timed_decorator.simple_timed import timed
 
@@ -126,15 +152,15 @@
     a, b = 0, 1
     for _ in range(n):
         a, b = b, a + b
     return a
 
 
 fibonacci(10000)
-# fibonacci() -> total time: 2062400ns
+# fibonacci() -> total time: 1062400ns
 ```
 
 Using seconds instead of nanoseconds. 
 ```py
 from timed_decorator.simple_timed import timed
 
 
@@ -149,15 +175,15 @@
         return recursive_fibonacci(n - 1) + recursive_fibonacci(n - 2)
     if n == 1:
         return 0
     return 1
 
 
 call_recursive_fibonacci(30)
-# call_recursive_fibonacci() -> total time: 0.098s
+# call_recursive_fibonacci() -> total time: 0.045s
 ```
 
 Displaying function parameters:
 ```py
 from timed_decorator.simple_timed import timed
 import numpy as np
 
@@ -340,15 +366,15 @@
 
 from timed_decorator.simple_timed import timed
 
 logging.basicConfig()
 logging.root.setLevel(logging.NOTSET)
 
 
-@timed(logger_name='TEST_LOGGER')
+@timed(logger_name='TEST_LOGGER', stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 fn()
 ```
@@ -368,15 +394,15 @@
 
 log_stream = StringIO()
 log_handler = logging.StreamHandler(log_stream)
 logging.root.setLevel(logging.NOTSET)
 logging.getLogger('TEST_LOGGER').addHandler(log_handler)
 
 
-@timed(logger_name='TEST_LOGGER')
+@timed(logger_name='TEST_LOGGER', stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 fn()
 
@@ -392,24 +418,22 @@
 from time import sleep
 
 from timed_decorator.simple_timed import timed
 
 ns = {}
 
 
-@timed(out=ns)
+@timed(out=ns, stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 print(ns)
 fn()
 print(ns)
 ```
 Prints
 ```
-fn() -> total time: 1000767300ns
 {'fn': 1000767300}
-fn() -> total time: 1000238800ns
 {'fn': 2001006100}
 ```
```

### Comparing `timed_decorator-1.2.2/README.md` & `timed_decorator-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # timed-decorator
 
 ## Installation
 
 ```
-pip install timed-decorator
+pip install --upgrade timed-decorator
 ```
 
 ## Usage
 
 Attach it to the function you want to time and run the application. 
 
 ```py
@@ -24,17 +24,19 @@
     y_squared = (b ** 2).sum(dim=1)
     return x_squared.unsqueeze(-1) + y_squared.unsqueeze(0) - 2 * diff
 
 
 a = torch.rand((10000, 800))
 b = torch.rand((12000, 800))
 batched_euclidean_distance(a, b)
-a = a.cuda()
-b = b.cuda()
-batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
+
+if torch.cuda.is_available():
+    a = a.cuda()
+    b = b.cuda()
+    batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
 ```
 Prints:
 ```
 batched_euclidean_distance(CpuTensor[10000, 800], CpuTensor[12000, 800]) -> total time: 685659400ns
 batched_euclidean_distance(CudaTensor[10000, 800], CudaTensor[12000, 800]) -> total time: 260411900ns
 ```
 
@@ -45,19 +47,21 @@
     * `disable_gc` (`bool`): If `True`, disabled garbage collection during function execution. Default: `False`.
     * `use_seconds` (`bool`): If `True`, displays the elapsed time in seconds. Default: `False`.
     * `precision` (`int`): Used in conjunction with `use_seconds`, represents the decimal points used for printing seconds. Default: `9`.
     * `show_args` (`bool`): If `True`, displays the function arguments according to `display_level`. Useful when timing function calls with arguments of different magnitude. Default: `False`.
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
-    * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Can't be used in conjunction with `logger_name`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
-    * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`. See [Using a logger](#using-a-logger).
-    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as key. If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict)
+    * `stdout` (`bool`): If `True`, writes the elapsed time to stdout. Default: `True`.
+    * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Default: `None`.
+    * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
+    * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
+    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as key. If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
 
-2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after substracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
+2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 ### Examples
 
 Simple usage.
 ```py
 from timed_decorator.simple_timed import timed
 
@@ -68,15 +72,35 @@
     a, b = 0, 1
     for _ in range(n):
         a, b = b, a + b
     return a
 
 
 fibonacci(10000)
-# fibonacci() -> total time: 2114100ns
+# fibonacci() -> total time: 1114100ns
+```
+
+Getting both the function's return value and the elapsed time.
+```py
+from timed_decorator.simple_timed import timed
+
+
+@timed(return_time=True)
+def fibonacci(n: int) -> int:
+    assert n > 0
+    a, b = 0, 1
+    for _ in range(n):
+        a, b = b, a + b
+    return a
+
+
+value, elapsed = fibonacci(10000)
+print(f'10000th fibonacci number has {len(str(value))} digits. Calculating it took {elapsed}ns.')
+# fibonacci() -> total time: 1001200ns
+# 10000th fibonacci number has 2090 digits. Calculating it took 1001200ns.
 ```
 
 Set `collect_gc=False` to disable pre-collection of garbage.
 
 ```py
 from timed_decorator.simple_timed import timed
 
@@ -87,15 +111,15 @@
     a, b = 0, 1
     for _ in range(n):
         a, b = b, a + b
     return a
 
 
 fibonacci(10000)
-# fibonacci() -> total time: 2062400ns
+# fibonacci() -> total time: 1062400ns
 ```
 
 Using seconds instead of nanoseconds. 
 ```py
 from timed_decorator.simple_timed import timed
 
 
@@ -110,15 +134,15 @@
         return recursive_fibonacci(n - 1) + recursive_fibonacci(n - 2)
     if n == 1:
         return 0
     return 1
 
 
 call_recursive_fibonacci(30)
-# call_recursive_fibonacci() -> total time: 0.098s
+# call_recursive_fibonacci() -> total time: 0.045s
 ```
 
 Displaying function parameters:
 ```py
 from timed_decorator.simple_timed import timed
 import numpy as np
 
@@ -301,15 +325,15 @@
 
 from timed_decorator.simple_timed import timed
 
 logging.basicConfig()
 logging.root.setLevel(logging.NOTSET)
 
 
-@timed(logger_name='TEST_LOGGER')
+@timed(logger_name='TEST_LOGGER', stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 fn()
 ```
@@ -329,15 +353,15 @@
 
 log_stream = StringIO()
 log_handler = logging.StreamHandler(log_stream)
 logging.root.setLevel(logging.NOTSET)
 logging.getLogger('TEST_LOGGER').addHandler(log_handler)
 
 
-@timed(logger_name='TEST_LOGGER')
+@timed(logger_name='TEST_LOGGER', stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 fn()
 
@@ -353,24 +377,22 @@
 from time import sleep
 
 from timed_decorator.simple_timed import timed
 
 ns = {}
 
 
-@timed(out=ns)
+@timed(out=ns, stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 print(ns)
 fn()
 print(ns)
 ```
 Prints
 ```
-fn() -> total time: 1000767300ns
 {'fn': 1000767300}
-fn() -> total time: 1000238800ns
 {'fn': 2001006100}
-```
+```
```

### Comparing `timed_decorator-1.2.2/tests/test_usage.py` & `timed_decorator-1.3.0/tests/test_usage.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,30 +46,30 @@
         def nested_fn():
             @nested_timed(collect_gc=False, use_seconds=True, precision=3)
             def sleeping_fn(x):
                 sleep(x)
 
             @nested_timed(collect_gc=False, use_seconds=True, precision=3)
             def other_fn():
-                sleep(0.5)
-                sleeping_fn(0.5)
+                sleep(0.1)
+                sleeping_fn(0.1)
 
-            sleep(1)
-            sleeping_fn(1)
+            sleep(0.1)
+            sleeping_fn(0.1)
             other_fn()
-            sleeping_fn(1)
+            sleeping_fn(0.1)
 
         nested_fn()
 
     def test_file_usage(self):
         filename = 'file.txt'
 
-        @timed(file_path=filename)
+        @timed(file_path=filename, stdout=False)
         def fn():
-            sleep(1)
+            sleep(0.5)
 
         try:
             fn()
             fn()
             with open(filename, 'r') as f:
                 lines = f.readlines()
                 self.assertEqual(len(lines), 2)
@@ -82,34 +82,44 @@
     def test_logger_usage(self):
         logger_name = 'TEST_LOGGER'
         log_stream = StringIO()
         log_handler = logging.StreamHandler(log_stream)
         logging.root.setLevel(logging.NOTSET)
         logging.getLogger(logger_name).addHandler(log_handler)
 
-        @timed(logger_name=logger_name)
+        @timed(logger_name=logger_name, stdout=False)
         def fn():
-            sleep(1)
+            sleep(0.5)
 
         fn()
         fn()
 
         logged = log_stream.getvalue().split('\n')[:-1]
         self.assertEqual(len(logged), 2)
         self.assertIn(fn.__name__, logged[0])
         self.assertIn(fn.__name__, logged[1])
 
     def test_ns_output(self):
         ns = {}
 
-        @timed(out=ns)
+        @timed(out=ns, stdout=False)
         def fn():
-            sleep(1)
+            sleep(0.5)
 
         fn()
 
         self.assertIsInstance(ns[fn.__name__], int)
-        self.assertGreater(ns[fn.__name__], 1**9)
+        self.assertGreater(ns[fn.__name__], 1**9 / 2)
+
+    def test_return_time(self):
+        @timed(return_time=True, stdout=False)
+        def fn():
+            sleep(0.5)
+
+        _, elapsed = fn()
+
+        self.assertIsInstance(elapsed, int)
+        self.assertGreater(elapsed, 1**9 / 2)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timed_decorator-1.2.2/timed_decorator/nested_timed.py` & `timed_decorator-1.3.0/timed_decorator/nested_timed.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,18 @@
                  disable_gc: bool = False,
                  use_seconds: bool = False,
                  precision: int = 9,
                  show_args: bool = False,
                  show_kwargs: bool = False,
                  display_level: int = 1,
                  sep: str = ', ',
+                 stdout: bool = True,
                  file_path: Union[str, None] = None,
                  logger_name: Union[str, None] = None,
+                 return_time: bool = False,
                  out: dict = None):
     """
     A nested timing decorator that measures the time elapsed during the function call and accounts for other decorators
     further in the call stack.
     It uses perf_counter_ns for measuring which includes time elapsed during sleep and is system-wide.
 
     Args:
@@ -36,28 +38,28 @@
         show_args (bool): If `True`, displays the function arguments according to `display_level`. Useful when timing
             function calls with arguments of different magnitude. Default: `False`.
         show_kwargs (bool): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
         display_level (int): The level of verbosity used when printing function arguments ad keyword arguments. If `0`,
             prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays,
             tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
         sep (str): The separator used when printing function arguments and keyword arguments. Default: `', '`.
+        stdout (bool): If `True`, writes the elapsed time to stdout. Default: `True`.
         file_path (str): If not `None`, writes the measurement at the end of the given file path. For thread safe
-            file writing configure use `logger_name` instead. Can't be used in conjunction with `logger_name`. If both
-            `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
+            file writing configure use `logger_name` instead. Default: `None`.
         logger_name (str): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction
-            with `file_path`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
+            with `file_path`. Default: `None`.
+        return_time (bool): If `True`, returns the elapsed time in addition to the wrapped function's return value.
+            Default: `False`.
         out (dict): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as
             key. If the key already exists, adds the time to the existing value. Default: `None`.
     """
-    assert file_path is None or logger_name is None
-
     gc_collect = collect if collect_gc else nop
     time_formatter = TimeFormatter(use_seconds, precision)
     input_formatter = InputFormatter(show_args, show_kwargs, display_level, sep)
-    logger = Logger(file_path, logger_name)
+    logger = Logger(stdout, file_path, logger_name)
     ns_out = write_mutable if out is not None else nop
 
     def decorator(fn):
         @wraps(fn)
         def wrap(*args, **kwargs):
             global nested_level, nested_times
             nested_level += 1
@@ -93,12 +95,14 @@
                     nested_times[nested_level] = []
                 nested_times[nested_level].append(elapsed)
 
             ns_out(out, fn.__name__, elapsed)
             logger('\t' * nested_level + f'{input_formatter(fn.__name__, *args, **kwargs)} '
                                          f'-> total time: {time_formatter(elapsed)}, '
                                          f'own time: {time_formatter(own_time)}')
+            if return_time:
+                return ret, elapsed
             return ret
 
         return wrap
 
     return decorator
```

### Comparing `timed_decorator-1.2.2/timed_decorator/simple_timed.py` & `timed_decorator-1.3.0/timed_decorator/simple_timed.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,18 @@
           disable_gc: bool = False,
           use_seconds: bool = False,
           precision: int = 9,
           show_args: bool = False,
           show_kwargs: bool = False,
           display_level: int = 1,
           sep: str = ', ',
+          stdout: bool = True,
           file_path: Union[str, None] = None,
           logger_name: Union[str, None] = None,
+          return_time: bool = False,
           out: dict = None):
     """
     A simple timing decorator that measures the time elapsed during the function call and prints it.
     It uses perf_counter_ns for measuring which includes time elapsed during sleep and is system-wide.
 
     Args:
         collect_gc (bool): If `True`, runs a full garbage collection before timing the wrapped function. Default:
@@ -32,28 +34,28 @@
         show_args (bool): If `True`, displays the function arguments according to `display_level`. Useful when timing
             function calls with arguments of different magnitude. Default: `False`.
         show_kwargs (bool): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
         display_level (int): The level of verbosity used when printing function arguments ad keyword arguments. If `0`,
             prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays,
             tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
         sep (str): The separator used when printing function arguments and keyword arguments. Default: `', '`.
+        stdout (bool): If `True`, writes the elapsed time to stdout. Default: `True`.
         file_path (str): If not `None`, writes the measurement at the end of the given file path. For thread safe
-            file writing configure use `logger_name` instead. Can't be used in conjunction with `logger_name`. If both
-            `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
+            file writing configure use `logger_name` instead. Default: `None`.
         logger_name (str): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction
-            with `file_path`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
+            with `file_path`. Default: `None`.
+        return_time (bool): If `True`, returns the elapsed time in addition to the wrapped function's return value.
+            Default: `False`.
         out (dict): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as
             key. If the key already exists, adds the time to the existing value. Default: `None`.
     """
-    assert file_path is None or logger_name is None
-
     gc_collect = collect if collect_gc else nop
     time_formatter = TimeFormatter(use_seconds, precision)
     input_formatter = InputFormatter(show_args, show_kwargs, display_level, sep)
-    logger = Logger(file_path, logger_name)
+    logger = Logger(stdout, file_path, logger_name)
     ns_out = write_mutable if out is not None else nop
 
     def decorator(fn):
         @wraps(fn)
         def wrap(*args, **kwargs):
             gc_collect()
             if disable_gc:
@@ -67,12 +69,14 @@
             finally:
                 if disable_gc:
                     gc.enable()
 
             elapsed = end - start
             ns_out(out, fn.__name__, elapsed)
             logger(f'{input_formatter(fn.__name__, *args, **kwargs)} -> total time: {time_formatter(elapsed)}')
+            if return_time:
+                return ret, elapsed
             return ret
 
         return wrap
 
     return decorator
```

### Comparing `timed_decorator-1.2.2/timed_decorator/utils.py` & `timed_decorator-1.3.0/timed_decorator/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,28 +46,30 @@
     def __call__(self, nanoseconds):
         if self.use_seconds:
             return f'{nanoseconds / 1e9:.{self.precision}f}s'
         return f'{nanoseconds}ns'
 
 
 class Logger:
-    def __init__(self, file_path: Union[str, None], logger_name: Union[str, None]):
-        assert file_path is None or logger_name is None
-
+    def __init__(self, stdout: bool, file_path: Union[str, None], logger_name: Union[str, None]):
+        self.stdout = stdout
         self.file_path = file_path
         self.logger_name = logger_name
 
     def __call__(self, string: str):
+        if self.stdout:
+            print(string)
+
         if self.file_path is not None:
             with open(self.file_path, 'a') as f:
                 f.write(string + '\n')
-        elif self.logger_name is not None:
+
+        if self.logger_name is not None:
             logging.getLogger(self.logger_name).info(string)
-        else:
-            print(string)
+
 
 
 class InputFormatter:
     def __init__(self, show_args: bool = False, show_kwargs: bool = False, display_level: int = 1, sep: str = ', '):
         self.show_args = show_args
         self.show_kwargs = show_kwargs
         self.display_level = display_level
```

### Comparing `timed_decorator-1.2.2/timed_decorator.egg-info/PKG-INFO` & `timed_decorator-1.3.0/timed_decorator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timed-decorator
-Version: 1.2.2
+Version: 1.3.0
 Summary: A timing decorator for python functions.
 Author-email: George Stoica <george.stoica@senticlab.com>
 Maintainer-email: George Stoica <george.stoica@senticlab.com>
 License: Copyright (c) 2024 George Stoica
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
@@ -25,28 +25,30 @@
         OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
         WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: repository, https://github.com/ancestor-mithril/timed-decorator
 Keywords: timing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 
 # timed-decorator
 
 ## Installation
 
 ```
-pip install timed-decorator
+pip install --upgrade timed-decorator
 ```
 
 ## Usage
 
 Attach it to the function you want to time and run the application. 
 
 ```py
@@ -63,17 +65,19 @@
     y_squared = (b ** 2).sum(dim=1)
     return x_squared.unsqueeze(-1) + y_squared.unsqueeze(0) - 2 * diff
 
 
 a = torch.rand((10000, 800))
 b = torch.rand((12000, 800))
 batched_euclidean_distance(a, b)
-a = a.cuda()
-b = b.cuda()
-batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
+
+if torch.cuda.is_available():
+    a = a.cuda()
+    b = b.cuda()
+    batched_euclidean_distance(a, b)  # Cuda device is synchronized if function arguments are on device.
 ```
 Prints:
 ```
 batched_euclidean_distance(CpuTensor[10000, 800], CpuTensor[12000, 800]) -> total time: 685659400ns
 batched_euclidean_distance(CudaTensor[10000, 800], CudaTensor[12000, 800]) -> total time: 260411900ns
 ```
 
@@ -84,19 +88,21 @@
     * `disable_gc` (`bool`): If `True`, disabled garbage collection during function execution. Default: `False`.
     * `use_seconds` (`bool`): If `True`, displays the elapsed time in seconds. Default: `False`.
     * `precision` (`int`): Used in conjunction with `use_seconds`, represents the decimal points used for printing seconds. Default: `9`.
     * `show_args` (`bool`): If `True`, displays the function arguments according to `display_level`. Useful when timing function calls with arguments of different magnitude. Default: `False`.
     * `show_kwargs` (`bool`): If `True`, displays the keyword arguments according to `display_level`. Default: `False`.
     * `display_level` (`int`): The level of verbosity used when printing function arguments ad keyword arguments. If `0`, prints the type of the parameters. If `1`, prints values for all primitive types, shapes for arrays, tensors, dataframes and length for sequences. Otherwise, prints values for all parameters. Default: `1`.
     * `sep` (`str`): The separator used when printing function arguments and keyword arguments. Default: `', '`.
-    * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Can't be used in conjunction with `logger_name`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`.
-    * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. If both `file_path` and `logger_name` are `None`, writes to stdout. Default: `None`. See [Using a logger](#using-a-logger).
-    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as key. If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict)
+    * `stdout` (`bool`): If `True`, writes the elapsed time to stdout. Default: `True`.
+    * `file_path` (`str`): If not `None`, writes the measurement at the end of the given file path. For thread safe file writing configure use `logger_name` instead. Default: `None`.
+    * `logger_name` (`str`): If not `None`, uses the given logger to print the measurement. Can't be used in conjunction with `file_path`. Default: `None`. See [Using a logger](#using-a-logger).
+    * `return_time` (`bool`): If `True`, returns the elapsed time in addition to the wrapped function's return value. Default: `False`.
+    * `out` (`dict`): If not `None`, stores the elapsed time in nanoseconds in the given dict using the function name as key. If the key already exists, adds the time to the existing value. Default: `None`. See [Storing the elapsed time in a dict](#storing-the-elapsed-time-in-a-dict).
 
-2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after substracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
+2. `nested_timed` is similar to `timed`, however it is designed to work nicely with multiple timed functions that call each other, displaying both the total execution time and the difference after subtracting other timed functions on the same call stack. See [Nested timing decorator](#nested-timing-decorator).
 
 ### Examples
 
 Simple usage.
 ```py
 from timed_decorator.simple_timed import timed
 
@@ -107,15 +113,35 @@
     a, b = 0, 1
     for _ in range(n):
         a, b = b, a + b
     return a
 
 
 fibonacci(10000)
-# fibonacci() -> total time: 2114100ns
+# fibonacci() -> total time: 1114100ns
+```
+
+Getting both the function's return value and the elapsed time.
+```py
+from timed_decorator.simple_timed import timed
+
+
+@timed(return_time=True)
+def fibonacci(n: int) -> int:
+    assert n > 0
+    a, b = 0, 1
+    for _ in range(n):
+        a, b = b, a + b
+    return a
+
+
+value, elapsed = fibonacci(10000)
+print(f'10000th fibonacci number has {len(str(value))} digits. Calculating it took {elapsed}ns.')
+# fibonacci() -> total time: 1001200ns
+# 10000th fibonacci number has 2090 digits. Calculating it took 1001200ns.
 ```
 
 Set `collect_gc=False` to disable pre-collection of garbage.
 
 ```py
 from timed_decorator.simple_timed import timed
 
@@ -126,15 +152,15 @@
     a, b = 0, 1
     for _ in range(n):
         a, b = b, a + b
     return a
 
 
 fibonacci(10000)
-# fibonacci() -> total time: 2062400ns
+# fibonacci() -> total time: 1062400ns
 ```
 
 Using seconds instead of nanoseconds. 
 ```py
 from timed_decorator.simple_timed import timed
 
 
@@ -149,15 +175,15 @@
         return recursive_fibonacci(n - 1) + recursive_fibonacci(n - 2)
     if n == 1:
         return 0
     return 1
 
 
 call_recursive_fibonacci(30)
-# call_recursive_fibonacci() -> total time: 0.098s
+# call_recursive_fibonacci() -> total time: 0.045s
 ```
 
 Displaying function parameters:
 ```py
 from timed_decorator.simple_timed import timed
 import numpy as np
 
@@ -340,15 +366,15 @@
 
 from timed_decorator.simple_timed import timed
 
 logging.basicConfig()
 logging.root.setLevel(logging.NOTSET)
 
 
-@timed(logger_name='TEST_LOGGER')
+@timed(logger_name='TEST_LOGGER', stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 fn()
 ```
@@ -368,15 +394,15 @@
 
 log_stream = StringIO()
 log_handler = logging.StreamHandler(log_stream)
 logging.root.setLevel(logging.NOTSET)
 logging.getLogger('TEST_LOGGER').addHandler(log_handler)
 
 
-@timed(logger_name='TEST_LOGGER')
+@timed(logger_name='TEST_LOGGER', stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 fn()
 
@@ -392,24 +418,22 @@
 from time import sleep
 
 from timed_decorator.simple_timed import timed
 
 ns = {}
 
 
-@timed(out=ns)
+@timed(out=ns, stdout=False)
 def fn():
     sleep(1)
 
 
 fn()
 print(ns)
 fn()
 print(ns)
 ```
 Prints
 ```
-fn() -> total time: 1000767300ns
 {'fn': 1000767300}
-fn() -> total time: 1000238800ns
 {'fn': 2001006100}
 ```
```

