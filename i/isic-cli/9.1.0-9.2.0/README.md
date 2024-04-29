# Comparing `tmp/isic-cli-9.1.0.tar.gz` & `tmp/isic-cli-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-cli-9.1.0.tar", last modified: Mon Jan 15 17:13:26 2024, max compression
+gzip compressed data, was "isic-cli-9.2.0.tar", last modified: Fri Mar  1 03:58:07 2024, max compression
```

## Comparing `isic-cli-9.1.0.tar` & `isic-cli-9.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.493095 isic-cli-9.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-01-15 17:13:10.000000 isic-cli-9.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-15 17:13:10.000000 isic-cli-9.1.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.489095 isic-cli-9.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.489095 isic-cli-9.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-01-15 17:13:10.000000 isic-cli-9.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-15 17:13:10.000000 isic-cli-9.1.0/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-15 17:13:10.000000 isic-cli-9.1.0/.github/workflows/release.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      415 2024-01-15 17:13:10.000000 isic-cli-9.1.0/.github/zip_and_upload_package.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-15 17:13:10.000000 isic-cli-9.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-15 17:13:10.000000 isic-cli-9.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-01-15 17:13:26.493095 isic-cli-9.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-01-15 17:13:10.000000 isic-cli-9.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.489095 isic-cli-9.1.0/isic_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.489095 isic-cli-9.1.0/isic_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/accession.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.493095 isic-cli-9.1.0/isic_cli/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/io/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.493095 isic-cli-9.1.0/isic_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-01-15 17:13:10.000000 isic-cli-9.1.0/isic_cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.493095 isic-cli-9.1.0/isic_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-01-15 17:13:26.000000 isic-cli-9.1.0/isic_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-15 17:13:26.000000 isic-cli-9.1.0/isic_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 17:13:26.000000 isic-cli-9.1.0/isic_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-01-15 17:13:26.000000 isic-cli-9.1.0/isic_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-15 17:13:26.000000 isic-cli-9.1.0/isic_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-15 17:13:26.000000 isic-cli-9.1.0/isic_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-15 17:13:10.000000 isic-cli-9.1.0/justfile
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-15 17:13:10.000000 isic-cli-9.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 17:13:26.493095 isic-cli-9.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-01-15 17:13:10.000000 isic-cli-9.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 17:13:26.493095 isic-cli-9.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tests/test_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tests/test_cli_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tests/test_cli_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tests/test_cli_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-15 17:13:10.000000 isic-cli-9.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.430656 isic-cli-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-01 03:57:54.000000 isic-cli-9.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-01 03:57:54.000000 isic-cli-9.2.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.422656 isic-cli-9.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.422656 isic-cli-9.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-01 03:57:54.000000 isic-cli-9.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-01 03:57:54.000000 isic-cli-9.2.0/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-01 03:57:54.000000 isic-cli-9.2.0/.github/workflows/release.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      415 2024-03-01 03:57:54.000000 isic-cli-9.2.0/.github/zip_and_upload_package.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-01 03:57:54.000000 isic-cli-9.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-01 03:57:54.000000 isic-cli-9.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-01 03:58:07.430656 isic-cli-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-03-01 03:57:54.000000 isic-cli-9.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.422656 isic-cli-9.2.0/isic_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.426656 isic-cli-9.2.0/isic_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/accession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.426656 isic-cli-9.2.0/isic_cli/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/io/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.426656 isic-cli-9.2.0/isic_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-03-01 03:57:54.000000 isic-cli-9.2.0/isic_cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.430656 isic-cli-9.2.0/isic_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-01 03:58:07.000000 isic-cli-9.2.0/isic_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-03-01 03:58:07.000000 isic-cli-9.2.0/isic_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 03:58:07.000000 isic-cli-9.2.0/isic_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-01 03:58:07.000000 isic-cli-9.2.0/isic_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-01 03:58:07.000000 isic-cli-9.2.0/isic_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-01 03:58:07.000000 isic-cli-9.2.0/isic_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-01 03:57:54.000000 isic-cli-9.2.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-01 03:57:54.000000 isic-cli-9.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 03:58:07.430656 isic-cli-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-01 03:57:54.000000 isic-cli-9.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 03:58:07.430656 isic-cli-9.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tests/test_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tests/test_cli_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tests/test_cli_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tests/test_cli_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-01 03:57:54.000000 isic-cli-9.2.0/tox.ini
```

### Comparing `isic-cli-9.1.0/.github/workflows/ci.yml` & `isic-cli-9.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/.github/workflows/package.yml` & `isic-cli-9.2.0/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/.github/workflows/release.yml` & `isic-cli-9.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/.gitignore` & `isic-cli-9.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/LICENSE` & `isic-cli-9.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/PKG-INFO` & `isic-cli-9.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 9.1.0
+Version: 9.2.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8
 Requires-Dist: django-s3-file-field-client>=1.0.0
 Requires-Dist: girder-cli-oauth-client<1.0.0
 Requires-Dist: humanize
