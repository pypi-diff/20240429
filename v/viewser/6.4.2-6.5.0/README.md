# Comparing `tmp/viewser-6.4.2.tar.gz` & `tmp/viewser-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewser-6.4.2.tar", max compression
+gzip compressed data, was "viewser-6.5.0.tar", max compression
```

## Comparing `viewser-6.4.2.tar` & `viewser-6.5.0.tar`

### file list

```diff
@@ -1,75 +1,78 @@
--rw-r--r--   0        0        0    19916 2024-04-23 09:00:35.451016 viewser-6.4.2/LICENSE
--rw-r--r--   0        0        0    16854 2024-04-23 09:00:35.451016 viewser-6.4.2/README.md
--rw-r--r--   0        0        0      878 2024-04-23 09:00:35.451016 viewser-6.4.2/pyproject.toml
--rw-r--r--   0        0        0       79 2024-04-23 09:00:35.451016 viewser-6.4.2/viewser/__init__.py
--rw-r--r--   0        0        0     1779 2024-04-23 09:00:35.451016 viewser-6.4.2/viewser/cli.py
--rw-r--r--   0        0        0        0 2024-04-23 09:00:35.451016 viewser-6.4.2/viewser/commands/__init__.py
--rw-r--r--   0        0        0       22 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/config/__init__.py
--rw-r--r--   0        0        0     3184 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/config/cli.py
--rw-r--r--   0        0        0       61 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/documentation/__init__.py
--rw-r--r--   0        0        0     3733 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/documentation/cli.py
--rw-r--r--   0        0        0     3484 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/documentation/formatting.py
--rw-r--r--   0        0        0     2070 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/documentation/operations.py
--rw-r--r--   0        0        0      909 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/documentation/wrapped_views_doc.py
--rw-r--r--   0        0        0       21 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/help/__init__.py
--rw-r--r--   0        0        0      790 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/help/cli.py
--rw-r--r--   0        0        0      242 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/help/operations.py
--rw-r--r--   0        0        0       22 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/logs/__init__.py
--rw-r--r--   0        0        0      393 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/logs/cli.py
--rw-r--r--   0        0        0       22 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/model/__init__.py
--rw-r--r--   0        0        0     3531 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/model/cli.py
--rw-r--r--   0        0        0      731 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/model/formatting.py
--rw-r--r--   0        0        0        1 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/model/models.py
--rw-r--r--   0        0        0       22 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/notebooks/__init__.py
--rw-r--r--   0        0        0     1766 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/notebooks/cli.py
--rw-r--r--   0        0        0     6167 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/notebooks/operations.py
--rw-r--r--   0        0        0       60 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/__init__.py
--rw-r--r--   0        0        0     2245 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/cli.py
--rw-r--r--   0        0        0     1269 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/formatting.py
--rw-r--r--   0        0        0      133 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/models/__init__.py
--rw-r--r--   0        0        0     3059 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/models/column.py
--rw-r--r--   0        0        0     6085 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/models/queryset.py
--rw-r--r--   0        0        0     2285 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/models/transform.py
--rw-r--r--   0        0        0      313 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/models/util.py
--rw-r--r--   0        0        0     8241 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/operations.py
--rw-r--r--   0        0        0      231 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/queryset/queryset_list.py
--rw-r--r--   0        0        0       22 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/system/__init__.py
--rw-r--r--   0        0        0     1816 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/system/cli.py
--rw-r--r--   0        0        0     1371 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/system/formatting.py
--rw-r--r--   0        0        0      481 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/commands/system/models.py
--rw-r--r--   0        0        0       73 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/error_handling/__init__.py
--rw-r--r--   0        0        0     3929 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/error_handling/checks.py
--rw-r--r--   0        0        0     2164 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/error_handling/error_handling.py
--rw-r--r--   0        0        0     7304 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/error_handling/errors.py
--rw-r--r--   0        0        0     6252 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/error_handling/exceptions.py
--rw-r--r--   0        0        0      205 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/hirearchical_dict.py
--rw-r--r--   0        0        0      706 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/operations.py
--rw-r--r--   0        0        0     5859 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/remotes.py
--rw-r--r--   0        0        0      868 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/__init__.py
--rw-r--r--   0        0        0     4168 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/config_resolver.py
--rw-r--r--   0        0        0      182 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/db.py
--rw-r--r--   0        0        0      295 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/defaults.py
--rw-r--r--   0        0        0       47 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/interactive.py
--rw-r--r--   0        0        0      389 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/models.py
--rw-r--r--   0        0        0     1401 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/static.py
--rw-r--r--   0        0        0      181 2024-04-23 09:00:35.455016 viewser-6.4.2/viewser/settings/validation.py
--rw-r--r--   0        0        0      387 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/storage/azure.py
--rw-r--r--   0        0        0     2443 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/storage/db.py
--rw-r--r--   0        0        0     1462 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/storage/metadata_storage_serializer.py
--rw-r--r--   0        0        0     1175 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/storage/model_object.py
--rw-r--r--   0        0        0        0 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/__init__.py
--rw-r--r--   0        0        0      842 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/animations.py
--rw-r--r--   0        0        0      322 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/ascii_art.py
--rw-r--r--   0        0        0        0 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/__init__.py
--rw-r--r--   0        0        0     3186 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/abc.py
--rw-r--r--   0        0        0      144 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/conventions.py
--rw-r--r--   0        0        0      830 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/errors.py
--rw-r--r--   0        0        0      291 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/formatters.py
--rw-r--r--   0        0        0      177 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/generic_models.py
--rw-r--r--   0        0        0      196 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/json_formatter.py
--rw-r--r--   0        0        0      443 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/sections.py
--rw-r--r--   0        0        0      103 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/formatting/styles.py
--rw-r--r--   0        0        0       32 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/models.py
--rw-r--r--   0        0        0       82 2024-04-23 09:00:35.459015 viewser-6.4.2/viewser/tui/utils.py
--rw-r--r--   0        0        0    18189 1970-01-01 00:00:00.000000 viewser-6.4.2/PKG-INFO
+-rw-r--r--   0        0        0    19916 2024-04-29 13:44:58.806424 viewser-6.5.0/LICENSE
+-rw-r--r--   0        0        0    22367 2024-04-29 13:44:58.806424 viewser-6.5.0/README.md
+-rw-r--r--   0        0        0      878 2024-04-29 13:44:58.806424 viewser-6.5.0/pyproject.toml
+-rw-r--r--   0        0        0       79 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/__init__.py
+-rw-r--r--   0        0        0     1779 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/cli.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/config/__init__.py
+-rw-r--r--   0        0        0     3184 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/config/cli.py
+-rw-r--r--   0        0        0       61 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/__init__.py
+-rw-r--r--   0        0        0     3733 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/cli.py
+-rw-r--r--   0        0        0     3484 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/formatting.py
+-rw-r--r--   0        0        0     2070 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/operations.py
+-rw-r--r--   0        0        0      909 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/documentation/wrapped_views_doc.py
+-rw-r--r--   0        0        0       21 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/help/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/help/cli.py
+-rw-r--r--   0        0        0      242 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/help/operations.py
+-rw-r--r--   0        0        0       22 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/logs/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/logs/cli.py
+-rw-r--r--   0        0        0       22 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/model/__init__.py
+-rw-r--r--   0        0        0     3531 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/model/cli.py
+-rw-r--r--   0        0        0      731 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/model/formatting.py
+-rw-r--r--   0        0        0        1 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/model/models.py
+-rw-r--r--   0        0        0       22 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/notebooks/__init__.py
+-rw-r--r--   0        0        0     1766 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/notebooks/cli.py
+-rw-r--r--   0        0        0     6167 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/notebooks/operations.py
+-rw-r--r--   0        0        0       60 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/queryset/__init__.py
+-rw-r--r--   0        0        0     2245 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/queryset/cli.py
+-rw-r--r--   0        0        0     2529 2024-04-29 13:44:58.806424 viewser-6.5.0/viewser/commands/queryset/config_drift.py
+-rw-r--r--   0        0        0     6209 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/drift_detection.py
+-rw-r--r--   0        0        0     1269 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/formatting.py
+-rw-r--r--   0        0        0    12542 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/integrity_checks.py
+-rw-r--r--   0        0        0      133 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/__init__.py
+-rw-r--r--   0        0        0     3059 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/column.py
+-rw-r--r--   0        0        0     7755 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/queryset.py
+-rw-r--r--   0        0        0     2285 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/transform.py
+-rw-r--r--   0        0        0      313 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/models/util.py
+-rw-r--r--   0        0        0     9112 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/operations.py
+-rw-r--r--   0        0        0      231 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/queryset/queryset_list.py
+-rw-r--r--   0        0        0       22 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/system/__init__.py
+-rw-r--r--   0        0        0     1816 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/system/cli.py
+-rw-r--r--   0        0        0     1371 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/system/formatting.py
+-rw-r--r--   0        0        0      481 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/commands/system/models.py
+-rw-r--r--   0        0        0       73 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/__init__.py
+-rw-r--r--   0        0        0     3929 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/checks.py
+-rw-r--r--   0        0        0     2164 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/error_handling.py
+-rw-r--r--   0        0        0     7304 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/errors.py
+-rw-r--r--   0        0        0     6252 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/error_handling/exceptions.py
+-rw-r--r--   0        0        0      205 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/hirearchical_dict.py
+-rw-r--r--   0        0        0      706 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/operations.py
+-rw-r--r--   0        0        0     5859 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/remotes.py
+-rw-r--r--   0        0        0      868 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/__init__.py
+-rw-r--r--   0        0        0     4168 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/config_resolver.py
+-rw-r--r--   0        0        0      182 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/db.py
+-rw-r--r--   0        0        0      295 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/defaults.py
+-rw-r--r--   0        0        0       47 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/interactive.py
+-rw-r--r--   0        0        0      389 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/models.py
+-rw-r--r--   0        0        0     1401 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/static.py
+-rw-r--r--   0        0        0      181 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/settings/validation.py
+-rw-r--r--   0        0        0      387 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/storage/azure.py
+-rw-r--r--   0        0        0     2443 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/storage/db.py
+-rw-r--r--   0        0        0     1462 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/storage/metadata_storage_serializer.py
+-rw-r--r--   0        0        0     1175 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/storage/model_object.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/__init__.py
+-rw-r--r--   0        0        0      842 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/animations.py
+-rw-r--r--   0        0        0      322 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/ascii_art.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/__init__.py
+-rw-r--r--   0        0        0     3186 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/abc.py
+-rw-r--r--   0        0        0      144 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/conventions.py
+-rw-r--r--   0        0        0      830 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/errors.py
+-rw-r--r--   0        0        0      291 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/formatters.py
+-rw-r--r--   0        0        0      177 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/generic_models.py
+-rw-r--r--   0        0        0      196 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/json_formatter.py
+-rw-r--r--   0        0        0      443 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/sections.py
+-rw-r--r--   0        0        0      103 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/formatting/styles.py
+-rw-r--r--   0        0        0       32 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/models.py
+-rw-r--r--   0        0        0       82 2024-04-29 13:44:58.810423 viewser-6.5.0/viewser/tui/utils.py
+-rw-r--r--   0        0        0    23702 1970-01-01 00:00:00.000000 viewser-6.5.0/PKG-INFO
```

### Comparing `viewser-6.4.2/LICENSE` & `viewser-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/README.md` & `viewser-6.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -70,21 +70,31 @@
 
 with <loa> being one of ['any', 'country_month', 'priogrid_month', 'priogrid_year']
 
 Show docstring for a particular transform:
 
 `viewser transforms show <transform-name>`
 
