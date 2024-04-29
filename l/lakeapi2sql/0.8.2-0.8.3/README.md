# Comparing `tmp/lakeapi2sql-0.8.2.tar.gz` & `tmp/lakeapi2sql-0.8.3.tar.gz`

## Comparing `lakeapi2sql-0.8.2.tar` & `lakeapi2sql-0.8.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.2/Cargo.toml
--rw-r--r--   0     1001      127      118 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/.editorconfig
--rw-r--r--   0     1001      127     2966 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     3110 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/.gitignore
--rw-r--r--   0     1001      127       76 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/.vscode/settings.json
--rw-r--r--   0     1001      127     1081 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/LICENSE
--rw-r--r--   0     1001      127     1388 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/README.md
--rw-r--r--   0     1001      127        0 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      127     3102 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      127        0 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/py.typed
--rw-r--r--   0     1001      127    22394 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/src/arrow_convert.rs
--rw-r--r--   0     1001      127     6809 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/src/bulk_insert.rs
--rw-r--r--   0     1001      127     1519 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/src/connect.rs
--rw-r--r--   0     1001      127     5190 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/test/__init__.py
--rw-r--r--   0     1001      127     1649 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/test/test_insert.py
--rw-r--r--   0     1001      127     1663 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/test/test_insert_reader.py
--rw-r--r--   0     1001      127    69760 2024-04-16 07:23:45.000000 lakeapi2sql-0.8.2/Cargo.lock
--rw-r--r--   0     1001      127      693 2024-04-16 07:23:40.000000 lakeapi2sql-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.3/Cargo.toml
+-rw-r--r--   0     1001      127      118 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/.editorconfig
+-rw-r--r--   0     1001      127     2966 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     3110 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/.gitignore
+-rw-r--r--   0     1001      127       76 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/.vscode/settings.json
+-rw-r--r--   0     1001      127     1081 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/LICENSE
+-rw-r--r--   0     1001      127     1388 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/README.md
+-rw-r--r--   0     1001      127        0 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      127     3102 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      127        0 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/py.typed
+-rw-r--r--   0     1001      127    22898 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/src/arrow_convert.rs
+-rw-r--r--   0     1001      127     6809 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/src/bulk_insert.rs
+-rw-r--r--   0     1001      127     1519 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/src/connect.rs
+-rw-r--r--   0     1001      127     5190 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/test/__init__.py
+-rw-r--r--   0     1001      127     1649 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/test/test_insert.py
+-rw-r--r--   0     1001      127     1663 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/test/test_insert_reader.py
+-rw-r--r--   0     1001      127    69775 2024-04-29 09:22:52.000000 lakeapi2sql-0.8.3/Cargo.lock
+-rw-r--r--   0     1001      127      693 2024-04-29 09:22:42.000000 lakeapi2sql-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.3/PKG-INFO
```

### Comparing `lakeapi2sql-0.8.2/Cargo.toml` & `lakeapi2sql-0.8.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lake2sql"
-version = "0.8.1"
+version = "0.8.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "lake2sql"
 crate-type = ["lib", "cdylib"]
