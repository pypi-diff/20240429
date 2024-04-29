# Comparing `tmp/bean_rs-0.3.0.tar.gz` & `tmp/bean_rs-0.3.1.tar.gz`

## Comparing `bean_rs-0.3.0.tar` & `bean_rs-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 bean_rs-0.3.0/Cargo.toml
--rw-r--r--   0     1001      127      612 2024-04-15 21:47:40.000000 bean_rs-0.3.0/.github/workflows/crates.yml
--rw-r--r--   0     1001      127     3863 2024-04-15 21:47:40.000000 bean_rs-0.3.0/.github/workflows/pypi.yml
--rw-r--r--   0     1001      127      260 2024-04-15 21:47:40.000000 bean_rs-0.3.0/.github/workflows/test.yml
--rw-r--r--   0     1001      127      686 2024-04-15 21:47:40.000000 bean_rs-0.3.0/.gitignore
--rw-r--r--   0     1001      127    36722 2024-04-15 21:47:40.000000 bean_rs-0.3.0/Cargo.lock
--rw-r--r--   0     1001      127     1070 2024-04-15 21:47:40.000000 bean_rs-0.3.0/LICENSE
--rw-r--r--   0     1001      127      381 2024-04-15 21:47:40.000000 bean_rs-0.3.0/Makefile
--rw-r--r--   0     1001      127     1600 2024-04-15 21:47:40.000000 bean_rs-0.3.0/README.md
--rw-r--r--   0     1001      127     1248 2024-04-15 21:47:40.000000 bean_rs-0.3.0/example.bean
--rw-r--r--   0     1001      127     3209 2024-04-15 21:47:40.000000 bean_rs-0.3.0/grammar.pest
--rw-r--r--   0     1001      127      223 2024-04-15 21:47:40.000000 bean_rs-0.3.0/python/bean_rs/__init__.py
--rw-r--r--   0     1001      127      281 2024-04-15 21:47:40.000000 bean_rs-0.3.0/python/bean_rs/bean_rs.pyi
--rw-r--r--   0     1001      127        0 2024-04-15 21:47:40.000000 bean_rs-0.3.0/python/bean_rs/py.typed
--rw-r--r--   0     1001      127      137 2024-04-15 21:47:40.000000 bean_rs-0.3.0/python/tests/test_load.py
--rw-r--r--   0     1001      127      421 2024-04-15 21:47:40.000000 bean_rs-0.3.0/requirements-dev.lock
--rw-r--r--   0     1001      127      207 2024-04-15 21:47:40.000000 bean_rs-0.3.0/requirements.lock
--rw-r--r--   0     1001      127    15030 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/book.rs
--rw-r--r--   0     1001      127    23315 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/data.rs
--rw-r--r--   0     1001      127     1082 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/error.rs
--rw-r--r--   0     1001      127       95 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/grammar.rs
--rw-r--r--   0     1001      127      239 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/ledger.rs
--rw-r--r--   0     1001      127     1494 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/lib.rs
--rw-r--r--   0     1001      127     4404 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/loader.rs
--rw-r--r--   0     1001      127     1285 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/main.rs
--rw-r--r--   0     1001      127     2753 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/utils.rs
--rw-r--r--   0     1001      127      536 2024-04-15 21:47:40.000000 bean_rs-0.3.0/tests/cli.rs
--rw-r--r--   0     1001      127     1327 2024-04-15 21:47:40.000000 bean_rs-0.3.0/tests/integration_test.rs
--rw-r--r--   0     1001      127     1264 2024-04-15 21:47:40.000000 bean_rs-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2303 1970-01-01 00:00:00.000000 bean_rs-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 bean_rs-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      127      612 2024-04-29 15:46:23.000000 bean_rs-0.3.1/.github/workflows/crates.yml
+-rw-r--r--   0     1001      127     3863 2024-04-29 15:46:23.000000 bean_rs-0.3.1/.github/workflows/pypi.yml
+-rw-r--r--   0     1001      127      260 2024-04-29 15:46:23.000000 bean_rs-0.3.1/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      686 2024-04-29 15:46:23.000000 bean_rs-0.3.1/.gitignore
+-rw-r--r--   0     1001      127    36722 2024-04-29 15:46:23.000000 bean_rs-0.3.1/Cargo.lock
+-rw-r--r--   0     1001      127     1070 2024-04-29 15:46:23.000000 bean_rs-0.3.1/LICENSE
+-rw-r--r--   0     1001      127      381 2024-04-29 15:46:23.000000 bean_rs-0.3.1/Makefile
+-rw-r--r--   0     1001      127     1600 2024-04-29 15:46:23.000000 bean_rs-0.3.1/README.md
+-rw-r--r--   0     1001      127     1248 2024-04-29 15:46:23.000000 bean_rs-0.3.1/example.bean
+-rw-r--r--   0     1001      127     3209 2024-04-29 15:46:23.000000 bean_rs-0.3.1/grammar.pest
+-rw-r--r--   0     1001      127      223 2024-04-29 15:46:23.000000 bean_rs-0.3.1/python/bean_rs/__init__.py
+-rw-r--r--   0     1001      127      281 2024-04-29 15:46:23.000000 bean_rs-0.3.1/python/bean_rs/bean_rs.pyi
+-rw-r--r--   0     1001      127        0 2024-04-29 15:46:23.000000 bean_rs-0.3.1/python/bean_rs/py.typed
+-rw-r--r--   0     1001      127      137 2024-04-29 15:46:23.000000 bean_rs-0.3.1/python/tests/test_load.py
+-rw-r--r--   0     1001      127      421 2024-04-29 15:46:23.000000 bean_rs-0.3.1/requirements-dev.lock
+-rw-r--r--   0     1001      127      207 2024-04-29 15:46:23.000000 bean_rs-0.3.1/requirements.lock
+-rw-r--r--   0     1001      127    15030 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/book.rs
+-rw-r--r--   0     1001      127    23315 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/data.rs
+-rw-r--r--   0     1001      127     1082 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/error.rs
+-rw-r--r--   0     1001      127       95 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/grammar.rs
+-rw-r--r--   0     1001      127      239 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/ledger.rs
+-rw-r--r--   0     1001      127     1494 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/lib.rs
+-rw-r--r--   0     1001      127     4404 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/loader.rs
+-rw-r--r--   0     1001      127     1285 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/main.rs
+-rw-r--r--   0     1001      127     2753 2024-04-29 15:46:23.000000 bean_rs-0.3.1/src/utils.rs
+-rw-r--r--   0     1001      127      536 2024-04-29 15:46:23.000000 bean_rs-0.3.1/tests/cli.rs
+-rw-r--r--   0     1001      127     1327 2024-04-29 15:46:23.000000 bean_rs-0.3.1/tests/integration_test.rs
+-rw-r--r--   0     1001      127     1264 2024-04-29 15:46:23.000000 bean_rs-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2303 1970-01-01 00:00:00.000000 bean_rs-0.3.1/PKG-INFO
```

### Comparing `bean_rs-0.3.0/Cargo.toml` & `bean_rs-0.3.1/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [package]
 name = "bean-rs"
 license = "MIT"
 authors = ["Chris Arderne <chris@rdrn.me"]
 description = "beancount clone in Rust"
