# Comparing `tmp/redshift_client-5.0.1.tar.gz` & `tmp/redshift_client-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redshift_client-5.0.1.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
+gzip compressed data, was "redshift_client-5.1.0.tar", last modified: Tue Jan  1 00:00:00 1980, max compression
```

## Comparing `redshift_client-5.0.1.tar` & `redshift_client-5.1.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 redshift_client-5.0.1/.envrc
--rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 redshift_client-5.0.1/.gitignore
--rw-r--r--   0        0        0     1798 1980-01-01 00:00:00.000000 redshift_client-5.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      314 1980-01-01 00:00:00.000000 redshift_client-5.0.1/.pylintrc
--rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/ci/check.nix
--rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/ci/utils.sh
--rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/default.nix
--rw-r--r--   0        0        0      645 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/deps/arch_lint.nix
--rw-r--r--   0        0        0      345 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/deps/boto3/redshift-stubs.nix
--rw-r--r--   0        0        0      844 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/deps/boto3/stubs.nix
--rw-r--r--   0        0        0     1157 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/deps/default.nix
--rw-r--r--   0        0        0      653 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/deps/fa_purity.nix
--rw-r--r--   0        0        0      206 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/deps/psycopg2/stubs.nix
--rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/dev_env/default.nix
--rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/dev_env/hook.sh
--rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/dev_env/vs_settings.py
--rw-r--r--   0        0        0      310 1980-01-01 00:00:00.000000 redshift_client-5.0.1/build/filter.nix
--rw-r--r--   0        0        0     1913 1980-01-01 00:00:00.000000 redshift_client-5.0.1/flake.lock
--rw-r--r--   0        0        0     1140 1980-01-01 00:00:00.000000 redshift_client-5.0.1/flake.nix
--rw-r--r--   0        0        0      281 1980-01-01 00:00:00.000000 redshift_client-5.0.1/makes.lock.nix
--rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 redshift_client-5.0.1/makes.nix
--rw-r--r--   0        0        0      714 1980-01-01 00:00:00.000000 redshift_client-5.0.1/mypy.ini
--rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 redshift_client-5.0.1/nix.conf
--rw-r--r--   0        0        0      667 1980-01-01 00:00:00.000000 redshift_client-5.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/__init__.py
--rw-r--r--   0        0        0     2770 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/_utils.py
--rw-r--r--   0        0        0      270 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/__init__.py
--rw-r--r--   0        0        0     4554 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_core.py
--rw-r--r--   0        0        0      492 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_factory.py
--rw-r--r--   0        0        0      864 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_schema/__init__.py
--rw-r--r--   0        0        0     7451 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_schema/_methods.py
--rw-r--r--   0        0        0     1065 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_table/__init__.py
--rw-r--r--   0        0        0     2160 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_table/_assert.py
--rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_table/_encode.py
--rw-r--r--   0        0        0    10894 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_table/_methods.py
--rw-r--r--   0        0        0     1922 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/client/_table/_new.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/__init__.py
--rw-r--r--   0        0        0      496 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/column.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/data_type/__init__.py
--rw-r--r--   0        0        0     1589 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/data_type/alias.py
--rw-r--r--   0        0        0     1585 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/data_type/core.py
--rw-r--r--   0        0        0     1565 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/data_type/decode.py
--rw-r--r--   0        0        0      843 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/id_objs.py
--rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/schema.py
--rw-r--r--   0        0        0     6793 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/core/table.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/py.typed
--rw-r--r--   0        0        0      721 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/__init__.py
--rw-r--r--   0        0        0     7989 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_client_1/__init__.py
--rw-r--r--   0        0        0     1295 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_client_1/_assert.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_core/__init__.py
--rw-r--r--   0        0        0      994 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_core/client.py
--rw-r--r--   0        0        0     3164 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_core/connection.py
--rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_core/creds.py
--rw-r--r--   0        0        0     2624 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_core/primitive.py
--rw-r--r--   0        0        0     1029 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_core/query.py
--rw-r--r--   0        0        0      833 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_factory.py
--rw-r--r--   0        0        0     1801 1980-01-01 00:00:00.000000 redshift_client-5.0.1/redshift_client/sql_client/_temp_creds.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.0.1/tests/arch/__init__.py
--rw-r--r--   0        0        0     1858 1980-01-01 00:00:00.000000 redshift_client-5.0.1/tests/arch/arch.py
--rw-r--r--   0        0        0     1055 1980-01-01 00:00:00.000000 redshift_client-5.0.1/tests/arch/test_arch.py
--rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.0.1/tests/py.typed
--rw-r--r--   0        0        0      233 1980-01-01 00:00:00.000000 redshift_client-5.0.1/tests/test_column.py
--rw-r--r--   0        0        0     1618 1980-01-01 00:00:00.000000 redshift_client-5.0.1/tests/test_table.py
--rw-r--r--   0        0        0      462 1980-01-01 00:00:00.000000 redshift_client-5.0.1/tests/test_temp_creds.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 redshift_client-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0       84 1980-01-01 00:00:00.000000 redshift_client-5.1.0/.envrc
+-rw-r--r--   0        0        0       47 1980-01-01 00:00:00.000000 redshift_client-5.1.0/.gitignore
+-rw-r--r--   0        0        0     1798 1980-01-01 00:00:00.000000 redshift_client-5.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      314 1980-01-01 00:00:00.000000 redshift_client-5.1.0/.pylintrc
+-rw-r--r--   0        0        0      262 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/ci/check.nix
+-rw-r--r--   0        0        0      191 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/ci/utils.sh
+-rw-r--r--   0        0        0     1368 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/default.nix
+-rw-r--r--   0        0        0      645 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/arch_lint.nix
+-rw-r--r--   0        0        0      345 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/boto3/redshift-stubs.nix
+-rw-r--r--   0        0        0      844 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/boto3/stubs.nix
+-rw-r--r--   0        0        0     1157 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/default.nix
+-rw-r--r--   0        0        0      653 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/fa_purity.nix
+-rw-r--r--   0        0        0      206 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/deps/psycopg2/stubs.nix
+-rw-r--r--   0        0        0      182 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/dev_env/default.nix
+-rwxr-xr-x   0        0        0      131 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/dev_env/hook.sh
+-rw-r--r--   0        0        0     1482 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/dev_env/vs_settings.py
+-rw-r--r--   0        0        0      310 1980-01-01 00:00:00.000000 redshift_client-5.1.0/build/filter.nix
+-rw-r--r--   0        0        0     1913 1980-01-01 00:00:00.000000 redshift_client-5.1.0/flake.lock
+-rw-r--r--   0        0        0     1140 1980-01-01 00:00:00.000000 redshift_client-5.1.0/flake.nix
+-rw-r--r--   0        0        0      281 1980-01-01 00:00:00.000000 redshift_client-5.1.0/makes.lock.nix
+-rw-r--r--   0        0        0      680 1980-01-01 00:00:00.000000 redshift_client-5.1.0/makes.nix
+-rw-r--r--   0        0        0      714 1980-01-01 00:00:00.000000 redshift_client-5.1.0/mypy.ini
+-rw-r--r--   0        0        0      260 1980-01-01 00:00:00.000000 redshift_client-5.1.0/nix.conf
+-rw-r--r--   0        0        0      667 1980-01-01 00:00:00.000000 redshift_client-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0      112 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/__init__.py
+-rw-r--r--   0        0        0     2996 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/_utils.py
+-rw-r--r--   0        0        0      336 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/__init__.py
+-rw-r--r--   0        0        0     6335 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_core.py
+-rw-r--r--   0        0        0      941 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_factory.py
+-rw-r--r--   0        0        0      864 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_schema/__init__.py
+-rw-r--r--   0        0        0     7451 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_schema/_methods.py
+-rw-r--r--   0        0        0     1120 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/__init__.py
+-rw-r--r--   0        0        0     2160 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/_assert.py
+-rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/_encode.py
+-rw-r--r--   0        0        0    12271 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/_methods.py
+-rw-r--r--   0        0        0     1922 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/client/_table/_new.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/__init__.py
+-rw-r--r--   0        0        0      496 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/column.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/data_type/__init__.py
+-rw-r--r--   0        0        0     1589 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/data_type/alias.py
+-rw-r--r--   0        0        0     1585 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/data_type/core.py
+-rw-r--r--   0        0        0     1565 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/data_type/decode.py
+-rw-r--r--   0        0        0      843 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/id_objs.py
+-rw-r--r--   0        0        0      589 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/schema.py
+-rw-r--r--   0        0        0     6793 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/core/table.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/py.typed
+-rw-r--r--   0        0        0      751 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/__init__.py
+-rw-r--r--   0        0        0     8811 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_client_1/__init__.py
+-rw-r--r--   0        0        0     1295 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_client_1/_assert.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/__init__.py
+-rw-r--r--   0        0        0     1167 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/client.py
+-rw-r--r--   0        0        0     3164 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/connection.py
+-rw-r--r--   0        0        0      283 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/creds.py
+-rw-r--r--   0        0        0     2624 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/primitive.py
+-rw-r--r--   0        0        0     1029 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_core/query.py
+-rw-r--r--   0        0        0      833 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_factory.py
+-rw-r--r--   0        0        0     1801 1980-01-01 00:00:00.000000 redshift_client-5.1.0/redshift_client/sql_client/_temp_creds.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/arch/__init__.py
+-rw-r--r--   0        0        0     1858 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/arch/arch.py
+-rw-r--r--   0        0        0     1055 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/arch/test_arch.py
+-rw-r--r--   0        0        0        0 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/py.typed
+-rw-r--r--   0        0        0      233 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/test_column.py
+-rw-r--r--   0        0        0     1618 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/test_table.py
+-rw-r--r--   0        0        0      462 1980-01-01 00:00:00.000000 redshift_client-5.1.0/tests/test_temp_creds.py
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 redshift_client-5.1.0/PKG-INFO
```

### Comparing `redshift_client-5.0.1/.gitlab-ci.yml` & `redshift_client-5.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/build/default.nix` & `redshift_client-5.1.0/build/default.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/build/deps/arch_lint.nix` & `redshift_client-5.1.0/build/deps/arch_lint.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/build/deps/boto3/stubs.nix` & `redshift_client-5.1.0/build/deps/boto3/stubs.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/build/deps/default.nix` & `redshift_client-5.1.0/build/deps/default.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/build/deps/fa_purity.nix` & `redshift_client-5.1.0/build/deps/fa_purity.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/build/dev_env/vs_settings.py` & `redshift_client-5.1.0/build/dev_env/vs_settings.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/flake.lock` & `redshift_client-5.1.0/flake.lock`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/flake.nix` & `redshift_client-5.1.0/flake.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/makes.nix` & `redshift_client-5.1.0/makes.nix`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/mypy.ini` & `redshift_client-5.1.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/pyproject.toml` & `redshift_client-5.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/_utils.py` & `redshift_client-5.1.0/redshift_client/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,19 +48,27 @@
     _inner: FrozenSet[_T]
 
     @staticmethod
     def new(item: _T) -> NonEmptySet[_T]:
         return NonEmptySet(_Private(), frozenset([item]))
 
     @staticmethod
