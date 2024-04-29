# Comparing `tmp/copykitten-1.1.1.tar.gz` & `tmp/copykitten-1.2.0.tar.gz`

## Comparing `copykitten-1.1.1.tar` & `copykitten-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 copykitten-1.1.1/Cargo.toml
--rw-r--r--   0     1001      127       57 2024-02-20 11:21:49.000000 copykitten-1.1.1/.flake8
--rw-r--r--   0     1001      127     5267 2024-02-20 11:21:49.000000 copykitten-1.1.1/.github/workflows/build-test.yml
--rw-r--r--   0     1001      127      339 2024-02-20 11:21:49.000000 copykitten-1.1.1/.github/workflows/lint.yml
--rw-r--r--   0     1001      127      955 2024-02-20 11:21:49.000000 copykitten-1.1.1/.github/workflows/publish.yml
--rw-r--r--   0     1001      127      686 2024-02-20 11:21:49.000000 copykitten-1.1.1/.gitignore
--rw-r--r--   0     1001      127     1897 2024-02-20 11:21:49.000000 copykitten-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0     1001      127      661 2024-02-20 11:21:49.000000 copykitten-1.1.1/CHANGELOG.md
--rw-r--r--   0     1001      127     1071 2024-02-20 11:21:49.000000 copykitten-1.1.1/LICENSE
--rw-r--r--   0     1001      127     3750 2024-02-20 11:21:49.000000 copykitten-1.1.1/README.md
--rw-r--r--   0     1001      127      172 2024-02-20 11:21:49.000000 copykitten-1.1.1/python/copykitten/__init__.py
--rw-r--r--   0     1001      127     1904 2024-02-20 11:21:49.000000 copykitten-1.1.1/python/copykitten/_copykitten.pyi
--rw-r--r--   0     1001      127        0 2024-02-20 11:21:49.000000 copykitten-1.1.1/python/copykitten/py.typed
--rw-r--r--   0     1001      127       50 2024-02-20 11:21:49.000000 copykitten-1.1.1/requirements-dev.txt
--rw-r--r--   0     1001      127     2364 2024-02-20 11:21:49.000000 copykitten-1.1.1/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-02-20 11:21:49.000000 copykitten-1.1.1/tests/__init__.py
--rw-r--r--   0     1001      127     3505 2024-02-20 11:21:49.000000 copykitten-1.1.1/tests/clipboard.py
--rw-r--r--   0     1001      127     2065 2024-02-20 11:21:49.000000 copykitten-1.1.1/tests/conftest.py
--rw-r--r--   0     1001      127     2204 2024-02-20 11:21:49.000000 copykitten-1.1.1/tests/test_lib.py
--rw-r--r--   0     1001      127     2783 2024-02-20 11:21:49.000000 copykitten-1.1.1/tests/utils.py
--rw-r--r--   0     1001      127    17889 2024-02-20 11:21:49.000000 copykitten-1.1.1/Cargo.lock
--rw-r--r--   0     1001      127     1180 2024-02-20 11:21:49.000000 copykitten-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 copykitten-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 copykitten-1.2.0/Cargo.toml
+-rw-r--r--   0     1001      127       57 2024-04-29 20:32:28.000000 copykitten-1.2.0/.flake8
+-rw-r--r--   0     1001      127     5263 2024-04-29 20:32:28.000000 copykitten-1.2.0/.github/workflows/build-test.yml
+-rw-r--r--   0     1001      127      339 2024-04-29 20:32:28.000000 copykitten-1.2.0/.github/workflows/lint.yml
+-rw-r--r--   0     1001      127      955 2024-04-29 20:32:28.000000 copykitten-1.2.0/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      686 2024-04-29 20:32:28.000000 copykitten-1.2.0/.gitignore
+-rw-r--r--   0     1001      127     1996 2024-04-29 20:32:28.000000 copykitten-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0     1001      127      727 2024-04-29 20:32:28.000000 copykitten-1.2.0/CHANGELOG.md
+-rw-r--r--   0     1001      127     1071 2024-04-29 20:32:28.000000 copykitten-1.2.0/LICENSE
+-rw-r--r--   0     1001      127     3750 2024-04-29 20:32:28.000000 copykitten-1.2.0/README.md
+-rw-r--r--   0     1001      127      172 2024-04-29 20:32:28.000000 copykitten-1.2.0/python/copykitten/__init__.py
+-rw-r--r--   0     1001      127     1904 2024-04-29 20:32:28.000000 copykitten-1.2.0/python/copykitten/_copykitten.pyi
+-rw-r--r--   0     1001      127        0 2024-04-29 20:32:28.000000 copykitten-1.2.0/python/copykitten/py.typed
+-rw-r--r--   0     1001      127       50 2024-04-29 20:32:28.000000 copykitten-1.2.0/requirements-dev.txt
+-rw-r--r--   0     1001      127     2364 2024-04-29 20:32:28.000000 copykitten-1.2.0/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-29 20:32:28.000000 copykitten-1.2.0/tests/__init__.py
+-rw-r--r--   0     1001      127     4390 2024-04-29 20:32:28.000000 copykitten-1.2.0/tests/clipboard.py
+-rw-r--r--   0     1001      127      866 2024-04-29 20:32:28.000000 copykitten-1.2.0/tests/conftest.py
+-rw-r--r--   0     1001      127     2190 2024-04-29 20:32:28.000000 copykitten-1.2.0/tests/test_lib.py
+-rw-r--r--   0     1001      127    19375 2024-04-29 20:32:28.000000 copykitten-1.2.0/Cargo.lock
+-rw-r--r--   0     1001      127     1261 2024-04-29 20:32:28.000000 copykitten-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 copykitten-1.2.0/PKG-INFO
```

### Comparing `copykitten-1.1.1/.github/workflows/build-test.yml` & `copykitten-1.2.0/.github/workflows/build-test.yml`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         uses: actions/upload-artifact@v4
         with:
           name: wheels-${{ runner.os }}
           path: dist
 
   macos:
     name: Build & test on MacOS
-    runs-on: macos-latest
+    runs-on: macos-12
     strategy:
       matrix:
         # If this workflow is called to build for release, build for x64 and ARM64
         # processors. However, run tests only for x64, as GH doesn't provide
         # ARM64 runners.
         target: ${{ inputs.release && fromJSON('["x64", "aarch64"]') || fromJSON('["x64"]') }}
         # If this workflow is called to build for release, build using
```

