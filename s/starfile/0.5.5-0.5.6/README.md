# Comparing `tmp/starfile-0.5.5.tar.gz` & `tmp/starfile-0.5.6.tar.gz`

## Comparing `starfile-0.5.5.tar` & `starfile-0.5.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 starfile-0.5.5/.copier-answers.yml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 starfile-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 starfile-0.5.5/mkdocs.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 starfile-0.5.5/setup.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 starfile-0.5.5/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 starfile-0.5.5/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 starfile-0.5.5/.github/dependabot.yml
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 starfile-0.5.5/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 starfile-0.5.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 starfile-0.5.5/docs/index.md
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 starfile-0.5.5/docs/examples/merging.md
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 starfile-0.5.5/docs/examples/multi_block.md
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 starfile-0.5.5/docs/examples/single_block.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 starfile-0.5.5/src/starfile/__init__.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 starfile-0.5.5/src/starfile/__main__.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 starfile-0.5.5/src/starfile/functions.py
--rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 starfile-0.5.5/src/starfile/parser.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 starfile-0.5.5/src/starfile/typing.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 starfile-0.5.5/src/starfile/utils.py
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 starfile-0.5.5/src/starfile/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/__init__.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/constants.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/test_functional_interface.py
--rw-r--r--   0        0        0     8477 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/test_parsing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/test_read_write_round_trip.py
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/test_writing.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/utils.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/basic_double_quote.star
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/basic_single_quote.star
--rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/default_pipeline.star
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/empty_loop.star
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/loop_double_quote.star
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/loop_single_quote.star
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/one_loop.star
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/postprocess.star
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/rln3.1_data_style.star
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/single_line_end_of_multiblock.star
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/single_line_middle_of_multiblock.star
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/two_basic_blocks.star
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/two_single_line_loop_blocks.star
--rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/relion_tutorial/run_it025_optimiser_2D.star
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/relion_tutorial/run_it025_optimiser_3D.star
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/relion_tutorial/run_it025_sampling_2D.star
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 starfile-0.5.5/tests/data/relion_tutorial/run_it025_sampling_3D.star
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 starfile-0.5.5/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 starfile-0.5.5/LICENSE
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 starfile-0.5.5/README.md
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 starfile-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 starfile-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 starfile-0.5.6/.copier-answers.yml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 starfile-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 starfile-0.5.6/mkdocs.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 starfile-0.5.6/setup.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 starfile-0.5.6/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 starfile-0.5.6/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 starfile-0.5.6/.github/dependabot.yml
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 starfile-0.5.6/.github/workflows/build-and-deploy-docs.yml
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 starfile-0.5.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 starfile-0.5.6/docs/index.md
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 starfile-0.5.6/docs/examples/merging.md
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 starfile-0.5.6/docs/examples/multi_block.md
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 starfile-0.5.6/docs/examples/single_block.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 starfile-0.5.6/src/starfile/__init__.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 starfile-0.5.6/src/starfile/__main__.py
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 starfile-0.5.6/src/starfile/functions.py
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 starfile-0.5.6/src/starfile/parser.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 starfile-0.5.6/src/starfile/typing.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 starfile-0.5.6/src/starfile/utils.py
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 starfile-0.5.6/src/starfile/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/__init__.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/constants.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/test_functional_interface.py
+-rw-r--r--   0        0        0     8960 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/test_parsing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/test_read_write_round_trip.py
+-rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/test_writing.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/utils.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/basic_double_quote.star
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/basic_single_quote.star
+-rw-r--r--   0        0        0    12768 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/default_pipeline.star
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/empty_loop.star
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/loop_double_quote.star
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/loop_single_quote.star
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/one_loop.star
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/postprocess.star
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/rln3.1_data_style.star
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/single_line_end_of_multiblock.star
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/single_line_middle_of_multiblock.star
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/two_basic_blocks.star
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/two_single_line_loop_blocks.star
+-rw-r--r--   0        0        0     6125 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/relion_tutorial/run_it025_optimiser_2D.star
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/relion_tutorial/run_it025_optimiser_3D.star
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/relion_tutorial/run_it025_sampling_2D.star
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 starfile-0.5.6/tests/data/relion_tutorial/run_it025_sampling_3D.star
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 starfile-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 starfile-0.5.6/LICENSE
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 starfile-0.5.6/README.md
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 starfile-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 starfile-0.5.6/PKG-INFO
```

### Comparing `starfile-0.5.5/.pre-commit-config.yaml` & `starfile-0.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/mkdocs.yml` & `starfile-0.5.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/.github/workflows/build-and-deploy-docs.yml` & `starfile-0.5.6/.github/workflows/build-and-deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/.github/workflows/ci.yml` & `starfile-0.5.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/docs/index.md` & `starfile-0.5.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/docs/examples/merging.md` & `starfile-0.5.6/docs/examples/merging.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/docs/examples/multi_block.md` & `starfile-0.5.6/docs/examples/multi_block.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/docs/examples/single_block.md` & `starfile-0.5.6/docs/examples/single_block.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/src/starfile/__main__.py` & `starfile-0.5.6/src/starfile/__main__.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/src/starfile/utils.py` & `starfile-0.5.6/src/starfile/utils.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/src/starfile/writer.py` & `starfile-0.5.6/src/starfile/writer.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/constants.py` & `starfile-0.5.6/tests/constants.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/test_functional_interface.py` & `starfile-0.5.6/tests/test_functional_interface.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/test_parsing.py` & `starfile-0.5.6/tests/test_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,38 +239,51 @@
 
 def test_empty_loop_block():
     """Parsing an empty loop block should return an empty dataframe."""
     parser = StarParser(empty_loop)
     assert len(parser.data_blocks) == 1
 
 