-    def from_set(items: FrozenSet[_T]) -> ResultE[NonEmptySet[_T]]:
+    def optional_non_empty(items: FrozenSet[_T]) -> Maybe[NonEmptySet[_T]]:
         if items != frozenset([]):
-            return Result.success(NonEmptySet(_Private(), frozenset(items)))
+            return Maybe.from_value(NonEmptySet(_Private(), frozenset(items)))
+        return Maybe.empty()
+
+    @classmethod
+    def from_set(cls, items: FrozenSet[_T]) -> ResultE[NonEmptySet[_T]]:
         error = ValueError("`FrozenSet` must not be empty.")
-        return Result.failure(Exception(error))
+        return (
+            cls.optional_non_empty(items)
+            .to_result()
+            .alt(lambda _: cast_exception(error))
+        )
 
     def to_set(self) -> FrozenSet[_T]:
         return self._inner
 
     def __contains__(self, item: _T) -> bool:
         return item in self._inner
```

### Comparing `redshift_client-5.0.1/redshift_client/client/_schema/__init__.py` & `redshift_client-5.1.0/redshift_client/client/_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/client/_schema/_methods.py` & `redshift_client-5.1.0/redshift_client/client/_schema/_methods.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/client/_table/__init__.py` & `redshift_client-5.1.0/redshift_client/client/_table/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 def new_table_client(sql: SqlClient) -> TableClient:
     return TableClient(
         lambda t, p, r: _methods.unload(sql, t, p, r),
         lambda t, m, r, h: _methods.load(sql, t, m, r, h),
         lambda t: _methods.get(sql, t),
         lambda t: _methods.exist(sql, t),
         lambda i, t, s, m: _methods.insert(sql, i, t, s, m),
+        lambda i, g: _methods.named_insert(sql, i, g),
         lambda t, n: _methods.rename(sql, t, n),
         lambda t: _methods.delete(sql, t, False),
         lambda t: _methods.delete(sql, t, True),
         lambda t, c: _methods.add_column(sql, t, c),
         lambda t, d: _methods.add_columns(sql, t, d),
         lambda i, t, _: _new.new(sql, i, t, False),
         lambda i, t, _: _new.new(sql, i, t, True),
```

### Comparing `redshift_client-5.0.1/redshift_client/client/_table/_assert.py` & `redshift_client-5.1.0/redshift_client/client/_table/_assert.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/client/_table/_methods.py` & `redshift_client-5.1.0/redshift_client/client/_table/_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,16 +33,18 @@
     cast_exception,
 )
 from redshift_client import (
     _utils,
 )
 from redshift_client.client._core import (
     AwsRole,
+    GroupedRows,
     NanHandler,
     S3Prefix,
+    TableRow,
 )
 from redshift_client.core.column import (
     Column,
     ColumnId,
     ColumnObj,
 )
 from redshift_client.core.id_objs import (
@@ -58,14 +60,15 @@
     DbPrimitive,
     DbPrimitiveFactory,
     Limit,
     Query,
     QueryValues,
     RowData,
     SqlClient,
+    Template,
 )
 from typing import (
     Dict,
     TypeVar,
 )
 
 _T = TypeVar("_T")
