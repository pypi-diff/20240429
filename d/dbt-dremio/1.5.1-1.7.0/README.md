# Comparing `tmp/dbt-dremio-1.5.1.tar.gz` & `tmp/dbt-dremio-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-dremio-1.5.1.tar", last modified: Thu Feb  1 00:32:02 2024, max compression
+gzip compressed data, was "dbt-dremio-1.7.0.tar", last modified: Mon Apr 29 20:16:08 2024, max compression
```

## Comparing `dbt-dremio-1.5.1.tar` & `dbt-dremio-1.7.0.tar`

### file list

```diff
@@ -1,85 +1,89 @@
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.614905 dbt-dremio-1.5.1/
--rw-r--r--   0 ravjotb    (503) staff       (20)    11348 2022-10-17 23:38:32.000000 dbt-dremio-1.5.1/LICENSE
--rw-r--r--   0 ravjotb    (503) staff       (20)       47 2022-10-17 23:38:32.000000 dbt-dremio-1.5.1/MANIFEST.in
--rw-r--r--   0 ravjotb    (503) staff       (20)     3284 2024-02-01 00:32:02.615000 dbt-dremio-1.5.1/PKG-INFO
--rw-r--r--   0 ravjotb    (503) staff       (20)     2736 2024-02-01 00:31:45.000000 dbt-dremio-1.5.1/README.md
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.583369 dbt-dremio-1.5.1/dbt/
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.583096 dbt-dremio-1.5.1/dbt/adapters/
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.598922 dbt-dremio-1.5.1/dbt/adapters/dremio/
--rw-r--r--   0 ravjotb    (503) staff       (20)      965 2022-11-18 18:42:01.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/__init__.py
--rw-r--r--   0 ravjotb    (503) staff       (20)      595 2024-01-29 22:16:32.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/__version__.py
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.600368 dbt-dremio-1.5.1/dbt/adapters/dremio/api/
--rw-r--r--   0 ravjotb    (503) staff       (20)      737 2022-11-18 18:42:01.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/api/__init__.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     2248 2023-03-14 21:48:59.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/api/authentication.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     6338 2024-01-29 22:16:32.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/api/cursor.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     1552 2022-11-18 18:42:01.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/api/handle.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     3678 2023-03-14 21:48:59.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/api/parameters.py
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.601261 dbt-dremio-1.5.1/dbt/adapters/dremio/api/rest/
--rw-r--r--   0 ravjotb    (503) staff       (20)     7551 2023-03-14 21:48:59.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/api/rest/endpoints.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     1661 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/api/rest/error.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     4914 2022-11-18 18:42:01.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/api/rest/url_builder.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     8565 2024-01-29 22:16:32.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/connections.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     4138 2023-08-11 18:54:16.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/credentials.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     6553 2024-01-31 22:43:13.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/impl.py
--rw-r--r--   0 ravjotb    (503) staff       (20)     3021 2024-01-29 22:16:32.000000 dbt-dremio-1.5.1/dbt/adapters/dremio/relation.py
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.583427 dbt-dremio-1.5.1/dbt/include/
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.602073 dbt-dremio-1.5.1/dbt/include/dremio/
--rw-r--r--   0 ravjotb    (503) staff       (20)       52 2022-10-18 21:16:05.000000 dbt-dremio-1.5.1/dbt/include/dremio/__init__.py
--rw-r--r--   0 ravjotb    (503) staff       (20)      815 2023-03-09 00:07:33.000000 dbt-dremio-1.5.1/dbt/include/dremio/dbt_project.yml
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.584477 dbt-dremio-1.5.1/dbt/include/dremio/macros/
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.604973 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/
--rw-r--r--   0 ravjotb    (503) staff       (20)     2237 2023-02-28 17:07:36.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/apply_grants.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     3980 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/columns.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     2540 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/data_preparation.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1985 2023-02-28 17:07:36.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/external_query.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     5692 2024-01-29 22:16:32.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/format.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     8334 2023-03-09 00:07:33.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/metadata.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1518 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/relation.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1080 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/snapshot.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1932 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/sources.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)      648 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/timestamp.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.605296 dbt-dremio-1.5.1/dbt/include/dremio/macros/builtins/
--rw-r--r--   0 ravjotb    (503) staff       (20)     2382 2024-01-29 22:16:32.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/builtins/builtins.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.606584 dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/
--rw-r--r--   0 ravjotb    (503) staff       (20)     1079 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1223 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1185 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/get_custom_schema.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)      791 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/is_datalake_node.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.607500 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/
--rw-r--r--   0 ravjotb    (503) staff       (20)     1604 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/helpers.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.608335 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/incremental/
--rw-r--r--   0 ravjotb    (503) staff       (20)     5197 2024-01-29 22:16:32.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1613 2023-02-28 17:07:36.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1502 2023-02-28 17:07:36.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/incremental/validate.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.609741 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/reflection/
--rw-r--r--   0 ravjotb    (503) staff       (20)     4326 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/reflection/create_reflection.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1448 2023-02-28 17:07:36.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/reflection/helpers.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     4393 2024-01-26 00:40:03.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/reflection/reflection.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.610201 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/seed/
--rw-r--r--   0 ravjotb    (503) staff       (20)     1823 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/seed/helpers.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     2401 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.611082 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/table/
--rw-r--r--   0 ravjotb    (503) staff       (20)     1956 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/table/alter_pds.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1986 2023-08-11 18:54:16.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/table/create_table_as.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1999 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/table/table.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     2425 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/twin_strategy.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.612154 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/
--rw-r--r--   0 ravjotb    (503) staff       (20)     1445 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/create_or_replace_view.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)      974 2023-08-11 18:54:16.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/create_view_as.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1393 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/helpers.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     1997 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/view.sql
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.613221 dbt-dremio-1.5.1/dbt/include/dremio/macros/utils/
--rw-r--r--   0 ravjotb    (503) staff       (20)      732 2023-02-28 17:07:36.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/utils/array_append.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)      730 2023-02-28 17:07:36.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/utils/array_concat.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)      848 2023-02-28 17:07:36.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/utils/array_construct.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)      104 2023-02-01 21:41:10.000000 dbt-dremio-1.5.1/dbt/include/dremio/macros/utils/data_types.sql
--rw-r--r--   0 ravjotb    (503) staff       (20)     2097 2023-03-10 23:06:14.000000 dbt-dremio-1.5.1/dbt/include/dremio/profile_template.yml
-drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-02-01 00:32:02.614757 dbt-dremio-1.5.1/dbt_dremio.egg-info/
--rw-r--r--   0 ravjotb    (503) staff       (20)     3284 2024-02-01 00:32:02.000000 dbt-dremio-1.5.1/dbt_dremio.egg-info/PKG-INFO
--rw-r--r--   0 ravjotb    (503) staff       (20)     2942 2024-02-01 00:32:02.000000 dbt-dremio-1.5.1/dbt_dremio.egg-info/SOURCES.txt
--rw-r--r--   0 ravjotb    (503) staff       (20)        1 2024-02-01 00:32:02.000000 dbt-dremio-1.5.1/dbt_dremio.egg-info/dependency_links.txt
--rw-r--r--   0 ravjotb    (503) staff       (20)       38 2024-02-01 00:32:02.000000 dbt-dremio-1.5.1/dbt_dremio.egg-info/requires.txt
--rw-r--r--   0 ravjotb    (503) staff       (20)        4 2024-02-01 00:32:02.000000 dbt-dremio-1.5.1/dbt_dremio.egg-info/top_level.txt
--rw-r--r--   0 ravjotb    (503) staff       (20)       87 2022-10-17 23:38:32.000000 dbt-dremio-1.5.1/pyproject.toml
--rw-r--r--   0 ravjotb    (503) staff       (20)       74 2024-02-01 00:32:02.615341 dbt-dremio-1.5.1/setup.cfg
--rw-r--r--   0 ravjotb    (503) staff       (20)     1645 2024-01-29 22:16:32.000000 dbt-dremio-1.5.1/setup.py
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.256294 dbt-dremio-1.7.0/
+-rw-r--r--   0 ravjotb    (503) staff       (20)    11348 2022-10-17 23:38:32.000000 dbt-dremio-1.7.0/LICENSE
+-rw-r--r--   0 ravjotb    (503) staff       (20)       47 2022-10-17 23:38:32.000000 dbt-dremio-1.7.0/MANIFEST.in
+-rw-r--r--   0 ravjotb    (503) staff       (20)     3439 2024-04-29 20:16:08.256546 dbt-dremio-1.7.0/PKG-INFO
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2868 2024-04-27 00:15:59.000000 dbt-dremio-1.7.0/README.md
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.218401 dbt-dremio-1.7.0/dbt/
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.218104 dbt-dremio-1.7.0/dbt/adapters/
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.240229 dbt-dremio-1.7.0/dbt/adapters/dremio/
+-rw-r--r--   0 ravjotb    (503) staff       (20)      965 2022-11-18 18:42:01.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/__init__.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)      596 2024-04-27 00:15:59.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/__version__.py
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.241631 dbt-dremio-1.7.0/dbt/adapters/dremio/api/
+-rw-r--r--   0 ravjotb    (503) staff       (20)      737 2022-11-18 18:42:01.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/api/__init__.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2248 2023-03-14 21:48:59.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/api/authentication.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     6392 2024-04-19 00:13:00.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/api/cursor.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1552 2022-11-18 18:42:01.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/api/handle.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     3678 2023-03-14 21:48:59.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/api/parameters.py
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.242426 dbt-dremio-1.7.0/dbt/adapters/dremio/api/rest/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     7577 2024-04-19 00:13:00.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/api/rest/endpoints.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1661 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/api/rest/error.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     4914 2022-11-18 18:42:01.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/api/rest/url_builder.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     9080 2024-04-19 00:13:00.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/connections.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     4137 2024-04-19 00:12:57.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/credentials.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     6893 2024-04-27 00:15:59.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/impl.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)     3021 2024-01-29 22:16:32.000000 dbt-dremio-1.7.0/dbt/adapters/dremio/relation.py
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.218468 dbt-dremio-1.7.0/dbt/include/
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.243223 dbt-dremio-1.7.0/dbt/include/dremio/
+-rw-r--r--   0 ravjotb    (503) staff       (20)       52 2022-10-18 21:16:05.000000 dbt-dremio-1.7.0/dbt/include/dremio/__init__.py
+-rw-r--r--   0 ravjotb    (503) staff       (20)      815 2023-03-09 00:07:33.000000 dbt-dremio-1.7.0/dbt/include/dremio/dbt_project.yml
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.219429 dbt-dremio-1.7.0/dbt/include/dremio/macros/
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.245821 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2237 2023-02-28 17:07:36.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/apply_grants.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     3980 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/columns.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2540 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/data_preparation.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1985 2023-02-28 17:07:36.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/external_query.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     5678 2024-04-19 00:12:57.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/format.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)    13109 2024-04-27 00:15:59.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/metadata.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1518 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/relation.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1080 2024-04-19 00:12:57.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/snapshot.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1932 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/sources.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)      648 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/timestamp.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)      187 2024-04-19 00:12:57.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/validate_sql.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.246061 dbt-dremio-1.7.0/dbt/include/dremio/macros/builtins/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2382 2024-01-29 22:16:32.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/builtins/builtins.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.247125 dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1079 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1223 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1185 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/get_custom_schema.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)      803 2024-04-19 00:12:57.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/is_datalake_node.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.248403 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/
+-rw-r--r--   0 ravjotb    (503) staff       (20)      644 2024-04-19 00:12:57.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/can_clone_table.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2621 2024-04-19 00:12:57.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/clone.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1604 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/helpers.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.249307 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/incremental/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     5197 2024-01-29 22:16:32.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1613 2024-04-29 17:47:18.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1502 2023-02-28 17:07:36.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/incremental/validate.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.250427 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/reflection/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     4326 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/reflection/create_reflection.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1449 2024-04-19 00:13:00.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/reflection/helpers.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     4394 2024-04-19 00:13:00.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/reflection/reflection.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.251088 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/seed/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1823 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/seed/helpers.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2401 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.252142 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/table/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1956 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/table/alter_pds.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1986 2023-08-11 18:54:16.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/table/create_table_as.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1999 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/table/table.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2425 2024-04-10 19:31:03.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/twin_strategy.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.253138 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1445 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/create_or_replace_view.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)      974 2023-08-11 18:54:16.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/create_view_as.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1393 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/helpers.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1997 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/view.sql
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.254717 dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/
+-rw-r--r--   0 ravjotb    (503) staff       (20)      732 2023-02-28 17:07:36.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/array_append.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)      730 2023-02-28 17:07:36.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/array_concat.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)      848 2023-02-28 17:07:36.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/array_construct.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)      104 2023-02-01 21:41:10.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/data_types.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     3889 2024-04-27 00:15:59.000000 dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/date_spine.sql
+-rw-r--r--   0 ravjotb    (503) staff       (20)     2097 2023-03-10 23:06:14.000000 dbt-dremio-1.7.0/dbt/include/dremio/profile_template.yml
+drwxr-xr-x   0 ravjotb    (503) staff       (20)        0 2024-04-29 20:16:08.256110 dbt-dremio-1.7.0/dbt_dremio.egg-info/
+-rw-r--r--   0 ravjotb    (503) staff       (20)     3439 2024-04-29 20:16:08.000000 dbt-dremio-1.7.0/dbt_dremio.egg-info/PKG-INFO
+-rw-r--r--   0 ravjotb    (503) staff       (20)     3157 2024-04-29 20:16:08.000000 dbt-dremio-1.7.0/dbt_dremio.egg-info/SOURCES.txt
+-rw-r--r--   0 ravjotb    (503) staff       (20)        1 2024-04-29 20:16:08.000000 dbt-dremio-1.7.0/dbt_dremio.egg-info/dependency_links.txt
+-rw-r--r--   0 ravjotb    (503) staff       (20)       40 2024-04-29 20:16:08.000000 dbt-dremio-1.7.0/dbt_dremio.egg-info/requires.txt
+-rw-r--r--   0 ravjotb    (503) staff       (20)        4 2024-04-29 20:16:08.000000 dbt-dremio-1.7.0/dbt_dremio.egg-info/top_level.txt
+-rw-r--r--   0 ravjotb    (503) staff       (20)       87 2022-10-17 23:38:32.000000 dbt-dremio-1.7.0/pyproject.toml
+-rw-r--r--   0 ravjotb    (503) staff       (20)       74 2024-04-29 20:16:08.256959 dbt-dremio-1.7.0/setup.cfg
+-rw-r--r--   0 ravjotb    (503) staff       (20)     1678 2024-04-29 20:15:24.000000 dbt-dremio-1.7.0/setup.py
```

### Comparing `dbt-dremio-1.5.1/LICENSE` & `dbt-dremio-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/PKG-INFO` & `dbt-dremio-1.7.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: dbt-dremio
-Version: 1.5.1
+Version: 1.7.0
 Summary: The Dremio adapter plugin for dbt
 Home-page: https://github.com/dremio/dbt-dremio
 Author: Dremio
 License: Apache Software License 2.0 (http://www.apache.org/licenses/LICENSE-2.0)
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
 
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 
 dbt is the T in ELT. Organize, cleanse, denormalize, filter, rename, and pre-aggregate the raw data in your warehouse so that it's ready for analysis.
 
-## dbt-dremio version 1.5.1
+## Documentation
+
+[Dremio docs for our dbt adapter ](https://github.com/dremio/dbt-dremio/wiki/Using-Materializations-with-Dremio)
+
+## dbt-dremio version 1.7.0
 
 The `dbt-dremio` package contains all of the code enabling dbt to work with [Dremio](https://www.dremio.com/). For more information on using dbt with Dremio, consult [the docs](https://docs.getdbt.com/reference/warehouse-profiles/dremio-profile).
 
 The dbt-dremio package supports both Dremio Cloud and Dremio Software (versions 22.0 and later).
 
-Version 1.5.1 of the dbt-dremio adapter is compatible with dbt-core versions 1.2.0 to 1.5.*.
+Version 1.7.0 of the dbt-dremio adapter is compatible with dbt-core versions 1.2.0 to 1.7.*.
 
 > Prior to version 1.1.0b, dbt-dremio was created and maintained by [Fabrice Etanchaud](https://github.com/fabrice-etanchaud) on [their GitHub repo](https://github.com/fabrice-etanchaud/dbt-dremio). Code for using Dremio REST APIs was originally authored by [Ryan Murray](https://github.com/rymurr). Contributors in this repo are credited for laying the groundwork and maintaining the adapter till version 1.0.6.5. The dbt-dremio adapter is maintained and distributed by Dremio starting with version 1.1.0b.
 
 ## Getting started
 
 -   [Install dbt-dremio](https://docs.getdbt.com/reference/warehouse-setups/dremio-setup)
-    -   Version 1.5.1 of dbt-dremio requires dbt-core >= 1.2.0 and <= 1.5.*. Installing dbt-dremio will automatically upgrade existing dbt-core versions earlier than 1.2.0 to 1.5.*, or install dbt-core v1.5.0 if no version of dbt-core is found.
+    -   Version 1.7.0 of dbt-dremio requires dbt-core >= 1.2.0 and <= 1.7.*. Installing dbt-dremio will automatically upgrade existing dbt-core versions earlier than 1.2.0 to 1.7.*, or install dbt-core v1.7.0 if no version of dbt-core is found.
 -   Read the [introduction](https://docs.getdbt.com/docs/introduction/) and [viewpoint](https://docs.getdbt.com/docs/about/viewpoint/)
 
 ## Join the dbt Community
 
 -   Be part of the conversation in the [dbt Community Slack](http://community.getdbt.com/)
 -   Read more on the [dbt Community Discourse](https://discourse.getdbt.com)
```

### Comparing `dbt-dremio-1.5.1/README.md` & `dbt-dremio-1.7.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 
 dbt is the T in ELT. Organize, cleanse, denormalize, filter, rename, and pre-aggregate the raw data in your warehouse so that it's ready for analysis.
 
-## dbt-dremio version 1.5.1
+## Documentation
+
+[Dremio docs for our dbt adapter ](https://github.com/dremio/dbt-dremio/wiki/Using-Materializations-with-Dremio)
+
+## dbt-dremio version 1.7.0
 
 The `dbt-dremio` package contains all of the code enabling dbt to work with [Dremio](https://www.dremio.com/). For more information on using dbt with Dremio, consult [the docs](https://docs.getdbt.com/reference/warehouse-profiles/dremio-profile).
 
 The dbt-dremio package supports both Dremio Cloud and Dremio Software (versions 22.0 and later).
 
-Version 1.5.1 of the dbt-dremio adapter is compatible with dbt-core versions 1.2.0 to 1.5.*.
+Version 1.7.0 of the dbt-dremio adapter is compatible with dbt-core versions 1.2.0 to 1.7.*.
 
 > Prior to version 1.1.0b, dbt-dremio was created and maintained by [Fabrice Etanchaud](https://github.com/fabrice-etanchaud) on [their GitHub repo](https://github.com/fabrice-etanchaud/dbt-dremio). Code for using Dremio REST APIs was originally authored by [Ryan Murray](https://github.com/rymurr). Contributors in this repo are credited for laying the groundwork and maintaining the adapter till version 1.0.6.5. The dbt-dremio adapter is maintained and distributed by Dremio starting with version 1.1.0b.
 
 ## Getting started
 
 -   [Install dbt-dremio](https://docs.getdbt.com/reference/warehouse-setups/dremio-setup)
-    -   Version 1.5.1 of dbt-dremio requires dbt-core >= 1.2.0 and <= 1.5.*. Installing dbt-dremio will automatically upgrade existing dbt-core versions earlier than 1.2.0 to 1.5.*, or install dbt-core v1.5.0 if no version of dbt-core is found.
+    -   Version 1.7.0 of dbt-dremio requires dbt-core >= 1.2.0 and <= 1.7.*. Installing dbt-dremio will automatically upgrade existing dbt-core versions earlier than 1.2.0 to 1.7.*, or install dbt-core v1.7.0 if no version of dbt-core is found.
 -   Read the [introduction](https://docs.getdbt.com/docs/introduction/) and [viewpoint](https://docs.getdbt.com/docs/about/viewpoint/)
 
 ## Join the dbt Community
 
 -   Be part of the conversation in the [dbt Community Slack](http://community.getdbt.com/)
 -   Read more on the [dbt Community Discourse](https://discourse.getdbt.com)
```

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/__init__.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/__version__.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,8 +5,9 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = "1.5.1"
+version = "1.7.0"
+
```

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/api/__init__.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/api/authentication.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/api/authentication.py`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/api/cursor.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/api/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
+import time
+
 import agate
 
 from dbt.adapters.dremio.api.rest.endpoints import (
     sql_endpoint,
     job_status,
     job_results,
     job_cancel_api,
@@ -119,14 +121,16 @@
         job_id = self._job_id
 
         last_job_state = ""
         job_status_response = job_status(self._parameters, job_id)
         job_status_state = job_status_response["jobState"]
 
         while True:
+            time.sleep(0.2)
+            
             if job_status_state != last_job_state:
                 logger.debug(f"Job State = {job_status_state}")
 
             if job_status_state == "FAILED":
                 error_message = job_status_response["errorMessage"]
                 raise Exception(f"ERROR: {error_message}")
```

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/api/handle.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/api/handle.py`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/api/parameters.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/api/parameters.py`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/api/rest/endpoints.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/api/rest/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,42 +35,43 @@
 from dbt.adapters.dremio.api.parameters import Parameters
 from dbt.adapters.dremio.api.rest.url_builder import UrlBuilder
 
 from dbt.events import AdapterLogger
 
 logger = AdapterLogger("dremio")
 
+session = requests.Session()
 
 def _get(url, request_headers, details="", ssl_verify=True):
-    response = requests.get(url, headers=request_headers, verify=ssl_verify)
+    response = session.get(url, headers=request_headers, verify=ssl_verify)
     return _check_error(response, details)
 
 
 def _post(
     url,
     request_headers=None,
     json=None,
     details="",
     ssl_verify=True,
     timeout=None,
 ):
     if isinstance(json, str):
         json = jsonlib.loads(json)
-    response = requests.post(
+    response = session.post(
         url,
         headers=request_headers,
         timeout=timeout,
         verify=ssl_verify,
         json=json,
     )
     return _check_error(response, details)
 
 
 def _delete(url, request_headers, details="", ssl_verify=True):
-    response = requests.delete(url, headers=request_headers, verify=ssl_verify)
+    response = session.delete(url, headers=request_headers, verify=ssl_verify)
     return _check_error(response, details)
 
 
 def _raise_for_status(self):
     """Raises stored :class:`HTTPError`, if one occurred. Copy from requests request.raise_for_status()"""
 
     http_error_msg = ""
```

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/api/rest/error.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/api/rest/error.py`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/api/rest/url_builder.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/api/rest/url_builder.py`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/connections.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import agate
-from typing import Tuple
+from typing import Tuple, Optional
 from contextlib import contextmanager
 
 from dbt.adapters.dremio.api.cursor import DremioCursor
 from dbt.adapters.dremio.api.handle import DremioHandle
 from dbt.adapters.dremio.api.parameters import ParametersBuilder
 
 import time
@@ -36,24 +36,25 @@
     DremioAlreadyExistsException,
     DremioNotFoundException,
     DremioRequestTimeoutException,
     DremioTooManyRequestsException,
     DremioInternalServerException,
     DremioServiceUnavailableException,
     DremioGatewayTimeoutException,
+    DremioBadRequestException,
 )
 
 from dbt.events import AdapterLogger
 
 logger = AdapterLogger("dremio")
 
 
 class DremioConnectionManager(SQLConnectionManager):
     TYPE = "dremio"
-    DEFAULT_CONNECTION_RETRIES = 1
+    DEFAULT_CONNECTION_RETRIES = 5
 
     retries = DEFAULT_CONNECTION_RETRIES
 
     @contextmanager
     def exception_handler(self, sql):
         try:
             yield
@@ -167,15 +168,19 @@
     @classmethod
     def get_response(cls, cursor: DremioCursor) -> AdapterResponse:
         rows = cursor.rowcount
         message = "OK" if rows == -1 else str(rows)
         return AdapterResponse(_message=message, rows_affected=rows)
 
     def execute(
-        self, sql: str, auto_begin: bool = False, fetch: bool = False
+        self,
+        sql: str,
+        auto_begin: bool = False,
+        fetch: bool = False,
+        limit: Optional[int] = None,
     ) -> Tuple[AdapterResponse, agate.Table]:
         sql = self._add_query_comment(sql)
         _, cursor = self.add_query(sql, auto_begin, fetch=fetch)
         response = self.get_response(cursor)
         if fetch:
             table = cursor.table
         else:
@@ -201,25 +206,30 @@
                 )
             except DremioNotFoundException:
                 logger.debug("Catalog not found. Returning")
                 return
 
             delete_catalog(api_parameters, catalog_info["id"])
 
-    def create_catalog(self, database, schema):
+    def create_catalog(self, relation):
         thread_connection = self.get_thread_connection()
         connection = self.open(thread_connection)
         credentials = connection.credentials
         api_parameters = connection.handle.get_parameters()
+        database = relation.database
+        schema = relation.schema
 
         if database == ("@" + credentials.UID):
             logger.debug("Database is default: creating folders only")
         else:
+            logger.debug(f"Creating space: {database}")
             self._create_space(database, api_parameters)
+
         if database != credentials.datalake:
+            logger.debug(f"Creating folder(s): {database}.{schema}")
             self._create_folders(database, schema, api_parameters)
         return
 
     def _make_new_space_json(self, name) -> json:
         python_dict = {"entityType": "space", "name": name}
         return json.dumps(python_dict)
 
@@ -239,13 +249,18 @@
         for folder in schema.split("."):
             temp_path_list.append(folder)
             folder_json = self._make_new_folder_json(temp_path_list)
             try:
                 create_catalog_api(api_parameters, folder_json)
             except DremioAlreadyExistsException:
                 logger.debug(f"Folder {folder} already exists.")
+            except DremioBadRequestException as e:
+               if "Can not create a folder inside a [SOURCE]" in e.message:
+                   logger.debug(f"Ignoring {e}")
+               else:
+                   raise e
 
     def _create_path_list(self, database, schema):
         path = [database]
         folders = schema.split(".")
         path.extend(folders)
         return path
```

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/credentials.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     cloud_host: Optional[str] = None
     software_host: Optional[str] = None
     port: Optional[int] = 9047  # for rest endpoint
     use_ssl: Optional[bool] = True
     verify_ssl: Optional[bool] = True
 
     _ALIASES = {
-        # Only terms on right-side will be used going forward.
+        # Only terms on left-side will be used going forward.
         "username": "UID",  # backwards compatibility with existing profiles
         "user": "UID",
         "password": "PWD",
         "object_storage_source": "datalake",
         "object_storage_path": "root_path",
         "dremio_space": "database",
         "dremio_space_folder": "schema",
```

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/impl.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/impl.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,24 +17,42 @@
 from dbt.adapters.dremio import DremioConnectionManager
 from dbt.adapters.dremio.relation import DremioRelation
 from typing import Dict
 
 from typing import List
 from typing import Optional
 from dbt.adapters.base.relation import BaseRelation
+
+from dbt.adapters.capability import (
+    CapabilityDict,
+    CapabilitySupport,
+    Support,
+    Capability,
+)
 from dbt.adapters.sql.impl import DROP_RELATION_MACRO_NAME
 from dbt.events import AdapterLogger
 
 logger = AdapterLogger("dremio")
 
 
 class DremioAdapter(SQLAdapter):
     ConnectionManager = DremioConnectionManager
     Relation = DremioRelation
 
+    _capabilities = CapabilityDict(
+        {
+            Capability.TableLastModifiedMetadata: CapabilitySupport(
+                support=Support.Full
+            ),
+            Capability.SchemaMetadataByRelations: CapabilitySupport(
+                support=Support.Full
+            ),
+        }
+    )
+
     @classmethod
     def date_function(cls):
         return "current_date"
 
     @classmethod
     def convert_text_type(cls, agate_table, col_idx):
         return "varchar"
@@ -57,17 +75,15 @@
         return "decimal" if decimals else "bigint"
 
     @classmethod
     def convert_time_type(cls, agate_table, col_idx):
         return "time"
 
     def create_schema(self, relation: DremioRelation) -> None:
-        database = relation.database
-        schema = relation.schema
-        self.connections.create_catalog(database, schema)
+        self.connections.create_catalog(relation)
 
     def drop_schema(self, relation: DremioRelation) -> None:
         if relation.type == "table":
             self.execute_macro(DROP_RELATION_MACRO_NAME, kwargs={"relation": relation})
 
         else:
             database = relation.database
```

### Comparing `dbt-dremio-1.5.1/dbt/adapters/dremio/relation.py` & `dbt-dremio-1.7.0/dbt/adapters/dremio/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/dbt_project.yml` & `dbt-dremio-1.7.0/dbt/include/dremio/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/apply_grants.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/columns.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/data_preparation.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/data_preparation.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/external_query.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/external_query.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/format.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/format.sql`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     ,'line_delimiter':'lineDelimiter'
     ,'skip_first_line':'skipFirstLine'
     ,'extract_header':'extractHeader'
     ,'trim_header':'trimHeader'
     ,'auto_generated_column_names':'autoGenerateColumnNames'
     ,'pretty_print':'prettyPrint'} -%}
   {%- set options = [] -%}
-  {%- set format = config.get('format', validator=validation.any[basestring]) or 'iceberg' -%}
+  {%- set format = config.get('format', validator=validation.any[basestring])-%}
   {%- if format in ['text', 'json', 'arrow', 'parquet', 'iceberg'] -%}
     {%- do options.append("type=>'" ~ format ~ "'") -%}
     {%- if format == 'text' -%}
       {%- for key in ['field_delimiter', 'line_delimiter', 'quote', 'comment', 'escape'] -%}
         {%- set value = config.get(key, validator=validation.any[basestring]) -%}
         {%- set key = key_map[key] or key -%}
         {%- if value is not none -%}
```

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/relation.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/snapshot.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/snapshot.sql`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.*/
 
+
 {% macro dremio__snapshot_merge_sql(target, source, insert_cols) -%}
     {%- set insert_cols_csv = insert_cols | join(', ') -%}
 
     merge into {{ target }} as DBT_INTERNAL_DEST
     using {{ source }} as DBT_INTERNAL_SOURCE
     on DBT_INTERNAL_SOURCE.dbt_scd_id = DBT_INTERNAL_DEST.dbt_scd_id
 
@@ -23,8 +24,8 @@
         then update
         set dbt_valid_to = DBT_INTERNAL_SOURCE.dbt_valid_to
 
     when not matched
         then insert ({{ insert_cols_csv }})
         values ({{ insert_cols_csv }})
 
-{% endmacro %}
+{% endmacro %}
```

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/sources.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/sources.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/adapters/timestamp.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/adapters/timestamp.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/builtins/builtins.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/builtins/builtins.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/get_custom_alias.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/get_custom_database.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/get_custom_schema.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/get_custom_name/is_datalake_node.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/get_custom_name/is_datalake_node.sql`

 * *Files 17% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.*/
 
 {% macro is_datalake_node(node) -%}
-  {{ return(node.resource_type in ['test', 'seed']
+  {{ return(node.resource_type in ['test', 'seed', 'snapshot']
     or (node.resource_type == 'model' and node.config.materialized not in ['view', 'reflection'])) }}
 {%- endmacro %}
```

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/helpers.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/incremental/incremental.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/incremental/strategies.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/incremental/validate.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/reflection/create_reflection.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/reflection/create_reflection.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/reflection/helpers.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/reflection/helpers.sql`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.*/
 
 {% macro drop_reflection_if_exists(relation, reflection) %}
-  {% if reflection is not none and reflection.type == 'materializedview' %}
+  {% if reflection is not none and reflection.type == 'materialized_view' %}
     {% call statement('drop reflection') -%}
       alter dataset {{ relation }}
         drop reflection {{ reflection.include(database=False, schema=False) }}
     {%- endcall %}
   {% endif %}
 {% endmacro %}
```

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/reflection/reflection.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/reflection/reflection.sql`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         {% set external_target = source(raw_external_target[0], raw_external_target[1]) %}
       {% endif %}
     {% endif %}
   {% endif %}
 
   {%- set old_relation = adapter.get_relation(database=anchor.database, schema=anchor.schema, identifier=identifier) -%}
   {%- set target_relation = api.Relation.create(
-      identifier=identifier, schema=anchor.schema, database=anchor.database, type='materializedview') -%}
+      identifier=identifier, schema=anchor.schema, database=anchor.database, type='materialized_view') -%}
 
   {%- set reflection_type = dbt_dremio_validate_get_reflection_type(raw_reflection_type) -%}
   {% if (reflection_type == 'raw' and display is none)
     or (reflection_type == 'aggregate' and (dimensions is none or measures is none)) %}
     {% set columns = adapter.get_columns_in_relation(anchor) %}
     {% if reflection_type == 'raw' %}
       {% set display = columns | map(attribute='name') | list %}
```

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/seed/helpers.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/seed/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/seed/seed.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/table/alter_pds.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/table/alter_pds.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/table/create_table_as.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/table/table.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/twin_strategy.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/twin_strategy.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/create_or_replace_view.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/create_view_as.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/helpers.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/materializations/view/view.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/utils/array_append.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/array_append.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/utils/array_concat.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/array_concat.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/macros/utils/array_construct.sql` & `dbt-dremio-1.7.0/dbt/include/dremio/macros/utils/array_construct.sql`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt/include/dremio/profile_template.yml` & `dbt-dremio-1.7.0/dbt/include/dremio/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-dremio-1.5.1/dbt_dremio.egg-info/PKG-INFO` & `dbt-dremio-1.7.0/dbt_dremio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: dbt-dremio
-Version: 1.5.1
+Version: 1.7.0
 Summary: The Dremio adapter plugin for dbt
 Home-page: https://github.com/dremio/dbt-dremio
 Author: Dremio
 License: Apache Software License 2.0 (http://www.apache.org/licenses/LICENSE-2.0)
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
 
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to transform their data using the same practices that software engineers use to build applications.
 
 dbt is the T in ELT. Organize, cleanse, denormalize, filter, rename, and pre-aggregate the raw data in your warehouse so that it's ready for analysis.
 
-## dbt-dremio version 1.5.1
+## Documentation
+
+[Dremio docs for our dbt adapter ](https://github.com/dremio/dbt-dremio/wiki/Using-Materializations-with-Dremio)
+
+## dbt-dremio version 1.7.0
 
 The `dbt-dremio` package contains all of the code enabling dbt to work with [Dremio](https://www.dremio.com/). For more information on using dbt with Dremio, consult [the docs](https://docs.getdbt.com/reference/warehouse-profiles/dremio-profile).
 
 The dbt-dremio package supports both Dremio Cloud and Dremio Software (versions 22.0 and later).
 
-Version 1.5.1 of the dbt-dremio adapter is compatible with dbt-core versions 1.2.0 to 1.5.*.
+Version 1.7.0 of the dbt-dremio adapter is compatible with dbt-core versions 1.2.0 to 1.7.*.
 
 > Prior to version 1.1.0b, dbt-dremio was created and maintained by [Fabrice Etanchaud](https://github.com/fabrice-etanchaud) on [their GitHub repo](https://github.com/fabrice-etanchaud/dbt-dremio). Code for using Dremio REST APIs was originally authored by [Ryan Murray](https://github.com/rymurr). Contributors in this repo are credited for laying the groundwork and maintaining the adapter till version 1.0.6.5. The dbt-dremio adapter is maintained and distributed by Dremio starting with version 1.1.0b.
 
 ## Getting started
 
 -   [Install dbt-dremio](https://docs.getdbt.com/reference/warehouse-setups/dremio-setup)
-    -   Version 1.5.1 of dbt-dremio requires dbt-core >= 1.2.0 and <= 1.5.*. Installing dbt-dremio will automatically upgrade existing dbt-core versions earlier than 1.2.0 to 1.5.*, or install dbt-core v1.5.0 if no version of dbt-core is found.
+    -   Version 1.7.0 of dbt-dremio requires dbt-core >= 1.2.0 and <= 1.7.*. Installing dbt-dremio will automatically upgrade existing dbt-core versions earlier than 1.2.0 to 1.7.*, or install dbt-core v1.7.0 if no version of dbt-core is found.
 -   Read the [introduction](https://docs.getdbt.com/docs/introduction/) and [viewpoint](https://docs.getdbt.com/docs/about/viewpoint/)
 
 ## Join the dbt Community
 
 -   Be part of the conversation in the [dbt Community Slack](http://community.getdbt.com/)
 -   Read more on the [dbt Community Discourse](https://discourse.getdbt.com)
```

### Comparing `dbt-dremio-1.5.1/dbt_dremio.egg-info/SOURCES.txt` & `dbt-dremio-1.7.0/dbt_dremio.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,22 @@
 dbt/include/dremio/macros/adapters/external_query.sql
 dbt/include/dremio/macros/adapters/format.sql
 dbt/include/dremio/macros/adapters/metadata.sql
 dbt/include/dremio/macros/adapters/relation.sql
 dbt/include/dremio/macros/adapters/snapshot.sql
 dbt/include/dremio/macros/adapters/sources.sql
 dbt/include/dremio/macros/adapters/timestamp.sql
+dbt/include/dremio/macros/adapters/validate_sql.sql
 dbt/include/dremio/macros/builtins/builtins.sql
 dbt/include/dremio/macros/get_custom_name/get_custom_alias.sql
 dbt/include/dremio/macros/get_custom_name/get_custom_database.sql
 dbt/include/dremio/macros/get_custom_name/get_custom_schema.sql
 dbt/include/dremio/macros/get_custom_name/is_datalake_node.sql
+dbt/include/dremio/macros/materializations/can_clone_table.sql
+dbt/include/dremio/macros/materializations/clone.sql
 dbt/include/dremio/macros/materializations/helpers.sql
 dbt/include/dremio/macros/materializations/twin_strategy.sql
 dbt/include/dremio/macros/materializations/incremental/incremental.sql
 dbt/include/dremio/macros/materializations/incremental/strategies.sql
 dbt/include/dremio/macros/materializations/incremental/validate.sql
 dbt/include/dremio/macros/materializations/reflection/create_reflection.sql
 dbt/include/dremio/macros/materializations/reflection/helpers.sql
@@ -53,12 +56,13 @@
 dbt/include/dremio/macros/materializations/view/create_view_as.sql
 dbt/include/dremio/macros/materializations/view/helpers.sql
 dbt/include/dremio/macros/materializations/view/view.sql
 dbt/include/dremio/macros/utils/array_append.sql
 dbt/include/dremio/macros/utils/array_concat.sql
 dbt/include/dremio/macros/utils/array_construct.sql
 dbt/include/dremio/macros/utils/data_types.sql
+dbt/include/dremio/macros/utils/date_spine.sql
 dbt_dremio.egg-info/PKG-INFO
 dbt_dremio.egg-info/SOURCES.txt
 dbt_dremio.egg-info/dependency_links.txt
 dbt_dremio.egg-info/requires.txt
 dbt_dremio.egg-info/top_level.txt
```

### Comparing `dbt-dremio-1.5.1/setup.py` & `dbt-dremio-1.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,32 +17,35 @@
 # pull the long description from the README
 README = Path(__file__).parent / "README.md"
 
 
 README
 
 package_name = "dbt-dremio"
-package_version = "1.5.1"
+
+package_version = "1.7.0"
+
 description = """The Dremio adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=README.read_text(),
     license="Apache Software License 2.0 (http://www.apache.org/licenses/LICENSE-2.0)",
     author="Dremio",
     url="https://github.com/dremio/dbt-dremio",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-core>=1.2, <1.6.0",
+        "dbt-core>=1.2, <=1.7.13",
         "requests>=2.31.0",
     ],
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3.11",
     ],
+    python_requires=">=3.8",
 )
```