### Comparing `copykitten-1.1.1/.github/workflows/publish.yml` & `copykitten-1.2.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `copykitten-1.1.1/.gitignore` & `copykitten-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `copykitten-1.1.1/.pre-commit-config.yaml` & `copykitten-1.2.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -87,7 +87,12 @@
       - id: isort
         name: isort-check
         args:
           - --check-only
         stages:
           - manual
         types: [python]
+
+  - repo: https://github.com/jendrikseipp/vulture
+    rev: 'v2.11'
+    hooks:
+      - id: vulture
```

### Comparing `copykitten-1.1.1/CHANGELOG.md` & `copykitten-1.2.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+# [1.2.0] - 2024-04-29
+### Changed
+- Update `arboard` to 3.4.0. 
+
 ## [1.1.1] - 2024-02-20
 ### Fixed
 - Fix `paste_image` return type.
 
 ## [1.1.0] - 2024-02-19
 ### Added
 - Added support for image copying/pasting with `copy_image`/`paste_image` functions.
```

### Comparing `copykitten-1.1.1/LICENSE` & `copykitten-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `copykitten-1.1.1/README.md` & `copykitten-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `copykitten-1.1.1/python/copykitten/_copykitten.pyi` & `copykitten-1.2.0/python/copykitten/_copykitten.pyi`

 * *Files identical despite different names*

### Comparing `copykitten-1.1.1/src/lib.rs` & `copykitten-1.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `copykitten-1.1.1/tests/clipboard.py` & `copykitten-1.2.0/tests/clipboard.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,47 @@
 import io
 import subprocess
+import sys
 import tempfile
 from pathlib import Path
-from typing import Callable
+from typing import Callable, Generic, TypeVar, cast
 
 from PIL import Image
 
 ReadClipboard = Callable[[], str]
 WriteClipboard = Callable[[str], None]
 ReadClipboardImage = Callable[[], Image.Image]
 WriteClipboardImage = Callable[[Image.Image], None]
 
+T = TypeVar("T")
+
+
+class Resolver(Generic[T]):
+    platform_mapping = {"win32": "win", "linux": "linux", "darwin": "macos"}
+
+    def __set_name__(self, _, name):
+        self.action = name
+
+    def __get__(self, _, __) -> T:
+        variables = globals()
+        platform = self.platform_mapping[sys.platform]
+        function_name = f"{self.action}_{platform}"
+
+        try:
+            return cast(T, variables[function_name])
+        except KeyError:
+            raise RuntimeError(f"Cannot find suitable clipboard for {sys.platform}.")
+
+
+class Clipboard:
+    read = Resolver[ReadClipboard]()
+    write = Resolver[WriteClipboard]()
+    read_image = Resolver[ReadClipboardImage]()
+    write_image = Resolver[WriteClipboardImage]()
+
 
 def read_macos() -> str:
     return subprocess.check_output("pbpaste").decode().strip()
 
 
 def write_macos(content: str) -> None:
     subprocess.run("pbcopy", input=content, text=True)
@@ -57,46 +84,53 @@
     # null bytes to the content.
     subprocess.check_call(("powershell.exe", "Set-Clipboard", content))
 
 
 def read_image_win() -> Image.Image:
     tmp_dir = tempfile.gettempdir()
     tmp_file = Path(tmp_dir) / "pasted_image.png"
-    subprocess.run((
-        "powershell.exe",
-        "Add-Type",
-        "-Assembly",
-        "System.Drawing,",
-        "System.Windows.Forms;",
-        "[System.Windows.Forms.Clipboard]::GetImage().Save(\"%s\")" % tmp_file
-    ), check=True)
+    subprocess.run(
+        (
+            "powershell.exe",
+            "Add-Type",
+            "-Assembly",
+            "System.Drawing,",
+            "System.Windows.Forms;",
+            '[System.Windows.Forms.Clipboard]::GetImage().Save("%s")' % tmp_file,
+        ),
+        check=True,
+    )
 
     try:
         img = Image.open(tmp_file)
         img.load()
     finally:
         tmp_file.unlink()
 
     return img
 
 
 def write_image_win(img: Image.Image) -> None:
     tmp_dir = tempfile.gettempdir()
-    tmp_file = Path(tmp_dir) / f"copied_image.png"
+    tmp_file = Path(tmp_dir) / "copied_image.png"
 
     try:
         img.save(tmp_file)
-        subprocess.run((
+        subprocess.run(
+            (
                 "powershell.exe",
                 "Add-Type",
                 "-Assembly",
                 "System.Drawing,",
                 "System.Windows.Forms;",
-                "[System.Windows.Forms.Clipboard]::SetImage([System.Drawing.Image]::FromFile(\"%s\"))" % tmp_file
-            ), check=True)
+                '[System.Windows.Forms.Clipboard]::SetImage([System.Drawing.Image]::FromFile("%s"))'
+                % tmp_file,
+            ),
+            check=True,
+        )
     finally:
         tmp_file.unlink()
 
 
 def read_linux() -> str:
     return subprocess.check_output(("xclip", "-sel", "clipboard", "-o")).decode()
 
@@ -111,9 +145,11 @@
     return Image.open(buffer, formats=["png"])
 
 
 def write_image_linux(img: Image.Image) -> None:
     buffer = io.BytesIO()
     img.save(buffer, format="png")
     subprocess.run(
-        ("xclip", "-sel", "clipboard", "-i", "-target", "image/png"), input=buffer.getvalue(), check=True
+        ("xclip", "-sel", "clipboard", "-i", "-target", "image/png"),
+        input=buffer.getvalue(),
+        check=True,
     )
```