+List querysets stored in the queryset database:
+
+`viewser querysets list`
+
+Produce code required to generate a queryset
+
+`viewser querysets show <queryset-name>`
+
 ## Via API
 
 The full functionality of viewser is exposed via its API for use in scripts and notebooks
 
 The two fundamental objects used to define what data is fetched by the client are the *Queryset* and the *Column*, where a 
 Queryset consists of one or more Columns. 
 
+### Defining a new queryset from scratch
+
 To define a queryset, one first imports the Queryset and Column classes
 
 `from viewser import Queryset, Column`
 
 A new queryset is then created by 
 
 `new_queryset = (Queryset("queryset_name", "level of analysis"))`
@@ -120,15 +130,15 @@
 
 The second argument to the Column instance `from_loa` specifies which level of analysis the requested raw data is defined at. If the user does not know this, they need to examine the database using the viewser CLI. 
 
 If the wrong loa is specified, the queryset will be rejected by the server and an error message detailing which columns have been requested from the wrong loa will be returned.
 
 The final argument to the Column instance is the name of the raw column to be fetched from the database. If a non-existant column is requested, the queryset will be rejected by the server and an error message detailing which columns are unavailable will be returned.
 
-## Aggregation/disaggregation
+#### Aggregation/disaggregation
 
 The definition of a queryset must include the *target* level of analysis, at which the resulting data will be presented to the user.
 
 The definition of each column in a queryset must specify the *source* level of analysis, at which the raw data used to define that column is stored in the database.
 
 If these loas differ for a given column, the necessary aggregation or disaggregation is performed automatically.
 
