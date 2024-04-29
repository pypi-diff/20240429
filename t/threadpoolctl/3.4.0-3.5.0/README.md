# Comparing `tmp/threadpoolctl-3.4.0.tar.gz` & `tmp/threadpoolctl-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threadpoolctl-3.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "threadpoolctl-3.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `threadpoolctl-3.4.0.tar` & `threadpoolctl-3.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     6633 2024-02-14 15:28:49.147424 threadpoolctl-3.4.0/.azure_pipeline.yml
--rw-r--r--   0        0        0       14 2019-04-03 14:59:03.684333 threadpoolctl-3.4.0/.codecov.yml
--rw-r--r--   0        0        0       28 2019-04-03 14:59:03.684333 threadpoolctl-3.4.0/.coveragerc
--rw-r--r--   0        0        0      302 2023-07-12 08:17:49.739681 threadpoolctl-3.4.0/.gitignore
--rw-r--r--   0        0        0     5284 2024-03-20 13:36:20.768322 threadpoolctl-3.4.0/CHANGES.md
--rw-r--r--   0        0        0     1507 2019-04-03 14:59:03.684333 threadpoolctl-3.4.0/LICENSE
--rw-r--r--   0        0        0    12497 2024-02-14 15:28:49.151424 threadpoolctl-3.4.0/README.md
--rw-r--r--   0        0        0      862 2021-09-28 09:58:55.838120 threadpoolctl-3.4.0/benchmarks/bench_context_manager_overhead.py
--rw-r--r--   0        0        0       47 2021-09-15 13:26:21.489843 threadpoolctl-3.4.0/conftest.py
--rwxr-xr-x   0        0        0      521 2023-12-17 15:23:13.940468 threadpoolctl-3.4.0/continuous_integration/build_test_ext.sh
--rw-r--r--   0        0        0     1769 2023-06-30 15:31:34.528461 threadpoolctl-3.4.0/continuous_integration/check_no_test_skipped.py
--rw-r--r--   0        0        0     1281 2023-12-13 09:38:54.935551 threadpoolctl-3.4.0/continuous_integration/install.cmd
--rwxr-xr-x   0        0        0     3160 2023-12-13 09:38:54.939551 threadpoolctl-3.4.0/continuous_integration/install.sh
--rwxr-xr-x   0        0        0     1811 2024-02-06 08:45:04.404626 threadpoolctl-3.4.0/continuous_integration/install_with_blis.sh
--rwxr-xr-x   0        0        0     2461 2024-02-14 15:28:49.151424 threadpoolctl-3.4.0/continuous_integration/install_with_flexiblas.sh
--rw-r--r--   0        0        0     1745 2024-02-07 12:42:18.877825 threadpoolctl-3.4.0/continuous_integration/posix.yml
--rw-r--r--   0        0        0      320 2023-12-13 09:38:54.939551 threadpoolctl-3.4.0/continuous_integration/test_script.cmd
--rwxr-xr-x   0        0        0      613 2024-01-17 10:19:28.785481 threadpoolctl-3.4.0/continuous_integration/test_script.sh
--rwxr-xr-x   0        0        0      303 2019-04-03 14:59:03.684333 threadpoolctl-3.4.0/continuous_integration/upload_codecov.sh
--rw-r--r--   0        0        0      928 2024-01-17 10:00:27.319912 threadpoolctl-3.4.0/continuous_integration/windows.yml
--rw-r--r--   0        0        0       39 2019-04-03 14:59:03.684333 threadpoolctl-3.4.0/dev-requirements.txt
--rw-r--r--   0        0        0     3924 2023-07-12 08:17:49.739681 threadpoolctl-3.4.0/multiple_openmp.md
--rw-r--r--   0        0        0      988 2024-02-09 14:27:12.738413 threadpoolctl-3.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2020-06-02 21:31:29.138258 threadpoolctl-3.4.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2021-09-15 13:26:21.493843 threadpoolctl-3.4.0/tests/_openmp_test_helper/__init__.py
--rw-r--r--   0        0        0      572 2023-12-14 16:36:28.766260 threadpoolctl-3.4.0/tests/_openmp_test_helper/build_utils.py
--rw-r--r--   0        0        0     1286 2023-12-13 09:38:54.939551 threadpoolctl-3.4.0/tests/_openmp_test_helper/nested_prange_blas.pyx
--rw-r--r--   0        0        0     1661 2024-02-07 12:42:18.885825 threadpoolctl-3.4.0/tests/_openmp_test_helper/nested_prange_blas_custom.pyx
--rw-r--r--   0        0        0       47 2024-02-06 08:45:04.408626 threadpoolctl-3.4.0/tests/_openmp_test_helper/openmp_helpers_inner.pxd
--rw-r--r--   0        0        0      927 2024-02-06 08:45:04.408626 threadpoolctl-3.4.0/tests/_openmp_test_helper/openmp_helpers_inner.pyx
--rw-r--r--   0        0        0      724 2021-09-15 13:26:21.493843 threadpoolctl-3.4.0/tests/_openmp_test_helper/openmp_helpers_outer.pyx
--rw-r--r--   0        0        0     1122 2021-09-24 08:18:13.956710 threadpoolctl-3.4.0/tests/_openmp_test_helper/setup_inner.py
--rw-r--r--   0        0        0     1133 2024-02-07 12:42:18.877825 threadpoolctl-3.4.0/tests/_openmp_test_helper/setup_nested_prange_blas.py
--rw-r--r--   0        0        0     1122 2021-09-24 08:18:13.956710 threadpoolctl-3.4.0/tests/_openmp_test_helper/setup_outer.py
--rw-r--r--   0        0        0     2090 2023-12-13 09:38:54.943551 threadpoolctl-3.4.0/tests/_pyMylib/__init__.py
--rw-r--r--   0        0        0      249 2023-07-12 08:17:49.743681 threadpoolctl-3.4.0/tests/_pyMylib/my_threaded_lib.c
--rw-r--r--   0        0        0    30051 2024-02-14 15:28:49.155423 threadpoolctl-3.4.0/tests/test_threadpoolctl.py
--rw-r--r--   0        0        0     2396 2024-02-07 12:42:18.877825 threadpoolctl-3.4.0/tests/utils.py
--rw-r--r--   0        0        0    49753 2024-03-20 13:36:20.768322 threadpoolctl-3.4.0/threadpoolctl.py
--rw-r--r--   0        0        0    13249 1970-01-01 00:00:00.000000 threadpoolctl-3.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6854 2024-04-29 07:47:23.342179 threadpoolctl-3.5.0/.azure_pipeline.yml
+-rw-r--r--   0        0        0       14 2024-04-25 16:02:52.837982 threadpoolctl-3.5.0/.codecov.yml
+-rw-r--r--   0        0        0       28 2024-04-25 16:02:52.837982 threadpoolctl-3.5.0/.coveragerc
+-rw-r--r--   0        0        0      302 2024-04-25 16:02:52.837982 threadpoolctl-3.5.0/.gitignore
+-rw-r--r--   0        0        0     5578 2024-04-29 13:41:05.157064 threadpoolctl-3.5.0/CHANGES.md
+-rw-r--r--   0        0        0     1507 2024-04-25 16:02:52.837982 threadpoolctl-3.5.0/LICENSE
+-rw-r--r--   0        0        0    13098 2024-04-29 07:47:23.342179 threadpoolctl-3.5.0/README.md
+-rw-r--r--   0        0        0      862 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/benchmarks/bench_context_manager_overhead.py
+-rw-r--r--   0        0        0       47 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/conftest.py
+-rwxr-xr-x   0        0        0      521 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/continuous_integration/build_test_ext.sh
+-rw-r--r--   0        0        0     1769 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/continuous_integration/check_no_test_skipped.py
+-rw-r--r--   0        0        0     1281 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/continuous_integration/install.cmd
+-rwxr-xr-x   0        0        0     3559 2024-04-29 07:47:23.342179 threadpoolctl-3.5.0/continuous_integration/install.sh
+-rwxr-xr-x   0        0        0     1811 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/continuous_integration/install_with_blis.sh
+-rwxr-xr-x   0        0        0     2461 2024-04-29 07:47:23.342179 threadpoolctl-3.5.0/continuous_integration/install_with_flexiblas.sh
+-rw-r--r--   0        0        0     1753 2024-04-29 07:47:23.342179 threadpoolctl-3.5.0/continuous_integration/posix.yml
+-rw-r--r--   0        0        0      320 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/continuous_integration/test_script.cmd
+-rwxr-xr-x   0        0        0      612 2024-04-29 07:47:23.342179 threadpoolctl-3.5.0/continuous_integration/test_script.sh
+-rwxr-xr-x   0        0        0      303 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/continuous_integration/upload_codecov.sh
+-rw-r--r--   0        0        0      928 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/continuous_integration/windows.yml
+-rw-r--r--   0        0        0       39 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/dev-requirements.txt
+-rw-r--r--   0        0        0     3924 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/multiple_openmp.md
+-rw-r--r--   0        0        0      988 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/__init__.py
+-rw-r--r--   0        0        0      572 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/build_utils.py
+-rw-r--r--   0        0        0     1286 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/nested_prange_blas.pyx
+-rw-r--r--   0        0        0     1661 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/nested_prange_blas_custom.pyx
+-rw-r--r--   0        0        0       47 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/openmp_helpers_inner.pxd
+-rw-r--r--   0        0        0      927 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/openmp_helpers_inner.pyx
+-rw-r--r--   0        0        0      724 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/openmp_helpers_outer.pyx
+-rw-r--r--   0        0        0     1122 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/setup_inner.py
+-rw-r--r--   0        0        0     1133 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/setup_nested_prange_blas.py
+-rw-r--r--   0        0        0     1122 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_openmp_test_helper/setup_outer.py
+-rw-r--r--   0        0        0     2090 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_pyMylib/__init__.py
+-rw-r--r--   0        0        0      249 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/_pyMylib/my_threaded_lib.c
+-rw-r--r--   0        0        0    30051 2024-04-29 07:47:23.346179 threadpoolctl-3.5.0/tests/test_threadpoolctl.py
+-rw-r--r--   0        0        0     2396 2024-04-25 16:02:52.841982 threadpoolctl-3.5.0/tests/utils.py
+-rw-r--r--   0        0        0    50023 2024-04-29 13:41:05.157064 threadpoolctl-3.5.0/threadpoolctl.py
+-rw-r--r--   0        0        0    13850 1970-01-01 00:00:00.000000 threadpoolctl-3.5.0/PKG-INFO
```

### Comparing `threadpoolctl-3.4.0/.azure_pipeline.yml` & `threadpoolctl-3.5.0/.azure_pipeline.yml`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,20 @@
           PACKAGER: 'pip'
 
   - template: continuous_integration/posix.yml
     parameters:
       name: Linux
       vmImage: ubuntu-20.04
       matrix:
+        # Linux environment with development versions of numpy and scipy
+        pylatest_pip_dev:
+          PACKAGER: 'pip-dev'
+          PYTHON_VERSION: '*'
+          CC_OUTER_LOOP: 'gcc'
+          CC_INNER_LOOP: 'gcc'
         # Linux environment to test that packages that comes with Ubuntu 20.04
         # are correctly handled.
         py38_ubuntu_atlas_gcc_gcc:
           PACKAGER: 'ubuntu'
           APT_BLAS: 'libatlas3-base libatlas-base-dev'
           PYTHON_VERSION: '3.8'
           CC_OUTER_LOOP: 'gcc'
```

