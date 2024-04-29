# Comparing `tmp/pylint-silent-1.4.tar.gz` & `tmp/pylint_silent-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint-silent-1.4.tar", last modified: Mon Feb 12 04:04:43 2024, max compression
+gzip compressed data, was "pylint_silent-1.4.1.tar", last modified: Mon Apr 29 00:42:52 2024, max compression
```

## Comparing `pylint-silent-1.4.tar` & `pylint_silent-1.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 udi       (1000) udi       (1000)        0 2024-02-12 04:04:43.906103 pylint-silent-1.4/
--rw-r--r--   0 udi       (1000) udi       (1000)     7014 2024-02-12 04:04:43.906103 pylint-silent-1.4/PKG-INFO
--rw-rw-r--   0 udi       (1000) udi       (1000)     5938 2024-02-12 03:59:13.000000 pylint-silent-1.4/README.md
-drwxrwxr-x   0 udi       (1000) udi       (1000)        0 2024-02-12 04:04:43.906103 pylint-silent-1.4/pylint_silent/
--rw-rw-r--   0 udi       (1000) udi       (1000)    10530 2024-02-12 04:00:06.000000 pylint-silent-1.4/pylint_silent/__init__.py
--rw-rw-r--   0 udi       (1000) udi       (1000)     1798 2024-02-12 03:54:54.000000 pylint-silent-1.4/pylint_silent/__main__.py
-drwxrwxr-x   0 udi       (1000) udi       (1000)        0 2024-02-12 04:04:43.906103 pylint-silent-1.4/pylint_silent.egg-info/
--rw-r--r--   0 udi       (1000) udi       (1000)     7014 2024-02-12 04:04:43.000000 pylint-silent-1.4/pylint_silent.egg-info/PKG-INFO
--rw-rw-r--   0 udi       (1000) udi       (1000)      286 2024-02-12 04:04:43.000000 pylint-silent-1.4/pylint_silent.egg-info/SOURCES.txt
--rw-rw-r--   0 udi       (1000) udi       (1000)        1 2024-02-12 04:04:43.000000 pylint-silent-1.4/pylint_silent.egg-info/dependency_links.txt
--rw-rw-r--   0 udi       (1000) udi       (1000)       62 2024-02-12 04:04:43.000000 pylint-silent-1.4/pylint_silent.egg-info/entry_points.txt
--rw-rw-r--   0 udi       (1000) udi       (1000)       14 2024-02-12 04:04:43.000000 pylint-silent-1.4/pylint_silent.egg-info/top_level.txt
--rw-rw-r--   0 udi       (1000) udi       (1000)     2059 2024-02-12 03:54:54.000000 pylint-silent-1.4/pyproject.toml
--rw-rw-r--   0 udi       (1000) udi       (1000)       38 2024-02-12 04:04:43.906103 pylint-silent-1.4/setup.cfg
-drwxrwxr-x   0 udi       (1000) udi       (1000)        0 2024-02-12 04:04:43.906103 pylint-silent-1.4/tests/
--rw-rw-r--   0 udi       (1000) udi       (1000)     8532 2024-02-12 03:54:54.000000 pylint-silent-1.4/tests/test_samples.py
+drwxrwxr-x   0 udi       (1000) udi       (1000)        0 2024-04-29 00:42:52.092399 pylint_silent-1.4.1/
+-rw-r--r--   0 udi       (1000) udi       (1000)     7099 2024-04-29 00:42:52.092399 pylint_silent-1.4.1/PKG-INFO
+-rw-rw-r--   0 udi       (1000) udi       (1000)     6021 2024-04-29 00:35:05.000000 pylint_silent-1.4.1/README.md
+drwxrwxr-x   0 udi       (1000) udi       (1000)        0 2024-04-29 00:42:52.092399 pylint_silent-1.4.1/pylint_silent/
+-rw-rw-r--   0 udi       (1000) udi       (1000)    10583 2024-04-29 00:35:25.000000 pylint_silent-1.4.1/pylint_silent/__init__.py
+-rw-rw-r--   0 udi       (1000) udi       (1000)     1798 2024-02-12 03:54:54.000000 pylint_silent-1.4.1/pylint_silent/__main__.py
+drwxrwxr-x   0 udi       (1000) udi       (1000)        0 2024-04-29 00:42:52.092399 pylint_silent-1.4.1/pylint_silent.egg-info/
+-rw-r--r--   0 udi       (1000) udi       (1000)     7099 2024-04-29 00:42:52.000000 pylint_silent-1.4.1/pylint_silent.egg-info/PKG-INFO
+-rw-rw-r--   0 udi       (1000) udi       (1000)      286 2024-04-29 00:42:52.000000 pylint_silent-1.4.1/pylint_silent.egg-info/SOURCES.txt
+-rw-rw-r--   0 udi       (1000) udi       (1000)        1 2024-04-29 00:42:52.000000 pylint_silent-1.4.1/pylint_silent.egg-info/dependency_links.txt
+-rw-rw-r--   0 udi       (1000) udi       (1000)       62 2024-04-29 00:42:52.000000 pylint_silent-1.4.1/pylint_silent.egg-info/entry_points.txt
+-rw-rw-r--   0 udi       (1000) udi       (1000)       14 2024-04-29 00:42:52.000000 pylint_silent-1.4.1/pylint_silent.egg-info/top_level.txt
+-rw-rw-r--   0 udi       (1000) udi       (1000)     2059 2024-04-29 00:02:03.000000 pylint_silent-1.4.1/pyproject.toml
+-rw-rw-r--   0 udi       (1000) udi       (1000)       38 2024-04-29 00:42:52.092399 pylint_silent-1.4.1/setup.cfg
+drwxrwxr-x   0 udi       (1000) udi       (1000)        0 2024-04-29 00:42:52.092399 pylint_silent-1.4.1/tests/
+-rw-rw-r--   0 udi       (1000) udi       (1000)     8469 2024-04-29 00:10:24.000000 pylint_silent-1.4.1/tests/test_samples.py
```

### Comparing `pylint-silent-1.4/PKG-INFO` & `pylint_silent-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-silent
-Version: 1.4
+Version: 1.4.1
 Summary: Automatically add code comments to silence the output of pylint
 Author-email: Udi Fuchs <udifuchs@gmail.com>
 License: GPL-2.0-or-later
 Project-URL: Homepage, http://github.com/udifuchs/pylint-silent
 Keywords: pylint
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Development Status :: 5 - Production/Stable
@@ -132,14 +132,18 @@
 ### Summary
 `pylint`'s motto is: **It's not just a linter that annoys you!**
 
 `pylint-silent` helps `pylint` live up to its motto.
 
 ### Changelog
 
