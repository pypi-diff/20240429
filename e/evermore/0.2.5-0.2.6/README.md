# Comparing `tmp/evermore-0.2.5.tar.gz` & `tmp/evermore-0.2.6.tar.gz`

## Comparing `evermore-0.2.5.tar` & `evermore-0.2.6.tar`

### file list

```diff
@@ -1,53 +1,56 @@
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 evermore-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 evermore-0.2.5/.readthedocs.yaml
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 evermore-0.2.5/CONTRIBUTING.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 evermore-0.2.5/pixi.toml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 evermore-0.2.5/.github/dependabot.yml
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 evermore-0.2.5/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 evermore-0.2.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0    14463 2020-02-02 00:00:00.000000 evermore-0.2.5/assets/favicon.png
--rw-r--r--   0        0        0    19246 2020-02-02 00:00:00.000000 evermore-0.2.5/assets/logo.png
--rw-r--r--   0        0        0    85492 2020-02-02 00:00:00.000000 evermore-0.2.5/assets/logo_vertical.png
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/Makefile
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/conf.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/getting_started.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/index.md
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/_static/styles_sphinx_book_theme.css
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/api/effect.md
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/api/index.md
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/api/loss.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/api/modifier.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/api/parameter.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/api/pdf.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/api/sample.md
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 evermore-0.2.5/docs/api/util.md
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/bin_by_bin_uncs.py
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/dnn_weights_constraint.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/grad_nll.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/model.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/nll_fit.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/nll_profiling.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/nuisance_parameter.ipynb
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/serialize_model.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 evermore-0.2.5/examples/toy_generation.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/__init__.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/custom_types.py
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/effect.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/loss.py
--rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/modifier.py
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/parameter.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/pdf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/py.typed
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/sample.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/staterror.py
--rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 evermore-0.2.5/src/evermore/util.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 evermore-0.2.5/tests/test_likelihood.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 evermore-0.2.5/tests/test_model.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 evermore-0.2.5/tests/test_parameter.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 evermore-0.2.5/tests/test_pdf.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 evermore-0.2.5/tests/test_util.py
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 evermore-0.2.5/.gitignore
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 evermore-0.2.5/LICENSE
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 evermore-0.2.5/README.md
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 evermore-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 evermore-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 evermore-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 evermore-0.2.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 evermore-0.2.6/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 evermore-0.2.6/pixi.toml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 evermore-0.2.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 evermore-0.2.6/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 evermore-0.2.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    14463 2020-02-02 00:00:00.000000 evermore-0.2.6/assets/favicon.png
+-rw-r--r--   0        0        0    19246 2020-02-02 00:00:00.000000 evermore-0.2.6/assets/logo.png
+-rw-r--r--   0        0        0    85492 2020-02-02 00:00:00.000000 evermore-0.2.6/assets/logo_vertical.png
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/Makefile
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/binned_likelihood.md
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/building_blocks.md
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/conf.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/evermore_for_ATLAS.md
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/evermore_for_CMS.md
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/index.md
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/tips_and_tricks.md
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/_static/styles_sphinx_book_theme.css
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/effect.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/index.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/loss.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/modifier.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/parameter.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/pdf.md
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 evermore-0.2.6/docs/api/util.md
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/bin_by_bin_uncs.py
+-rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/dnn_weights_constraint.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/grad_nll.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/model.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/nll_fit.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/nll_profiling.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/serialize_model.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/toy_generation.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 evermore-0.2.6/examples/unbinned_model.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/__init__.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/custom_types.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/effect.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/loss.py
+-rw-r--r--   0        0        0    12814 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/modifier.py
+-rw-r--r--   0        0        0     9861 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/parameter.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/pdf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/py.typed
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/staterror.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 evermore-0.2.6/src/evermore/util.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_effect.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_loss.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_modifier.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_parameter.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_pdf.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 evermore-0.2.6/tests/test_util.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 evermore-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 evermore-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 evermore-0.2.6/README.md
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 evermore-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 evermore-0.2.6/PKG-INFO
```

### Comparing `evermore-0.2.5/.pre-commit-config.yaml` & `evermore-0.2.6/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -15,21 +15,14 @@
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: name-tests-test
         args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
-  - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v4.0.0-alpha.8"
-    hooks:
-      - id: prettier
-        types_or: [yaml, markdown, html, css, scss, javascript, json]
-        args: [--prose-wrap=always]
-
   - repo: https://github.com/astral-sh/ruff-pre-commit
     rev: "v0.3.3"
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
```

### Comparing `evermore-0.2.5/.readthedocs.yaml` & `evermore-0.2.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/CONTRIBUTING.md` & `evermore-0.2.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/pixi.toml` & `evermore-0.2.6/pixi.toml`

 * *Files 18% similar despite different names*

```diff
@@ -21,13 +21,18 @@
 imageio = "*"
 optimistix = "*"
 flax = "*"
 
 [host-dependencies]
 pip = "*"
 sphinx = "*"
+sphinx-copybutton = "*"
+sphinx-book-theme = "*"
+sphinx-design = "*"
+sphinx-togglebutton = "*"
 
 [tasks]
 postinstall = "pip install -e '.[dev]' && pip install pre-commit && pre-commit install"
 test = "pytest"
 lint = "ruff check . --fix --show-fixes"
 checkall = "pre-commit run --all-files"
+builddocs = "sphinx-build -M html ./docs ./build -W --keep-going"
```

### Comparing `evermore-0.2.5/.github/workflows/cd.yml` & `evermore-0.2.6/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/.github/workflows/ci.yml` & `evermore-0.2.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/assets/favicon.png` & `evermore-0.2.6/assets/favicon.png`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/assets/logo.png` & `evermore-0.2.6/assets/logo.png`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/assets/logo_vertical.png` & `evermore-0.2.6/assets/logo_vertical.png`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/docs/Makefile` & `evermore-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/docs/conf.py` & `evermore-0.2.6/docs/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,26 +38,30 @@
     "use_edit_page_button": True,
 }
 html_context = {"default_mode": "light"}
 html_logo = "../assets/favicon.png"
 html_favicon = "../assets/favicon.png"
 
 extensions = [
+    "myst_parser",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx.ext.autosectionlabel",
-    "myst_parser",
     "sphinx_copybutton",
+    "sphinx_design",
+    "sphinx_togglebutton",
 ]
 
 myst_enable_extensions = [
     "colon_fence",
+    "html_image",
+    "deflist",
 ]
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
 }
 
 nitpick_ignore = [
@@ -66,9 +70,23 @@
 ]
 
 always_document_param_types = True
 
 autodoc_member_order = "bysource"
 
 
+mathjax3_config = {
+    "tex2jax": {"inlineMath": [["$", "$"], ["\\(", "\\)"]]},
+    "tex": {
+        "macros": {
+            "bm": ["\\boldsymbol{#1}", 1],  # \usepackage{bm}, see mathjax/MathJax#1219
+            "pyhf": r"\texttt{pyhf}",
+            "Combine": r"\texttt{Combine}",
+            "JAX": r"\texttt{JAX}",
+            "PyTree": r"\texttt{PyTree}",
+        }
+    },
+}
+
+
 def setup(app):
     app.add_css_file("styles_sphinx_book_theme.css")
```

### Comparing `evermore-0.2.5/examples/bin_by_bin_uncs.py` & `evermore-0.2.6/examples/bin_by_bin_uncs.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from operator import itemgetter
+
 import equinox as eqx
 import jax.numpy as jnp
 from jaxtyping import Array
 
 import evermore as evm
 
 
@@ -16,23 +18,23 @@
             hists=hists, histsw2=histsw2, threshold=10.0
         )
 
     def __call__(self, hists: dict) -> dict[str, Array]:
         expectations = {}
 
         # signal process
-        signal_mcstat_mod = self.staterrors.get(where=lambda p: p["signal"])
+        signal_mcstat_mod = self.staterrors.modifier(getter=lambda p: p["signal"])
         expectations["signal"] = signal_mcstat_mod(hists["signal"])
 
         # bkg1 process
