# Comparing `tmp/moyopy-0.1.7.tar.gz` & `tmp/moyopy-0.1.8.tar.gz`

## Comparing `moyopy-0.1.7.tar` & `moyopy-0.1.8.tar`

### file list

```diff
@@ -1,65 +1,68 @@
--rw-r--r--   0     1001      127      903 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/Cargo.toml
--rw-r--r--   0     1001      127      245 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/README.md
--rw-r--r--   0     1001      127      703 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/benches/dataset.rs
--rw-r--r--   0     1001      127     2493 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/benches/translation_search.rs
--rw-r--r--   0     1001      127     2926 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/base/cell.rs
--rw-r--r--   0     1001      127     1123 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/base/error.rs
--rw-r--r--   0     1001      127     2932 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/base/lattice.rs
--rw-r--r--   0     1001      127     3830 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/base/operation.rs
--rw-r--r--   0     1001      127     2146 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/base/tolerance.rs
--rw-r--r--   0     1001      127     9891 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/base/transformation.rs
--rw-r--r--   0     1001      127      559 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/base.rs
--rw-r--r--   0     1001      127     8405 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/data/arithmetic_crystal_class.rs
--rw-r--r--   0     1001      127     7841 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/data/classification.rs
--rw-r--r--   0     1001      127    20576 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/data/hall_symbol.rs
--rw-r--r--   0     1001      127    81241 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/data/hall_symbol_database.rs
--rw-r--r--   0     1001      127     7762 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/data/point_group.rs
--rw-r--r--   0     1001      127     3370 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/data/setting.rs
--rw-r--r--   0     1001      127   201241 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/data/wyckoff.rs
--rw-r--r--   0     1001      127      740 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/data.rs
--rw-r--r--   0     1001      127    19605 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/identify/point_group.rs
--rw-r--r--   0     1001      127    13483 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/identify/space_group.rs
--rw-r--r--   0     1001      127       68 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/identify.rs
--rw-r--r--   0     1001      127     8765 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/lib.rs
--rw-r--r--   0     1001      127      901 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math/cycle_checker.rs
--rw-r--r--   0     1001      127     5124 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math/delaunay.rs
--rw-r--r--   0     1001      127     2284 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math/elementary.rs
--rw-r--r--   0     1001      127     4148 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math/hnf.rs
--rw-r--r--   0     1001      127     2440 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math/integer_system.rs
--rw-r--r--   0     1001      127     7889 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math/minkowski.rs
--rw-r--r--   0     1001      127    14588 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math/niggli.rs
--rw-r--r--   0     1001      127     4889 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math/snf.rs
--rw-r--r--   0     1001      127      344 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/math.rs
--rw-r--r--   0     1001      127    11991 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/search/primitive_cell.rs
--rw-r--r--   0     1001      127    12095 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/search/solve.rs
--rw-r--r--   0     1001      127    12714 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/search/symmetry_search.rs
--rw-r--r--   0     1001      127      250 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/search.rs
--rw-r--r--   0     1001      127    14886 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/symmetrize/standardize.rs
--rw-r--r--   0     1001      127       94 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/src/symmetrize.rs
--rw-r--r--   0     1001      127     5985 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/assets/mp-1185639.json
--rw-r--r--   0     1001      127     5374 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/assets/mp-1197586.json
--rw-r--r--   0     1001      127     9958 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/assets/mp-1201492.json
--rw-r--r--   0     1001      127      820 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/assets/mp-1221598.json
--rw-r--r--   0     1001      127      735 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/assets/mp-1277787.json
--rw-r--r--   0     1001      127     3820 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/assets/mp-30665.json
--rw-r--r--   0     1001      127     1370 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/assets/mp-550745.json
--rw-r--r--   0     1001      127     5272 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/assets/mp-569901.json
--rw-r--r--   0     1001      127    20173 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyo/tests/test_moyo_dataset.rs
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 moyopy-0.1.7/moyopy/Cargo.toml
--rw-r--r--   0     1001      127      315 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/README.md
--rw-r--r--   0     1001      127       37 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/python/moyopy/__init__.py
--rw-r--r--   0     1001      127     2504 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/python/moyopy/_moyopy.pyi
--rw-r--r--   0     1001      127        0 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/python/moyopy/py.typed
--rw-r--r--   0     1001      127      623 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/python/tests/conftest.py
--rw-r--r--   0     1001      127      394 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/python/tests/test_moyo_dataset.py
--rw-r--r--   0     1001      127     4934 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/src/base.rs
--rw-r--r--   0     1001      127      704 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/src/data.rs
--rw-r--r--   0     1001      127     4123 2024-04-24 12:08:48.000000 moyopy-0.1.7/moyopy/src/lib.rs
--rw-r--r--   0     1001      127    42989 2024-04-24 12:08:48.000000 moyopy-0.1.7/Cargo.lock
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 moyopy-0.1.7/Cargo.toml
--rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 moyopy-0.1.7/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-04-24 12:08:48.000000 moyopy-0.1.7/python/moyopy/py.typed
--rw-r--r--   0     1001      127       37 2024-04-24 12:08:48.000000 moyopy-0.1.7/python/moyopy/__init__.py
--rw-r--r--   0     1001      127     2504 2024-04-24 12:08:48.000000 moyopy-0.1.7/python/moyopy/_moyopy.pyi
--rw-r--r--   0     1001      127      315 2024-04-24 12:08:48.000000 moyopy-0.1.7/README.md
--rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 moyopy-0.1.7/PKG-INFO
+-rw-r--r--   0     1001      127      799 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/Cargo.toml
+-rw-r--r--   0     1001      127      857 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/README.md
+-rw-r--r--   0     1001      127      703 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/benches/dataset.rs
+-rw-r--r--   0     1001      127     2493 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/benches/translation_search.rs
+-rw-r--r--   0     1001      127     3116 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/base/cell.rs
+-rw-r--r--   0     1001      127     1123 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/base/error.rs
+-rw-r--r--   0     1001      127     2932 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/base/lattice.rs
+-rw-r--r--   0     1001      127     3830 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/base/operation.rs
+-rw-r--r--   0     1001      127     2291 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/base/tolerance.rs
+-rw-r--r--   0     1001      127     9891 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/base/transformation.rs
+-rw-r--r--   0     1001      127      559 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/base.rs
+-rw-r--r--   0     1001      127     8405 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/data/arithmetic_crystal_class.rs
+-rw-r--r--   0     1001      127     7841 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/data/classification.rs
+-rw-r--r--   0     1001      127    20576 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/data/hall_symbol.rs
+-rw-r--r--   0     1001      127    81326 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/data/hall_symbol_database.rs
+-rw-r--r--   0     1001      127     7762 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/data/point_group.rs
+-rw-r--r--   0     1001      127     3421 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/data/setting.rs
+-rw-r--r--   0     1001      127   201241 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/data/wyckoff.rs
+-rw-r--r--   0     1001      127      740 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/data.rs
+-rw-r--r--   0     1001      127    19605 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/identify/point_group.rs
+-rw-r--r--   0     1001      127    13483 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/identify/space_group.rs
+-rw-r--r--   0     1001      127       68 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/identify.rs
+-rw-r--r--   0     1001      127    10323 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/lib.rs
+-rw-r--r--   0     1001      127      901 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math/cycle_checker.rs
+-rw-r--r--   0     1001      127     5124 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math/delaunay.rs
+-rw-r--r--   0     1001      127     2284 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math/elementary.rs
+-rw-r--r--   0     1001      127     4148 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math/hnf.rs
+-rw-r--r--   0     1001      127     2440 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math/integer_system.rs
+-rw-r--r--   0     1001      127     7889 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math/minkowski.rs
+-rw-r--r--   0     1001      127    14588 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math/niggli.rs
+-rw-r--r--   0     1001      127     4889 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math/snf.rs
+-rw-r--r--   0     1001      127      344 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/math.rs
+-rw-r--r--   0     1001      127    12016 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/search/primitive_cell.rs
+-rw-r--r--   0     1001      127    12095 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/search/solve.rs
+-rw-r--r--   0     1001      127    12741 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/search/symmetry_search.rs
+-rw-r--r--   0     1001      127      250 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/search.rs
+-rw-r--r--   0     1001      127    14888 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/symmetrize/standardize.rs
+-rw-r--r--   0     1001      127       94 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/src/symmetrize.rs
+-rw-r--r--   0     1001      127     5985 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/assets/mp-1185639.json
+-rw-r--r--   0     1001      127     5374 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/assets/mp-1197586.json
+-rw-r--r--   0     1001      127     9958 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/assets/mp-1201492.json
+-rw-r--r--   0     1001      127      820 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/assets/mp-1221598.json
+-rw-r--r--   0     1001      127      735 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/assets/mp-1277787.json
+-rw-r--r--   0     1001      127     3820 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/assets/mp-30665.json
+-rw-r--r--   0     1001      127     1370 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/assets/mp-550745.json
+-rw-r--r--   0     1001      127     5272 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/assets/mp-569901.json
+-rw-r--r--   0     1001      127    20157 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyo/tests/test_moyo_dataset.rs
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 moyopy-0.1.8/moyopy/Cargo.toml
+-rw-r--r--   0     1001      127      363 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/README.md
+-rw-r--r--   0     1001      127      767 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/examples/basic.py
+-rw-r--r--   0     1001      127     3567 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/examples/pymatgen_structure.py
+-rw-r--r--   0     1001      127        9 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/examples/requirements.txt
+-rw-r--r--   0     1001      127       37 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/python/moyopy/__init__.py
+-rw-r--r--   0     1001      127     2504 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/python/moyopy/_moyopy.pyi
+-rw-r--r--   0     1001      127        0 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/python/moyopy/py.typed
+-rw-r--r--   0     1001      127      623 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/python/tests/conftest.py
+-rw-r--r--   0     1001      127      430 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/python/tests/test_moyo_dataset.py
+-rw-r--r--   0     1001      127     5234 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/src/base.rs
+-rw-r--r--   0     1001      127      731 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/src/data.rs
+-rw-r--r--   0     1001      127     4114 2024-04-29 05:31:32.000000 moyopy-0.1.8/moyopy/src/lib.rs
+-rw-r--r--   0     1001      127    43444 2024-04-29 05:31:32.000000 moyopy-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 moyopy-0.1.8/Cargo.toml
+-rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 moyopy-0.1.8/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-29 05:31:32.000000 moyopy-0.1.8/python/moyopy/py.typed
+-rw-r--r--   0     1001      127       37 2024-04-29 05:31:32.000000 moyopy-0.1.8/python/moyopy/__init__.py
+-rw-r--r--   0     1001      127     2504 2024-04-29 05:31:32.000000 moyopy-0.1.8/python/moyopy/_moyopy.pyi
+-rw-r--r--   0     1001      127      363 2024-04-29 05:31:32.000000 moyopy-0.1.8/README.md
+-rw-r--r--   0        0        0     1450 1970-01-01 00:00:00.000000 moyopy-0.1.8/PKG-INFO
```

