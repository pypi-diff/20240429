# Comparing `tmp/outspin-0.3.1.tar.gz` & `tmp/outspin-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outspin-0.3.1.tar", max compression
+gzip compressed data, was "outspin-0.3.2.tar", max compression
```

## Comparing `outspin-0.3.1.tar` & `outspin-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1057 2024-01-28 15:05:03.231433 outspin-0.3.1/LICENSE
--rw-r--r--   0        0        0     7000 2024-04-03 21:43:21.246732 outspin-0.3.1/README.md
--rw-r--r--   0        0        0     1125 2024-04-09 19:53:54.397507 outspin-0.3.1/outspin/__init__.py
--rw-r--r--   0        0        0      285 2024-01-28 13:30:06.837380 outspin-0.3.1/outspin/constants.py
--rw-r--r--   0        0        0      321 2024-01-28 13:37:17.150786 outspin-0.3.1/outspin/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-09 19:53:20.976750 outspin-0.3.1/outspin/py.typed
--rw-r--r--   0        0        0     2472 2024-04-09 19:46:12.969478 outspin-0.3.1/outspin/unix.py
--rw-r--r--   0        0        0     1891 2024-04-14 18:16:33.560291 outspin-0.3.1/outspin/windows.py
--rw-r--r--   0        0        0     1093 2024-04-19 20:56:04.935037 outspin-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 outspin-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-04-29 17:12:37.923408 outspin-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7000 2024-04-29 17:12:37.923550 outspin-0.3.2/README.md
+-rw-r--r--   0        0        0     1125 2024-04-29 17:12:37.923772 outspin-0.3.2/outspin/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-29 17:12:37.923845 outspin-0.3.2/outspin/constants.py
+-rw-r--r--   0        0        0      321 2024-04-29 17:12:37.923914 outspin-0.3.2/outspin/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:12:37.923951 outspin-0.3.2/outspin/py.typed
+-rw-r--r--   0        0        0     2522 2024-04-29 17:21:42.228894 outspin-0.3.2/outspin/unix.py
+-rw-r--r--   0        0        0     1891 2024-04-29 17:12:37.924116 outspin-0.3.2/outspin/windows.py
+-rw-r--r--   0        0        0     1093 2024-04-29 17:21:42.229070 outspin-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7597 1970-01-01 00:00:00.000000 outspin-0.3.2/PKG-INFO
```

### Comparing `outspin-0.3.1/LICENSE` & `outspin-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `outspin-0.3.1/README.md` & `outspin-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `outspin-0.3.1/outspin/__init__.py` & `outspin-0.3.2/outspin/__init__.py`

 * *Files identical despite different names*

### Comparing `outspin-0.3.1/outspin/unix.py` & `outspin-0.3.2/outspin/unix.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,14 +80,16 @@
 
 
 def _getch() -> str:  # pragma: no cover
     old_state = termios.tcgetattr(1)
     tty.setcbreak(1)
     try:
         return os.read(1, 8).decode("utf-8")
+    except KeyboardInterrupt:
+        return "^C"
     finally:
         termios.tcsetattr(1, termios.TCSADRAIN, old_state)
 
 
 def get_key() -> str:
     """Return a keypress from standard input."""
     return _MODS.get(ch := _getch(), ch)
```

### Comparing `outspin-0.3.1/outspin/windows.py` & `outspin-0.3.2/outspin/windows.py`

 * *Files identical despite different names*

### Comparing `outspin-0.3.1/pyproject.toml` & `outspin-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "outspin"
-version = "0.3.1"
+version = "0.3.2"
 description = "Conveniently read single char inputs in the console."
 authors = ["trag1c <trag1cdev@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `outspin-0.3.1/PKG-INFO` & `outspin-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outspin
-Version: 0.3.1
+Version: 0.3.2
 Summary: Conveniently read single char inputs in the console.
 License: MIT
 Author: trag1c
 Author-email: trag1cdev@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

