# Comparing `tmp/zetl-3.3.8.tar.gz` & `tmp/zetl-3.3.9.tar.gz`

## Comparing `zetl-3.3.8.tar` & `zetl-3.3.9.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 zetl-3.3.8/PyPI-Recovery-Codes-iamthedave-2024-04-29T14_24_52.946204.txt
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 zetl-3.3.8/testszetl_pythonscript_temp.log
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/.schemawiz_config3
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/1.CURRENT_DATE.sql
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/BMONAS-Finalresend.csv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/__init__.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/common.py
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/local_sqlite_db
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/menu.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/mysql_export.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/mysql_extract.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/mysql_import.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/postgres_export.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/postgres_extract.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/postgres_import.py
--rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/run.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sample.csv
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sample7.csv
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sqlite_export.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sqlite_extract.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/sqlite_import.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/view.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/z.sample8.ddl
--rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl.db
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_this_file.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_this_folder.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1/0.init.sql
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1/10.version_check.sql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl1 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl2/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl2/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl2 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl2 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl3/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl3/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl3 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl3 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy - Copy/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy - Copy/z_etl.csv
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/0.version_check.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/z_etl.csv
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/another_postgrescheck.sql
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/check.sql
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/postgrescheck.sql
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 zetl-3.3.8/src/zetl/zetl_scripts/test/z_etl.csv
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/.schemawiz_config3
--rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/backup.bat
--rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/chk_zetl.bat
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/floats.csv
--rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/local_sqlite_db
--rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/restore.bat
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/sample.csv
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/sample.tsv
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/sampletable.ddl
--rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/tesla.csv
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/z_etl.csv
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/z_log.csv
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_pythonscript_temp.log
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/audit/10.audit.sql
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/audit/z_etl.csv
--rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/backup/15.extract_csv_files.bat
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/backup/z_etl.csv
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/demo2/1.somethings.sql
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/demo2/z_etl.csv
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/demo3/1.tms.sql
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/demo3/z_etl.csv
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/empty_log/1.truncate_zlog.sql
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/empty_log/z_etl.csv
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/view_log/1.latest_log_view.sql
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 zetl-3.3.8/tests/zetl_scripts/view_log/z_etl.csv
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 zetl-3.3.8/.gitignore
--rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 zetl-3.3.8/LICENSE
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 zetl-3.3.8/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 zetl-3.3.8/pyproject.toml
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 zetl-3.3.8/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 zetl-3.3.9/PyPI-Recovery-Codes-iamthedave-2024-04-29T14_24_52.946204.txt
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 zetl-3.3.9/testszetl_pythonscript_temp.log
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/.schemawiz_config3
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/1.CURRENT_DATE.sql
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/BMONAS-Finalresend.csv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/__init__.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/common.py
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/local_sqlite_db
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/menu.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/mysql_export.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/mysql_extract.py
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/mysql_import.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/postgres_export.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/postgres_extract.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/postgres_import.py
+-rw-r--r--   0        0        0    29892 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/run.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/sample.csv
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/sample7.csv
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/sqlite_export.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/sqlite_extract.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/sqlite_import.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/view.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/z.sample8.ddl
+-rw-r--r--   0        0        0    32768 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl.db
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_this_file.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_this_folder.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl1/0.init.sql
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl1/10.version_check.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl1/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl1 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl1 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl2/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl2/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl2 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl2 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl3/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl3/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl3 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl3 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl4/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl4/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl4 - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl4 - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl4 - Copy - Copy/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl4 - Copy - Copy/z_etl.csv
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/0.version_check.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/etl4 - Copy - Copy (2)/z_etl.csv
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/test/another_postgrescheck.sql
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/test/check.sql
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/test/postgrescheck.sql
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 zetl-3.3.9/src/zetl/zetl_scripts/test/z_etl.csv
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/.schemawiz_config3
+-rwxr-xr-x   0        0        0      316 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/backup.bat
+-rwxr-xr-x   0        0        0       69 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/chk_zetl.bat
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/floats.csv
+-rw-r--r--   0        0        0    57344 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/local_sqlite_db
+-rwxr-xr-x   0        0        0      295 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/restore.bat
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/sample.csv
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/sample.tsv
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/sampletable.ddl
+-rw-r--r--   0        0        0    50392 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/tesla.csv
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/z_etl.csv
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/z_log.csv
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_pythonscript_temp.log
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/audit/10.audit.sql
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/audit/z_etl.csv
+-rwxr-xr-x   0        0        0      237 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/backup/15.extract_csv_files.bat
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/backup/z_etl.csv
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/demo2/1.somethings.sql
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/demo2/z_etl.csv
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/demo3/1.tms.sql
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/demo3/z_etl.csv
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/empty_log/1.truncate_zlog.sql
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/empty_log/z_etl.csv
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/view_log/1.latest_log_view.sql
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 zetl-3.3.9/tests/zetl_scripts/view_log/z_etl.csv
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 zetl-3.3.9/.gitignore
+-rw-r--r--   0        0        0    18431 2020-02-02 00:00:00.000000 zetl-3.3.9/LICENSE
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 zetl-3.3.9/README.md
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 zetl-3.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 zetl-3.3.9/PKG-INFO
```

### Comparing `zetl-3.3.8/src/zetl/BMONAS-Finalresend.csv` & `zetl-3.3.9/src/zetl/BMONAS-Finalresend.csv`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/common.py` & `zetl-3.3.9/src/zetl/common.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/local_sqlite_db` & `zetl-3.3.9/src/zetl/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/menu.py` & `zetl-3.3.9/src/zetl/menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 				em.run_zetl(em.etl_list[user_selection])
 			else:
 				print("You broke something ")
 
 class etl_menu:
 	def get_dir_separator(self):
 		somepath = os.getcwd()
-		if somepath.find('/'):
+		if somepath.find('/') > -1:
 			self.dir_sep = '/'
 		else:
 			self.dir_sep = '\\'
 
 		return self.dir_sep
 
 	def __init__(self):
```