### Comparing `copykitten-1.1.1/tests/test_lib.py` & `copykitten-1.2.0/tests/test_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import sys
-from io import BytesIO
 from time import sleep
 
 import pytest
 from PIL import Image
 
 import copykitten
 from tests.clipboard import (
@@ -45,14 +44,15 @@
 
 @pytest.mark.repeat(ITERATIONS)
 def test_clear(read_clipboard: ReadClipboard, write_clipboard: WriteClipboard):
     write_clipboard("text")
     sleep(SLEEP_TIME)
     copykitten.clear()
     sleep(SLEEP_TIME)
+
     actual = read_clipboard()
 
     assert actual == ""
 
 
 @pytest.mark.repeat(ITERATIONS)
 def test_paste_text(write_clipboard: WriteClipboard):
@@ -64,21 +64,25 @@
     assert actual == "text"
 
 
 def test_copy_image(test_image: Image.Image, read_clipboard_image: ReadClipboardImage):
     test_image_bytes = test_image.tobytes()
     copykitten.copy_image(test_image_bytes, test_image.width, test_image.height)
     sleep(SLEEP_TIME)
+
     pasted_image = read_clipboard_image()
 
     assert test_image_bytes == pasted_image.tobytes()
 
 
-@pytest.mark.skipif(sys.platform == "win32", reason="No way to reliably assert result on Windows yet")
+@pytest.mark.skipif(
+    sys.platform == "win32", reason="No way to reliably assert result on Windows yet"
+)
 def test_paste_image(test_image: Image.Image, write_clipboard_image: WriteClipboardImage):
     write_clipboard_image(test_image)
     sleep(SLEEP_TIME)
+
     pasted_image, width, height = copykitten.paste_image()
 
     assert test_image.tobytes() == pasted_image
     assert width == test_image.width
     assert height == test_image.height
```

### Comparing `copykitten-1.1.1/Cargo.lock` & `copykitten-1.2.0/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,27 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "arboard"
-version = "3.3.0"
+version = "3.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aafb29b107435aa276664c1db8954ac27a6e105cdad3c88287a199eb0e313c08"
+checksum = "9fb4009533e8ff8f1450a5bcbc30f4242a1d34442221f72314bea1f5dc9c7f89"
 dependencies = [
  "clipboard-win",
  "core-graphics",
  "image",
  "log",
- "objc",
- "objc-foundation",
- "objc_id",
+ "objc2",
+ "objc2-app-kit",
+ "objc2-foundation",
  "parking_lot",
- "thiserror",
- "winapi",
+ "windows-sys 0.48.0",
  "x11rb",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -36,24 +35,33 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
-name = "block"
-version = "0.1.6"
+name = "bitflags"
+version = "2.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+
+[[package]]
+name = "block2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d8c1fef690941d3e7788d328517591fecc684c084084702d6ff1641e993699a"
+checksum = "43ff7d91d3c1d568065b06c899777d1e48dcf76103a672a0adbc238a7f247f1e"
+dependencies = [
+ "objc2",
+]
 
 [[package]]
 name = "bytemuck"
-version = "1.14.0"
+version = "1.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "374d28ec25809ee0e23827c2ab573d729e293f281dfe393500e7ad618baa61c6"
+checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
@@ -61,101 +69,99 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clipboard-win"
-version = "4.5.0"
+version = "5.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7191c27c2357d9b7ef96baac1773290d4ca63b24205b82a3fd8a0637afcf0362"
+checksum = "79f4473f5144e20d9aceaf2972478f06ddf687831eafeeb434fbaf0acc4144ad"
 dependencies = [
  "error-code",
- "str-buf",
- "winapi",
 ]
 
 [[package]]
-name = "color_quant"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
-
-[[package]]
 name = "copykitten"
-version = "1.1.1"
+version = "1.2.0"
 dependencies = [
  "arboard",
  "pyo3",
 ]
 
 [[package]]
 name = "core-foundation"
-version = "0.9.3"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "core-graphics"
-version = "0.22.3"
+version = "0.23.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2581bbab3b8ffc6fcbd550bf46c355135d16e9ff2a6ea032ad6b9bf1d7efe4fb"
+checksum = "970a29baf4110c26fedbc7f82107d42c23f7e88e404c4577ed73fe99ff85a212"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "core-foundation",
  "core-graphics-types",
  "foreign-types",
  "libc",
 ]
 
 [[package]]
 name = "core-graphics-types"
-version = "0.1.2"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2bb142d41022986c1d8ff29103a1411c8a3dfad3552f87a4f8dc50d61d4f4e33"
+checksum = "45390e6114f68f718cc7a830514a96f903cccd70d02a8f6d9f643ac4ba45afaf"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "core-foundation",
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
-name = "error-code"
-version = "2.3.1"
+name = "errno"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64f18991e7bf11e7ffee451b5318b5c1a73c52d0d0ada6e5a3017c8c1ced6a21"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
- "str-buf",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "error-code"
+version = "3.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a0474425d51df81997e2f90a21591180b38eccf27292d755f3e30750225c175b"
+
+[[package]]
 name = "fdeflate"
-version = "0.3.1"
+version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64d6dafc854908ff5da46ff3f8f473c6984119a2876a383a860246dd7841a868"
+checksum = "4f9bfee30e4dedf0ab8b422f03af778d9612b63f502710fc500a334ebe2de645"
 dependencies = [
  "simd-adler32",
 ]
 
 [[package]]
 name = "flate2"
 version = "1.0.28"
@@ -164,205 +170,196 @@
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "foreign-types"
-version = "0.3.2"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
+checksum = "d737d9aa519fb7b749cbc3b962edcf310a8dd1f4b67c91c4f83975dbdd17d965"
 dependencies = [
+ "foreign-types-macros",
  "foreign-types-shared",
 ]
 
 [[package]]
+name = "foreign-types-macros"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a5c6c585bc94aaf2c7b51dd4c2ba22680844aba4c687be581871a6f518c5742"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn",
+]
+
+[[package]]
 name = "foreign-types-shared"