@@ -149,15 +159,15 @@
                .with_column(Column("ged_sb", from_loa="country_month", from_column="ged_sb_best_sum_nokgi")
                             .aggregate('avg')
                            )
                    )
 
 If a non-existent aggregation function is specified, the queryset will be rejected by the server and an error message detailing which columns have incorrect aggregation functions will be returned.
 
-## Transforms
+#### Transforms
 
 Any queryset column may specify an arbitrary number of transforms to be done to the raw data *after* any necessary aggregation/disaggregation has been done.
 
 Transforms are added to columns using the `transform` method
 
     new_queryset = (Queryset("simple_conflict", "country_month")
 
@@ -170,21 +180,37 @@
 
 Each transform method has a general transform type, e.g. `missing` followed by a specific function with brackets for arguments.
 
 A list of available transforms can be obtained using the viewser CLI. A notebook giving examples of what each transform does can be found at https://github.com/prio-data/views3/tree/master/examples.
 
 Note that not all transforms are available at all levels of analysis. If a transform is requested at an innapproprite loa, the queryset will be rejected by the server and an error message detailing which columns have requested incompatible transforms and loas will be returned.
 
-## Publising a queryset
+### Making a new queryset by merging two or more existing querysets
+
+It is sometimes desirable to make a larger queryset by merging several existing querysets. This can be done with the from_merger method. The method requires at mininum a list of querysets to be merged and a name for the merged queryset. Optionally, a theme and description can also be passed. There is also a boolean verbose flag, described below.
+For example
+    
+    querysets_to_merge = ['queryset1','querysets2','queryset3']
+    merged_queryset = Queryset.from_merger(querysets_to_merge,'my_merged_queryset',theme='my_theme',description='description')
+
+Before merging, some checks are performed. The querysets to be merged must all have the same target LOA. If the querysets to be merged contain two or more columns with the same name, the method checks that all the definitions of that column are exactly the same (same raw data, same transforms with same parameters). If this is the case, one copy of this column is included in the merged queryset (if the verbose flag is True, the method reports that this has been done). If there are multiple definitions of the columns with the same column name, the attempt at merging is aborted.
+
+### Recreating a queryset from storage
+
+If a queryset has already been published to the queryset store (see below), the queryset object can be regenerated by doing
+
+    queryset = Queryset.from_storage(queryset_name)
+
+### Publising a queryset
 
-Before a queryset can be fetched, it must be published to a permanent database on the server. This is done using the `publish()` method:
+Before a new queryset (written from scratch or created by merging existing querysets) can be fetched, it must be published to a permanent database on the server. This is done using the `publish()` method:
 
     data = new_queryset.publish()
 
-## Fetching a queryset
+### Fetching a queryset
 
 A published queryset can be fetched using the `.fetch()` method
 
     data = new_queryset.fetch()
 
 which can also be chained with the `publish()` method:
 
@@ -265,10 +291,60 @@
 
 This message indicates only that the queryset is waiting in the transform queue. Once computation of transforms begins, the status message will be replaced by one of the form
 
 `Queryset [queryset name] transform in progress - l of m jobs remaining`
 
 When all transforms have completed, downloading of the completed dataframe begins. The status message at this point will cease updating, which can make it appear that the client is hung in the case of large querysets. Users are asked to be patient :) .
 