### Comparing `moyopy-0.1.7/moyo/Cargo.toml` & `moyopy-0.1.8/moyo/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -14,29 +14,28 @@
 name = "moyo"
 
 [dependencies]
 nalgebra.workspace = true
 serde.workspace = true
 serde_json.workspace = true
 approx.workspace = true
-itertools = "0.11.0"
+log.workspace = true
+itertools = "0.11"
 thiserror = "1.0"
-union-find = "0.4.2"
+union-find = "0.4"
 strum = "0.25"
 strum_macros = "0.25"
-kiddo = "4.2.0"
-# Disable trace level logs in release build
-log = { version = "0.4", features = ["release_max_level_debug"] }
+kiddo = "4.2"
 
 [dev-dependencies]
-rand = "0.8.5"
-rstest = "0.18.2"
+rand = "0.8"
+rstest = "0.18"
 criterion = { version = "0.4", features = ["html_reports"] }
-env_logger = "0.11.3"
-test-log = "0.2.15"
+env_logger = "0.11"
+test-log = "0.2"
 
 [[bench]]
 name = "translation_search"
 path = "benches/translation_search.rs"
 harness = false
 
 [[bench]]
```

### Comparing `moyopy-0.1.7/moyo/benches/dataset.rs` & `moyopy-0.1.8/moyo/benches/dataset.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/benches/translation_search.rs` & `moyopy-0.1.8/moyo/benches/translation_search.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/base/cell.rs` & `moyopy-0.1.8/moyo/src/base/cell.rs`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 pub struct Cell {
     pub lattice: Lattice,
     pub positions: Vec<Position>,
     pub numbers: Vec<AtomicSpecie>,
 }
 
 impl Cell {
+    /// * `lattice`: Lattice of the cell.
+    /// * `positions`: `positions[i]` is a fractional coordinates of the i-th site.
+    /// * `numbers`: `numbers[i]` is a number of the i-th site.
     pub fn new(lattice: Lattice, positions: Vec<Position>, numbers: Vec<AtomicSpecie>) -> Self {
         if positions.len() != numbers.len() {
             panic!("positions and numbers should be the same length");
         }
         Self {
             lattice,
             positions,
```