-
-@pytest.mark.parametrize("quote_character, filename", [("'",basic_single_quote), 
-                                                 ('"',basic_double_quote), 
-                                                 ])
-def test_quote_basic(quote_character,filename):
+@pytest.mark.parametrize("quote_character, filename", [("'", basic_single_quote),
+                                                       ('"', basic_double_quote),
+                                                       ])
+def test_quote_basic(quote_character, filename):
     parser = StarParser(filename)
     assert len(parser.data_blocks) == 1
     assert parser.data_blocks['']['no_quote_string'] == "noquote"
     assert parser.data_blocks['']['quote_string'] == "quote string"
     assert parser.data_blocks['']['whitespace_string'] == " "
     assert parser.data_blocks['']['empty_string'] == ""
 
-@pytest.mark.parametrize("quote_character, filename", [("'",loop_single_quote), 
-                                                 ('"',loop_double_quote), 
-                                                 ])
-def test_quote_loop(quote_character,filename):
+
+@pytest.mark.parametrize("quote_character, filename", [("'", loop_single_quote),
+                                                       ('"', loop_double_quote),
+                                                       ])
+def test_quote_loop(quote_character, filename):
     import math
     parser = StarParser(filename)
     assert len(parser.data_blocks) == 1
-    assert parser.data_blocks[''].loc[0,'no_quote_string'] == "noquote"
-    assert parser.data_blocks[''].loc[0,'quote_string'] == "quote string"
-    assert parser.data_blocks[''].loc[0,'whitespace_string'] == " "
-    assert parser.data_blocks[''].loc[0,'empty_string'] == ""
+    assert parser.data_blocks[''].loc[0, 'no_quote_string'] == "noquote"
+    assert parser.data_blocks[''].loc[0, 'quote_string'] == "quote string"
+    assert parser.data_blocks[''].loc[0, 'whitespace_string'] == " "
+    assert parser.data_blocks[''].loc[0, 'empty_string'] == ""
 
     assert parser.data_blocks[''].dtypes['number_and_string'] == object
     assert parser.data_blocks[''].dtypes['number_and_empty'] == 'float64'
     assert parser.data_blocks[''].dtypes['number'] == 'float64'
     assert parser.data_blocks[''].dtypes['empty_string_and_normal_string'] == object
 
-    assert math.isnan(parser.data_blocks[''].loc[1,'number_and_empty'])
-    assert parser.data_blocks[''].loc[0,'empty_string_and_normal_string'] == ''
+    assert math.isnan(parser.data_blocks[''].loc[1, 'number_and_empty'])
+    assert parser.data_blocks[''].loc[0, 'empty_string_and_normal_string'] == ''
+
+
+def test_parse_as_string():
+    parser = StarParser(postprocess, parse_as_string=['rlnFinalResolution', 'rlnResolution'])
+
+    # check 'rlnFinalResolution' is parsed as string in general (basic) block
+    block = parser.data_blocks['general']
+    assert type(block['rlnFinalResolution']) == str
+
+    # check 'rlnResolution' is parsed as string in fsc (loop) block
+    df = parser.data_blocks['fsc']
+    assert df['rlnResolution'].dtype == 'object'
+
```

### Comparing `starfile-0.5.5/tests/test_read_write_round_trip.py` & `starfile-0.5.6/tests/test_read_write_round_trip.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/test_writing.py` & `starfile-0.5.6/tests/test_writing.py`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/default_pipeline.star` & `starfile-0.5.6/tests/data/default_pipeline.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/one_loop.star` & `starfile-0.5.6/tests/data/one_loop.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/postprocess.star` & `starfile-0.5.6/tests/data/postprocess.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/rln3.1_data_style.star` & `starfile-0.5.6/tests/data/rln3.1_data_style.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/single_line_end_of_multiblock.star` & `starfile-0.5.6/tests/data/single_line_end_of_multiblock.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/relion_tutorial/run_it025_optimiser_2D.star` & `starfile-0.5.6/tests/data/relion_tutorial/run_it025_optimiser_2D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/relion_tutorial/run_it025_optimiser_3D.star` & `starfile-0.5.6/tests/data/relion_tutorial/run_it025_optimiser_3D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/relion_tutorial/run_it025_sampling_2D.star` & `starfile-0.5.6/tests/data/relion_tutorial/run_it025_sampling_2D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/tests/data/relion_tutorial/run_it025_sampling_3D.star` & `starfile-0.5.6/tests/data/relion_tutorial/run_it025_sampling_3D.star`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/LICENSE` & `starfile-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/README.md` & `starfile-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/pyproject.toml` & `starfile-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starfile-0.5.5/PKG-INFO` & `starfile-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfile
-Version: 0.5.5
+Version: 0.5.6
 Summary: STAR file I/O in Python
 Project-URL: homepage, https://github.com/teamtomo/starfile
 Project-URL: repository, https://github.com/teamtomo/starfile
 Author-email: Alister Burt <alisterburt@gmail.com>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

