# Comparing `tmp/bosing-2.0.0b7.tar.gz` & `tmp/bosing-2.0.0b8.tar.gz`

## Comparing `bosing-2.0.0b7.tar` & `bosing-2.0.0b8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 bosing-2.0.0b7/Cargo.toml
--rw-r--r--   0     1001      127      505 2024-04-26 16:24:55.000000 bosing-2.0.0b7/.github/dependabot.yml
--rw-r--r--   0     1001      127     6323 2024-04-26 16:24:55.000000 bosing-2.0.0b7/.github/workflows/ci.yml
--rw-r--r--   0     1001      127      696 2024-04-26 16:24:55.000000 bosing-2.0.0b7/.gitignore
--rw-r--r--   0     1001      127      972 2024-04-26 16:24:55.000000 bosing-2.0.0b7/.readthedocs.yaml
--rw-r--r--   0     1001      127     1068 2024-04-26 16:24:55.000000 bosing-2.0.0b7/LICENSE.txt
--rw-r--r--   0     1001      127     1360 2024-04-26 16:24:55.000000 bosing-2.0.0b7/README.md
--rw-r--r--   0     1001      127    10185 2024-04-26 16:24:55.000000 bosing-2.0.0b7/bosing.pyi
--rw-r--r--   0     1001      127       78 2024-04-26 16:24:55.000000 bosing-2.0.0b7/clippy.toml
--rw-r--r--   0     1001      127      634 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/Makefile
--rw-r--r--   0     1001      127      175 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      127     1147 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/_templates/autosummary/module.rst
--rw-r--r--   0     1001      127       82 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/api.rst
--rw-r--r--   0     1001      127     1464 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/conf.py
--rw-r--r--   0     1001      127     1258 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/index.rst
--rw-r--r--   0     1001      127     1716 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/instruction.rst
--rw-r--r--   0     1001      127      765 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/make.bat
--rw-r--r--   0     1001      127      347 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/quickstart.rst
--rw-r--r--   0     1001      127       22 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/requirements.txt
--rw-r--r--   0     1001      127     5534 2024-04-26 16:24:55.000000 bosing-2.0.0b7/docs/schedule.rst
--rw-r--r--   0     1001      127     1171 2024-04-26 16:24:55.000000 bosing-2.0.0b7/example/flexible.py
--rw-r--r--   0     1001      127      533 2024-04-26 16:24:55.000000 bosing-2.0.0b7/example/hann.py
--rw-r--r--   0     1001      127      788 2024-04-26 16:24:55.000000 bosing-2.0.0b7/example/interp.py
--rw-r--r--   0     1001      127      696 2024-04-26 16:24:55.000000 bosing-2.0.0b7/example/overlap.py
--rw-r--r--   0     1001      127     2074 2024-04-26 16:24:55.000000 bosing-2.0.0b7/example/schedule.py
--rw-r--r--   0     1001      127     1924 2024-04-26 16:24:55.000000 bosing-2.0.0b7/example/schedule_stress.py
--rw-r--r--   0     1001      127     6064 2024-04-26 16:24:55.000000 bosing-2.0.0b7/ruff_defaults.toml
--rw-r--r--   0     1001      127     7368 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/executor.rs
--rw-r--r--   0     1001      127    62172 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/lib.rs
--rw-r--r--   0     1001      127    12363 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/pulse.rs
--rw-r--r--   0     1001      127     1667 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/quant.rs
--rw-r--r--   0     1001      127     2481 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/schedule/absolute.rs
--rw-r--r--   0     1001      127     7389 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/schedule/grid.rs
--rw-r--r--   0     1001      127     3326 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/schedule/play.rs
--rw-r--r--   0     1001      127     2350 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/schedule/repeat.rs
--rw-r--r--   0     1001      127     3966 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/schedule/simple.rs
--rw-r--r--   0     1001      127     5760 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/schedule/stack.rs
--rw-r--r--   0     1001      127    11084 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/schedule.rs
--rw-r--r--   0     1001      127     6642 2024-04-26 16:24:55.000000 bosing-2.0.0b7/src/shape.rs
--rw-r--r--   0     1001      127       14 2024-04-26 16:24:55.000000 bosing-2.0.0b7/stubtest-allowlist.txt
--rw-r--r--   0     1001      127        0 2024-04-26 16:24:55.000000 bosing-2.0.0b7/tests/__init__.py
--rw-r--r--   0     1001      127     1291 2024-04-26 16:24:55.000000 bosing-2.0.0b7/tests/test_basic.py
--rw-r--r--   0     1001      127    18607 2024-04-26 16:25:00.000000 bosing-2.0.0b7/Cargo.lock
--rw-r--r--   0     1001      127     1867 2024-04-26 16:24:55.000000 bosing-2.0.0b7/pyproject.toml
--rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 bosing-2.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 bosing-2.0.0b8/Cargo.toml
+-rw-r--r--   0     1001      127      505 2024-04-29 09:00:49.000000 bosing-2.0.0b8/.github/dependabot.yml
+-rw-r--r--   0     1001      127     6323 2024-04-29 09:00:49.000000 bosing-2.0.0b8/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      696 2024-04-29 09:00:49.000000 bosing-2.0.0b8/.gitignore
+-rw-r--r--   0     1001      127      972 2024-04-29 09:00:49.000000 bosing-2.0.0b8/.readthedocs.yaml
+-rw-r--r--   0     1001      127     1068 2024-04-29 09:00:49.000000 bosing-2.0.0b8/LICENSE.txt
+-rw-r--r--   0     1001      127     1360 2024-04-29 09:00:49.000000 bosing-2.0.0b8/README.md
+-rw-r--r--   0     1001      127    10422 2024-04-29 09:00:49.000000 bosing-2.0.0b8/bosing.pyi
+-rw-r--r--   0     1001      127       78 2024-04-29 09:00:49.000000 bosing-2.0.0b8/clippy.toml
+-rw-r--r--   0     1001      127      634 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/Makefile
+-rw-r--r--   0     1001      127      175 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      127     1147 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/_templates/autosummary/module.rst
+-rw-r--r--   0     1001      127       82 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/api.rst
+-rw-r--r--   0     1001      127     1464 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/conf.py
+-rw-r--r--   0     1001      127     1258 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/index.rst
+-rw-r--r--   0     1001      127     1716 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/instruction.rst
+-rw-r--r--   0     1001      127      765 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/make.bat
+-rw-r--r--   0     1001      127      347 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/quickstart.rst
+-rw-r--r--   0     1001      127       22 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/requirements.txt
+-rw-r--r--   0     1001      127     5534 2024-04-29 09:00:49.000000 bosing-2.0.0b8/docs/schedule.rst
+-rw-r--r--   0     1001      127     1171 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/flexible.py
+-rw-r--r--   0     1001      127      533 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/hann.py
+-rw-r--r--   0     1001      127      788 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/interp.py
+-rw-r--r--   0     1001      127      696 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/overlap.py
+-rw-r--r--   0     1001      127     2074 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/schedule.py
+-rw-r--r--   0     1001      127     1956 2024-04-29 09:00:49.000000 bosing-2.0.0b8/example/schedule_stress.py
+-rw-r--r--   0     1001      127     6064 2024-04-29 09:00:49.000000 bosing-2.0.0b8/ruff_defaults.toml
+-rw-r--r--   0     1001      127     7368 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/executor.rs
+-rw-r--r--   0     1001      127    63728 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/lib.rs
+-rw-r--r--   0     1001      127    12363 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/pulse.rs
+-rw-r--r--   0     1001      127     1667 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/quant.rs
+-rw-r--r--   0     1001      127     2481 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/absolute.rs
+-rw-r--r--   0     1001      127     7389 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/grid.rs
+-rw-r--r--   0     1001      127     3326 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/play.rs
+-rw-r--r--   0     1001      127     2350 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/repeat.rs
+-rw-r--r--   0     1001      127     3966 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/simple.rs
+-rw-r--r--   0     1001      127     5760 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule/stack.rs
+-rw-r--r--   0     1001      127    11084 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/schedule.rs
+-rw-r--r--   0     1001      127     6642 2024-04-29 09:00:49.000000 bosing-2.0.0b8/src/shape.rs
+-rw-r--r--   0     1001      127       14 2024-04-29 09:00:49.000000 bosing-2.0.0b8/stubtest-allowlist.txt
+-rw-r--r--   0     1001      127        0 2024-04-29 09:00:49.000000 bosing-2.0.0b8/tests/__init__.py
+-rw-r--r--   0     1001      127     1291 2024-04-29 09:00:49.000000 bosing-2.0.0b8/tests/test_basic.py
+-rw-r--r--   0     1001      127    18617 2024-04-29 09:01:00.000000 bosing-2.0.0b8/Cargo.lock
+-rw-r--r--   0     1001      127     1867 2024-04-29 09:00:49.000000 bosing-2.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 bosing-2.0.0b8/PKG-INFO
```

### Comparing `bosing-2.0.0b7/Cargo.toml` & `bosing-2.0.0b8/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "bosing"
-version = "2.0.0-beta.7"
+version = "2.0.0-beta.8"
 edition = "2021"
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "bosing"
 crate-type = ["cdylib"]
