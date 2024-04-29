# Comparing `tmp/test_pypi_package_example-1.7.0.dev1714390008.tar.gz` & `tmp/test_pypi_package_example-1.7.0.dev1714398267.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_pypi_package_example-1.7.0.dev1714390008.tar", max compression
+gzip compressed data, was "test_pypi_package_example-1.7.0.dev1714398267.tar", max compression
```

## Comparing `test_pypi_package_example-1.7.0.dev1714390008.tar` & `test_pypi_package_example-1.7.0.dev1714398267.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     9580 2024-04-29 15:26:31.856958 test_pypi_package_example-1.7.0.dev1714390008/LICENSE
--rw-r--r--   0        0        0       36 2024-04-29 14:35:36.566311 test_pypi_package_example-1.7.0.dev1714390008/README.md
--rw-r--r--   0        0        0      516 2024-04-29 15:26:49.218876 test_pypi_package_example-1.7.0.dev1714390008/pyproject.toml
--rw-r--r--   0        0        0      257 2024-04-29 14:18:53.883210 test_pypi_package_example-1.7.0.dev1714390008/src/test_pypi_package_example/__init__.py
--rw-r--r--   0        0        0      266 2024-04-29 13:44:37.003930 test_pypi_package_example-1.7.0.dev1714390008/src/test_pypi_package_example/main.py
--rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 test_pypi_package_example-1.7.0.dev1714390008/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-04-29 17:44:05.432184 test_pypi_package_example-1.7.0.dev1714398267/LICENSE
+-rw-r--r--   0        0        0       36 2024-04-29 14:35:36.566311 test_pypi_package_example-1.7.0.dev1714398267/README.md
+-rw-r--r--   0        0        0      516 2024-04-29 17:44:28.304266 test_pypi_package_example-1.7.0.dev1714398267/pyproject.toml
+-rw-r--r--   0        0        0      257 2024-04-29 14:18:53.883210 test_pypi_package_example-1.7.0.dev1714398267/src/test_pypi_package_example/__init__.py
+-rw-r--r--   0        0        0      266 2024-04-29 13:44:37.003930 test_pypi_package_example-1.7.0.dev1714398267/src/test_pypi_package_example/main.py
+-rw-r--r--   0        0        0      307 1970-01-01 00:00:00.000000 test_pypi_package_example-1.7.0.dev1714398267/PKG-INFO
```

### Comparing `test_pypi_package_example-1.7.0.dev1714390008/LICENSE` & `test_pypi_package_example-1.7.0.dev1714398267/LICENSE`

 * *Files identical despite different names*

### Comparing `test_pypi_package_example-1.7.0.dev1714390008/pyproject.toml` & `test_pypi_package_example-1.7.0.dev1714398267/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "test-pypi-package-example"
-version = "1.7.0.dev1714390008"
+version = "1.7.0.dev1714398267"
 description = ""
 authors = ["Lemuel Watts <Watts_Lemuel@bah.com>"]
 readme = "README.md"
 packages = [{include = "test_pypi_package_example", from = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.11.4, <3.12"
```

