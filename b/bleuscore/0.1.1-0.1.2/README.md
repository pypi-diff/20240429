# Comparing `tmp/bleuscore-0.1.1.tar.gz` & `tmp/bleuscore-0.1.2.tar.gz`

## Comparing `bleuscore-0.1.1.tar` & `bleuscore-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,41 @@
--rw-r--r--   0        0        0      733 1970-01-01 00:00:00.000000 bleuscore-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127      900 2024-04-26 07:51:00.000000 bleuscore-0.1.1/.github/workflows/doc.yml
--rw-r--r--   0     1001      127     5153 2024-04-26 07:51:00.000000 bleuscore-0.1.1/.github/workflows/maturin.yml
--rw-r--r--   0     1001      127     1374 2024-04-26 07:51:00.000000 bleuscore-0.1.1/.github/workflows/rust.yml
--rw-r--r--   0     1001      127      456 2024-04-26 07:51:00.000000 bleuscore-0.1.1/.gitignore
--rw-r--r--   0     1001      127      478 2024-04-26 07:51:00.000000 bleuscore-0.1.1/CHANGELOG.md
--rw-r--r--   0     1001      127     1068 2024-04-26 07:51:00.000000 bleuscore-0.1.1/LICENSE
--rw-r--r--   0     1001      127     2848 2024-04-26 07:51:00.000000 bleuscore-0.1.1/README.md
--rw-r--r--   0     1001      127   302127 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/n_1.png
--rw-r--r--   0     1001      127   110049 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/n_100.png
--rw-r--r--   0     1001      127   136288 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/n_10000.png
--rw-r--r--   0     1001      127   117831 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/n_100000.png
--rw-r--r--   0     1001      127   351628 2024-04-26 07:51:00.000000 bleuscore-0.1.1/asset/benchmark/simple.png
--rw-r--r--   0     1001      127      178 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/bench.sh
--rw-r--r--   0     1001      127      206 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/hf_evaluate.py
--rw-r--r--   0     1001      127     8279 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/local_hf_bleu.py
--rw-r--r--   0     1001      127      179 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/rs_bleuscore.py
--rw-r--r--   0     1001      127      247 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/sacre_bleu.py
--rw-r--r--   0     1001      127      223 2024-04-26 07:51:00.000000 bleuscore-0.1.1/benchmark/simple/simulation_data.py
--rw-r--r--   0     1001      127      146 2024-04-26 07:51:00.000000 bleuscore-0.1.1/python/bleuscore/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-26 07:51:00.000000 bleuscore-0.1.1/python/bleuscore/py.typed
--rw-r--r--   0     1001      127     4735 2024-04-26 07:51:00.000000 bleuscore-0.1.1/src/bleu.rs
--rw-r--r--   0     1001      127     2819 2024-04-26 07:51:00.000000 bleuscore-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127     3508 2024-04-26 07:51:00.000000 bleuscore-0.1.1/src/ngram.rs
--rw-r--r--   0     1001      127     3862 2024-04-26 07:51:00.000000 bleuscore-0.1.1/src/tokenizer.rs
--rw-r--r--   0     1001      127      484 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/conftest.py
--rw-r--r--   0     1001      127     4897 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/py_bleu.py
--rw-r--r--   0     1001      127     3488 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/py_token.py
--rw-r--r--   0     1001      127     4463 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/test_bleu_score.py
--rw-r--r--   0     1001      127     1318 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/test_tokenizer.py
--rw-r--r--   0     1001      127     1074 2024-04-26 07:51:00.000000 bleuscore-0.1.1/tests/util.py
--rw-r--r--   0     1001      127    14179 2024-04-26 07:51:05.000000 bleuscore-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127     1983 2024-04-26 07:51:00.000000 bleuscore-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4373 1970-01-01 00:00:00.000000 bleuscore-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 bleuscore-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127      575 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/bench_base.yml
+-rw-r--r--   0     1001      127     1044 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/bench_pr.yml
+-rw-r--r--   0     1001      127      900 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/doc.yml
+-rw-r--r--   0     1001      127     5153 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/maturin.yml
+-rw-r--r--   0     1001      127     1374 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.github/workflows/rust.yml
+-rw-r--r--   0     1001      127      456 2024-04-29 15:13:40.000000 bleuscore-0.1.2/.gitignore
+-rw-r--r--   0     1001      127      768 2024-04-29 15:13:40.000000 bleuscore-0.1.2/CHANGELOG.md
+-rw-r--r--   0     1001      127     1068 2024-04-29 15:13:40.000000 bleuscore-0.1.2/LICENSE
+-rw-r--r--   0     1001      127     4837 2024-04-29 15:13:40.000000 bleuscore-0.1.2/README.md
+-rw-r--r--   0     1001      127   302127 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/n_1.png
+-rw-r--r--   0     1001      127   110049 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/n_100.png
+-rw-r--r--   0     1001      127   136288 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/n_10000.png
+-rw-r--r--   0     1001      127   117831 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/n_100000.png
+-rw-r--r--   0     1001      127   351628 2024-04-29 15:13:40.000000 bleuscore-0.1.2/asset/benchmark/simple.png
+-rw-r--r--   0     1001      127     4687 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/README.md
+-rw-r--r--   0     1001      127   102651 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/bench.png
+-rw-r--r--   0     1001      127      624 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/bench.sh
+-rw-r--r--   0     1001      127     1742 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/bench_plot.py
+-rw-r--r--   0     1001      127     4239 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/result.json
+-rw-r--r--   0     1001      127      311 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/hf_evaluate.py
+-rw-r--r--   0     1001      127     8385 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/local_hf_bleu.py
+-rw-r--r--   0     1001      127      284 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/rs_bleuscore.py
+-rw-r--r--   0     1001      127      352 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/sacre_bleu.py
+-rw-r--r--   0     1001      127      473 2024-04-29 15:13:40.000000 bleuscore-0.1.2/benchmark/simple/util.py
+-rw-r--r--   0     1001      127      146 2024-04-29 15:13:40.000000 bleuscore-0.1.2/python/bleuscore/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-29 15:13:40.000000 bleuscore-0.1.2/python/bleuscore/py.typed
+-rw-r--r--   0     1001      127       31 2024-04-29 15:13:40.000000 bleuscore-0.1.2/rust-toolchain.toml
+-rw-r--r--   0     1001      127     7450 2024-04-29 15:13:40.000000 bleuscore-0.1.2/src/bleu.rs
+-rw-r--r--   0     1001      127     2892 2024-04-29 15:13:40.000000 bleuscore-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127     3640 2024-04-29 15:13:40.000000 bleuscore-0.1.2/src/ngram.rs
+-rw-r--r--   0     1001      127     4343 2024-04-29 15:13:40.000000 bleuscore-0.1.2/src/tokenizer.rs
+-rw-r--r--   0     1001      127      484 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/conftest.py
+-rw-r--r--   0     1001      127     4897 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/py_bleu.py
+-rw-r--r--   0     1001      127     3488 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/py_token.py
+-rw-r--r--   0     1001      127     4463 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/test_bleu_score.py
+-rw-r--r--   0     1001      127     1318 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/test_tokenizer.py
+-rw-r--r--   0     1001      127     1074 2024-04-29 15:13:40.000000 bleuscore-0.1.2/tests/util.py
+-rw-r--r--   0     1001      127    16044 2024-04-29 15:13:53.000000 bleuscore-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127     1983 2024-04-29 15:13:40.000000 bleuscore-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6362 1970-01-01 00:00:00.000000 bleuscore-0.1.2/PKG-INFO
```

### Comparing `bleuscore-0.1.1/Cargo.toml` & `bleuscore-0.1.2/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "bleuscore"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 authors = ["Mathew Shen <datahonor@gmail.com>"]
 repository = "https://github.com/shenxiangzhuang/bleuscore"
 readme = "README.md"
 license = "MIT"
 description = "A fast(not yet :) bleu score calculator"
 keywords = ["NLP", "Tokenizer", "BLEU", "DeepLearning"]