@@ -12,14 +12,15 @@
 [dependencies]
 anyhow = "1.0.82"
 bspline = "1.1.0"
 cached = "0.49.3"
 enum_dispatch = "0.3.13"
 float-cmp = "0.9.0"
 hashbrown = { version = "0.14.3", features = ["rayon"] }
+indoc = "2.0.5"
 itertools = "0.12.1"
 ndarray = { version = "0.15.6", features = ["rayon"] }
 num = "0.4.1"
 numpy = "0.21.0"
 ordered-float = "4.2.0"
 pyo3 = { version = "0.21.0", features = ["hashbrown"] }
 rayon = "1.10.0"
```

### Comparing `bosing-2.0.0b7/.github/workflows/ci.yml` & `bosing-2.0.0b8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/.gitignore` & `bosing-2.0.0b8/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/.readthedocs.yaml` & `bosing-2.0.0b8/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/LICENSE.txt` & `bosing-2.0.0b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/README.md` & `bosing-2.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/bosing.pyi` & `bosing-2.0.0b8/bosing.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,31 @@
         cls,
         base_freq: float,
         sample_rate: float,
         length: int,
         *,
         delay: float = ...,
         align_level: int = ...,
+        iq_matrix: npt.ArrayLike | None = ...,
+        iq_offset: tuple[float, float] | None = ...,
     ) -> Self: ...
     @property
     def base_freq(self) -> float: ...
     @property
     def sample_rate(self) -> float: ...
     @property
     def length(self) -> int: ...
     @property
     def delay(self) -> float: ...
     @property
     def align_level(self) -> int: ...
