# Comparing `tmp/pyproject_hooks-1.0.0.tar.gz` & `tmp/pyproject_hooks-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_hooks-1.0.0.tar", last modified: Mon Nov 21 11:52:09 2022, max compression
+gzip compressed data, was "pyproject_hooks-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyproject_hooks-1.0.0.tar` & `pyproject_hooks-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,8 @@
--rw-r--r--   0        0        0      115 2022-11-21 11:34:48.350629 pyproject_hooks-1.0.0/.bumpversion.cfg
--rw-r--r--   0        0        0     1686 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       88 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/.gitignore
--rw-r--r--   0        0        0      144 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/.readthedocs.yml
--rw-r--r--   0        0        0     1081 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/LICENSE
--rw-r--r--   0        0        0      675 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/README.rst
--rw-r--r--   0        0        0       68 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/dev-requirements.txt
--rw-r--r--   0        0        0     2497 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/docs/changelog.rst
--rw-r--r--   0        0        0     1693 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/docs/conf.py
--rw-r--r--   0        0        0     1302 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/docs/index.rst
--rw-r--r--   0        0        0     1546 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/docs/pyproject_hooks.rst
--rw-r--r--   0        0        0      389 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/docs/release-process.rst
--rw-r--r--   0        0        0       12 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/docs/requirements.txt
--rw-r--r--   0        0        0      741 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      129 2022-11-21 11:27:47.303607 pyproject_hooks-1.0.0/pytest.ini
--rw-r--r--   0        0        0      491 2022-11-21 11:34:48.350629 pyproject_hooks-1.0.0/src/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      121 2022-11-21 11:27:47.304607 pyproject_hooks-1.0.0/src/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    11920 2022-11-21 11:27:47.304607 pyproject_hooks-1.0.0/src/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      546 2022-11-21 11:27:47.304607 pyproject_hooks-1.0.0/src/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    10927 2022-11-21 11:27:47.304607 pyproject_hooks-1.0.0/src/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0        0 2022-11-21 11:27:47.304607 pyproject_hooks-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     1946 2022-11-21 11:27:47.304607 pyproject_hooks-1.0.0/tests/samples/buildsys_pkgs/buildsys.py
--rw-r--r--   0        0        0     1012 2022-11-21 11:27:47.304607 pyproject_hooks-1.0.0/tests/samples/buildsys_pkgs/buildsys_minimal.py
--rw-r--r--   0        0        0       92 2022-11-21 11:27:47.304607 pyproject_hooks-1.0.0/tests/samples/buildsys_pkgs/buildsys_minimal_editable.py
--rw-r--r--   0        0        0     1081 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg1/pkg1-0.5.dist-info/LICENSE
--rw-r--r--   0        0        0      253 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg1/pkg1-0.5.dist-info/METADATA
--rw-r--r--   0        0        0      336 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg1/pkg1-0.5.dist-info/RECORD
--rw-r--r--   0        0        0      101 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg1/pkg1-0.5.dist-info/WHEEL
--rw-r--r--   0        0        0       52 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg1/pkg1.py
--rw-r--r--   0        0        0      171 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg1/pyproject.toml
--rw-r--r--   0        0        0     1081 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg2/pkg2-0.5.dist-info/LICENSE
--rw-r--r--   0        0        0      251 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg2/pkg2-0.5.dist-info/METADATA
--rw-r--r--   0        0        0      336 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg2/pkg2-0.5.dist-info/RECORD
--rw-r--r--   0        0        0      100 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg2/pkg2-0.5.dist-info/WHEEL
--rw-r--r--   0        0        0       52 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg2/pkg2.py
--rw-r--r--   0        0        0       64 2022-11-21 11:27:47.305607 pyproject_hooks-1.0.0/tests/samples/pkg2/pyproject.toml
--rw-r--r--   0        0        0     1081 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/pkg3/pkg3-0.5.dist-info/LICENSE
--rw-r--r--   0        0        0      251 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/pkg3/pkg3-0.5.dist-info/METADATA
--rw-r--r--   0        0        0      336 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/pkg3/pkg3-0.5.dist-info/RECORD
--rw-r--r--   0        0        0      100 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/pkg3/pkg3-0.5.dist-info/WHEEL
--rw-r--r--   0        0        0       52 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/pkg3/pkg3.py
--rw-r--r--   0        0        0       73 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/pkg3/pyproject.toml
--rw-r--r--   0        0        0       88 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/pkg_intree/backend/intree_backend.py
--rw-r--r--   0        0        0       74 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/pkg_intree/pyproject.toml
--rw-r--r--   0        0        0       90 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/setup-py/pyproject.toml
--rw-r--r--   0        0        0       98 2022-11-21 11:27:47.306607 pyproject_hooks-1.0.0/tests/samples/setup-py/setup.py
--rw-r--r--   0        0        0       90 2022-11-21 11:27:47.307607 pyproject_hooks-1.0.0/tests/samples/test-for-issue-104/pyproject.toml
--rw-r--r--   0        0        0      249 2022-11-21 11:27:47.307607 pyproject_hooks-1.0.0/tests/samples/test-for-issue-104/setup.py
--rw-r--r--   0        0        0     6880 2022-11-21 11:27:47.307607 pyproject_hooks-1.0.0/tests/test_call_hooks.py
--rw-r--r--   0        0        0     3554 2022-11-21 11:27:47.307607 pyproject_hooks-1.0.0/tests/test_hook_fallbacks.py
--rw-r--r--   0        0        0     1790 2022-11-21 11:27:47.307607 pyproject_hooks-1.0.0/tests/test_inplace_hooks.py
--rw-r--r--   0        0        0      396 2022-11-21 11:27:47.307607 pyproject_hooks-1.0.0/tox.ini
--rw-r--r--   0        0        0     1341 1970-01-01 00:00:00.000000 pyproject_hooks-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      675 2024-04-29 07:28:50.002159 pyproject_hooks-1.1.0/README.rst
+-rw-r--r--   0        0        0      767 2024-04-29 07:28:50.002159 pyproject_hooks-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      691 2024-04-29 07:28:50.002159 pyproject_hooks-1.1.0/src/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0    14936 2024-04-29 07:28:50.002159 pyproject_hooks-1.1.0/src/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      557 2024-04-29 07:28:50.002159 pyproject_hooks-1.1.0/src/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    11603 2024-04-29 07:28:50.002159 pyproject_hooks-1.1.0/src/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0        0 2024-04-29 07:28:50.002159 pyproject_hooks-1.1.0/src/pyproject_hooks/py.typed
+-rw-r--r--   0        0        0     1288 1970-01-01 00:00:00.000000 pyproject_hooks-1.1.0/PKG-INFO
```

### Comparing `pyproject_hooks-1.0.0/README.rst` & `pyproject_hooks-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyproject_hooks-1.0.0/pyproject.toml` & `pyproject_hooks-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 [project]
 name = "pyproject_hooks"
 authors = [
     {name = "Thomas Kluyver", email = "thomas@kluyver.me.uk"},
 ]
 readme = "README.rst"
 requires-python = ">=3.7"