+## Input drift detection
+
+The viewser package is able to perform a series of tests on the data fetched from the remote service which are designed to detect, and issue warnings about, anomalies in the data. 
+
+Two broad types of anomaly can be monitored
+
+### Global anomalies
+
+These examine the whole dataset, whatever its dimensions (thought on terms of time_units x space_units x features). The available anomaly detectors are
+
+ - global_missingness: simply reports if the total fraction of missing (i.e. NaN) values across the whole dataset exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - global zeros: reports if the total fraction of zero values across the whole dataset exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - time_missingness: reports if the fraction of missingness across any (space_units x features) slices exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - space_missingness: reports if the fraction of missingness across any (time_units x features) slices exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - feature_missingness: reports if the fraction of missingness for any feature (over all time and space units) exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - time_zeros: reports if the fraction of zeros across any (space_units x features) slices exceeds a threshold. Threshold should be a number between 0 and 1 and close to 1, e.g. 0.95.
+
+
+ - space_zeros: reports if the fraction of zeros across any (time_units x features) slices exceeds a threshold. Threshold should be a number between 0 and 1 close to 1, e.g. 0.95.
+
+
+ - feature_zeros: reports if the fraction of zeros for any feature (over all time and space units) exceeds a threshold. Threshold should be a number between 0 and 1 close to 1, e.g. 0.95.
+
+
+### Recent data anomalies
+These partition the dataset into three partitions, defined by two integers n and m. If the most recent time unit in the dateset is k: the test partition consists of the most recent n time units, i.e. k-n+1 to k inclusive (usually n would be 1 so the test parition simply consists of the most recent time unit k), the standard partition consists of the most recent k-m-n to k-n time units. The time units before k-m-n are discarded. The available anomaly detectors are
+- delta_completeness: reports, for each feature, if the ratio of missingness fractions in the test and standard partitions is greater than a threshold. Threshold should be a number between 0 and 1, e.g. 0.25.
+
+
+- delta_zeros: reports, for each feature, if the ratio of the fraction of zeros in the test and standard partitions is greater than a threshold. Threshold should be a number between 0 and 1, e.g. 0.25.
+
+
+- extreme_values: reports, for each feature, if the most extreme value in the test partition is more than (threshold) standard deviations from the mean of the data in the test partition. Threshold should be a number in the range 2-7, e.g. 5.
+
+
+- ks_drift: for each feature, performs a two-sample Kolmogorov-Smirnoff test (https://en.wikipedia.org/wiki/Kolmogorov–Smirnov_test#Two-sample_Kolmogorov–Smirnov_test) between the data in the test and standard partitions and reports if (1/the returned p-value) exceeds a threshold. Threshold should be a large number, e.g. 100.
+
+
+- ecod_drift: for all features simultaneously, reports if the fraction of data-points considered outliers in the test partition exceeds that in the standard partition, according to an ECOD model (https://pyod.readthedocs.io/en/latest/_modules/pyod/models/ecod.html#ECOD) trained on the standard partition, exceeds a threshold. Threshold should be a number between 0 and 1, e.g. 0.25.
+
 ## Funding
 
 The contents of this repository is the outcome of projects that have received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 694640, *ViEWS*) and Horizon Europe (Grant agreement No. 101055176, *ANTICIPATE*; and No. 101069312, *ViEWS* (ERC-2022-POC1)), Riksbankens Jubileumsfond (Grant agreement No. M21-0002, *Societies at Risk*), Uppsala University, Peace Research Institute Oslo, the United Nations Economic and Social Commission for Western Asia (*ViEWS-ESCWA*), the United Kingdom Foreign, Commonwealth & Development Office (GSRA – *Forecasting Fatalities in Armed Conflict*), the Swedish Research Council (*DEMSCORE*), the Swedish Foundation for Strategic Environmental Research (*MISTRA Geopolitics*), the Norwegian MFA (*Conflict Trends* QZA-18/0227), and the United Nations High Commissioner for Refugees (*the Sahel Predictive Analytics project*).
```

### Comparing `viewser-6.4.2/pyproject.toml` & `viewser-6.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "viewser"
-version = "6.4.2"
+version = "6.5.0"
 description = "The Views 3 CLI tool"
 authors = ["peder2911 <pglandsverk@gmail.com>"]
 readme = "README.md"
 homepage = "https://www.github.com/prio-data/viewser"
 license = "CC-BY-NC"
 
 [tool.poetry.dependencies]
```

### Comparing `viewser-6.4.2/viewser/cli.py` & `viewser-6.5.0/viewser/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/config/cli.py` & `viewser-6.5.0/viewser/commands/config/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/documentation/cli.py` & `viewser-6.5.0/viewser/commands/documentation/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/documentation/formatting.py` & `viewser-6.5.0/viewser/commands/documentation/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/documentation/operations.py` & `viewser-6.5.0/viewser/commands/documentation/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/documentation/wrapped_views_doc.py` & `viewser-6.5.0/viewser/commands/documentation/wrapped_views_doc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/help/cli.py` & `viewser-6.5.0/viewser/commands/help/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/model/cli.py` & `viewser-6.5.0/viewser/commands/model/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/model/formatting.py` & `viewser-6.5.0/viewser/commands/model/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/notebooks/cli.py` & `viewser-6.5.0/viewser/commands/notebooks/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/notebooks/operations.py` & `viewser-6.5.0/viewser/commands/notebooks/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/queryset/cli.py` & `viewser-6.5.0/viewser/commands/queryset/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/queryset/formatting.py` & `viewser-6.5.0/viewser/commands/queryset/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/queryset/models/column.py` & `viewser-6.5.0/viewser/commands/queryset/models/column.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/queryset/models/queryset.py` & `viewser-6.5.0/viewser/commands/queryset/models/queryset.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
+import requests
 from views_schema import queryset_manager as schema
 from viewser.commands.queryset.operations import QuerysetOperations
 from viewser import settings
 from viewser.settings import defaults
 from . import column, util
 
 logger = logging.getLogger(__name__)
 queryset_operations = QuerysetOperations(
         settings.QUERYSET_URL,
         defaults.default_error_handler())
 
+
 class Queryset(schema.Queryset):
     """
     Queryset
     ========
 
     parameters:
         name (str): Unique name
@@ -38,14 +40,48 @@
     Most methods can be chained, allowing for concise, readable queryset
     definitions.
     """
     def __init__(self, name, loa):
         super().__init__(name=name, loa=loa, operations=[])
 
     @classmethod
+    def from_storage(cls, name):
+
+        config = settings.config_resolver.ConfigResolver(settings.db.Session)
+
+        remote_url = config.get("REMOTE_URL")
+
+        response = requests.request(method="GET", url=f'{remote_url}/querysets/querysets/{name}')
+
+        if response.status_code == 404:
+            raise RuntimeError(f'queryset {name} does not appear to be in the queryset store')
+
+        json_ = response.json()
+
+        allowed_fields = ['name', 'loa', 'description', 'themes', 'operations']
+        allowed_namespaces = ['base', 'trf']
+
+        for key in json_.keys():
+            if key not in allowed_fields:
+                raise RuntimeError(f'Queryset json contains unrecognised field: {key}')
+
+        for column in json_['operations']:
+            for operation in column:
+                if operation['namespace'] not in allowed_namespaces:
+                    raise RuntimeError(f"Queryset operation contains unrecognised namespace: {operation['namespace']}")
+
+        qs = cls(name=json_['name'], loa=json_['loa'])
+
+        qs.operations = json_['operations']
+        qs.themes = json_['themes']
+        qs.description = json_['description']
+
+        return qs
+
+    @classmethod
     def from_merger(cls, querysets, name, theme=None, description=None, verbose=False):
 
         def rename_to_string(column):
             rename_string = ''.join([column[0].namespace, column[0].name, str(column[0].arguments)])
             return rename_string
 
         def database_to_string(column):
@@ -100,15 +136,15 @@
                         database_strings.append(database_string)
                         transform_strings.append(transform_string)
                         columns.append(column)
 
         qs_merged = cls(name=name, loa=loas[0])
 
         qs_merged.operations = columns
-        qs_merged.themes = [] if theme is None else [theme,]
+        qs_merged.themes = [] if theme is None else [theme, ]
         qs_merged.description = description
 
         return qs_merged
 
     @util.deepcopy_self
     def with_column(self, col: column.Column):
         """
@@ -183,7 +219,22 @@
 
         Fetch the dataset corresponding to this queryset in its current state.
         Requires a self.push first.
         """
         logger.info(f"Fetching queryset {self.name}")
         dataset = queryset_operations.fetch(self.name, *args, **kwargs)
         return dataset
+
+    def fetch_with_drift_detection(self, *args, **kwargs):
+        """
+        fetch
+        =====
+
+        returns:
+            pandas.DataFrame
+
+        Fetch the dataset corresponding to this queryset in its current state.
+        Requires a self.push first.
+        """
+        logger.info(f"Fetching queryset {self.name}")
+        dataset = queryset_operations.fetch_with_drift_detection(self.name, *args, **kwargs)
+        return dataset
```

### Comparing `viewser-6.4.2/viewser/commands/queryset/models/transform.py` & `viewser-6.5.0/viewser/commands/queryset/models/transform.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/queryset/operations.py` & `viewser-6.5.0/viewser/commands/queryset/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 queryset_operations
 ===================
 
 """
 import sys
 import time
-from typing import Optional
+from typing import Optional, Dict
 from urllib import parse
 from tqdm import tqdm
 import json
 import logging
 import pandas as pd
 import io
 import requests
 from views_schema import queryset_manager as queryset_schema
 from viewser.error_handling import error_handling
 
 from IPython.display import clear_output
 
 from . import queryset_list
+from . import drift_detection
 
 logger = logging.getLogger(__name__)
 
 
 class QuerysetOperations():
 
     def __init__(self,
@@ -70,14 +71,39 @@
             queryset_name,
             start_date,
             end_date
             )
 
         return f
 
+    def fetch_with_drift_detection(self, queryset_name: str, start_date: str, end_date: str, drift_config_dict:
+                                   Optional[Dict]):
+        """
+        fetch_with_drift_detection
+        =====
+
+        parameters:
+            queryset_name (str): Name of the queryset to fetch
+            start_date: first month to include in output
+            end_data: last month to include in output
+            drift_config_dict: dictionary specifying which drift detection parameters to use
+
+        returns:
+            Dataframe corresponding to queryset (if query succeeds)
+
+        """
+
+        f = self.fetch(queryset_name, start_date, end_date)
+
+        input_gate = drift_detection.InputGate(f, drift_config_dict=drift_config_dict)
+
+        alerts = input_gate.assemble_alerts()
+
+        return f, alerts
+
     def list(self):
         """
         list
         ====
 
         returns:
             Returns a list of queryset names if operation succeeds.
```

### Comparing `viewser-6.4.2/viewser/commands/system/cli.py` & `viewser-6.5.0/viewser/commands/system/cli.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/commands/system/formatting.py` & `viewser-6.5.0/viewser/commands/system/formatting.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/error_handling/checks.py` & `viewser-6.5.0/viewser/error_handling/checks.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/error_handling/error_handling.py` & `viewser-6.5.0/viewser/error_handling/error_handling.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/error_handling/errors.py` & `viewser-6.5.0/viewser/error_handling/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/error_handling/exceptions.py` & `viewser-6.5.0/viewser/error_handling/exceptions.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/operations.py` & `viewser-6.5.0/viewser/operations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/remotes.py` & `viewser-6.5.0/viewser/remotes.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/settings/__init__.py` & `viewser-6.5.0/viewser/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/settings/config_resolver.py` & `viewser-6.5.0/viewser/settings/config_resolver.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/settings/static.py` & `viewser-6.5.0/viewser/settings/static.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/storage/db.py` & `viewser-6.5.0/viewser/storage/db.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/storage/metadata_storage_serializer.py` & `viewser-6.5.0/viewser/storage/metadata_storage_serializer.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/storage/model_object.py` & `viewser-6.5.0/viewser/storage/model_object.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/tui/animations.py` & `viewser-6.5.0/viewser/tui/animations.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/tui/formatting/abc.py` & `viewser-6.5.0/viewser/tui/formatting/abc.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/viewser/tui/formatting/errors.py` & `viewser-6.5.0/viewser/tui/formatting/errors.py`

 * *Files identical despite different names*

### Comparing `viewser-6.4.2/PKG-INFO` & `viewser-6.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viewser
-Version: 6.4.2
+Version: 6.5.0
 Summary: The Views 3 CLI tool
 Home-page: https://www.github.com/prio-data/viewser
 License: CC-BY-NC
 Author: peder2911
 Author-email: pglandsverk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -106,21 +106,31 @@
 
 with <loa> being one of ['any', 'country_month', 'priogrid_month', 'priogrid_year']
 
 Show docstring for a particular transform:
 
 `viewser transforms show <transform-name>`
 
+List querysets stored in the queryset database:
+
+`viewser querysets list`
+
+Produce code required to generate a queryset
+
+`viewser querysets show <queryset-name>`
+
 ## Via API
 
 The full functionality of viewser is exposed via its API for use in scripts and notebooks
 
 The two fundamental objects used to define what data is fetched by the client are the *Queryset* and the *Column*, where a 
 Queryset consists of one or more Columns. 
 
+### Defining a new queryset from scratch
+
 To define a queryset, one first imports the Queryset and Column classes
 
 `from viewser import Queryset, Column`
 
 A new queryset is then created by 
 
 `new_queryset = (Queryset("queryset_name", "level of analysis"))`
@@ -156,15 +166,15 @@
 
 The second argument to the Column instance `from_loa` specifies which level of analysis the requested raw data is defined at. If the user does not know this, they need to examine the database using the viewser CLI. 
 
 If the wrong loa is specified, the queryset will be rejected by the server and an error message detailing which columns have been requested from the wrong loa will be returned.
 
 The final argument to the Column instance is the name of the raw column to be fetched from the database. If a non-existant column is requested, the queryset will be rejected by the server and an error message detailing which columns are unavailable will be returned.
 
-## Aggregation/disaggregation
+#### Aggregation/disaggregation
 
 The definition of a queryset must include the *target* level of analysis, at which the resulting data will be presented to the user.
 
 The definition of each column in a queryset must specify the *source* level of analysis, at which the raw data used to define that column is stored in the database.
 
 If these loas differ for a given column, the necessary aggregation or disaggregation is performed automatically.
 
@@ -185,15 +195,15 @@
                .with_column(Column("ged_sb", from_loa="country_month", from_column="ged_sb_best_sum_nokgi")
                             .aggregate('avg')
                            )
                    )
 
 If a non-existent aggregation function is specified, the queryset will be rejected by the server and an error message detailing which columns have incorrect aggregation functions will be returned.
 