### Comparing `moyopy-0.1.7/moyo/src/base/error.rs` & `moyopy-0.1.8/moyo/src/base/error.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/base/lattice.rs` & `moyopy-0.1.8/moyo/src/base/lattice.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/base/operation.rs` & `moyopy-0.1.8/moyo/src/base/operation.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/base/tolerance.rs` & `moyopy-0.1.8/moyo/src/base/tolerance.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-use log::warn;
+use log::debug;
 
 use super::error::MoyoError;
 
 pub const EPS: f64 = 1e-8;
 
 const INITIAL_SYMMETRY_SEARCH_STRIDE: f64 = 2.0;
 
 #[derive(Debug, Copy, Clone)]
+/// Tolerance for angle in comparing basis vectors in symmetry search.
 pub enum AngleTolerance {
+    /// Tolerance in radian.
     Radian(f64),
+    /// Default tolerance same as Spglib.
     Default,
 }
 
 pub struct ToleranceHandler {
     pub symprec: f64,
     pub angle_tolerance: AngleTolerance,
     stride: f64,
@@ -47,28 +50,28 @@
     fn increase_tolerance(&self) -> (f64, AngleTolerance) {
         let symprec = self.symprec * self.stride;
         let angle_tolerance = if let AngleTolerance::Radian(angle) = self.angle_tolerance {
             AngleTolerance::Radian(angle * self.stride)
         } else {
             AngleTolerance::Default
         };
-        warn!(
+        debug!(
             "Increase tolerance to symprec={}, angle_tolerance={:?}",
             symprec, angle_tolerance
         );
         (symprec, angle_tolerance)
     }
 
     fn reduce_tolerance(&self) -> (f64, AngleTolerance) {
         let symprec = self.symprec / self.stride;
         let angle_tolerance = if let AngleTolerance::Radian(angle) = self.angle_tolerance {
             AngleTolerance::Radian(angle / self.stride)
         } else {
             AngleTolerance::Default
         };
-        warn!(
+        debug!(
             "Reduce tolerance to symprec={}, angle_tolerance={:?}",
             symprec, angle_tolerance
         );
         (symprec, angle_tolerance)
     }
 }
```

### Comparing `moyopy-0.1.7/moyo/src/base/transformation.rs` & `moyopy-0.1.8/moyo/src/base/transformation.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/base.rs` & `moyopy-0.1.8/moyo/src/base.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/data/arithmetic_crystal_class.rs` & `moyopy-0.1.8/moyo/src/data/arithmetic_crystal_class.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/data/classification.rs` & `moyopy-0.1.8/moyo/src/data/classification.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/data/hall_symbol.rs` & `moyopy-0.1.8/moyo/src/data/hall_symbol.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/data/hall_symbol_database.rs` & `moyopy-0.1.8/moyo/src/data/hall_symbol_database.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 use super::arithmetic_crystal_class::ArithmeticNumber;
 use super::hall_symbol::Centering;
 
+/// ITA number for space group types (1 - 230)
 pub type Number = i32;
+/// Number for Hall symbols (1 - 530)
 pub type HallNumber = i32;
 
 #[derive(Debug, Clone)]
 pub struct HallSymbolEntry {
     pub hall_number: HallNumber,
     pub number: Number,
     pub arithmetic_number: ArithmeticNumber,
```

### Comparing `moyopy-0.1.7/moyo/src/data/point_group.rs` & `moyopy-0.1.8/moyo/src/data/point_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/data/setting.rs` & `moyopy-0.1.8/moyo/src/data/setting.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use super::hall_symbol_database::HallNumber;
 
 #[derive(Debug, Copy, Clone, PartialEq)]
+/// Preference for the setting of the space group.
 pub enum Setting {
     HallNumber(HallNumber),
     /// The setting of the smallest Hall number
     Spglib,
     /// Unique axis b, cell choice 1 for monoclinic, hexagonal axes for rhombohedral, and origin choice 2 for centrosymmetric space groups
     Standard,
 }
```

### Comparing `moyopy-0.1.7/moyo/src/data/wyckoff.rs` & `moyopy-0.1.8/moyo/src/data/wyckoff.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/data.rs` & `moyopy-0.1.8/moyo/src/data.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/identify/point_group.rs` & `moyopy-0.1.8/moyo/src/identify/point_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/identify/space_group.rs` & `moyopy-0.1.8/moyo/src/identify/space_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/lib.rs` & `moyopy-0.1.8/moyo/src/lib.rs`

 * *Files 25% similar despite different names*

```diff
@@ -5,34 +5,39 @@
 pub mod base;
 pub mod data;
 pub mod identify;
 pub mod math;
 pub mod search;
 pub mod symmetrize;
 
+pub use base::{
+    AngleTolerance, Cell, Lattice, MoyoError, Operations, OriginShift, Rotation, Translation,
+};
+pub use data::{HallNumber, Number, Setting};
+
 use nalgebra::Matrix3;
 
-use crate::base::{
-    AngleTolerance, Cell, MoyoError, Operations, OriginShift, ToleranceHandler, Transformation,
-};
-use crate::data::{HallNumber, Number, Setting};
+use crate::base::{ToleranceHandler, Transformation};
 use crate::identify::SpaceGroup;
 use crate::search::{PrimitiveCell, PrimitiveSymmetrySearch};
 use crate::symmetrize::{orbits_in_cell, StandardizedCell};
 
 #[derive(Debug)]
 pub struct MoyoDataset {
     // ------------------------------------------------------------------------
     // Space-group type
     // ------------------------------------------------------------------------
+    /// Space group number.
     pub number: Number,
+    /// Hall symbol number.
     pub hall_number: HallNumber,
     // ------------------------------------------------------------------------
     // Symmetry operations in the input cell
     // ------------------------------------------------------------------------
+    /// Symmetry operations in the input cell.
     pub operations: Operations,
     // ------------------------------------------------------------------------
     // Site symmetry
     // ------------------------------------------------------------------------
     /// Spglib's `crystallographic_orbits` not `equivalent_atoms`
     /// The `i`th atom in the input cell is equivalent to the `orbits[i]`th atom in the **input** cell.
     /// For example, orbits=[0, 0, 2, 2, 2, 2] means the first two atoms are equivalent and the last four atoms are equivalent to each other.
@@ -41,40 +46,72 @@
     pub wyckoffs: Vec<char>,
     /// Site symmetry symbols for each site in the input cell.
     /// The orientation of the site symmetry is w.r.t. the standardized cell.
     pub site_symmetry_symbols: Vec<String>,
     // ------------------------------------------------------------------------
     // Standardized cell
     // ------------------------------------------------------------------------
+    /// Standardized cell
     pub std_cell: Cell,
     /// Linear part of transformation from the input cell to the standardized cell.
     pub std_linear: Matrix3<f64>,
     /// Origin shift of transformation from the input cell to the standardized cell.
     pub std_origin_shift: OriginShift,
     /// Rigid rotation
     pub std_rotation_matrix: Matrix3<f64>,
     // ------------------------------------------------------------------------
     // Primitive standardized cell
     // ------------------------------------------------------------------------
+    /// Primitive standardized cell
     pub prim_std_cell: Cell,
     /// Linear part of transformation from the input cell to the primitive standardized cell.
     pub prim_std_linear: Matrix3<f64>,
     /// Origin shift of transformation from the input cell to the primitive standardized cell.
     pub prim_std_origin_shift: OriginShift,
     /// Mapping sites in the input cell to those in the primitive standardized cell.
     /// The `i`th atom in the input cell is mapped to the `mapping_to_std_prim[i]`th atom in the primitive standardized cell.
     pub mapping_std_prim: Vec<usize>,
     // ------------------------------------------------------------------------
     // Final parameters
     // ------------------------------------------------------------------------
+    /// Actually used `symprec` in iterative symmetry search.
     pub symprec: f64,
+    /// Actually used `angle_tolerance` in iterative symmetry search.
     pub angle_tolerance: AngleTolerance,
 }
 
 impl MoyoDataset {
+    /// Create a new `MoyoDataset` from the input cell.
+    ///
+    /// # Examples
+    /// ```
+    /// use nalgebra::{matrix, vector, Matrix3, Vector3};
+    /// use moyo::{MoyoDataset, Cell, AngleTolerance, Setting, Lattice};
+    /// let lattice = Lattice::new(matrix![
+    ///     4.603, 0.0, 0.0;
+    ///     0.0, 4.603, 0.0;
+    ///     0.0, 0.0, 2.969;
+    /// ]);
+    /// let x_4f = 0.3046;
+    /// let positions = vec![
+    ///     Vector3::new(0.0, 0.0, 0.0),                // Ti(2a)
+    ///     Vector3::new(0.5, 0.5, 0.5),                // Ti(2a)
+    ///     Vector3::new(x_4f, x_4f, 0.0),              // O(4f)
+    ///     Vector3::new(-x_4f, -x_4f, 0.0),            // O(4f)
+    ///     Vector3::new(-x_4f + 0.5, x_4f + 0.5, 0.5), // O(4f)
+    ///     Vector3::new(x_4f + 0.5, -x_4f + 0.5, 0.5), // O(4f)
+    /// ];
+    /// let numbers = vec![0, 0, 1, 1, 1, 1];
+    /// let cell = Cell::new(lattice, positions, numbers);
+    /// let symprec = 1e-5;
+    /// let angle_tolerance = AngleTolerance::Default;
+    /// let setting = Setting::Standard;
+    /// let dataset = MoyoDataset::new(&cell, symprec, angle_tolerance, setting).unwrap();
+    /// assert_eq!(dataset.number, 136);  // P4_2/mnm
+    /// ```
     pub fn new(
         cell: &Cell,
         symprec: f64,
         angle_tolerance: AngleTolerance,
         setting: Setting,
     ) -> Result<Self, MoyoError> {
         let (prim_cell, symmetry_search, symprec, angle_tolerance) =
```

### Comparing `moyopy-0.1.7/moyo/src/math/cycle_checker.rs` & `moyopy-0.1.8/moyo/src/math/cycle_checker.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/math/delaunay.rs` & `moyopy-0.1.8/moyo/src/math/delaunay.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/math/elementary.rs` & `moyopy-0.1.8/moyo/src/math/elementary.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/math/hnf.rs` & `moyopy-0.1.8/moyo/src/math/hnf.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/math/integer_system.rs` & `moyopy-0.1.8/moyo/src/math/integer_system.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/math/minkowski.rs` & `moyopy-0.1.8/moyo/src/math/minkowski.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/math/niggli.rs` & `moyopy-0.1.8/moyo/src/math/niggli.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/math/snf.rs` & `moyopy-0.1.8/moyo/src/math/snf.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/search/primitive_cell.rs` & `moyopy-0.1.8/moyo/src/search/primitive_cell.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use std::collections::BTreeMap;
 
-use log::{debug, warn};
+use log::debug;
 use nalgebra::{Dyn, Matrix3, OMatrix, Vector3, U3};
 
 use super::solve::{
     pivot_site_indices, solve_correspondence, symmetrize_translation_from_permutation,
     PeriodicKdTree,
 };
 use crate::base::{
@@ -41,15 +41,17 @@
         let minimum_basis_norm = reduced_lattice
             .basis
             .column_iter()
             .map(|v| v.norm())
             .fold(f64::INFINITY, f64::min);
         let rough_symprec = 2.0 * symprec;
         if rough_symprec > minimum_basis_norm / 2.0 {
-            warn!("symprec is too large compared to the basis vectors. Consider reducing symprec.");
+            debug!(
+                "symprec is too large compared to the basis vectors. Consider reducing symprec."
+            );
             return Err(MoyoError::TooLargeToleranceError);
         }
 
         // Try possible translations: overlap the `src`the site to the `dst`th site
         let pkdtree = PeriodicKdTree::new(&reduced_cell, rough_symprec);
         let pivot_site_indices = pivot_site_indices(&reduced_cell.numbers);
         let mut permutations_translations_tmp = vec![];
@@ -84,15 +86,15 @@
                 translations.push(translation);
                 permutations.push(permutation.clone());
             }
         }
 
         let size = translations.len() as i32;
         if (size == 0) || (reduced_cell.num_atoms() % (size as usize) != 0) {
-            warn!("Failed to properly find translations: {} translations in {} atoms. Consider increasing symprec.", size, reduced_cell.num_atoms());
+            debug!("Failed to properly find translations: {} translations in {} atoms. Consider increasing symprec.", size, reduced_cell.num_atoms());
             return Err(MoyoError::TooSmallToleranceError);
         }
         debug!("Found {} pure translations", size);
 
         // Recover a transformation matrix from primitive to input cell
         let mut columns: Vec<Vector3<i32>> = vec![
             Vector3::new(size, 0, 0),
@@ -112,15 +114,15 @@
             .ok_or(MoyoError::PrimitiveCellError)?
             .map(|e| e.round() as i32);
         if relative_ne!(
             trans_mat.map(|e| e as f64).determinant(),
             size as f64,
             epsilon = EPS
         ) {
-            warn!("Failed to find a transformation matrix to a primitive cell. Consider increasing symprec.");
+            debug!("Failed to find a transformation matrix to a primitive cell. Consider increasing symprec.");
             return Err(MoyoError::TooSmallToleranceError);
         }
 
         // Primitive cell
         let (primitive_cell, site_mapping) = primitive_cell_from_transformation(
             &reduced_cell,
             &trans_mat,
```

### Comparing `moyopy-0.1.7/moyo/src/search/solve.rs` & `moyopy-0.1.8/moyo/src/search/solve.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/src/search/symmetry_search.rs` & `moyopy-0.1.8/moyo/src/search/symmetry_search.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use itertools::iproduct;
 use std::collections::{HashMap, HashSet, VecDeque};
 
-use log::{debug, warn};
+use log::debug;
 use nalgebra::{Matrix3, Vector3};
 
 use super::solve::{
     pivot_site_indices, solve_correspondence, symmetrize_translation_from_permutation,
     PeriodicKdTree,
 };
 use crate::base::{
@@ -32,15 +32,17 @@
         symprec: f64,
         angle_tolerance: AngleTolerance,
     ) -> Result<Self, MoyoError> {
         // Check if symprec is sufficiently small
         let minimum_basis_norm = primitive_cell.lattice.basis.column(0).norm();
         let rough_symprec = 2.0 * symprec;
         if rough_symprec > minimum_basis_norm / 2.0 {
-            warn!("symprec is too large compared to the basis vectors. Consider reducing symprec.");
+            debug!(
+                "symprec is too large compared to the basis vectors. Consider reducing symprec."
+            );
             return Err(MoyoError::TooLargeToleranceError);
         }
 
         // Search symmetry operations
         let pkdtree = PeriodicKdTree::new(primitive_cell, rough_symprec);
         let bravais_group =
             search_bravais_group(&primitive_cell.lattice, symprec, angle_tolerance)?;
@@ -81,15 +83,15 @@
                 rough_translation,
             );
             if distance < symprec {
                 operations_and_permutations.push((rotation, translation, permutation.clone()));
             }
         }
         if operations_and_permutations.is_empty() {
-            warn!(
+            debug!(
                 "No symmetry operations are found. Consider increasing symprec and angle_tolerance."
             );
             return Err(MoyoError::TooSmallToleranceError);
         }
 
         // Recover operations by group multiplication
         let mut queue = VecDeque::new();
@@ -120,15 +122,15 @@
                     + translation_lhs)
                     .map(|e| e - e.round());
                 let new_permutation = permutation_lhs.clone() * permutation_rhs.clone();
                 queue.push_back((new_rotation, new_translation, new_permutation));
             }
         }
         if rotations.len() != operations_and_permutations.len() {
-            warn!("Found operations do not form a group. Consider reducing symprec and angle_tolerance.");
+            debug!("Found operations do not form a group. Consider reducing symprec and angle_tolerance.");
             return Err(MoyoError::TooLargeToleranceError);
         }
 
         // Check closure
         let mut translations_map = HashMap::new();
         for (rotation, translation) in rotations.iter().zip(translations.iter()) {
             translations_map.insert(rotation.clone(), translation.clone());
@@ -146,15 +148,15 @@
                 if primitive_cell.lattice.cartesian_coords(&diff).norm() > rough_symprec {
                     closed = false;
                     break;
                 }
             }
         }
         if !closed {
-            warn!("Some centering translations are missing. Consider reducing symprec and angle_tolerance.");
+            debug!("Some centering translations are missing. Consider reducing symprec and angle_tolerance.");
             return Err(MoyoError::TooLargeToleranceError);
         }
 
         debug!("Order of point group: {}", rotations.len());
         Ok(Self {
             operations: Operations::new(rotations, translations),
             permutations,
@@ -255,15 +257,15 @@
             rotations.push(rotation);
         }
     }
 
     // Recover rotations by group multiplication
     let complemented_rotations = traverse(&rotations);
     if complemented_rotations.len() != rotations.len() {
-        warn!("Found automorphisms for the lattice do not form a group. Consider reducing symprec and angle_tolerance.");
+        debug!("Found automorphisms for the lattice do not form a group. Consider reducing symprec and angle_tolerance.");
         return Err(MoyoError::TooLargeToleranceError);
     }
     debug!("Order of Bravais group: {}", complemented_rotations.len());
     Ok(complemented_rotations)
 }
 
 /// Compare (basis.column(col1), basis.column(col2)) and (b1, b2)
```

### Comparing `moyopy-0.1.7/moyo/src/symmetrize/standardize.rs` & `moyopy-0.1.8/moyo/src/symmetrize/standardize.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use itertools::{iproduct, izip};
-use log::warn;
+use log::debug;
 use nalgebra::linalg::{Cholesky, QR};
 use nalgebra::{vector, Matrix3, Vector3};
 use std::collections::HashMap;
 
 use crate::base::{
     orbits_from_permutations, Cell, Lattice, MoyoError, Operations, Permutation, Position,
     Rotation, Transformation, UnimodularTransformation, EPS,
@@ -210,15 +210,15 @@
             ) {
                 representative_wyckoffs[orbit] = Some(wyckoff);
             }
         }
 
         for (i, wyckoff) in representative_wyckoffs.iter().enumerate() {
             if wyckoff.is_none() {
-                warn!(
+                debug!(
                     "Failed to assign Wyckoff positions with multiplicity {}: {:?}",
                     multiplicities[i], std_cell.positions[i]
                 );
             }
         }
         let representative_wyckoffs = representative_wyckoffs
             .into_iter()
```

### Comparing `moyopy-0.1.7/moyo/tests/assets/mp-1185639.json` & `moyopy-0.1.8/moyo/tests/assets/mp-1185639.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/tests/assets/mp-1197586.json` & `moyopy-0.1.8/moyo/tests/assets/mp-1197586.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/tests/assets/mp-1201492.json` & `moyopy-0.1.8/moyo/tests/assets/mp-1201492.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/tests/assets/mp-1221598.json` & `moyopy-0.1.8/moyo/tests/assets/mp-1221598.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/tests/assets/mp-1277787.json` & `moyopy-0.1.8/moyo/tests/assets/mp-1277787.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/tests/assets/mp-30665.json` & `moyopy-0.1.8/moyo/tests/assets/mp-30665.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/tests/assets/mp-550745.json` & `moyopy-0.1.8/moyo/tests/assets/mp-550745.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/tests/assets/mp-569901.json` & `moyopy-0.1.8/moyo/tests/assets/mp-569901.json`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyo/tests/test_moyo_dataset.rs` & `moyopy-0.1.8/moyo/tests/test_moyo_dataset.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 use nalgebra::{matrix, vector, Matrix3, Vector3};
 use serde_json;
 use std::fs;
 use std::path::Path;
 use test_log::test;
 
-use moyo::base::{AngleTolerance, Cell, Lattice, Permutation, Rotation, Translation};
-use moyo::data::Setting;
-use moyo::MoyoDataset;
+use moyo::base::Permutation;
+use moyo::{AngleTolerance, Cell, Lattice, MoyoDataset, Rotation, Setting, Translation};
 
 /// Sanity-check MoyoDataset
 fn assert_dataset(
     cell: &Cell,
     symprec: f64,
     angle_tolerance: AngleTolerance,
     setting: Setting,
```

### Comparing `moyopy-0.1.7/moyopy/Cargo.toml` & `moyopy-0.1.8/moyopy/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 description.workspace = true
 edition.workspace = true
 license.workspace = true
 repository.workspace = true
 version.workspace = true
 
 [package.metadata.release]
-release = true
+release = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "moyopy"
 crate-type = ["cdylib"]
 
 [dependencies]
-moyo = { path = "../moyo", version = "0.1.7" }
+moyo = { path = "../moyo", version = "0.1.8" }
 nalgebra.workspace = true
 serde.workspace = true
 serde_json.workspace = true
 approx.workspace = true
+log.workspace = true
+pyo3-log = "0.10"
 
 [dependencies.pyo3]
-version = "0.20.3"
+version = "0.21"
 # "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
 features = ["abi3-py38"]
```

### Comparing `moyopy-0.1.7/moyopy/python/moyopy/_moyopy.pyi` & `moyopy-0.1.8/moyopy/python/moyopy/_moyopy.pyi`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyopy/python/tests/conftest.py` & `moyopy-0.1.8/moyopy/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/moyopy/src/base.rs` & `moyopy-0.1.8/moyopy/src/base.rs`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::types::PyType;
 use serde::de::{Deserialize, Deserializer};
 use serde::ser::{Serialize, Serializer};
 use serde_json;
 
-use moyo::base::{Cell, Lattice, MoyoError, Operations};
+use moyo::base::Operations;
+use moyo::{Cell, Lattice, MoyoError};
 
 // Unfortunately, "PyCell" is already reversed by pyo3...
 #[derive(Debug, Clone)]
 #[pyclass(name = "Cell")]
 #[pyo3(module = "moyopy")]
 pub struct PyStructure(Cell);
 
@@ -65,17 +66,30 @@
     }
 
     pub fn serialize_json(&self) -> PyResult<String> {
         serde_json::to_string(self).map_err(|e| PyValueError::new_err(e.to_string()))
     }
 
     #[classmethod]