-dependencies = [
-    "tomli >=1.1.0 ; python_version<'3.11'",
-]
+dependencies = []
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Source = "https://github.com/pypa/pyproject-hooks"
 Documentation = "https://pyproject-hooks.readthedocs.io/"
 Changelog = "https://pyproject-hooks.readthedocs.io/en/latest/changelog.html"
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+src = ["src", "tests"]
+
+[tool.ruff.isort]
+known-first-party = ["pyproject_hooks", "tests"]
```

### Comparing `pyproject_hooks-1.0.0/src/pyproject_hooks/_in_process/__init__.py` & `pyproject_hooks-1.1.0/src/pyproject_hooks/_in_process/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,12 +7,15 @@
 import importlib.resources as resources
 
 try:
     resources.files
 except AttributeError:
     # Python 3.8 compatibility
     def _in_proc_script_path():
-        return resources.path(__package__, '_in_process.py')
+        return resources.path(__package__, "_in_process.py")
+
 else:
+
     def _in_proc_script_path():
         return resources.as_file(
-            resources.files(__package__).joinpath('_in_process.py'))
+            resources.files(__package__).joinpath("_in_process.py")
+        )
```

### Comparing `pyproject_hooks-1.0.0/src/pyproject_hooks/_in_process/_in_process.py` & `pyproject_hooks-1.1.0/src/pyproject_hooks/_in_process/_in_process.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This is invoked in a subprocess to call the build backend hooks.
 
 It expects:
 - Command line args: hook_name, control_dir
 - Environment variables:
