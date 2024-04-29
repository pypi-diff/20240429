# Comparing `tmp/setuptools_ext-0.7.tar.gz` & `tmp/setuptools_ext-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools_ext-0.7.tar", last modified: Mon Apr 29 02:03:21 2024, max compression
+gzip compressed data, was "setuptools_ext-0.8.tar", last modified: Mon Apr 29 08:17:03 2024, max compression
```

## Comparing `setuptools_ext-0.7.tar` & `setuptools_ext-0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 02:03:21.251917 setuptools_ext-0.7/
--rw-r--r--   0 wim        (501) staff       (20)     1066 2022-04-20 07:49:46.000000 setuptools_ext-0.7/LICENSE
--rw-r--r--   0 wim        (501) staff       (20)     9207 2024-04-29 02:03:21.251639 setuptools_ext-0.7/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)     8751 2024-04-17 23:32:21.000000 setuptools_ext-0.7/README.rst
--rw-r--r--   0 wim        (501) staff       (20)      564 2024-04-29 02:03:12.000000 setuptools_ext-0.7/pyproject.toml
--rw-r--r--   0 wim        (501) staff       (20)       38 2024-04-29 02:03:21.251967 setuptools_ext-0.7/setup.cfg
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 02:03:21.251356 setuptools_ext-0.7/setuptools_ext.egg-info/
--rw-r--r--   0 wim        (501) staff       (20)     9207 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)      269 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/SOURCES.txt
--rw-r--r--   0 wim        (501) staff       (20)        1 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/dependency_links.txt
--rw-r--r--   0 wim        (501) staff       (20)       53 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/requires.txt
--rw-r--r--   0 wim        (501) staff       (20)       15 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/top_level.txt
--rw-r--r--   0 wim        (501) staff       (20)     8174 2024-04-29 02:03:12.000000 setuptools_ext-0.7/setuptools_ext.py
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 02:03:21.250992 setuptools_ext-0.7/tests/
--rw-r--r--   0 wim        (501) staff       (20)     3614 2024-04-18 05:48:36.000000 setuptools_ext-0.7/tests/test_setuptools_ext.py
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 08:17:03.716151 setuptools_ext-0.8/
+-rw-r--r--   0 wim        (501) staff       (20)     1066 2022-04-20 07:49:46.000000 setuptools_ext-0.8/LICENSE
+-rw-r--r--   0 wim        (501) staff       (20)     9265 2024-04-29 08:17:03.715865 setuptools_ext-0.8/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)     8751 2024-04-17 23:32:21.000000 setuptools_ext-0.8/README.rst
+-rw-r--r--   0 wim        (501) staff       (20)      733 2024-04-29 08:15:29.000000 setuptools_ext-0.8/pyproject.toml
+-rw-r--r--   0 wim        (501) staff       (20)       38 2024-04-29 08:17:03.716204 setuptools_ext-0.8/setup.cfg
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 08:17:03.715583 setuptools_ext-0.8/setuptools_ext.egg-info/
+-rw-r--r--   0 wim        (501) staff       (20)     9265 2024-04-29 08:17:03.000000 setuptools_ext-0.8/setuptools_ext.egg-info/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)      269 2024-04-29 08:17:03.000000 setuptools_ext-0.8/setuptools_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 wim        (501) staff       (20)        1 2024-04-29 08:17:03.000000 setuptools_ext-0.8/setuptools_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 wim        (501) staff       (20)       99 2024-04-29 08:17:03.000000 setuptools_ext-0.8/setuptools_ext.egg-info/requires.txt
+-rw-r--r--   0 wim        (501) staff       (20)       15 2024-04-29 08:17:03.000000 setuptools_ext-0.8/setuptools_ext.egg-info/top_level.txt
+-rw-r--r--   0 wim        (501) staff       (20)     8830 2024-04-29 08:15:29.000000 setuptools_ext-0.8/setuptools_ext.py
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 08:17:03.715352 setuptools_ext-0.8/tests/
+-rw-r--r--   0 wim        (501) staff       (20)     4171 2024-04-29 08:15:29.000000 setuptools_ext-0.8/tests/test_setuptools_ext.py
```

### Comparing `setuptools_ext-0.7/LICENSE` & `setuptools_ext-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_ext-0.7/PKG-INFO` & `setuptools_ext-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: setuptools-ext
-Version: 0.7
+Version: 0.8
 Summary: Extension of setuptools to support all core metadata fields
 Author: Wim Glenn
 Author-email: hey@wimglenn.com
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/setuptools-ext
 Keywords: setuptools,packaging,metadata
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0.0
 Requires-Dist: tomli; python_version < "3.11"
+Requires-Dist: importlib_metadata; python_version < "3.8"
 
 |pypi|_ |actions|_ |codecov|_ |womm|_
 
 .. |pypi| image:: https://img.shields.io/pypi/v/setuptools-ext.svg
 .. _pypi: https://pypi.org/project/setuptools-ext
 
 .. |actions| image:: https://github.com/wimglenn/setuptools-ext/actions/workflows/tests.yml/badge.svg
