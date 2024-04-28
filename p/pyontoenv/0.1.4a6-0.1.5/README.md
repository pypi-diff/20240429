# Comparing `tmp/pyontoenv-0.1.4a6.tar.gz` & `tmp/pyontoenv-0.1.5.tar.gz`

## Comparing `pyontoenv-0.1.4a6.tar` & `pyontoenv-0.1.5.tar`

### file list

```diff
@@ -1,59 +1,60 @@
--rw-r--r--   0      501       20      776 2024-04-05 16:43:55.000000 pyontoenv-0.1.4a6/lib/Cargo.toml
--rw-r--r--   0      501       20     5324 2024-04-14 16:26:59.000000 pyontoenv-0.1.4a6/lib/src/config.rs
--rw-r--r--   0      501       20     2071 2024-04-06 02:39:54.000000 pyontoenv-0.1.4a6/lib/src/consts.rs
--rw-r--r--   0      501       20     3267 2024-04-05 19:54:52.000000 pyontoenv-0.1.4a6/lib/src/doctor.rs
--rw-r--r--   0      501       20      350 2024-04-14 15:35:07.000000 pyontoenv-0.1.4a6/lib/src/errors.rs
--rw-r--r--   0      501       20    40288 2024-04-14 23:31:38.000000 pyontoenv-0.1.4a6/lib/src/lib.rs
--rw-r--r--   0      501       20    13633 2024-04-14 04:36:13.000000 pyontoenv-0.1.4a6/lib/src/ontology.rs
--rw-r--r--   0      501       20     3521 2024-04-05 19:55:30.000000 pyontoenv-0.1.4a6/lib/src/policy.rs
--rw-r--r--   0      501       20     6428 2024-04-14 16:50:33.000000 pyontoenv-0.1.4a6/lib/src/util.rs
--rw-r--r--   0      501       20  1689944 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/Brick-1.3.ttl
--rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/model
--rw-r--r--   0      501       20      321 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/model.n3
--rw-r--r--   0      501       20      537 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/model.nt
--rw-r--r--   0      501       20     1248 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/model.ttl
--rw-r--r--   0      501       20      789 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/model.xml
--rw-r--r--   0      501       20      909 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0      501       20   146214 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0      501       20    30521 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0      501       20   163975 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0      501       20    18438 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0      501       20  1323794 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0      501       20    17472 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0      501       20  1456008 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0      501       20   104496 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0      501       20  1255550 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/bacnet.ttl
--rw-r--r--   0      501       20    44502 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/brickpatches.ttl
--rw-r--r--   0      501       20    81761 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/rec.ttl
--rw-r--r--   0      501       20     4069 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/recimports.ttl
--rw-r--r--   0      501       20    11876 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/lib/tests/data/support/ref-schema.ttl
--rw-r--r--   0      501       20     1160 2024-04-09 16:33:12.000000 pyontoenv-0.1.4a6/lib/tests/data2/ont1.ttl
--rw-r--r--   0      501       20     1132 2024-04-09 16:33:13.000000 pyontoenv-0.1.4a6/lib/tests/data2/ont2.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 16:33:29.000000 pyontoenv-0.1.4a6/lib/tests/data2/ont3.ttl
--rw-r--r--   0      501       20     1106 2024-04-09 16:33:46.000000 pyontoenv-0.1.4a6/lib/tests/data2/ont4.ttl
--rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a6/lib/tests/fileendings/model
--rw-r--r--   0      501       20      321 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a6/lib/tests/fileendings/model.n3
--rw-r--r--   0      501       20      537 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a6/lib/tests/fileendings/model.nt
--rw-r--r--   0      501       20     1248 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a6/lib/tests/fileendings/model.ttl
--rw-r--r--   0      501       20      789 2024-04-09 16:46:26.000000 pyontoenv-0.1.4a6/lib/tests/fileendings/model.xml
--rw-r--r--   0      501       20  1689944 2024-04-03 15:52:01.000000 pyontoenv-0.1.4a6/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
--rw-r--r--   0      501       20     1160 2024-04-09 19:04:23.000000 pyontoenv-0.1.4a6/lib/tests/updates/v1/ont1.ttl
--rw-r--r--   0      501       20     1132 2024-04-09 19:04:23.000000 pyontoenv-0.1.4a6/lib/tests/updates/v1/ont2.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 19:04:48.000000 pyontoenv-0.1.4a6/lib/tests/updates/v1/ont3.ttl
--rw-r--r--   0      501       20     1106 2024-04-09 19:05:31.000000 pyontoenv-0.1.4a6/lib/tests/updates/v1/ont4.ttl
--rw-r--r--   0      501       20     1135 2024-04-09 19:05:07.000000 pyontoenv-0.1.4a6/lib/tests/updates/v2/ont3.ttl
--rw-r--r--   0      501       20     1129 2024-04-10 00:42:38.000000 pyontoenv-0.1.4a6/lib/tests/updates/v2/ont5.ttl
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a6/python/Cargo.toml
--rw-r--r--   0      501       20     2886 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/python/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/python/.gitignore
--rw-r--r--   0      501       20       71 2024-03-28 12:07:46.000000 pyontoenv-0.1.4a6/python/build.rs
--rw-r--r--   0      501       20     5241 2024-04-14 04:04:40.000000 pyontoenv-0.1.4a6/python/poetry.lock
--rw-r--r--   0      501       20       71 2024-04-05 23:45:30.000000 pyontoenv-0.1.4a6/python/requirements.dev.txt
--rw-r--r--   0      501       20    12301 2024-04-15 01:47:24.000000 pyontoenv-0.1.4a6/python/src/lib.rs
--rw-r--r--   0      501       20      484 2024-04-15 01:39:02.000000 pyontoenv-0.1.4a6/python/test.py
--rw-r--r--   0      501       20      206 2024-04-13 23:20:44.000000 pyontoenv-0.1.4a6/python/token
--rw-r--r--   0      501       20    73476 2024-04-15 01:47:17.000000 pyontoenv-0.1.4a6/Cargo.lock
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a6/Cargo.toml
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a6/pyproject.toml
--rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 pyontoenv-0.1.4a6/PKG-INFO
+-rw-r--r--   0     1001      127      776 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/Cargo.toml
+-rw-r--r--   0     1001      127     5324 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/config.rs
+-rw-r--r--   0     1001      127     2180 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/consts.rs
+-rw-r--r--   0     1001      127     3267 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/doctor.rs
+-rw-r--r--   0     1001      127      350 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/errors.rs
+-rw-r--r--   0     1001      127    38576 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/lib.rs
+-rw-r--r--   0     1001      127    13633 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/ontology.rs
+-rw-r--r--   0     1001      127     3521 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/policy.rs
+-rw-r--r--   0     1001      127     4646 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/transform.rs
+-rw-r--r--   0     1001      127     6428 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/src/util.rs
+-rw-r--r--   0     1001      127  1689944 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/Brick-1.3.ttl
+-rw-r--r--   0     1001      127     1248 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model
+-rw-r--r--   0     1001      127      321 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model.n3
+-rw-r--r--   0     1001      127      537 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model.nt
+-rw-r--r--   0     1001      127     1248 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model.ttl
+-rw-r--r--   0     1001      127      789 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/model.xml
+-rw-r--r--   0     1001      127      909 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   146214 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0     1001      127    30521 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   163975 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0     1001      127  1323794 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127    17472 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127  1456008 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127   104496 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0     1001      127  1255550 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/bacnet.ttl
+-rw-r--r--   0     1001      127    44502 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/brickpatches.ttl
+-rw-r--r--   0     1001      127    81761 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/rec.ttl
+-rw-r--r--   0     1001      127     4069 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/recimports.ttl
+-rw-r--r--   0     1001      127    11876 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data/support/ref-schema.ttl
+-rw-r--r--   0     1001      127     1160 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data2/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data2/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data2/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/data2/ont4.ttl
+-rw-r--r--   0     1001      127     1248 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model
+-rw-r--r--   0     1001      127      321 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model.n3
+-rw-r--r--   0     1001      127      537 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model.nt
+-rw-r--r--   0     1001      127     1248 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model.ttl
+-rw-r--r--   0     1001      127      789 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/fileendings/model.xml
+-rw-r--r--   0     1001      127  1689944 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
+-rw-r--r--   0     1001      127     1160 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v1/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v1/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v1/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v1/ont4.ttl
+-rw-r--r--   0     1001      127     1135 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v2/ont3.ttl
+-rw-r--r--   0     1001      127     1129 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/lib/tests/updates/v2/ont5.ttl
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.5/python/Cargo.toml
+-rw-r--r--   0     1001      127     2886 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/.gitignore
+-rw-r--r--   0     1001      127      731 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/README.md
+-rw-r--r--   0     1001      127       71 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/build.rs
+-rw-r--r--   0     1001      127     5241 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/poetry.lock
+-rw-r--r--   0     1001      127       71 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/requirements.dev.txt
+-rw-r--r--   0     1001      127    14479 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/src/lib.rs
+-rw-r--r--   0     1001      127      694 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/python/test.py
+-rw-r--r--   0     1001      127    73924 2024-04-28 23:37:31.000000 pyontoenv-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 pyontoenv-0.1.5/Cargo.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1374 1970-01-01 00:00:00.000000 pyontoenv-0.1.5/PKG-INFO
```

