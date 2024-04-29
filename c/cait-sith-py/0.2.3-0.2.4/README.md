# Comparing `tmp/cait_sith_py-0.2.3.tar.gz` & `tmp/cait_sith_py-0.2.4.tar.gz`

## Comparing `cait_sith_py-0.2.3.tar` & `cait_sith_py-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 cait_sith_py-0.2.3/Cargo.toml
--rw-r--r--   0     1001      127     2650 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     1890 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/.gitignore
--rw-r--r--   0     1001      127    11357 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/LICENSE
--rw-r--r--   0     1001      127     1572 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/action.rs
--rw-r--r--   0     1001      127     1995 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/arithmetic.rs
--rw-r--r--   0     1001      127     3158 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/keyshare.rs
--rw-r--r--   0     1001      127     1698 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/lib.rs
--rw-r--r--   0     1001      127     1551 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/participant.rs
--rw-r--r--   0     1001      127     4118 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/presign.rs
--rw-r--r--   0     1001      127     1728 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/protocol.rs
--rw-r--r--   0     1001      127     4020 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/sign.rs
--rw-r--r--   0     1001      127     4259 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/src/triples.rs
--rw-r--r--   0     1001      127    35142 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/Cargo.lock
--rw-r--r--   0     1001      127      923 2024-04-22 04:32:17.000000 cait_sith_py-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 cait_sith_py-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 cait_sith_py-0.2.4/Cargo.toml
+-rw-r--r--   0     1001      127     2650 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1890 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/LICENSE
+-rw-r--r--   0     1001      127     1572 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/action.rs
+-rw-r--r--   0     1001      127     1995 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/arithmetic.rs
+-rw-r--r--   0     1001      127     3158 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/keyshare.rs
+-rw-r--r--   0     1001      127     1698 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/lib.rs
+-rw-r--r--   0     1001      127     1579 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/participant.rs
+-rw-r--r--   0     1001      127     4118 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/presign.rs
+-rw-r--r--   0     1001      127     1728 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/protocol.rs
+-rw-r--r--   0     1001      127     4020 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/sign.rs
+-rw-r--r--   0     1001      127     4598 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/src/triples.rs
+-rw-r--r--   0     1001      127    35142 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/Cargo.lock
+-rw-r--r--   0     1001      127      923 2024-04-29 01:18:43.000000 cait_sith_py-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      394 1970-01-01 00:00:00.000000 cait_sith_py-0.2.4/PKG-INFO
```

### Comparing `cait_sith_py-0.2.3/.github/workflows/CI.yml` & `cait_sith_py-0.2.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/.gitignore` & `cait_sith_py-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/LICENSE` & `cait_sith_py-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/src/action.rs` & `cait_sith_py-0.2.4/src/action.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/src/arithmetic.rs` & `cait_sith_py-0.2.4/src/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/src/keyshare.rs` & `cait_sith_py-0.2.4/src/keyshare.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/src/lib.rs` & `cait_sith_py-0.2.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/src/participant.rs` & `cait_sith_py-0.2.4/src/participant.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 use cait_sith::protocol::Participant;
 use pyo3::pyclass::CompareOp;
 use pyo3::{pyclass, pymethods, IntoPy, PyObject, Python};
-use serde::Serialize;
+use serde::{Deserialize, Serialize};
 
 /// Represents a participant in the protocol.
 ///
 /// Each participant should be uniquely identified by some number, which this
 /// struct holds. In our case, we use a `u32`, which is enough for billions of
 /// participants. That said, you won't actually be able to make the protocols
 /// work with billions of users.
 #[pyclass(name = "Participant")]
