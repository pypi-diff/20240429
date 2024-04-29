# Comparing `tmp/multicounter-0.1.4.tar.gz` & `tmp/multicounter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicounter-0.1.4.tar", max compression
+gzip compressed data, was "multicounter-0.2.0.tar", max compression
```

## Comparing `multicounter-0.1.4.tar` & `multicounter-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    16725 2023-07-11 22:21:56.633995 multicounter-0.1.4/LICENSE
--rw-r--r--   0        0        0     2969 2023-07-11 22:21:56.633995 multicounter-0.1.4/README.md
--rw-r--r--   0        0        0      273 2023-07-11 22:21:56.633995 multicounter-0.1.4/multicounter/__init__.py
--rw-r--r--   0        0        0      826 2023-07-11 22:21:56.633995 multicounter-0.1.4/multicounter/multicounter.py
--rw-r--r--   0        0        0      429 2023-07-11 22:21:56.633995 multicounter-0.1.4/multicounter/py.typed
--rw-r--r--   0        0        0      659 2023-07-11 22:21:56.633995 multicounter-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 multicounter-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-04-29 16:53:02.848582 multicounter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4488 2024-04-29 16:53:02.848582 multicounter-0.2.0/README.md
+-rw-r--r--   0        0        0      273 2024-04-29 16:53:02.848582 multicounter-0.2.0/multicounter/__init__.py
+-rw-r--r--   0        0        0      826 2024-04-29 16:53:02.848582 multicounter-0.2.0/multicounter/multicounter.py
+-rw-r--r--   0        0        0      429 2024-04-29 16:53:02.848582 multicounter-0.2.0/multicounter/py.typed
+-rw-r--r--   0        0        0      665 2024-04-29 16:53:02.848582 multicounter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5314 1970-01-01 00:00:00.000000 multicounter-0.2.0/PKG-INFO
```

### Comparing `multicounter-0.1.4/LICENSE` & `multicounter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `multicounter-0.1.4/multicounter/multicounter.py` & `multicounter-0.2.0/multicounter/multicounter.py`

 * *Files identical despite different names*

### Comparing `multicounter-0.1.4/pyproject.toml` & `multicounter-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "multicounter"
-version = "0.1.4"
+version = "0.2.0"
 description = "A simple, elegant counter with support for counting multiple things at once."
 authors = ["Joseph Hale <me@jhale.dev>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://github.com/thehale/multicounter"
 repository = "https://github.com/thehale/multicounter"
 documentation = "https://github.com/thehale/multicounter"
 keywords = [ "counter", "statistics" ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+black = "^24.4.2"
 pytest = "^7.4"
 pre-commit = "^2.21.0"
-black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