### Comparing `zetl-3.3.8/src/zetl/mysql_export.py` & `zetl-3.3.9/src/zetl/mysql_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/mysql_extract.py` & `zetl-3.3.9/src/zetl/mysql_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/mysql_import.py` & `zetl-3.3.9/src/zetl/mysql_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 		print('mysql_import.py [csv_filename] [tablename] [WithTruncate]') 
 		print('')
 		print('bool WithTruncate = [True,False]')
 
 class dbimport():
 	def get_dir_separator(self):
 			somepath = os.getcwd()
-		if somepath.find('/'):
+		if somepath.find('/') > -1:
 			self.dir_sep = '/'
 		else:
 			self.dir_sep = '\\'
 
 		return self.dir_sep
 
 	def __init__(self,csv_filename,tablename='',WithTruncate=False):
```

### Comparing `zetl-3.3.8/src/zetl/postgres_export.py` & `zetl-3.3.9/src/zetl/postgres_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/postgres_extract.py` & `zetl-3.3.9/src/zetl/postgres_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/postgres_import.py` & `zetl-3.3.9/src/zetl/postgres_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 		print('')
 		print('bool WithTruncate = [True,False]')
 
 
 class dbimport():
 	def get_dir_separator(self):
 			somepath = os.getcwd()
-		if somepath.find('/'):
+		if somepath.find('/') > -1:
 			self.dir_sep = '/'
 		else:
 			self.dir_sep = '\\'
 
 		return self.dir_sep
 	def __init__(self,csv_filename,tablename='',WithTruncate=False):
 		self.dir_sep = get_dir_separator()
```

### Comparing `zetl-3.3.8/src/zetl/run.py` & `zetl-3.3.9/src/zetl/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import sys
 import os
 import re
 from datetime import *
 
 def get_dir_separator():
 	somepath = os.getcwd()
-	if somepath.find('/'):
+	if somepath.find('/') > -1:
 		dir_sep = '/'
 	else:
 		dir_sep = '\\'
 
 	return dir_sep
 
 def main():
```

### Comparing `zetl-3.3.8/src/zetl/sqlite_export.py` & `zetl-3.3.9/src/zetl/sqlite_export.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/sqlite_extract.py` & `zetl-3.3.9/src/zetl/sqlite_extract.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/sqlite_import.py` & `zetl-3.3.9/src/zetl/sqlite_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 		print('sqlite_import.py [csv_filename] [tablename] [WithTruncate]') 
 		print('')
 		print('bool WithTruncate = [True,False]')
 
 class dbimport():
 	def get_dir_separator(self):
 		somepath = os.getcwd()
-		if somepath.find('/'):
+		if somepath.find('/') > -1:
 			dir_sep = '/'
 		else:
 			dir_sep = '\\'
 
 		return dir_sep
 	def __init__(self,csv_filename,tablename='',WithTruncate=False):
 		tbl = tablename
```

### Comparing `zetl-3.3.8/src/zetl/view.py` & `zetl-3.3.9/src/zetl/view.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/zetl.db` & `zetl-3.3.9/src/zetl/zetl.db`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/zetl_this_file.py` & `zetl-3.3.9/src/zetl/zetl_this_file.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/zetl_this_folder.py` & `zetl-3.3.9/src/zetl/zetl_this_folder.py`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql` & `zetl-3.3.9/src/zetl/zetl_scripts/test/1.another_mysqlcheck.sql`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/tests/local_sqlite_db` & `zetl-3.3.9/tests/local_sqlite_db`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/tests/tesla.csv` & `zetl-3.3.9/tests/tesla.csv`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/tests/zetl_pythonscript_temp.log` & `zetl-3.3.9/tests/zetl_pythonscript_temp.log`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/LICENSE` & `zetl-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/README.md` & `zetl-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `zetl-3.3.8/pyproject.toml` & `zetl-3.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling","schemawizard_package","postgresdave_package","mysqldave_package","garbledave_package"]
 
 build-backend = "hatchling.build"
 
 [project]
 name = "zetl"
-version = "3.3.8"
+version = "3.3.9"
 dependencies = [
   'schemawizard_package >= 2.5.1',
   'postgresdave_package >= 1.8.0',
   'mysqldave_package >= 1.5.0',
   'sqlitedave_package >= 1.3.0',
   'garbledave_package >= 1.0.0 '
 ]
```

### Comparing `zetl-3.3.8/PKG-INFO` & `zetl-3.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zetl
-Version: 3.3.8
+Version: 3.3.9
 Summary: A simple ETL framework for Python, SQL and BAT files which uses a Postgres database for activity logging.
 Project-URL: Homepage, https://github.com/daveskura/zetl
 Project-URL: Author Linkedin, https://www.linkedin.com/in/2166883
 Author-email: Dave Skura <dskura@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