-      PEP517_BUILD_BACKEND=entry.point:spec
-      PEP517_BACKEND_PATH=paths (separated with os.pathsep)
+      _PYPROJECT_HOOKS_BUILD_BACKEND=entry.point:spec
+      _PYPROJECT_HOOKS_BACKEND_PATH=paths (separated with os.pathsep)
 - control_dir/input.json:
   - {"kwargs": {...}}
 
 Results:
 - control_dir/output.json
   - {"return_val": ...}
 """
@@ -17,84 +17,100 @@
 import os.path
 import re
 import shutil
 import sys
 import traceback
 from glob import glob
 from importlib import import_module
+from importlib.machinery import PathFinder
 from os.path import join as pjoin
 
 # This file is run as a script, and `import wrappers` is not zip-safe, so we
 # include write_json() and read_json() from wrappers.py.
 
 
 def write_json(obj, path, **kwargs):
-    with open(path, 'w', encoding='utf-8') as f:
+    with open(path, "w", encoding="utf-8") as f:
         json.dump(obj, f, **kwargs)
 
 
 def read_json(path):
-    with open(path, encoding='utf-8') as f:
+    with open(path, encoding="utf-8") as f:
         return json.load(f)
 
 
 class BackendUnavailable(Exception):
     """Raised if we cannot import the backend"""
-    def __init__(self, traceback):
-        self.traceback = traceback
-
 
-class BackendInvalid(Exception):
-    """Raised if the backend is invalid"""
-    def __init__(self, message):
+    def __init__(self, message, traceback=None):
+        super().__init__(message)
         self.message = message
+        self.traceback = traceback
 
 
 class HookMissing(Exception):
     """Raised if a hook is missing and we are not executing the fallback"""
+
     def __init__(self, hook_name=None):
         super().__init__(hook_name)
         self.hook_name = hook_name
 
 
-def contained_in(filename, directory):
-    """Test if a file is located within the given directory."""
-    filename = os.path.normcase(os.path.abspath(filename))
-    directory = os.path.normcase(os.path.abspath(directory))
-    return os.path.commonprefix([filename, directory]) == directory
-
-
 def _build_backend():
     """Find and load the build backend"""
-    # Add in-tree backend directories to the front of sys.path.
-    backend_path = os.environ.get('PEP517_BACKEND_PATH')
+    backend_path = os.environ.get("_PYPROJECT_HOOKS_BACKEND_PATH")
+    ep = os.environ["_PYPROJECT_HOOKS_BUILD_BACKEND"]
+    mod_path, _, obj_path = ep.partition(":")
+
     if backend_path:
+        # Ensure in-tree backend directories have the highest priority when importing.
         extra_pathitems = backend_path.split(os.pathsep)
-        sys.path[:0] = extra_pathitems
+        sys.meta_path.insert(0, _BackendPathFinder(extra_pathitems, mod_path))
 
-    ep = os.environ['PEP517_BUILD_BACKEND']
-    mod_path, _, obj_path = ep.partition(':')
     try:
         obj = import_module(mod_path)
     except ImportError:
-        raise BackendUnavailable(traceback.format_exc())
-
-    if backend_path:
-        if not any(
-            contained_in(obj.__file__, path)
-            for path in extra_pathitems
-        ):
-            raise BackendInvalid("Backend was not loaded from backend-path")
+        msg = f"Cannot import {mod_path!r}"
+        raise BackendUnavailable(msg, traceback.format_exc())
 
     if obj_path:
-        for path_part in obj_path.split('.'):
+        for path_part in obj_path.split("."):
             obj = getattr(obj, path_part)
     return obj
 
 
+class _BackendPathFinder:
+    """Implements the MetaPathFinder interface to locate modules in ``backend-path``.
+
+    Since the environment provided by the frontend can contain all sorts of
+    MetaPathFinders, the only way to ensure the backend is loaded from the
+    right place is to prepend our own.
+    """
+
+    def __init__(self, backend_path, backend_module):
+        self.backend_path = backend_path
+        self.backend_module = backend_module
+        self.backend_parent, _, _ = backend_module.partition(".")
+
+    def find_spec(self, fullname, _path, _target=None):
+        if "." in fullname:
+            # Rely on importlib to find nested modules based on parent's path
+            return None
+
+        # Ignore other items in _path or sys.path and use backend_path instead:
+        spec = PathFinder.find_spec(fullname, path=self.backend_path)
+        if spec is None and fullname == self.backend_parent:
+            # According to the spec, the backend MUST be loaded from backend-path.
+            # Therefore, we can halt the import machinery and raise a clean error.
+            msg = f"Cannot find module {self.backend_module!r} in {self.backend_path!r}"
+            raise BackendUnavailable(msg)
+
+        return spec
+
+
 def _supported_features():
     """Return the list of options features supported by the backend.
 
     Returns a list of strings.
     The only possible value is 'build_editable'.
     """
     backend = _build_backend()
@@ -129,15 +145,16 @@
     except AttributeError:
         return []
     else:
         return hook(config_settings)
 
 
 def prepare_metadata_for_build_wheel(
-        metadata_directory, config_settings, _allow_fallback):
+    metadata_directory, config_settings, _allow_fallback
+):
     """Invoke optional prepare_metadata_for_build_wheel
 
     Implements a fallback by building a wheel if the hook isn't defined,
     unless _allow_fallback is False in which case HookMissing is raised.
     """
     backend = _build_backend()
     try:
@@ -146,20 +163,22 @@
         if not _allow_fallback:
             raise HookMissing()
     else:
         return hook(metadata_directory, config_settings)
     # fallback to build_wheel outside the try block to avoid exception chaining
     # which can be confusing to users and is not relevant
     whl_basename = backend.build_wheel(metadata_directory, config_settings)
-    return _get_wheel_metadata_from_wheel(whl_basename, metadata_directory,
-                                          config_settings)
+    return _get_wheel_metadata_from_wheel(
+        whl_basename, metadata_directory, config_settings
+    )
 
 
 def prepare_metadata_for_build_editable(
-        metadata_directory, config_settings, _allow_fallback):
+    metadata_directory, config_settings, _allow_fallback
+):
     """Invoke optional prepare_metadata_for_build_editable
 
     Implements a fallback by building an editable wheel if the hook isn't
     defined, unless _allow_fallback is False in which case HookMissing is
     raised.
     """
     backend = _build_backend()
@@ -167,73 +186,74 @@
         hook = backend.prepare_metadata_for_build_editable
     except AttributeError:
         if not _allow_fallback:
             raise HookMissing()
         try:
             build_hook = backend.build_editable
         except AttributeError:
-            raise HookMissing(hook_name='build_editable')
+            raise HookMissing(hook_name="build_editable")
         else:
             whl_basename = build_hook(metadata_directory, config_settings)
-            return _get_wheel_metadata_from_wheel(whl_basename,
-                                                  metadata_directory,
-                                                  config_settings)
+            return _get_wheel_metadata_from_wheel(
+                whl_basename, metadata_directory, config_settings
+            )
     else:
         return hook(metadata_directory, config_settings)
 
 
-WHEEL_BUILT_MARKER = 'PEP517_ALREADY_BUILT_WHEEL'
+WHEEL_BUILT_MARKER = "PYPROJECT_HOOKS_ALREADY_BUILT_WHEEL"
 
 
 def _dist_info_files(whl_zip):
     """Identify the .dist-info folder inside a wheel ZipFile."""
     res = []
     for path in whl_zip.namelist():
-        m = re.match(r'[^/\\]+-[^/\\]+\.dist-info/', path)
+        m = re.match(r"[^/\\]+-[^/\\]+\.dist-info/", path)
         if m:
             res.append(path)
     if res:
         return res
     raise Exception("No .dist-info folder found in wheel")
 
 
-def _get_wheel_metadata_from_wheel(
-        whl_basename, metadata_directory, config_settings):
+def _get_wheel_metadata_from_wheel(whl_basename, metadata_directory, config_settings):
     """Extract the metadata from a wheel.
 
     Fallback for when the build backend does not
     define the 'get_wheel_metadata' hook.
     """
     from zipfile import ZipFile
-    with open(os.path.join(metadata_directory, WHEEL_BUILT_MARKER), 'wb'):
+
+    with open(os.path.join(metadata_directory, WHEEL_BUILT_MARKER), "wb"):
         pass  # Touch marker file
 
     whl_file = os.path.join(metadata_directory, whl_basename)
     with ZipFile(whl_file) as zipf:
         dist_info = _dist_info_files(zipf)
         zipf.extractall(path=metadata_directory, members=dist_info)
-    return dist_info[0].split('/')[0]
+    return dist_info[0].split("/")[0]
 
 
 def _find_already_built_wheel(metadata_directory):
-    """Check for a wheel already built during the get_wheel_metadata hook.
-    """
+    """Check for a wheel already built during the get_wheel_metadata hook."""
     if not metadata_directory:
         return None
     metadata_parent = os.path.dirname(metadata_directory)
     if not os.path.isfile(pjoin(metadata_parent, WHEEL_BUILT_MARKER)):
         return None
 
-    whl_files = glob(os.path.join(metadata_parent, '*.whl'))
+    whl_files = glob(os.path.join(metadata_parent, "*.whl"))
     if not whl_files:
-        print('Found wheel built marker, but no .whl files')
+        print("Found wheel built marker, but no .whl files")
         return None
     if len(whl_files) > 1:
-        print('Found multiple .whl files; unspecified behaviour. '
-              'Will call build_wheel.')
+        print(
+            "Found multiple .whl files; unspecified behaviour. "
+            "Will call build_wheel."
+        )
         return None
 
     # Exactly one .whl file
     return whl_files[0]
 
 
 def build_wheel(wheel_directory, config_settings, metadata_directory=None):
@@ -244,16 +264,17 @@
     will copy it rather than rebuilding the wheel.
     """
     prebuilt_whl = _find_already_built_wheel(metadata_directory)
     if prebuilt_whl:
         shutil.copy2(prebuilt_whl, wheel_directory)
         return os.path.basename(prebuilt_whl)
 