+#### 1.4.1 (2024-04-28)
+
+* Preserve file permissions also during reset. Fixes #6.
+
 #### 1.4 (2024-02-11)
 
 * Update compatible python versions to currently supported python 3.8 through 3.12.
 
 #### 1.3 (2023-05-12)
 
 * Mark every pylint-silent comment with a signature. Fixes #4. PR #5.
```

### Comparing `pylint-silent-1.4/README.md` & `pylint_silent-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,18 @@
 ### Summary
 `pylint`'s motto is: **It's not just a linter that annoys you!**
 
 `pylint-silent` helps `pylint` live up to its motto.
 
 ### Changelog
 
+#### 1.4.1 (2024-04-28)
+
+* Preserve file permissions also during reset. Fixes #6.
+
 #### 1.4 (2024-02-11)
 
 * Update compatible python versions to currently supported python 3.8 through 3.12.
 
 #### 1.3 (2023-05-12)
 
 * Mark every pylint-silent comment with a signature. Fixes #4. PR #5.
```

### Comparing `pylint-silent-1.4/pylint_silent/__init__.py` & `pylint_silent-1.4.1/pylint_silent/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Add "# pylint: disable" comments to silence the output of pylint."""
 import os
 import shutil
 from typing import Dict, List, Set
 
-VERSION = "1.4"
+VERSION = "1.4.1"
 
 EPILOG = """
 Commands:
   apply <pylint-output-file>
       Add pylint comments based on the output of pylint.
   reset <python-file> ...
       Remove pylint comments from specified python files.
@@ -197,14 +197,15 @@
                 if other_comment_pos > 0:
                     stripped_line += "  " + line[other_comment_pos:].rstrip()
                 line = stripped_line + EOL
                 something_changed = True
             out_file.write(line)
 
     if something_changed:
+        shutil.copymode(py_filename, out_filename)
         os.rename(out_filename, py_filename)
     else:
         os.remove(out_filename)
 
 
 def statistics(py_filenames: List[str], signature: str) -> None:
     """Show statistics on pylint comments from a list of python files."""
```

### Comparing `pylint-silent-1.4/pylint_silent/__main__.py` & `pylint_silent-1.4.1/pylint_silent/__main__.py`

 * *Files identical despite different names*

### Comparing `pylint-silent-1.4/pylint_silent.egg-info/PKG-INFO` & `pylint_silent-1.4.1/pylint_silent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylint-silent
-Version: 1.4
+Version: 1.4.1
 Summary: Automatically add code comments to silence the output of pylint
 Author-email: Udi Fuchs <udifuchs@gmail.com>
 License: GPL-2.0-or-later
 Project-URL: Homepage, http://github.com/udifuchs/pylint-silent
 Keywords: pylint
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Development Status :: 5 - Production/Stable
@@ -132,14 +132,18 @@
 ### Summary
 `pylint`'s motto is: **It's not just a linter that annoys you!**
 
 `pylint-silent` helps `pylint` live up to its motto.
 
 ### Changelog
 
+#### 1.4.1 (2024-04-28)
+
+* Preserve file permissions also during reset. Fixes #6.
+
 #### 1.4 (2024-02-11)
 
 * Update compatible python versions to currently supported python 3.8 through 3.12.
 
 #### 1.3 (2023-05-12)
 
 * Mark every pylint-silent comment with a signature. Fixes #4. PR #5.
