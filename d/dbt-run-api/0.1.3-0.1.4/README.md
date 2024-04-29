# Comparing `tmp/dbt_run_api-0.1.3.tar.gz` & `tmp/dbt_run_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_run_api-0.1.3.tar", max compression
+gzip compressed data, was "dbt_run_api-0.1.4.tar", max compression
```

## Comparing `dbt_run_api-0.1.3.tar` & `dbt_run_api-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1060 2024-04-25 10:34:28.761518 dbt_run_api-0.1.3/LICENSE
--rw-r--r--   0        0        0      979 2024-04-25 10:34:28.765518 dbt_run_api-0.1.3/dbt_run_api/__init__.py
--rw-r--r--   0        0        0      346 2024-04-25 10:34:28.765518 dbt_run_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 dbt_run_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-04-29 10:02:24.047110 dbt_run_api-0.1.4/LICENSE
+-rw-r--r--   0        0        0      949 2024-04-29 10:02:24.047110 dbt_run_api-0.1.4/dbt_run_api/__init__.py
+-rw-r--r--   0        0        0      346 2024-04-29 10:02:24.047110 dbt_run_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 dbt_run_api-0.1.4/PKG-INFO
```

### Comparing `dbt_run_api-0.1.3/LICENSE` & `dbt_run_api-0.1.4/LICENSE`

 * *Files identical despite different names*