@@ -73,14 +76,18 @@
 
 def _assert_bool(raw: _T) -> bool:
     if isinstance(raw, bool):
         return raw
     raise TypeError("Expected bool")
 
 
+def _int_to_str(value: int) -> str:
+    return str(value)
+
+
 def unload(
     client: SqlClient, table: DbTableId, prefix: S3Prefix, role: AwsRole
 ) -> Cmd[ResultE[ManifestId]]:
     """
     prefix: a s3 uri prefix
     role: an aws role id-arn
     """
@@ -237,14 +244,53 @@
     for i, c in enumerate(table.order):
         identifiers[f"field_{i}"] = c.name.to_str()
     return client.values(
         Query.dynamic_query(stm, FrozenDict(identifiers)), items, limit
     )
 
 
+def named_insert(
+    client: SqlClient,
+    table_id: DbTableId,
+    data: GroupedRows,
+) -> Cmd[ResultE[None]]:
+    _enumerated = PureIterFactory.from_list(data.table.order).enumerate(1)
+    _field_placeholders = _enumerated.map(
+        lambda t: "{field_" + _int_to_str(t[0]) + "}"
+    )
+    _template = _enumerated.map(
+        lambda t: "%(field_" + _int_to_str(t[0]) + ")s"
+    )
+    _field_map = FrozenDict(
+        dict(_enumerated.map(lambda t: (t[1], "field_" + _int_to_str(t[0]))))
+    )
+    _fields = ",".join(_field_placeholders)
+    stm = "INSERT INTO {schema}.{table} " f"({_fields}) VALUES %s"
+    identifiers: Dict[str, str] = dict(
+        _enumerated.map(
+            lambda t: ("field_" + _int_to_str(t[0]), t[1].name.to_str())
+        )
+    ) | {
+        "schema": table_id.schema.name.to_str(),
+        "table": table_id.table.name.to_str(),
+    }
+
+    def _to_fields_map(item: TableRow) -> QueryValues:
+        return QueryValues(
+            FrozenDict({_field_map[k]: v for k, v in item.row.items()})
+        )
+
+    values = PureIterFactory.from_list(data.rows).map(_to_fields_map)
+    return client.named_values(
+        Query.dynamic_query(stm, FrozenDict(identifiers)),
+        Template(_template.to_list()),
+        values.to_list(),
+    )
+
+
 def rename(
     client: SqlClient, table_id: DbTableId, new_name: str
 ) -> Cmd[ResultE[TableId]]:
     stm = """
         ALTER TABLE {schema}.{table} RENAME TO {new_name}
     """
     identifiers: Dict[str, str] = {
```

### Comparing `redshift_client-5.0.1/redshift_client/client/_table/_new.py` & `redshift_client-5.1.0/redshift_client/client/_table/_new.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/core/data_type/alias.py` & `redshift_client-5.1.0/redshift_client/core/data_type/alias.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/core/data_type/core.py` & `redshift_client-5.1.0/redshift_client/core/data_type/core.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/core/data_type/decode.py` & `redshift_client-5.1.0/redshift_client/core/data_type/decode.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/core/id_objs.py` & `redshift_client-5.1.0/redshift_client/core/id_objs.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/core/schema.py` & `redshift_client-5.1.0/redshift_client/core/schema.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/core/table.py` & `redshift_client-5.1.0/redshift_client/core/table.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/__init__.py` & `redshift_client-5.1.0/redshift_client/sql_client/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ._core.client import (
     Limit,
     QueryValues,
     RowData,
     SqlClient,
+    Template,
 )
 from ._core.connection import (
     DbConnection,
     IsolationLvl,
 )
 from ._core.creds import (
     Credentials,
@@ -38,8 +39,9 @@
     "RowData",
     "QueryValues",
     "Limit",
     "SqlClient",
     "SqlClientFactory",
     "LoginUtils",
     "TempCredsUser",
+    "Template",
 ]
```

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/_client_1/__init__.py` & `redshift_client-5.1.0/redshift_client/sql_client/_client_1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     _assert,
 )
 from .._core.client import (
     Limit,
     QueryValues,
     RowData,
     SqlClient,
+    Template,
 )
 from .._core.primitive import (
     DbPrimitive,
 )
 from .._core.query import (
     Query,
 )
@@ -221,14 +222,35 @@
                     _args,
                     page_size=limit.limit,
                 )
             )
 
         return Cmd.from_cmd(_action)
 
+    def named_values(
+        self, query: Query, template: Template, args: FrozenList[QueryValues]
+    ) -> Cmd[ResultE[None]]:
+        def _action() -> ResultE[None]:
+            self._log.debug("Executing query over values: %s", query.statement)
+            _args: PureIter[
+                FrozenDict[str, Primitive | datetime]
+            ] = PureIterFactory.from_list(args).map(
+                lambda q: _to_raw(q.values)
+            )
+            return _handle_psycopg_errors(
+                lambda: extras.execute_values(  # type: ignore[misc]
+                    self._cursor,
+                    query.statement,
+                    _args,
+                    template=",".join(template.keys),
+                )
+            )
+
+        return Cmd.from_cmd(_action)
+
     def fetch_one(self) -> Cmd[ResultE[Maybe[RowData]]]:
         def _action() -> ResultE[Maybe[RowData]]:
             self._log.debug("Fetching one row")
             return (
                 _handle_psycopg_errors(
                     lambda: _assert.assert_fetch_one(self._cursor.fetchone())  # type: ignore[misc]
                 )
@@ -275,12 +297,13 @@
 
 def new_sql_client(_log: Logger, _cursor: CursorStub) -> SqlClient:
     _client = _SqlClient_1(_log, _cursor)
     return SqlClient(
         _client.execute,
         _client.batch,
         _client.values,
+        _client.named_values,
         _client.fetch_one(),
         _client.fetch_all(),
         _client.fetch_chunk,
         _client.fetch_chunks_stream,
     )
```

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/_client_1/_assert.py` & `redshift_client-5.1.0/redshift_client/sql_client/_client_1/_assert.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/_core/client.py` & `redshift_client-5.1.0/redshift_client/sql_client/_core/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,20 +28,28 @@
 
 @dataclass(frozen=True)
 class QueryValues:
     values: FrozenDict[str, DbPrimitive]
 
 
 @dataclass(frozen=True)
+class Template:
+    keys: FrozenList[str]
+
+
+@dataclass(frozen=True)
 class Limit:
     limit: int
 
 
 @dataclass(frozen=True)
 class SqlClient:
     execute: Callable[[Query, QueryValues | None], Cmd[ResultE[None]]]
     batch: Callable[[Query, FrozenList[QueryValues]], Cmd[ResultE[None]]]
     values: Callable[[Query, PureIter[RowData], Limit], Cmd[ResultE[None]]]
+    named_values: Callable[
+        [Query, Template, FrozenList[QueryValues]], Cmd[ResultE[None]]
+    ]
     fetch_one: Cmd[ResultE[Maybe[RowData]]]
     fetch_all: Cmd[ResultE[FrozenList[RowData]]]
     fetch_chunk: Callable[[int], Cmd[ResultE[FrozenList[RowData]]]]
     fetch_chunks_stream: Callable[[int], Stream[ResultE[FrozenList[RowData]]]]
```

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/_core/connection.py` & `redshift_client-5.1.0/redshift_client/sql_client/_core/connection.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/_core/primitive.py` & `redshift_client-5.1.0/redshift_client/sql_client/_core/primitive.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/_core/query.py` & `redshift_client-5.1.0/redshift_client/sql_client/_core/query.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/_factory.py` & `redshift_client-5.1.0/redshift_client/sql_client/_factory.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/redshift_client/sql_client/_temp_creds.py` & `redshift_client-5.1.0/redshift_client/sql_client/_temp_creds.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/tests/arch/arch.py` & `redshift_client-5.1.0/tests/arch/arch.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/tests/arch/test_arch.py` & `redshift_client-5.1.0/tests/arch/test_arch.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/tests/test_table.py` & `redshift_client-5.1.0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `redshift_client-5.0.1/PKG-INFO` & `redshift_client-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redshift_client
-Version: 5.0.1
+Version: 5.1.0
 Summary: Redshift client-SDK
 Author-email: Product Team <development@fluidattacks.com>
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: boto3 >=1.28.57, <2.0.0
 Requires-Dist: Deprecated >=1.2.12, <2.0.0
 Requires-Dist: psycopg2 >=2.8.6, <3.0.0
```