-    pub fn deserialize_json(_cls: &PyType, s: &str) -> PyResult<Self> {
+    pub fn deserialize_json(_cls: &Bound<'_, PyType>, s: &str) -> PyResult<Self> {
         serde_json::from_str(s).map_err(|e| PyValueError::new_err(e.to_string()))
     }
+
+    fn __repr__(&self) -> String {
+        format!(
+            "Cell(basis={:?}, positions={:?}, numbers={:?})",
+            self.basis(),
+            self.positions(),
+            self.numbers()
+        )
+    }
+
+    fn __str__(&self) -> String {
+        self.__repr__()
+    }
 }
 
 impl From<PyStructure> for Cell {
     fn from(structure: PyStructure) -> Self {
         structure.0
     }
 }
```

### Comparing `moyopy-0.1.7/moyopy/src/data.rs` & `moyopy-0.1.8/moyopy/src/data.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 use pyo3::prelude::*;
 use pyo3::types::PyType;
 
-use moyo::data::Setting;
+use moyo::Setting;
 
 #[derive(Debug, Clone)]
 #[pyclass(name = "Setting")]
 #[pyo3(module = "moyopy")]
 pub struct PySetting(Setting);
 
 #[pymethods]
 impl PySetting {
     #[classmethod]
-    pub fn spglib(_cls: &PyType) -> PyResult<Self> {
+    pub fn spglib(_cls: &Bound<'_, PyType>) -> PyResult<Self> {
         Ok(Self(Setting::Spglib))
     }
 
     #[classmethod]
-    pub fn standard(_cls: &PyType) -> PyResult<Self> {
+    pub fn standard(_cls: &Bound<'_, PyType>) -> PyResult<Self> {
         Ok(Self(Setting::Standard))
     }
 
     #[classmethod]
-    pub fn hall_number(_cls: &PyType, hall_number: i32) -> PyResult<Self> {
+    pub fn hall_number(_cls: &Bound<'_, PyType>, hall_number: i32) -> PyResult<Self> {
         Ok(Self(Setting::HallNumber(hall_number)))
     }
 }
 
 impl From<PySetting> for Setting {
     fn from(setting: PySetting) -> Self {
         setting.0
```

### Comparing `moyopy-0.1.7/moyopy/src/lib.rs` & `moyopy-0.1.8/moyopy/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 use base::PyOperations;
 use pyo3::prelude::*;
 use std::sync::OnceLock;
 
 pub mod base;
 pub mod data;
 
-use moyo::base::AngleTolerance;
-use moyo::data::Setting;
-use moyo::MoyoDataset;
+use moyo::{AngleTolerance, MoyoDataset, Setting};
 
 use crate::base::{PyMoyoError, PyStructure};
 use crate::data::PySetting;
 
 #[derive(Debug)]
 #[pyclass(name = "MoyoDataset")]
 #[pyo3(module = "moyopy")]
@@ -142,15 +140,17 @@
         version.replace("-alpha", "a").replace("-beta", "b")
     })
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 #[pyo3(name = "_moyopy")]
-fn moyopy(_py: Python, m: &PyModule) -> PyResult<()> {
+fn moyopy(m: &Bound<'_, PyModule>) -> PyResult<()> {
+    pyo3_log::init();
+
     m.add("__version__", moyopy_version())?;
 
     // lib
     m.add_class::<PyMoyoDataset>()?;
 
     // base
     m.add_class::<base::PyStructure>()?;
```

### Comparing `moyopy-0.1.7/Cargo.lock` & `moyopy-0.1.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "arc-swap"
+version = "1.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
+
+[[package]]
 name = "atty"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
 dependencies = [
  "hermit-abi",
  "libc",
@@ -614,15 +620,15 @@
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "moyo"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "approx",
  "criterion",
  "env_logger",
  "itertools 0.11.0",
  "kiddo",
  "log",
@@ -636,20 +642,22 @@
  "test-log",
  "thiserror",
  "union-find",
 ]
 
 [[package]]
 name = "moyopy"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "approx",
+ "log",
  "moyo",
  "nalgebra",
  "pyo3",
+ "pyo3-log",
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "nalgebra"
 version = "0.32.5"
@@ -848,17 +856,17 @@
 checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -866,49 +874,60 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
+name = "pyo3-log"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2af49834b8d2ecd555177e63b273b708dea75150abc6f5341d0a6e1a9623976c"
+dependencies = [
+ "arc-swap",
+ "log",
+ "pyo3",
+]
+
+[[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
```

### Comparing `moyopy-0.1.7/pyproject.toml` & `moyopy-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/python/moyopy/_moyopy.pyi` & `moyopy-0.1.8/python/moyopy/_moyopy.pyi`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.7/PKG-INFO` & `moyopy-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: moyopy
-Version: 0.1.7
+Version: 0.1.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -20,15 +20,19 @@
 Author: Kohei Shinohara <kshinohara0508@gmail.com>
 Author-email: Kohei Shinohara <kshinohara0508@gmail.com>
 License: MIT OR Apache-2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/spglib/moyo
 
-# moyopy
+# Moyopy
 
 [![image](https://img.shields.io/pypi/v/moyopy.svg)](https://pypi.python.org/pypi/moyopy)
 [![image](https://img.shields.io/pypi/l/moyopy.svg)](https://pypi.python.org/pypi/moyopy)
 [![image](https://img.shields.io/pypi/pyversions/moyopy.svg)](https://pypi.python.org/pypi/moyopy)
 
 Python interface of Moyo
 
+## Examples
+
+See [example directory](examples)
+
```

