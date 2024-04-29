# Comparing `tmp/automationhat-0.4.1.tar.gz` & `tmp/automationhat-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automationhat-0.4.1.tar", last modified: Tue Feb  8 14:02:38 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `automationhat-0.4.1.tar` & `automationhat-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,31 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-08 14:02:38.972860 automationhat-0.4.1/
--rw-r--r--   0 pi        (1000) pi        (1000)      939 2022-02-08 13:57:48.000000 automationhat-0.4.1/CHANGELOG.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1070 2022-02-08 13:37:49.000000 automationhat-0.4.1/LICENSE.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      104 2022-02-08 13:37:49.000000 automationhat-0.4.1/MANIFEST.in
--rw-r--r--   0 pi        (1000) pi        (1000)     7395 2022-02-08 14:02:38.972860 automationhat-0.4.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     5147 2022-02-08 13:57:57.000000 automationhat-0.4.1/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-08 14:02:38.968860 automationhat-0.4.1/automationhat/
--rw-r--r--   0 pi        (1000) pi        (1000)     9903 2022-02-08 13:57:18.000000 automationhat-0.4.1/automationhat/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4233 2022-02-08 13:37:49.000000 automationhat-0.4.1/automationhat/pins.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2022-02-08 14:02:38.972860 automationhat-0.4.1/automationhat.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     7395 2022-02-08 14:02:38.000000 automationhat-0.4.1/automationhat.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      298 2022-02-08 14:02:38.000000 automationhat-0.4.1/automationhat.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2022-02-08 14:02:38.000000 automationhat-0.4.1/automationhat.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       45 2022-02-08 14:02:38.000000 automationhat-0.4.1/automationhat.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       14 2022-02-08 14:02:38.000000 automationhat-0.4.1/automationhat.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)     1232 2022-02-08 14:02:38.972860 automationhat-0.4.1/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)     2181 2022-02-08 13:37:49.000000 automationhat-0.4.1/setup.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 automationhat-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 automationhat-1.0.0/Makefile
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 automationhat-1.0.0/README.md
+-rw-r--r--   0        0        0     6572 2020-02-02 00:00:00.000000 automationhat-1.0.0/autohat_360.png
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 automationhat-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9720 2020-02-02 00:00:00.000000 automationhat-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 automationhat-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0    64262 2020-02-02 00:00:00.000000 automationhat-1.0.0/terminal.jpg
+-rwxr-xr-x   0        0        0     5367 2020-02-02 00:00:00.000000 automationhat-1.0.0/test.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 automationhat-1.0.0/tox.ini
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 automationhat-1.0.0/uninstall.sh
+-rw-r--r--   0        0        0    10235 2020-02-02 00:00:00.000000 automationhat-1.0.0/automationhat/__init__.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 automationhat-1.0.0/automationhat/pins.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 automationhat-1.0.0/documentation/REFERENCE.md
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat/analog.py
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat/input.py
+-rwxr-xr-x   0        0        0      317 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat/lights.py
+-rwxr-xr-x   0        0        0      537 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat/output.py
+-rwxr-xr-x   0        0        0      332 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat/relay.py
+-rwxr-xr-x   0        0        0     1943 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat-mini/analog.py
+-rwxr-xr-x   0        0        0     1511 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat-mini/input.py
+-rwxr-xr-x   0        0        0     1902 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat-mini/output.py
+-rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat-mini/images/analog-inputs-blank.jpg
+-rw-r--r--   0        0        0    10205 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat-mini/images/inputs-blank.jpg
+-rw-r--r--   0        0        0     8958 2020-02-02 00:00:00.000000 automationhat-1.0.0/examples/hat-mini/images/outputs-blank.jpg
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 automationhat-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 automationhat-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 automationhat-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 automationhat-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 automationhat-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 automationhat-1.0.0/PKG-INFO
```

### Comparing `automationhat-0.4.1/CHANGELOG.txt` & `automationhat-1.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+1.0.0
+-----
+
+* Refactor to gpiod/gpiodevice.
+* Repackage to hatch/pyproject.toml.
+
 0.4.1
 -----
 
 * Update for SN3218 v2.0.0
 
 0.4.0
 -----