```

### Comparing `pylint-silent-1.4/pyproject.toml` & `pylint_silent-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylint-silent-1.4/tests/test_samples.py` & `pylint_silent-1.4.1/tests/test_samples.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,14 +73,22 @@
     def run_pylint_to_file(self, out_file: str) -> Optional[int]:
         """Run pylint on our python test files redirecting stdout to file."""
         with open(out_file, "w", encoding="utf-8") as out, \
              redirect_stdout(out):
             return self.run_pylint("--max-module-lines=10")
 
 
+def assert_files_equal(file_1: str, file_2: str) -> None:
+    """Check that both file are the same and have the same permissions."""
+    assert filecmp.cmp(file_1, file_2), f"diff {file_1} {file_2}"
+    f1_mode = os.stat(file_1).st_mode
+    f2_mode = os.stat(file_2).st_mode
+    assert f1_mode == f2_mode, f"diff mode {file_1}({f1_mode:o}) {file_2}({f2_mode:o})"
+
+
 @pytest.fixture(name="ctx")
 def fixture_ctx(tmpdir: str) -> Context:
     """Create context fixture for running tests."""
     return Context(tmpdir)
 
 
 def test_version_option() -> None:
@@ -107,16 +115,15 @@
     pylint_output = ctx.temp_sample_filename + "lint"
     ctx.run_pylint_to_file(pylint_output)
 
     # Apply pylint-silent changed based on output from pylint.
     run_pylint_silent("apply", "--max-line-length=70", pylint_output)
 
     # Test that the expected python file was generated.
-    assert filecmp.cmp(ctx.temp_sample_filename, ctx.sample_after_apply), \
-        f"diff {ctx.temp_sample_filename} {ctx.sample_after_apply}"
+    assert_files_equal(ctx.temp_sample_filename, ctx.sample_after_apply)
 
     # Test that pylint is indeed silent now.
     exitcode = ctx.run_pylint("--disable=duplicate-code")
     assert exitcode == 0
 
 
 def test_apply_signature(ctx: Context) -> None:
@@ -125,16 +132,15 @@
     pylint_output = ctx.temp_sample_filename + "lint"
     ctx.run_pylint_to_file(pylint_output)
 
     # Apply pylint-silent changed based on output from pylint.
     run_pylint_silent("apply", "--signature", pylint_output)
 
     # Test that the expected python file was generated.
-    assert filecmp.cmp(ctx.temp_sample_filename, ctx.sample_after_apply_w_sig), \
-        f"diff {ctx.temp_sample_filename} {ctx.sample_after_apply_w_sig}"
+    assert_files_equal(ctx.temp_sample_filename, ctx.sample_after_apply_w_sig)
 
     # Test that pylint is indeed silent now.
     exitcode = ctx.run_pylint("--disable=duplicate-code")
     assert exitcode == 0
 
 
 def test_stats(ctx: Context) -> None:
@@ -172,38 +178,34 @@
 
 def test_reset(ctx: Context) -> None:
     """Test 'pylint-silent reset'.
     Remove all generated comments and test that we are back to the original code.
     """
     run_pylint_silent("reset", ctx.temp_sample_after_apply)
 
-    assert filecmp.cmp(ctx.temp_sample_after_apply, ctx.sample_filename), \
-        f"diff {ctx.temp_sample_after_apply} {ctx.sample_filename}"
+    assert_files_equal(ctx.temp_sample_after_apply, ctx.sample_filename)
 
     # Test resetting a clean file.
     run_pylint_silent("reset", ctx.temp_sample_after_apply)
 
-    assert filecmp.cmp(ctx.temp_sample_after_apply, ctx.sample_filename), \
-        f"diff {ctx.temp_sample_filename} {ctx.sample_filename}"
+    assert_files_equal(ctx.temp_sample_after_apply, ctx.sample_filename)
 
     # Test resetting a file with signature.
     run_pylint_silent("reset", "--signature", ctx.temp_sample_after_apply_w_sig)
 
-    assert filecmp.cmp(ctx.temp_sample_after_apply_w_sig, ctx.sample_filename), \
-        f"diff {ctx.temp_sample_filename} {ctx.sample_filename}"
+    assert_files_equal(ctx.temp_sample_after_apply_w_sig, ctx.sample_filename)
 
 
 def test_reset_sample2(ctx: Context) -> None:
     """Test 'pylint-silent reset' of the second sample file.
 
     Remove all pylint comments and test that we preserve other comments
     """
     run_pylint_silent("reset", ctx.temp_sample2_filename)
 
-    assert filecmp.cmp(ctx.sample2_after_reset, ctx.temp_sample2_filename), \
-        f"diff {ctx.sample2_after_reset} {ctx.temp_sample2_filename}"
+    assert_files_equal(ctx.sample2_after_reset, ctx.temp_sample2_filename)
 
     # Test resetting a file without signatures but with --signature (should fail)
     run_pylint_silent("reset", "--signature", ctx.temp_sample2_again_filename)
     assert (
         filecmp.cmp(ctx.sample2_after_reset, ctx.temp_sample2_again_filename) is False
     )
```