@@ -15,12 +15,14 @@
 crate-type = ["cdylib", "rlib"]
 
 [dependencies]
 cached = "0.50.0"
 regex = "1.10.4"
 lazy_static = "1.4.0"
 counter = "0.5.7"
+rayon = "1.10.0"
+ahash = "0.8.11"
 
 [dependencies.pyo3]
 version = "0.21.1"
 # "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
 features = ["abi3-py38"]
```

### Comparing `bleuscore-0.1.1/.github/workflows/doc.yml` & `bleuscore-0.1.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/.github/workflows/maturin.yml` & `bleuscore-0.1.2/.github/workflows/maturin.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/.github/workflows/rust.yml` & `bleuscore-0.1.2/.github/workflows/rust.yml`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/LICENSE` & `bleuscore-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/asset/benchmark/n_1.png` & `bleuscore-0.1.2/asset/benchmark/n_1.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/asset/benchmark/n_100.png` & `bleuscore-0.1.2/asset/benchmark/n_100.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/asset/benchmark/n_10000.png` & `bleuscore-0.1.2/asset/benchmark/n_10000.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/asset/benchmark/n_100000.png` & `bleuscore-0.1.2/asset/benchmark/n_100000.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/asset/benchmark/simple.png` & `bleuscore-0.1.2/asset/benchmark/simple.png`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/benchmark/simple/local_hf_bleu.py` & `bleuscore-0.1.2/benchmark/simple/local_hf_bleu.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,18 @@
 
     bleu = geo_mean * bp
 
     return bleu, precisions, bp, ratio, translation_length, reference_length
 
 
 if __name__ == "__main__":
-    from simulation_data import predictions, references
+    from util import get_simulation_data, get_arg_parser
+
+    args = get_arg_parser().parse_args()
+    predictions, references = get_simulation_data(int(args.n))
 
     results = compute_bleu(
         reference_corpus=references,
         translation_corpus=predictions,
         max_order=4,
         smooth=False,
     )