### Comparing `pyontoenv-0.1.4a6/lib/Cargo.toml` & `pyontoenv-0.1.5/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/src/config.rs` & `pyontoenv-0.1.5/lib/src/config.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/src/consts.rs` & `pyontoenv-0.1.5/lib/src/consts.rs`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 pub const HAS_GRAPH_METADATA: NamedNodeRef<'_> =
     NamedNodeRef::new_unchecked("http://www.linkedmodel.org/schema/vaem#hasGraphMetadata");
 pub const REVISION: NamedNodeRef<'_> =
     NamedNodeRef::new_unchecked("http://www.linkedmodel.org/schema/vaem#revision");
 // shacl
 pub const PREFIXES: NamedNodeRef<'_> =
     NamedNodeRef::new_unchecked("http://www.w3.org/ns/shacl#prefixes");
+pub const DECLARE: NamedNodeRef<'_> =
+    NamedNodeRef::new_unchecked("http://www.w3.org/ns/shacl#declare");
 
 pub const ONTOLOGY_VERSION_IRIS: [NamedNodeRef<'_>; 10] = [
     VERSION_INFO,
     VERSION_IRI,
     DEFINED_BY,
     SEE_ALSO,
     CREATED,
```

### Comparing `pyontoenv-0.1.4a6/lib/src/doctor.rs` & `pyontoenv-0.1.5/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/src/lib.rs` & `pyontoenv-0.1.5/lib/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pub mod consts;
 pub mod doctor;
 pub mod errors;
 pub mod ontology;
 pub mod policy;
 #[macro_use]
 pub mod util;
+pub mod transform;
 
 use crate::config::Config;
 use crate::consts::{IMPORTS, ONTOLOGY, PREFIXES, TYPE};
 use crate::doctor::{Doctor, DuplicateOntology, OntologyDeclaration};
 use crate::ontology::{GraphIdentifier, Ontology, OntologyLocation};
 use anyhow::Result;
 use chrono::prelude::*;
@@ -57,63 +58,75 @@
 
 #[derive(Serialize, Deserialize)]
 pub struct OntoEnv {
     config: Config,
     #[serde(serialize_with = "ontologies_ser", deserialize_with = "ontologies_de")]
     ontologies: HashMap<GraphIdentifier, Ontology>,
     dependency_graph: DiGraph<GraphIdentifier, (), petgraph::Directed>,
-    #[serde(skip, default = "default_store")]
-    store: Store,
     #[serde(skip)]
     read_only: bool,
 }
 
 // probably need some graph "identifier" that incorporates location and version..
 
 impl OntoEnv {
-    pub fn new(config: Config) -> Result<Self> {
+    pub fn new(config: Config, recreate: bool) -> Result<Self> {
         // create the config.root/.ontoenv directory so it exists before the store
         // is created
         let ontoenv_dir = config.root.join(".ontoenv");
+
+        // if recreate is False, raise an error if the directory already exists
+        if ontoenv_dir.exists() && !recreate {
+            return Err(anyhow::anyhow!(
+                "OntoEnv directory already exists: {:?}. Run 'refresh' or use the --recreate flag to recreate the environment.",
+                ontoenv_dir
+            ));
+        }
+
         std::fs::create_dir_all(&ontoenv_dir)?;
 
         // create the store in the root/.ontoenv/store.db directory
-        let store = Store::open(ontoenv_dir.join("store.db"))?;
         Ok(Self {
             config,
             ontologies: HashMap::new(),
             dependency_graph: DiGraph::new(),
-            store,
             read_only: false,
         })
     }
 
+    // TODO: add a read-only version? make this thread-safe?
+    fn store(&self) -> Result<Store> {
+        let ontoenv_dir = self.config.root.join(".ontoenv");
+        std::fs::create_dir_all(&ontoenv_dir)?;
+        Store::open(ontoenv_dir.join("store.db"))
+            .map_err(|e| anyhow::anyhow!("Could not open store: {}", e))
+    }
+
     pub fn new_readonly(config: Config) -> Result<Self> {
         // create the store in the root/.ontoenv/store.db directory
         let store = Store::open_secondary(config.root.join(".ontoenv/store.db"))?;
         Ok(Self {
             config,
             ontologies: HashMap::new(),
             dependency_graph: DiGraph::new(),
-            store,
             read_only: true,
         })
     }
 
     pub fn close(self) {}
 
     //TODO: add import_graph which imports a single graph into a given graph
 
     pub fn num_graphs(&self) -> usize {
         self.ontologies.len()
     }
 
     pub fn num_triples(&self) -> Result<usize> {
         // this construction coerces the error the the correct type
-        Ok(self.store.len()?)
+        Ok(self.store()?.len()?)
     }
 
     pub fn get_ontology_with_policy(
         &self,
         name: NamedNodeRef,
         policy: &dyn policy::ResolutionPolicy,
     ) -> Option<Ontology> {
@@ -144,27 +157,18 @@
             .find(|&ontology| ontology.location() == Some(location))
     }
 
     pub fn from_file(path: &Path) -> Result<Self> {
         let file = std::fs::File::open(path)?;
         let reader = BufReader::new(file);
         let env: OntoEnv = serde_json::from_reader(reader)?;
-        // load store from root/.ontoenv/store.db
-        let ontoenv_dir = env.config.root.join(".ontoenv");
-        let store = Store::open(ontoenv_dir.join("store.db"))?;
-        Ok(Self { store, read_only: false, ..env })
-    }
-
-    pub fn from_file_readonly(path: &Path) -> Result<Self> {
-        let file = std::fs::File::open(path)?;
-        let reader = BufReader::new(file);
-        let env: OntoEnv = serde_json::from_reader(reader)?;
-        // load store from root/.ontoenv/store.db
-        let store = Store::open_secondary(env.config.root.join(".ontoenv/store.db"))?;
-        Ok(Self { store, read_only: true, ..env })
+        Ok(Self {
+            read_only: false,
+            ..env
+        })
     }
 
     /// creates a new directory called .ontoenv in self.root and saves:
     /// - the configuration as ontoenv.json
     /// - all graphs in the environment as .ttl files
     /// - the dependency graph as a json file
     pub fn save_to_directory(&self) -> Result<()> {
@@ -172,19 +176,14 @@
         info!("Saving ontology environment to: {:?}", ontoenv_dir);
         std::fs::create_dir_all(&ontoenv_dir)?;
         // save the configuration
         let config_path = ontoenv_dir.join("ontoenv.json");
         let config_str = serde_json::to_string_pretty(&self)?;
         let mut file = std::fs::File::create(config_path)?;
         file.write_all(config_str.as_bytes())?;
-        // save the dependency graph
-        //let dep_graph_path = ontoenv_dir.join("dependency_graph.json");
-        //let dep_graph_str = serde_json::to_string_pretty(&self.dependency_graph)?;
-        //let mut file = std::fs::File::create(dep_graph_path)?;
-        //file.write_all(dep_graph_str.as_bytes())?;
         Ok(())
     }
 
     fn update_dependency_graph(&mut self, updated_ids: Option<Vec<GraphIdentifier>>) -> Result<()> {
         // traverse the owl:imports closure and build the dependency graph
         let mut stack: VecDeque<GraphIdentifier> = match updated_ids {
             Some(ids) => ids.into(),
@@ -205,15 +204,15 @@
                     continue;
                 }
                 info!("Adding import: {}", import);
                 let location = OntologyLocation::from_str(import.as_str())?;
                 let imp = match self.add_or_update_ontology_from_location(location) {
                     Ok(imp) => imp,
                     Err(e) => {
-                        error!("Failed to read ontology file: {}", e);
+                        error!("Failed to read ontology file {}: {}", import.as_str(), e);
                         continue;
                     }
                 };
                 stack.push_back(imp);
             }
         }
 
@@ -260,17 +259,18 @@
         for ontology in self.ontologies.keys() {
             let location = self
                 .ontologies
                 .get(ontology)
                 .ok_or(anyhow::anyhow!("Ontology not found"))?
                 .location();
             if let Some(location) = location {
-                // if location is a file and the file does not exist, remove the ontology
+                // if location is a file and the file does not exist or it is no longer in the set
+                // of included paths, remove the ontology
                 if let OntologyLocation::File(path) = location {
-                    if !path.exists() {
+                    if !path.exists() || !self.config.is_included(path) {
                         to_remove.push(ontology.clone());
                     }
                 }
             }
         }
         for ontology in to_remove.iter() {
             debug!("Removing ontology: {:?}", ontology);
@@ -396,18 +396,16 @@
         };
 
         // Step four: update the dependency graph for all updated ontologies
         info!("Updating dependency graphs for updated ontologies");
         self.update_dependency_graph(Some(updated_ids))?;
 
         // optimize the store for storage + queries
-        if !self.read_only {
-            info!("Optimizing store");
-            self.store.optimize()?;
-        }
+        info!("Optimizing store");
+        self.store()?.optimize()?;
 
         Ok(())
     }
 
     /// Returns the GraphViz dot representation of the dependency graph
     pub fn dep_graph_to_dot(&self) -> Result<String> {
         self.rooted_dep_graph_to_dot(self.ontologies.keys().cloned().collect())
@@ -524,27 +522,29 @@
 
         // if the graph is already in the store, remove it and add the new graph
         let graphname: NamedOrBlankNode = match id.graphname()? {
             GraphName::NamedNode(n) => NamedOrBlankNode::NamedNode(n),
             _ => return Err(anyhow::anyhow!("Graph name not found")),
         };
 
-        if self.store.contains_named_graph(graphname.as_ref())? {
-            self.store.remove_named_graph(graphname.as_ref())?;
+        let store = self.store()?;
+
+        if store.contains_named_graph(graphname.as_ref())? {
+            store.remove_named_graph(graphname.as_ref())?;
         }
 
         info!("Adding graph to store: {:?}", graphname);
         for triple in graph.into_iter() {
             let q: QuadRef = QuadRef::new(
                 triple.subject,
                 triple.predicate,
                 triple.object,
                 graphname.as_ref(),
             );
-            self.store.insert(q)?;
+            store.insert(q)?;
         }
 
         Ok(id)
     }
 
     pub fn graph_ids(&self) -> Vec<GraphIdentifier> {
         self.ontologies.keys().cloned().collect()
@@ -565,18 +565,16 @@
         }
         graphs
     }
 
     pub fn get_graph(&self, id: &GraphIdentifier) -> Result<Graph> {
         let mut graph = Graph::new();
         let name = id.graphname()?;
-        for quad in self
-            .store
-            .quads_for_pattern(None, None, None, Some(name.as_ref()))
-        {
+        let store = self.store()?;
+        for quad in store.quads_for_pattern(None, None, None, Some(name.as_ref())) {
             graph.insert(quad?.as_ref());
         }
         Ok(graph)
     }
 
     /// Returns a table of metadata for the given graph
     pub fn graph_metadata(&self, id: &GraphIdentifier) -> HashMap<String, String> {
@@ -638,88 +636,47 @@
         &self,
         graph_ids: &[GraphIdentifier],
         rewrite_sh_prefixes: Option<bool>,
         remove_owl_imports: Option<bool>,
     ) -> Result<Dataset> {
         // compute union of all graphs
         let mut union: Dataset = Dataset::new();
+        let store = self.store()?;
         for id in graph_ids {
             let graphname: NamedOrBlankNode = match id.graphname()? {
                 GraphName::NamedNode(n) => NamedOrBlankNode::NamedNode(n),
                 _ => continue,
             };
 
-            if !self.store.contains_named_graph(graphname.as_ref())? {
+            if !store.contains_named_graph(graphname.as_ref())? {
                 return Err(anyhow::anyhow!("Graph not found: {:?}", id));
             }
 
             let mut count = 0;
-            for quad in
-                self.store
-                    .quads_for_pattern(None, None, None, Some(id.graphname()?.as_ref()))
-            {
+            for quad in store.quads_for_pattern(None, None, None, Some(id.graphname()?.as_ref())) {
                 count += 1;
                 union.insert(quad?.as_ref());
             }
             info!("Added {} triples from graph: {:?}", count, id);
-
-            //let d = g.into_dataset();
-            //graph.insert_all(d.quads())?;
         }
         let first_id = graph_ids
             .first()
             .ok_or(anyhow::anyhow!("No graphs found"))?;
         let root_ontology: SubjectRef = SubjectRef::NamedNode(first_id.name());
 
         // Rewrite sh:prefixes
         // defaults to true if not specified
         if let Some(true) = rewrite_sh_prefixes.or(Some(true)) {
-            // rewrite sh:prefixes
-            // the ontology is the first graph in the list
-            let mut to_remove: Vec<Quad> = vec![];
-            let mut to_add: Vec<Quad> = vec![];
-            info!("Rewriting sh:prefixes to point to: {:?}", root_ontology);
-            for quad in union.quads_for_predicate(PREFIXES) {
-                let s = quad.subject;
-                let g = quad.graph_name;
-                let new_quad = QuadRef::new(s, PREFIXES, root_ontology, g);
-                to_remove.push(quad.into());
-                to_add.push(new_quad.into());
-            }
-            for quad in to_remove {
-                union.remove(quad.as_ref());
-            }
-            for quad in to_add {
-                union.insert(quad.as_ref());
-            }
+            transform::rewrite_sh_prefixes(&mut union, root_ontology);
         }
         // remove owl:imports
         if let Some(true) = remove_owl_imports.or(Some(true)) {
-            // remove owl:imports
-            let mut to_remove: Vec<Quad> = vec![];
-            for quad in union.quads_for_predicate(IMPORTS) {
-                to_remove.push(quad.into());
-            }
-            for quad in to_remove {
-                union.remove(quad.as_ref());
-            }
-        }
-        // remove owl:Ontology declarations that are not the first graph
-        let mut to_remove: Vec<Quad> = vec![];
-        for quad in union.quads_for_object(ONTOLOGY) {
-            let s = quad.subject;
-            let p = quad.predicate;
-            if p == TYPE && s != root_ontology {
-                debug!("Removing ontology declaration: {:?}", s);
-                to_remove.push(quad.into());
-            }
-        }
-        for quad in to_remove {
-            union.remove(quad.as_ref());
+            transform::remove_owl_imports(&mut union)
         }
+        transform::remove_ontology_declarations(&mut union, root_ontology);
         Ok(union)
     }
 
     /// Returns a list of issues with the environment
     pub fn doctor(&self) {
         let mut doctor = Doctor::new();
         doctor.add_check(Box::new(DuplicateOntology {}));
```

### Comparing `pyontoenv-0.1.4a6/lib/src/ontology.rs` & `pyontoenv-0.1.5/lib/src/ontology.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/src/policy.rs` & `pyontoenv-0.1.5/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/src/util.rs` & `pyontoenv-0.1.5/lib/src/util.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/Brick-1.3.ttl` & `pyontoenv-0.1.5/lib/tests/data/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/model` & `pyontoenv-0.1.5/lib/tests/data/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/model.nt` & `pyontoenv-0.1.5/lib/tests/data/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/model.ttl` & `pyontoenv-0.1.5/lib/tests/data/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/model.xml` & `pyontoenv-0.1.5/lib/tests/data/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/bacnet.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/brickpatches.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/rec.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/recimports.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data/support/ref-schema.ttl` & `pyontoenv-0.1.5/lib/tests/data/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data2/ont1.ttl` & `pyontoenv-0.1.5/lib/tests/data2/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data2/ont2.ttl` & `pyontoenv-0.1.5/lib/tests/data2/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data2/ont3.ttl` & `pyontoenv-0.1.5/lib/tests/data2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/data2/ont4.ttl` & `pyontoenv-0.1.5/lib/tests/data2/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/fileendings/model` & `pyontoenv-0.1.5/lib/tests/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/fileendings/model.nt` & `pyontoenv-0.1.5/lib/tests/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/fileendings/model.ttl` & `pyontoenv-0.1.5/lib/tests/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/fileendings/model.xml` & `pyontoenv-0.1.5/lib/tests/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.5/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/updates/v1/ont1.ttl` & `pyontoenv-0.1.5/lib/tests/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/updates/v1/ont2.ttl` & `pyontoenv-0.1.5/lib/tests/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/updates/v1/ont3.ttl` & `pyontoenv-0.1.5/lib/tests/updates/v1/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/updates/v1/ont4.ttl` & `pyontoenv-0.1.5/lib/tests/updates/v1/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/updates/v2/ont3.ttl` & `pyontoenv-0.1.5/lib/tests/updates/v2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/lib/tests/updates/v2/ont5.ttl` & `pyontoenv-0.1.5/lib/tests/updates/v2/ont5.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/python/Cargo.toml` & `pyontoenv-0.1.5/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/python/.github/workflows/CI.yml` & `pyontoenv-0.1.5/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/python/.gitignore` & `pyontoenv-0.1.5/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/python/poetry.lock` & `pyontoenv-0.1.5/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.4a6/python/src/lib.rs` & `pyontoenv-0.1.5/python/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 use ::ontoenv as ontoenvrs;
 use ::ontoenv::consts::{ONTOLOGY, TYPE};
 use ::ontoenv::ontology::OntologyLocation;
+use ::ontoenv::transform;
 use anyhow::Error;
-use oxigraph::model::{BlankNode, Literal, NamedNode, NamedNodeRef, Term};
+use oxigraph::model::{BlankNode, Literal, NamedNode, NamedNodeRef, Term, SubjectRef};
 use pyo3::{
     prelude::*,
-    types::{PyBool, PyString, PyTuple},
+    types::{PyBool, PyString, PyTuple, IntoPyDict},
 };
 use std::borrow::Borrow;
 use std::path::{Path, PathBuf};
 use std::sync::Once;
 
 static INIT: Once = Once::new();
 
@@ -118,22 +119,22 @@
 struct Config {
     cfg: ontoenvrs::config::Config,
 }
 
 #[pymethods]
 impl Config {
     #[new]
-    #[pyo3(signature = (root, search_directories, require_ontology_names=false, strict=false, offline=false, resolution_policy="default".to_owned(), includes=vec![], excludes=vec![]))]
+    #[pyo3(signature = (search_directories, require_ontology_names=false, strict=false, offline=false, resolution_policy="default".to_owned(), root=".".to_owned(), includes=vec![], excludes=vec![]))]
     fn new(
-        root: String,
         search_directories: Vec<String>,
         require_ontology_names: bool,
         strict: bool,
         offline: bool,
         resolution_policy: String,
+        root: String,
         includes: Option<Vec<String>>,
         excludes: Option<Vec<String>>,
     ) -> PyResult<Self> {
         Ok(Config {
             cfg: ontoenvrs::config::Config::new(
                 root.to_string().into(),
                 Some(
@@ -166,50 +167,42 @@
 struct OntoEnv {
     inner: ontoenvrs::OntoEnv,
 }
 
 #[pymethods]
 impl OntoEnv {
     #[new]
-    #[pyo3(signature = (config=None, read_only=false, path=Path::new(".").to_owned()))]
+    #[pyo3(signature = (config=None, path=Path::new(".").to_owned(), recreate=false))]
     fn new(
         _py: Python,
         config: Option<&Bound<'_, Config>>,
-        read_only: bool,
         path: Option<PathBuf>,
+        recreate: bool,
     ) -> PyResult<Self> {
         // wrap env_logger::init() in a Once to ensure it's only called once. This can
         // happen if a user script creates multiple OntoEnv instances
         INIT.call_once(|| {
             env_logger::init();
         });
 
         let mut env = if let Some(p) = path {
             let config_path = p.join(".ontoenv").join("ontoenv.json");
-            if read_only {
-                let e = ontoenvrs::OntoEnv::from_file_readonly(&config_path)
-                    .map_err(anyhow_to_pyerr)?;
+            if let Ok(e) = ontoenvrs::OntoEnv::from_file(&config_path) {
                 println!("Loaded OntoEnv from file");
                 OntoEnv { inner: e }
             } else {
-                if let Ok(e) = ontoenvrs::OntoEnv::from_file(&config_path) {
-                    println!("Loaded OntoEnv from file");
-                    OntoEnv { inner: e }
-                } else {
-                    println!("Creating new OntoEnv");
-                    OntoEnv {
-                        inner: ontoenvrs::OntoEnv::new(config.unwrap().borrow().cfg.clone())
-                            .map_err(anyhow_to_pyerr)?,
-                    }
+                println!("Creating new OntoEnv");
+                OntoEnv {
+                    inner: ontoenvrs::OntoEnv::new(config.unwrap().borrow().cfg.clone(), recreate)
+                        .map_err(anyhow_to_pyerr)?,
                 }
             }
         } else {
-            println!("Creating new OntoEnv");
             OntoEnv {
-                inner: ontoenvrs::OntoEnv::new(config.unwrap().borrow().cfg.clone())
+                inner: ontoenvrs::OntoEnv::new(config.unwrap().borrow().cfg.clone(), recreate)
                     .map_err(anyhow_to_pyerr)?,
             }
         };
 
         env.inner.update().map_err(anyhow_to_pyerr)?;
         env.inner.save_to_directory().map_err(anyhow_to_pyerr)?;
         Ok(env)
@@ -226,14 +219,64 @@
         Ok(format!(
             "<OntoEnv: {} graphs, {} triples>",
             self.inner.num_graphs(),
             self.inner.num_triples().map_err(anyhow_to_pyerr)?
         ))
     }
 
+    fn import_graph(&self, py: Python, destination_graph: &Bound<'_, PyAny>, uri: &str) -> PyResult<()> {
+        let rdflib = py.import_bound("rdflib")?;
+        let iri = NamedNode::new(uri)
+            .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
+        let ont = self
+            .inner
+            .get_ontology_by_name(iri.as_ref())
+            .ok_or_else(|| PyErr::new::<pyo3::exceptions::PyValueError, _>("Ontology not found"))?;
+        let mut graph = ont.graph().map_err(anyhow_to_pyerr)?;
+
+        // get the owl:Ontology IRI from the destination_graph
+        // call value with TYPE and ONTOLOGY
+        let uriref_constructor = rdflib.getattr("URIRef")?;
+        let type_uri = uriref_constructor.call1((TYPE.as_str(),))?;
+        let ontology_uri = uriref_constructor.call1((ONTOLOGY.as_str(),))?;
+        let kwargs = [("predicate", type_uri), ("object", ontology_uri)].into_py_dict_bound(py);
+        let result = destination_graph.call_method("value", (), Some(&kwargs))?;
+        if !result.is_none() {
+            // extract the IRI from the result, turn into a SubjectRef
+            let ontology = NamedNode::new(result.extract::<String>()?).map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
+            let base_ontology: SubjectRef = SubjectRef::NamedNode(ontology.as_ref());
+
+            // apply the transforms to make the graph compatible with the destination graph
+            transform::rewrite_sh_prefixes_graph(&mut graph, base_ontology);
+            transform::remove_ontology_declarations_graph(&mut graph, base_ontology);
+        }
+        transform::remove_owl_imports_graph(&mut graph);
+
+        Python::with_gil(|_py| {
+            for triple in graph.into_iter() {
+                let s: Term = triple.subject.into();
+                let p: Term = triple.predicate.into();
+                let o: Term = triple.object.into();
+
+                let t = PyTuple::new_bound(
+                    destination_graph.py(),
+                    &[
+                        term_to_python(destination_graph.py(), &rdflib, s)?,
+                        term_to_python(destination_graph.py(), &rdflib, p)?,
+                        term_to_python(destination_graph.py(), &rdflib, o)?,
+                    ],
+                );
+
+                destination_graph.getattr("add")?.call1((t,))?;
+            }
+            Ok::<(), PyErr>(())
+        })?;
+        Ok(())
+    }
+
     #[pyo3(signature = (uri, destination_graph, rewrite_sh_prefixes=false, remove_owl_imports=false))]
     fn get_closure(
         &self,
         py: Python,
         uri: &str,
         destination_graph: &Bound<'_, PyAny>,
         rewrite_sh_prefixes: bool,
```

### Comparing `pyontoenv-0.1.4a6/Cargo.lock` & `pyontoenv-0.1.5/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,20 @@
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
+name = "base64"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+
+[[package]]
 name = "bindgen"
 version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
 dependencies = [
  "bitflags 2.5.0",
  "cexpr",
@@ -160,15 +166,15 @@
  "log",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
- "syn 2.0.58",
+ "syn 2.0.60",
  "which",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -199,20 +205,21 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.92"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
@@ -224,25 +231,25 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "serde",
  "wasm-bindgen",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "clang-sys"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "67523a3b4be3ce1989d607a828d036249522dd9c1c8de7f4dd2dae43a37369d1"
@@ -279,15 +286,15 @@
 version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
  "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
@@ -380,15 +387,15 @@
 checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim 0.10.0",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
@@ -402,15 +409,15 @@
 name = "darling_macro"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core 0.20.8",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "decoded-char"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5440d1dc8ea7cae44cda3c64568db29bfa2434aba51ae66a50c00488841a65a3"
@@ -475,17 +482,17 @@
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "encoding_rs"
 version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
@@ -529,17 +536,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
@@ -631,15 +638,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -738,17 +745,17 @@
 checksum = "43a3c133739dddd0d2990f9a4bdf8eb4b21ef50e4851ca85ab661199821d510e"
 dependencies = [
  "ahash 0.8.11",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -903,15 +910,15 @@
 [[package]]
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
  "serde",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -946,17 +953,17 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.28"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -1230,28 +1237,28 @@
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "locspan"
@@ -1400,15 +1407,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.4-alpha6"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1426,15 +1433,15 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.4-alpha6"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
@@ -1459,15 +1466,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1560,70 +1567,70 @@
 checksum = "edeb0770b5afd066427e12e38998e15de7c2cc6048a5817bbb602130d42a55c9"
 dependencies = [
  "js-sys",
 ]
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "pct-str"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77d207ec8d182c2fef45f028b9b9507770df19e89b3e14827ccd95d4a23f6003"
 dependencies = [
  "utf8-decode",
 ]
 
 [[package]]
 name = "peg"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "400bcab7d219c38abf8bd7cc2054eb9bbbd4312d66f6a5557d572a203f646f61"
+checksum = "8a625d12ad770914cbf7eff6f9314c3ef803bfe364a1b20bc36ddf56673e71e5"
 dependencies = [
  "peg-macros",
  "peg-runtime",
 ]
 
 [[package]]
 name = "peg-macros"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46e61cce859b76d19090f62da50a9fe92bab7c2a5f09e183763559a2ac392c90"
+checksum = "f241d42067ed3ab6a4fece1db720838e1418f36d868585a27931f95d6bc03582"
 dependencies = [
  "peg-runtime",
  "proc-macro2",
  "quote",
 ]
 
 [[package]]
 name = "peg-runtime"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36bae92c60fa2398ce4678b98b2c4b5a7c61099961ca1fa305aec04a9ad28922"
+checksum = "e3aeb8f54c078314c2065ee649a7241f46b9d8e418e1a9581ba0546657d7aa3a"
 
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
@@ -1688,20 +1695,20 @@
 checksum = "a239bcdfda2c685fda1add3b4695c06225f50075e3cfb5b954e91545587edff2"
 dependencies = [
  "ryu_floating_decimal",
 ]
 
 [[package]]
 name = "prettyplease"
-version = "0.2.17"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8d3928fb5db768cb86f891ff014f0144589297e3c6a1aba6ed7cecfdace270c7"
+checksum = "5ac2cf0f2e4f42b49f5ffd07dae8d746508ef7526c13940e5f524012ae6c6550"
 dependencies = [
  "proc-macro2",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
@@ -1722,26 +1729,26 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -1749,60 +1756,60 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck 0.4.1",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.4-alpha6"
+version = "0.1.5"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
@@ -1907,19 +1914,19 @@
 checksum = "678054eb77286b51581ba43620cc911abf02758c91f93f479767aed0f90458b2"
 dependencies = [
  "rand_core 0.3.1",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
@@ -1958,15 +1965,15 @@
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
- "base64",
+ "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -2035,32 +2042,32 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
 dependencies = [
- "base64",
+ "base64 0.21.7",
 ]
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
@@ -2122,37 +2129,37 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.199"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -2175,40 +2182,40 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_with"
-version = "3.7.0"
+version = "3.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee80b0e361bbf88fd2f6e242ccd19cfda072cb0faa6ae694ecee08199938569a"
+checksum = "0ad483d2ab0149d5a5ebcd9972a3852711e0153d863bf5a5d0391d28883c4a20"
 dependencies = [
- "base64",
+ "base64 0.22.0",
  "chrono",
  "hex",
  "indexmap 1.9.3",
  "indexmap 2.2.6",
  "serde",
  "serde_derive",
  "serde_json",
  "serde_with_macros",
  "time",
 ]
 
 [[package]]
 name = "serde_with_macros"
-version = "3.7.0"
+version = "3.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6561dc161a9224638a31d876ccdfefbc1df91d3f3a8342eddb35f055d48c7655"
+checksum = "65569b702f41443e8bc8bbb1c5779bd0450bbe723b56198980e80ec45780bce2"
 dependencies = [
  "darling 0.20.8",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "sha-1"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f5058ada175748e33390e40e872bd0fe59a19f265d0158daa551c5a88a76009c"
@@ -2335,17 +2342,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2401,37 +2408,37 @@
  "fastrand",
  "rustix",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.35"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef89ece63debf11bc32d1ed8d078ac870cbeb44da02afb02a9ff135ae7ca0582"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
@@ -2649,15 +2656,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2683,15 +2690,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2734,34 +2741,34 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
@@ -2771,15 +2778,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -2791,110 +2798,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
@@ -2915,9 +2929,9 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.58",
+ "syn 2.0.60",
 ]
```

### Comparing `pyontoenv-0.1.4a6/Cargo.toml` & `pyontoenv-0.1.5/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.4-alpha6"
+version = "0.1.5"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
```

### Comparing `pyontoenv-0.1.4a6/pyproject.toml` & `pyontoenv-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.4a6"
+version = "0.1.5"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

