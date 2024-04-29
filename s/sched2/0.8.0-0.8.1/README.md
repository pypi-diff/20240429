# Comparing `tmp/sched2-0.8.0.tar.gz` & `tmp/sched2-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sched2-0.8.0.tar", max compression
+gzip compressed data, was "sched2-0.8.1.tar", max compression
```

## Comparing `sched2-0.8.0.tar` & `sched2-0.8.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2023-01-04 16:55:36.505678 sched2-0.8.0/LICENSE
--rw-r--r--   0        0        0     1762 2024-02-27 00:15:04.258586 sched2-0.8.0/README.md
--rw-r--r--   0        0        0      443 2024-03-08 07:13:10.302517 sched2-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9705 2024-03-08 07:07:34.335041 sched2-0.8.0/sched2.py
--rw-r--r--   0        0        0     2369 1970-01-01 00:00:00.000000 sched2-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-01-04 16:55:36.505678 sched2-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2239 2024-03-13 20:39:42.012907 sched2-0.8.1/README.md
+-rw-r--r--   0        0        0      443 2024-04-29 05:13:30.016700 sched2-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    10295 2024-04-29 05:13:53.642293 sched2-0.8.1/sched2.py
+-rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 sched2-0.8.1/PKG-INFO
```

### Comparing `sched2-0.8.0/LICENSE` & `sched2-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sched2-0.8.0/README.md` & `sched2-0.8.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,77 @@
 The `sched2` module extends the general purpose event scheduler `sched` from Python's standard library. `sched2.scheduler` is a subclass of `sched.scheduler` that adds new features such as the `every` and `cron` decorators. It's a practical tool for automating tasks that need to run repeatedly after certain time delays or at specific times.
 
 # Install
 
-To install the `sched2` module, you can use `pip`, the package installer for Python. Open a terminal and run the following command:
+`sched2` is available on PyPI.
 
 ```bash
 pip install sched2
 ```
 
 # Examples
 
 The code below uses the `every` decorator to schedule checking the public IP address every two minutes.
+Then every day at 9:00, the `cron` decorator is used to send a report via email.
+Finally, the `on` decorator is used to send an email when the IP address changes.
+
 
 ```python
+from smtplib import SMTP_SSL
 from urllib.request import urlopen
+
 from sched2 import scheduler
 
 # Create a scheduler
 sc = scheduler()
 
+# we'll use this to remember the last IP address between runs
+last_ip = None
 
-@sc.every(120)  # Run every two minutes
+
+@sc.every(30)  # Run every two minutes
 def print_ip_address():
+    global last_ip
+
     ip = urlopen("https://icanhazip.com/").read().decode("utf-8").strip()
+
     print(f"Public IP address: {ip}")
 
-# Run the scheduler
-sc.run()
-```
+    last_ip = last_ip or ip  # reset last_ip
+    if ip != last_ip:
+        last_ip = ip
 
+        # Emit an event when the IP address changes
+        sc.emit("ip_changed", kwargs={"new_ip": ip})
 
-The following code does something similar, but here we use the `cron` decorator to schedule an email report to be sent every weekday at 9:00.
 
-```python
-from smtplib import SMTP_SSL
-from sched2 import scheduler
+@sc.cron("0 9 * * 1-5")  # Run every weekday at 9:00
+def send_report():
+    sendmail("Daily Report", "The numbers are up!")
 
-# Create a scheduler
-sc = scheduler()
 
+@sc.on("ip_changed")  # Run when 'ip_changed' event is emitted
+def send_email(new_ip):
+    sendmail("IP Address Changed", f"New IP address: {ip}")
 
-@sc.cron("0 9 * * 1-5")  # Run every weekday at 9:00
-def send_report():
+
+def sendmail(subject, body):
+    """Send an email using SMTP_SSL."""
     with SMTP_SSL("smtp.example.com") as smtp:
         smtp.login("me@example.com", "password")
         smtp.sendmail(
             "me@example.com",
             "team@example.com",
-            "Subject: Daily Report\n\nThe numbers are up!",
+            f"{subject}\n\n{body}",
         )
 
 
 # Run the scheduler
 sc.run()
+
 ```
 
 # Source Code and Issues
 