-Requires-Dist: isic-metadata>=1.0.0
+Requires-Dist: isic-metadata>=1.1.0
 Requires-Dist: more-itertools
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: retryable-requests
 Requires-Dist: rich
 Requires-Dist: sentry-sdk
 Requires-Dist: tenacity
```

### Comparing `isic-cli-9.1.0/README.md` & `isic-cli-9.2.0/README.md`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/cli/__init__.py` & `isic-cli-9.2.0/isic_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/cli/accession.py` & `isic-cli-9.2.0/isic_cli/cli/accession.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/cli/collection.py` & `isic-cli-9.2.0/isic_cli/cli/collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/cli/image.py` & `isic-cli-9.2.0/isic_cli/cli/image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/cli/metadata.py` & `isic-cli-9.2.0/isic_cli/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/cli/types.py` & `isic-cli-9.2.0/isic_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/cli/user.py` & `isic-cli-9.2.0/isic_cli/cli/user.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/cli/utils.py` & `isic-cli-9.2.0/isic_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/io/http.py` & `isic-cli-9.2.0/isic_cli/io/http.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/session.py` & `isic-cli-9.2.0/isic_cli/session.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli/utils/version.py` & `isic-cli-9.2.0/isic_cli/utils/version.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/isic_cli.egg-info/PKG-INFO` & `isic-cli-9.2.0/isic_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 9.1.0
+Version: 9.2.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8
 Requires-Dist: django-s3-file-field-client>=1.0.0
 Requires-Dist: girder-cli-oauth-client<1.0.0
 Requires-Dist: humanize
-Requires-Dist: isic-metadata>=1.0.0
+Requires-Dist: isic-metadata>=1.1.0
 Requires-Dist: more-itertools
 Requires-Dist: packaging
 Requires-Dist: requests
 Requires-Dist: retryable-requests
 Requires-Dist: rich
 Requires-Dist: sentry-sdk
 Requires-Dist: tenacity
```

### Comparing `isic-cli-9.1.0/isic_cli.egg-info/SOURCES.txt` & `isic-cli-9.2.0/isic_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/pyproject.toml` & `isic-cli-9.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/setup.py` & `isic-cli-9.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     install_requires=[
         # we use the path_type=Path feature from click which was added in Click 8
         "click>=8",
         "django-s3-file-field-client>=1.0.0",
         # We expect girder-cli-oauth-client to drop oob support in the future
         "girder-cli-oauth-client<1.0.0",
         "humanize",
-        "isic-metadata>=1.0.0",
+        "isic-metadata>=1.1.0",
         "more-itertools",
         "packaging",
         "requests",
         "retryable-requests",
         "rich",
         "sentry-sdk",
         "tenacity",
```

### Comparing `isic-cli-9.1.0/tests/conftest.py` & `isic-cli-9.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/tests/test_cli_base.py` & `isic-cli-9.2.0/tests/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/tests/test_cli_collection.py` & `isic-cli-9.2.0/tests/test_cli_collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/tests/test_cli_image.py` & `isic-cli-9.2.0/tests/test_cli_image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/tests/test_cli_metadata.py` & `isic-cli-9.2.0/tests/test_cli_metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/tests/test_utils.py` & `isic-cli-9.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-9.1.0/tox.ini` & `isic-cli-9.2.0/tox.ini`

 * *Files identical despite different names*

