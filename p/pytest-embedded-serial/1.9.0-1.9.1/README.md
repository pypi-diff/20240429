# Comparing `tmp/pytest_embedded_serial-1.9.0.tar.gz` & `tmp/pytest_embedded_serial-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_embedded_serial-1.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pytest_embedded_serial-1.9.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pytest_embedded_serial-1.9.0.tar` & `pytest_embedded_serial-1.9.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1094 2024-04-25 11:36:08.627318 pytest_embedded_serial-1.9.0/LICENSE
--rw-r--r--   0        0        0      195 2024-04-25 11:36:08.627318 pytest_embedded_serial-1.9.0/README.md
--rw-r--r--   0        0        0     3293 2024-04-25 11:36:08.627318 pytest_embedded_serial-1.9.0/pyproject.toml
--rw-r--r--   0        0        0      176 2024-04-25 11:36:08.627318 pytest_embedded_serial-1.9.0/pytest_embedded_serial/__init__.py
--rw-r--r--   0        0        0     1271 2024-04-25 11:36:08.627318 pytest_embedded_serial-1.9.0/pytest_embedded_serial/dut.py
--rw-r--r--   0        0        0     6184 2024-04-25 11:36:08.627318 pytest_embedded_serial-1.9.0/pytest_embedded_serial/serial.py
--rw-r--r--   0        0        0     3224 2024-04-25 11:36:08.627318 pytest_embedded_serial-1.9.0/tests/test_serial.py
--rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1094 2024-04-26 05:38:44.157606 pytest_embedded_serial-1.9.1/LICENSE
+-rw-r--r--   0        0        0      195 2024-04-26 05:38:44.157606 pytest_embedded_serial-1.9.1/README.md
+-rw-r--r--   0        0        0     3293 2024-04-26 05:38:44.157606 pytest_embedded_serial-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0      176 2024-04-26 05:38:44.157606 pytest_embedded_serial-1.9.1/pytest_embedded_serial/__init__.py
+-rw-r--r--   0        0        0     1271 2024-04-26 05:38:44.157606 pytest_embedded_serial-1.9.1/pytest_embedded_serial/dut.py
+-rw-r--r--   0        0        0     6184 2024-04-26 05:38:44.157606 pytest_embedded_serial-1.9.1/pytest_embedded_serial/serial.py
+-rw-r--r--   0        0        0     3224 2024-04-26 05:38:44.157606 pytest_embedded_serial-1.9.1/tests/test_serial.py
+-rw-r--r--   0        0        0     1549 1970-01-01 00:00:00.000000 pytest_embedded_serial-1.9.1/PKG-INFO
```

### Comparing `pytest_embedded_serial-1.9.0/LICENSE` & `pytest_embedded_serial-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.9.0/pyproject.toml` & `pytest_embedded_serial-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python",
     "Topic :: Software Development :: Testing",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.7"
 
 dependencies = [
-    "pytest-embedded~=1.9.0",
+    "pytest-embedded~=1.9.1",
     "pyserial~=3.0",
 ]
 
 [project.urls]
 homepage = "https://github.com/espressif/pytest-embedded"
 repository = "https://github.com/espressif/pytest-embedded"
 documentation = "https://docs.espressif.com/projects/pytest-embedded/en/latest/"
```

### Comparing `pytest_embedded_serial-1.9.0/pytest_embedded_serial/dut.py` & `pytest_embedded_serial-1.9.1/pytest_embedded_serial/dut.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.9.0/pytest_embedded_serial/serial.py` & `pytest_embedded_serial-1.9.1/pytest_embedded_serial/serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.9.0/tests/test_serial.py` & `pytest_embedded_serial-1.9.1/tests/test_serial.py`

 * *Files identical despite different names*

### Comparing `pytest_embedded_serial-1.9.0/PKG-INFO` & `pytest_embedded_serial-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-serial
-Version: 1.9.0
+Version: 1.9.1
 Summary: Make pytest-embedded plugin work with Serial.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: pytest-embedded~=1.9.0
+Requires-Dist: pytest-embedded~=1.9.1
 Requires-Dist: pyserial~=3.0
 Project-URL: changelog, https://github.com/espressif/pytest-embedded/blob/main/CHANGELOG.md
 Project-URL: documentation, https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Project-URL: homepage, https://github.com/espressif/pytest-embedded
 Project-URL: repository, https://github.com/espressif/pytest-embedded
 
 ### pytest-embedded-serial
```
