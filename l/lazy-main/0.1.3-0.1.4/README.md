# Comparing `tmp/lazy_main-0.1.3.tar.gz` & `tmp/lazy_main-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_main-0.1.3.tar", max compression
+gzip compressed data, was "lazy_main-0.1.4.tar", max compression
```

## Comparing `lazy_main-0.1.3.tar` & `lazy_main-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      789 2024-03-27 01:42:39.964025 lazy_main-0.1.3/README.md
--rw-r--r--   0        0        0       32 2024-03-21 06:24:25.541134 lazy_main-0.1.3/lazy_main/__init__.py
--rw-r--r--   0        0        0     2556 2024-04-11 06:26:22.699016 lazy_main-0.1.3/lazy_main/lazy_main.py
--rw-r--r--   0        0        0      277 2024-04-11 06:26:43.010839 lazy_main-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 lazy_main-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1259 2024-04-29 05:24:16.777567 lazy_main-0.1.4/README.md
+-rw-r--r--   0        0        0       32 2024-03-21 06:24:25.541134 lazy_main-0.1.4/lazy_main/__init__.py
+-rw-r--r--   0        0        0     2665 2024-04-29 05:21:02.740305 lazy_main-0.1.4/lazy_main/lazy_main.py
+-rw-r--r--   0        0        0      277 2024-04-29 05:21:17.823871 lazy_main-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 lazy_main-0.1.4/PKG-INFO
```

### Comparing `lazy_main-0.1.3/README.md` & `lazy_main-0.1.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -3,41 +3,73 @@
 
 ## Installation
 ```sh
 pip install lazy-main
 ```
 
 ## How to Use
-```python
+```py
 from lazy_main import LazyMain
 
 def main(*args, **kwargs):
     print("Hello World!")
 
 def error_handler(exception):
     print("An error occurred!", exception)
 
 if __name__ == "__main__":
     LazyMain(
         main=main,
         error_handler=error_handler, # This is optional.
         sleep_min=3,
         sleep_max=5,
-        loop_count=-1 # -1 Means it will loop infinitely.
+        print_logs=True,
+        loop_count=-1, # -1 Means it will loop infinitely.
     ).run()
 ```
 
 You can also pass arguments to the `main` function.
 
-```python
+```py
 from lazy_main import LazyMain
 
 def main(*args, **kwargs):
     print(kwargs["hello"]) # World!
 
 if __name__ == "__main__":
     LazyMain(
         main=main,
     ).run(
         hello="World!",
     )
+```
+
+Returning `True` will print the total elapsed time.
+
+```py
+from lazy_main import LazyMain
+
+def main():
+    return True
+
+if __name__ == "__main__":
+    LazyMain(
+        main=main,
+    ).run() # Done in 0.10s.
+```
+
+Returning `SIGTERM` will terminate the loop.
+
+```py
+from lazy_main import LazyMain
+import signal
+
+def main():
+    return signal.SIGTERM
+
+if __name__ == "__main__":
+    LazyMain(
+        main=main,
+    ).run()
+
+    print("I'm free!")
 ```
```

### Comparing `lazy_main-0.1.3/lazy_main/lazy_main.py` & `lazy_main-0.1.4/lazy_main/lazy_main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from random import random
 from time import perf_counter, sleep
 import traceback
-from typing import Callable
+import signal
+from typing import Callable, Union
 
 
 class LazyMain:
     def __init__(
         self,
-        main: Callable[..., bool],
+        main: Callable[..., Union[bool, signal.Signals]],
         error_handler: Callable[[Exception], None] = None,  # type: ignore
         print_logs: bool = True,
         sleep_min: int = 3,
         sleep_max: int = 5,
         loop_count: int = -1,
         run_once: bool = None,  # type: ignore
         run_forever: bool = None,  # type: ignore
@@ -51,19 +52,23 @@
             t1 = perf_counter()
 
             try:
                 ok = self.main(*args, **kwargs)
             except Exception as e:
                 if self.print_logs:
                     print("An error ocurred.", e)
-                traceback.print_exc()
+
+                    traceback.print_exc()
 
                 if self.error_handler != None:
                     self.error_handler(e)
 
+            if ok == signal.SIGTERM:
+                break
+
             sleep_time = self.__get_sleep_time()
 
             if self.loop_count > 0:
                 self.loop_count -= 1
 
             if ok:
                 t2 = perf_counter()
```

### Comparing `lazy_main-0.1.3/PKG-INFO` & `lazy_main-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-main
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Mister Nyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -18,41 +18,73 @@
 
 ## Installation
 ```sh
 pip install lazy-main
 ```
 
 ## How to Use
-```python
+```py
 from lazy_main import LazyMain
 
 def main(*args, **kwargs):
     print("Hello World!")
 
 def error_handler(exception):
     print("An error occurred!", exception)
 
 if __name__ == "__main__":
     LazyMain(
         main=main,
         error_handler=error_handler, # This is optional.
         sleep_min=3,
         sleep_max=5,
-        loop_count=-1 # -1 Means it will loop infinitely.
+        print_logs=True,
+        loop_count=-1, # -1 Means it will loop infinitely.
     ).run()
 ```
 
 You can also pass arguments to the `main` function.
 
-```python
+```py
 from lazy_main import LazyMain
 
 def main(*args, **kwargs):
     print(kwargs["hello"]) # World!
 
 if __name__ == "__main__":
     LazyMain(
         main=main,
     ).run(
         hello="World!",
     )
 ```
+
+Returning `True` will print the total elapsed time.
+
+```py
+from lazy_main import LazyMain
+
+def main():
+    return True
+
+if __name__ == "__main__":
+    LazyMain(
+        main=main,
+    ).run() # Done in 0.10s.
+```
+
+Returning `SIGTERM` will terminate the loop.
+
+```py
+from lazy_main import LazyMain
+import signal
+
+def main():
+    return signal.SIGTERM
+
+if __name__ == "__main__":
+    LazyMain(
+        main=main,
+    ).run()
+
+    print("I'm free!")
+```
```

