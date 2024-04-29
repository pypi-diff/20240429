# Comparing `tmp/zetl-3.3.7.tar.gz` & `tmp/zetl-3.3.8.tar.gz`

## Comparing `zetl-3.3.7.tar` & `zetl-3.3.8.tar`

### file list

```diff
@@ -1,81 +1,82 @@
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 zetl-3.3.7/testszetl_pythonscript_temp.log
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/.schemawiz_config3
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/1.CURRENT_DATE.sql
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/BMONAS-Finalresend.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/__init__.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/common.py
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/local_sqlite_db
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/menu.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/mysql_export.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/mysql_extract.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/mysql_import.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/postgres_export.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/postgres_extract.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/postgres_import.py
--rw-r--r--   0        0        0    29446 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/run.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/sample.csv
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/sample7.csv
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/sqlite_export.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/sqlite_extract.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/sqlite_import.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/view.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/z.sample8.ddl
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl.db
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_this_file.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_this_folder.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl1/0.init.sql
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl1/10.version_check.sql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl1/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl1 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl1 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl2/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl2/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl2 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl2 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl3/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl3/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl3 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl3 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl4/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl4/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl4 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl4 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl4 - Copy - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl4 - Copy - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/z_etl.csv
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/test/another_postgrescheck.sql
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/test/check.sql
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/test/postgrescheck.sql
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 zetl-3.3.7/src/zetl/zetl_scripts/test/z_etl.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/.schemawiz_config3
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/backup.bat
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/chk_zetl.bat
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/floats.csv
--rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/local_sqlite_db
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/restore.bat
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/sample.csv
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/sample.tsv
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/sampletable.ddl
--rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/tesla.csv
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/z_etl.csv
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/z_log.csv
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_pythonscript_temp.log
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/audit/10.audit.sql
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/audit/z_etl.csv
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/backup/15.extract_csv_files.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/backup/z_etl.csv
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/demo2/1.somethings.sql
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/demo2/z_etl.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/demo3/1.tms.sql
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/demo3/z_etl.csv
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/empty_log/1.truncate_zlog.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/empty_log/z_etl.csv
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/view_log/1.latest_log_view.sql
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 zetl-3.3.7/tests/zetl_scripts/view_log/z_etl.csv
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 zetl-3.3.7/.gitignore
--rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 zetl-3.3.7/LICENSE
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 zetl-3.3.7/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 zetl-3.3.7/pyproject.toml
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 zetl-3.3.7/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 zetl-3.3.8/PyPI-Recovery-Codes-iamthedave-2024-04-29T14_24_52.946204.txt
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 zetl-3.3.8/testszetl_pythonscript_temp.log
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/.schemawiz_config3
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/1.CURRENT_DATE.sql
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/BMONAS-Finalresend.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/__init__.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/common.py
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/local_sqlite_db
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/menu.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/mysql_export.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/mysql_extract.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/mysql_import.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/postgres_export.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/postgres_extract.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/postgres_import.py
+-rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/run.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sample.csv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sample7.csv
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sqlite_export.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sqlite_extract.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sqlite_import.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/view.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/z.sample8.ddl
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl.db
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_this_file.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_this_folder.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1/0.init.sql
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1/10.version_check.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl2/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl2/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl2 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl2 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl3/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl3/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl3 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl3 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/z_etl.csv
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/another_postgrescheck.sql
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/check.sql
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/postgrescheck.sql
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/z_etl.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/.schemawiz_config3
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/backup.bat
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/chk_zetl.bat
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/floats.csv
+-rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/local_sqlite_db
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/restore.bat
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/sample.csv
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/sample.tsv
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/sampletable.ddl
+-rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/tesla.csv
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/z_etl.csv
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/z_log.csv
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_pythonscript_temp.log
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/audit/10.audit.sql
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/audit/z_etl.csv
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/backup/15.extract_csv_files.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/backup/z_etl.csv
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/demo2/1.somethings.sql
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/demo2/z_etl.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/demo3/1.tms.sql
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/demo3/z_etl.csv
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/empty_log/1.truncate_zlog.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/empty_log/z_etl.csv
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/view_log/1.latest_log_view.sql
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/view_log/z_etl.csv
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 zetl-3.3.8/.gitignore
+-rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 zetl-3.3.8/LICENSE
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 zetl-3.3.8/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 zetl-3.3.8/pyproject.toml
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 zetl-3.3.8/PKG-INFO
```

