# Comparing `tmp/pawz-0.2.0.tar.gz` & `tmp/pawz-0.2.1.tar.gz`

## Comparing `pawz-0.2.0.tar` & `pawz-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pawz-0.2.0/dev-requirements.txt
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pawz-0.2.0/justfile
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pawz-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pawz-0.2.0/src/pawz/__init__.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pawz-0.2.0/src/pawz-core/Cargo.toml
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 pawz-0.2.0/src/pawz-core/pyproject.toml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pawz-0.2.0/src/pawz-core/readme.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pawz-0.2.0/src/pawz-core/src/lib.rs
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pawz-0.2.0/src/pawz-core/src/main.rs
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pawz-0.2.0/.gitignore
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pawz-0.2.0/LICENSE
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pawz-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pawz-0.2.0/readme.md
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 pawz-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pawz-0.2.1/dev-requirements.txt
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pawz-0.2.1/justfile
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pawz-0.2.1/.vscode/settings.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 pawz-0.2.1/src/pawz/__init__.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pawz-0.2.1/src/pawz-core/Cargo.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 pawz-0.2.1/src/pawz-core/pyproject.toml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pawz-0.2.1/src/pawz-core/readme.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pawz-0.2.1/src/pawz-core/src/lib.rs
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pawz-0.2.1/src/pawz-core/src/main.rs
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pawz-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 pawz-0.2.1/LICENSE
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 pawz-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 pawz-0.2.1/readme.md
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 pawz-0.2.1/PKG-INFO
```

### Comparing `pawz-0.2.0/justfile` & `pawz-0.2.1/justfile`

 * *Files 3% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     @maturin dev -m src/pawz-core/Cargo.toml
     @pip install --upgrade -e '.[all]'
 
 # uninstall
 uninstall:
     @pip uninstall pawz pawz-core -y
 
-# publish-test
+# release-test
 release-test:
     just build
     @twine upload --repository testpypi src/pawz-core/dist/* -u __token__ -p ${PYPI_TEST_TOKEN}
     @twine upload --repository testpypi dist/* -u __token__ -p ${PYPI_TEST_TOKEN}
 
-# publish
+# release
 release:
     just build
     @twine upload src/pawz-core/dist/* -u __token__ -p ${PYPI_TOKEN}
     @twine upload dist/* -u __token__ -p ${PYPI_TOKEN}
 
 # clean
 clean:
```

### Comparing `pawz-0.2.0/src/pawz-core/pyproject.toml` & `pawz-0.2.1/src/pawz-core/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "pawz_core"
+dynamic = ["version"]
 authors = [{ name = "Cody", email = "cody@dkdc.dev" }]
-description = "pawz the dog (core)"
+description = "pawz core functionality (Rust!)"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 dependencies = []
-dynamic = ["version"]
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [project.urls]
 "Homepage" = "https://github.com/lostmygithubaccount/pawz"
 "Bug Tracker" = "https://github.com/lostmygithubaccount/pawz/issues"
```

### Comparing `pawz-0.2.0/LICENSE` & `pawz-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pawz-0.2.0/pyproject.toml` & `pawz-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pawz"
-version = "0.2.0"
+version = "0.2.1"
 authors = [{ name = "Cody", email = "cody@dkdc.dev" }]
 description = "a demo of Python + Rust"
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `pawz-0.2.0/PKG-INFO` & `pawz-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pawz
-Version: 0.2.0
+Version: 0.2.1
 Summary: a demo of Python + Rust
 Project-URL: Homepage, https://github.com/lostmygithubaccount/pawz
 Project-URL: Bug Tracker, https://github.com/lostmygithubaccount/pawz/issues
 Author-email: Cody <cody@dkdc.dev>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