-#[derive(Debug, Clone, Copy, PartialEq, Eq, PartialOrd, Ord, Serialize, Hash)]
+#[derive(Debug, Clone, Copy, PartialEq, Eq, PartialOrd, Ord, Serialize, Hash, Deserialize)]
 pub struct PyParticipant {
     #[pyo3(get)]
     id: u32,
 }
 
 #[pymethods]
 impl PyParticipant {
```

### Comparing `cait_sith_py-0.2.3/src/presign.rs` & `cait_sith_py-0.2.4/src/presign.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/src/protocol.rs` & `cait_sith_py-0.2.4/src/protocol.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/src/sign.rs` & `cait_sith_py-0.2.4/src/sign.rs`

 * *Files identical despite different names*

### Comparing `cait_sith_py-0.2.3/src/triples.rs` & `cait_sith_py-0.2.4/src/triples.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 use cait_sith::protocol::Action;
 use cait_sith::protocol::{MessageData, Participant, Protocol};
 use cait_sith::triples::{TripleGenerationOutput, TriplePub, TripleShare};
 use k256::Secp256k1;
 use pyo3::prelude::*;
 use pyo3::{pyclass, pyfunction, PyResult};
+use serde::{Deserialize, Serialize};
 
 use crate::{
     create_action_enum, create_protocol, participant::convert_participants,
     participant::PyParticipant,
 };
 
 #[pyclass(name = "TripleShare")]
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, Serialize, Deserialize)]
 pub struct PyTripleShare {
     #[pyo3(get)]
     pub a: String,
     #[pyo3(get)]
     pub b: String,
     #[pyo3(get)]
     pub c: String,
@@ -40,15 +41,15 @@
             b: serde_json::from_str(&value.b).unwrap(),
             c: serde_json::from_str(&value.c).unwrap(),
         }
     }
 }
 
 #[pyclass(name = "TriplePublic")]
-#[derive(Clone, Debug)]
+#[derive(Clone, Debug, Serialize, Deserialize)]
 pub struct PyTriplePublic {
     #[pyo3(get)]
     pub big_a: String,
     #[pyo3(get)]
     pub big_b: String,
     #[pyo3(get)]
     pub big_c: String,
@@ -82,22 +83,34 @@
             participants: convert_participants(value.participants),
             threshold: value.threshold,
         }
     }
 }
 
 #[pyclass(name = "TripleGenerationOutput")]
-#[derive(Debug, Clone)]
+#[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct PyTripleGenerationOutput {
     #[pyo3(get)]
     pub share: PyTripleShare,
     #[pyo3(get)]
     pub public: PyTriplePublic,
 }
 
+#[pymethods]
+impl PyTripleGenerationOutput {
+    fn to_json(&self) -> String {
+        serde_json::to_string(&self).unwrap()
+    }
+
+    #[new]
+    fn new(json_data: String) -> Self {
+        serde_json::from_str(&json_data).unwrap()
+    }
+}
+
 impl From<TripleGenerationOutput<Secp256k1>> for PyTripleGenerationOutput {
     fn from(value: TripleGenerationOutput<Secp256k1>) -> Self {
         Self {
             share: value.0.into(),
             public: value.1.into(),
         }
     }
@@ -132,13 +145,12 @@
 pub fn py_generate_triple(
     participants: Vec<PyParticipant>,
     me: PyParticipant,
     threshold: usize,
 ) -> PyResult<TripleGenerationProtocol> {
     let participants: Vec<Participant> = convert_participants(participants);
     let me = me.into();
-    let protocol =
-        cait_sith::triples::generate_triple(participants.as_slice(), me, threshold)
-            .map_err(|err| PyErr::new::<pyo3::exceptions::PyRuntimeError, _>(format!("{}", err)))?;
+    let protocol = cait_sith::triples::generate_triple(participants.as_slice(), me, threshold)
+        .map_err(|err| PyErr::new::<pyo3::exceptions::PyRuntimeError, _>(format!("{}", err)))?;
     let wrapped = Arc::new(Mutex::new(protocol));
     Ok(TripleGenerationProtocol { protocol: wrapped })
 }
```

### Comparing `cait_sith_py-0.2.3/Cargo.lock` & `cait_sith_py-0.2.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
  "serde",
  "smol",
  "subtle",
 ]
 
 [[package]]
 name = "cait-sith-py"
-version = "0.2.3"
+version = "0.2.4"
 dependencies = [
  "cait-sith",
  "k256",
  "pyo3",
  "serde",
  "serde_json",
 ]
```

### Comparing `cait_sith_py-0.2.3/pyproject.toml` & `cait_sith_py-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cait_sith_py"
-version = "0.2.3"
+version = "0.2.4"
 description = "Cait Sith rust wrapper on python"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 [tool.poetry.dev-dependencies]
 maturin = "0.14.3"
@@ -19,15 +19,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 
 [project]
 name = "cait_sith_py"
-version = "0.2.3"
+version = "0.2.4"
 description = "Cait Sith rust wrapper on python"
 license = {file = "LICENSE"} # relative to the package/ directory
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