-version = "0.1.1"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
+checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
 
 [[package]]
 name = "gethostname"
-version = "0.3.0"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb65d4ba3173c56a500b555b532f72c42e8d1fe64962b518897f8959fae2c177"
+checksum = "0176e0459c2e4a1fe232f984bca6890e681076abb9934f6cea7c326f3fc47818"
 dependencies = [
  "libc",
- "winapi",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "image"
-version = "0.24.7"
+version = "0.25.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f3dfdbdd72063086ff443e297b61695500514b1e41095b6fb9a5ab48a70a711"
+checksum = "fd54d660e773627692c524beaad361aca785a4f9f5730ce91f42aabe5bce3d11"
 dependencies = [
  "bytemuck",
  "byteorder",
- "color_quant",
- "num-rational",
  "num-traits",
  "png",
  "tiff",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
 
 [[package]]
 name = "jpeg-decoder"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc0000e42512c92e31c2252315bda326620a4e034105e900c98ec492fa077b3e"
+checksum = "f5d4a7da358eff58addd2877a45865158f0d78c911d43a5784ceb7bbf52833b0"
 
 [[package]]
 name = "libc"
-version = "0.2.150"
+version = "0.2.153"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+
+[[package]]
+name = "linux-raw-sys"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
-
-[[package]]
-name = "malloc_buf"
-version = "0.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62bb907fe88d54d8d9ce32a3cceab4218ed2f6b7d35617cafe9adf84e43919cb"
-dependencies = [
- "libc",
-]
-
-[[package]]
-name = "memoffset"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
-dependencies = [
- "autocfg",
-]
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
  "simd-adler32",
 ]
 
 [[package]]
-name = "nix"
-version = "0.26.4"
+name = "num-traits"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "598beaf3cc6fdd9a5dfb1630c2800c7acd31df7aaf0f565796fba2b53ca1af1b"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
- "bitflags",
- "cfg-if",
- "libc",
- "memoffset 0.7.1",
+ "autocfg",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
+name = "objc-sys"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
+checksum = "da284c198fb9b7b0603f8635185e85fbd5b64ee154b1ed406d489077de2d6d60"
 
 [[package]]
-name = "num-rational"
-version = "0.4.1"
+name = "objc2"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "b4b25e1034d0e636cd84707ccdaa9f81243d399196b8a773946dcffec0401659"
 dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
+ "objc-sys",
+ "objc2-encode",
 ]
 
 [[package]]
