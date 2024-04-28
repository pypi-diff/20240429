# Comparing `tmp/pawz_core-0.2.0.tar.gz` & `tmp/pawz_core-0.2.1.tar.gz`

## Comparing `pawz_core-0.2.0.tar` & `pawz_core-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 pawz_core-0.2.0/Cargo.toml
--rw-r--r--   0      501       20     8995 2024-04-26 13:12:07.000000 pawz_core-0.2.0/Cargo.lock
--rw-r--r--   0      501       20       56 2024-04-26 12:50:45.000000 pawz_core-0.2.0/README.md
--rw-r--r--   0      501       20       56 2024-04-26 12:50:45.000000 pawz_core-0.2.0/readme.md
--rw-r--r--   0      501       20      423 2024-04-26 13:06:57.000000 pawz_core-0.2.0/src/lib.rs
--rw-r--r--   0      501       20       45 2024-04-26 12:31:06.000000 pawz_core-0.2.0/src/main.rs
--rw-r--r--   0      501       20      623 2024-04-26 12:50:45.000000 pawz_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 pawz_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      161 1970-01-01 00:00:00.000000 pawz_core-0.2.1/Cargo.toml
+-rw-r--r--   0      501       20     8995 2024-04-28 22:40:55.000000 pawz_core-0.2.1/Cargo.lock
+-rw-r--r--   0      501       20       56 2024-04-26 12:50:45.000000 pawz_core-0.2.1/README.md
+-rw-r--r--   0      501       20       56 2024-04-26 12:50:45.000000 pawz_core-0.2.1/readme.md
+-rw-r--r--   0      501       20      423 2024-04-26 13:14:45.000000 pawz_core-0.2.1/src/lib.rs
+-rw-r--r--   0      501       20       45 2024-04-26 12:31:06.000000 pawz_core-0.2.1/src/main.rs
+-rw-r--r--   0      501       20      635 2024-04-28 22:40:50.000000 pawz_core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 pawz_core-0.2.1/PKG-INFO
```

### Comparing `pawz_core-0.2.0/Cargo.lock` & `pawz_core-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 name = "pathdiff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
 
 [[package]]
 name = "pawz_core"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "open",
  "pyo3",
 ]
 
 [[package]]
 name = "portable-atomic"
```

### Comparing `pawz_core-0.2.0/pyproject.toml` & `pawz_core-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "pawz_core"
+dynamic = ["version"]
 authors = [{ name = "Cody", email = "cody@dkdc.dev" }]
-description = "pawz the dog (core)"
+description = "pawz core functionality (Rust!)"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = []
-dynamic = ["version"]
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [project.urls]
 "Homepage" = "https://github.com/lostmygithubaccount/pawz"
 "Bug Tracker" = "https://github.com/lostmygithubaccount/pawz/issues"
```

### Comparing `pawz_core-0.2.0/PKG-INFO` & `pawz_core-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: pawz_core
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Summary: pawz the dog (core)
+Summary: pawz core functionality (Rust!)
 Author-email: Cody <cody@dkdc.dev>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/lostmygithubaccount/pawz
 Project-URL: Bug Tracker, https://github.com/lostmygithubaccount/pawz/issues
 
 # pawz-core
```