-version = "0.3.0"  # set by Github Actions CI
+version = "0.3.1"  # set by Github Actions CI
 edition = "2021"
+repository = "https://github.com/carderne/bean-rs"
 
 [dependencies]
 chrono = "0.4.31"
 clap = { version = "4.4.18", features = ["derive"] }
 env_logger = "0.11.0"
 log = "0.4.20"
 pest = "2.7.6"
```

### Comparing `bean_rs-0.3.0/.github/workflows/crates.yml` & `bean_rs-0.3.1/.github/workflows/crates.yml`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/.github/workflows/pypi.yml` & `bean_rs-0.3.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/.gitignore` & `bean_rs-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/Cargo.lock` & `bean_rs-0.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bean-rs"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "assert_cmd",
  "chrono",
  "clap",
  "env_logger",
  "log",
  "pest",
```

### Comparing `bean_rs-0.3.0/LICENSE` & `bean_rs-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/README.md` & `bean_rs-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/example.bean` & `bean_rs-0.3.1/example.bean`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/grammar.pest` & `bean_rs-0.3.1/grammar.pest`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/src/book.rs` & `bean_rs-0.3.1/src/book.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/src/data.rs` & `bean_rs-0.3.1/src/data.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/src/error.rs` & `bean_rs-0.3.1/src/error.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/src/lib.rs` & `bean_rs-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/src/loader.rs` & `bean_rs-0.3.1/src/loader.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/src/main.rs` & `bean_rs-0.3.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/src/utils.rs` & `bean_rs-0.3.1/src/utils.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/tests/cli.rs` & `bean_rs-0.3.1/tests/cli.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/tests/integration_test.rs` & `bean_rs-0.3.1/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/pyproject.toml` & `bean_rs-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bean_rs-0.3.0/PKG-INFO` & `bean_rs-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bean-rs
-Version: 0.3.0
+Version: 0.3.1
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 License-File: LICENSE
```