### Comparing `threadpoolctl-3.4.0/CHANGES.md` & `threadpoolctl-3.5.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+3.5.0 (2024-04-29)
+==================
+
+- Added support for the Scientific Python version of OpenBLAS
+  (https://github.com/MacPython/openblas-libs), which exposes symbols with different
+  names than the ones of the original OpenBLAS library.
+  https://github.com/joblib/threadpoolctl/pull/175
+
 3.4.0 (2024-03-20)
 ==================
 
 - Added support for Python interpreters statically linked against libc or linked against
   alternative implementations of libc like musl (on Alpine Linux for instance).
   https://github.com/joblib/threadpoolctl/pull/171
```

### Comparing `threadpoolctl-3.4.0/LICENSE` & `threadpoolctl-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/README.md` & `threadpoolctl-3.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -328,32 +328,48 @@
   use in nested parallel calls.
 
 
 ## Maintainers
 
 To make a release:
 
-Bump the version number (`__version__`) in `threadpoolctl.py`.
+- Bump the version number (`__version__`) in `threadpoolctl.py` and update the
+  release date in `CHANGES.md`.
 
-Build the distribution archives:
+- Build the distribution archives:
 
 ```bash
 pip install flit
 flit build
 ```
 
-Check the contents of `dist/`.
+and check the contents of `dist/`.
 
-If everything is fine, make a commit for the release, tag it, push the
-tag to github and then:
+- If everything is fine, make a commit for the release, tag it and push the
+tag to github:
 
 ```bash
-flit publish
+git tag -a X.Y.Z
+git push git@github.com:joblib/threadpoolctl.git X.Y.Z
 ```
 
+- Upload the wheels and source distribution to PyPI using flit. Since PyPI doesn't
+  allow password authentication anymore, the username needs to be changed to the
+  generic name `__token__`:
+
+```bash
+FLIT_USERNAME=__token__ flit publish
+```
+
+  and a PyPI token has to be passed in place of the password.
+
+- Create a PR for the release on the [conda-forge feedstock](https://github.com/conda-forge/threadpoolctl-feedstock) (or wait for the bot to make it).
+
+- Publish the release on github.
+
 ### Credits
 
 The initial dynamic library introspection code was written by @anton-malakhov
 for the smp package available at https://github.com/IntelPython/smp .
 
 threadpoolctl extends this for other operating systems. Contrary to smp,
 threadpoolctl does not attempt to limit the size of Python multiprocessing
```

### Comparing `threadpoolctl-3.4.0/benchmarks/bench_context_manager_overhead.py` & `threadpoolctl-3.5.0/benchmarks/bench_context_manager_overhead.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/continuous_integration/build_test_ext.sh` & `threadpoolctl-3.5.0/continuous_integration/build_test_ext.sh`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/continuous_integration/check_no_test_skipped.py` & `threadpoolctl-3.5.0/continuous_integration/check_no_test_skipped.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/continuous_integration/install.cmd` & `threadpoolctl-3.5.0/continuous_integration/install.cmd`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/continuous_integration/install.sh` & `threadpoolctl-3.5.0/continuous_integration/install.sh`

 * *Files 18% similar despite different names*

```diff
@@ -61,14 +61,23 @@
     # numpy and scipy
     TO_INSTALL="python=$PYTHON_VERSION pip"
     make_conda $TO_INSTALL
     if [[ "$NO_NUMPY" != "true" ]]; then
         pip install numpy scipy
     fi
 
+elif [[ "$PACKAGER" == "pip-dev" ]]; then
+    # Use conda to build an empty python env and then use pip to install
+    # numpy and scipy dev versions
+    TO_INSTALL="python=$PYTHON_VERSION pip"
+    make_conda $TO_INSTALL
+
+    dev_anaconda_url=https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
+    pip install --pre --upgrade --timeout=60 --extra-index $dev_anaconda_url numpy scipy
+
 elif [[ "$PACKAGER" == "ubuntu" ]]; then
     # Remove the ubuntu toolchain PPA that seems to be invalid:
     # https://github.com/scikit-learn/scikit-learn/pull/13934
     sudo add-apt-repository --remove ppa:ubuntu-toolchain-r/test
     sudo apt-get update
     sudo apt-get install python3-scipy python3-virtualenv $APT_BLAS
     python3 -m virtualenv --system-site-packages --python=python3 $VIRTUALENV
```

### Comparing `threadpoolctl-3.4.0/continuous_integration/install_with_blis.sh` & `threadpoolctl-3.5.0/continuous_integration/install_with_blis.sh`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/continuous_integration/install_with_flexiblas.sh` & `threadpoolctl-3.5.0/continuous_integration/install_with_flexiblas.sh`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/continuous_integration/posix.yml` & `threadpoolctl-3.5.0/continuous_integration/posix.yml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   strategy:
     matrix:
       ${{ insert }}: ${{ parameters.matrix }}
 
   steps:
     - bash: echo "##vso[task.prependpath]$CONDA/bin"
       displayName: Add conda to PATH
-      condition: or(startsWith(variables['PACKAGER'], 'conda'), eq(variables['PACKAGER'], 'pip'))
+      condition: or(startsWith(variables['PACKAGER'], 'conda'), startsWith(variables['PACKAGER'], 'pip'))
     - bash: sudo chown -R $USER $CONDA
       # On Hosted macOS, the agent user doesn't have ownership of Miniconda's installation directory/
       # We need to take ownership if we want to update conda or install packages globally
       displayName: Take ownership of conda installation
       condition: eq('${{ parameters.name }}', 'macOS')
     - script: |
         continuous_integration/install.sh
```

### Comparing `threadpoolctl-3.4.0/continuous_integration/test_script.sh` & `threadpoolctl-3.5.0/continuous_integration/test_script.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/bin/bash
 
 set -e
 
 if [[ "$PACKAGER" == conda* ]]; then
     source activate $VIRTUALENV
     conda list
-elif [[ "$PACKAGER" == "pip" ]]; then
+elif [[ "$PACKAGER" == pip* ]]; then
     # we actually use conda to install the base environment:
     source activate $VIRTUALENV
     pip list
 elif [[ "$PACKAGER" == "ubuntu" ]]; then
     source $VIRTUALENV/bin/activate
     pip list
 fi
```

### Comparing `threadpoolctl-3.4.0/continuous_integration/windows.yml` & `threadpoolctl-3.5.0/continuous_integration/windows.yml`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/multiple_openmp.md` & `threadpoolctl-3.5.0/multiple_openmp.md`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/pyproject.toml` & `threadpoolctl-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_openmp_test_helper/build_utils.py` & `threadpoolctl-3.5.0/tests/_openmp_test_helper/build_utils.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_openmp_test_helper/nested_prange_blas.pyx` & `threadpoolctl-3.5.0/tests/_openmp_test_helper/nested_prange_blas.pyx`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_openmp_test_helper/nested_prange_blas_custom.pyx` & `threadpoolctl-3.5.0/tests/_openmp_test_helper/nested_prange_blas_custom.pyx`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_openmp_test_helper/openmp_helpers_inner.pyx` & `threadpoolctl-3.5.0/tests/_openmp_test_helper/openmp_helpers_inner.pyx`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_openmp_test_helper/openmp_helpers_outer.pyx` & `threadpoolctl-3.5.0/tests/_openmp_test_helper/openmp_helpers_outer.pyx`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_openmp_test_helper/setup_inner.py` & `threadpoolctl-3.5.0/tests/_openmp_test_helper/setup_inner.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_openmp_test_helper/setup_nested_prange_blas.py` & `threadpoolctl-3.5.0/tests/_openmp_test_helper/setup_nested_prange_blas.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_openmp_test_helper/setup_outer.py` & `threadpoolctl-3.5.0/tests/_openmp_test_helper/setup_outer.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/_pyMylib/__init__.py` & `threadpoolctl-3.5.0/tests/_pyMylib/__init__.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/test_threadpoolctl.py` & `threadpoolctl-3.5.0/tests/test_threadpoolctl.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/tests/utils.py` & `threadpoolctl-3.5.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `threadpoolctl-3.4.0/threadpoolctl.py` & `threadpoolctl-3.5.0/threadpoolctl.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 # adapted from code by Intel developer @anton-malakhov available at
 # https://github.com/IntelPython/smp (Copyright (c) 2017, Intel Corporation)
 # and also published under the BSD 3-Clause license
 import os
 import re
 import sys
 import ctypes
+import itertools
 import textwrap
 from typing import final
 import warnings
 from ctypes.util import find_library
 from abc import ABC, abstractmethod
 from functools import lru_cache
 from contextlib import ContextDecorator
 
-__version__ = "3.4.0"
+__version__ = "3.5.0"
 __all__ = [
     "threadpool_limits",
     "threadpool_info",
     "ThreadpoolController",
     "LibController",
     "register",
 ]
@@ -107,28 +108,27 @@
     @final
     def __init__(self, *, filepath=None, prefix=None, parent=None):
         """This is not meant to be overriden by subclasses."""
         self.parent = parent
         self.prefix = prefix
         self.filepath = filepath
         self.dynlib = ctypes.CDLL(filepath, mode=_RTLD_NOLOAD)
+        self._symbol_prefix, self._symbol_suffix = self._find_affixes()
         self.version = self.get_version()
         self.set_additional_attributes()
 
     def info(self):
         """Return relevant info wrapped in a dict"""
-        exposed_attrs = {
+        hidden_attrs = ("dynlib", "parent", "_symbol_prefix", "_symbol_suffix")
+        return {
             "user_api": self.user_api,
             "internal_api": self.internal_api,
             "num_threads": self.num_threads,
-            **vars(self),
+            **{k: v for k, v in vars(self).items() if k not in hidden_attrs},
         }
-        exposed_attrs.pop("dynlib")
-        exposed_attrs.pop("parent")
-        return exposed_attrs
 
     def set_additional_attributes(self):
         """Set additional attributes meant to be exposed in the info dict"""
 
     @property
     def num_threads(self):
         """Exposes the current thread limit as a dynamic property
@@ -145,104 +145,95 @@
     def set_num_threads(self, num_threads):
         """Set the maximum number of threads to use"""
 
     @abstractmethod
     def get_version(self):
         """Return the version of the shared library"""
 
+    def _find_affixes(self):
+        """Return the affixes for the symbols of the shared library"""
+        return "", ""
+
+    def _get_symbol(self, name):
+        """Return the symbol of the shared library accounding for the affixes"""
+        return getattr(
+            self.dynlib, f"{self._symbol_prefix}{name}{self._symbol_suffix}", None
+        )
+
 
 class OpenBLASController(LibController):
     """Controller class for OpenBLAS"""
 
     user_api = "blas"
     internal_api = "openblas"
-    filename_prefixes = ("libopenblas", "libblas")
-    check_symbols = (
-        "openblas_get_num_threads",
-        "openblas_get_num_threads64_",
-        "openblas_set_num_threads",
-        "openblas_set_num_threads64_",
-        "openblas_get_config",
-        "openblas_get_config64_",
-        "openblas_get_parallel",
-        "openblas_get_parallel64_",
-        "openblas_get_corename",
-        "openblas_get_corename64_",
+    filename_prefixes = ("libopenblas", "libblas", "libscipy_openblas")
+
+    _symbol_prefixes = ("", "scipy_")
+    _symbol_suffixes = ("", "64_", "_64")
+
+    # All variations of "openblas_get_num_threads", accounting for the affixes
+    check_symbols = tuple(
+        f"{prefix}openblas_get_num_threads{suffix}"
+        for prefix, suffix in itertools.product(_symbol_prefixes, _symbol_suffixes)
     )
 
+    def _find_affixes(self):
+        for prefix, suffix in itertools.product(
+            self._symbol_prefixes, self._symbol_suffixes
+        ):
+            if hasattr(self.dynlib, f"{prefix}openblas_get_num_threads{suffix}"):
+                return prefix, suffix
+
     def set_additional_attributes(self):
         self.threading_layer = self._get_threading_layer()
         self.architecture = self._get_architecture()
 
     def get_num_threads(self):
-        get_func = getattr(
-            self.dynlib,
-            "openblas_get_num_threads",
-            # Symbols differ when built for 64bit integers in Fortran
-            getattr(self.dynlib, "openblas_get_num_threads64_", lambda: None),
-        )
-
-        return get_func()
+        get_num_threads_func = self._get_symbol("openblas_get_num_threads")
+        if get_num_threads_func is not None:
+            return get_num_threads_func()
+        return None
 
     def set_num_threads(self, num_threads):
-        set_func = getattr(
-            self.dynlib,
-            "openblas_set_num_threads",
-            # Symbols differ when built for 64bit integers in Fortran
-            getattr(
-                self.dynlib, "openblas_set_num_threads64_", lambda num_threads: None
-            ),
-        )
-        return set_func(num_threads)
+        set_num_threads_func = self._get_symbol("openblas_set_num_threads")
+        if set_num_threads_func is not None:
+            return set_num_threads_func(num_threads)
+        return None
 
     def get_version(self):
         # None means OpenBLAS is not loaded or version < 0.3.4, since OpenBLAS
         # did not expose its version before that.
-        get_config = getattr(
-            self.dynlib,
-            "openblas_get_config",
-            getattr(self.dynlib, "openblas_get_config64_", None),
-        )
-        if get_config is None:
+        get_version_func = self._get_symbol("openblas_get_config")
+        if get_version_func is not None:
+            get_version_func.restype = ctypes.c_char_p
+            config = get_version_func().split()
+            if config[0] == b"OpenBLAS":
+                return config[1].decode("utf-8")
             return None
-
-        get_config.restype = ctypes.c_char_p
-        config = get_config().split()
-        if config[0] == b"OpenBLAS":
-            return config[1].decode("utf-8")
         return None
 
     def _get_threading_layer(self):
         """Return the threading layer of OpenBLAS"""
-        openblas_get_parallel = getattr(
-            self.dynlib,
-            "openblas_get_parallel",
-            getattr(self.dynlib, "openblas_get_parallel64_", None),
-        )
-        if openblas_get_parallel is None:
-            return "unknown"
-        threading_layer = openblas_get_parallel()
-        if threading_layer == 2:
-            return "openmp"
-        elif threading_layer == 1:
-            return "pthreads"
-        return "disabled"
+        get_threading_layer_func = self._get_symbol("openblas_get_parallel")
+        if get_threading_layer_func is not None:
+            threading_layer = get_threading_layer_func()
+            if threading_layer == 2:
+                return "openmp"
+            elif threading_layer == 1:
+                return "pthreads"
+            return "disabled"
+        return "unknown"
 
     def _get_architecture(self):
         """Return the architecture detected by OpenBLAS"""
-        get_corename = getattr(
-            self.dynlib,
-            "openblas_get_corename",
-            getattr(self.dynlib, "openblas_get_corename64_", None),
-        )
-        if get_corename is None:
-            return None
-
-        get_corename.restype = ctypes.c_char_p
-        return get_corename().decode("utf-8")
+        get_architecture_func = self._get_symbol("openblas_get_corename")
+        if get_architecture_func is not None:
+            get_architecture_func.restype = ctypes.c_char_p
+            return get_architecture_func().decode("utf-8")
+        return None
 
 
 class BLISController(LibController):
     """Controller class for BLIS"""
 
     user_api = "blas"
     internal_api = "blis"
```

### Comparing `threadpoolctl-3.4.0/PKG-INFO` & `threadpoolctl-3.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threadpoolctl
-Version: 3.4.0
+Version: 3.5.0
 Summary: threadpoolctl
 Home-page: https://github.com/joblib/threadpoolctl
 License: BSD-3-Clause
 Author: Thomas Moreau
 Author-email: thomas.moreau.2010@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -348,32 +348,48 @@
   use in nested parallel calls.
 
 
 ## Maintainers
 
 To make a release:
 
-Bump the version number (`__version__`) in `threadpoolctl.py`.
+- Bump the version number (`__version__`) in `threadpoolctl.py` and update the
+  release date in `CHANGES.md`.
 
-Build the distribution archives:
+- Build the distribution archives:
 
 ```bash
 pip install flit
 flit build
 ```
 
-Check the contents of `dist/`.
+and check the contents of `dist/`.
 
-If everything is fine, make a commit for the release, tag it, push the
-tag to github and then:
+- If everything is fine, make a commit for the release, tag it and push the
+tag to github:
 
 ```bash
-flit publish
+git tag -a X.Y.Z
+git push git@github.com:joblib/threadpoolctl.git X.Y.Z
 ```
 
+- Upload the wheels and source distribution to PyPI using flit. Since PyPI doesn't
+  allow password authentication anymore, the username needs to be changed to the
+  generic name `__token__`:
+
+```bash
+FLIT_USERNAME=__token__ flit publish
+```
+
+  and a PyPI token has to be passed in place of the password.
+
+- Create a PR for the release on the [conda-forge feedstock](https://github.com/conda-forge/threadpoolctl-feedstock) (or wait for the bot to make it).
+
+- Publish the release on github.
+
 ### Credits
 
 The initial dynamic library introspection code was written by @anton-malakhov
 for the smp package available at https://github.com/IntelPython/smp .
 
 threadpoolctl extends this for other operating systems. Contrary to smp,
 threadpoolctl does not attempt to limit the size of Python multiprocessing
```