-    return _build_backend().build_wheel(wheel_directory, config_settings,
-                                        metadata_directory)
+    return _build_backend().build_wheel(
+        wheel_directory, config_settings, metadata_directory
+    )
 
 
 def build_editable(wheel_directory, config_settings, metadata_directory=None):
     """Invoke the optional build_editable hook.
 
     If a wheel was already built in the
     prepare_metadata_for_build_editable fallback, this
@@ -289,65 +310,64 @@
 
 class _DummyException(Exception):
     """Nothing should ever raise this exception"""
 
 
 class GotUnsupportedOperation(Exception):
     """For internal use when backend raises UnsupportedOperation"""
+
     def __init__(self, traceback):
         self.traceback = traceback
 
 
 def build_sdist(sdist_directory, config_settings):
     """Invoke the mandatory build_sdist hook."""
     backend = _build_backend()
     try:
         return backend.build_sdist(sdist_directory, config_settings)
-    except getattr(backend, 'UnsupportedOperation', _DummyException):
+    except getattr(backend, "UnsupportedOperation", _DummyException):
         raise GotUnsupportedOperation(traceback.format_exc())
 
 
 HOOK_NAMES = {
-    'get_requires_for_build_wheel',
-    'prepare_metadata_for_build_wheel',
-    'build_wheel',
-    'get_requires_for_build_editable',
-    'prepare_metadata_for_build_editable',
-    'build_editable',
-    'get_requires_for_build_sdist',
-    'build_sdist',
-    '_supported_features',
+    "get_requires_for_build_wheel",
+    "prepare_metadata_for_build_wheel",
+    "build_wheel",
+    "get_requires_for_build_editable",
+    "prepare_metadata_for_build_editable",
+    "build_editable",
+    "get_requires_for_build_sdist",
+    "build_sdist",
+    "_supported_features",
 }
 
 
 def main():
     if len(sys.argv) < 3:
         sys.exit("Needs args: hook_name, control_dir")
     hook_name = sys.argv[1]
     control_dir = sys.argv[2]
     if hook_name not in HOOK_NAMES:
         sys.exit("Unknown hook: %s" % hook_name)
     hook = globals()[hook_name]
 
-    hook_input = read_json(pjoin(control_dir, 'input.json'))
+    hook_input = read_json(pjoin(control_dir, "input.json"))
 
-    json_out = {'unsupported': False, 'return_val': None}
+    json_out = {"unsupported": False, "return_val": None}
     try:
-        json_out['return_val'] = hook(**hook_input['kwargs'])
+        json_out["return_val"] = hook(**hook_input["kwargs"])
     except BackendUnavailable as e:
-        json_out['no_backend'] = True
-        json_out['traceback'] = e.traceback
-    except BackendInvalid as e:
-        json_out['backend_invalid'] = True
-        json_out['backend_error'] = e.message
+        json_out["no_backend"] = True
+        json_out["traceback"] = e.traceback
+        json_out["backend_error"] = e.message
     except GotUnsupportedOperation as e:
-        json_out['unsupported'] = True
-        json_out['traceback'] = e.traceback
+        json_out["unsupported"] = True
+        json_out["traceback"] = e.traceback
     except HookMissing as e:
-        json_out['hook_missing'] = True
-        json_out['missing_hook_name'] = e.hook_name or hook_name
+        json_out["hook_missing"] = True
+        json_out["missing_hook_name"] = e.hook_name or hook_name
 
-    write_json(json_out, pjoin(control_dir, 'output.json'), indent=2)
+    write_json(json_out, pjoin(control_dir, "output.json"), indent=2)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `pyproject_hooks-1.0.0/PKG-INFO` & `pyproject_hooks-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pyproject_hooks
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wrappers to call pyproject.toml-based build backend hooks.
 Author-email: Thomas Kluyver <thomas@kluyver.me.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: tomli >=1.1.0 ; python_version<'3.11'
 Project-URL: Changelog, https://pyproject-hooks.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://pyproject-hooks.readthedocs.io/
 Project-URL: Source, https://github.com/pypa/pyproject-hooks
 
 ``pyproject-hooks``
 ===================
```