-Help improve sched2 by reporting any issues or suggestions on the issue tracker at [github.com/medecau/sched2/issues](https://github.com/medecau/sched2/issues).
+The source code for `sched2` is available on GitHub at [github.com/medecau/sched2](https://github.com/medecau/sched2).
+
+You can help improve sched2 by reporting any issues or suggestions on the issue tracker at [github.com/medecau/sched2/issues](https://github.com/medecau/sched2/issues).
```

### Comparing `sched2-0.8.0/sched2.py` & `sched2-0.8.1/sched2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,57 @@
 """
 .. include:: README.md
 """
 
+from contextlib import suppress
 import datetime as dt
 import random
 import re
 import sched
 from collections import defaultdict
 from functools import partial
 
 __all__ = ["scheduler"]
 
 _sentinel = object()
 
 
+def suppress_exceptions(exceptions):
+    """A decorator that suppresses exceptions raised by a function."""
+
+    def decorator(action):
+        def wrapper(*args, **kwargs):
+            with suppress(exceptions):
+                return action(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
 class scheduler(sched.scheduler):
     """A subclass of the `sched.scheduler` class from the standard library.
 
     This subclass adds additional functionality to the `scheduler` class,
     including the ability to schedule events using relative time intervals
     and a decorator for scheduling events to run at regular intervals.
     """
 
     __listeners = defaultdict(list)
 
     def repeat(
-        self, delay, priority, action, immediate=True, argument=(), kwargs=_sentinel
+        self,
+        delay,
+        priority,
+        action,
+        *,
+        immediate=True,
+        suppress=None,
+        argument=(),
+        kwargs=_sentinel,
     ):
         """Schedule an event to be run at regular intervals.
 
         This method is a variant of the `sched2.enter` method that re-schedules itself
         after each run. It allows a function to be scheduled to run at regular
         intervals by specifying the `delay` and `priority` as arguments.
 
@@ -44,14 +66,17 @@
         In the event that the function returns a `True`ish value, the function
         will not be re-scheduled.
         """
 
         if kwargs is _sentinel:
             kwargs = {}
 
+        if suppress:
+            action = suppress_exceptions(suppress)(action)
+
         partial_action = partial(action, *argument, **kwargs)
 
         def repeater(action):
             # if the action returns a Trueish value, do not re-schedule
             if not action():
                 self.enter(delay, priority, repeater, (partial_action,))
 
@@ -59,15 +84,15 @@
         self.enter(initial_delay, priority, repeater, (partial_action,))
 
         # this return value is used by the decorator
         # do not change this to return partial_action
         # we return the original action so it can be decorated multiple times
         return action
 
-    def every(self, delay, priority=0, immediate=True):
+    def every(self, delay, *, priority=0, immediate=True, suppress=None):
         """Schedule an event to be run at regular intervals using a decorator.
 
         This method is a variant of the `sched2.repeat` method that can be used as a
         decorator. It allows a function to be scheduled to run at regular
         intervals by specifying the `delay` and `priority` as arguments. The
         default `priority` is `0`.
 
@@ -77,15 +102,17 @@
 
         In the event that the function returns a `True`ish value, the function
         will not be re-scheduled.
         """
 
         # we return a partial application of repeat
         # this will be immediately called to decorate the function
-        return partial(self.repeat, delay, priority, immediate=immediate)
+        return partial(
+            self.repeat, delay, priority, immediate=immediate, suppress=suppress
+        )
 
     def cron(self, rule, priority=0):
         """Schedule an event to be run at specific times using a cron-like syntax.
 
         A cron rule is a string with five space-separated fields that represent
         the minute, hour, day, month, and day of the week. Each field can contain
         a single value, a range of values, or a list of values separated by commas.
@@ -121,14 +148,16 @@
 
         def cron_runner(action):
             if check_rule(parsed_rule):
                 self.enter(0, priority, action)
             delay = 60 - self.timefunc() % 60
             self.enter(delay, 0, cron_runner, (action,))
 
+            return action
+
         return cron_runner
 
     @property
     def listeners(self):
         return self.__listeners.copy()
 
     def on(self, event, priority=0, action=None):
```

### Comparing `sched2-0.8.0/PKG-INFO` & `sched2-0.8.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sched2
-Version: 0.8.0
+Version: 0.8.1
 Summary: Event scheduler 2
 Home-page: https://medecau.github.io/sched2/
 License: MIT
 Author: Pedro Rodrigues
 Author-email: me@pdbr.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,64 +16,81 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 The `sched2` module extends the general purpose event scheduler `sched` from Python's standard library. `sched2.scheduler` is a subclass of `sched.scheduler` that adds new features such as the `every` and `cron` decorators. It's a practical tool for automating tasks that need to run repeatedly after certain time delays or at specific times.
 
 # Install
 
-To install the `sched2` module, you can use `pip`, the package installer for Python. Open a terminal and run the following command:
+`sched2` is available on PyPI.
 
 ```bash
 pip install sched2
 ```
 
 # Examples
 
 The code below uses the `every` decorator to schedule checking the public IP address every two minutes.
+Then every day at 9:00, the `cron` decorator is used to send a report via email.
+Finally, the `on` decorator is used to send an email when the IP address changes.
+
 
 ```python
+from smtplib import SMTP_SSL
 from urllib.request import urlopen
+
 from sched2 import scheduler
 
 # Create a scheduler
 sc = scheduler()
 
+# we'll use this to remember the last IP address between runs
+last_ip = None
 
-@sc.every(120)  # Run every two minutes
+
+@sc.every(30)  # Run every two minutes
 def print_ip_address():
+    global last_ip
+
     ip = urlopen("https://icanhazip.com/").read().decode("utf-8").strip()
+
     print(f"Public IP address: {ip}")
 
-# Run the scheduler
-sc.run()
-```
+    last_ip = last_ip or ip  # reset last_ip
+    if ip != last_ip:
+        last_ip = ip
 
+        # Emit an event when the IP address changes
+        sc.emit("ip_changed", kwargs={"new_ip": ip})
 
-The following code does something similar, but here we use the `cron` decorator to schedule an email report to be sent every weekday at 9:00.
 
-```python
-from smtplib import SMTP_SSL
-from sched2 import scheduler
+@sc.cron("0 9 * * 1-5")  # Run every weekday at 9:00
+def send_report():
+    sendmail("Daily Report", "The numbers are up!")
 
-# Create a scheduler
-sc = scheduler()
 
+@sc.on("ip_changed")  # Run when 'ip_changed' event is emitted
+def send_email(new_ip):
+    sendmail("IP Address Changed", f"New IP address: {ip}")
 
-@sc.cron("0 9 * * 1-5")  # Run every weekday at 9:00
-def send_report():
+
+def sendmail(subject, body):
+    """Send an email using SMTP_SSL."""
     with SMTP_SSL("smtp.example.com") as smtp:
         smtp.login("me@example.com", "password")
         smtp.sendmail(
             "me@example.com",
             "team@example.com",
-            "Subject: Daily Report\n\nThe numbers are up!",
+            f"{subject}\n\n{body}",
         )
 
 
 # Run the scheduler
 sc.run()
+
 ```
 
 # Source Code and Issues
 
-Help improve sched2 by reporting any issues or suggestions on the issue tracker at [github.com/medecau/sched2/issues](https://github.com/medecau/sched2/issues).
+The source code for `sched2` is available on GitHub at [github.com/medecau/sched2](https://github.com/medecau/sched2).
+
+You can help improve sched2 by reporting any issues or suggestions on the issue tracker at [github.com/medecau/sched2/issues](https://github.com/medecau/sched2/issues).
```

