# Comparing `tmp/sparkle_log-0.3.0.tar.gz` & `tmp/sparkle_log-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparkle_log-0.3.0.tar", max compression
+gzip compressed data, was "sparkle_log-0.4.0.tar", max compression
```

## Comparing `sparkle_log-0.3.0.tar` & `sparkle_log-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       55 2024-04-27 18:40:34.684340 sparkle_log-0.3.0/AUTHORS.md
--rw-r--r--   0        0        0     1071 2024-04-27 18:40:34.684340 sparkle_log-0.3.0/LICENSE
--rw-r--r--   0        0        0     1947 2024-04-27 18:40:34.684340 sparkle_log-0.3.0/README.md
--rw-r--r--   0        0        0     5338 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      836 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/__about__.py
--rw-r--r--   0        0        0      397 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/__init__.py
--rw-r--r--   0        0        0     3542 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/__main__.py
--rw-r--r--   0        0        0     2085 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/as_context_manager.py
--rw-r--r--   0        0        0     1251 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/as_decorator.py
--rw-r--r--   0        0        0     2464 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/drive_space.py
--rw-r--r--   0        0        0      109 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/graphs.py
--rw-r--r--   0        0        0     2722 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/log_writer.py
--rw-r--r--   0        0        0        0 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/py.typed
--rw-r--r--   0        0        0      526 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/scheduler.py
--rw-r--r--   0        0        0     2464 2024-04-27 18:40:34.688340 sparkle_log-0.3.0/sparkle_log/ui.py
--rw-r--r--   0        0        0     3251 1970-01-01 00:00:00.000000 sparkle_log-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-04-28 21:05:29.712746 sparkle_log-0.4.0/AUTHORS.md
+-rw-r--r--   0        0        0     1071 2024-04-28 21:05:29.712746 sparkle_log-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4764 2024-04-28 21:05:29.712746 sparkle_log-0.4.0/README.md
+-rw-r--r--   0        0        0     5338 2024-04-28 21:05:29.712746 sparkle_log-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      836 2024-04-28 21:05:29.712746 sparkle_log-0.4.0/sparkle_log/__about__.py
+-rw-r--r--   0        0        0      560 2024-04-28 21:05:29.712746 sparkle_log-0.4.0/sparkle_log/__init__.py
+-rw-r--r--   0        0        0     3552 2024-04-28 21:05:29.712746 sparkle_log-0.4.0/sparkle_log/__main__.py
+-rw-r--r--   0        0        0     2578 2024-04-28 21:05:29.712746 sparkle_log-0.4.0/sparkle_log/as_context_manager.py
+-rw-r--r--   0        0        0     1968 2024-04-28 21:05:29.716746 sparkle_log-0.4.0/sparkle_log/as_decorator.py
+-rw-r--r--   0        0        0      302 2024-04-28 21:05:29.716746 sparkle_log-0.4.0/sparkle_log/custom_types.py
+-rw-r--r--   0        0        0     2464 2024-04-28 21:05:29.716746 sparkle_log-0.4.0/sparkle_log/drive_space.py
+-rw-r--r--   0        0        0      109 2024-04-28 21:05:29.716746 sparkle_log-0.4.0/sparkle_log/graphs.py
+-rw-r--r--   0        0        0     3953 2024-04-28 21:05:29.716746 sparkle_log-0.4.0/sparkle_log/log_writer.py
+-rw-r--r--   0        0        0        0 2024-04-28 21:05:29.716746 sparkle_log-0.4.0/sparkle_log/py.typed
+-rw-r--r--   0        0        0      659 2024-04-28 21:05:29.716746 sparkle_log-0.4.0/sparkle_log/scheduler.py
+-rw-r--r--   0        0        0     2795 2024-04-28 21:05:29.716746 sparkle_log-0.4.0/sparkle_log/ui.py
+-rw-r--r--   0        0        0     6068 1970-01-01 00:00:00.000000 sparkle_log-0.4.0/PKG-INFO
```

### Comparing `sparkle_log-0.3.0/LICENSE` & `sparkle_log-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sparkle_log-0.3.0/pyproject.toml` & `sparkle_log-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sparkle-log"
-version = "0.3.0"
+version = "0.4.0"
 description = "Write sparkline graphs of CPU and memory usage to your logs."
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["monitoring", "logging" ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `sparkle_log-0.3.0/sparkle_log/__about__.py` & `sparkle_log-0.4.0/sparkle_log/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "__readme__",
     "__repository__",
     "__homepage__",
     "__documentation__",
 ]
 
 __title__ = "sparkle-log"
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 __description__ = "Write sparkline graphs of CPU and memory usage to your logs."
 __author__ = "Matthew Martin"
 __author_email__ = "matthewdeanmartin@gmail.com"
 __keywords__ = ["monitoring", "logging"]
 __status__ = "4 - Beta"
 __license__ = "MIT"
 __readme__ = "README.md"
```

### Comparing `sparkle_log-0.3.0/sparkle_log/__main__.py` & `sparkle_log-0.4.0/sparkle_log/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 import time
 from typing import Optional, Sequence, cast
 
 from sparkle_log.__about__ import __version__
 from sparkle_log.as_context_manager import MetricsLoggingContext
 from sparkle_log.as_decorator import monitor_metrics_on_call
-from sparkle_log.ui import GraphStyle
+from sparkle_log.custom_types import GraphStyle
 
 
 @monitor_metrics_on_call(("cpu",), 1)
 def log_memory_and_cpu():
     """Example with decorator"""
     while True:
         time.sleep(4)
```

### Comparing `sparkle_log-0.3.0/sparkle_log/as_context_manager.py` & `sparkle_log-0.4.0/sparkle_log/as_context_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,57 +3,72 @@
 """
 
 import logging
 import time
 from threading import Event, Thread
 from typing import Any, Optional
 
+from sparkle_log.custom_types import CustomMetricsCallBacks, GraphStyle
 from sparkle_log.graphs import GLOBAL_LOGGER
 from sparkle_log.scheduler import run_scheduler
-from sparkle_log.ui import GraphStyle
 
 
 class MetricsLoggingContext:
     """
     Context manager to log system metrics.
     """
 
-    def __init__(self, metrics=("cpu", "memory"), interval: int = 10, style: GraphStyle = "faces") -> None:
+    def __init__(
+        self,
+        metrics=("cpu", "memory"),
+        interval: int = 10,
+        style: GraphStyle = "faces",
+        custom_metrics: CustomMetricsCallBacks = None,
+    ) -> None:
         """Initialize the context manager."""
         if not metrics:
             metrics = ("cpu", "memory")
         else:
+            custom_metrics_names = custom_metrics.keys() if custom_metrics else []
             for metric in metrics:
-                if metric not in ("cpu", "memory", "drive"):
+                if metric not in ("cpu", "memory", "drive") and metric not in custom_metrics_names:
                     raise TypeError("Unexpected metric")
         self.metrics = metrics
         self.interval = interval
         self.style = style
         self.stop_event: Optional[Event] = None
         self.scheduler_thread: Optional[Thread] = None
+        self.custom_metrics = custom_metrics
 
     def __enter__(self) -> "MetricsLoggingContext":
         """Start the context manager, if logging enabled."""
         if GLOBAL_LOGGER.isEnabledFor(logging.INFO):
             self.stop_event = Event()
             self.scheduler_thread = Thread(
-                target=run_scheduler, args=(self.stop_event, self.metrics, self.interval, self.style)
+                target=run_scheduler,
+                args=(self.stop_event, self.metrics, self.interval, self.style, self.custom_metrics),
             )
             self.scheduler_thread.start()
         return self
 
     def __exit__(self, exc_type: Any, exc_value: Any, traceback: Any) -> None:
         """Stop the context manager."""
         if self.scheduler_thread and self.scheduler_thread.is_alive():
-            self.stop_event.set()
+            if self.stop_event:
+                self.stop_event.set()
             self.scheduler_thread.join()
 
 
 # Usage example with the context manager
 if __name__ == "__main__":
     logging.basicConfig(level=logging.INFO)
-    with MetricsLoggingContext(metrics=("cpu",), interval=1):
+    import random
+
+    def dodgy_metric():
+        return random.randint(0, 100)
+
+    with MetricsLoggingContext(metrics=("dodgy",), interval=1, custom_metrics={"dodgy": dodgy_metric}):
         # Execute some operations
         print("Monitoring system metrics during operations...")
         time.sleep(20)
         # Operations are now being monitored
         # The thread will be stopped when exiting this block
```

### Comparing `sparkle_log-0.3.0/sparkle_log/as_decorator.py` & `sparkle_log-0.4.0/sparkle_log/as_decorator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 This module contains the decorator to monitor the metrics of the system while the function is being executed.
 """
 
 import logging
+from asyncio import iscoroutinefunction
 from functools import wraps
 from threading import Event, Thread
 
+from sparkle_log.custom_types import GraphStyle
 from sparkle_log.graphs import GLOBAL_LOGGER
 from sparkle_log.scheduler import run_scheduler
-from sparkle_log.ui import GraphStyle
 
 INITIALIZED = False
 
 
 def monitor_metrics_on_call(metrics=("cpu", "memory"), interval=10, style: GraphStyle = "bar"):
     """
     Decorator to monitor the system metrics while the function is being executed.
@@ -34,10 +35,27 @@
                 return func(*args, **kwargs)
             finally:
                 # Stop the scheduler and wait for thread to finish
                 stop_event.set()
 
                 scheduler_thread.join()
 
-        return wrapper
+        @wraps(func)
+        async def async_wrapper(*args, **kwargs):
+            """Wrapper function"""
+            if not GLOBAL_LOGGER.isEnabledFor(logging.INFO):
+                return func(*args, **kwargs)
+            stop_event = Event()
+            scheduler_thread = Thread(target=run_scheduler, args=(stop_event, metrics, interval, style))
+            scheduler_thread.start()
+
+            try:
+                return await func(*args, **kwargs)
+            finally:
+                # Stop the scheduler and wait for thread to finish
+                stop_event.set()
+
+                scheduler_thread.join()
+
+        return async_wrapper if iscoroutinefunction(func) else wrapper
 
     return decorator
```

### Comparing `sparkle_log-0.3.0/sparkle_log/drive_space.py` & `sparkle_log-0.4.0/sparkle_log/drive_space.py`

 * *Files identical despite different names*

### Comparing `sparkle_log-0.3.0/sparkle_log/ui.py` & `sparkle_log-0.4.0/sparkle_log/ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Sparkline graph code goes here.
 """
 
-from typing import Literal
+from typing import cast
 
 import sparklines
 
-GraphStyle = Literal["bar", "faces", "jagged", "linear", "vertical", "ascii_art", "pie_chart"]
+from sparkle_log.custom_types import GraphStyle, NumberType
 
 
-def sparkline(numbers: list[int], style: GraphStyle = "bar") -> str:
+def sparkline(numbers: list[NumberType], style: GraphStyle = "bar") -> str:
     """Generate a simple sparkline string for a list of integers."""
     if style == "bar":
         for line in sparklines.sparklines(numbers):
             return line
     elif style == "jagged":
         return jagged_ascii_sparkline(numbers)
     elif style == "vertical":
@@ -25,57 +25,66 @@
     elif style == "pie_chart":
         return pie_chart_sparkline(numbers)
     elif style == "faces":
         return faces_sparkline(numbers)
     return ""
 
 
-def faces_sparkline(data):
+def faces_sparkline(data: list[NumberType]):
     """Generate a sparkline with face emojis."""
     symbols = ["😞", "😐", "😊", "😁"]
     return sparkline_it(data, symbols)
 
 
-def sparkline_it(data: list[int], symbols: list[str]):
+def sparkline_it(data: list[NumberType], symbols: list[str]):
     """Generate a sparkline with the given symbols."""
     noneless_data = [_ for _ in data if _ is not None]
     max_val = max(noneless_data)
     min_val = min(noneless_data)
     range_val = max_val - min_val
     if range_val == 0:  # Avoid division by zero
-        return "".join(symbols[0] for _ in data)
+        return "".join(" " for _ in data)
     if range_val * len(symbols) == 0:
         return " "
     return "".join(
         symbols[min(len(symbols) - 1, int((val - min_val) / range_val * len(symbols)))] if val is not None else " "
         for val in data
     )
 
 
-def pie_chart_sparkline(data):
+def pie_chart_sparkline(data: list[NumberType]):
     """Using different geometric shapes or other symbols"""
     symbols = ["○", "◔", "◑", "◕", "●"]
     return sparkline_it(data, symbols)
 
 
-def ascii_sparkline(data):
+def ascii_sparkline(data: list[NumberType]):
     """Using different ASCII characters."""
     symbols = [" ", ".", ":", "-", "=", "+", "*", "#", "%", "@"]
     return sparkline_it(data, symbols)
 
 
-def linear_ascii_sparkline(data):
+def linear_ascii_sparkline(data: list[NumberType]):
     """Ascii for Low, medium, and high levels"""
     levels = ["_", "-", "¯"]
     return sparkline_it(data, levels)
 
 
-def jagged_ascii_sparkline(data):
+def jagged_ascii_sparkline(data: list[NumberType]):
     """Ascii incorporating a peak character"""
     symbols = ["_", "-", "^", "¯"]
     return sparkline_it(data, symbols)
 
 
-def vertical_ascii_sparkline(data):
+def vertical_ascii_sparkline(data: list[NumberType]):
     """Ascii Using single and double vertical lines"""
     symbols = ["_", "|", "‖"]
     return sparkline_it(data, symbols)
+
+
+if __name__ == "__main__":
+
+    def run():
+        for style in ["bar", "jagged", "vertical", "linear", "ascii_art", "pie_chart", "faces"]:
+            print(f"{style}: {sparkline([1, 2, 3, 4, 5, 6, 7, 8, 9, 10], cast(GraphStyle, style))}")
+
+    run()
```

