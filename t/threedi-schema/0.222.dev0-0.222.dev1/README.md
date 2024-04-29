# Comparing `tmp/threedi-schema-0.222.dev0.tar.gz` & `tmp/threedi_schema-0.222.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threedi-schema-0.222.dev0.tar", last modified: Tue Apr  9 12:50:11 2024, max compression
+gzip compressed data, was "threedi_schema-0.222.dev1.tar", last modified: Mon Apr 29 12:47:21 2024, max compression
```

## Comparing `threedi-schema-0.222.dev0.tar` & `threedi_schema-0.222.dev1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.759864 threedi-schema-0.222.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-09 12:50:11.759864 threedi-schema-0.222.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 12:50:11.759864 threedi-schema-0.222.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.747864 threedi-schema-0.222.dev0/threedi_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.751864 threedi-schema-0.222.dev0/threedi_schema/application/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/application/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/application/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/application/threedi_database.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/beta_features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.751864 threedi-schema-0.222.dev0/threedi_schema/domain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    30374 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/domain/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.751864 threedi-schema-0.222.dev0/threedi_schema/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/infrastructure/spatial_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/infrastructure/spatialite_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/infrastructure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.751864 threedi-schema-0.222.dev0/threedi_schema/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.755864 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0200_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0202_remove_unused_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0203_remove_unused_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0205_settings_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0206_control_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0208_tables_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0209_remove_surface_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0210_global_raster_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0211_breach_and_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0216_vegetation_drag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0222_upgrade_db_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/migrations/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.755864 threedi-schema-0.222.dev0/threedi_schema/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.755864 threedi-schema-0.222.dev0/threedi_schema/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_beta_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_gpkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_migration_213.py
--rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-09 12:50:06.000000 threedi-schema-0.222.dev0/threedi_schema/tests/test_spatalite_versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 12:50:11.759864 threedi-schema-0.222.dev0/threedi_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-09 12:50:11.000000 threedi-schema-0.222.dev0/threedi_schema.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.419800 threedi_schema-0.222.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-29 12:47:21.419800 threedi_schema-0.222.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:47:21.419800 threedi_schema-0.222.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.407801 threedi_schema-0.222.dev1/threedi_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.407801 threedi_schema-0.222.dev1/threedi_schema/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/application/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/application/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/application/threedi_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/beta_features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.407801 threedi_schema-0.222.dev1/threedi_schema/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30963 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/domain/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.411800 threedi_schema-0.222.dev1/threedi_schema/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/infrastructure/spatial_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/infrastructure/spatialite_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/infrastructure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.411800 threedi_schema-0.222.dev1/threedi_schema/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.415800 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)    46413 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0200_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0202_remove_unused_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0203_remove_unused_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0205_settings_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0206_control_structures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0207_fix_schema_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0208_tables_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0209_remove_surface_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0210_global_raster_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0211_breach_and_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0215_groundwater_1d2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0216_vegetation_drag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0222_upgrade_db_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/migrations/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.415800 threedi_schema-0.222.dev1/threedi_schema/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.415800 threedi_schema-0.222.dev1/threedi_schema/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:16.000000 threedi_schema-0.222.dev1/threedi_schema/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_beta_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_gpkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_migration_213.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8873 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-04-29 12:47:17.000000 threedi_schema-0.222.dev1/threedi_schema/tests/test_spatalite_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:47:21.415800 threedi_schema-0.222.dev1/threedi_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 12:47:21.000000 threedi_schema-0.222.dev1/threedi_schema.egg-info/top_level.txt
```

### Comparing `threedi-schema-0.222.dev0/CHANGES.rst` & `threedi_schema-0.222.dev1/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/LICENSE` & `threedi_schema-0.222.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/PKG-INFO` & `threedi_schema-0.222.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.222.dev0
+Version: 0.222.dev1
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `threedi-schema-0.222.dev0/README.rst` & `threedi_schema-0.222.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/pyproject.toml` & `threedi_schema-0.222.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/application/schema.py` & `threedi_schema-0.222.dev1/threedi_schema/application/schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/application/threedi_database.py` & `threedi_schema-0.222.dev1/threedi_schema/application/threedi_database.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/beta_features.py` & `threedi_schema-0.222.dev1/threedi_schema/beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/domain/constants.py` & `threedi_schema-0.222.dev1/threedi_schema/domain/constants.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/domain/custom_types.py` & `threedi_schema-0.222.dev1/threedi_schema/domain/custom_types.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/domain/indexes.py` & `threedi_schema-0.222.dev1/threedi_schema/domain/indexes.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/domain/models.py` & `threedi_schema-0.222.dev1/threedi_schema/domain/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -152,14 +152,19 @@
     infiltration_rate_file = Column(String(255))
     infiltration_surface_option = Column(
         IntegerEnum(constants.InfiltrationSurfaceOption)
     )
     max_infiltration_volume = Column(Float)
     max_infiltration_volume_file = Column(Text)
 
+    # Alias needed for API compatibility
+    @property
+    def max_infiltration_volume_file(self):
+        return self.max_infiltration_volume_file
+
 
 class SurfaceParameter(Base):
     __tablename__ = "v2_surface_parameters"
     id = Column(Integer, primary_key=True)
     outflow_delay = Column(Float, nullable=False)
     surface_layer_thickness = Column(Float, nullable=False)
     infiltration = Column(Boolean, nullable=False)
@@ -229,14 +234,19 @@
     groundwater_hydraulic_conductivity_file = Column(String(255))
     groundwater_hydraulic_conductivity_aggregation = Column(
         IntegerEnum(constants.InitializationType)
     )
     leakage = Column(Float)
     leakage_file = Column(String(255))
 
+    # Alias needed for API compatibility
+    @property
+    def groundwater_hydro_connectivity_file(self):
+        return self.groundwater_hydraulic_conductivity_file
+
 
 class GridRefinement(Base):
     __tablename__ = "v2_grid_refinement"
     id = Column(Integer, primary_key=True)
 
     display_name = Column(String(255))
     refinement_level = Column(Integer, nullable=False)
@@ -398,27 +408,37 @@
     use_interception = Column(Boolean)
     use_structure_control = Column(Boolean)
     use_simple_infiltration = Column(Boolean)
     use_groundwater_flow = Column(Boolean)
     use_groundwater_storage = Column(Boolean)
     use_vegetation_drag_2d = Column(Boolean)
 
+    # Alias needed for API compatibility
+    @property
+    def frict_coef_file(self):
+        return self.friction_coefficient_file
+
 
 class InitialConditions(Base):
     __tablename__ = "initial_conditions"
     id = Column(Integer, primary_key=True)
     initial_groundwater_level = Column(Float)
     initial_groundwater_level_file = Column(String(255))
     initial_groundwater_level_aggregation = Column(
         IntegerEnum(constants.InitializationType)
     )
     initial_water_level = Column(Float)
     initial_water_level_aggregation = Column(IntegerEnum(constants.InitializationType))
     initial_water_level_file = Column(String(255))
 
+    # Alias needed for API compatibility
+    @property
+    def initial_waterlevel_file(self):
+        return self.initial_water_level_file
+
 
 class Interception(Base):
     __tablename__ = "interception"
     id = Column(Integer, primary_key=True)
     interception = Column(Float)
     interception_file = Column(String(255))
```