-## Transforms
+#### Transforms
 
 Any queryset column may specify an arbitrary number of transforms to be done to the raw data *after* any necessary aggregation/disaggregation has been done.
 
 Transforms are added to columns using the `transform` method
 
     new_queryset = (Queryset("simple_conflict", "country_month")
 
@@ -206,21 +216,37 @@
 
 Each transform method has a general transform type, e.g. `missing` followed by a specific function with brackets for arguments.
 
 A list of available transforms can be obtained using the viewser CLI. A notebook giving examples of what each transform does can be found at https://github.com/prio-data/views3/tree/master/examples.
 
 Note that not all transforms are available at all levels of analysis. If a transform is requested at an innapproprite loa, the queryset will be rejected by the server and an error message detailing which columns have requested incompatible transforms and loas will be returned.
 
-## Publising a queryset
+### Making a new queryset by merging two or more existing querysets
+
+It is sometimes desirable to make a larger queryset by merging several existing querysets. This can be done with the from_merger method. The method requires at mininum a list of querysets to be merged and a name for the merged queryset. Optionally, a theme and description can also be passed. There is also a boolean verbose flag, described below.
+For example
+    
+    querysets_to_merge = ['queryset1','querysets2','queryset3']
+    merged_queryset = Queryset.from_merger(querysets_to_merge,'my_merged_queryset',theme='my_theme',description='description')
+
+Before merging, some checks are performed. The querysets to be merged must all have the same target LOA. If the querysets to be merged contain two or more columns with the same name, the method checks that all the definitions of that column are exactly the same (same raw data, same transforms with same parameters). If this is the case, one copy of this column is included in the merged queryset (if the verbose flag is True, the method reports that this has been done). If there are multiple definitions of the columns with the same column name, the attempt at merging is aborted.
+
+### Recreating a queryset from storage
+
+If a queryset has already been published to the queryset store (see below), the queryset object can be regenerated by doing
+
+    queryset = Queryset.from_storage(queryset_name)
+
+### Publising a queryset
 
-Before a queryset can be fetched, it must be published to a permanent database on the server. This is done using the `publish()` method:
+Before a new queryset (written from scratch or created by merging existing querysets) can be fetched, it must be published to a permanent database on the server. This is done using the `publish()` method:
 
     data = new_queryset.publish()
 
-## Fetching a queryset
+### Fetching a queryset
 
 A published queryset can be fetched using the `.fetch()` method
 
     data = new_queryset.fetch()
 
 which can also be chained with the `publish()` method:
 
@@ -301,11 +327,61 @@
 
 This message indicates only that the queryset is waiting in the transform queue. Once computation of transforms begins, the status message will be replaced by one of the form
 
 `Queryset [queryset name] transform in progress - l of m jobs remaining`
 
 When all transforms have completed, downloading of the completed dataframe begins. The status message at this point will cease updating, which can make it appear that the client is hung in the case of large querysets. Users are asked to be patient :) .
 