-        bkg1_mcstat_mod = self.staterrors.get(where=lambda p: p["bkg1"])
+        bkg1_mcstat_mod = self.staterrors.modifier(getter=lambda p: p["bkg1"])
         expectations["bkg1"] = bkg1_mcstat_mod(hists["bkg1"])
 
         # bkg2 process
-        bkg2_mcstat_mod = self.staterrors.get(where=lambda p: p["bkg2"])
+        bkg2_mcstat_mod = self.staterrors.modifier(getter=lambda p: p["bkg2"])
         expectations["bkg2"] = bkg2_mcstat_mod(hists["bkg2"])
 
         # return the modified expectations
         return expectations
 
 
 hists = {
@@ -54,14 +56,10 @@
 
 # scale the histsw2 e.g. after minimization with
 # the best fit values of the staterror modifiers.
 # This is needed to get the correct stat. uncertainties
 modified_histsw2 = {}
 
 
-def where(process):
-    return lambda x: x[process]
-
-
 for process, histw2 in histsw2.items():
-    mod = model.staterrors.get(where=where(process))
+    mod = model.staterrors.modifier(getter=itemgetter(process))
     modified_histsw2[process] = mod(histw2)
```

### Comparing `evermore-0.2.5/examples/dnn_weights_constraint.py` & `evermore-0.2.6/examples/dnn_weights_constraint.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             mean=jnp.zeros((out_size, in_size)),
             width=jnp.full((out_size, in_size), 0.5),
         )
         self.weights = evm.Parameter(
             value=jax.random.normal(wkey, (out_size, in_size)),
             lower=-jnp.inf,
             upper=jnp.inf,
-            constraint=normal,
+            prior=normal,
         )
 
         # biases
         self.biases = jax.random.normal(bkey, (out_size,))
 
     def __call__(self, x: jax.Array):
         return self.weights.value @ x + self.biases
@@ -33,15 +33,15 @@
 @eqx.filter_jit
 def loss_fn(model, x, y):
     pred_y = jax.vmap(model)(x)
     mse = jax.numpy.mean((y - pred_y) ** 2)
     constraints = evm.loss.get_log_probs(model)
     # sum them all up for each weight
     constraints = jax.tree_util.tree_map(jnp.sum, constraints)
-    return mse + evm.util.sum_leaves(constraints)
+    return mse + evm.util.sum_over_leaves(constraints)
 
 
 batch_size, in_size, out_size = 32, 2, 3
 model = LinearConstrained(in_size, out_size, key=jax.random.PRNGKey(0))
 x = jax.numpy.zeros((batch_size, in_size))
 y = jax.numpy.zeros((batch_size, out_size))
 loss_val = loss_fn(model, x, y)
```

### Comparing `evermore-0.2.5/examples/grad_nll.py` & `evermore-0.2.6/examples/grad_nll.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import equinox as eqx
 import jax.numpy as jnp
 from model import hists, model, observation
 
 import evermore as evm
 
-nll = evm.loss.PoissonNLL()
+log_likelihood = evm.loss.PoissonLogLikelihood()
 
 
 @eqx.filter_jit
 def loss(model, hists, observation):
     expectations = model(hists)
     constraints = evm.loss.get_log_probs(model)
