# Comparing `tmp/ndjson_testrunner-1.1.2.tar.gz` & `tmp/ndjson_testrunner-1.1.3.tar.gz`

## Comparing `ndjson_testrunner-1.1.2.tar` & `ndjson_testrunner-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/.editorconfig
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/.prettierrc.yaml
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/.vscode/launch.json
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/.vscode/settings.json
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/src/ndjson_testrunner/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/src/ndjson_testrunner/py.typed
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/tests/tests.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/LICENSE
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/README.rst
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/.editorconfig
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/.prettierrc.yaml
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/.vscode/launch.json
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0     4965 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/src/ndjson_testrunner/__init__.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/src/ndjson_testrunner/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/src/ndjson_testrunner/py.typed
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/tests/tests.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/README.rst
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 ndjson_testrunner-1.1.3/PKG-INFO
```

### Comparing `ndjson_testrunner-1.1.2/.pre-commit-config.yaml` & `ndjson_testrunner-1.1.3/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # To install the git pre-commit hooks run:
 #   pre-commit install --install-hooks
 # To update the versions:
 #   pre-commit autoupdate
 # Note the order is intentional to avoid multiple passes of the hooks
 repos:
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.3
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix, --show-fixes]
       - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.3
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.6.1
+    rev: v1.9.0
     hooks:
       - id: mypy
```

### Comparing `ndjson_testrunner-1.1.2/.github/workflows/run_tests.yml` & `ndjson_testrunner-1.1.3/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `ndjson_testrunner-1.1.2/.vscode/settings.json` & `ndjson_testrunner-1.1.3/.vscode/settings.json`

 * *Files 18% similar despite different names*

```diff
@@ -4,18 +4,18 @@
   },
   "[json][jsonc][yaml]": {
     "editor.defaultFormatter": "esbenp.prettier-vscode",
   },
   "[python]": {
     "editor.defaultFormatter": "charliermarsh.ruff",
     "editor.codeActionsOnSave": {
-      "source.fixAll": true,
-      "source.organizeImports": true,
+      "source.fixAll": "explicit",
+      "source.organizeImports": "explicit",
     },
   },
   "python.analysis.typeCheckingMode": "basic",
   "python.testing.unittestEnabled": true,
   "python.testing.unittestArgs": ["-vv", "-s", "tests"],
   "python.terminal.activateEnvironment": false,
   "coverage-gutters.showGutterCoverage": true,
-  "editor.wordBasedSuggestions": false,
+  "editor.wordBasedSuggestions": "off",
 }
```

### Comparing `ndjson_testrunner-1.1.2/src/ndjson_testrunner/__init__.py` & `ndjson_testrunner-1.1.3/src/ndjson_testrunner/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,13 +137,7 @@
     def run(self, test: unittest.TestSuite | unittest.TestCase) -> JSONTestResult:
         """Run the given test case or test suite."""
         result = JSONTestResult(self.stream, self.failfast, self.buffer, self.tb_locals)
         unittest.registerResult(result)
         with self.filter_warnings():
             result.test_run(test)
         return result
-
-
-if __name__ == "__main__":
-    module = sys.argv[1]
-    sys.argv[1:] = sys.argv[2:]
-    unittest.main(module, testRunner=JSONTestRunner)
```

### Comparing `ndjson_testrunner-1.1.2/tests/tests.py` & `ndjson_testrunner-1.1.3/tests/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,20 +38,18 @@
 
 class TestRunner(unittest.TestCase):
     def setUp(self) -> None:
         self.capture = StringIO()
         self.runner = JSONTestRunner(self.capture)
 
     @overload
-    def run_test(self, name: str, subtests: Literal[False] = False) -> TestResultDict:
-        ...
+    def run_test(self, name: str, subtests: Literal[False] = False) -> TestResultDict: ...
 
     @overload
-    def run_test(self, name: str, subtests: Literal[True]) -> map[TestResultDict]:
-        ...
+    def run_test(self, name: str, subtests: Literal[True]) -> map[TestResultDict]: ...
 
     def run_test(self, name: str, subtests: bool = False) -> TestResultDict | map[TestResultDict]:
         self.runner.run(unittest.defaultTestLoader.loadTestsFromName(f"tests.TestsToBeTested.{name}"))
         v = self.capture.getvalue()
         self.assertTrue(v, "no JSON received")
         if subtests:
             return map(json.loads, v.strip().split("\n"))
```

### Comparing `ndjson_testrunner-1.1.2/LICENSE` & `ndjson_testrunner-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ndjson_testrunner-1.1.2/README.rst` & `ndjson_testrunner-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `ndjson_testrunner-1.1.2/pyproject.toml` & `ndjson_testrunner-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ndjson_testrunner-1.1.2/PKG-INFO` & `ndjson_testrunner-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: ndjson-testrunner
-Version: 1.1.2
+Version: 1.1.3
 Summary: A test runner that outputs newline delimited JSON results
 Project-URL: Source, https://github.com/flying-sheep/ndjson-testrunner
 Author-email: "Philipp A." <flying-sheep@web.de>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

