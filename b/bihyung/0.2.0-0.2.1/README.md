# Comparing `tmp/bihyung-0.2.0.tar.gz` & `tmp/bihyung-0.2.1.tar.gz`

## Comparing `bihyung-0.2.0.tar` & `bihyung-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 bihyung-0.2.0/bihyung/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-04-28 01:47:01.000000 bihyung-0.2.0/bihyung/.gitignore
--rw-r--r--   0     1001      127     4056 2024-04-28 01:47:01.000000 bihyung-0.2.0/bihyung/src/lib.rs
--rw-r--r--   0     1001      127   102229 2024-04-28 01:47:12.000000 bihyung-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 bihyung-0.2.0/Cargo.toml
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      445 1970-01-01 00:00:00.000000 bihyung-0.2.1/bihyung/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-04-28 23:20:21.000000 bihyung-0.2.1/bihyung/.gitignore
+-rw-r--r--   0     1001      127      426 2024-04-28 23:20:21.000000 bihyung-0.2.1/bihyung/langchain_example.py
+-rw-r--r--   0     1001      127     4056 2024-04-28 23:20:21.000000 bihyung-0.2.1/bihyung/src/lib.rs
+-rw-r--r--   0     1001      127   102173 2024-04-28 23:20:21.000000 bihyung-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 bihyung-0.2.1/Cargo.toml
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 bihyung-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      256 1970-01-01 00:00:00.000000 bihyung-0.2.1/PKG-INFO
```

### Comparing `bihyung-0.2.0/bihyung/.gitignore` & `bihyung-0.2.1/bihyung/.gitignore`

 * *Files identical despite different names*

### Comparing `bihyung-0.2.0/bihyung/src/lib.rs` & `bihyung-0.2.1/bihyung/src/lib.rs`

 * *Files identical despite different names*

### Comparing `bihyung-0.2.0/Cargo.lock` & `bihyung-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -278,18 +278,18 @@
 name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bihyung"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "enum_dispatch",
- "llm-daemon 0.2.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "llm-daemon 0.2.0",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
  "tracing",
  "tracing-subscriber",
  "url",
 ]
@@ -1662,54 +1662,54 @@
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "llm-daemon"
 version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "929c88315de03d76a11f848ef6a5794fcd72f305e5c14015c0551ac35ce0a190"
 dependencies = [
  "anyhow",
- "async-trait",
  "axum",
- "criterion",
  "daemonize",
  "futures",
  "hyper 1.3.1",
  "hyper-util",
- "langchain-rust",
  "reqwest 0.12.4",
  "serde",
  "serde_json",
  "tempfile",
  "tokio",
  "tracing",
  "tracing-subscriber",
- "tracing-test",
  "url",
 ]
 
 [[package]]
 name = "llm-daemon"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "929c88315de03d76a11f848ef6a5794fcd72f305e5c14015c0551ac35ce0a190"
+version = "0.2.1"
 dependencies = [
  "anyhow",
+ "async-trait",
  "axum",
+ "criterion",
  "daemonize",
  "futures",
  "hyper 1.3.1",
  "hyper-util",
+ "langchain-rust",
  "reqwest 0.12.4",
  "serde",
  "serde_json",
  "tempfile",
  "tokio",
  "tracing",
  "tracing-subscriber",
+ "tracing-test",
  "url",
 ]
 
 [[package]]
 name = "lock_api"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
```