```

### Comparing `automationhat-0.4.1/LICENSE.txt` & `automationhat-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `automationhat-0.4.1/automationhat/__init__.py` & `automationhat-1.0.0/automationhat/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,20 @@
 import atexit
 import time
 import warnings
 
-try:
-    import RPi.GPIO as GPIO
-except ImportError:
-    raise ImportError("This library requires the RPi.GPIO module\nInstall with: sudo python3 -m pip install RPi.GPIO")
-
-try:
-    import smbus
-except ImportError:
-    raise ImportError("This library requires python3-smbus\nInstall with: sudo apt install python3-smbus")
-
-try:
-    import ads1015
-except ImportError:
-    raise ImportError("This library requires ads1015\nInstall with: sudo python3 -m pip install ads1015")
-
-try:
-    import sn3218
-except ImportError:
-    raise ImportError("This library requires sn3218\nInstall with: sudo python3 -m pip install sn3218")
+import ads1015
+import gpiod
+import gpiodevice
+import sn3218
+from gpiod.line import Bias, Direction, Value
 
-from .pins import ObjectCollection, AsyncWorker, StoppableThread
+from .pins import AsyncWorker, ObjectCollection, StoppableThread  # noqa: F401
 
-__version__ = '0.4.1'
+__version__ = '1.0.0'
 
 
 RELAY_1 = 13
 RELAY_2 = 19
 RELAY_3 = 16
 
 INPUT_1 = 26
@@ -48,14 +34,15 @@
 automation_phat = True
 
 _led_states = [0] * 18
 _lights_need_updating = False
 _is_setup = False
 _t_update_lights = None
 _ads1015 = None
+_gpiochip = None
 
 
 class SNLight(object):
     def __init__(self, index):
         self.index = index
         self._max_brightness = float(128)
 
@@ -84,15 +71,15 @@
         :param value: Brightness of the light, from 0.0 to 1.0
         """
         global _lights_need_updating
 
         if self.index is None:
             return
 
-        if type(value) is not int and type(value) is not float:
+        if not isinstance(value, (int, float)):
             raise TypeError("Value must be int or float")
 
         if value >= 0 and value <= 1.0:
             _led_states[self.index] = int(self._max_brightness * value)
             if _t_update_lights is None and lights is not None:
                 lights.output(_led_states)
             else:
@@ -145,21 +132,22 @@
 class Pin(object):
     type = 'Pin'
 
     def __init__(self, pin):
         self.pin = pin
         self._last_value = None
         self._is_setup = False
+        self._gpioline = None
 
     def __call__(self):
         return filter(lambda x: x[0] != '_', dir(self))
 
     def read(self):
         self.setup()
-        return GPIO.input(self.pin)
+        return self._gpioline.get_value(self.pin) == Value.ACTIVE
 
     def setup(self):
         pass
 
     def has_changed(self):
         value = self.read()
 
@@ -169,18 +157,18 @@
         if value is not self._last_value:
             self._last_value = value
             return True
 
         return False
 
     def is_on(self):
-        return self.read() == 1
+        return self.read() is True
 
     def is_off(self):
-        return self.read() == 0
+        return self.read() is False
 
 
 class Input(Pin):
     type = 'Digital Input'
 
     def __init__(self, pin, led):
         self._en_auto_lights = True
@@ -188,24 +176,31 @@
         self.light = SNLight(led)
 
     def setup(self):
         if self._is_setup:
             return False
 
         setup()
-        GPIO.setup(self.pin, GPIO.IN)
+
+        self.pin = _gpiochip.line_offset_from_id(self.pin)
+
+        self._gpioline = _gpiochip.request_lines(consumer="AH", config={
+            self.pin: gpiod.LineSettings(direction=Direction.INPUT, bias=Bias.DISABLED)
+        })
+
         self._is_setup = True
 
     def auto_light(self, value=None):
         if value is not None:
             self._en_auto_lights = value
         return self._en_auto_lights
 
     def read(self):
-        value = Pin.read(self)
+        self.setup()
+        value = self._gpioline.get_value(self.pin) == Value.ACTIVE
         if self._en_auto_lights:
             self.light.write(value)
         return value
 
 
 class Output(Pin):
     type = 'Digital Output'
@@ -216,30 +211,36 @@
         self.light = SNLight(led)
 
     def setup(self):
         if self._is_setup:
             return False
 
         setup()
-        GPIO.setup(self.pin, GPIO.OUT, initial=0)
+
+        self.pin = _gpiochip.line_offset_from_id(self.pin)
+
+        self._gpioline = _gpiochip.request_lines(consumer="AH", config={
+            self.pin: gpiod.LineSettings(direction=Direction.OUTPUT, bias=Bias.DISABLED, output_value=Value.INACTIVE)
+        })
+
         self._is_setup = True
         return True
 
     def auto_light(self, value=None):
         if value is not None:
             self._en_auto_lights = value
         return self._en_auto_lights
 
     def write(self, value):
         """Write a value to the output.
 
         :param value: Value to write, either 1 for HIGH or 0 for LOW
         """
         self.setup()
-        GPIO.output(self.pin, value)
+        self._gpioline.set_value(self.pin, Value.ACTIVE if value else Value.INACTIVE)
         if self._en_auto_lights:
             self.light.write(1 if value else 0)
 
     def on(self):
         """Turn the output on/HIGH"""
         self.write(1)
 
@@ -268,32 +269,37 @@
 
     def setup(self):
         if self._is_setup:
             return False
 
         setup()
 
+        self.pin = _gpiochip.line_offset_from_id(self.pin)
+
         if is_automation_phat() and self.name == "one":
             self.pin = RELAY_3
 
-        GPIO.setup(self.pin, GPIO.OUT, initial=0)
+        self._gpioline = _gpiochip.request_lines(consumer="AH", config={
+            self.pin: gpiod.LineSettings(direction=Direction.OUTPUT, bias=Bias.DISABLED, output_value=Value.INACTIVE)
+        })
+
         self._is_setup = True
         return True
 
     def write(self, value):
         """Write a value to the relay.
 
         :param value: Value to write, either 0 for LOW or 1 for HIGH
         """
         self.setup()
 
         if is_automation_phat() and self.name in ["two", "three"]:
             warnings.warn("Relay '{}' is not supported on Automation pHAT".format(self.name))
 
-        GPIO.output(self.pin, value)
+        self._gpioline.set_value(self.pin, Value.ACTIVE if value else Value.INACTIVE)
 
         if self._en_auto_lights:
             if value:
                 self.light_no.write(1)
                 self.light_nc.write(0)
             else:
                 self.light_no.write(0)
@@ -343,23 +349,22 @@
     if not state and _t_update_lights is not None:
         _t_update_lights.stop()
         _t_update_lights.join()
         _t_update_lights = None
 
 
 def setup():
-    global automation_hat, automation_phat, lights, _ads1015, _is_setup, _t_update_lights
+    global automation_hat, automation_phat, lights, _ads1015, _is_setup, _t_update_lights, _gpiochip
 
     if _is_setup:
         return True
 
     _is_setup = True
 
-    GPIO.setmode(GPIO.BCM)
-    GPIO.setwarnings(False)
+    _gpiochip = gpiodevice.find_chip_by_platform()
 
     _ads1015 = ads1015.ADS1015()
     try:
         chip_type = _ads1015.detect_chip_type()
     except IOError:
         raise RuntimeError("No ADC detected, check your connections")
 
@@ -391,16 +396,14 @@
     if _t_update_lights:
         _t_update_lights.stop()
         _t_update_lights.join()
 
     if lights is not None:
         lights.output([0] * 18)
 
-    GPIO.cleanup()
-
 
 analog = ObjectCollection()
 analog._add(one=AnalogInput(0, 25.85, 0))
 analog._add(two=AnalogInput(1, 25.85, 1))
 analog._add(three=AnalogInput(2, 25.85, 2))
 analog._add(four=AnalogInput(3, 3.3, None))
```

### Comparing `automationhat-0.4.1/automationhat/pins.py` & `automationhat-1.0.0/automationhat/pins.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 getattr(self._all[node], name)
             def handler(*args, **kwargs):
                 return self._do(name, *args, **kwargs)
             handler.__name__ = name
             return handler
 
     def __getitem__(self, key):
-        """Supprot accessing with [n]"""
+        """Support accessing with [n]"""
         if isinstance(key, int):
             return self._all[self._index[key]]
         else:
             return self._all[key]
 
     def _do(self, name, *args, **kwargs):
         """Runs a function against all registered pins
```