+    @property
+    def iq_matrix(self) -> np.ndarray | None: ...
+    @property
+    def iq_offset(self) -> tuple[float, float] | None: ...
 
 @final
 class Alignment:
     End: ClassVar[Alignment]
     Start: ClassVar[Alignment]
     Center: ClassVar[Alignment]
     Stretch: ClassVar[Alignment]
```

### Comparing `bosing-2.0.0b7/docs/Makefile` & `bosing-2.0.0b8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/docs/_templates/autosummary/module.rst` & `bosing-2.0.0b8/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/docs/conf.py` & `bosing-2.0.0b8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/docs/index.rst` & `bosing-2.0.0b8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/docs/instruction.rst` & `bosing-2.0.0b8/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/docs/make.bat` & `bosing-2.0.0b8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/docs/schedule.rst` & `bosing-2.0.0b8/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/example/flexible.py` & `bosing-2.0.0b8/example/flexible.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/example/hann.py` & `bosing-2.0.0b8/example/hann.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/example/interp.py` & `bosing-2.0.0b8/example/interp.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/example/overlap.py` & `bosing-2.0.0b8/example/overlap.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/example/schedule.py` & `bosing-2.0.0b8/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/example/schedule_stress.py` & `bosing-2.0.0b8/example/schedule_stress.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 def gen_n(n: int):
     t0 = time.perf_counter()
     nxy = 64
     nu = 2 * nxy
     nm = nxy // 8
     channels = (
-        {f"xy{i}": Channel(3e6 * i, 2e9, 100000) for i in range(nxy)}
+        {f"xy{i}": Channel(3e6 * i, 2e9, 100000, iq_matrix=[[1, 0.1], [0.1, 1]]) for i in range(nxy)}
         | {f"u{i}": Channel(0, 2e9, 100000) for i in range(nu)}
         | {f"m{i}": Channel(0, 2e9, 100000) for i in range(nm)}
     )
     halfcos = np.sin(np.linspace(0, np.pi, 10))
     spline = make_interp_spline(np.linspace(-0.5, 0.5, 10), halfcos)
     shapes = {
         "hann": Hann(),
```

### Comparing `bosing-2.0.0b7/ruff_defaults.toml` & `bosing-2.0.0b8/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/executor.rs` & `bosing-2.0.0b8/src/executor.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/lib.rs` & `bosing-2.0.0b8/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 //! Although Element struct may contains [`Py<Element>`] as children, it is not
 //! possible to create cyclic references because we don't allow mutate the
 //! children after creation.
 use std::sync::Arc;
 
 use hashbrown::HashMap;
-use numpy::{prelude::*, AllowTypeChange, PyArray2, PyArrayLike2};
+use indoc::indoc;
+use numpy::{dot_bound, prelude::*, pyarray_bound, AllowTypeChange, PyArray2, PyArrayLike2};
 use pyo3::{
     exceptions::{PyRuntimeError, PyTypeError, PyValueError},
     prelude::*,
+    types::PyDict,
 };
 
 use crate::{
     executor::Executor,
     pulse::Sampler,
     quant::{Frequency, Time},
     schedule::ElementCommonBuilder,
@@ -31,36 +33,64 @@
 ///
 /// Args:
 ///     base_freq (float): Base frequency of the channel.
 ///     sample_rate (float): Sample rate of the channel.
 ///     length (int): Length of the waveform.
 ///     delay (float): Delay of the channel. Defaults to 0.0.
 ///     align_level (int): Time axis alignment granularity. Defaults to -10.
+///     iq_matrix (array_like[2, 2] | None): IQ matrix of the channel. Defaults
+///         to None.
+///     iq_offset (tuple[float, float]): IQ offset of the channel. Defaults to
+///         (0.0, 0.0).
 #[pyclass(get_all, frozen)]
 #[derive(Debug, Clone)]
 struct Channel {
     base_freq: f64,
     sample_rate: f64,
     length: usize,
     delay: f64,
     align_level: i32,
+    iq_matrix: Option<Py<PyArray2<f64>>>,
+    iq_offset: (f64, f64),
 }
 
 #[pymethods]
 impl Channel {
     #[new]
-    #[pyo3(signature = (base_freq, sample_rate, length, *, delay=0.0, align_level=-10))]
-    fn new(base_freq: f64, sample_rate: f64, length: usize, delay: f64, align_level: i32) -> Self {
-        Channel {
+    #[pyo3(signature = (base_freq, sample_rate, length, *, delay=0.0, align_level=-10, iq_matrix=None, iq_offset=(0.0, 0.0)))]
+    fn new(
+        py: Python<'_>,
+        base_freq: f64,
+        sample_rate: f64,
+        length: usize,
+        delay: f64,
+        align_level: i32,
+        iq_matrix: Option<PyArrayLike2<f64, AllowTypeChange>>,
+        iq_offset: (f64, f64),
+    ) -> PyResult<Self> {
+        let iq_matrix = if let Some(iq_matrix) = iq_matrix {
+            if iq_matrix.shape() != [2, 2] {
+                return Err(PyValueError::new_err("iq_matrix should be a 2x2 matrix"));
+            }
+            let kwargs = PyDict::new_bound(py);
+            kwargs.set_item("write", false)?;
+            iq_matrix.getattr("setflags")?.call((), Some(&kwargs))?;
+            Some(Bound::clone(&iq_matrix).unbind())
+        } else {
+            None
+        };
+        Ok(Channel {
             base_freq,
             sample_rate,
             length,
             delay,
             align_level,
-        }
+            iq_matrix,
+            iq_offset,
+        })
     }
 }
 
 /// Alignment of a schedule element.
 ///
 /// The alignment of a schedule element is used to align the element within its
 /// parent element. The alignment can be one of the following:
@@ -1992,21 +2022,16 @@
     schedule: &Bound<'_, Element>,
     time_tolerance: f64,
     amp_tolerance: f64,
     allow_oversize: bool,
     crosstalk: Option<(PyArrayLike2<'_, f64, AllowTypeChange>, Vec<String>)>,
 ) -> PyResult<HashMap<String, Py<PyArray2<f64>>>> {
     if let Some((crosstalk, names)) = &crosstalk {
-        if crosstalk.ndim() != 2 {
-            return Err(PyValueError::new_err("Crosstalk must be a 2D array."));
-        }
-        if crosstalk.shape()[0] != crosstalk.shape()[1] {
-            return Err(PyValueError::new_err("Crosstalk must be a square matrix."));
-        }
-        if crosstalk.shape()[0] != names.len() {
+        let nl = names.len();
+        if crosstalk.shape() != [nl, nl] {
             return Err(PyValueError::new_err(
                 "The size of the crosstalk matrix must be the same as the number of names.",
             ));
         }
     }
     let root = schedule.downcast::<Element>()?.get().0.clone();
     let measured = schedule::measure(root, f64::INFINITY);
@@ -2027,33 +2052,52 @@
     executor.execute(&arranged);
     let results = executor.into_result();
     let waveforms: HashMap<String, Bound<PyArray2<f64>>> = channels
         .iter()
         .map(|(n, c)| (n.clone(), PyArray2::zeros_bound(py, (2, c.length), false)))
         .collect();
     let mut sampler = Sampler::new(results);
-    for (n, c) in channels {
+    for (n, c) in &channels {
         // SAFETY: These arrays are just created.
-        let array = unsafe { waveforms[&n].as_array_mut() };
+        let array = unsafe { waveforms[n].as_array_mut() };
         sampler.add_channel(
-            n,
+            n.clone(),
             array,
             Frequency::new(c.sample_rate).unwrap(),
             Time::new(c.delay).unwrap(),
             c.align_level,
         );
     }
     if let Some((crosstalk, names)) = &crosstalk {
         sampler.set_crosstalk(crosstalk.as_array(), names.clone());
     }
     sampler.sample(time_tolerance);
     let waveforms = waveforms
         .into_iter()
-        .map(|(n, w)| (n, w.unbind()))
-        .collect();
+        .map(|(n, mut w)| {
+            let c = &channels[&n];
+            if let Some(iq_matrix) = &c.iq_matrix {
+                w = dot_bound(iq_matrix.bind(py), &w)?;
+            }
+            if c.iq_offset.0 != 0.0 || c.iq_offset.1 != 0.0 {
+                let locals = PyDict::new_bound(py);
+                locals.set_item("w", w.clone())?;
+                locals.set_item("offset", pyarray_bound![py, c.iq_offset.0, c.iq_offset.1])?;
+                py.run_bound(
+                    indoc! {"
+                        import numpy as np
+                        w += offset[:, np.newaxis]
+                    "},
+                    None,
+                    Some(&locals),
+                )?;
+            }
+            Ok((n, w.unbind()))
+        })
+        .collect::<PyResult<_>>()?;
     Ok(waveforms)
 }
 
 /// Generates microwave pulses for superconducting quantum computing
 /// experiments.
 ///
 /// .. caution::
```

### Comparing `bosing-2.0.0b7/src/pulse.rs` & `bosing-2.0.0b8/src/pulse.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/quant.rs` & `bosing-2.0.0b8/src/quant.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/schedule/absolute.rs` & `bosing-2.0.0b8/src/schedule/absolute.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/schedule/grid.rs` & `bosing-2.0.0b8/src/schedule/grid.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/schedule/play.rs` & `bosing-2.0.0b8/src/schedule/play.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/schedule/repeat.rs` & `bosing-2.0.0b8/src/schedule/repeat.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/schedule/simple.rs` & `bosing-2.0.0b8/src/schedule/simple.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/schedule/stack.rs` & `bosing-2.0.0b8/src/schedule/stack.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/schedule.rs` & `bosing-2.0.0b8/src/schedule.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/src/shape.rs` & `bosing-2.0.0b8/src/shape.rs`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/tests/test_basic.py` & `bosing-2.0.0b8/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/Cargo.lock` & `bosing-2.0.0b8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -36,22 +36,23 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bosing"
-version = "2.0.0-beta.7"
+version = "2.0.0-beta.8"
 dependencies = [
  "anyhow",
  "bspline",
  "cached",
  "enum_dispatch",
  "float-cmp",
  "hashbrown",
+ "indoc",
  "itertools",
  "ndarray",
  "num",
  "numpy",
  "ordered-float",
  "pyo3",
  "rayon",
```

### Comparing `bosing-2.0.0b7/pyproject.toml` & `bosing-2.0.0b8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bosing-2.0.0b7/PKG-INFO` & `bosing-2.0.0b8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 2.0.0b7
+Version: 2.0.0b8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
```

