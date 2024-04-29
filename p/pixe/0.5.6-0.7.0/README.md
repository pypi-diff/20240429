# Comparing `tmp/pixe-0.5.6.tar.gz` & `tmp/pixe-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixe-0.5.6.tar", last modified: Mon May 22 03:29:48 2023, max compression
+gzip compressed data, was "pixe-0.7.0.tar", last modified: Mon Apr 29 01:26:03 2024, max compression
```

## Comparing `pixe-0.5.6.tar` & `pixe-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 03:29:48.591004 pixe-0.5.6/
--rw-rw-r--   0 iroh      (1000) iroh      (1000)    11357 2023-02-28 15:56:19.000000 pixe-0.5.6/LICENSE
--rw-rw-r--   0 iroh      (1000) iroh      (1000)     4003 2023-05-22 03:29:48.590004 pixe-0.5.6/PKG-INFO
--rw-r--r--   0 iroh      (1000) iroh      (1000)     3382 2023-05-22 00:30:49.000000 pixe-0.5.6/README.md
-drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 03:29:48.590004 pixe-0.5.6/pixe.egg-info/
--rw-rw-r--   0 iroh      (1000) iroh      (1000)     4003 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/PKG-INFO
--rw-rw-r--   0 iroh      (1000) iroh      (1000)      255 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/SOURCES.txt
--rw-rw-r--   0 iroh      (1000) iroh      (1000)        1 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/dependency_links.txt
--rw-rw-r--   0 iroh      (1000) iroh      (1000)       34 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/entry_points.txt
--rw-rw-r--   0 iroh      (1000) iroh      (1000)      126 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/requires.txt
--rw-rw-r--   0 iroh      (1000) iroh      (1000)        5 2023-05-22 03:29:48.000000 pixe-0.5.6/pixe.egg-info/top_level.txt
--rw-r--r--   0 iroh      (1000) iroh      (1000)     7358 2023-05-22 03:26:18.000000 pixe-0.5.6/pixe.py
--rw-r--r--   0 iroh      (1000) iroh      (1000)      867 2023-05-22 03:28:27.000000 pixe-0.5.6/pyproject.toml
--rw-rw-r--   0 iroh      (1000) iroh      (1000)       38 2023-05-22 03:29:48.591004 pixe-0.5.6/setup.cfg
-drwxrwxr-x   0 iroh      (1000) iroh      (1000)        0 2023-05-22 03:29:48.590004 pixe-0.5.6/tests/
--rw-rw-r--   0 iroh      (1000) iroh      (1000)     3683 2023-02-28 15:56:19.000000 pixe-0.5.6/tests/test_integration.py
--rw-rw-r--   0 iroh      (1000) iroh      (1000)     1744 2023-02-28 15:56:19.000000 pixe-0.5.6/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.928824 pixe-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 01:26:00.000000 pixe-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-29 01:26:03.928824 pixe-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-29 01:26:00.000000 pixe-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 01:26:00.000000 pixe-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 01:26:03.928824 pixe-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.924823 pixe-0.7.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:00.000000 pixe-0.7.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.924823 pixe-0.7.0/src/filetypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-29 01:26:00.000000 pixe-0.7.0/src/filetypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-29 01:26:00.000000 pixe-0.7.0/src/filetypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-04-29 01:26:00.000000 pixe-0.7.0/src/filetypes/image_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-29 01:26:00.000000 pixe-0.7.0/src/filetypes/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.924823 pixe-0.7.0/src/pixe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 01:26:03.000000 pixe-0.7.0/src/pixe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-29 01:26:00.000000 pixe-0.7.0/src/pixe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 01:26:03.924823 pixe-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-04-29 01:26:00.000000 pixe-0.7.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-04-29 01:26:00.000000 pixe-0.7.0/tests/test_unit.py
```

### Comparing `pixe-0.5.6/LICENSE` & `pixe-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pixe-0.5.6/PKG-INFO` & `pixe-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: pixe
-Version: 0.5.6
-Summary: A digital helper to keep your files neat and tidy
-Author-email: Chris Wells <chris@ithuna.com>
-License: Apache License, Version 2.0
-Project-URL: homepage, https://github.com/ithuna/pixe.git
-Keywords: archive,photos,organize
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Topic :: System :: Archiving
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-License-File: LICENSE
-
 # pixe
 [![flake8](https://github.com/ithuna/pixe/actions/workflows/flake8.yml/badge.svg)](https://github.com/ithuna/pixe/actions/workflows/flake8.yml) [![pytest](https://github.com/ithuna/pixe/actions/workflows/pytest.yml/badge.svg)](https://github.com/ithuna/pixe/actions/workflows/pytest.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A digital helper to keep your files neat and tidy.
 
 In its most basic invocation: `pixe <directory with files>` `pixe` will copy all JPG files from a source directory into a new set of subdirectories based on capture date. These files will also be renamed based on said capture date and a calculated SHA1 hash.
```

### Comparing `pixe-0.5.6/pixe.egg-info/PKG-INFO` & `pixe-0.7.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 Metadata-Version: 2.1
 Name: pixe
-Version: 0.5.6
+Version: 0.7.0
 Summary: A digital helper to keep your files neat and tidy
 Author-email: Chris Wells <chris@ithuna.com>
 License: Apache License, Version 2.0
 Project-URL: homepage, https://github.com/ithuna/pixe.git
 Keywords: archive,photos,organize
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Topic :: System :: Archiving
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: Click<8.2,>=8.1.3
+Requires-Dist: Pillow<10.5,>=10.4.0
+Requires-Dist: piexif<1.2,>=1.1.3
+Requires-Dist: ffmpeg-python<0.3.0,>=0.2.0
+Requires-Dist: pillow-heif>=0.16.0
+Requires-Dist: pyexiftool>=0.5.0
+Provides-Extra: tests
+Requires-Dist: pytest<7.3,>=7.2.1; extra == "tests"
+Requires-Dist: pytest-cov<4.1,>=4.0.0; extra == "tests"
+Requires-Dist: pytest-freezegun<0.5.0,>=0.4.2; extra == "tests"
+Requires-Dist: flake8<6.1,>=6.0.0; extra == "tests"
 
 # pixe
 [![flake8](https://github.com/ithuna/pixe/actions/workflows/flake8.yml/badge.svg)](https://github.com/ithuna/pixe/actions/workflows/flake8.yml) [![pytest](https://github.com/ithuna/pixe/actions/workflows/pytest.yml/badge.svg)](https://github.com/ithuna/pixe/actions/workflows/pytest.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A digital helper to keep your files neat and tidy.
 
 In its most basic invocation: `pixe <directory with files>` `pixe` will copy all JPG files from a source directory into a new set of subdirectories based on capture date. These files will also be renamed based on said capture date and a calculated SHA1 hash.
```

### Comparing `pixe-0.5.6/pyproject.toml` & `pixe-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixe"
-version = "0.5.6"
+version = "0.7.0"
 description = "A digital helper to keep your files neat and tidy"
 readme = "README.md"
 requires-python = ">=3.11"
 license = {text = "Apache License, Version 2.0"}
 keywords = ["archive", "photos", "organize"]
 authors = [
     {name = "Chris Wells", email = "chris@ithuna.com"},
@@ -14,23 +14,30 @@
     "License :: OSI Approved :: Apache Software License",
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Topic :: System :: Archiving",
 ]
 dependencies = [
     "Click>=8.1.3,<8.2",
-    "Pillow>=9.4.0,<9.5",
+    "Pillow>=10.4.0,<10.5",
     "piexif>=1.1.3,<1.2",
+    "ffmpeg-python>=0.2.0,<0.3.0",
+    "pillow-heif >=0.16.0",
+    "pyexiftool >=0.5.0",
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest>=7.2.1,<7.3",
     "pytest-cov>=4.0.0,<4.1",
+    "pytest-freezegun>=0.4.2,<0.5.0",
     "flake8>=6.0.0,<6.1",
 ]
 
 [project.urls]
 homepage = "https://github.com/ithuna/pixe.git"
 
 [project.scripts]
-pixe = "pixe:cli"
+pixe = "pixe:cli"
+
+[tool.setuptools.dynamic]
+version = {attr = "package.__version__"}
```

### Comparing `pixe-0.5.6/tests/test_integration.py` & `pixe-0.7.0/tests/test_integration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import pathlib
-import os
 import datetime
 
 import pytest
 from click.testing import CliRunner
-import piexif
 
 import pixe
+import filetypes
 
 
 @pytest.fixture
 def runner():
     return CliRunner()
 
 
 @pytest.fixture
+def pixe_file():
+    return filetypes.factory
+
+
+@pytest.fixture
 def src_file(src_path):
     return src_path.joinpath("red.jpg")
 
 
 def test_single_file(runner, src_file, dst_path):
     dest_file = pathlib.Path(dst_path).joinpath(
-        "2020", "3", "20200321_031312_1cdef99be68dbdea159ec6fa8469b41ca13e9e6f.jpg"
+        "2020", "03-Mar", "20200321_031312_1cdef99be68dbdea159ec6fa8469b41ca13e9e6f.jpg"
     )
 
     results = runner.invoke(pixe.cli, f"--dest {dst_path} {src_file}")
 
     assert results.exit_code == 0
     assert dest_file.exists()
 
@@ -38,74 +42,78 @@
 
 def test_single_file_bad(runner, dst_path):
     results = runner.invoke(pixe.cli, f"--dest {dst_path} /dev/zero")
 
     assert results.exit_code == 2
 
 
+@pytest.mark.freeze_time(datetime.datetime.now())
 def test_single_file_duplicate(runner, src_file, dst_path):
     import_time = datetime.datetime.now()
     dest_file = dst_path.joinpath(
         "dups",
         import_time.strftime("%Y%m%d_%H%M%S"),
         "2020",
-        "3",
         "20200321_031312_1cdef99be68dbdea159ec6fa8469b41ca13e9e6f.jpg",
     )
     runner.invoke(pixe.cli, f"--dest {dst_path} {src_file}")
     results = runner.invoke(pixe.cli, f"--dest {dst_path} {src_file}")
 
     assert results.exit_code == 0
     assert dest_file.exists()
 
 
 def test_single_file_move(runner, src_file, dst_path):
-    dest_file = dst_path.joinpath("2020", "3", "20200321_031312_1cdef99be68dbdea159ec6fa8469b41ca13e9e6f.jpg")
+    dest_file = dst_path.joinpath("2020", "03-Mar", "20200321_031312_1cdef99be68dbdea159ec6fa8469b41ca13e9e6f.jpg")
 
     results = runner.invoke(pixe.cli, f"--move --dest {dst_path} {src_file}")
 
     assert results.exit_code == 0
     assert dest_file.exists()
     assert not src_file.exists()
 
 
 def test_single_file_copy_tagged(runner, src_path, dst_path):
     src_file = src_path.joinpath("dark/darkturquoise.jpg")
-    dest_file = dst_path.joinpath("2020", "12", "20201209_015501_a810b8552a4acf4e13164a74aab3016e583cc93e.jpg")
-    old_checksum = dest_file.stem.split("_")[2]
+    dst_file = dst_path.joinpath("2020", "12-Dec", "20201209_015501_a810b8552a4acf4e13164a74aab3016e583cc93e.jpg")
+    src_file_obj = filetypes.factory.get_file_obj(src_file)
+    dst_file_obj = filetypes.factory.get_file_obj(dst_file)
 
     results = runner.invoke(
         pixe.cli, f"--copy --owner 'Joe User' --copyright 'Copyright 2020 Joe User.' --dest {dst_path} {src_file}"
     )
-    src_exif = piexif.load(str(src_file))
-    dst_exif = piexif.load(str(dest_file))
-    new_checksum = pixe._calc_checksum(dest_file)
+    src_exif = src_file_obj.metadata
+    dst_exif = dst_file_obj.metadata
+    old_checksum = src_file_obj.checksum
+    new_checksum = dst_file_obj.checksum
 
     assert results.exit_code == 0
-    assert dest_file.exists()
+    assert dst_file.exists()
     assert src_exif != dst_exif
     assert dst_exif["Exif"][0xA430] == b"Joe User"
-    assert dst_exif["0th"][piexif.ImageIFD.Copyright] == b"Copyright 2020 Joe User."
+    assert dst_exif["0th"][33432] == b"Copyright 2020 Joe User."
     assert old_checksum == new_checksum
 
 
-def test_files_parallel(runner, src_path, dst_path):
-    results = runner.invoke(pixe.cli, f"--dest {dst_path} {src_path}")
-
-    assert results.exit_code == 0
-    assert dst_path.joinpath("2021", "12", "20211222_153825_d05cae67991384d221e95ae8b30994ce186695ed.jpg").exists()
-
-
-def test_files_serial(runner, src_path, dst_path):
-    results = runner.invoke(pixe.cli, f"--serial --dest {dst_path} {src_path}")
-
-    assert results.exit_code == 0
-    assert dst_path.joinpath("2021", "12", "20211222_153825_d05cae67991384d221e95ae8b30994ce186695ed.jpg").exists()
-
-
-def test_files_recurse(runner, src_path, dst_path):
-    results = runner.invoke(pixe.cli, f"--recurse --dest {dst_path} {src_path}")
-
-    assert results.exit_code == 0
-    assert dst_path.joinpath("2022", "2", "20220226_001821_476bf667385499407e1405f5909f88875dab1873.jpg").exists()
-    assert dst_path.joinpath("2018", "3", "20180319_100139_b78473e5c10d8fd945dd1eee9da7a82320d464d1.jpg").exists()
-    assert dst_path.joinpath("2021", "12", "20211222_153825_d05cae67991384d221e95ae8b30994ce186695ed.jpg").exists()
+# def test_files_parallel(runner, src_path, dst_path):
+#     # src_files = src_path.joinpath('light')
+#     results = runner.invoke(pixe.cli, f"--move --dest {dst_path} {src_files}")
+#
+#     assert results.exit_code == 0
+#     assert dst_path.joinpath("2021", "12", "20211222_153825_d05cae67991384d221e95ae8b30994ce186695ed.jpg").exists()
+#
+#
+# def test_files_serial(runner, src_path, dst_path):
+#     src_files = src_path.joinpath('light')
+#     results = runner.invoke(pixe.cli, f"--serial --move --dest {dst_path} {src_files}")
+#
+#     assert results.exit_code == 0
+#     assert dst_path.joinpath("2021", "12", "20211222_153825_d05cae67991384d221e95ae8b30994ce186695ed.jpg").exists()
+#
+#
+# def test_files_recurse(runner, src_path, dst_path):
+#     results = runner.invoke(pixe.cli, f"--recurse --move --dest {dst_path} {src_path}")
+#
+#     assert results.exit_code == 0
+#     assert dst_path.joinpath("2022", "2", "20220226_001821_476bf667385499407e1405f5909f88875dab1873.jpg").exists()
+#     assert dst_path.joinpath("2018", "3", "20180319_100139_b78473e5c10d8fd945dd1eee9da7a82320d464d1.jpg").exists()
+#     assert dst_path.joinpath("2021", "12", "20211222_153825_d05cae67991384d221e95ae8b30994ce186695ed.jpg").exists()
```

### Comparing `pixe-0.5.6/tests/test_unit.py` & `pixe-0.7.0/tests/test_unit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,80 @@
 import pathlib
 import datetime
-import os
 
 import pytest
 import piexif
 
 import pixe
+import filetypes
 
 
 @pytest.fixture
-def src_file(src_path):
-    return src_path.joinpath("red.jpg")
+def src_img_file(src_path):
+    return filetypes.factory.get_file_obj(src_path.joinpath("red.jpg"))
 
 
-def test_calc_checksum(src_file):
+@pytest.fixture
+def src_img_file_path(src_path):
+    return pathlib.Path(src_path.joinpath("red.jpg"))
+
+
+def test_img_file_checksum(src_img_file):
     expected_checksum = "1cdef99be68dbdea159ec6fa8469b41ca13e9e6f"
 
-    calculated_checksum = pixe._calc_checksum(src_file)
+    calculated_checksum = src_img_file.checksum
 
     assert expected_checksum == calculated_checksum
 
 
-def test_extract_date(src_file):
+def test_img_file_create_date(src_img_file):
     expected_date = datetime.datetime(2020, 3, 21, 3, 13, 12)
 
-    extracted_date = pixe._extract_date(src_file)
+    extracted_date = src_img_file.creation_date
 
     assert expected_date == extracted_date
 
 
-def test_new_tag_owner(src_file):
-    path_str = str(src_file)
+def test_img_file_add_metadata_owner(src_img_file_path):
+    path_str = str(src_img_file_path)
     orig_exif = piexif.load(path_str)
+    file_obj = filetypes.factory.get_file_obj(src_img_file_path)
 
-    new_exif = piexif.load(pixe._new_tags(src_file, owner="Joe User"))
+    file_obj.add_metadata(src_img_file_path, owner='Joe User')
+    new_exif = piexif.load(str(src_img_file_path))
 
     assert orig_exif != new_exif
     assert new_exif["Exif"][0xa430] == b"Joe User"
 
 
-def test_new_tag_copyright(src_file):
-    path_str = str(src_file)
+def test_img_file_add_metadata_copyright(src_img_file_path):
+    path_str = str(src_img_file_path)
     orig_exif = piexif.load(path_str)
+    file_obj = filetypes.factory.get_file_obj(src_img_file_path)
 
-    new_exif = piexif.load(
-        pixe._new_tags(src_file, copyright="Copyright 2023 Joe User.")
-    )
+    file_obj.add_metadata(src_img_file_path, copyright='Copyright 2023 Joe User.')
+    new_exif = piexif.load(str(src_img_file_path))
 
     assert orig_exif != new_exif
     assert new_exif["0th"][piexif.ImageIFD.Copyright] == b"Copyright 2023 Joe User."
 
 
-def test_process_file(src_file, dst_path):
+def test_process_file(src_img_file, dst_path):
     expected_file = pathlib.Path(dst_path).joinpath(
-        "2020", "3", "20200321_031312_1cdef99be68dbdea159ec6fa8469b41ca13e9e6f.jpg"
+        "2020", "03-Mar", "20200321_031312_1cdef99be68dbdea159ec6fa8469b41ca13e9e6f.jpg"
     )
 
-    pixe._process_file(src_file, dst_path)
+    pixe.process_file(src_img_file, dst_path)
 
     assert expected_file.exists()
 
 
-def test_process_file_no_date(src_path, dst_path):
+def test_process_img_file_no_date(src_path, dst_path):
     src_file = src_path.joinpath("chocolate.jpg")
     new_file = pathlib.Path(dst_path).joinpath(
-        "1902", "2", "19020220_000000_2a00d2b48e39f63cf834d4f7c50b2c1aa3b43a9c.jpg"
+        "1902", "02-Feb", "19020220_000000_2a00d2b48e39f63cf834d4f7c50b2c1aa3b43a9c.jpg"
     )
+    test_file = filetypes.image_file.ImageFile(src_file)
 
-    pixe._process_file(src_file, dst_path)
+    pixe.process_file(test_file, dst_path)
 
     assert new_file.exists()
```