### Comparing `zetl-3.3.7/src/zetl/BMONAS-Finalresend.csv` & `zetl-3.3.8/src/zetl/BMONAS-Finalresend.csv`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/common.py` & `zetl-3.3.8/src/zetl/common.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/local_sqlite_db` & `zetl-3.3.8/src/zetl/local_sqlite_db`

 * *Files 4% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -26,15 +26,15 @@
 				activity_type real PRIMARY KEY,
 				currently text, 
 				previously text, 
 				keyfld text, 
 				prvkeyfld text, 
 				dtm text
 			);
-INSERT INTO z_activity VALUES(NULL,'idle','Running etl1',NULL,NULL,NULL);
+INSERT INTO z_activity VALUES(NULL,'idle','Running \etl1',NULL,NULL,NULL);
 CREATE TABLE z_global (
 			name text PRIMARY KEY,
 			value text
 		);
 INSERT INTO z_global VALUES('gblvar_rundate','CURRENT_DATE');
 INSERT INTO z_global VALUES('gblvar_label','all fruits');
 CREATE TABLE z_log (
```

### Comparing `zetl-3.3.7/src/zetl/menu.py` & `zetl-3.3.8/src/zetl/menu.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,16 +26,26 @@
 			elif user_selection <= option_count and user_selection > -1:
 				print("Running ", user_selection, em.etl_list[user_selection])
 				em.run_zetl(em.etl_list[user_selection])
 			else:
 				print("You broke something ")
 
 class etl_menu:
+	def get_dir_separator(self):
+		somepath = os.getcwd()
+		if somepath.find('/'):
+			self.dir_sep = '/'
+		else:
+			self.dir_sep = '\\'
+
+		return self.dir_sep
+
 	def __init__(self):
-		self.etl_path = os.getcwd() + '\\zetl_scripts'
+		self.dir_sep = self.get_dir_separator()
+		self.etl_path = os.getcwd() + self.dir_sep + 'zetl_scripts'
 		self.etl_list = []
 		self.etlcount = 0
 		self.findetls()
 
 	def run_zetl(self,etl_name_to_run):
 		run_parameter = ''
 		my_zetl = zetl()
@@ -43,15 +53,15 @@
 		my_zetl.zetldb.load_folders_to_zetl() 
 		my_zetl.proper_run(etl_name_to_run,run_parameter)
 
 	def findetls(self):
 		self.etl_list.append('exit from zetl.menu')
 		subfolders = [ f.path for f in os.scandir(self.etl_path) if f.is_dir() ]
 		for etlwithpath in subfolders:
-			etl = etlwithpath.split(self.etl_path+'\\')[1]
+			etl = etlwithpath.split(self.etl_path)[1]
 			self.etl_list.append(etl)
 		self.etlcount = len(self.etl_list)
 
 	def show_menu(self):
 
 		print ("zetl menu v1.0 \n --------------") #
 		for nbr in range(0,self.etlcount):
```

### Comparing `zetl-3.3.7/src/zetl/mysql_export.py` & `zetl-3.3.8/src/zetl/mysql_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/mysql_extract.py` & `zetl-3.3.8/src/zetl/mysql_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/mysql_import.py` & `zetl-3.3.8/src/zetl/sqlite_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
   Dave Skura,2023
 """
 import sys
 from schemawizard_package.schemawizard import schemawiz
 
 def main():
-	if len(sys.argv) == 1 or sys.argv[1] == 'mysql_import.py': # no parameters
-		print('usage: ')
-		print('mysql_import.py [csv_filename] [tablename] [WithTruncate]') 
+	if len(sys.argv) == 1 or sys.argv[1] == 'sqlite_import.py': # no parameters
+		print('usage: \n')
+		print('sqlite_import.py [csv_filename] [tablename] [WithTruncate]') 
 		print('')
-		print('bool WithTruncate = [True,False]')
+
+		print("\t - text csv_filename = 'anyfilename.csv'")
+		print("\t - text tablename = 'anytablename'")
+		print('\t - bool WithTruncate = [True,False]\n')
 
 	elif (len(sys.argv) == 2) : 
 		csv_filename = sys.argv[1]
 		myexp = dbimport(csv_filename)
 
 	elif (len(sys.argv) == 3) : 
 		csv_filename = sys.argv[1]
@@ -28,48 +31,57 @@
 
 		myexp = dbimport(csv_filename,tablename,WithTruncate)
 
 	else:
 		print('Error: Incorrect number of parameters.')
 		print('')
 		print('usage: ')
-		print('mysql_import.py [csv_filename] [tablename] [WithTruncate]') 
+		print('sqlite_import.py [csv_filename] [tablename] [WithTruncate]') 
 		print('')
 		print('bool WithTruncate = [True,False]')
 
 class dbimport():
+	def get_dir_separator(self):
+		somepath = os.getcwd()
+		if somepath.find('/'):
+			dir_sep = '/'
+		else:
+			dir_sep = '\\'
+
+		return dir_sep
 	def __init__(self,csv_filename,tablename='',WithTruncate=False):
 		tbl = tablename
 		dber = schemawiz()
-		if ((tablename != '') and (dber.dbthings.mysql_db.does_table_exist(tablename))):
-			dber.justload_mysql_from_csv(csv_filename,tablename,WithTruncate)
+		if ((tablename != '') and (dber.dbthings.sqlite_db.does_table_exist(tablename))):
+			dber.justload_sqlite_from_csv(csv_filename,tablename,WithTruncate)
 		else:
 			output_ddl_filename = 'z.' + self.getoutputfilename(csv_filename,tablename) + '.ddl'
-			tbl = dber.createload_mysql_from_csv(csv_filename,tablename,output_ddl_filename)
+			tbl = dber.createload_sqlite_from_csv(csv_filename,tablename,output_ddl_filename)
 
-		print(dber.dbthings.mysql_db.queryone('SELECT COUNT(*) FROM ' + tbl))
-		dber.dbthings.mysql_db.close()
+		dber.dbthings.sqlite_db.close()
 
 		print(csv_filename + ' imported to ' + tbl)
 
 	def getoutputfilename(self,csv_filename,ddl_output_filename):
 		# zetl_scripts/someetl/thisfile.csv
-		filedelimiter = '\\'
-		if csv_filename.find('/') > -1:
-			filedelimiter = '/'
+		filedelimiter = self.get_dir_separator()
 
 		newfile = ''
 		partlist = csv_filename.split(filedelimiter)
 		if partlist[0] != csv_filename:
 			for i in range(0,len(partlist)-1):
 				newfile += partlist[i] + filedelimiter
 
 		newfile += ddl_output_filename
 		return newfile
 
 if __name__ == '__main__':
-	#myexp = dbimport('BMONAS-Finalresend.csv','sample8',True)
-	#tbl = schemawiz().createload_mysql_from_csv('sample7.csv','restored_sample7')
- 
+	#myexp = dbimport('sample.csv','thistbl',False)
+
+	#tbl = schemawiz().createload_sqlite_from_csv('sample.csv','thistbl')
+	#data = schemawiz().dbthings.sqlite_db.query('SELECT * FROM thistbl')
+	#for row in data:
+	#	print(row)
+
 	main()
```

### Comparing `zetl-3.3.7/src/zetl/postgres_export.py` & `zetl-3.3.8/src/zetl/postgres_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/postgres_extract.py` & `zetl-3.3.8/src/zetl/postgres_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/postgres_import.py` & `zetl-3.3.8/src/zetl/postgres_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
   Dave Skura,2023
 """
-import sys
+import sys,os
 from schemawizard_package.schemawizard import schemawiz
 
 def main():
 	if len(sys.argv) == 1 or sys.argv[1] == 'postgres_import.py': # no parameters
 		print('usage: ')
 		print('postgres_import.py [csv_filename] [tablename] [WithTruncate]') 
 		print('')
@@ -34,33 +34,41 @@
 		print('usage: ')
 		print('postgres_import.py [csv_filename] [tablename] [WithTruncate]') 
 		print('')
 		print('bool WithTruncate = [True,False]')
 
 
 class dbimport():
-	def __init__(self,csv_filename,tablename='',WithTruncate=False):
+	def get_dir_separator(self):
+			somepath = os.getcwd()
+		if somepath.find('/'):
+			self.dir_sep = '/'
+		else:
+			self.dir_sep = '\\'
 
+		return self.dir_sep
+	def __init__(self,csv_filename,tablename='',WithTruncate=False):
+		self.dir_sep = get_dir_separator()
 		tbl = tablename
 		dber = schemawiz()
 		if ((tablename != '') and (dber.dbthings.postgres_db.does_table_exist(tablename))):
 			dber.justload_postgres_from_csv(csv_filename,tablename,WithTruncate)
 		else:
 			output_ddl_filename = self.getoutputfilename(csv_filename,'z.' + tablename) + '.ddl'
 			tbl = dber.createload_postgres_from_csv(csv_filename,tablename,output_ddl_filename)
 
 		print(dber.dbthings.postgres_db.queryone('SELECT COUNT(*) FROM ' + tbl))
 
 		print(csv_filename + ' imported to ' + tbl)
 
 	def getoutputfilename(self,csv_filename,ddl_output_filename):
 		# zetl_scripts/someetl/thisfile.csv
-		filedelimiter = '\\'
-		if csv_filename.find('/') > -1:
-			filedelimiter = '/'
+		filedelimiter = self.dir_sep
+		#if csv_filename.find('/') > -1:
+		#	filedelimiter = '/'
 
 		newfile = ''
 		partlist = csv_filename.split(filedelimiter)
 		if partlist[0] != csv_filename:
 			for i in range(0,len(partlist)-1):
 				newfile += partlist[i] + filedelimiter
```

### Comparing `zetl-3.3.7/src/zetl/run.py` & `zetl-3.3.8/src/zetl/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,28 @@
 
 import warnings
 import sys
 import os
 import re
 from datetime import *
 
+def get_dir_separator():
+	somepath = os.getcwd()
+	if somepath.find('/'):
+		dir_sep = '/'
+	else:
+		dir_sep = '\\'
+
+	return dir_sep
+
 def main():
+	self.dir_sep
+
 	#my_zetl = zetl()
-	#my_zetl = zetl('c:\\dave\\ETL\\DOM_Ranking','c:\\dave\\ETL\\DOM_Ranking\\zetl_scripts')
-	my_zetl = zetl('c:\\dave\\git\zetl\\tests','c:\\dave\\git\zetl\\tests\\zetl_scripts')
+	my_zetl = zetl('c:' + get_dir_separator() +  'dave' + get_dir_separator() +  'git' + get_dir_separator() +  'zetl' + get_dir_separator() +  'tests','c:' + get_dir_separator() +  'dave' + get_dir_separator() +  'git' + get_dir_separator() +  'zetl' + get_dir_separator() +  'tests' + get_dir_separator() +  'zetl_scripts')
 	my_zetl.set_logging_on()
 	my_zetl.zetldb.empty_zetl()						# empty the master zetl table	
 	my_zetl.zetldb.load_folders_to_zetl() # load master zetl table from folders
 
 	if len(sys.argv) == 1 or sys.argv[1] == 'run.py': # no parameters
 		my_zetl.loggerman('')
 		my_zetl.loggerman('usage: ')
@@ -47,28 +57,25 @@
 	#my_zetl.proper_run('etl1','')
 	#my_zetl.proper_run('demo2','')
 	my_zetl.proper_run('audit','')
 	sys.exit(0)
 
 class zetl:
 	def __init__(self,parent_dir = '',script_dir='',silent_on=False):
-		launch_dir =  '.\\'
+		launch_dir =  '.' + get_dir_separator()
 		if parent_dir != '':
-			if len(parent_dir.split('/')) > len(parent_dir.split('\\')):
-				filepath_delimiter = '/'
-			else:
-				filepath_delimiter = '\\'
+			filepath_delimiter = get_dir_separator()
 
 			if parent_dir[-1:] != filepath_delimiter:
 				launch_dir =  parent_dir + filepath_delimiter
 			else:
 				launch_dir = parent_dir
 
 
-		self.script_directory = '.\\zetl_scripts'
+		self.script_directory = '.' + filepath_delimiter +'zetl_scripts'
 
 		if script_dir != '':
 			self.script_directory = script_dir
 
 		#now = (datetime.now())
 		#sztoday=str(now.year) + '-' + ('0' + str(now.month))[-2:] + '-' + str(now.day)
 		self.silent_on = silent_on
@@ -235,15 +242,15 @@
 	def run_one_etl_step(self,etl_name,stepnum,steptablename,cmdfile,run_parameter='',cmdfilename=''):
 		script_variables = {'SHOWQUERY':'True','DB_TYPE':'','DB_USERNAME':'','DB_USERPWD':'','DB_HOST':'','DB_PORT':'','DB_NAME':'','DB_SCHEMA':''}
 		global_variables = {}
 
 		if cmdfilename != '':
 			findcmdfile = cmdfilename
 		else:
-			findcmdfile = self.script_directory + '\\' + etl_name + '\\' + cmdfile
+			findcmdfile = self.script_directory + get_dir_separator() + etl_name + get_dir_separator() + cmdfile
 
 		try:
 			f = open(findcmdfile,'r') 
 			sqlfromfile = f.read()
 
 			f.close()
 		except Exception as e:
@@ -450,17 +457,17 @@
 			consoleoutput = ''
 			stepnum = row[0]
 			steptablename = ''
 			if row[1]:
 				steptablename = row[1]
 
 			cmdfile = row[2]
-			foundfile = folder + '\\' + cmdfile
+			foundfile = folder + get_dir_separator() + cmdfile
 			if cmdfile.lower().endswith('.sql') or cmdfile.lower().endswith('.ddl'):
-				self.run_one_etl_step(folder,stepnum,steptablename,cmdfile,'',folder + '\\' + cmdfile)
+				self.run_one_etl_step(folder,stepnum,steptablename,cmdfile,'',folder + get_dir_separator() + cmdfile)
 
 			elif cmdfile.lower().endswith('.py'):
 
 				lid = self.logstepstart(folder,stepnum,cmdfile,steptablename,'Python script',0)
 
 				self.loggerman('\n file ' + cmdfile + '\n')
 				cmd_to_run = 'py ' + foundfile + ' '
@@ -567,15 +574,15 @@
 			consoleoutput = ''
 			stepnum = row[0]
 			steptablename = ''
 			if row[1]:
 				steptablename = row[1]
 
 			cmdfile = row[2]
-			foundfile = self.script_directory + '\\' + etl_name + '\\' + cmdfile
+			foundfile = self.script_directory + get_dir_separator() + etl_name + get_dir_separator() + cmdfile
 			#print('stepnum = \t\t' + str(stepnum))
 			#print('steptablename = \t' + steptablename)
 			#print('cmdfile = \t\t' + cmdfile)
 			if cmdfile.lower().endswith('.sql') or cmdfile.lower().endswith('.ddl'):
 				self.run_one_etl_step(etl_name,stepnum,steptablename,cmdfile,run_parameter)
 
 			elif cmdfile.lower().endswith('.py'):
@@ -643,15 +650,15 @@
 		return self.zetldb.db.queryone(prm)
 
 
 class zetldbaccess:
 
 	def __init__(self,parent_dir = '',script_dir='',silent_on=False):
 		dbfile = ''
-		launch_dir = '.\\'
+		launch_dir = '.' + get_dir_separator()
 		if parent_dir != '':
 			launch_dir = parent_dir
 
 		
 		dbfile = launch_dir + 'local_sqlite_db'
 		self.db = sqlite_db(dbfile)
 		self.db.connect()
@@ -681,28 +688,28 @@
 		if folder != '':
 			zsql += "WHERE upper(etl_name) like upper('" + folder + "') "
 		zsql += ' ORDER BY etl_name '
 		etl_list = self.db.query(zsql)
 		for etl in etl_list:
 			etl_name = etl[0]
 			qry = "SELECT stepnum,cmdfile,steptablename,estrowcount FROM z_etl WHERE etl_name = '" + etl_name + "' ORDER BY stepnum"
-			csv_filename = folder + '\\z_etl.csv'
+			csv_filename = folder + get_dir_separator() + 'z_etl.csv'
 			self.db.export_query_to_csv(qry,csv_filename)
 
 
 	def export_zetl(self,etl_name =''):
 		zsql = ' SELECT DISTINCT etl_name FROM z_etl '
 		if etl_name != '':
 			zsql += "WHERE upper(etl_name) like upper('" + etl_name + "') "
 		zsql += ' ORDER BY etl_name '
 		etl_list = self.db.query(zsql)
 		for etl in etl_list:
 			etl_name = etl[0]
 			qry = "SELECT stepnum,cmdfile,steptablename,estrowcount FROM z_etl WHERE etl_name = '" + etl_name + "' ORDER BY stepnum"
-			csv_filename = self.script_directory + '\\' + etl_name + '\\z_etl.csv'
+			csv_filename = self.script_directory + get_dir_separator() + etl_name + get_dir_separator() + 'z_etl.csv'
 			self.db.export_query_to_csv(qry,csv_filename)
 
 	def empty_zetl(self,etl_name=''):
 		try:
 			dsql = "DELETE FROM z_etl "
 			if etl_name != '':
 				dsql += " WHERE upper(etl_name) like upper('" + etl_name + "') "
@@ -765,15 +772,15 @@
 		self.db.commit()
 
 	def load_z_etlcsv_if_forced(self,etl_name='',option=''):
 		szdelimiter = ','
 		if (etl_name != '' and option == '-f'):
 			self.empty_zetl()
 			qualified_table = "z_etl"
-			csv_filename = self.script_directory + '\\' + etl_name + '\\z_etl.csv'
+			csv_filename = self.script_directory + get_dir_separator() + etl_name + get_dir_separator() + 'z_etl.csv'
 			f = open(csv_filename,'r')
 			hdrs = f.read(1000).split('\n')[0].strip().split(szdelimiter)
 			f.close()		
 			
 			isqlhdr = 'INSERT INTO ' + qualified_table + '('
 
 			for i in range(0,len(hdrs)):
@@ -813,15 +820,14 @@
 			except:
 					return False
 
 	def add_etl_step(self,p_etl_name,p_etl_step,p_etl_filename):
 		isql = "INSERT INTO z_etl(etl_name,stepnum,cmdfile) VALUES ('" + p_etl_name + "'," + p_etl_step + ",'" + p_etl_filename + "')"
 		self.db.execute(isql)
 		self.db.commit()
-		#print('Adding ' + p_etl_name + '\\' + p_etl_filename)
 
 	def etl_step_exists(self,etl_name,etl_step):
 		sql = "SELECT COUNT(*) FROM z_etl WHERE etl_name = '" + etl_name + "' and stepnum = " + etl_step
 		etlrowcount = self.db.queryone(sql)
 		if etlrowcount == 0:
 			return False
 		else:
@@ -876,19 +882,19 @@
 		etl_folder = self.script_directory 
 		subdirs = [x[0] for x in os.walk(etl_folder)]
 		for i in range(0,len(subdirs)):
 
 			possible_etl_dir = subdirs[i]
 			zetl_foldername_only=possible_etl_dir.split(etl_folder)[1]
 
-			if len(zetl_foldername_only.split('\\')) == 2:
-				etl_name = zetl_foldername_only.split('\\')[1]
+			if len(zetl_foldername_only.split(get_dir_separator())) == 2:
+				etl_name = zetl_foldername_only.split(get_dir_separator())[1]
 
 				if (etl_name != 'zetl_scripts') and (this_etl_name == 'all' or etl_name == this_etl_name):
-					for etl_script_file in os.listdir(etl_folder + '\\' + etl_name):
+					for etl_script_file in os.listdir(etl_folder + get_dir_separator() + etl_name):
 						if etl_script_file.endswith(".sql") or etl_script_file.endswith(".ddl") or etl_script_file.endswith(".py") or etl_script_file.endswith(".bat"):
 							if len(etl_script_file.split('.')) == 3:
 								etl_step = etl_script_file.split('.')[0]
 								file_suffix = etl_script_file.split('.')[1] + '.' + etl_script_file.split('.')[2]
 								if self.is_an_int(etl_step):
 									if not self.etl_step_exists(etl_name,etl_step):
 										self.add_etl_step(etl_name,etl_step,etl_script_file)
```

### Comparing `zetl-3.3.7/src/zetl/sqlite_export.py` & `zetl-3.3.8/src/zetl/sqlite_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/sqlite_extract.py` & `zetl-3.3.8/src/zetl/sqlite_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/sqlite_import.py` & `zetl-3.3.8/src/zetl/mysql_import.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """
   Dave Skura,2023
 """
-import sys
+import sys,os
 from schemawizard_package.schemawizard import schemawiz
 
 def main():
-	if len(sys.argv) == 1 or sys.argv[1] == 'sqlite_import.py': # no parameters
-		print('usage: \n')
-		print('sqlite_import.py [csv_filename] [tablename] [WithTruncate]') 
+	if len(sys.argv) == 1 or sys.argv[1] == 'mysql_import.py': # no parameters
+		print('usage: ')
+		print('mysql_import.py [csv_filename] [tablename] [WithTruncate]') 
 		print('')
-
-		print("\t - text csv_filename = 'anyfilename.csv'")
-		print("\t - text tablename = 'anytablename'")
-		print('\t - bool WithTruncate = [True,False]\n')
+		print('bool WithTruncate = [True,False]')
 
 	elif (len(sys.argv) == 2) : 
 		csv_filename = sys.argv[1]
 		myexp = dbimport(csv_filename)
 
 	elif (len(sys.argv) == 3) : 
 		csv_filename = sys.argv[1]
@@ -31,51 +28,58 @@
 
 		myexp = dbimport(csv_filename,tablename,WithTruncate)
 
 	else:
 		print('Error: Incorrect number of parameters.')
 		print('')
 		print('usage: ')
-		print('sqlite_import.py [csv_filename] [tablename] [WithTruncate]') 
+		print('mysql_import.py [csv_filename] [tablename] [WithTruncate]') 
 		print('')
 		print('bool WithTruncate = [True,False]')
 
 class dbimport():
+	def get_dir_separator(self):
+			somepath = os.getcwd()
+		if somepath.find('/'):
+			self.dir_sep = '/'
+		else:
+			self.dir_sep = '\\'
+
+		return self.dir_sep
+
 	def __init__(self,csv_filename,tablename='',WithTruncate=False):
+		self.dir_sep = self.get_dir_separator()
 		tbl = tablename
 		dber = schemawiz()
-		if ((tablename != '') and (dber.dbthings.sqlite_db.does_table_exist(tablename))):
-			dber.justload_sqlite_from_csv(csv_filename,tablename,WithTruncate)
+		if ((tablename != '') and (dber.dbthings.mysql_db.does_table_exist(tablename))):
+			dber.justload_mysql_from_csv(csv_filename,tablename,WithTruncate)
 		else:
 			output_ddl_filename = 'z.' + self.getoutputfilename(csv_filename,tablename) + '.ddl'
-			tbl = dber.createload_sqlite_from_csv(csv_filename,tablename,output_ddl_filename)
+			tbl = dber.createload_mysql_from_csv(csv_filename,tablename,output_ddl_filename)
 
-		dber.dbthings.sqlite_db.close()
+		print(dber.dbthings.mysql_db.queryone('SELECT COUNT(*) FROM ' + tbl))
+		dber.dbthings.mysql_db.close()
 
 		print(csv_filename + ' imported to ' + tbl)
 
 	def getoutputfilename(self,csv_filename,ddl_output_filename):
 		# zetl_scripts/someetl/thisfile.csv
-		filedelimiter = '\\'
+		filedelimiter = self.dir_sep
 		if csv_filename.find('/') > -1:
 			filedelimiter = '/'
 
 		newfile = ''
 		partlist = csv_filename.split(filedelimiter)
 		if partlist[0] != csv_filename:
 			for i in range(0,len(partlist)-1):
 				newfile += partlist[i] + filedelimiter
 
 		newfile += ddl_output_filename
 		return newfile
 
 if __name__ == '__main__':
-	#myexp = dbimport('sample.csv','thistbl',False)
-
-	#tbl = schemawiz().createload_sqlite_from_csv('sample.csv','thistbl')
-	#data = schemawiz().dbthings.sqlite_db.query('SELECT * FROM thistbl')
-	#for row in data:
-	#	print(row)
-
+	#myexp = dbimport('BMONAS-Finalresend.csv','sample8',True)
+	#tbl = schemawiz().createload_mysql_from_csv('sample7.csv','restored_sample7')
+ 
 	main()
```

### Comparing `zetl-3.3.7/src/zetl/view.py` & `zetl-3.3.8/src/zetl/view.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/zetl.db` & `zetl-3.3.8/src/zetl/zetl.db`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/zetl_this_file.py` & `zetl-3.3.8/src/zetl/zetl_this_file.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/zetl_this_folder.py` & `zetl-3.3.8/src/zetl/zetl_this_folder.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql` & `zetl-3.3.8/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/tests/local_sqlite_db` & `zetl-3.3.8/tests/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/tests/tesla.csv` & `zetl-3.3.8/tests/tesla.csv`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/tests/zetl_pythonscript_temp.log` & `zetl-3.3.8/tests/zetl_pythonscript_temp.log`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/LICENSE` & `zetl-3.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/README.md` & `zetl-3.3.8/README.md`

 * *Files identical despite different names*

### Comparing `zetl-3.3.7/pyproject.toml` & `zetl-3.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","schemawizard_package","postgresdave_package","mysqldave_package","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "zetl"
-version = "3.3.7"
+version = "3.3.8"
 dependencies = [
   'schemawizard_package >= 2.5.1',
   'postgresdave_package >= 1.8.0',
   'mysqldave_package >= 1.5.0',
   'sqlitedave_package >= 1.3.0',
   'garbledave_package >= 1.0.0 '
 ]
```

### Comparing `zetl-3.3.7/PKG-INFO` & `zetl-3.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zetl
-Version: 3.3.7
+Version: 3.3.8
 Summary: A simple ETL framework for Python, SQL and BAT files which uses a Postgres database for activity logging.
 Project-URL: Homepage, https://github.com/daveskura/zetl
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