-    loss_val = nll(
-        expectation=evm.util.sum_leaves(expectations),
+    loss_val = log_likelihood(
+        expectation=evm.util.sum_over_leaves(expectations),
         observation=observation,
     )
     # add constraint
-    loss_val += evm.util.sum_leaves(constraints)
+    loss_val += evm.util.sum_over_leaves(constraints)
     return -jnp.sum(loss_val)
 
 
 loss_val = loss(model, hists, observation)
 grads = eqx.filter_grad(loss)(model, hists, observation)
```

### Comparing `evermore-0.2.5/examples/model.py` & `evermore-0.2.6/examples/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from __future__ import annotations
 
 import equinox as eqx
 import jax.numpy as jnp
-from jaxtyping import Array
+from jaxtyping import Array, PyTree
 
 import evermore as evm
 
 
 class SPlusBModel(eqx.Module):
-    mu: evm.FreeFloating
-    norm1: evm.NormalConstrained
-    norm2: evm.NormalConstrained
-    shape1: evm.NormalConstrained
+    mu: evm.Parameter
+    norm1: evm.NormalParameter
+    norm2: evm.NormalParameter
+    shape1: evm.NormalParameter
 
-    def __init__(self, hist: dict[str, Array], histw2: dict[str, Array]) -> None:
-        self = evm.parameter.auto_init(self)
+    def __init__(self, hist: PyTree, histw2: PyTree) -> None:
+        evm.util.dataclass_auto_init(self)
 
     def __call__(self, hists: dict) -> dict[str, Array]:
         expectations = {}
 
         # signal process
-        sig_mod = self.mu.unconstrained()
+        sig_mod = self.mu.scale()
         expectations["signal"] = sig_mod(hists["nominal"]["signal"])
 
         # bkg1 process
-        bkg1_lnN = self.norm1.log_normal(up=jnp.array([1.1]), down=jnp.array([0.9]))
-        bkg1_shape = self.shape1.shape(
-            up=hists["shape_up"]["bkg1"],
-            down=hists["shape_down"]["bkg1"],
+        bkg1_lnN = self.norm1.scale_log(up=jnp.array([1.1]), down=jnp.array([0.9]))
+        bkg1_shape = self.shape1.morphing(
+            up_template=hists["shape_up"]["bkg1"],
+            down_template=hists["shape_down"]["bkg1"],
         )
         # combine modifiers
         bkg1_mod = bkg1_lnN @ bkg1_shape
         expectations["bkg1"] = bkg1_mod(hists["nominal"]["bkg1"])
 
         # bkg2 process
-        bkg2_lnN = self.norm2.log_normal(up=jnp.array([1.05]), down=jnp.array([0.95]))
-        bkg2_shape = self.shape1.shape(
-            up=hists["shape_up"]["bkg2"],
-            down=hists["shape_down"]["bkg2"],
+        bkg2_lnN = self.norm2.scale_log(up=jnp.array([1.05]), down=jnp.array([0.95]))
+        bkg2_shape = self.shape1.morphing(
+            up_template=hists["shape_up"]["bkg2"],
+            down_template=hists["shape_down"]["bkg2"],
         )
         # combine modifiers
         bkg2_mod = bkg2_lnN @ bkg2_shape
         expectations["bkg2"] = bkg2_mod(hists["nominal"]["bkg2"])
 
         # return the modified expectations
         return expectations
```

### Comparing `evermore-0.2.5/examples/nll_fit.py` & `evermore-0.2.6/examples/nll_fit.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,44 +5,51 @@
 from model import hists, model, observation
 
 import evermore as evm
 
 optim = optax.sgd(learning_rate=1e-2)
 opt_state = optim.init(eqx.filter(model, eqx.is_inexact_array))
 
-nll = evm.loss.PoissonNLL()
+log_likelihood = evm.loss.PoissonLogLikelihood()
 
 
 @eqx.filter_jit
-def loss(model, hists, observation):
+def loss(dynamic_model, static_model, hists, observation):
+    model = eqx.combine(dynamic_model, static_model)
     expectations = model(hists)
     constraints = evm.loss.get_log_probs(model)
-    loss_val = nll(
-        expectation=evm.util.sum_leaves(expectations),
+    loss_val = log_likelihood(
+        expectation=evm.util.sum_over_leaves(expectations),
         observation=observation,
     )
     # add constraint
-    loss_val += evm.util.sum_leaves(constraints)
+    loss_val += evm.util.sum_over_leaves(constraints)
     return -jnp.sum(loss_val)
 
 
 @eqx.filter_jit
 def make_step(model, opt_state, events, observation):
     # differentiate full analysis
-    grads = eqx.filter_grad(loss)(model, events, observation)
+    dynamic_model, static_model = eqx.partition(
+        model, evm.parameter.value_filter_spec(model)
+    )
+    grads = eqx.filter_grad(loss)(dynamic_model, static_model, events, observation)
     updates, opt_state = optim.update(grads, opt_state)
     # apply nuisance parameter and DNN weight updates
     model = eqx.apply_updates(model, updates)
     return model, opt_state
 
 
 # minimize model with 1000 steps
 for step in range(1000):
     if step % 100 == 0:
-        loss_val = loss(model, hists, observation)
+        dynamic_model, static_model = eqx.partition(
+            model, evm.parameter.value_filter_spec(model)
+        )
+        loss_val = loss(dynamic_model, static_model, hists, observation)
         print(f"{step=} - {loss_val=:.6f}")
     model, opt_state = make_step(model, opt_state, hists, observation)
 
 
 # For low overhead it is recommended to use jax.lax.fori_loop.
 # In case you want to jit the for loop, you can use the following function,
 # this will prevent jax from unrolling the loop and creating a huge graph
```

### Comparing `evermore-0.2.5/examples/nll_profiling.py` & `evermore-0.2.6/examples/nll_profiling.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,63 @@
 import equinox as eqx
 import jax
 import jax.numpy as jnp
-import jax.tree_util as jtu
 import optax
 from jaxtyping import Array
 
 import evermore as evm
 
 
 def fixed_mu_fit(mu: Array) -> Array:
     from model import hists, model, observation
 
-    nll = evm.loss.PoissonNLL()
+    log_likelihood = evm.loss.PoissonLogLikelihood()
 
     optim = optax.sgd(learning_rate=1e-2)
     opt_state = optim.init(eqx.filter(model, eqx.is_inexact_array))
 
     model = eqx.tree_at(lambda t: t.mu.value, model, mu)
 
     # filter out mu from the model (no gradients will be calculated for mu!)
     # see: https://github.com/patrick-kidger/equinox/blob/main/examples/frozen_layer.ipynb
-    filter_spec = jtu.tree_map(lambda _: True, model)
+    filter_spec = evm.parameter.value_filter_spec(model)
     filter_spec = eqx.tree_at(
         lambda tree: tree.mu.value,
         filter_spec,
         replace=False,
     )
 
     @eqx.filter_jit
-    def loss(diff_model, static_model, hists, observation):
-        model = eqx.combine(diff_model, static_model)
+    def loss(dynamic_model, static_model, hists, observation):
+        model = eqx.combine(dynamic_model, static_model)
         expectations = model(hists)
         constraints = evm.loss.get_log_probs(model)
-        loss_val = nll(
-            expectation=evm.util.sum_leaves(expectations),
+        loss_val = log_likelihood(
+            expectation=evm.util.sum_over_leaves(expectations),
             observation=observation,
         )
         # add constraint
-        loss_val += evm.util.sum_leaves(constraints)
+        loss_val += evm.util.sum_over_leaves(constraints)
         return -2 * jnp.sum(loss_val)
 
     @eqx.filter_jit
-    def make_step(model, opt_state, events, observation):
+    def make_step(model, opt_state, hists, observation):
         # differentiate
-        diff_model, static_model = eqx.partition(model, filter_spec)
-        grads = eqx.filter_grad(loss)(diff_model, static_model, events, observation)
+        dynamic_model, static_model = eqx.partition(model, filter_spec)
+        grads = eqx.filter_grad(loss)(dynamic_model, static_model, hists, observation)
         updates, opt_state = optim.update(grads, opt_state)
         # apply nuisance parameter and DNN weight updates
         model = eqx.apply_updates(model, updates)
         return model, opt_state
 
     # minimize model with 1000 steps
     for _ in range(1000):
         model, opt_state = make_step(model, opt_state, hists, observation)
-    diff_model, static_model = eqx.partition(model, filter_spec)
-    return loss(diff_model, static_model, hists, observation)
+    dynamic_model, static_model = eqx.partition(model, filter_spec)
+    return loss(dynamic_model, static_model, hists, observation)
 
 
 mus = jnp.linspace(0, 5, 11)
 # for loop over mu values
 for mu in mus:
     print(f"[for-loop] mu={mu:.2f} - NLL={fixed_mu_fit(jnp.array(mu)):.6f}")
```

### Comparing `evermore-0.2.5/examples/toy_generation.py` & `evermore-0.2.6/examples/toy_generation.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 from model import hists, model, observation
 
 import evermore as evm
 
 key = jax.random.PRNGKey(0)
 
 # generate a new model with sampled parameters according to their constraint pdfs
-toymodel = evm.sample.sample_parameters(model, key)
+toymodel = evm.parameter.sample(model, key)
 
 
 # generate new expectation based on the toy model
 def toy_expectation(
     key: PRNGKeyArray,
     module: eqx.Module,
     hists: dict,
 ) -> Array:
-    toymodel = evm.sample.sample_parameters(model, key)
+    toymodel = evm.parameter.sample(model, key)
     expectations = toymodel(hists)
-    return evm.util.sum_leaves(expectations)
+    return evm.util.sum_over_leaves(expectations)
 
 
 expectation = toy_expectation(key, model, hists)
 
 
 # generate a new expectations vectorized over many keys
 keys = jax.random.split(key, 1000)
```

### Comparing `evermore-0.2.5/src/evermore/__init__.py` & `evermore-0.2.6/src/evermore/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,53 +7,46 @@
 __author__ = "Peter Fackeldey"
 __email__ = "peter.fackeldey@rwth-aachen.de"
 __copyright__ = "Copyright 2023, Peter Fackeldey"
 __credits__ = ["Peter Fackeldey"]
 __contact__ = "https://github.com/pfackeldey/evermore"
 __license__ = "BSD-3-Clause"
 __status__ = "Development"
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 
 # expose public API
 
 __all__ = [
     "__version__",
     "effect",
     "loss",
     "parameter",
     "pdf",
     "util",
-    "sample",
     "modifier",
     "staterror",
     # explicitely expose some classes
     "Parameter",
-    "FreeFloating",
-    "NormalConstrained",
-    "PoissonConstrained",
+    "NormalParameter",
     "Modifier",
-    "ModifierBase",
 ]
 
 
 def __dir__():
     return __all__
 
 
 from evermore import (  # noqa: E402
     effect,
     loss,
     modifier,
     parameter,
     pdf,
-    sample,
     staterror,
     util,
 )
-from evermore.modifier import Modifier, ModifierBase  # noqa: E402
-from evermore.parameter import (  # noqa: E402
-    FreeFloating,
-    NormalConstrained,
+from evermore.modifier import Modifier  # noqa: E402
+from evermore.parameter import (  # noqa: E402,
+    NormalParameter,
     Parameter,
-    PoissonConstrained,
 )
```

### Comparing `evermore-0.2.5/src/evermore/loss.py` & `evermore-0.2.6/src/evermore/loss.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,69 +3,68 @@
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from jaxtyping import Array, PyTree
 
 from evermore.custom_types import PDFLike
-from evermore.parameter import Parameter
-from evermore.util import _params_map
+from evermore.parameter import Parameter, params_map
 
 __all__ = [
     "get_log_probs",
     "get_boundary_constraints",
-    "PoissonNLL",
+    "PoissonLogLikelihood",
 ]
 
 
 def __dir__():
     return __all__
 
 
 def get_log_probs(module: PyTree) -> PyTree:
     def _constraint(param: Parameter) -> Array:
-        constraint = param.constraint
-        if isinstance(constraint, PDFLike):
-            constraint = cast(PDFLike, constraint)
-            return constraint.log_prob(param.value)
+        prior = param.prior
+        if isinstance(prior, PDFLike):
+            prior = cast(PDFLike, prior)
+            return prior.log_prob(param.value)
         return jnp.array([0.0])
 
     # constraints from pdfs
-    return _params_map(_constraint, module)
+    return params_map(_constraint, module)
 
 
 def get_boundary_constraints(module: PyTree) -> PyTree:
-    return _params_map(lambda p: p.boundary_constraint, module)
+    return params_map(lambda p: p.boundary_constraint, module)
 
 
-class PoissonNLL(eqx.Module):
+class PoissonLogLikelihood(eqx.Module):
     """
-    Poisson negative log-likelihood (NLL).
+    Poisson log-likelihood.
 
     Usage:
 
-        .. code-block:: python
+    .. code-block:: python
 
-            import evermore as evm
+        import evermore as evm
 
-            nll = evm.loss.PoissonNLL()
+        nll = evm.loss.PoissonLogLikelihood()
 
-            def loss(model, x, y):
-                expectation = model(x)
-                loss = nll(expectation, y)
-                constraints = evm.loss.get_log_probs(model)
-                loss += evm.util.sum_leaves(constraints))
-                return -jnp.sum(loss)
+        def loss(model, x, y):
+            expectation = model(x)
+            loss = nll(expectation, y)
+            constraints = evm.loss.get_log_probs(model)
+            loss += evm.util.sum_over_leaves(constraints)
+            return -jnp.sum(loss)
     """
 
     @property
-    def logpdf(self) -> Callable:
+    def log_prob(self) -> Callable:
         return jax.scipy.stats.poisson.logpmf
 
-    @jax.named_scope("evm.loss.PoissonNLL")
+    @jax.named_scope("evm.loss.PoissonLogLikelihood")
     def __call__(self, expectation: Array, observation: Array) -> Array:
         # poisson log-likelihood
         return jnp.sum(
-            self.logpdf(observation, expectation)
-            - self.logpdf(observation, observation),
+            self.log_prob(observation, expectation)
+            - self.log_prob(observation, observation),
             axis=-1,
         )
```

### Comparing `evermore-0.2.5/src/evermore/modifier.py` & `evermore-0.2.6/src/evermore/modifier.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,100 +5,102 @@
 from functools import partial
 from typing import TYPE_CHECKING
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
-from jaxtyping import Array
+from jaxtyping import Array, ArrayLike, PyTree
 
-from evermore.custom_types import SF, ModifierLike
+from evermore.custom_types import ModifierLike, OffsetAndScale
 from evermore.effect import DEFAULT_EFFECT
 from evermore.parameter import Parameter
 from evermore.util import tree_stack
 
 if TYPE_CHECKING:
     from evermore.effect import Effect
 
 __all__ = [
     "ModifierBase",
     "Modifier",
-    "compose",
-    "where",
-    "mask",
-    "transform",
+    "Compose",
+    "Where",
+    "BooleanMask",
+    "Transform",
+    "TransformOffset",
+    "TransformScale",
 ]
 
 
 def __dir__():
     return __all__
 
 
 class AbstractModifier(eqx.Module):
     @abc.abstractmethod
-    def scale_factor(self: ModifierLike, hist: Array) -> SF: ...
+    def offset_and_scale(self: ModifierLike, hist: Array) -> OffsetAndScale: ...
 
     @abc.abstractmethod
     def __call__(self: ModifierLike, hist: Array) -> Array: ...
 
     @abc.abstractmethod
-    def __matmul__(self: ModifierLike, other: ModifierLike) -> compose: ...
+    def __matmul__(self: ModifierLike, other: ModifierLike) -> Compose: ...
 
 
 class ApplyFn(eqx.Module):
     @jax.named_scope("evm.modifier.ApplyFn")
     def __call__(self: ModifierLike, hist: Array) -> Array:
-        sf = self.scale_factor(hist=hist)
-        # apply
-        return sf.multiplicative * (hist + sf.additive)
+        os = self.offset_and_scale(hist=hist)
+        return os.scale * (hist + os.offset)
 
 
 class MatMulCompose(eqx.Module):
-    def __matmul__(self: ModifierLike, other: ModifierLike) -> compose:
-        return compose(self, other)
+    def __matmul__(self: ModifierLike, other: ModifierLike) -> Compose:
+        return Compose(self, other)
 
 
 class ModifierBase(ApplyFn, MatMulCompose, AbstractModifier):
     """
     This serves as a base class for all modifiers.
     It automatically implements the __call__ method to apply the scale factors to the hist array
     and the __matmul__ method to compose two modifiers.
 
     Custom modifiers should inherit from this class and implement the scale_factor method.
 
     Example:
 
-        .. code-block:: python
+    .. code-block:: python
 
-            import equinox as eqx
-            import jax.numpy as jnp
-            import jax.tree_util as jtu
-            from jaxtyping import Array
+        import equinox as eqx
+        import jax.numpy as jnp
+        import jax.tree_util as jtu
+        from jaxtyping import Array
+
+        import evermore as evm
 
-            import evermore as evm
 
-            class clip(evm.ModifierBase):
-                modifier: evm.ModifierBase
-                min_sf: float = eqx.field(static=True)
-                max_sf: float = eqx.field(static=True)
+        class Clip(evm.modifier.ModifierBase):
+            modifier: evm.custom_types.ModifierLike
+            min_sf: float = eqx.field(static=True)
+            max_sf: float = eqx.field(static=True)
 
-                def scale_factor(self, hist: Array) -> evm.custrom_types.SF:
-                    sf = self.modifier.scale_factor(hist)
-                    return jtu.tree_map(lambda x: jnp.clip(x, self.min_sf, self.max_sf), sf)
+            def offset_and_scale(self, hist: Array) -> evm.custom_types.OffsetAndScale:
+                os = self.modifier.offset_and_scale(hist)
+                return jtu.tree_map(lambda x: jnp.clip(x, self.min_sf, self.max_sf), os)
 
 
-            parameter = evm.Parameter(value=1.1)
-            modifier = parameter.unconstrained()
+        parameter = evm.Parameter(value=1.1)
+        modifier = parameter.scale()
 
-            clipped_modifier = clip(modifier=modifier, min_sf=0.8, max_sf=1.2)
+        clipped_modifier = Clip(modifier=modifier, min_sf=0.8, max_sf=1.2)
 
-            # this example is trivial, because you can also implement it with `evm.modifier.transform`:
-            from functools import partial
+        # this example is trivial, because you can also implement it with *evm.modifier.Transform*:
+        from functools import partial
 
-            clipped_modifier = evm.modifier.transform(partial(jnp.clip, a_min=0.8, a_max=1.2), modifier)
+        clipped_modifier = evm.modifier.Transform(partial(jnp.clip, a_min=0.8, a_max=1.2), modifier)
     """
 
 
 class Modifier(ModifierBase):
     """
     Create a new modifier for a given parameter and penalty.
 
@@ -106,220 +108,241 @@
 
     .. code-block:: python
 
         import jax.numpy as jnp
         import evermore as evm
 
         mu = evm.Parameter(value=1.1)
-        norm = evm.Parameter(value=0.0)
+        norm = evm.NormalParameter(value=0.0)
 
         # create a new parameter and a penalty
-        modify = evm.Modifier(parameter=mu, effect=evm.effect.unconstrained())
+        modify = evm.Modifier(parameter=mu, effect=evm.effect.Linear(offset=0, slope=1))
         # or shorthand
-        modify = mu.unconstrained()
+        modify = mu.scale(offset=0, slope=1)
 
         # apply the Modifier
         modify(jnp.array([10, 20, 30]))
         # -> Array([11., 22., 33.], dtype=float32, weak_type=True),
 
         # log_normal effect
-        modify = evm.Modifier(parameter=norm, effect=evm.effect.log_normal(jnp.array([0.8, 1.2])))
+        modify = evm.Modifier(parameter=norm, effect=evm.effect.AsymmetricExponential(up=1.2, down=0.8))
         # or shorthand
-        modify = norm.log_normal(jnp.array([0.8, 1.2]))
+        modify = norm.scale_log(up=1.2, down=0.8)
 
         # poisson effect
         hist = jnp.array([10, 20, 30])
-        modify = evm.Modifier(parameter=norm, effect=evm.effect.poisson(hist))
+        parameter = evm.Parameter(value=1.0, prior=evm.pdf.Poisson(lamb=hist))
+        modify = evm.Modifier(parameter=parameter, effect=evm.effect.Linear(offset=1, slope=1))
         # or shorthand
-        modify = norm.poisson(hist)
+        modify = norm.scale(offset=1, slope=1)
 
         # shape effect
-        up = jnp.array([12, 23, 35])
-        down = jnp.array([8, 19, 26])
-        modify = evm.Modifier(parameter=norm, effect=evm.effect.shape(up, down))
+        up_template = jnp.array([12, 23, 35])
+        down_template = jnp.array([8, 19, 26])
+        modify = evm.Modifier(parameter=norm, effect=evm.effect.VerticalTemplateMorphing(up_template=up_template, down_template=down_template))
         # or shorthand
-        modify = norm.shape(up, down)
+        modify = norm.morphing(up_template=up_template, down_template=down_template)
     """
 
-    parameter: Parameter
+    parameter: PyTree[Parameter]
     effect: Effect
 
-    def __init__(self, parameter: Parameter, effect: Effect = DEFAULT_EFFECT) -> None:
+    def __init__(
+        self, parameter: PyTree[Parameter], effect: Effect = DEFAULT_EFFECT
+    ) -> None:
         self.parameter = parameter
         self.effect = effect
 
-    def scale_factor(self, hist: Array) -> SF:
-        return self.effect.scale_factor(parameter=self.parameter, hist=hist)
+    def offset_and_scale(self, hist: Array) -> OffsetAndScale:
+        return self.effect(parameter=self.parameter, hist=hist)
 
 
-class where(ModifierBase):
+class Where(ModifierBase):
     """
     Combine two modifiers based on a condition.
 
     The condition is a boolean array, and the two modifiers are applied to the data based on the condition.
 
     Example:
 
-        .. code-block:: python
+    .. code-block:: python
 
-            import jax.numpy as jnp
-            import evermore as evm
+        import jax.numpy as jnp
+        import evermore as evm
 
-            hist = jnp.array([5, 20, 30])
-            syst = evm.Parameter(value=0.1)
+        hist = jnp.array([5, 20, 30])
+        syst = evm.NormalParameter(value=0.1)
 
-            norm = syst.log_normal(up=jnp.array([1.1]), down=jnp.array([0.9]))
-            shape = syst.shape(up=jnp.array([7, 22, 31]), down=jnp.array([4, 16, 27]))
+        norm = syst.scale_log(up=jnp.array([1.1]), down=jnp.array([0.9]))
+        shape = syst.morphing(up_template=jnp.array([7, 22, 31]), down_template=jnp.array([4, 16, 27]))
 
-            # apply norm if hist < 10, else apply shape
-            modifier = evm.modifier.where(hist < 10, norm, shape)
+        # apply norm if hist < 10, else apply shape
+        modifier = evm.modifier.Where(hist < 10, norm, shape)
 
-            # apply
-            modifier(hist)
-            # -> Array([ 5.049494, 20.281374, 30.181376], dtype=float32)
+        # apply
+        modifier(hist)
+        # -> Array([ 5.049494, 20.281374, 30.181376], dtype=float32)
 
-            # for comparison:
-            norm(hist)
-            # -> Array([ 5.049494, 20.197975, 30.296963], dtype=float32)
-            shape(hist)
-            # -> Array([ 5.1593127, 20.281374 , 30.181376 ], dtype=float32)
+        # for comparison:
+        norm(hist)
+        # -> Array([ 5.049494, 20.197975, 30.296963], dtype=float32)
+        shape(hist)
+        # -> Array([ 5.1593127, 20.281374 , 30.181376 ], dtype=float32)
     """
 
     condition: Array
-    modifier_true: Modifier
-    modifier_false: Modifier
+    modifier_true: ModifierLike
+    modifier_false: ModifierLike
 
-    def scale_factor(self, hist: Array) -> SF:
-        true_sf = self.modifier_true.scale_factor(hist)
-        false_sf = self.modifier_false.scale_factor(hist)
+    def offset_and_scale(self, hist: Array) -> OffsetAndScale:
+        true_os = self.modifier_true.offset_and_scale(hist)
+        false_os = self.modifier_false.offset_and_scale(hist)
 
         def _where(true: Array, false: Array) -> Array:
             return jnp.where(self.condition, true, false)
 
-        return jtu.tree_map(_where, true_sf, false_sf)
+        return jtu.tree_map(_where, true_os, false_os)
 
 
-class mask(ModifierBase):
+class BooleanMask(ModifierBase):
     """
     Mask a modifier for specific bins.
 
     The mask is a boolean array (True, False for each bin).
     The modifier is only applied to the bins where the mask is True.
 
     Example:
 
-        .. code-block:: python
+    .. code-block:: python
 
-            import jax.numpy as jnp
-            import evermore as evm
+        import jax.numpy as jnp
+        import evermore as evm
 
-            hist = jnp.array([5, 20, 30])
-            syst = evm.Parameter(value=0.1)
+        hist = jnp.array([5, 20, 30])
+        syst = evm.NormalParameter(value=0.1)
 
-            norm = syst.log_normal(jnp.array([0.9, 1.1]))
-            mask = jnp.array([True, False, True])
+        norm = syst.scale_log(up=1.1, down=0.9)
+        mask = jnp.array([True, False, True])
 
-            modifier = evm.modifier.mask(mask, norm)
+        modifier = evm.modifier.BooleanMask(mask, norm)
 
-            # apply
-            modifier(hist)
-            # -> Array([ 5.049494, 20.      , 30.296963], dtype=float32)
+        # apply
+        modifier(hist)
+        # -> Array([ 5.049494, 20.      , 30.296963], dtype=float32)
     """
 
-    where: Array
-    modifier: Modifier
+    mask: Array
+    modifier: ModifierLike
 
-    def scale_factor(self, hist: Array) -> SF:
-        sf = self.modifier.scale_factor(hist)
+    def offset_and_scale(self, hist: Array) -> OffsetAndScale:
+        os = self.modifier.offset_and_scale(hist)
 
-        def _mask(true: Array, false: Array) -> Array:
-            return jnp.where(self.where, true, false)
+        def _mask(true: ArrayLike, false: ArrayLike) -> Array:
+            return jnp.where(self.mask, true, false)
 
-        return SF(
-            multiplicative=_mask(sf.multiplicative, jnp.ones_like(hist)),
-            additive=_mask(sf.additive, jnp.zeros_like(hist)),
+        return OffsetAndScale(
+            offset=_mask(os.offset, 0.0),
+            scale=_mask(os.scale, 1.0),
         )
 
 
-class transform(ModifierBase):
+class Transform(ModifierBase):
     """
     Transform the scale factors of a modifier.
 
     The `transform_fn` is a function that is applied to both, multiplicative and additive scale factors.
 
     Example:
 
-        .. code-block:: python
+    .. code-block:: python
 
-            import jax.numpy as jnp
-            import evermore as evm
+        import jax.numpy as jnp
+        import evermore as evm
 
-            hist = jnp.array([5, 20, 30])
-            syst = evm.Parameter(value=0.1)
+        hist = jnp.array([5, 20, 30])
+        syst = evm.NormalParameter(value=0.1)
 
-            norm = syst.log_normal(jnp.array([0.9, 1.1]))
+        norm = syst.scale_log(up=1.1, down=0.9)
 
-            transformed_norm = evm.modifier.transform(jnp.sqrt, norm)
+        transformed_norm = evm.modifier.Transform(jnp.sqrt, norm)
 
-            # apply
-            transformed_norm(hist)
-            # -> Array([ 5.024686, 20.098743, 30.148115], dtype=float32)
+        # apply
+        transformed_norm(hist)
+        # -> Array([ 5.024686, 20.098743, 30.148115], dtype=float32)
 
-            # for comparison:
-            norm(hist)
-            # -> Array([ 5.049494, 20.197975, 30.296963], dtype=float32)
+        # for comparison:
+        norm(hist)
+        # -> Array([ 5.049494, 20.197975, 30.296963], dtype=float32)
     """
 
     transform_fn: Callable = eqx.field(static=True)
-    modifier: Modifier
+    modifier: ModifierLike
+
+    def offset_and_scale(self, hist: Array) -> OffsetAndScale:
+        os = self.modifier.offset_and_scale(hist)
+        return jtu.tree_map(self.transform_fn, os)
+
+
+class TransformOffset(ModifierBase):
+    transform_fn: Callable = eqx.field(static=True)
+    modifier: ModifierLike
+
+    def offset_and_scale(self, hist: Array) -> OffsetAndScale:
+        os = self.modifier.offset_and_scale(hist)
+        return OffsetAndScale(offset=self.transform_fn(os.offset), scale=os.scale)
+
+
+class TransformScale(ModifierBase):
+    transform_fn: Callable = eqx.field(static=True)
+    modifier: ModifierLike
 
-    def scale_factor(self, hist: Array) -> SF:
-        sf = self.modifier.scale_factor(hist)
-        return jtu.tree_map(self.transform_fn, sf)
+    def offset_and_scale(self, hist: Array) -> OffsetAndScale:
+        os = self.modifier.offset_and_scale(hist)
+        return OffsetAndScale(offset=os.offset, scale=self.transform_fn(os.scale))
 
 
-class compose(ModifierBase):
+class Compose(ModifierBase):
     """
-    Composition of multiple modifiers, i.e.: `(f ∘ g ∘ h)(hist) = f(hist) * g(hist) * h(hist)`
+    Composition of multiple modifiers, in order to correctly apply them *together*.
     It behaves like a single modifier, but it is composed of multiple modifiers; it can be arbitrarly nested.
 
     Example:
 
     .. code-block:: python
 
         import jax.numpy as jnp
         import evermore as evm
 
         mu = evm.Parameter(value=1.1)
-        sigma = evm.Parameter(value=0.1)
-        sigma2 = evm.Parameter(value=0.2)
+        sigma = evm.NormalParameter(value=0.1)
+        sigma2 = evm.NormalParameter(value=0.2)
 
         hist = jnp.array([10, 20, 30])
 
         # all bins with bin content below 10 (threshold) are treated as poisson, else normal
 
         # create a new parameter and a composition of modifiers
-        mu_mod = mu.unconstrained()
-        sigma_mod = sigma.log_normal(up=jnp.array([1.1]), down=jnp.array([0.9]))
-        sigma2_mod = sigma2.log_normal(up=jnp.array([1.05]), down=jnp.array([0.95]))
-        composition = evm.modifier.compose(
+        mu_mod = mu.scale(offset=0, slope=1)
+        sigma_mod = sigma.scale_log(up=1.1, down=0.9)
+        sigma2_mod = sigma2.scale_log(up=1.05, down=0.95)
+        composition = evm.modifier.Compose(
             mu_mod,
             sigma_mod,
-            evm.modifier.where(hist < 15, sigma2_mod, sigma_mod),
+            evm.modifier.Where(hist < 15, sigma2_mod, sigma_mod),
         )
         # or shorthand
-        composition = mu_mod @ sigma_mod @ evm.modifier.where(hist < 15, sigma2_mod, sigma_mod)
+        composition = mu_mod @ sigma_mod @ evm.modifier.Where(hist < 15, sigma2_mod, sigma_mod)
 
         # apply the composition
         composition(hist)
 
         # nest compositions
-        composition = evm.modifier.compose(
+        composition = evm.modifier.Compose(
             composition,
-            evm.Modifier(parameter=sigma, effect=evm.effect.log_normal(up=jnp.array([1.2]), down=jnp.array([0.8]))),
+            evm.Modifier(parameter=sigma, effect=evm.effect.AsymmetricExponential(up=1.2, down=0.8)),
         )
 
         # jit
         import equinox as eqx
 
         eqx.filter_jit(composition)(hist)
     """
@@ -327,30 +350,31 @@
     modifiers: list[ModifierLike]
 
     def __init__(self, *modifiers: ModifierLike) -> None:
         self.modifiers = list(modifiers)
         # unroll nested compositions
         _modifiers = []
         for mod in self.modifiers:
-            if isinstance(mod, compose):
+            if isinstance(mod, Compose):
                 _modifiers.extend(mod.modifiers)
             else:
                 assert isinstance(mod, ModifierBase)
                 _modifiers.append(mod)
-        # by now all modifiers are either modifier or staterror
+        # by now all are modifiers
         self.modifiers = _modifiers
 
     def __len__(self) -> int:
         return len(self.modifiers)
 
-    def scale_factor(self, hist: Array) -> SF:
+    def offset_and_scale(self, hist: Array) -> OffsetAndScale:
         from collections import defaultdict
 
-        multiplicative_sf = jnp.ones_like(hist)
-        additive_sf = jnp.zeros_like(hist)
+        # initial scale and offset
+        scale = jnp.ones_like(hist)
+        offset = jnp.zeros_like(hist)
 
         groups = defaultdict(list)
         # first group modifiers into same tree structures
         for mod in self.modifiers:
             groups[hash(jtu.tree_structure(mod))].append(mod)
         # then do the `jax.lax.scan` loops
         for _, group_mods in groups.items():
@@ -362,25 +386,25 @@
             # without having to compile the fully unrolled loop.
             stack = tree_stack(group_mods, broadcast_leaves=True)  # type: ignore[arg-type]
             # scan over first axis of stack
             dynamic_stack, static_stack = eqx.partition(stack, eqx.is_array)
 
             def calc_sf(_hist, _dynamic_stack, _static_stack):
                 stack = eqx.combine(_dynamic_stack, _static_stack)
-                sf = stack.scale_factor(_hist)
-                return _hist, sf
+                os = stack.offset_and_scale(_hist)
+                return _hist, os
 
             # if there is only one modifier in the group, we can skip the scan
             if len(group_mods) == 1:
-                _, sf = calc_sf(hist, dynamic_stack, static_stack)
-                multiplicative_sf *= sf.multiplicative
-                additive_sf *= sf.additive
+                _, os = calc_sf(hist, dynamic_stack, static_stack)
+                scale *= os.scale
+                offset += os.offset
             else:
-                _, sf = jax.lax.scan(
+                _, os = jax.lax.scan(
                     partial(calc_sf, _static_stack=static_stack),
                     hist,
                     dynamic_stack,
                 )
-                multiplicative_sf *= jnp.prod(sf.multiplicative, axis=0)
-                additive_sf += jnp.sum(sf.additive, axis=0)
+                scale *= jnp.prod(os.scale, axis=0)
+                offset += jnp.sum(os.offset, axis=0)
 
-        return SF(multiplicative=multiplicative_sf, additive=additive_sf)
+        return OffsetAndScale(offset=offset, scale=scale)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `evermore-0.2.5/src/evermore/pdf.py` & `evermore-0.2.6/src/evermore/pdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from jaxtyping import Array, PRNGKeyArray
 
 __all__ = [
     "PDF",
-    "Flat",
     "Normal",
     "Poisson",
 ]
 
 
 def __dir__():
     return __all__
@@ -23,45 +22,32 @@
     @abstractmethod
     def log_prob(self, x: Array) -> Array: ...
 
     @abstractmethod
     def sample(self, key: PRNGKeyArray) -> Array: ...
 
 
-class Flat(PDF):
-    def log_prob(self, x: Array) -> Array:
-        return jnp.zeros_like(x)
-
-    def sample(self, key: PRNGKeyArray) -> Array:
-        # sample parameter from pdf
-        # what should be the ranges?
-        # +/-jnp.inf leads to nans...
-        # minval=??,
-        # maxval=??,
-        return jax.random.uniform(key)
-
-
 class Normal(PDF):
-    mean: Array
-    width: Array
+    mean: Array = eqx.field(converter=jnp.atleast_1d)
+    width: Array = eqx.field(converter=jnp.atleast_1d)
 
     def log_prob(self, x: Array) -> Array:
         logpdf_max = jax.scipy.stats.norm.logpdf(
             self.mean, loc=self.mean, scale=self.width
         )
         unnormalized = jax.scipy.stats.norm.logpdf(x, loc=self.mean, scale=self.width)
         return unnormalized - logpdf_max
 
     def sample(self, key: PRNGKeyArray) -> Array:
         # sample parameter from pdf
         return self.mean + self.width * jax.random.normal(key)
 
 
 class Poisson(PDF):
-    lamb: Array
+    lamb: Array = eqx.field(converter=jnp.atleast_1d)
 
     def log_prob(self, x: Array) -> Array:
         logpdf_max = jax.scipy.stats.poisson.logpmf(self.lamb, mu=self.lamb)
         unnormalized = jax.scipy.stats.poisson.logpmf((x + 1) * self.lamb, mu=self.lamb)
         return unnormalized - logpdf_max
 
     def sample(self, key: PRNGKeyArray) -> Array:
```

### Comparing `evermore-0.2.5/src/evermore/util.py` & `evermore-0.2.6/src/evermore/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,86 +5,81 @@
 from functools import partial
 from typing import Any
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
-from jaxtyping import Array, ArrayLike, PyTree
+from jaxtyping import Array, PyTree
 
 __all__ = [
-    "is_parameter",
-    "sum_leaves",
+    "filter_tree_map",
+    "sum_over_leaves",
     "tree_stack",
-    "as1darray",
+    "dataclass_auto_init",
     "dump_hlo_graph",
     "dump_jaxpr",
 ]
 
 
 def __dir__():
     return __all__
 
 
-def is_parameter(leaf: Any) -> bool:
-    from evermore.parameter import Parameter
-
-    return isinstance(leaf, Parameter)
-
-
-def _filtered_module_map(
+def filter_tree_map(
     fun: Callable,
     module: eqx.Module,
     filter: Callable,
 ) -> eqx.Module:
     params = eqx.filter(module, filter, is_leaf=filter)
     return jtu.tree_map(
         fun,
         params,
         is_leaf=filter,
     )
 
 
-_params_map = partial(_filtered_module_map, filter=is_parameter)
-
-
-def sum_leaves(tree: PyTree) -> Array:
+def sum_over_leaves(tree: PyTree) -> Array:
     return jtu.tree_reduce(operator.add, tree)
 
 
 def tree_stack(trees: list[PyTree], broadcast_leaves: bool = False) -> PyTree:
     """
-    Turn an array of evm.Modifier(s) into a evm.Modifier of arrays.
+    Turns e.g. an array of evm.Modifier(s) into a evm.Modifier of arrays.
 
-    It is important that the jax.Array(s) of the underlying evm.Parameter have the same shape.
+    It is important that the jax.Array(s) of the underlying Arrays have the same shape.
     Same applies for the effect leaves (e.g. width). However, the effect leaves can be
     broadcasted to the same shape if broadcast_effect_leaves is set to True.
 
+    The stacked PyTree will have the static nodes of the first PyTree in the list.
+
     Example:
 
-        .. code-block:: python
+    .. code-block:: python
+
+        import evermore as evm
+        import jax
+        import jax.numpy as jnp
 
-            import evermore as evm
-            import jax
-            import jax.numpy as jnp
-
-            modifier = [
-                evm.NormalConstrained().log_normal(up=jnp.array([0.9, 0.95]), down=jnp.array([1.1, 1.14])),
-                evm.NormalConstrained().log_normal(up=jnp.array([0.8]), down=jnp.array([1.2])),
-            ]
-            print(modifier_stack2(modifier))
-            # -> Modifier(
-            #      parameter=NormalConstrained(
-            #        value=f32[2,1], # <- stacked dimension (2, 1)
-            #        lower=f32[1],
-            #        upper=f32[1],
-            #        constraint=Gauss(mean=f32[1], width=f32[1])
-            #      ),
-            #      effect=log_normal(up=f32[2,1], down=f32[2,1]) # <- stacked dimension (2, 1)
-            #    )
+        modifiers = [
+            evm.NormalParameter().scale_log(up=jnp.array([1.1]), down=jnp.array([0.9])),
+            evm.NormalParameter().scale_log(up=jnp.array([1.2]), down=jnp.array([0.8])),
+        ]
+        print(evm.util.tree_stack(modifiers))
+        # -> Modifier(
+        #      parameter=NormalParameter(
+        #        name=None,
+        #        value=f32[2,1], # <- stacked dimension (2, 1)
+        #        lower=f32[2,1], # <- stacked dimension (2, 1)
+        #        upper=f32[2,1], # <- stacked dimension (2, 1)
+        #        prior=Normal(mean=f32[2,1], width=f32[2,1]), # <- stacked dimension (2,1)
+        #        frozen=False
+        #      ),
+        #      effect=AsymmetricExponential(up=f32[2,1], down=f32[2,1]) # <- stacked dimension (2, 1)
+        #    )
     """
     # If there is only one modifier, we can return it directly
     if len(trees) == 1:
         return trees[0]
     leaves_list = []
     treedef_list = []
     for tree in trees:
@@ -101,33 +96,28 @@
                 jnp.stack(jtu.tree_map(partial(jnp.broadcast_to, shape=shape), leaves))
             )
         else:
             stacked_leaves.append(jnp.stack(leaves))
     return jtu.tree_unflatten(treedef_list[0], stacked_leaves)
 
 
-def as1darray(x: ArrayLike) -> Array:
-    """
-    Converts `x` to a 1d array.
-
-    Example:
-
-    .. code-block:: python
-
-        import jax.numpy as jnp
-
-
-        as1darray(1.0)
-        # -> Array([1.], dtype=float32, weak_type=True)
-
-        as1darray(jnp.array(1.0))
-        # -> Array([1.], dtype=float32, weak_type=True)
-    """
-
-    return jnp.atleast_1d(jnp.asarray(x))
+def dataclass_auto_init(module: eqx.Module) -> eqx.Module:
+    import dataclasses
+    import typing
+
+    from evermore.parameter import NormalParameter, Parameter
+
+    type_hints = typing.get_type_hints(module.__class__)
+    for field in dataclasses.fields(module):
+        name = field.name
+        hint = type_hints[name]
+        # we only have reasonable defaults for `FreeFloating` and `NormalConstrained`
+        if issubclass(hint, Parameter | NormalParameter) and not hasattr(module, name):
+            setattr(module, name, hint())
+    return module
 
 
 def dump_jaxpr(fun: Callable, *args: Any, **kwargs: Any) -> str:
     """Helper function to dump the Jaxpr of a function.
 
     Example:
```

### Comparing `evermore-0.2.5/.gitignore` & `evermore-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/LICENSE` & `evermore-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evermore-0.2.5/README.md` & `evermore-0.2.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center" style="height:250px;width:250px">
 <img src="https://raw.githubusercontent.com/pfackeldey/evermore/main/assets/logo.png" alt="logo"></img>
 </div>
 
 # evermore
 
-[![Documentation Status](https://readthedocs.org/projects/dilax/badge/?version=latest)](https://dilax.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/evermore/badge/?version=latest)](https://evermore.readthedocs.io/en/latest/?badge=latest)
 [![Actions Status][actions-badge]][actions-link]
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 Differentiable (binned) likelihoods in JAX.
 
 ## Installation
@@ -28,57 +28,67 @@
 ## Example - Model and Loss Definition
 
 See more in `examples/`
 
 _evermore_ in a nutshell:
 
 ```python3
+from typing import NamedTuple
+
 import equinox as eqx
 import jax
 import jax.numpy as jnp
-from jaxtyping import Array
+from jaxtyping import Array, PyTree
 
 import evermore as evm
 
 jax.config.update("jax_enable_x64", True)
 
 
 # define a simple model with two processes and two parameters
-class Model(eqx.Module):
-    mu: evm.FreeFloating
-    syst: evm.NormalConstrained
-
-    def __call__(self, hists: dict[str, Array]) -> Array:
-        mu_modifier = self.mu.unconstrained()
-        syst_modifier = self.syst.log_normal(up=jnp.array([1.1]), down=jnp.array([0.9]))
-        return mu_modifier(hists["signal"]) + syst_modifier(hists["bkg"])
-
-
-nll = evm.loss.PoissonNLL()
+def model(params: PyTree, hists: dict[str, Array]) -> Array:
+  mu_modifier = params.mu.scale()
+  syst_modifier = params.syst.scale_log(up=1.1, down=0.9)
+  return mu_modifier(hists["signal"]) + syst_modifier(hists["bkg"])
 
 
-def loss(model: Model, hists: dict[str, Array], observation: Array) -> Array:
-    expectation = model(hists)
+def loss(
+  diffable: PyTree,
+  static: PyTree,
+  hists: dict[str, Array],
+  observation: Array,
+) -> Array:
+    params = eqx.combine(diffable, static)
+    expectation = model(params, hists)
     # Poisson NLL of the expectation and observation
-    log_likelihood = nll(expectation, observation)
+    log_likelihood = evm.loss.PoissonLogLikelihood()(expectation, observation)
     # Add parameter constraints from logpdfs
-    constraints = evm.loss.get_log_probs(model)
-    log_likelihood += evm.util.sum_leaves(constraints)
+    constraints = evm.loss.get_log_probs(params)
+    log_likelihood += evm.util.sum_over_leaves(constraints)
     return -jnp.sum(log_likelihood)
 
 
-# setup model and data
+# setup data
 hists = {"signal": jnp.array([3]), "bkg": jnp.array([10])}
 observation = jnp.array([15])
-model = Model(mu=evm.FreeFloating(), syst=evm.NormalConstrained())
 
-# negative log-likelihood
-loss_val = loss(model, hists, observation)
-# gradients of negative log-likelihood w.r.t. model parameters
-grads = eqx.filter_grad(loss)(model, hists, observation)
+
+# define parameters, can be any PyTree of evm.Parameters
+class Params(NamedTuple):
+  mu: evm.Parameter
+  syst: evm.NormalParameter
+
+
+params = Params(mu=evm.Parameter(1.0), syst=evm.NormalParameter(0.0))
+diffable, static = evm.parameter.partition(params)
+
+# Calculate negative log-likelihood/loss
+loss_val = loss(diffable, static, hists, observation)
+# gradients of negative log-likelihood w.r.t. diffable parameters
+grads = eqx.filter_grad(loss)(diffable, static, hists, observation)
 print(f"{grads.mu.value=}, {grads.syst.value=}")
 # -> grads.mu.value=Array([-0.46153846]), grads.syst.value=Array([-0.15436207])
 ```
 
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) for instructions on how to contribute.
```

### Comparing `evermore-0.2.5/pyproject.toml` & `evermore-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 dev = ["pytest >=6", "pytest-cov >=3", "optax", "jaxopt >=0.6"]
 docs = [
     "sphinx>=7.0",
     "myst_parser>=0.13",
     "sphinx_copybutton",
     "sphinx_autodoc_typehints",
     "sphinx-book-theme",
+    "sphinx-design",
+    "sphinx-togglebutton",
 ]
 
 [project.urls]
 Homepage = "https://github.com/pfackeldey/evermore"
 "Bug Tracker" = "https://github.com/pfackeldey/evermore/issues"
 Discussions = "https://github.com/pfackeldey/evermore/discussions"
 Changelog = "https://github.com/pfackeldey/evermore/releases"
```

### Comparing `evermore-0.2.5/PKG-INFO` & `evermore-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: evermore
-Version: 0.2.5
+Version: 0.2.6
 Summary: Differentiable (binned) likelihoods in JAX.
 Project-URL: Homepage, https://github.com/pfackeldey/evermore
 Project-URL: Bug Tracker, https://github.com/pfackeldey/evermore/issues
 Project-URL: Discussions, https://github.com/pfackeldey/evermore/discussions
 Project-URL: Changelog, https://github.com/pfackeldey/evermore/releases
 Author-email: Peter Fackeldey <peter.fackeldey@rwth-aachen.de>
 License-File: LICENSE
@@ -32,27 +32,29 @@
 Requires-Dist: pytest-cov>=3; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-book-theme; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx-design; extra == 'docs'
+Requires-Dist: sphinx-togglebutton; extra == 'docs'
 Requires-Dist: sphinx>=7.0; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest-cov>=3; extra == 'test'
 Requires-Dist: pytest>=6; extra == 'test'
 Description-Content-Type: text/markdown
 
 <div align="center" style="height:250px;width:250px">
 <img src="https://raw.githubusercontent.com/pfackeldey/evermore/main/assets/logo.png" alt="logo"></img>
 </div>
 
 # evermore
 
-[![Documentation Status](https://readthedocs.org/projects/dilax/badge/?version=latest)](https://dilax.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/evermore/badge/?version=latest)](https://evermore.readthedocs.io/en/latest/?badge=latest)
 [![Actions Status][actions-badge]][actions-link]
 [![PyPI version][pypi-version]][pypi-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 Differentiable (binned) likelihoods in JAX.
 
 ## Installation
@@ -72,57 +74,67 @@
 ## Example - Model and Loss Definition
 
 See more in `examples/`
 
 _evermore_ in a nutshell:
 
 ```python3
+from typing import NamedTuple
+
 import equinox as eqx
 import jax
 import jax.numpy as jnp
-from jaxtyping import Array
+from jaxtyping import Array, PyTree
 
 import evermore as evm
 
 jax.config.update("jax_enable_x64", True)
 
 
 # define a simple model with two processes and two parameters
-class Model(eqx.Module):
-    mu: evm.FreeFloating
-    syst: evm.NormalConstrained
-
-    def __call__(self, hists: dict[str, Array]) -> Array:
-        mu_modifier = self.mu.unconstrained()
-        syst_modifier = self.syst.log_normal(up=jnp.array([1.1]), down=jnp.array([0.9]))
-        return mu_modifier(hists["signal"]) + syst_modifier(hists["bkg"])
-
-
-nll = evm.loss.PoissonNLL()
+def model(params: PyTree, hists: dict[str, Array]) -> Array:
+  mu_modifier = params.mu.scale()
+  syst_modifier = params.syst.scale_log(up=1.1, down=0.9)
+  return mu_modifier(hists["signal"]) + syst_modifier(hists["bkg"])
 
 
-def loss(model: Model, hists: dict[str, Array], observation: Array) -> Array:
-    expectation = model(hists)
+def loss(
+  diffable: PyTree,
+  static: PyTree,
+  hists: dict[str, Array],
+  observation: Array,
+) -> Array:
+    params = eqx.combine(diffable, static)
+    expectation = model(params, hists)
     # Poisson NLL of the expectation and observation
-    log_likelihood = nll(expectation, observation)
+    log_likelihood = evm.loss.PoissonLogLikelihood()(expectation, observation)
     # Add parameter constraints from logpdfs
-    constraints = evm.loss.get_log_probs(model)
-    log_likelihood += evm.util.sum_leaves(constraints)
+    constraints = evm.loss.get_log_probs(params)
+    log_likelihood += evm.util.sum_over_leaves(constraints)
     return -jnp.sum(log_likelihood)
 
 
-# setup model and data
+# setup data
 hists = {"signal": jnp.array([3]), "bkg": jnp.array([10])}
 observation = jnp.array([15])
-model = Model(mu=evm.FreeFloating(), syst=evm.NormalConstrained())
 
-# negative log-likelihood
-loss_val = loss(model, hists, observation)
-# gradients of negative log-likelihood w.r.t. model parameters
-grads = eqx.filter_grad(loss)(model, hists, observation)
+
+# define parameters, can be any PyTree of evm.Parameters
+class Params(NamedTuple):
+  mu: evm.Parameter
+  syst: evm.NormalParameter
+
+
+params = Params(mu=evm.Parameter(1.0), syst=evm.NormalParameter(0.0))
+diffable, static = evm.parameter.partition(params)
+
+# Calculate negative log-likelihood/loss
+loss_val = loss(diffable, static, hists, observation)
+# gradients of negative log-likelihood w.r.t. diffable parameters
+grads = eqx.filter_grad(loss)(diffable, static, hists, observation)
 print(f"{grads.mu.value=}, {grads.syst.value=}")
 # -> grads.mu.value=Array([-0.46153846]), grads.syst.value=Array([-0.15436207])
 ```
 
 ## Contributing
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) for instructions on how to contribute.
```