```

### Comparing `bleuscore-0.1.1/src/lib.rs` & `bleuscore-0.1.2/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -16,29 +16,34 @@
 [huggingface evaluate](https://github.com/huggingface/evaluate/blob/main/metrics/bleu/bleu.py)
 and [sacrebleu](https://github.com/mjpost/sacrebleu)
 
 
 # Basic usage:
 
 ```rust
+use bleuscore::compute_score;
+
 // get the references and prediction data:
 let references: Vec<Vec<String>> = vec![vec!["Hello, World!".to_string()]];
 let predictions: Vec<String> = vec!["Yellow, World!".to_string()];
 
 // set the parameters:
 let max_order: usize = 4;
 let smooth: bool = true;
 
 // calculate the BLEU score:
-let res = compute_score(references, predictions, max_order, smooth);
+let res = compute_score(&references, &predictions, max_order, smooth);
 println!("result: {:?}", res);
 // result: BleuScore { bleu: 0.668740304976422, precisions: [0.8, 0.75, 0.6666666666666666, 0.5],
 // brevity_penalty: 1.0, length_ratio: 1.0, translation_length: 4, reference_length: 4 }
 ```
 !*/
+#![feature(test)]
+extern crate test;
+
 mod tokenizer;
 pub use crate::tokenizer::{Tokenizer, Tokenizer13a, TokenizerRegex};
 mod bleu;
 mod ngram;
 pub use crate::bleu::{compute_score, BleuScore};
 
 use pyo3::prelude::*;
@@ -62,15 +67,15 @@
 #[pyo3(signature = (references, predictions, max_order=4, smooth=false))]
 fn compute(
     references: Vec<Vec<String>>,
     predictions: Vec<String>,
     max_order: usize,
     smooth: bool,
 ) -> PyResult<PyObject> {
-    let bleu = compute_score(references, predictions, max_order, smooth);
+    let bleu = compute_score(&references, &predictions, max_order, smooth);
     Python::with_gil(|py| {
         let bleu_dict = [
             ("bleu", bleu.bleu.to_object(py)),
             ("precisions", bleu.precisions.to_object(py)),
             ("brevity_penalty", bleu.brevity_penalty.to_object(py)),
             ("length_ratio", bleu.length_ratio.to_object(py)),
             ("translation_length", bleu.translation_length.to_object(py)),
```

### Comparing `bleuscore-0.1.1/src/tokenizer.rs` & `bleuscore-0.1.2/src/tokenizer.rs`

 * *Files 12% similar despite different names*

```diff
@@ -139,7 +139,26 @@
             res,
             vec![
                 "/", "usr", "/", "sbin", "/", "sendmail", "-", "0", "errors", ",", "12", "warnings"
             ]
         )
     }
 }
+
+#[cfg(test)]
+mod benchmark {
+    use crate::tokenizer;
+    use crate::tokenizer::Tokenizer;
+    use test::Bencher;
+    #[bench]
+    fn bench_tokenizer(b: &mut Bencher) {
+        let tokenizer_regex = tokenizer::Tokenizer13a::new();
+        let line = "Hello, &quot;World!<skipped>";
+
+        let iter_num: usize = 100;
+        b.iter(|| {
+            std::hint::black_box(for _ in 1..=iter_num {
+                tokenizer_regex.tokenize(line);
+            });
+        });
+    }
+}
```

### Comparing `bleuscore-0.1.1/tests/py_bleu.py` & `bleuscore-0.1.2/tests/py_bleu.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/tests/py_token.py` & `bleuscore-0.1.2/tests/py_token.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/tests/test_bleu_score.py` & `bleuscore-0.1.2/tests/test_bleu_score.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/tests/test_tokenizer.py` & `bleuscore-0.1.2/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/tests/util.py` & `bleuscore-0.1.2/tests/util.py`

 * *Files identical despite different names*

### Comparing `bleuscore-0.1.1/Cargo.lock` & `bleuscore-0.1.2/Cargo.lock`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 [[package]]
 name = "ahash"
 version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
+ "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
@@ -39,20 +40,22 @@
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bleuscore"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
+ "ahash",
  "cached",
  "counter",
  "lazy_static",
  "pyo3",
+ "rayon",
  "regex",
 ]
 
 [[package]]
 name = "cached"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -97,14 +100,39 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2d458e66999348f56fd3ffcfbb7f7951542075ca8359687c703de6500c1ddccd"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "crossbeam-deque"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
+dependencies = [
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
 name = "darling"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
@@ -132,24 +160,41 @@
 dependencies = [
  "darling_core",
  "quote",
  "syn",
 ]
 
 [[package]]
+name = "either"
+version = "1.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
+
+[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
+name = "getrandom"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "wasi",
+]
+
+[[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 dependencies = [
  "ahash",
  "allocator-api2",
 ]
 
 [[package]]
 name = "heck"
@@ -337,14 +382,34 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rayon"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
+dependencies = [
+ "either",
+ "rayon-core",
+]
+
+[[package]]
+name = "rayon-core"
+version = "1.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
+dependencies = [
+ "crossbeam-deque",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
@@ -448,14 +513,20 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "wasi"
+version = "0.11.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
+
+[[package]]
 name = "windows-targets"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
```

### Comparing `bleuscore-0.1.1/pyproject.toml` & `bleuscore-0.1.2/pyproject.toml`

 * *Files identical despite different names*