```

### Comparing `setuptools_ext-0.7/README.rst` & `setuptools_ext-0.8/README.rst`

 * *Files identical despite different names*

### Comparing `setuptools_ext-0.7/setuptools_ext.egg-info/PKG-INFO` & `setuptools_ext-0.8/setuptools_ext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: setuptools-ext
-Version: 0.7
+Version: 0.8
 Summary: Extension of setuptools to support all core metadata fields
 Author: Wim Glenn
 Author-email: hey@wimglenn.com
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/setuptools-ext
 Keywords: setuptools,packaging,metadata
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: setuptools>=61.0.0
 Requires-Dist: tomli; python_version < "3.11"
+Requires-Dist: importlib_metadata; python_version < "3.8"
 
 |pypi|_ |actions|_ |codecov|_ |womm|_
 
 .. |pypi| image:: https://img.shields.io/pypi/v/setuptools-ext.svg
 .. _pypi: https://pypi.org/project/setuptools-ext
 
 .. |actions| image:: https://github.com/wimglenn/setuptools-ext/actions/workflows/tests.yml/badge.svg
```

### Comparing `setuptools_ext-0.7/setuptools_ext.py` & `setuptools_ext-0.8/setuptools_ext.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 from setuptools.build_meta import build_wheel as orig_build_wheel
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
+if sys.version_info >= (3, 8):
+    from importlib.metadata import version
+else:
+    from importlib_metadata import version
+
 
 allowed_fields = {
     x.lower(): x
     for x in [
         "Platform",
         "Supported-Platform",
         "Download-URL",
@@ -43,40 +48,49 @@
             continue
         if not isinstance(vals, list):
             t = type(vals).__name__
             print(f"WARNING: coercing the value of {key} from {t} to list")
             vals = [vals]
         extra_metadata[header] = vals
     whl = orig_build_wheel(wheel_directory, config_settings, metadata_directory)
-    if extra_metadata:
-        rewrite_whl(Path(wheel_directory) / whl, extra_metadata)
+    rewrite_whl(Path(wheel_directory) / whl, extra_metadata)
     return whl
 
 
 def rewrite_metadata(data, extra_metadata):
     """
     Rewrite the METADATA file to include the given additional metadata.
     """
-    pkginfo = email.message_from_string(data.decode())
+    pkginfo = email.message_from_bytes(data)
     # delete some annoying kv that distutils seems to put in there for no reason
     for key in dict(pkginfo):
         if pkginfo.get_all(key) == ["UNKNOWN"]:
             if key.lower() not in ["metadata-version", "name", "version"]:
                 del pkginfo[key]
     new_headers = extra_metadata.items()
     for key, vals in new_headers:
         already_present = pkginfo.get_all(key, [])
         for val in vals:
             if val not in already_present:
                 pkginfo.add_header(key, val)
-    policy = email.policy.Compat32(max_line_length=0)
+    policy = email.policy.EmailPolicy(refold_source="none")
     result = pkginfo.as_bytes(policy=policy)
     return result
 
 
+def rewrite_archive_metadata(orig_bytes):
+    lines = orig_bytes.splitlines()
+    for i, line in enumerate(lines):
+        if line.startswith(b"Generator: "):
+            suffix = b" + setuptools-ext (%s)"
+            line += suffix % version("setuptools-ext").encode()
+            lines[i] = line
+    return b"\n".join(lines) + b"\n"
+
+
 class WheelRecord:
     """
     Represents the RECORD file of a wheel, which can be updated with new checksums
     using the record_file method.
 
     See also the (limited) spec on RECORD at
     https://packaging.python.org/en/latest/specifications/binary-distribution-format/#signed-wheel-files
@@ -200,14 +214,20 @@
     # that's potentially a setuptools bug (seems like a PEP 517 violation), so it might
     # be changed later on, but unfortunately for now the only option is to rewrite the
     # generated .whl with our modifications
     tmppath = path.parent.joinpath("." + path.name)
 
     with zipfile.ZipFile(str(path), "r") as whl_zip:
         whl = WheelModifier(whl_zip)
+
         metadata_filename = f"{whl.dist_info_dirname()}/METADATA"
         metadata = rewrite_metadata(whl.read(metadata_filename), extra_metadata)
         whl.write(metadata_filename, metadata)
+
+        archive_metadata_filename = f"{whl.dist_info_dirname()}/WHEEL"
+        archive_metadata = rewrite_archive_metadata(whl.read(archive_metadata_filename))
+        whl.write(archive_metadata_filename, archive_metadata)
+
         with tmppath.open("wb") as whl_fh:
             whl.write_wheel(whl_fh)
 
     shutil.move(tmppath, path)
```

