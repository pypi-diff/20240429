# Comparing `tmp/hybrid_pke-1.0.1.tar.gz` & `tmp/hybrid_pke-1.0.2.tar.gz`

## Comparing `hybrid_pke-1.0.1.tar` & `hybrid_pke-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 hybrid_pke-1.0.1/Cargo.toml
--rw-r--r--   0      501       20      263 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/.github/release-drafter.yml
--rw-r--r--   0      501       20     5359 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/.gitignore
--rw-r--r--   0      501       20    10846 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/LICENSE
--rw-r--r--   0      501       20      818 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/Makefile
--rw-r--r--   0      501       20      278 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/NOTICE
--rw-r--r--   0      501       20     8054 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/README.md
--rw-r--r--   0      501       20      639 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/pyproject.toml
--rw-r--r--   0      501       20      291 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/release.toml
--rw-r--r--   0      501       20       86 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/requirements-dev.in
--rw-r--r--   0      501       20     1268 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/requirements-dev.txt
--rw-r--r--   0      501       20      264 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/setup.cfg
--rw-r--r--   0      501       20     2465 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/src/config.rs
--rw-r--r--   0      501       20     1594 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/src/context.rs
--rw-r--r--   0      501       20     2767 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/src/errors.rs
--rw-r--r--   0      501       20    12271 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/src/hpke.rs
--rw-r--r--   0      501       20     2255 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/src/lib.rs
--rw-r--r--   0      501       20     1645 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/tests/config_test.py
--rw-r--r--   0      501       20     1250 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/tests/context_test.py
--rw-r--r--   0      501       20     3579 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/tests/hpke_test.py
--rw-r--r--   0      501       20     5791 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/tests/kat_test.py
--rw-r--r--   0      501       20     3328 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/tests/kat_test_utils.py
--rw-r--r--   0      501       20  5892257 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/tests/test-vectors.json
--rw-r--r--   0      501       20    25810 2023-01-31 19:45:22.000000 hybrid_pke-1.0.1/Cargo.lock
--rw-r--r--   0        0        0     8644 1970-01-01 00:00:00.000000 hybrid_pke-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      466 1970-01-01 00:00:00.000000 hybrid_pke-1.0.2/Cargo.toml
+-rw-r--r--   0      501       20     4793 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      685 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/.gitignore
+-rw-r--r--   0      501       20    10846 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/LICENSE
+-rw-r--r--   0      501       20      822 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/Makefile
+-rw-r--r--   0      501       20      278 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/NOTICE
+-rw-r--r--   0      501       20     9156 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/README.md
+-rw-r--r--   0      501       20      639 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/pyproject.toml
+-rw-r--r--   0      501       20      291 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/release.toml
+-rw-r--r--   0      501       20       52 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/requirements-dev.in
+-rw-r--r--   0      501       20      641 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/requirements-dev.txt
+-rw-r--r--   0      501       20      264 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/setup.cfg
+-rw-r--r--   0      501       20     2465 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/src/config.rs
+-rw-r--r--   0      501       20     1688 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/src/context.rs
+-rw-r--r--   0      501       20     2559 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/src/errors.rs
+-rw-r--r--   0      501       20    13214 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/src/hpke.rs
+-rw-r--r--   0      501       20     2307 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/src/lib.rs
+-rw-r--r--   0      501       20     1645 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/tests/config_test.py
+-rw-r--r--   0      501       20     1250 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/tests/context_test.py
+-rw-r--r--   0      501       20     3579 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/tests/hpke_test.py
+-rw-r--r--   0      501       20     5791 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/tests/kat_test.py
+-rw-r--r--   0      501       20     3328 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/tests/kat_test_utils.py
+-rw-r--r--   0      501       20  5892257 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/tests/test-vectors.json
+-rw-r--r--   0      501       20    22114 2024-04-29 19:21:13.000000 hybrid_pke-1.0.2/Cargo.lock
+-rw-r--r--   0        0        0     9746 1970-01-01 00:00:00.000000 hybrid_pke-1.0.2/PKG-INFO
```

### Comparing `hybrid_pke-1.0.1/.github/workflows/CI.yml` & `hybrid_pke-1.0.2/.github/workflows/CI.yml`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,19 @@
   pull_request:
     branches: [ main ]
 
 jobs:
   linux:
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       id: py3
       with:
         python-version: ${{ matrix.python-version }}
         architecture: x64
     - name: Install Rust toolchain
       uses: actions-rs/toolchain@v1
       with:
@@ -49,21 +49,21 @@
       with:
         name: wheels
         path: dist
 
   windows:
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         target: [x64, x86]
     runs-on: windows-latest
     steps:
     - uses: actions/checkout@v3
     - name: Install Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       id: py3
       with:
         python-version: ${{ matrix.python-version }}
         architecture: ${{ matrix.target }}
     - name: Install Rust toolchain
       uses: actions-rs/toolchain@v1
       with:
@@ -89,20 +89,20 @@
       with:
         name: wheels
         path: dist
 
   macos:
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10", "3.11"]
-    runs-on: macos-latest
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+    runs-on: macos-13
     steps:
     - uses: actions/checkout@v3
     - name: Install Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       id: py3
       with:
         python-version: ${{ matrix.python-version }}
         architecture: x64
     - name: Install Rust toolchain
       uses: actions-rs/toolchain@v1
       with:
@@ -133,54 +133,37 @@
         pip install hybrid_pke --no-index --find-links dist --force-reinstall
         python -c "import hybrid_pke"
     - name: Upload wheels
       uses: actions/upload-artifact@v2
       with:
         name: wheels
         path: dist
-  
-  update_release_draft:
-    permissions:
-      contents: write
-      pull-requests: read
-    runs-on: ubuntu-latest
-    steps:
-    - name: Release drafter
-      id: release_drafter
-      uses: release-drafter/release-drafter@v5
-      with:
-        disable-autolabeler: true
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-    outputs:
-      upload_url: ${{ steps.release_drafter.outputs.upload_url }}
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
-    needs: [ linux, macos, windows, update_release_draft ]
+    needs: [ linux, macos, windows ]
     steps:
       - uses: actions/download-artifact@v2
         id: download
         with:
           name: wheels
       - name: Zip wheels into wheelhouse
         run: zip -r wheelhouse.zip . -i *.whl
         working-directory: ${{ steps.download.outputs.download-path }}
-      - name: Upload Release Asset
-        id: upload-release-asset
-        uses: actions/upload-release-asset@v1
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+      - name: Create GitHub Release
+        uses: softprops/action-gh-release@v2
         with:
-          upload_url: ${{ needs.update_release_draft.outputs.upload_url }}
-          asset_path: wheelhouse.zip
-          asset_name: wheelhouse.zip
-          asset_content_type: application/zip
+          generate_release_notes: true
+          files: |
+            wheelhouse.zip
+            LICENSE
+            NOTICE
+            README.md
       - uses: actions/setup-python@v2
         with:
           python-version: 3.9
       - name: Publish to PyPI
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `hybrid_pke-1.0.1/.gitignore` & `hybrid_pke-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/LICENSE` & `hybrid_pke-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/Makefile` & `hybrid_pke-1.0.2/Makefile`

 * *Files 14% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 test:
 	pytest -n auto .
 
 .PHONY: fmt
 fmt:
 	cargo fmt
 	isort .
-	black .
+	ruff format .
 
 .PHONY: lint
 lint:
 	cargo fmt --all -- --check
 	cargo clippy --all-targets -- -D warnings --no-deps
-	flake8 .
+	ruff .
 
 .PHONY: clean
 clean:
 	cargo clean
 	find ./ -depth -type d -name '__pycache__' -prune -print -exec rm -rf {} +
 
 .PHONY: ci-ready
```

