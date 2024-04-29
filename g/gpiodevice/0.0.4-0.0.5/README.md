# Comparing `tmp/gpiodevice-0.0.4.tar.gz` & `tmp/gpiodevice-0.0.5.tar.gz`

## Comparing `gpiodevice-0.0.4.tar` & `gpiodevice-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/Makefile
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/README.md
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/check.sh
--rwxr-xr-x   0        0        0     7022 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/install.sh
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/requirements-dev.txt
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/tox.ini
--rwxr-xr-x   0        0        0     1268 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/uninstall.sh
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/examples/README.md
--rwxr-xr-x   0        0        0      702 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/examples/gpiotool
--rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/__init__.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/errors.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/platform/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/platform/alienware.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/platform/pi.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/gpiodevice/platform/radxa.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/tests/test_features.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/LICENSE
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 gpiodevice-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/Makefile
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/README.md
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/check.sh
+-rwxr-xr-x   0        0        0     7022 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/requirements-dev.txt
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/tox.ini
+-rwxr-xr-x   0        0        0     1268 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/uninstall.sh
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/examples/README.md
+-rwxr-xr-x   0        0        0      702 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/examples/gpiotool
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/gpiodevice/__init__.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/gpiodevice/errors.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/gpiodevice/platform/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/gpiodevice/platform/alienware.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/gpiodevice/platform/pi.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/gpiodevice/platform/radxa.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/tests/test_features.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 gpiodevice-0.0.5/PKG-INFO
```

### Comparing `gpiodevice-0.0.4/Makefile` & `gpiodevice-0.0.5/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 	@echo "pytest:       run Python test fixtures"
 	@echo "clean:        clean Python build and dist directories"
 	@echo "build:        build Python distribution files"
 	@echo "testdeploy:   build and upload to test PyPi"
 	@echo "deploy:       build and upload to PyPi"
 	@echo "tag:          tag the repository with the current version\n"
 
+version:
+	@hatch version
+
 install:
 	./install.sh --unstable
 
 uninstall:
 	./uninstall.sh
 
 dev-deps:
@@ -40,15 +43,15 @@
 
 pytest:
 	tox -e py
 
 nopost:
 	@bash check.sh --nopost
 
-tag:
+tag: version
 	git tag -a "v${LIBRARY_VERSION}" -m "Version ${LIBRARY_VERSION}"
 
 build: check
 	@hatch build
 
 clean:
 	-rm -r dist
```

### Comparing `gpiodevice-0.0.4/README.md` & `gpiodevice-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/check.sh` & `gpiodevice-0.0.5/check.sh`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/install.sh` & `gpiodevice-0.0.5/install.sh`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/uninstall.sh` & `gpiodevice-0.0.5/uninstall.sh`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/examples/gpiotool` & `gpiodevice-0.0.5/examples/gpiotool`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/gpiodevice/__init__.py` & `gpiodevice-0.0.5/gpiodevice/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 from pathlib import Path
 
 import gpiod
 
 from . import errors, platform
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 
 CHIP_GLOB = "/dev/gpiochip*"
 
 
 # Deprecated
 friendly_errors: bool = False
@@ -148,16 +148,21 @@
 
 
 def get_pin(pin, label, settings):
     # Do nothing if given a user specified LineRequest/offset tuple
     if isinstance(pin, tuple):
         return pin
 
-    chip = find_chip_by_pins(pin)
-    line_offset = chip.line_offset_from_id(pin)
+    if isinstance(pin, int):
+        chip = find_chip_by_platform()
+        line_offset = pin
+    else:
+        chip = find_chip_by_pins(pin)
+        line_offset = chip.line_offset_from_id(pin)
+
     consumer = Path(sys.argv[0]).stem
     lines = chip.request_lines(consumer=f"{consumer}-{label}", config={line_offset: settings})
     return lines, line_offset
 
 
 def get_pins_for_platform(platforms):
     this_platform = platform.get_name()
```

### Comparing `gpiodevice-0.0.4/gpiodevice/errors.py` & `gpiodevice-0.0.5/gpiodevice/errors.py`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/gpiodevice/platform/radxa.py` & `gpiodevice-0.0.5/gpiodevice/platform/radxa.py`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/LICENSE` & `gpiodevice-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/pyproject.toml` & `gpiodevice-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpiodevice-0.0.4/PKG-INFO` & `gpiodevice-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gpiodevice
-Version: 0.0.4
+Version: 0.0.5
 Summary: Helper library for working with Linux gpiochip devices.
 Project-URL: GitHub, https://www.github.com/pimoroni/gpiodevice-python
 Project-URL: Homepage, https://www.pimoroni.com
 Author-email: Philip Howard <phil@pimoroni.com>
 Maintainer-email: Philip Howard <phil@pimoroni.com>
 License: MIT License
         
@@ -61,14 +61,19 @@
 gpiodevice is a simple middleware library intended to make some user-facing aspects of interfacing with Linux's GPIO character device ABI (via gpiod) simpler and friendlier.
 
 gpiodevice is not intended to replace gpiod, but collects some common patterns into a reusable library for GPIO-based Python projects.
 
 
 # Changelog
 
+0.0.5
+-----
+
+* Add support for int type in get_pin
+
 0.0.4
 -----
 
 * Gracefully handle a tuple being passed to get_pin
 * Match all pinctrl- gpiodevices for RPi in get_gpiochip_labels
 
 0.0.3
```