### Comparing `threedi-schema-0.222.dev0/threedi_schema/domain/views.py` & `threedi_schema-0.222.dev1/threedi_schema/domain/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/infrastructure/spatial_index.py` & `threedi_schema-0.222.dev1/threedi_schema/infrastructure/spatial_index.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/infrastructure/spatialite_versions.py` & `threedi_schema-0.222.dev1/threedi_schema/infrastructure/spatialite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/infrastructure/views.py` & `threedi_schema-0.222.dev1/threedi_schema/infrastructure/views.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/env.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/env.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0200_initial.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0200_initial.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0201_migrate_friction_type_4.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0202_remove_unused_tables.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0202_remove_unused_tables.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0203_remove_unused_cols.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0203_remove_unused_cols.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0204_reset_nullable_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0205_settings_defaults.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0205_settings_defaults.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0206_control_structures.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0206_control_structures.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0207_fix_schema_constraints.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0207_fix_schema_constraints.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0208_tables_settings.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0208_tables_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0209_remove_surface_type.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0209_remove_surface_type.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0210_global_raster_values.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0210_global_raster_values.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0211_breach_and_exchange.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0211_breach_and_exchange.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0212_breach_and_exchange_properties.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0213_connected_points_to_breaches.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0214_drop_cpoints_levees.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0215_groundwater_1d2d.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0215_groundwater_1d2d.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0216_vegetation_drag.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0216_vegetation_drag.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0217_rename_vegetation_columns.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0218_1d_vegetation_and_variable_friction.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0219_nullable_cross_section_location_friction_value.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0220_geopackage_compatiblility.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0221_remove_vegetation_drag_coeficients_col.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/migrations/versions/0222_upgrade_db_settings.py` & `threedi_schema-0.222.dev1/threedi_schema/migrations/versions/0222_upgrade_db_settings.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/scripts.py` & `threedi_schema-0.222.dev1/threedi_schema/scripts.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/tests/conftest.py` & `threedi_schema-0.222.dev1/threedi_schema/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/tests/test_beta_features.py` & `threedi_schema-0.222.dev1/threedi_schema/tests/test_beta_features.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/tests/test_gpkg.py` & `threedi_schema-0.222.dev1/threedi_schema/tests/test_gpkg.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/tests/test_migration.py` & `threedi_schema-0.222.dev1/threedi_schema/tests/test_migration.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/tests/test_migration_213.py` & `threedi_schema-0.222.dev1/threedi_schema/tests/test_migration_213.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/tests/test_schema.py` & `threedi_schema-0.222.dev1/threedi_schema/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema/tests/test_spatalite_versions.py` & `threedi_schema-0.222.dev1/threedi_schema/tests/test_spatalite_versions.py`

 * *Files identical despite different names*

### Comparing `threedi-schema-0.222.dev0/threedi_schema.egg-info/PKG-INFO` & `threedi_schema-0.222.dev1/threedi_schema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threedi-schema
-Version: 0.222.dev0
+Version: 0.222.dev1
 Summary: The schema of 3Di schematization files
 Author-email: Nelen & Schuurmans <info@nelen-schuurmans.nl>
 License: MIT
 Project-URL: Repository, https://github.com/nens/threedi-schema
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
```

### Comparing `threedi-schema-0.222.dev0/threedi_schema.egg-info/SOURCES.txt` & `threedi_schema-0.222.dev1/threedi_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