+## Input drift detection
+
+The viewser package is able to perform a series of tests on the data fetched from the remote service which are designed to detect, and issue warnings about, anomalies in the data. 
+
+Two broad types of anomaly can be monitored
+
+### Global anomalies
+
+These examine the whole dataset, whatever its dimensions (thought on terms of time_units x space_units x features). The available anomaly detectors are
+
+ - global_missingness: simply reports if the total fraction of missing (i.e. NaN) values across the whole dataset exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - global zeros: reports if the total fraction of zero values across the whole dataset exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - time_missingness: reports if the fraction of missingness across any (space_units x features) slices exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - space_missingness: reports if the fraction of missingness across any (time_units x features) slices exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - feature_missingness: reports if the fraction of missingness for any feature (over all time and space units) exceeds a threshold. Threshold should be a small number between 0 and 1, e.g. 0.05.
+
+
+ - time_zeros: reports if the fraction of zeros across any (space_units x features) slices exceeds a threshold. Threshold should be a number between 0 and 1 and close to 1, e.g. 0.95.
+
+
+ - space_zeros: reports if the fraction of zeros across any (time_units x features) slices exceeds a threshold. Threshold should be a number between 0 and 1 close to 1, e.g. 0.95.
+
+
+ - feature_zeros: reports if the fraction of zeros for any feature (over all time and space units) exceeds a threshold. Threshold should be a number between 0 and 1 close to 1, e.g. 0.95.
+
+
+### Recent data anomalies
+These partition the dataset into three partitions, defined by two integers n and m. If the most recent time unit in the dateset is k: the test partition consists of the most recent n time units, i.e. k-n+1 to k inclusive (usually n would be 1 so the test parition simply consists of the most recent time unit k), the standard partition consists of the most recent k-m-n to k-n time units. The time units before k-m-n are discarded. The available anomaly detectors are
+- delta_completeness: reports, for each feature, if the ratio of missingness fractions in the test and standard partitions is greater than a threshold. Threshold should be a number between 0 and 1, e.g. 0.25.
+
+
+- delta_zeros: reports, for each feature, if the ratio of the fraction of zeros in the test and standard partitions is greater than a threshold. Threshold should be a number between 0 and 1, e.g. 0.25.
+
+
+- extreme_values: reports, for each feature, if the most extreme value in the test partition is more than (threshold) standard deviations from the mean of the data in the test partition. Threshold should be a number in the range 2-7, e.g. 5.
+
+
+- ks_drift: for each feature, performs a two-sample Kolmogorov-Smirnoff test (https://en.wikipedia.org/wiki/Kolmogorov–Smirnov_test#Two-sample_Kolmogorov–Smirnov_test) between the data in the test and standard partitions and reports if (1/the returned p-value) exceeds a threshold. Threshold should be a large number, e.g. 100.
+
+
+- ecod_drift: for all features simultaneously, reports if the fraction of data-points considered outliers in the test partition exceeds that in the standard partition, according to an ECOD model (https://pyod.readthedocs.io/en/latest/_modules/pyod/models/ecod.html#ECOD) trained on the standard partition, exceeds a threshold. Threshold should be a number between 0 and 1, e.g. 0.25.
+
 ## Funding
 
 The contents of this repository is the outcome of projects that have received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 694640, *ViEWS*) and Horizon Europe (Grant agreement No. 101055176, *ANTICIPATE*; and No. 101069312, *ViEWS* (ERC-2022-POC1)), Riksbankens Jubileumsfond (Grant agreement No. M21-0002, *Societies at Risk*), Uppsala University, Peace Research Institute Oslo, the United Nations Economic and Social Commission for Western Asia (*ViEWS-ESCWA*), the United Kingdom Foreign, Commonwealth & Development Office (GSRA – *Forecasting Fatalities in Armed Conflict*), the Swedish Research Council (*DEMSCORE*), the Swedish Foundation for Strategic Environmental Research (*MISTRA Geopolitics*), the Norwegian MFA (*Conflict Trends* QZA-18/0227), and the United Nations High Commissioner for Refugees (*the Sahel Predictive Analytics project*).
```