### Comparing `hybrid_pke-1.0.1/README.md` & `hybrid_pke-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -216,11 +216,43 @@
 - `pytest -n auto .` runs the full test suite in parallel.
 - `maturin build --release -o dist --sdist` builds the extension module in release-mode and produces a wheel for your environment's OS and architecture.
 - The `-i`/`--interpreter` flag for `maturin` can be used to swap out different Python interpreters, if you have multiple Python installations.
 </details>
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
+## Releasing
+
+We use [`cargo-release`](https://github.com/crate-ci/cargo-release) to manage release commits and git tags. Our versioning follows SemVer, and after every release we immediately bump to a prerelease version with the `-dev0` suffix.
+
+<details><summary>Example release flow</summary>
+
+```console
+$ git checkout main
+$ cargo release patch --execute
+Upgrading hybrid_pke from X.X.X-dev0 to X.X.X
+   Replacing in pyproject.toml
+--- pyproject.toml      original
++++ pyproject.toml      replaced
+@@ -8 +8 @@
+-version = "X.X.X-dev0"  # NOTE: auto-updated during release
++version = "X.X.X"  # NOTE: auto-updated during release
+$ cargo release X.X.Y-dev0 --no-tag
+Upgrading hybrid_pke from X.X.X to X.X.Y-dev0
+   Replacing in pyproject.toml
+--- pyproject.toml      original
++++ pyproject.toml      replaced
+@@ -8 +8 @@
+-version = "X.X.X"  # NOTE: auto-updated during release
++version = "X.X.Y-dev0"  # NOTE: auto-updated during release
+$ git push origin main
+$ git push origin vX.X.X  # triggers automatic release steps in CI
+```
+
+</details>
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
 ## Related Projects
 - [hpke-py](https://github.com/ctz/hpke-py): An implementation of HPKE based on primitives from [cryptography.io](https://cryptography.io).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -95,11 +95,25 @@
 environment (`venv` or `conda` recommended) - `pytest .` tests the resulting
 Python package. - `pytest -n auto .` runs the full test suite in parallel. -
 `maturin build --release -o dist --sdist` builds the extension module in
 release-mode and produces a wheel for your environment's OS and architecture. -
 The `-i`/`--interpreter` flag for `maturin` can be used to swap out different
 Python interpreters, if you have multiple Python installations.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
+## Releasing We use [`cargo-release`](https://github.com/crate-ci/cargo-
+release) to manage release commits and git tags. Our versioning follows SemVer,
+and after every release we immediately bump to a prerelease version with the `-
+dev0` suffix. Example release flow ```console $ git checkout main $ cargo
+release patch --execute Upgrading hybrid_pke from X.X.X-dev0 to X.X.X Replacing
+in pyproject.toml --- pyproject.toml original +++ pyproject.toml replaced @@ -
+8 +8 @@ -version = "X.X.X-dev0" # NOTE: auto-updated during release +version =
+"X.X.X" # NOTE: auto-updated during release $ cargo release X.X.Y-dev0 --no-tag
+Upgrading hybrid_pke from X.X.X to X.X.Y-dev0 Replacing in pyproject.toml --
+- pyproject.toml original +++ pyproject.toml replaced @@ -8 +8 @@ -version =
+"X.X.X" # NOTE: auto-updated during release +version = "X.X.Y-dev0" # NOTE:
+auto-updated during release $ git push origin main $ git push origin vX.X.X #
+triggers automatic release steps in CI ```
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
 ## Related Projects - [hpke-py](https://github.com/ctz/hpke-py): An
 implementation of HPKE based on primitives from [cryptography.io](https://
 cryptography.io).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

### Comparing `hybrid_pke-1.0.1/pyproject.toml` & `hybrid_pke-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=0.13,<0.14"]
 build-backend = "maturin"
 
 [project]
 name = "hybrid_pke"
 description = "The Hybrid Public Key Encryption (HPKE) standard in Python"
-version = "1.0.1"  # NOTE: auto-updated during release
+version = "1.0.2"  # NOTE: auto-updated during release
 requires-python = ">=3.8"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Rust",
     "Programming Language :: Python",
```

### Comparing `hybrid_pke-1.0.1/src/config.rs` & `hybrid_pke-1.0.2/src/config.rs`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/src/context.rs` & `hybrid_pke-1.0.2/src/context.rs`

 * *Files 21% similar despite different names*

```diff
@@ -20,42 +20,42 @@
 }
 
 #[pymethods]
 impl PyContext {
     fn seal<'p>(
         &mut self,
         py: Python<'p>,
-        aad: &PyBytes,
-        plain_txt: &PyBytes,
-    ) -> PyResult<&'p PyBytes> {
+        aad: &Bound<'p, PyBytes>,
+        plain_txt: &Bound<'p, PyBytes>,
+    ) -> PyResult<Bound<'p, PyBytes>> {
         let aad = aad.as_bytes();
         let plain_txt = plain_txt.as_bytes();
         let cipher_txt = self.ctx.seal(aad, plain_txt).map_err(handle_hpke_error)?;
-        Ok(PyBytes::new(py, cipher_txt.as_slice()))
+        Ok(PyBytes::new_bound(py, cipher_txt.as_slice()))
     }
 
     fn open<'p>(
         &mut self,
         py: Python<'p>,
-        aad: &PyBytes,
-        cipher_txt: &PyBytes,
-    ) -> PyResult<&'p PyBytes> {
+        aad: &Bound<'p, PyBytes>,
+        cipher_txt: &Bound<'p, PyBytes>,
+    ) -> PyResult<Bound<'p, PyBytes>> {
         let aad = aad.as_bytes();
         let cipher_txt = cipher_txt.as_bytes();
         let plain_txt = self.ctx.open(aad, cipher_txt).map_err(handle_hpke_error)?;
-        Ok(PyBytes::new(py, plain_txt.as_slice()))
+        Ok(PyBytes::new_bound(py, plain_txt.as_slice()))
     }
 
     fn export<'p>(
         &self,
         py: Python<'p>,
-        exporter_context: &PyBytes,
+        exporter_context: &Bound<'p, PyBytes>,
         length: usize,
-    ) -> PyResult<&'p PyBytes> {
+    ) -> PyResult<Bound<'p, PyBytes>> {
         let exporter_context = exporter_context.as_bytes();
         let exporter_secret = self
             .ctx
             .export(exporter_context, length)
             .map_err(handle_hpke_error)?;
-        Ok(PyBytes::new(py, exporter_secret.as_slice()))
+        Ok(PyBytes::new_bound(py, exporter_secret.as_slice()))
     }
 }
```

### Comparing `hybrid_pke-1.0.1/src/errors.rs` & `hybrid_pke-1.0.2/src/errors.rs`

 * *Files 6% similar despite different names*

```diff
@@ -54,20 +54,14 @@
 );
 create_exception!(
     errors,
     InsufficientRandomness,
     PyException,
     "Unable to collect enough randomness."
 );
-create_exception!(
-    errors,
-    LockPoisoned,
-    PyException,
-    "A concurrency issue with an RwLock."
-);
 
 #[inline(always)]
 pub(crate) fn handle_hpke_error(e: HpkeError) -> PyErr {
     match e {
         HpkeError::OpenError => OpenError::new_err("Error opening an HPKE ciphertext."),
         HpkeError::InvalidConfig => {
             InvalidConfig::new_err("Invalid HPKE configuration or arguments.")
@@ -85,10 +79,9 @@
         HpkeError::CryptoError(s) => CryptoError::new_err(s),
         HpkeError::MessageLimitReached => {
             MessageLimitReached::new_err("Hit the message limit for this AEAD, key, and nonce.")
         }
         HpkeError::InsufficientRandomness => {
             InsufficientRandomness::new_err("Unable to collect enough randomness.")
         }
-        HpkeError::LockPoisoned => LockPoisoned::new_err("A concurrency issue with an RwLock."),
     }
 }
```

### Comparing `hybrid_pke-1.0.1/src/hpke.rs` & `hybrid_pke-1.0.2/src/hpke.rs`

 * *Files 25% similar despite different names*

```diff
@@ -43,30 +43,30 @@
             kem,
             kdf,
             aead,
             hpke,
         }
     }
 
-    pub fn __deepcopy__(&self, _memo: &PyAny) -> Self {
+    pub fn __deepcopy__(&self, _memo: Py<PyAny>) -> Self {
         self.clone()
     }
 
     /// Set up an HPKE sender context
-    #[args(psk = "None", psk_id = "None", sk_s = "None")]
+    #[pyo3(signature = ( pk_r, info, psk = None, psk_id = None, sk_s = None))]
     fn setup_sender<'p>(
-        &self,
+        &mut self,
         py: Python<'p>,
-        pk_r: &PyBytes,
-        info: &PyBytes,
-        psk: Option<&PyBytes>,
-        psk_id: Option<&PyBytes>,
-        sk_s: Option<&PyBytes>,
-    ) -> PyResult<(&'p PyBytes, PyContext)> {
-        let cfg = &self.hpke;
+        pk_r: &Bound<'p, PyBytes>,
+        info: &Bound<'p, PyBytes>,
+        psk: Option<&Bound<'p, PyBytes>>,
+        psk_id: Option<&Bound<'p, PyBytes>>,
+        sk_s: Option<&Bound<'p, PyBytes>>,
+    ) -> PyResult<(Bound<'p, PyBytes>, PyContext)> {
+        let cfg = &mut self.hpke;
 
         // convert args, drop py refs
         let pk_r = HpkePublicKey::new(pk_r.as_bytes().into());
         let info = info.as_bytes();
         let psk = psk.map(|x| x.as_bytes());
         let psk_id = psk_id.map(|x| x.as_bytes());
 
@@ -75,29 +75,29 @@
             None => cfg.setup_sender(&pk_r, info, psk, psk_id, None),
             Some(sk) => {
                 let sk = HpkePrivateKey::new(sk.as_bytes().into());
                 cfg.setup_sender(&pk_r, info, psk, psk_id, Some(&sk))
             }
         }
         .map_err(handle_hpke_error)?;
-        let encap_py = PyBytes::new(py, encap.as_slice());
+        let encap_py = PyBytes::new_bound(py, encap.as_slice());
         let context_py = PyContext::new(context);
         Ok((encap_py, context_py))
     }
 
     /// Set up an HPKE receiver context
-    #[args(psk = "None", psk_id = "None", pk_s = "None")]
-    fn setup_receiver(
+    #[pyo3(signature = (enc, sk_r, info, psk = None, psk_id = None, pk_s = None))]
+    fn setup_receiver<'p>(
         &self,
-        enc: &PyBytes,
-        sk_r: &PyBytes,
-        info: &PyBytes,
-        psk: Option<&PyBytes>,
-        psk_id: Option<&PyBytes>,
-        pk_s: Option<&PyBytes>,
+        enc: &Bound<'p, PyBytes>,
+        sk_r: &Bound<'p, PyBytes>,
+        info: &Bound<'p, PyBytes>,
+        psk: Option<&Bound<'p, PyBytes>>,
+        psk_id: Option<&Bound<'p, PyBytes>>,
+        pk_s: Option<&Bound<'p, PyBytes>>,
     ) -> PyResult<PyContext> {
         let cfg = &self.hpke;
 
         // convert args, drop py refs
         let enc = enc.as_bytes();
         let sk_r = HpkePrivateKey::new(sk_r.as_bytes().into());
         let info = info.as_bytes();
@@ -115,27 +115,27 @@
         .map_err(handle_hpke_error)?;
 
         Ok(PyContext::new(context))
     }
 
     /// Encrypt input, single-shot
     #[allow(clippy::too_many_arguments)]
-    #[args(psk = "None", psk_id = "None", sk_s = "None")]
+    #[pyo3(signature = (pk_r, info, aad, plain_txt, psk = None, psk_id = None, sk_s = None))]
     fn seal<'p>(
-        &self,
+        &mut self,
         py: Python<'p>,
-        pk_r: &PyBytes,
-        info: &PyBytes,
-        aad: &PyBytes,
-        plain_txt: &PyBytes,
-        psk: Option<&PyBytes>,
-        psk_id: Option<&PyBytes>,
-        sk_s: Option<&PyBytes>,
-    ) -> PyResult<(&'p PyBytes, &'p PyBytes)> {
-        let cfg = &self.hpke;
+        pk_r: &Bound<'p, PyBytes>,
+        info: &Bound<'p, PyBytes>,
+        aad: &Bound<'p, PyBytes>,
+        plain_txt: &Bound<'p, PyBytes>,
+        psk: Option<&Bound<'p, PyBytes>>,
+        psk_id: Option<&Bound<'p, PyBytes>>,
+        sk_s: Option<&Bound<'p, PyBytes>>,
+    ) -> PyResult<(Bound<'p, PyBytes>, Bound<'p, PyBytes>)> {
+        let cfg = &mut self.hpke;
 
         // convert args, drop py refs
         let pk_r = HpkePublicKey::new(pk_r.as_bytes().into());
         let info = info.as_bytes();
         let aad = aad.as_bytes();
         let plain_txt = plain_txt.as_bytes();
         let psk = psk.map(|x| x.as_bytes());
@@ -151,34 +151,34 @@
                 let sk = HpkePrivateKey::new(sk.as_bytes().into());
                 cfg.seal(&pk_r, info, aad, plain_txt, psk, psk_id, Some(&sk))
             }
         }
         .map_err(handle_hpke_error)?;
 
         // convert return vals back to PyBytes
-        let encap_py = PyBytes::new(py, encap.as_slice());
-        let cipher_txt_py = PyBytes::new(py, cipher_txt.as_slice());
+        let encap_py = PyBytes::new_bound(py, encap.as_slice());
+        let cipher_txt_py = PyBytes::new_bound(py, cipher_txt.as_slice());
         Ok((encap_py, cipher_txt_py))
     }
 
     /// Decrypt input, single-shot
     #[allow(clippy::too_many_arguments)]
-    #[args(psk = "None", psk_id = "None", pk_s = "None")]
+    #[pyo3(signature = (enc, sk_r, info, aad, cipher_txt, psk = None, psk_id = None, pk_s = None))]
     fn open<'p>(
         &self,
         py: Python<'p>,
-        enc: &PyBytes,
-        sk_r: &PyBytes,
-        info: &PyBytes,
-        aad: &PyBytes,
-        cipher_txt: &PyBytes,
-        psk: Option<&PyBytes>,
-        psk_id: Option<&PyBytes>,
-        pk_s: Option<&PyBytes>,
-    ) -> PyResult<&'p PyBytes> {
+        enc: &Bound<'p, PyBytes>,
+        sk_r: &Bound<'p, PyBytes>,
+        info: &Bound<'p, PyBytes>,
+        aad: &Bound<'p, PyBytes>,
+        cipher_txt: &Bound<'p, PyBytes>,
+        psk: Option<&Bound<'p, PyBytes>>,
+        psk_id: Option<&Bound<'p, PyBytes>>,
+        pk_s: Option<&Bound<'p, PyBytes>>,
+    ) -> PyResult<Bound<'p, PyBytes>> {
         let cfg = &self.hpke;
 
         // convert args, drop py refs
         let enc = enc.as_bytes();
         let sk_r = HpkePrivateKey::new(sk_r.as_bytes().into());
         let info = info.as_bytes();
         let aad = aad.as_bytes();
@@ -194,32 +194,32 @@
                 let pk = HpkePublicKey::new(pk.as_bytes().into());
                 cfg.open(enc, &sk_r, info, aad, cipher_txt, psk, psk_id, Some(&pk))
             }
         }
         .map_err(handle_hpke_error)?;
 
         // convert return val back to PyBytes
-        Ok(PyBytes::new(py, plain_txt.as_slice()))
+        Ok(PyBytes::new_bound(py, plain_txt.as_slice()))
     }
 
     /// Derive an exporter secret for sender with public key `pk_r`, single-shot
     #[allow(clippy::too_many_arguments)]
-    #[args(psk = "None", psk_id = "None", sk_s = "None")]
+    #[pyo3(signature=(pk_r, info, exporter_context, length, psk = None, psk_id = None, sk_s = None))]
     fn send_export<'p>(
-        &self,
+        &mut self,
         py: Python<'p>,
-        pk_r: &PyBytes,
-        info: &PyBytes,
-        exporter_context: &PyBytes,
+        pk_r: &Bound<'p, PyBytes>,
+        info: &Bound<'p, PyBytes>,
+        exporter_context: &Bound<'p, PyBytes>,
         length: usize,
-        psk: Option<&PyBytes>,
-        psk_id: Option<&PyBytes>,
-        sk_s: Option<&PyBytes>,
-    ) -> PyResult<(&'p PyBytes, &'p PyBytes)> {
-        let cfg = &self.hpke;
+        psk: Option<&Bound<'p, PyBytes>>,
+        psk_id: Option<&Bound<'p, PyBytes>>,
+        sk_s: Option<&Bound<'p, PyBytes>>,
+    ) -> PyResult<(Bound<'p, PyBytes>, Bound<'p, PyBytes>)> {
+        let cfg = &mut self.hpke;
 
         // convert args, drop py refs
         let pk_r = HpkePublicKey::new(pk_r.as_bytes().into());
         let info = info.as_bytes();
         let psk = psk.map(|x| x.as_bytes());
         let psk_id = psk_id.map(|x| x.as_bytes());
         let exporter_context = exporter_context.as_bytes();
@@ -239,34 +239,34 @@
                     length,
                 )
             }
         }
         .map_err(handle_hpke_error)?;
 
         // convert return vals back to PyBytes
-        let encap_py = PyBytes::new(py, encap.as_slice());
-        let exporter_secret_py = PyBytes::new(py, exporter_secret.as_slice());
+        let encap_py = PyBytes::new_bound(py, encap.as_slice());
+        let exporter_secret_py = PyBytes::new_bound(py, exporter_secret.as_slice());
         Ok((encap_py, exporter_secret_py))
     }
 
     /// Derive an exporter secret for receiver with private key `sk_r`, single-shot
     #[allow(clippy::too_many_arguments)]
-    #[args(psk = "None", psk_id = "None", pk_s = "None")]
+    #[pyo3(signature = (enc, sk_r, info, exporter_context, length, psk = None, psk_id = None, pk_s = None))]
     fn receiver_export<'p>(
         &self,
         py: Python<'p>,
-        enc: &PyBytes,
-        sk_r: &PyBytes,
-        info: &PyBytes,
-        exporter_context: &PyBytes,
+        enc: &Bound<'p, PyBytes>,
+        sk_r: &Bound<'p, PyBytes>,
+        info: &Bound<'p, PyBytes>,
+        exporter_context: &Bound<'p, PyBytes>,
         length: usize,
-        psk: Option<&PyBytes>,
-        psk_id: Option<&PyBytes>,
-        pk_s: Option<&PyBytes>,
-    ) -> PyResult<&'p PyBytes> {
+        psk: Option<&Bound<'p, PyBytes>>,
+        psk_id: Option<&Bound<'p, PyBytes>>,
+        pk_s: Option<&Bound<'p, PyBytes>>,
+    ) -> PyResult<Bound<'p, PyBytes>> {
         let cfg = &self.hpke;
 
         // convert all args and drop py refs immediately
         let enc = enc.as_bytes();
         let sk_r = HpkePrivateKey::new(sk_r.as_bytes().into());
         let info = info.as_bytes();
         let exporter_context = exporter_context.as_bytes();
@@ -297,25 +297,25 @@
                     exporter_context,
                     length,
                 )
             }
         }
         .map_err(handle_hpke_error)?;
 
-        Ok(PyBytes::new(py, exporter_secret.as_slice()))
+        Ok(PyBytes::new_bound(py, exporter_secret.as_slice()))
     }
 
     /// Create an encryption context from a shared secret
-    #[args(psk = "None", psk_id = "None")]
-    fn key_schedule(
+    #[pyo3(signature = (shared_secret, info, psk = None, psk_id = None))]
+    fn key_schedule<'p>(
         &self,
-        shared_secret: &PyBytes,
-        info: &PyBytes,
-        psk: Option<&PyBytes>,
-        psk_id: Option<&PyBytes>,
+        shared_secret: &Bound<'p, PyBytes>,
+        info: &Bound<'p, PyBytes>,
+        psk: Option<&Bound<'p, PyBytes>>,
+        psk_id: Option<&Bound<'p, PyBytes>>,
     ) -> PyResult<PyContext> {
         let no_psk = psk.is_none() & psk_id.is_none();
         let both_psk = psk.is_some() & psk_id.is_some();
         if !(no_psk | both_psk) {
             return Err(PyValueError::new_err(
                 format!("`psk` and `psk_id` must appear together or not at all. Found: psk={psk:?} and psk_id={psk_id:?}.")
             ));
@@ -329,35 +329,38 @@
         let context = cfg
             .key_schedule(shared_secret, info, psk, psk_id)
             .map_err(handle_hpke_error)?;
         Ok(PyContext::new(context))
     }
 
     /// Generate a key-pair according to the KemAlgorithm in this Hpke config
-    fn generate_key_pair<'p>(&self, py: Python<'p>) -> PyResult<(&'p PyBytes, &'p PyBytes)> {
-        let cfg = &self.hpke;
+    fn generate_key_pair<'p>(
+        &mut self,
+        py: Python<'p>,
+    ) -> PyResult<(Bound<'p, PyBytes>, Bound<'p, PyBytes>)> {
+        let cfg = &mut self.hpke;
         let keypair = cfg.generate_key_pair().map_err(handle_hpke_error)?;
         let (sk, pk) = keypair.into_keys();
-        let sk_py = PyBytes::new(py, sk.as_slice());
-        let pk_py = PyBytes::new(py, pk.as_slice());
+        let sk_py = PyBytes::new_bound(py, sk.as_slice());
+        let pk_py = PyBytes::new_bound(py, pk.as_slice());
         Ok((sk_py, pk_py))
     }
 
     /// Derive a key-pair from given randomness according to the KemAlgorithm in this Hpke config
     fn derive_key_pair<'p>(
         &self,
         py: Python<'p>,
-        ikm: &PyBytes,
-    ) -> PyResult<(&'p PyBytes, &'p PyBytes)> {
+        ikm: &Bound<'p, PyBytes>,
+    ) -> PyResult<(Bound<'p, PyBytes>, Bound<'p, PyBytes>)> {
         let cfg = &self.hpke;
         let ikm = ikm.as_bytes();
         let keypair = cfg.derive_key_pair(ikm).map_err(handle_hpke_error)?;
         let (sk, pk) = keypair.into_keys();
-        let sk_py = PyBytes::new(py, sk.as_slice());
-        let pk_py = PyBytes::new(py, pk.as_slice());
+        let sk_py = PyBytes::new_bound(py, sk.as_slice());
+        let pk_py = PyBytes::new_bound(py, pk.as_slice());
         Ok((sk_py, pk_py))
     }
 }
 
 impl From<&PyHpke> for Hpke {
     fn from(pyconfig: &PyHpke) -> Self {
         let mode = &pyconfig.mode;
```

### Comparing `hybrid_pke-1.0.1/tests/config_test.py` & `hybrid_pke-1.0.2/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/tests/context_test.py` & `hybrid_pke-1.0.2/tests/context_test.py`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/tests/hpke_test.py` & `hybrid_pke-1.0.2/tests/hpke_test.py`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/tests/kat_test.py` & `hybrid_pke-1.0.2/tests/kat_test.py`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/tests/kat_test_utils.py` & `hybrid_pke-1.0.2/tests/kat_test_utils.py`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/tests/test-vectors.json` & `hybrid_pke-1.0.2/tests/test-vectors.json`

 * *Files identical despite different names*

### Comparing `hybrid_pke-1.0.1/Cargo.lock` & `hybrid_pke-1.0.2/Cargo.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aead"
-version = "0.4.3"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b613b8e1e3cf911a086f53f03bf286f52fd7a7258e4fa606f0ef220d39d8877"
+checksum = "d122413f284cf2d62fb1b7db97e02edb8cda96d769b16e443a4f6195e35662b0"
 dependencies = [
+ "crypto-common",
  "generic-array",
 ]
 
 [[package]]
 name = "aes"
-version = "0.7.5"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e8b47f52ea9bae42228d07ec09eb676433d7c4ed1ebdf0f1d1c29ed446f1ab8"
+checksum = "b169f7a6d4742236a0a00c541b845991d0ac43e546831af1249753ab4c3aa3a0"
 dependencies = [
  "cfg-if",
  "cipher",
  "cpufeatures",
- "opaque-debug",
 ]
 
 [[package]]
 name = "aes-gcm"
-version = "0.9.4"
+version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df5f85a83a7d8b0442b6aa7b504b8212c1733da07b98aae43d4bc21b2cb3cdf6"
+checksum = "831010a0f742e1209b3bcea8fab6a8e149051ba6099432c8cb2cc117dec3ead1"
 dependencies = [
  "aead",
  "aes",
  "cipher",
  "ctr",
  "ghash",
  "subtle",
@@ -41,120 +41,94 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base16ct"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "349a06037c7bf932dd7e7d1f653678b2038b9ad46a74102f1fc7bd7872678cce"
-
-[[package]]
-name = "base64ct"
-version = "1.5.3"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b645a089122eccb6111b4f81cbc1a49f5900ac4666bb93ac027feaecf15607bf"
+checksum = "4c7f02d4ea65f2c1853089ffd8d2787bdbc63de2f0d29dedbcf8ccdfa0ccd4cf"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4152116fd6e9dadb291ae18fc1ec3575ed6d84c29642d97890f4b4a3417297e4"
-dependencies = [
- "generic-array",
-]
-
-[[package]]
-name = "block-buffer"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
-name = "bumpalo"
-version = "3.12.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
-
-[[package]]
-name = "byteorder"
-version = "1.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
-
-[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chacha20"
-version = "0.8.2"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c80e5460aa66fe3b91d40bcbdab953a597b60053e34d684ac6903f863b680a6"
+checksum = "c3613f74bd2eac03dad61bd53dbe620703d4371614fe0bc3b9f04dd36fe4e818"
 dependencies = [
  "cfg-if",
  "cipher",
  "cpufeatures",
- "zeroize",
 ]
 
 [[package]]
 name = "chacha20poly1305"
-version = "0.9.1"
+version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18446b09be63d457bbec447509e85f662f32952b035ce892290396bc0b0cff5"
+checksum = "10cd79432192d1c0f4e1a0fef9527696cc039165d729fb41b3f4f4f354c2dc35"
 dependencies = [
  "aead",
  "chacha20",
  "cipher",
  "poly1305",
  "zeroize",
 ]
 
 [[package]]
 name = "cipher"
-version = "0.3.0"
+version = "0.4.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ee52072ec15386f770805afd189a01c8841be8696bed250fa2f13c4c0d6dfb7"
+checksum = "773f3b9af64447d2ce9850330c473515014aa235e6a783b02db81ff39e4a3dad"
 dependencies = [
- "generic-array",
+ "crypto-common",
+ "inout",
+ "zeroize",
 ]
 
 [[package]]
 name = "const-oid"
-version = "0.7.1"
+version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4c78c047431fee22c1a7bb92e00ad095a02a983affe4d8a72e2a2c62c1b94f3"
+checksum = "c2459377285ad874054d797f3ccebf984978aa39129f6eafde5cdc8315b612f8"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crypto-bigint"
-version = "0.3.2"
+version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03c6a1d5fa1de37e071642dfa44ec552ca5b299adb128fab16138e24b548fd21"
+checksum = "0dc92fb57ca44df6db8059111ab3af99a63d5d0f8375d9972e319a379c6bab76"
 dependencies = [
  "generic-array",
  "rand_core",
  "subtle",
  "zeroize",
 ]
 
@@ -165,266 +139,241 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
-name = "crypto-mac"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1d1a86f49236c215f271d40892d5fc950490551400b02ef360692c29815c714"
-dependencies = [
- "generic-array",
- "subtle",
-]
-
-[[package]]
 name = "ctr"
-version = "0.8.0"
+version = "0.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "049bb91fb4aaf0e3c7efa6cd5ef877dbbbd15b39dad06d9948de4ec8a75761ea"
+checksum = "0369ee1ad671834580515889b80f2ea915f23b8be8d0daa4bbaf2ac5c7590835"
 dependencies = [
  "cipher",
 ]
 
 [[package]]
-name = "curve25519-dalek-ng"
-version = "4.1.1"
+name = "curve25519-dalek"
+version = "4.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c359b7249347e46fb28804470d071c921156ad62b3eef5d34e2ba867533dec8"
+checksum = "0a677b8922c94e01bdbb12126b0bc852f00447528dee1782229af9c720c3f348"
 dependencies = [
- "byteorder",
- "digest 0.9.0",
- "rand_core",
- "subtle-ng",
+ "cfg-if",
+ "cpufeatures",
+ "curve25519-dalek-derive",
+ "fiat-crypto",
+ "platforms",
+ "rustc_version",
+ "subtle",
  "zeroize",
 ]
 
 [[package]]
-name = "der"
-version = "0.5.1"
+name = "curve25519-dalek-derive"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6919815d73839e7ad218de758883aae3a257ba6759ce7a9992501efbb53d705c"
+checksum = "f46882e17999c6cc590af592290432be3bce0428cb0d5f8b6715e4dc7b383eb3"
 dependencies = [
- "const-oid",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
 ]
 
 [[package]]
-name = "digest"
-version = "0.9.0"
+name = "der"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3dd60d1080a57a05ab032377049e0591415d2b31afd7028356dbf3cc6dcb066"
+checksum = "f55bf8e7b65898637379c1b74eb1551107c8294ed26d855ceb9fd1a09cfc9bc0"
 dependencies = [
- "generic-array",
+ "const-oid",
+ "zeroize",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
 dependencies = [
- "block-buffer 0.10.3",
+ "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
-name = "ecdsa"
-version = "0.13.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0d69ae62e0ce582d56380743515fefaf1a8c70cec685d9677636d7e30ae9dc9"
-dependencies = [
- "der",
- "elliptic-curve",
- "rfc6979",
- "signature",
-]
-
-[[package]]
 name = "elliptic-curve"
-version = "0.11.12"
+version = "0.13.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25b477563c2bfed38a3b7a60964c49e058b2510ad3f12ba3483fd8f62c2306d6"
+checksum = "b5e6043086bf7973472e0c7dff2142ea0b680d30e18d9cc40f267efbf222bd47"
 dependencies = [
  "base16ct",
  "crypto-bigint",
- "der",
+ "digest",
  "ff",
  "generic-array",
  "group",
+ "hkdf",
  "rand_core",
  "sec1",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "ff"
-version = "0.11.1"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "131655483be284720a17d74ff97592b8e76576dc25563148601df2d7c9080924"
+checksum = "ded41244b729663b1e574f1b4fb731469f69f79c17667b5d776b16cda0479449"
 dependencies = [
  "rand_core",
  "subtle",
 ]
 
 [[package]]
+name = "fiat-crypto"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c007b1ae3abe1cb6f85a16305acd418b7ca6343b953633fee2b76d8f108b830f"
+
+[[package]]
 name = "generic-array"
 version = "0.14.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
 dependencies = [
  "typenum",
  "version_check",
+ "zeroize",
 ]
 
 [[package]]
 name = "getrandom"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
 dependencies = [
  "cfg-if",
- "js-sys",
  "libc",
  "wasi",
- "wasm-bindgen",
 ]
 
 [[package]]
 name = "ghash"
-version = "0.4.4"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1583cc1656d7839fd3732b80cf4f38850336cdb9b8ded1cd399ca62958de3c99"
+checksum = "f0d8a4362ccb29cb0b265253fb0a2728f592895ee6854fd9bc13f2ffda266ff1"
 dependencies = [
  "opaque-debug",
  "polyval",
 ]
 
 [[package]]
 name = "group"
-version = "0.11.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc5ac374b108929de78460075f3dc439fa66df9d8fc77e8f12caa5165fcf0c89"
+checksum = "f0f9ef7462f7c099f518d754361858f86d8a07af53ba9af0fe635bbccb151a63"
 dependencies = [
  "ff",
  "rand_core",
  "subtle",
 ]
 
 [[package]]
-name = "hkdf"
-version = "0.12.3"
+name = "heck"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "791a029f6b9fc27657f6f188ec6e5e43f6911f6f878e0dc5501396e09809d437"
-dependencies = [
- "hmac 0.12.1",
-]
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
-name = "hmac"
-version = "0.11.0"
+name = "hkdf"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a2a2320eb7ec0ebe8da8f744d7812d9fc4cb4d09344ac01898dbcb6a20ae69b"
+checksum = "791a029f6b9fc27657f6f188ec6e5e43f6911f6f878e0dc5501396e09809d437"
 dependencies = [
- "crypto-mac",
- "digest 0.9.0",
+ "hmac",
 ]
 
 [[package]]
 name = "hmac"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
- "digest 0.10.6",
+ "digest",
 ]
 
 [[package]]
 name = "hpke-rs"
-version = "0.1.0"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9c8449efb0694b5dd0ee0d7a5582eccce1eb3aeb6c25dc569143ceadc536ca5"
+checksum = "e11bd4ee27b79fa1820e72ef8489cc729c87299ec3f7f52b8fc8dcb87cb2d485"
 dependencies = [
  "hpke-rs-crypto",
  "log",
  "zeroize",
 ]
 
 [[package]]
 name = "hpke-rs-crypto"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fdcfe5eed821c92bedc9d05a1e8b4d42a858e5326031086bb5256b778ce9455"
+checksum = "1c3f1ae0a26c18d6469a70db1217136056261c4a244b09a755bc60bd4e055b67"
 dependencies = [
- "getrandom",
- "rand",
- "serde",
- "serde_json",
- "tls_codec",
+ "rand_core",
 ]
 
 [[package]]
 name = "hpke-rs-rust-crypto"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8603fbb7674b627cb9f3de6ae5ba8b7e621ef5fdea6489363cb4bef26e5fce52"
+checksum = "a08d4500baf0aced746723d3515d08212bdb9d941df6d1aca3d46d1619b2a1cf"
 dependencies = [
  "aes-gcm",
  "chacha20poly1305",
- "getrandom",
  "hkdf",
  "hpke-rs-crypto",
  "p256",
  "p384",
- "rand",
  "rand_chacha",
- "sha2 0.10.6",
- "x25519-dalek-ng",
+ "rand_core",
+ "sha2",
+ "x25519-dalek",
 ]
 
 [[package]]
 name = "hybrid_pke"
-version = "1.0.1"
+version = "1.0.2"
 dependencies = [
  "hpke-rs",
  "hpke-rs-crypto",
  "hpke-rs-rust-crypto",
  "pyo3",
  "rand",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
-name = "itoa"
-version = "1.0.5"
+name = "inout"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
-
-[[package]]
-name = "js-sys"
-version = "0.3.60"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "a0c10553d664a4d0bcff9f4215d0aac67a639cc68ef660840afe309b807bc9f5"
 dependencies = [
- "wasm-bindgen",
+ "generic-array",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -439,17 +388,17 @@
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.17.0"
@@ -460,32 +409,30 @@
 name = "opaque-debug"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "624a8340c38c1b80fd549087862da4ba43e08858af025b236e509b6649fc13d5"
 
 [[package]]
 name = "p256"
-version = "0.10.1"
+version = "0.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19736d80675fbe9fe33426268150b951a3fb8f5cfca2a23a17c85ef3adb24e3b"
+checksum = "c9863ad85fa8f4460f9c48cb909d38a0d689dba1f6f6988a5e3e0d31071bcd4b"
 dependencies = [
- "ecdsa",
  "elliptic-curve",
- "sec1",
- "sha2 0.9.9",
+ "primeorder",
 ]
 
 [[package]]
 name = "p384"
-version = "0.9.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "755d8266e41f57bd8562ed9b6e93cdcf73ead050e1e8c3a27ea3871b6643a20c"
+checksum = "70786f51bcc69f6a4c0360e063a4cac5419ef7c5cd5b3c99ad70f3be5ba79209"
 dependencies = [
  "elliptic-curve",
- "sec1",
+ "primeorder",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
@@ -504,127 +451,140 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
-name = "pkcs8"
-version = "0.8.0"
+name = "platforms"
+version = "3.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7cabda3fb821068a9a4fab19a683eac3af12edf0f34b94a8be53c4972b8149d0"
-dependencies = [
- "der",
- "spki",
- "zeroize",
-]
+checksum = "db23d408679286588f4d4644f965003d056e3dd5abcaaa938116871d7ce2fee7"
 
 [[package]]
 name = "poly1305"
-version = "0.7.2"
+version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "048aeb476be11a4b6ca432ca569e375810de9294ae78f4774e78ea98a9246ede"
+checksum = "8159bd90725d2df49889a078b54f4f79e87f1f8a8444194cdca81d38f5393abf"
 dependencies = [
  "cpufeatures",
  "opaque-debug",
  "universal-hash",
 ]
 
 [[package]]
 name = "polyval"
-version = "0.5.3"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8419d2b623c7c0896ff2d5d96e2cb4ede590fed28fcc34934f4c33c036e620a1"
+checksum = "9d1fe60d06143b2430aa532c94cfe9e29783047f06c0d7fd359a9a51b729fa25"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "opaque-debug",
  "universal-hash",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "primeorder"
+version = "0.13.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "353e1ca18966c16d9deb1c69278edbc5f194139612772bd9537af60ac231e1e6"
+dependencies = [
+ "elliptic-curve",
+]
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.50"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ef7d57beacfaf2d8aee5937dab7b7f28de3cb8b1828479bb5de2a7106f2bae2"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -661,50 +621,48 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "rfc6979"
-version = "0.1.0"
+name = "rustc_version"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96ef608575f6392792f9ecf7890c00086591d29a83910939d430753f7c050525"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
- "crypto-bigint",
- "hmac 0.11.0",
- "zeroize",
+ "semver",
 ]
 
 [[package]]
-name = "ryu"
-version = "1.0.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
-
-[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "sec1"
-version = "0.2.1"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08da66b8b0965a5555b6bd6639e68ccba85e1e2506f5fbb089e93f8a04e1a2d1"
+checksum = "48518a2b5775ba8ca5b46596aae011caa431e6ce7e4a67ead66d92f08884220e"
 dependencies = [
+ "base16ct",
  "der",
  "generic-array",
- "pkcs8",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
+name = "semver"
+version = "1.0.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
+
+[[package]]
 name = "serde"
 version = "1.0.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
 dependencies = [
  "serde_derive",
 ]
@@ -713,141 +671,81 @@
 name = "serde_derive"
 version = "1.0.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
-]
-
-[[package]]
-name = "serde_json"
-version = "1.0.91"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "877c235533714907a8c2464236f5c4b2a17262ef1bd71f38f35ea592c8da6883"
-dependencies = [
- "itoa",
- "ryu",
- "serde",
-]
-
-[[package]]
-name = "sha2"
-version = "0.9.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d58a1e1bf39749807d89cf2d98ac2dfa0ff1cb3faa38fbb64dd88ac8013d800"
-dependencies = [
- "block-buffer 0.9.0",
- "cfg-if",
- "cpufeatures",
- "digest 0.9.0",
- "opaque-debug",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if",
  "cpufeatures",
- "digest 0.10.6",
-]
-
-[[package]]
-name = "signature"
-version = "1.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02658e48d89f2bec991f9a78e69cfa4c316f8d6a6c4ec12fae1aeb263d486788"
-dependencies = [
- "digest 0.9.0",
- "rand_core",
+ "digest",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
-name = "spki"
-version = "0.5.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d01ac02a6ccf3e07db148d2be087da624fea0221a16152ed01f0496a6b0a27"
-dependencies = [
- "base64ct",
- "der",
-]
-
-[[package]]
 name = "subtle"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
 
 [[package]]
-name = "subtle-ng"
-version = "2.5.0"
+name = "syn"
+version = "1.0.107"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "734676eb262c623cec13c3155096e08d1f8f29adce39ba17948b18dad1e54142"
+checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "synstructure"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "unicode-xid",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
 
 [[package]]
-name = "tls_codec"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "172a9c24d46b5fe280b77f37161ed9a919229cb104085384e8bf30637c2e4bca"
-dependencies = [
- "tls_codec_derive",
- "zeroize",
-]
-
-[[package]]
-name = "tls_codec_derive"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a787719c86efec1535b071bde678f5fd649380e8005cd1ebd0afeb4bcc4d2a85"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
@@ -859,25 +757,25 @@
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "universal-hash"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f214e8f697e925001e66ec2c6e37a4ef93f0f78c2eed7814394e10c62025b05"
+checksum = "fc1de2c688dc15305988b563c3854064043356019f97a4b46276fe734c4f07ea"
 dependencies = [
- "generic-array",
+ "crypto-common",
  "subtle",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -886,68 +784,14 @@
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
-name = "wasm-bindgen"
-version = "0.2.83"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
-dependencies = [
- "cfg-if",
- "wasm-bindgen-macro",
-]
-
-[[package]]
-name = "wasm-bindgen-backend"
-version = "0.2.83"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
-dependencies = [
- "bumpalo",
- "log",
- "once_cell",
- "proc-macro2",
- "quote",
- "syn",
- "wasm-bindgen-shared",
-]
-
-[[package]]
-name = "wasm-bindgen-macro"
-version = "0.2.83"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
-dependencies = [
- "quote",
- "wasm-bindgen-macro-support",
-]
-
-[[package]]
-name = "wasm-bindgen-macro-support"
-version = "0.2.83"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
- "wasm-bindgen-backend",
- "wasm-bindgen-shared",
-]
-
-[[package]]
-name = "wasm-bindgen-shared"
-version = "0.2.83"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
-
-[[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
@@ -997,38 +841,38 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "447660ad36a13288b1db4d4248e857b510e8c3a225c822ba4fb748c0aafecffd"
 
 [[package]]
-name = "x25519-dalek-ng"
-version = "1.1.1"
+name = "x25519-dalek"
+version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7074de8999662970c3c4c8f7f30925028dd8f4ca31ad4c055efa9cdf2ec326"
+checksum = "c7e468321c81fb07fa7f4c636c3972b9100f0346e5b6a9f2bd0603a52f7ed277"
 dependencies = [
- "curve25519-dalek-ng",
- "rand",
+ "curve25519-dalek",
  "rand_core",
+ "serde",
  "zeroize",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.5.7"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c394b5bd0c6f669e7275d9c20aa90ae064cb22e75a1cad54e1b34088034b149f"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
 dependencies = [
  "zeroize_derive",
 ]
 
 [[package]]
 name = "zeroize_derive"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44bf07cb3e50ea2003396695d58bf46bc9887a1f362260446fad6bc4e79bd36c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "synstructure",
 ]
```

### Comparing `hybrid_pke-1.0.1/PKG-INFO` & `hybrid_pke-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hybrid_pke
-Version: 1.0.1
+Version: 1.0.2
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security :: Cryptography
 License-File: LICENSE
 License-File: NOTICE
@@ -231,11 +231,43 @@
 - `pytest -n auto .` runs the full test suite in parallel.
 - `maturin build --release -o dist --sdist` builds the extension module in release-mode and produces a wheel for your environment's OS and architecture.
 - The `-i`/`--interpreter` flag for `maturin` can be used to swap out different Python interpreters, if you have multiple Python installations.
 </details>
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
+## Releasing
+
+We use [`cargo-release`](https://github.com/crate-ci/cargo-release) to manage release commits and git tags. Our versioning follows SemVer, and after every release we immediately bump to a prerelease version with the `-dev0` suffix.
+
+<details><summary>Example release flow</summary>
+
+```console
+$ git checkout main
+$ cargo release patch --execute
+Upgrading hybrid_pke from X.X.X-dev0 to X.X.X
+   Replacing in pyproject.toml
+--- pyproject.toml      original
++++ pyproject.toml      replaced
+@@ -8 +8 @@
+-version = "X.X.X-dev0"  # NOTE: auto-updated during release
++version = "X.X.X"  # NOTE: auto-updated during release
+$ cargo release X.X.Y-dev0 --no-tag
+Upgrading hybrid_pke from X.X.X to X.X.Y-dev0
+   Replacing in pyproject.toml
+--- pyproject.toml      original
++++ pyproject.toml      replaced
+@@ -8 +8 @@
+-version = "X.X.X"  # NOTE: auto-updated during release
++version = "X.X.Y-dev0"  # NOTE: auto-updated during release
+$ git push origin main
+$ git push origin vX.X.X  # triggers automatic release steps in CI
+```
+
+</details>
+
+<p align="right">(<a href="#top">back to top</a>)</p>
+
 ## Related Projects
 - [hpke-py](https://github.com/ctz/hpke-py): An implementation of HPKE based on primitives from [cryptography.io](https://cryptography.io).
 
 <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hybrid_pke Version: 1.0.1 Classifier: License ::
+Metadata-Version: 2.1 Name: hybrid_pke Version: 1.0.2 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Rust Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Topic :: Security
 :: Cryptography License-File: LICENSE License-File: NOTICE Summary: The Hybrid
 Public Key Encryption (HPKE) standard in Python Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM Project-
 URL: repository, https://github.com/capeprivacy/hybrid-pke Hybrid PKE
@@ -103,11 +103,25 @@
 environment (`venv` or `conda` recommended) - `pytest .` tests the resulting
 Python package. - `pytest -n auto .` runs the full test suite in parallel. -
 `maturin build --release -o dist --sdist` builds the extension module in
 release-mode and produces a wheel for your environment's OS and architecture. -
 The `-i`/`--interpreter` flag for `maturin` can be used to swap out different
 Python interpreters, if you have multiple Python installations.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
+## Releasing We use [`cargo-release`](https://github.com/crate-ci/cargo-
+release) to manage release commits and git tags. Our versioning follows SemVer,
+and after every release we immediately bump to a prerelease version with the `-
+dev0` suffix. Example release flow ```console $ git checkout main $ cargo
+release patch --execute Upgrading hybrid_pke from X.X.X-dev0 to X.X.X Replacing
+in pyproject.toml --- pyproject.toml original +++ pyproject.toml replaced @@ -
+8 +8 @@ -version = "X.X.X-dev0" # NOTE: auto-updated during release +version =
+"X.X.X" # NOTE: auto-updated during release $ cargo release X.X.Y-dev0 --no-tag
+Upgrading hybrid_pke from X.X.X to X.X.Y-dev0 Replacing in pyproject.toml --
+- pyproject.toml original +++ pyproject.toml replaced @@ -8 +8 @@ -version =
+"X.X.X" # NOTE: auto-updated during release +version = "X.X.Y-dev0" # NOTE:
+auto-updated during release $ git push origin main $ git push origin vX.X.X #
+triggers automatic release steps in CI ```
+                                                                  (_b_a_c_k_ _t_o_ _t_o_p)
 ## Related Projects - [hpke-py](https://github.com/ctz/hpke-py): An
 implementation of HPKE based on primitives from [cryptography.io](https://
 cryptography.io).
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
```