```

### Comparing `lakeapi2sql-0.8.2/.github/workflows/CI.yml` & `lakeapi2sql-0.8.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/.gitignore` & `lakeapi2sql-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/LICENSE` & `lakeapi2sql-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/README.md` & `lakeapi2sql-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/lakeapi2sql/bulk_insert.py` & `lakeapi2sql-0.8.3/lakeapi2sql/bulk_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/src/arrow_convert.rs` & `lakeapi2sql-0.8.3/src/arrow_convert.rs`

 * *Files 1% similar despite different names*

```diff
@@ -348,19 +348,29 @@
                 for val in ba.iter() {
                     token_rows[rowindex].push(ColumnData::F32(val));
                     rowindex += 1;
                 }
             }
             arrow::datatypes::DataType::Float64 => {
                 let ba = col.as_any().downcast_ref::<Float64Array>().unwrap();
-
-                let mut rowindex = 0;
-                for val in ba.iter() {
-                    token_rows[rowindex].push(ColumnData::F64(val));
-                    rowindex += 1;
+                if coltype == &ColumnType::Int4 || coltype == &ColumnType::Intn {
+                    let mut rowindex = 0;
+                    for val in ba.iter() {
+                        token_rows[rowindex].push(ColumnData::I32(match val {
+                            Some(v) => Some(v as i32),
+                            None => None,
+                        }));
+                        rowindex += 1;
+                    }
+                } else {
+                    let mut rowindex = 0;
+                    for val in ba.iter() {
+                        token_rows[rowindex].push(ColumnData::F64(val));
+                        rowindex += 1;
+                    }
                 }
             }
             arrow::datatypes::DataType::Date32 => {
                 let ba = col.as_any().downcast_ref::<Date32Array>().unwrap();
                 if coltype == &ColumnType::Datetime || coltype == &ColumnType::Datetimen {
                     let mut rowindex = 0;
                     for val in ba.iter() {
```

### Comparing `lakeapi2sql-0.8.2/src/bulk_insert.rs` & `lakeapi2sql-0.8.3/src/bulk_insert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/src/connect.rs` & `lakeapi2sql-0.8.3/src/connect.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/src/lib.rs` & `lakeapi2sql-0.8.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/test/test_insert.py` & `lakeapi2sql-0.8.3/test/test_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/test/test_insert_reader.py` & `lakeapi2sql-0.8.3/test/test_insert_reader.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.2/Cargo.lock` & `lakeapi2sql-0.8.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 dependencies = [
  "ahash 0.8.11",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
 version = "48.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -250,15 +250,15 @@
 dependencies = [
  "ahash 0.8.11",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
 ]
 
 [[package]]
 name = "arrow-schema"
 version = "48.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aaf4d737bba93da59f16129bec21e087aed0be84ff840e74146d4703879436cb"
@@ -312,15 +312,15 @@
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "asynchronous-codec"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4057f2c32adbb2fc158e22fb38433c8e9bbf76b75a4732c7c0cbaf695fb65568"
@@ -399,15 +399,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "51670c3aa053938b0ee3bd67c3817e471e626151131b934038e83c5bf8de48f5"
 dependencies = [
  "once_cell",
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
  "syn_derive",
 ]
 
 [[package]]
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -445,20 +445,21 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -581,15 +582,15 @@
 name = "enumflags2_derive"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c785274071b1b420972453b306eeca06acf4633829db4223b58a2a8c5953bc4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
@@ -602,17 +603,17 @@
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
 name = "flatbuffers"
 version = "23.5.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dac53e22462d78c16d64a1cd22371b54cc3fe94aa15e7886a2fa6e5d1ab8640"
 dependencies = [
@@ -708,15 +709,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -810,17 +811,17 @@
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
  "ahash 0.7.8",
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
 
@@ -951,15 +952,15 @@
 [[package]]
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
@@ -974,17 +975,17 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -992,15 +993,15 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lake2sql"
-version = "0.8.1"
+version = "0.8.3"
 dependencies = [
  "arrow",
  "futures",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
@@ -1098,17 +1099,17 @@
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
 name = "log"
@@ -1316,15 +1317,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1339,33 +1340,33 @@
  "libc",
  "pkg-config",
  "vcpkg",
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
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
@@ -1442,17 +1443,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -1552,28 +1553,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
@@ -1656,19 +1657,19 @@
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
 dependencies = [
  "rand_core 0.5.1",
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
@@ -1824,30 +1825,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
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
 name = "rustls"
-version = "0.21.10"
+version = "0.21.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "3f56a14d1f48b391359b22f731fd4bd7e43c97f3c50eee276f3aa09c94784d3e"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -1946,30 +1947,30 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
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
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
@@ -2043,17 +2044,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.59"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2061,15 +2062,15 @@
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1329189c02ff984e9736652b1631330da25eaa6bc639089ed4915d25446cbe7b"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
@@ -2117,30 +2118,30 @@
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
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tiberius"
 version = "0.12.2"
 source = "git+https://github.com/aersam/tiberius.git?branch=bulk#8cee1fe5d765358ca568c96423766ae3b582b9e8"
 dependencies = [
@@ -2235,15 +2236,15 @@
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -2316,15 +2317,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -2448,15 +2449,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2482,15 +2483,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -2744,15 +2745,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.60",
 ]
 
 [[package]]
 name = "zstd"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
```

### Comparing `lakeapi2sql-0.8.2/pyproject.toml` & `lakeapi2sql-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.8.2"
+version = "0.8.3"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = ["pyarrow >= 8.0.0"]
```

### Comparing `lakeapi2sql-0.8.2/PKG-INFO` & `lakeapi2sql-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lakeapi2sql
-Version: 0.8.2
+Version: 0.8.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: azure-identity >=1.12.0 ; extra == 'azure'
 Provides-Extra: azure
 License-File: LICENSE
```