-name = "num-traits"
-version = "0.2.17"
+name = "objc2-app-kit"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "fb79768a710a9a1798848179edb186d1af7e8a8679f369e4b8d201dd2a034047"
 dependencies = [
- "autocfg",
+ "block2",
+ "objc2",
+ "objc2-core-data",
+ "objc2-foundation",
 ]
 
 [[package]]
-name = "objc"
-version = "0.2.7"
+name = "objc2-core-data"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "915b1b472bc21c53464d6c8461c9d3af805ba1ef837e1cac254428f4a77177b1"
+checksum = "6e092bc42eaf30a08844e6a076938c60751225ec81431ab89f5d1ccd9f958d6c"
 dependencies = [
- "malloc_buf",
+ "block2",
+ "objc2",
+ "objc2-foundation",
 ]
 
 [[package]]
-name = "objc-foundation"
-version = "0.1.1"
+name = "objc2-encode"
+version = "4.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1add1b659e36c9607c7aab864a76c7a4c2760cd0cd2e120f3fb8b952c7e22bf9"
-dependencies = [
- "block",
- "objc",
- "objc_id",
-]
+checksum = "88658da63e4cc2c8adb1262902cd6af51094df0488b760d6fd27194269c0950a"
 
 [[package]]
-name = "objc_id"
-version = "0.1.1"
+name = "objc2-foundation"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c92d4ddb4bd7b50d730c215ff871754d0da6b2178849f8a2a2ab69712d0c073b"
+checksum = "cfaefe14254871ea16c7d88968c0ff14ba554712a20d76421eec52f0a7fb8904"
 dependencies = [
- "objc",
+ "block2",
+ "objc2",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
@@ -376,116 +373,137 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "png"
-version = "0.17.10"
+version = "0.17.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd75bf2d8dd3702b9707cdbc56a5b9ef42cec752eb8b3bafc01234558442aa64"
+checksum = "06e4b0d3d1312775e782c86c91a111aa1f910cbb65e1337f9975b5f9a554b5e1"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "crc32fast",
  "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.70"
+version = "1.0.78"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39278fbbf5fb4f646ce651690877f89d1c5811a3d4acb27700c1cb3cdb78fd3b"
+checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04e8453b658fe480c3e70c8ed4e3d3ec33eb74988bd186561b0cc66b85c3bc4b"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.9.0",
+ "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a96fe70b176a89cff78f2fa7b3c930081e163d5379b4dcdf993e3ae29ca662e5"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "214929900fd25e6604661ed9cf349727c8920d47deff196c4e28165a6ef2a96b"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dac53072f717aa1bfa4db832b39de8c875b7c7af4f4a6fe93cdbf9264cf8383b"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7774b5a8282bd4f25f803b1f0d945120be959a36c72e08e7cd031c792fdfd424"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "rustix"
+version = "0.38.31"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6ea3e1a662af26cd7a3ba09c0297a31af215563ecf42817c98df621387f4e949"
+dependencies = [
+ "bitflags 2.4.2",
+ "errno",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
@@ -494,66 +512,40 @@
 name = "simd-adler32"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d66dc143e6b11c1eddc06d5c423cfc97062865baf299914ab64caa38182078fe"
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
-
-[[package]]
-name = "str-buf"
-version = "1.0.6"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e08d8363704e6c71fc928674353e6b7c23dcea9d82d7012c8faf2a3a025f8d0"
+checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
 
 [[package]]
 name = "syn"
-version = "2.0.39"
+version = "2.0.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23e78b90f2fcf45d3e842032ce32e3f2d1545ba6636271dcbf24fa306d87be7a"
+checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
-
-[[package]]
-name = "thiserror"
-version = "1.0.50"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a7210f5c9a7156bb50aa36aed4c95afb51df0df00713949448cf9e97d382d2"
-dependencies = [
- "thiserror-impl",
-]
-
-[[package]]
-name = "thiserror-impl"
-version = "1.0.50"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266b2e40bc00e5a6c09c3584011e08b06f123c00362c92b975ba9843aaaa14b8"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tiff"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d172b0f4d3fba17ba89811858b9d3d97f928aece846475bbda076ca46736211"
+checksum = "ba1310fcea54c6a9a4fd1aad794ecc02c31682f6bfbecdf460bf19533eed1e3e"
 dependencies = [
  "flate2",
  "jpeg-decoder",
  "weezl",
 ]
 
 [[package]]
@@ -566,120 +558,159 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "weezl"
-version = "0.1.7"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9193164d4de03a926d909d3bc7c30543cecb35400c02114792c2cae20d5e2dbb"
+checksum = "53a85b86a771b1c87058196170769dd264f66c0782acf1ae6cc51bfd64b39082"
 
 [[package]]
-name = "winapi"
-version = "0.3.9"
+name = "windows-sys"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
-name = "winapi-wsapoll"
-version = "0.1.1"
+name = "windows-sys"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44c17110f57155602a80dca10be03852116403c9ff3cd25b079d666f2aa3df6e"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "winapi",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
+name = "windows-targets"
+version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
 
 [[package]]
 name = "windows-targets"
-version = "0.48.5"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+
+[[package]]
 name = "x11rb"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1641b26d4dec61337c35a1b1aaf9e3cba8f46f0b43636c609ab0291a648040a"
+checksum = "f8f25ead8c7e4cba123243a6367da5d3990e0d3affa708ea19dce96356bd9f1a"
 dependencies = [
  "gethostname",
- "nix",
- "winapi",
- "winapi-wsapoll",
+ "rustix",
  "x11rb-protocol",
 ]
 
 [[package]]
 name = "x11rb-protocol"
-version = "0.12.0"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82d6c3f9a0fb6701fab8f6cea9b0c0bd5d6876f1f89f7fada07e558077c344bc"
-dependencies = [
- "nix",
-]
+checksum = "e63e71c4b8bd9ffec2c963173a4dc4cbde9ee96961d4fcb4429db9929b606c34"
```

### Comparing `copykitten-1.1.1/pyproject.toml` & `copykitten-1.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -30,10 +30,14 @@
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
 
+[tool.vulture]
+paths = ["python", "tests"]
+ignore_names = ["read_*", "write_*"]
+
 [tool.maturin]
 python-source = "python"
 module-name = "copykitten._copykitten"
```

### Comparing `copykitten-1.1.1/PKG-INFO` & `copykitten-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: copykitten
-Version: 1.1.1
+Version: 1.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

