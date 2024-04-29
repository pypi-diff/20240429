# Comparing `tmp/emzed_gui-3.0.0a8.tar.gz` & `tmp/emzed_gui-3.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emzed_gui-3.0.0a8.tar", last modified: Fri Aug 25 07:55:49 2023, max compression
+gzip compressed data, was "emzed_gui-3.0.0a9.tar", last modified: Fri Oct 20 08:50:33 2023, max compression
```

## Comparing `emzed_gui-3.0.0a8.tar` & `emzed_gui-3.0.0a9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.655383 emzed_gui-3.0.0a8/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-07-31 14:44:51.000000 emzed_gui-3.0.0a8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      159 2023-08-25 07:55:49.655383 emzed_gui-3.0.0a8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-31 14:44:51.000000 emzed_gui-3.0.0a8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-25 07:55:49.655383 emzed_gui-3.0.0a8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-08-25 07:52:43.000000 emzed_gui-3.0.0a8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.640383 emzed_gui-3.0.0a8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.642383 emzed_gui-3.0.0a8/src/emzed_gui/
--rw-rw-rw-   0 root         (0) root         (0)     3560 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3127 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/_qt_compat.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/configs.py
--rwxrwxrwx   0 root         (0) root         (0)    10804 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/dialog_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     2044 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/emzed_dialog.py
--rwxrwxrwx   0 root         (0) root         (0)     5044 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/file_dialogs.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/fix_import_order.py
--rw-rw-rw-   0 root         (0) root         (0)     2506 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-07-31 14:44:51.000000 emzed_gui-3.0.0a8/src/emzed_gui/inspect.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2023-07-31 14:44:51.000000 emzed_gui-3.0.0a8/src/emzed_gui/inspectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.648383 emzed_gui-3.0.0a8/src/emzed_gui/optimized/
--rw-rw-rw-   0 root         (0) root         (0)     1829 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/optimized/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1142893 2023-08-25 07:55:48.000000 emzed_gui-3.0.0a8/src/emzed_gui/optimized/optimized.c
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/optimized/optimized.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.648383 emzed_gui-3.0.0a8/src/emzed_gui/peakmap_explorer/
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/peakmap_explorer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25909 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/peakmap_explorer/peakmap_explorer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.649383 emzed_gui-3.0.0a8/src/emzed_gui/resources/
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    35620 2023-07-31 14:44:51.000000 emzed_gui-3.0.0a8/src/emzed_gui/resources/icon64.png
--rw-rw-rw-   0 root         (0) root         (0)     1737 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/simple_dialogs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.651383 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/_debug.py
--rw-rw-rw-   0 root         (0) root         (0)     3174 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/_table_explorer_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/ask_value.py
--rw-rw-rw-   0 root         (0) root         (0)     5215 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/async_runner.py
--rw-rw-rw-   0 root         (0) root         (0)     2094 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/button_delegate.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/image_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/inspect.py
--rwxrwxrwx   0 root         (0) root         (0)    43637 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_explorer.py
--rw-rw-rw-   0 root         (0) root         (0)     5596 2023-07-31 14:44:51.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_explorer_layout.py
--rwxrwxrwx   0 root         (0) root         (0)    32387 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_explorer_model.py
--rw-rw-rw-   0 root         (0) root         (0)    11644 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_explorer_model_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     4435 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_view.py
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/text_delegate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.654383 emzed_gui-3.0.0a8/src/emzed_gui/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1134 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5347 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_ask_value_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5712 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_choose_range.py
--rw-rw-rw-   0 root         (0) root         (0)     2969 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_choose_spectra_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     3380 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_choose_value.py
--rw-rw-rw-   0 root         (0) root         (0)     3439 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_column_selection_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4133 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_filter_criteria_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     8294 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_image_scaling_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     5987 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_integration_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     4619 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_spectra_selector_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     3483 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_string_filter.py
--rw-rw-rw-   0 root         (0) root         (0)     6631 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/_view_range_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     4142 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/ask_value_dialogs.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/choose_spectra_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     3182 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/column_selection_dialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/config.py
--rw-rw-rw-   0 root         (0) root         (0)    22839 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/eic_plotting_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     9914 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/filter_criteria_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     6077 2023-07-31 14:44:51.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/image_scaling_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     2577 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/integration_widget.py
--rwxrwxrwx   0 root         (0) root         (0)    14338 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/modified_guiqwt.py
--rw-rw-rw-   0 root         (0) root         (0)    16550 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/mz_plotting_widget.py
--rw-rw-rw-   0 root         (0) root         (0)    32240 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/peakmap_plotting_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     4479 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/spectra_selector_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     3357 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/ts_plotting_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     5043 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/src/emzed_gui/widgets/view_range_widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.647383 emzed_gui-3.0.0a8/src/emzed_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)      159 2023-08-25 07:55:49.000000 emzed_gui-3.0.0a8/src/emzed_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2732 2023-08-25 07:55:49.000000 emzed_gui-3.0.0a8/src/emzed_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-25 07:55:49.000000 emzed_gui-3.0.0a8/src/emzed_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-25 07:53:03.000000 emzed_gui-3.0.0a8/src/emzed_gui.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       89 2023-08-25 07:55:49.000000 emzed_gui-3.0.0a8/src/emzed_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-08-25 07:55:49.000000 emzed_gui-3.0.0a8/src/emzed_gui.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-25 07:55:49.655383 emzed_gui-3.0.0a8/tests/
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-01 21:00:31.000000 emzed_gui-3.0.0a8/tests/test_import.py
--rw-rw-rw-   0 root         (0) root         (0)     1540 2023-08-25 07:46:03.000000 emzed_gui-3.0.0a8/tests/test_peak_map_optimizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.067046 emzed_gui-3.0.0a9/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2023-10-20 08:50:33.066046 emzed_gui-3.0.0a9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-10-20 08:50:33.067046 emzed_gui-3.0.0a9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.055046 emzed_gui-3.0.0a9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.058046 emzed_gui-3.0.0a9/src/emzed_gui/
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3127 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/_qt_compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/configs.py
+-rwxrwxrwx   0 root         (0) root         (0)    10804 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/dialog_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2044 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/emzed_dialog.py
+-rwxrwxrwx   0 root         (0) root         (0)     5044 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/file_dialogs.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/fix_import_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)     1558 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/inspectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.060046 emzed_gui-3.0.0a9/src/emzed_gui/optimized/
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/optimized/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1175944 2023-10-20 08:50:32.000000 emzed_gui-3.0.0a9/src/emzed_gui/optimized/optimized.c
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/optimized/optimized.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.060046 emzed_gui-3.0.0a9/src/emzed_gui/peakmap_explorer/
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/peakmap_explorer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25909 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/peakmap_explorer/peakmap_explorer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.061046 emzed_gui-3.0.0a9/src/emzed_gui/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      787 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    35620 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/resources/icon64.png
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/simple_dialogs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.062046 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/_debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     3174 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/_table_explorer_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/ask_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/async_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/button_delegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/image_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/inspect.py
+-rwxrwxrwx   0 root         (0) root         (0)    43477 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_explorer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5596 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_explorer_layout.py
+-rwxrwxrwx   0 root         (0) root         (0)    32300 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_explorer_model.py
+-rw-rw-rw-   0 root         (0) root         (0)    11644 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_explorer_model_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4435 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_view.py
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/text_delegate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.066046 emzed_gui-3.0.0a9/src/emzed_gui/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5347 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_ask_value_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5712 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_choose_range.py
+-rw-rw-rw-   0 root         (0) root         (0)     2969 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_choose_spectra_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     3380 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_choose_value.py
+-rw-rw-rw-   0 root         (0) root         (0)     3439 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_column_selection_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4133 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_filter_criteria_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     8294 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_image_scaling_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5987 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_integration_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     4619 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_spectra_selector_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     3483 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_string_filter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6631 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/_view_range_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     4142 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/ask_value_dialogs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/choose_spectra_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     3182 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/column_selection_dialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    22915 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/eic_plotting_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     9914 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/filter_criteria_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     6077 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/image_scaling_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/integration_widget.py
+-rwxrwxrwx   0 root         (0) root         (0)    14338 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/modified_guiqwt.py
+-rw-rw-rw-   0 root         (0) root         (0)    16550 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/mz_plotting_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)    32240 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/peakmap_plotting_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/spectra_selector_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     3357 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/ts_plotting_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     5043 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/src/emzed_gui/widgets/view_range_widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.059046 emzed_gui-3.0.0a9/src/emzed_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-10-20 08:50:33.000000 emzed_gui-3.0.0a9/src/emzed_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-10-20 08:50:33.000000 emzed_gui-3.0.0a9/src/emzed_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-20 08:50:33.000000 emzed_gui-3.0.0a9/src/emzed_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-20 08:47:54.000000 emzed_gui-3.0.0a9/src/emzed_gui.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       89 2023-10-20 08:50:33.000000 emzed_gui-3.0.0a9/src/emzed_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-10-20 08:50:33.000000 emzed_gui-3.0.0a9/src/emzed_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-20 08:50:33.066046 emzed_gui-3.0.0a9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/tests/test_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     1540 2023-10-20 08:47:37.000000 emzed_gui-3.0.0a9/tests/test_peak_map_optimizations.py
```

### Comparing `emzed_gui-3.0.0a8/LICENSE` & `emzed_gui-3.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/setup.py` & `emzed_gui-3.0.0a9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             include_dirs=[numpy.get_include()],
         )
     ]
 )
 
 setup(
     name="emzed_gui",
-    version="3.0.0a8",
+    version="3.0.0a9",
     description="",
     url="",
     author="Uwe Schmitt",
     author_email="uwe.schmitt@id.ethz.ch",
     license="MIT",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/__init__.py` & `emzed_gui-3.0.0a9/src/emzed_gui/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/_qt_compat.py` & `emzed_gui-3.0.0a9/src/emzed_gui/_qt_compat.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/configs.py` & `emzed_gui-3.0.0a9/src/emzed_gui/configs.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/dialog_builder.py` & `emzed_gui-3.0.0a9/src/emzed_gui/dialog_builder.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/emzed_dialog.py` & `emzed_gui-3.0.0a9/src/emzed_gui/emzed_dialog.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/file_dialogs.py` & `emzed_gui-3.0.0a9/src/emzed_gui/file_dialogs.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/helpers.py` & `emzed_gui-3.0.0a9/src/emzed_gui/helpers.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/inspect.py` & `emzed_gui-3.0.0a9/src/emzed_gui/inspect.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/inspectors.py` & `emzed_gui-3.0.0a9/src/emzed_gui/inspectors.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/optimized/__init__.py` & `emzed_gui-3.0.0a9/src/emzed_gui/optimized/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/optimized/optimized.c` & `emzed_gui-3.0.0a9/src/emzed_gui/optimized/optimized.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 3.0.0 */
+/* Generated by Cython 3.0.4 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/core/include"
         ],
         "name": "emzed_gui.optimized.optimized",
         "sources": [
             "src/emzed_gui/optimized/optimized.pyx"
         ]
     },
     "module_name": "emzed_gui.optimized.optimized"
@@ -54,18 +54,23 @@
     #endif
     
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0"
+#if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
+#define __PYX_EXTRA_ABI_MODULE_NAME "limited"
+#else
+#define __PYX_EXTRA_ABI_MODULE_NAME ""
+#endif
+#define CYTHON_ABI "3_0_4" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000F0
+#define CYTHON_HEX_VERSION 0x030004F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,14 +95,15 @@
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
+#define __PYX_LIMITED_VERSION_HEX PY_VERSION_HEX
 #if defined(GRAALVM_PYTHON)
   /* For very preliminary testing purposes. Most variables are set the same as PyPy.
      The existence of this section does not imply that anything works or is even tested */
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 1
@@ -156,16 +162,17 @@
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
-  #undef CYTHON_USE_TYPE_SPECS
-  #define CYTHON_USE_TYPE_SPECS 0
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -209,14 +216,18 @@
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(CYTHON_LIMITED_API)
+  #ifdef Py_LIMITED_API
+    #undef __PYX_LIMITED_VERSION_HEX
+    #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
+  #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 1
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_CLINE_IN_TRACEBACK
   #define CYTHON_CLINE_IN_TRACEBACK 0
@@ -256,15 +267,15 @@
     #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_MODULE_STATE
   #define CYTHON_USE_MODULE_STATE 1
   #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
+    #define CYTHON_USE_TP_FINALIZE 0
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
@@ -478,14 +489,22 @@
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
+#ifndef CYTHON_USE_CPP_STD_MOVE
+  #if defined(__cplusplus) && (\
+    __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600))
+    #define CYTHON_USE_CPP_STD_MOVE 1
+  #else
+    #define CYTHON_USE_CPP_STD_MOVE 0
+  #endif
+#endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
             typedef unsigned char     uint8_t;
             typedef unsigned short    uint16_t;
             typedef unsigned int      uint32_t;
@@ -577,67 +596,99 @@
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_DefaultClassType PyClass_Type
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
   #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+#if CYTHON_COMPILING_IN_LIMITED_API
+    static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject *co=NULL, *result=NULL;
+        PyObject *exception_table = NULL;
+        PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
+        #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
+        PyObject *version_info; // borrowed
+        #endif
+        PyObject *py_minor_version = NULL;
+        long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
-        if (!(empty = PyTuple_New(0))) goto end;
-        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+        #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
+        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        #else
+        if (!(version_info = PySys_GetObject("version_info"))) goto end;
+        if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
+        minor_version = PyLong_AsLong(py_minor_version);
+        if (minor_version == -1 && PyErr_Occurred()) goto end;
+        #endif
+        if (!(types_module = PyImport_ImportModule("types"))) goto end;
+        if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
+        if (minor_version <= 7) {
+            (void)p;
+            result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else if (minor_version <= 10) {
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, fline, lnos, fv, cell);
+        } else {
+            if (!(exception_table = PyBytes_FromStringAndSize(NULL, 0))) goto end;
+            result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
+                          c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
+        }
     end:
-        Py_XDECREF((PyObject*) co);
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(empty);
+        Py_XDECREF(code_type);
+        Py_XDECREF(exception_table);
+        Py_XDECREF(types_module);
+        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
+    #ifndef CO_OPTIMIZED
+    #define CO_OPTIMIZED 0x0001
+    #endif
+    #ifndef CO_NEWLOCALS
+    #define CO_NEWLOCALS 0x0002
+    #endif
+    #ifndef CO_VARARGS
+    #define CO_VARARGS 0x0004
+    #endif
+    #ifndef CO_VARKEYWORDS
+    #define CO_VARKEYWORDS 0x0008
+    #endif
+    #ifndef CO_ASYNC_GENERATOR
+    #define CO_ASYNC_GENERATOR 0x0200
+    #endif
+    #ifndef CO_GENERATOR
+    #define CO_GENERATOR 0x0020
+    #endif
+    #ifndef CO_COROUTINE
+    #define CO_COROUTINE 0x0080
+    #endif
+#elif PY_VERSION_HEX >= 0x030B0000
+  static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+    PyCodeObject *result;
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    if (!empty_bytes) return NULL;
+    result =
+      #if PY_VERSION_HEX >= 0x030C0000
+        PyUnstable_Code_NewWithPosOnlyArgs
+      #else
+        PyCode_NewWithPosOnlyArgs
+      #endif
+        (a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, name, fline, lnos, empty_bytes);
+    Py_DECREF(empty_bytes);
+    return result;
+  }
 #elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
@@ -729,15 +780,40 @@
                                             size_t nargsf, PyObject *kwnames);
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
 #else
   #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
   #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
 #endif
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_MAJOR_VERSION >= 0x030900B1
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_CheckExact(func)
+#else
+#define __Pyx_PyCFunction_CheckExact(func)  PyCFunction_Check(func)
+#endif
+#define __Pyx_CyOrPyCFunction_Check(func)  PyCFunction_Check(func)
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  (((PyCFunctionObject*)(func))->m_ml->ml_meth)
+#elif !CYTHON_COMPILING_IN_LIMITED_API
+#define __Pyx_CyOrPyCFunction_GET_FUNCTION(func)  PyCFunction_GET_FUNCTION(func)
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_CyOrPyCFunction_GET_FLAGS(func)  (((PyCFunctionObject*)(func))->m_ml->ml_flags)
+static CYTHON_INLINE PyObject* __Pyx_CyOrPyCFunction_GET_SELF(PyObject *func) {
+    return (__Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_STATIC) ? NULL : ((PyCFunctionObject*)func)->m_self;
+}
+#endif
+static CYTHON_INLINE int __Pyx__IsSameCFunction(PyObject *func, void *cfunc) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    return PyCFunction_Check(func) && PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+#else
+    return PyCFunction_Check(func) && PyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+#endif
+}
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCFunction(func, cfunc)
+#if __PYX_LIMITED_VERSION_HEX < 0x030900B1
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
   typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
   #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
   #define __Pyx_PyCMethod  PyCMethod
 #endif
 #ifndef METH_METHOD
@@ -879,14 +955,19 @@
   #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
   #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
 #else
   #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
   #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
   #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
+#else
+  #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
+#endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
     PyTypeObject *type = Py_TYPE(obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
@@ -1005,17 +1086,33 @@
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
 #endif
 #if CYTHON_ASSUME_SAFE_MACROS
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_ITEM(o, i)
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) (PyTuple_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyList_SET_ITEM(o, i, v) (PyList_SET_ITEM(o, i, v), (0))
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_GET_SIZE(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_GET_SIZE(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_GET_SIZE(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_GET_SIZE(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_GET_SIZE(o)
 #else
+  #define __Pyx_PySequence_ITEM(o, i) PySequence_GetItem(o, i)
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
+  #define __Pyx_PyTuple_SET_ITEM(o, i, v) PyTuple_SetItem(o, i, v)
+  #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
+  #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
+  #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
+  #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
+  #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
+  #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
   #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
@@ -1171,17 +1268,18 @@
 #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define __Pyx_sst_abs(value) llabs(value)
 #elif defined (__GNUC__)
     #define __Pyx_sst_abs(value) __builtin_llabs(value)
 #else
     #define __Pyx_sst_abs(value) ((value<0) ? -value : value)
 #endif
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject*);
 static CYTHON_INLINE const char* __Pyx_PyObject_AsStringAndSize(PyObject*, Py_ssize_t* length);
-#define __Pyx_PyByteArray_FromString(s) PyByteArray_FromStringAndSize((const char*)s, strlen((const char*)s))
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char*);
 #define __Pyx_PyByteArray_FromStringAndSize(s, l) PyByteArray_FromStringAndSize((const char*)s, l)
 #define __Pyx_PyBytes_FromString        PyBytes_FromString
 #define __Pyx_PyBytes_FromStringAndSize PyBytes_FromStringAndSize
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char*);
 #if PY_MAJOR_VERSION < 3
     #define __Pyx_PyStr_FromString        __Pyx_PyBytes_FromString
     #define __Pyx_PyStr_FromStringAndSize __Pyx_PyBytes_FromStringAndSize
@@ -1289,14 +1387,15 @@
   #if PY_VERSION_HEX >= 0x030C00A5
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
   #else
   #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
   #endif
 #endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
+#include <string.h>
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
     const char* default_encoding_c;
@@ -1339,14 +1438,15 @@
 }
 #endif
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT && PY_MAJOR_VERSION >= 3
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_DecodeUTF8(c_str, size, NULL)
 #else
 #define __Pyx_PyUnicode_FromStringAndSize(c_str, size) PyUnicode_Decode(c_str, size, __PYX_DEFAULT_STRING_ENCODING, NULL)
 #if __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
+#include <string.h>
 static char* __PYX_DEFAULT_STRING_ENCODING;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     char* default_encoding_c;
     sys = PyImport_ImportModule("sys");
     if (!sys) goto bad;
@@ -1519,14 +1619,15 @@
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Using GNU atomics"
     #endif
 #elif CYTHON_ATOMICS && defined(_MSC_VER)
     #include <intrin.h>
     #undef __pyx_atomic_int_type
     #define __pyx_atomic_int_type long
+    #undef __pyx_nonatomic_int_type
     #define __pyx_nonatomic_int_type long
     #pragma intrinsic (_InterlockedExchangeAdd)
     #define __pyx_atomic_incr_aligned(value) _InterlockedExchangeAdd(value, 1)
     #define __pyx_atomic_decr_aligned(value) _InterlockedExchangeAdd(value, -1)
     #ifdef __PYX_DEBUG_ATOMICS
         #pragma message ("Using MSVC atomics")
     #endif
@@ -1558,177 +1659,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1787,42 +1888,42 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2109,33 +2210,50 @@
 /* BytesEquals.proto */
 static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* UnicodeEquals.proto */
 static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
 
 /* fastcall.proto */
-#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_VARARGS(args, i) PySequence_GetItem(args, i)
+#elif CYTHON_ASSUME_SAFE_MACROS
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#else
+    #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+    #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
+#else
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
+    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+#endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg) __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
 #else
 #define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
 #endif
 
@@ -2172,15 +2290,15 @@
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
 #if !CYTHON_VECTORCALL
 #if PY_VERSION_HEX >= 0x03080000
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
   #define __Pxy_PyFrame_Initialize_Offsets()
   #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
@@ -2357,28 +2475,42 @@
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
 /* AssertionsEnabled.proto */
-#define __Pyx_init_assertions_enabled()
 #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define __pyx_assertions_enabled() (1)
-#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
-  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
-#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  #define __Pyx_init_assertions_enabled()  (0)
+  #define __pyx_assertions_enabled()  (1)
+#elif CYTHON_COMPILING_IN_LIMITED_API  ||  (CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030C0000)
   static int __pyx_assertions_enabled_flag;
   #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
-  #undef __Pyx_init_assertions_enabled
-  static void __Pyx_init_assertions_enabled(void) {
-    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  static int __Pyx_init_assertions_enabled(void) {
+    PyObject *builtins, *debug, *debug_str;
+    int flag;
+    builtins = PyEval_GetBuiltins();
+    if (!builtins) goto bad;
+    debug_str = PyUnicode_FromStringAndSize("__debug__", 9);
+    if (!debug_str) goto bad;
+    debug = PyObject_GetItem(builtins, debug_str);
+    Py_DECREF(debug_str);
+    if (!debug) goto bad;
+    flag = PyObject_IsTrue(debug);
+    Py_DECREF(debug);
+    if (flag == -1) goto bad;
+    __pyx_assertions_enabled_flag = flag;
+    return 0;
+  bad:
+    __pyx_assertions_enabled_flag = 1;
+    return -1;
   }
 #else
-  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+  #define __Pyx_init_assertions_enabled()  (0)
+  #define __pyx_assertions_enabled()  (!Py_OptimizeFlag)
 #endif
 
 /* RaiseTooManyValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseTooManyValuesError(Py_ssize_t expected);
 
 /* RaiseNeedMoreValuesToUnpack.proto */
 static CYTHON_INLINE void __Pyx_RaiseNeedMoreValuesError(Py_ssize_t index);
@@ -2426,17 +2558,14 @@
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
 #if PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
 #endif
 
-/* ssize_strlen.proto */
-static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s);
-
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 #define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
@@ -2552,44 +2681,59 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
-#define __PYX_HAVE_RT_ImportType_proto_3_0_0
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_4
+#define __PYX_HAVE_RT_ImportType_proto_3_0_4
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_4(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_4(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_0 {
-   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
+enum __Pyx_ImportType_CheckSize_3_0_4 {
+   __Pyx_ImportType_CheckSize_Error_3_0_4 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_4 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_4 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_4(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_4 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 #else
 static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
 #endif
 
 /* PyMethodNew.proto */
-#if PY_MAJOR_VERSION >= 3
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    PyObject *typesModule=NULL, *methodType=NULL, *result=NULL;
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    typesModule = PyImport_ImportModule("types");
+    if (!typesModule) return NULL;
+    methodType = PyObject_GetAttrString(typesModule, "MethodType");
+    Py_DECREF(typesModule);
+    if (!methodType) return NULL;
+    result = PyObject_CallFunctionObjArgs(methodType, func, self, NULL);
+    Py_DECREF(methodType);
+    return result;
+}
+#elif PY_MAJOR_VERSION >= 3
 static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
     CYTHON_UNUSED_VAR(typ);
     if (!self)
         return __Pyx_NewRef(func);
     return PyMethod_New(func, self);
 }
 #else
@@ -2605,62 +2749,69 @@
 #define __Pyx_CyFunction_USED
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
 #define __Pyx_CYFUNCTION_CCLASS        0x04
 #define __Pyx_CYFUNCTION_COROUTINE     0x08
 #define __Pyx_CyFunction_GetClosure(f)\
     (((__pyx_CyFunctionObject *) (f))->func_closure)
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_CyFunction_GetClassObj(f)\
       (((__pyx_CyFunctionObject *) (f))->func_classobj)
 #else
   #define __Pyx_CyFunction_GetClassObj(f)\
       ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
 #endif
 #define __Pyx_CyFunction_SetClassObj(f, classobj)\
     __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
 #define __Pyx_CyFunction_Defaults(type, f)\
     ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
 #define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
     ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
 typedef struct {
-#if PY_VERSION_HEX < 0x030900B1
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject_HEAD
+    PyObject *func;
+#elif PY_VERSION_HEX < 0x030900B1
     PyCFunctionObject func;
 #else
     PyCMethodObject func;
 #endif
 #if CYTHON_BACKPORT_VECTORCALL
     __pyx_vectorcallfunc func_vectorcall;
 #endif
-#if PY_VERSION_HEX < 0x030500A0
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_weakreflist;
 #endif
     PyObject *func_dict;
     PyObject *func_name;
     PyObject *func_qualname;
     PyObject *func_doc;
     PyObject *func_globals;
     PyObject *func_code;
     PyObject *func_closure;
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
     size_t defaults_size;  // used by FusedFunction for copying defaults
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
+#undef __Pyx_CyOrPyCFunction_Check
 #define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyOrPyCFunction_Check(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
 #define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc);
+#undef __Pyx_IsSameCFunction
+#define __Pyx_IsSameCFunction(func, cfunc)   __Pyx__IsSameCyOrCFunction(func, cfunc)
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
 static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
@@ -2938,15 +3089,16 @@
 typedef const char *__Pyx_TypeName;
 #define __Pyx_FMT_TYPENAME "%.200s"
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
 /* CheckBinaryVersion.proto */
-static int __Pyx_check_binary_version(void);
+static unsigned long __Pyx_get_runtime_version(void);
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
@@ -4515,26 +4667,32 @@
 static int __pyx_array___cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_array___cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_shape = 0;
   Py_ssize_t __pyx_v_itemsize;
   PyObject *__pyx_v_format = 0;
   PyObject *__pyx_v_mode = 0;
   int __pyx_v_allocate_buffer;
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[5] = {0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_shape,&__pyx_n_s_itemsize,&__pyx_n_s_format,&__pyx_n_s_mode,&__pyx_n_s_allocate_buffer,0};
-    PyObject* values[5] = {0,0,0,0,0};
-    values[3] = ((PyObject *)__pyx_n_s_c);
+    values[3] = __Pyx_Arg_NewRef_VARARGS(((PyObject *)__pyx_n_s_c));
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  5: values[4] = __Pyx_Arg_VARARGS(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = __Pyx_Arg_VARARGS(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -4546,43 +4704,52 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shape)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_shape)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 131, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_itemsize)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_itemsize)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 131, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(1, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_format)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_format)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[2]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 131, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(1, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mode);
-          if (value) { values[3] = value; kw_args--; }
+          if (value) { values[3] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 131, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_allocate_buffer);
-          if (value) { values[4] = value; kw_args--; }
+          if (value) { values[4] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 131, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 131, __pyx_L3_error)
       }
@@ -4613,18 +4780,26 @@
  *                   mode="c", bint allocate_buffer=True):             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
       __pyx_v_allocate_buffer = ((int)1);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, __pyx_nargs); __PYX_ERR(1, 131, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("View.MemoryView.array.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(1, 131, __pyx_L1_error)
   if (unlikely(((PyObject *)__pyx_v_format) == Py_None)) {
     PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(1, 131, __pyx_L1_error)
@@ -4640,14 +4815,20 @@
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer) {
   int __pyx_v_idx;
   Py_ssize_t __pyx_v_dim;
@@ -4677,15 +4858,15 @@
  *         self.itemsize = itemsize
  * 
  */
   if (unlikely(__pyx_v_shape == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 137, __pyx_L1_error)
   }
-  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 137, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(1, 137, __pyx_L1_error)
   __pyx_v_self->ndim = ((int)__pyx_t_1);
 
   /* "View.MemoryView":138
  * 
  *         self.ndim = <int> len(shape)
  *         self.itemsize = itemsize             # <<<<<<<<<<<<<<
  * 
@@ -4769,24 +4950,26 @@
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format
  */
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 147, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
         __pyx_t_7 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_n_s_ASCII};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 147, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
@@ -4884,21 +5067,28 @@
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError, f"Invalid shape in axis {idx}: {dim}."
  */
   __pyx_t_7 = 0;
-  __pyx_t_4 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_4); __pyx_t_1 = 0;
+  __pyx_t_4 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = 0;
   for (;;) {
-    if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 159, __pyx_L1_error)
+      #endif
+      if (__pyx_t_1 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(1, 159, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 159, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(1, 159, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_9;
     __pyx_v_idx = __pyx_t_7;
     __pyx_t_7 = (__pyx_t_7 + 1);
@@ -5173,18 +5363,19 @@
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  */
 
 /* Python wrapper */
 CYTHON_UNUSED static int __pyx_array_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
 CYTHON_UNUSED static int __pyx_array_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(((struct __pyx_array_obj *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5406,15 +5597,16 @@
     /* "View.MemoryView":201
  *         else:
  *             info.ndim = 1
  *             info.shape = &self.len if flags & PyBUF_ND else NULL             # <<<<<<<<<<<<<<
  *             info.strides = NULL
  * 
  */
-    if (((__pyx_v_flags & PyBUF_ND) != 0)) {
+    __pyx_t_1 = ((__pyx_v_flags & PyBUF_ND) != 0);
+    if (__pyx_t_1) {
       __pyx_t_5 = (&__pyx_v_self->len);
     } else {
       __pyx_t_5 = NULL;
     }
     __pyx_v_info->shape = __pyx_t_5;
 
     /* "View.MemoryView":202
@@ -5459,15 +5651,16 @@
   /* "View.MemoryView":207
  *         info.itemsize = self.itemsize
  *         info.readonly = 0
  *         info.format = self.format if flags & PyBUF_FORMAT else NULL             # <<<<<<<<<<<<<<
  *         info.obj = self
  * 
  */
-  if (((__pyx_v_flags & PyBUF_FORMAT) != 0)) {
+  __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
+  if (__pyx_t_1) {
     __pyx_t_2 = __pyx_v_self->format;
   } else {
     __pyx_t_2 = NULL;
   }
   __pyx_v_info->format = __pyx_t_2;
 
   /* "View.MemoryView":208
@@ -5519,28 +5712,27 @@
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
 /* Python wrapper */
 static void __pyx_array___dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_array___dealloc__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":211
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data and self.data is not NULL:
@@ -5644,47 +5836,47 @@
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":219
  *         PyObject_Free(self._shape)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def memview(self):
  *         return self.get_memview()
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_5array_7memview_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_5array_7memview_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_5array_7memview___get__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":221
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
  *     @cname('get_memview')
@@ -5729,15 +5921,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_memview", 0);
+  __Pyx_RefNannySetupContext("get_memview", 1);
 
   /* "View.MemoryView":225
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
@@ -5756,19 +5948,19 @@
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF((PyObject *)__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_v_self);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self));
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self))) __PYX_ERR(1, 226, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1)) __PYX_ERR(1, 226, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2)) __PYX_ERR(1, 226, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 226, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
@@ -5802,29 +5994,28 @@
  *         return self._shape[0]
  * 
  */
 
 /* Python wrapper */
 static Py_ssize_t __pyx_array___len__(PyObject *__pyx_v_self); /*proto*/
 static Py_ssize_t __pyx_array___len__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__len__", 0);
 
   /* "View.MemoryView":229
  * 
  *     def __len__(self):
  *         return self._shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, attr):
@@ -5838,33 +6029,33 @@
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":231
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_array___getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_attr); /*proto*/
 static PyObject *__pyx_array___getattr__(PyObject *__pyx_v_self, PyObject *__pyx_v_attr) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getattr__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(((struct __pyx_array_obj *)__pyx_v_self), ((PyObject *)__pyx_v_attr));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5872,15 +6063,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getattr__", 0);
+  __Pyx_RefNannySetupContext("__getattr__", 1);
 
   /* "View.MemoryView":232
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
@@ -5922,18 +6113,19 @@
  *         return self.memview[item]
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_array___getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_item); /*proto*/
 static PyObject *__pyx_array___getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_item) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getitem__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(((struct __pyx_array_obj *)__pyx_v_self), ((PyObject *)__pyx_v_item));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -5941,15 +6133,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 1);
 
   /* "View.MemoryView":235
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, item, value):
@@ -5991,33 +6183,34 @@
  *         self.memview[item] = value
  * 
  */
 
 /* Python wrapper */
 static int __pyx_array___setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_item, PyObject *__pyx_v_value); /*proto*/
 static int __pyx_array___setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_item, PyObject *__pyx_v_value) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setitem__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array_12__setitem__(((struct __pyx_array_obj *)__pyx_v_self), ((PyObject *)__pyx_v_item), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_12__setitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setitem__", 0);
+  __Pyx_RefNannySetupContext("__setitem__", 1);
 
   /* "View.MemoryView":238
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
  * 
@@ -6065,20 +6258,28 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
   __pyx_r = __pyx_pf___pyx_array___reduce_cython__(((struct __pyx_array_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -6087,15 +6288,15 @@
 
 static PyObject *__pyx_pf___pyx_array___reduce_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -6137,74 +6338,99 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("View.MemoryView.array.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_array_2__setstate_cython__(((struct __pyx_array_obj *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_array_2__setstate_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -6234,23 +6460,21 @@
  * 
  */
 
 static int __pyx_array_allocate_buffer(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_v_i;
   PyObject **__pyx_v_p;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_allocate_buffer", 0);
 
   /* "View.MemoryView":254
  *     cdef PyObject **p
  * 
  *     self.free_data = True             # <<<<<<<<<<<<<<
  *     self.data = <char *>malloc(self.len)
  *     if not self.data:
@@ -6380,15 +6604,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView._allocate_buffer", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":268
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format, char *c_mode, char *buf):             # <<<<<<<<<<<<<<
@@ -6404,24 +6627,25 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("array_cwrapper", 0);
+  __Pyx_RefNannySetupContext("array_cwrapper", 1);
 
   /* "View.MemoryView":270
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format, char *c_mode, char *buf):
  *     cdef array result
  *     cdef str mode = "fortran" if c_mode[0] == b'f' else "c"  # this often comes from a constant C string.             # <<<<<<<<<<<<<<
  * 
  *     if buf is NULL:
  */
-  if (((__pyx_v_c_mode[0]) == 'f')) {
+  __pyx_t_2 = ((__pyx_v_c_mode[0]) == 'f');
+  if (__pyx_t_2) {
     __Pyx_INCREF(__pyx_n_s_fortran);
     __pyx_t_1 = __pyx_n_s_fortran;
   } else {
     __Pyx_INCREF(__pyx_n_s_c);
     __pyx_t_1 = __pyx_n_s_c;
   }
   __pyx_v_mode = ((PyObject*)__pyx_t_1);
@@ -6448,22 +6672,22 @@
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_shape);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_shape)) __PYX_ERR(1, 273, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1)) __PYX_ERR(1, 273, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3)) __PYX_ERR(1, 273, __pyx_L1_error);
     __Pyx_INCREF(__pyx_v_mode);
     __Pyx_GIVEREF(__pyx_v_mode);
-    PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_v_mode);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_v_mode)) __PYX_ERR(1, 273, __pyx_L1_error);
     __pyx_t_1 = 0;
     __pyx_t_3 = 0;
     __pyx_t_3 = ((PyObject *)__pyx_tp_new_array(((PyTypeObject *)__pyx_array_type), __pyx_t_4, NULL)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 273, __pyx_L1_error)
     __Pyx_GOTREF((PyObject *)__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
@@ -6490,22 +6714,22 @@
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = PyTuple_New(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_shape);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_shape)) __PYX_ERR(1, 275, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3)) __PYX_ERR(1, 275, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_t_4)) __PYX_ERR(1, 275, __pyx_L1_error);
     __Pyx_INCREF(__pyx_v_mode);
     __Pyx_GIVEREF(__pyx_v_mode);
-    PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_v_mode);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_v_mode)) __PYX_ERR(1, 275, __pyx_L1_error);
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 275, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(1, 275, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_tp_new_array(((PyTypeObject *)__pyx_array_type), __pyx_t_1, __pyx_t_4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 275, __pyx_L1_error)
     __Pyx_GOTREF((PyObject *)__pyx_t_3);
@@ -6568,70 +6792,93 @@
  *     def __repr__(self):
  */
 
 /* Python wrapper */
 static int __pyx_MemviewEnum___init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_MemviewEnum___init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_name)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 304, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 304, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_name = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 304, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("View.MemoryView.Enum.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self), __pyx_v_name);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__init__", 0);
+  __Pyx_RefNannySetupContext("__init__", 1);
 
   /* "View.MemoryView":305
  *     cdef object name
  *     def __init__(self, name):
  *         self.name = name             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return self.name
@@ -6663,29 +6910,30 @@
  *         return self.name
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_MemviewEnum___repr__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_MemviewEnum___repr__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum_2__repr__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum_2__repr__(struct __pyx_MemviewEnum_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__repr__", 0);
+  __Pyx_RefNannySetupContext("__repr__", 1);
 
   /* "View.MemoryView":307
  *         self.name = name
  *     def __repr__(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
@@ -6728,20 +6976,28 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
   __pyx_r = __pyx_pf___pyx_MemviewEnum___reduce_cython__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -6757,28 +7013,28 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.name,)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  */
   __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_self->name);
   __Pyx_GIVEREF(__pyx_v_self->name);
-  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_self->name);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_self->name)) __PYX_ERR(1, 5, __pyx_L1_error);
   __pyx_v_state = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "(tree fragment)":6
  *     cdef bint use_setstate
  *     state = (self.name,)
  *     _dict = getattr(self, '__dict__', None)             # <<<<<<<<<<<<<<
@@ -6807,15 +7063,15 @@
  *         use_setstate = True
  *     else:
  */
     __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 8, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_v__dict);
     __Pyx_GIVEREF(__pyx_v__dict);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v__dict)) __PYX_ERR(1, 8, __pyx_L1_error);
     __pyx_t_3 = PyNumber_InPlaceAdd(__pyx_v_state, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 8, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF_SET(__pyx_v_state, ((PyObject*)__pyx_t_3));
     __pyx_t_3 = 0;
 
     /* "(tree fragment)":9
@@ -6869,30 +7125,30 @@
     __Pyx_XDECREF(__pyx_r);
     __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pyx_unpickle_Enum); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))))) __PYX_ERR(1, 13, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_136983863);
     __Pyx_GIVEREF(__pyx_int_136983863);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_136983863);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_136983863)) __PYX_ERR(1, 13, __pyx_L1_error);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, Py_None)) __PYX_ERR(1, 13, __pyx_L1_error);
     __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(1, 13, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_state);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_state)) __PYX_ERR(1, 13, __pyx_L1_error);
     __pyx_t_3 = 0;
     __pyx_t_1 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
     /* "(tree fragment)":12
@@ -6915,27 +7171,27 @@
     __Pyx_XDECREF(__pyx_r);
     __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_Enum); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))))) __PYX_ERR(1, 15, __pyx_L1_error);
     __Pyx_INCREF(__pyx_int_136983863);
     __Pyx_GIVEREF(__pyx_int_136983863);
-    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_136983863);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_int_136983863)) __PYX_ERR(1, 15, __pyx_L1_error);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_state)) __PYX_ERR(1, 15, __pyx_L1_error);
     __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error);
     __pyx_t_4 = 0;
     __pyx_t_1 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
@@ -6980,75 +7236,100 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_state = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 16, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 16, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("View.MemoryView.Enum.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_MemviewEnum_2__setstate_cython__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_MemviewEnum_2__setstate_cython__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0x82a3537, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
   if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 17, __pyx_L1_error)
@@ -7086,25 +7367,31 @@
 
 /* Python wrapper */
 static int __pyx_memoryview___cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_memoryview___cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_obj = 0;
   int __pyx_v_flags;
   int __pyx_v_dtype_is_object;
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[3] = {0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return -1;
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_obj,&__pyx_n_s_flags,&__pyx_n_s_dtype_is_object,0};
-    PyObject* values[3] = {0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -7112,29 +7399,35 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_obj)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_obj)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flags)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flags)) != 0)) {
+          (void)__Pyx_Arg_NewRef_VARARGS(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(1, 349, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dtype_is_object);
-          if (value) { values[2] = value; kw_args--; }
+          if (value) { values[2] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
           else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 349, __pyx_L3_error)
       }
@@ -7152,25 +7445,39 @@
     __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
     if (values[2]) {
       __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 349, __pyx_L3_error)
     } else {
       __pyx_v_dtype_is_object = ((int)0);
     }
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, __pyx_nargs); __PYX_ERR(1, 349, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("View.MemoryView.memoryview.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview___cinit__(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_obj, __pyx_v_flags, __pyx_v_dtype_is_object);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static int __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview___cinit__(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_obj, int __pyx_v_flags, int __pyx_v_dtype_is_object) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -7178,15 +7485,15 @@
   int __pyx_t_2;
   int __pyx_t_3;
   Py_intptr_t __pyx_t_4;
   size_t __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__cinit__", 0);
+  __Pyx_RefNannySetupContext("__cinit__", 1);
 
   /* "View.MemoryView":350
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
@@ -7501,33 +7808,32 @@
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
 /* Python wrapper */
 static void __pyx_memoryview___dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_memoryview___dealloc__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_2__dealloc__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_2__dealloc__(struct __pyx_memoryview_obj *__pyx_v_self) {
   int __pyx_v_i;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   PyThread_type_lock __pyx_t_5;
   PyThread_type_lock __pyx_t_6;
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":377
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
@@ -7717,15 +8023,14 @@
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":397
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
@@ -7744,15 +8049,15 @@
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_item_pointer", 0);
+  __Pyx_RefNannySetupContext("get_item_pointer", 1);
 
   /* "View.MemoryView":399
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
@@ -7764,37 +8069,50 @@
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
-    __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
     __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 401, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(1, 401, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 401, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -7869,18 +8187,19 @@
  *         if index is Ellipsis:
  *             return self
  */
 
 /* Python wrapper */
 static PyObject *__pyx_memoryview___getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_index); /*proto*/
 static PyObject *__pyx_memoryview___getitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_index) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getitem__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_4__getitem__(((struct __pyx_memoryview_obj *)__pyx_v_self), ((PyObject *)__pyx_v_index));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -7894,15 +8213,15 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   char *__pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__getitem__", 0);
+  __Pyx_RefNannySetupContext("__getitem__", 1);
 
   /* "View.MemoryView":408
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
@@ -8057,18 +8376,19 @@
  *         if self.view.readonly:
  *             raise TypeError, "Cannot assign to read-only memoryview"
  */
 
 /* Python wrapper */
 static int __pyx_memoryview___setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_value); /*proto*/
 static int __pyx_memoryview___setitem__(PyObject *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_value) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setitem__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_6__setitem__(((struct __pyx_memoryview_obj *)__pyx_v_self), ((PyObject *)__pyx_v_index), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -8355,19 +8675,19 @@
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
         __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 438, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_v_obj);
         __Pyx_GIVEREF(__pyx_v_obj);
-        PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj)) __PYX_ERR(1, 438, __pyx_L4_error);
         __Pyx_GIVEREF(__pyx_t_6);
-        PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6)) __PYX_ERR(1, 438, __pyx_L4_error);
         __Pyx_GIVEREF(__pyx_t_7);
-        PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
+        if (__Pyx_PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7)) __PYX_ERR(1, 438, __pyx_L4_error);
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
         __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 438, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_7);
         __pyx_t_7 = 0;
@@ -8504,15 +8824,15 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
+  __Pyx_RefNannySetupContext("setitem_slice_assignment", 1);
 
   /* "View.MemoryView":448
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  *         cdef __Pyx_memviewslice msrc = get_slice_from_memview(src, &src_slice)[0]             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mdst = get_slice_from_memview(dst, &dst_slice)[0]
  * 
@@ -8597,15 +8917,15 @@
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
+  __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 1);
 
   /* "View.MemoryView":455
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
@@ -8870,15 +9190,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("setitem_indexed", 0);
+  __Pyx_RefNannySetupContext("setitem_indexed", 1);
 
   /* "View.MemoryView":486
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
@@ -8941,15 +9261,15 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("convert_item_to_object", 0);
+  __Pyx_RefNannySetupContext("convert_item_to_object", 1);
 
   /* "View.MemoryView":492
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
@@ -8996,24 +9316,26 @@
  */
       __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 497, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
-      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      #if CYTHON_UNPACK_METHODS
+      if (likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_7);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_8 = 1;
         }
       }
+      #endif
       {
         PyObject *__pyx_callargs[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
         __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_8, 2+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
         if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 497, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
@@ -9189,15 +9511,15 @@
   char *__pyx_t_9;
   char *__pyx_t_10;
   char *__pyx_t_11;
   char *__pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assign_item_from_object", 0);
+  __Pyx_RefNannySetupContext("assign_item_from_object", 1);
 
   /* "View.MemoryView":508
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
@@ -9227,15 +9549,15 @@
     __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(1, 514, __pyx_L1_error);
     __pyx_t_3 = 0;
     __pyx_t_3 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = PyNumber_Add(__pyx_t_4, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 514, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -9267,24 +9589,26 @@
   /*else*/ {
     __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 516, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 516, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     __pyx_t_6 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
         __pyx_t_6 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_t_1, __pyx_v_value};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_6, 2+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 516, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
@@ -9379,18 +9703,19 @@
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  */
 
 /* Python wrapper */
 CYTHON_UNUSED static int __pyx_memoryview_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
 CYTHON_UNUSED static int __pyx_memoryview_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__getbuffer__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_8__getbuffer__(((struct __pyx_memoryview_obj *)__pyx_v_self), ((Py_buffer *)__pyx_v_info), ((int)__pyx_v_flags));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -9718,18 +10043,19 @@
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_1T_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_1T_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_1T___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -9738,15 +10064,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":556
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
@@ -9805,33 +10131,34 @@
  *     def base(self):
  *         return self._get_base()
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_4base_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_4base_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":562
  *     @property
  *     def base(self):
  *         return self._get_base()             # <<<<<<<<<<<<<<
  * 
  *     cdef _get_base(self):
@@ -9869,15 +10196,15 @@
  *         return self.obj
  * 
  */
 
 static PyObject *__pyx_memoryview__get_base(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_get_base", 0);
+  __Pyx_RefNannySetupContext("_get_base", 1);
 
   /* "View.MemoryView":565
  * 
  *     cdef _get_base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -9909,18 +10236,19 @@
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_5shape_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_5shape_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_5shape___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -9932,15 +10260,15 @@
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":569
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -9993,18 +10321,19 @@
  *     def strides(self):
  *         if self.view.strides == NULL:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_7strides_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_7strides_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_7strides___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10017,15 +10346,15 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":573
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError, "Buffer view does not expose strides"
@@ -10107,18 +10436,19 @@
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_10suboffsets_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_10suboffsets_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_10suboffsets___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10131,15 +10461,15 @@
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":581
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
@@ -10225,33 +10555,34 @@
  *     def ndim(self):
  *         return self.view.ndim
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_4ndim_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_4ndim_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":588
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10289,33 +10620,34 @@
  *     def itemsize(self):
  *         return self.view.itemsize
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_8itemsize_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_8itemsize_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":592
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10353,18 +10685,19 @@
  *     def nbytes(self):
  *         return self.size * self.view.itemsize
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_6nbytes_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_6nbytes_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_6nbytes___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10373,15 +10706,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":596
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
@@ -10427,18 +10760,19 @@
  *     def size(self):
  *         if self._size is None:
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_4size_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_15View_dot_MemoryView_10memoryview_4size_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_pf_15View_dot_MemoryView_10memoryview_4size___get__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10451,15 +10785,15 @@
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_RefNannySetupContext("__get__", 1);
 
   /* "View.MemoryView":600
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
@@ -10567,30 +10901,29 @@
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
 /* Python wrapper */
 static Py_ssize_t __pyx_memoryview___len__(PyObject *__pyx_v_self); /*proto*/
 static Py_ssize_t __pyx_memoryview___len__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("__len__", 0);
 
   /* "View.MemoryView":611
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
@@ -10633,33 +10966,33 @@
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":616
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
 /* Python wrapper */
 static PyObject *__pyx_memoryview___repr__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_memoryview___repr__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_12__repr__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10668,15 +11001,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__repr__", 0);
+  __Pyx_RefNannySetupContext("__repr__", 1);
 
   /* "View.MemoryView":617
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
@@ -10707,17 +11040,17 @@
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
   __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 617, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(1, 617, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(1, 617, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 617, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
@@ -10751,18 +11084,19 @@
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_memoryview___str__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_memoryview___str__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__str__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_14__str__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10770,15 +11104,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__str__", 0);
+  __Pyx_RefNannySetupContext("__str__", 1);
 
   /* "View.MemoryView":621
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
@@ -10791,15 +11125,15 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 621, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 621, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(1, 621, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 621, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
@@ -10844,20 +11178,28 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_c_contig (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("is_c_contig", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "is_c_contig", 0))) return NULL;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_16is_c_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -10870,15 +11212,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_c_contig", 0);
+  __Pyx_RefNannySetupContext("is_c_contig", 1);
 
   /* "View.MemoryView":627
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
@@ -10939,20 +11281,28 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_f_contig (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("is_f_contig", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "is_f_contig", 0))) return NULL;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_18is_f_contig(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -10965,15 +11315,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("is_f_contig", 0);
+  __Pyx_RefNannySetupContext("is_f_contig", 1);
 
   /* "View.MemoryView":633
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
@@ -11034,20 +11384,28 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy", 0))) return NULL;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_20copy(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -11060,15 +11418,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("copy", 0);
+  __Pyx_RefNannySetupContext("copy", 1);
 
   /* "View.MemoryView":638
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
@@ -11147,20 +11505,28 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("copy_fortran (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("copy_fortran", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "copy_fortran", 0))) return NULL;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_22copy_fortran(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -11174,15 +11540,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("copy_fortran", 0);
+  __Pyx_RefNannySetupContext("copy_fortran", 1);
 
   /* "View.MemoryView":650
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
@@ -11259,20 +11625,28 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
   __pyx_r = __pyx_pf___pyx_memoryview___reduce_cython__(((struct __pyx_memoryview_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -11281,15 +11655,15 @@
 
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -11331,74 +11705,99 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("View.MemoryView.memoryview.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_memoryview_2__setstate_cython__(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -11434,15 +11833,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
+  __Pyx_RefNannySetupContext("memoryview_cwrapper", 1);
 
   /* "View.MemoryView":663
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
@@ -11451,19 +11850,19 @@
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_o);
   __Pyx_GIVEREF(__pyx_v_o);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o)) __PYX_ERR(1, 663, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1)) __PYX_ERR(1, 663, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2)) __PYX_ERR(1, 663, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 663, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryview_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
@@ -11517,17 +11916,15 @@
  * cdef inline bint memoryview_check(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("memoryview_check", 0);
 
   /* "View.MemoryView":669
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o) noexcept:
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
@@ -11542,15 +11939,14 @@
  * cdef inline bint memoryview_check(object o) noexcept:             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":671
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
@@ -11574,15 +11970,15 @@
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_UCS4 __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_unellipsify", 0);
+  __Pyx_RefNannySetupContext("_unellipsify", 1);
 
   /* "View.MemoryView":677
  *     """
  *     cdef Py_ssize_t idx
  *     tup = <tuple>index if isinstance(index, tuple) else (index,)             # <<<<<<<<<<<<<<
  * 
  *     result = [slice(None)] * ndim
@@ -11592,15 +11988,15 @@
     __Pyx_INCREF(((PyObject*)__pyx_v_index));
     __pyx_t_1 = __pyx_v_index;
   } else {
     __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 677, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_index);
     __Pyx_GIVEREF(__pyx_v_index);
-    PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index)) __PYX_ERR(1, 677, __pyx_L1_error);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   }
   __pyx_v_tup = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":679
@@ -11612,15 +12008,15 @@
  */
   __pyx_t_1 = PyList_New(1 * ((__pyx_v_ndim<0) ? 0:__pyx_v_ndim)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 679, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   { Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < __pyx_v_ndim; __pyx_temp++) {
       __Pyx_INCREF(__pyx_slice__5);
       __Pyx_GIVEREF(__pyx_slice__5);
-      PyList_SET_ITEM(__pyx_t_1, __pyx_temp, __pyx_slice__5);
+      if (__Pyx_PyList_SET_ITEM(__pyx_t_1, __pyx_temp, __pyx_slice__5)) __PYX_ERR(1, 679, __pyx_L1_error);
     }
   }
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":680
  * 
@@ -11656,21 +12052,28 @@
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   if (unlikely(__pyx_v_tup == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
     __PYX_ERR(1, 683, __pyx_L1_error)
   }
-  __pyx_t_1 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_1); __pyx_t_4 = 0;
+  __pyx_t_1 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_1);
+  __pyx_t_4 = 0;
   for (;;) {
-    if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+    {
+      Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
+      #if !CYTHON_ASSUME_SAFE_MACROS
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 683, __pyx_L1_error)
+      #endif
+      if (__pyx_t_4 >= __pyx_temp) break;
+    }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(1, 683, __pyx_L1_error)
     #else
-    __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 683, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 683, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_3);
     __pyx_t_3 = 0;
 
     /* "View.MemoryView":684
  *     idx = 0
@@ -11699,15 +12102,15 @@
  *                 seen_ellipsis = True
  *             have_slices = True
  */
         if (unlikely(__pyx_v_tup == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
           __PYX_ERR(1, 686, __pyx_L1_error)
         }
-        __pyx_t_5 = PyTuple_GET_SIZE(__pyx_v_tup); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 686, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyTuple_GET_SIZE(__pyx_v_tup); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 686, __pyx_L1_error)
         __pyx_v_idx = (__pyx_v_idx + (__pyx_v_ndim - __pyx_t_5));
 
         /* "View.MemoryView":687
  *             if not seen_ellipsis:
  *                 idx += ndim - len(tup)
  *                 seen_ellipsis = True             # <<<<<<<<<<<<<<
  *             have_slices = True
@@ -11887,17 +12290,17 @@
   __pyx_t_7 = 0;
   __pyx_L9_bool_binop_done:;
   __pyx_t_7 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(1, 698, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_7)) __PYX_ERR(1, 698, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_7 = 0;
   __pyx_r = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* "View.MemoryView":671
@@ -11931,23 +12334,21 @@
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
 static int assert_direct_dimensions(Py_ssize_t *__pyx_v_suboffsets, int __pyx_v_ndim) {
   Py_ssize_t __pyx_v_suboffset;
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
   /* "View.MemoryView":701
  * 
  * cdef int assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim) except -1:
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError, "Indirect dimensions not supported"
@@ -12006,15 +12407,14 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView.assert_direct_dimensions", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "View.MemoryView":711
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
@@ -12052,15 +12452,15 @@
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
   int __pyx_t_10;
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memview_slice", 0);
+  __Pyx_RefNannySetupContext("memview_slice", 1);
 
   /* "View.MemoryView":712
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
@@ -12202,37 +12602,50 @@
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             cindex = index
  */
   __pyx_t_5 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
-    __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2); __pyx_t_6 = 0;
+    __pyx_t_2 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
     __pyx_t_6 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 747, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 747, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_8 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         #endif
       } else {
-        if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
+          #endif
+          if (__pyx_t_6 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_8 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_6); __Pyx_INCREF(__pyx_t_8); __pyx_t_6++; if (unlikely((0 < 0))) __PYX_ERR(1, 747, __pyx_L1_error)
         #else
-        __pyx_t_8 = PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 747, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         #endif
       }
     } else {
       __pyx_t_8 = __pyx_t_7(__pyx_t_2);
       if (unlikely(!__pyx_t_8)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -13393,15 +13806,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   Py_UCS4 __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("pybuffer_index", 0);
+  __Pyx_RefNannySetupContext("pybuffer_index", 1);
 
   /* "View.MemoryView":898
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
@@ -13891,26 +14304,25 @@
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
 /* Python wrapper */
 static void __pyx_memoryviewslice___dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_memoryviewslice___dealloc__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
+  __pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__dealloc__", 0);
 
   /* "View.MemoryView":964
  * 
  *     def __dealloc__(self):
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
@@ -13922,15 +14334,14 @@
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":966
  *         __PYX_XCLEAR_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
@@ -13941,15 +14352,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("convert_item_to_object", 0);
+  __Pyx_RefNannySetupContext("convert_item_to_object", 1);
 
   /* "View.MemoryView":967
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
@@ -14028,15 +14439,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("assign_item_from_object", 0);
+  __Pyx_RefNannySetupContext("assign_item_from_object", 1);
 
   /* "View.MemoryView":973
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
@@ -14105,15 +14516,15 @@
  *         return self.from_object
  * 
  */
 
 static PyObject *__pyx_memoryviewslice__get_base(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("_get_base", 0);
+  __Pyx_RefNannySetupContext("_get_base", 1);
 
   /* "View.MemoryView":979
  * 
  *     cdef _get_base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  * 
@@ -14156,20 +14567,28 @@
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   if (unlikely(__pyx_nargs > 0)) {
     __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
   if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
   __pyx_r = __pyx_pf___pyx_memoryviewslice___reduce_cython__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
@@ -14178,15 +14597,15 @@
 
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 1);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
@@ -14228,74 +14647,99 @@
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[1] = {0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
-    PyObject* values[1] = {0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
         if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v___pyx_state = values[0];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf___pyx_memoryviewslice_2__setstate_cython__(((struct __pyx_memoryviewslice_obj *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 1);
 
   /* "(tree fragment)":4
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
   __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
@@ -14339,15 +14783,15 @@
   Py_ssize_t *__pyx_t_6;
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
+  __Pyx_RefNannySetupContext("memoryview_fromslice", 1);
 
   /* "View.MemoryView":1007
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
@@ -14384,20 +14828,20 @@
  */
   __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
-  PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None)) __PYX_ERR(1, 1013, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
-  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0)) __PYX_ERR(1, 1013, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_2 = ((PyObject *)__pyx_tp_new__memoryviewslice(((PyTypeObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1013, __pyx_L1_error)
   __Pyx_GOTREF((PyObject *)__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
@@ -14716,15 +15160,15 @@
   __Pyx_memviewslice *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
+  __Pyx_RefNannySetupContext("get_slice_from_memview", 1);
 
   /* "View.MemoryView":1055
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
@@ -14813,21 +15257,20 @@
  */
 
 static void __pyx_memoryview_slice_copy(struct __pyx_memoryview_obj *__pyx_v_memview, __Pyx_memviewslice *__pyx_v_dst) {
   int __pyx_v_dim;
   Py_ssize_t *__pyx_v_shape;
   Py_ssize_t *__pyx_v_strides;
   Py_ssize_t *__pyx_v_suboffsets;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
-  __Pyx_RefNannySetupContext("slice_copy", 0);
+  int __pyx_t_6;
 
   /* "View.MemoryView":1067
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
@@ -14906,15 +15349,16 @@
     /* "View.MemoryView":1077
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object')
  */
-    if ((__pyx_v_suboffsets != 0)) {
+    __pyx_t_6 = (__pyx_v_suboffsets != 0);
+    if (__pyx_t_6) {
       __pyx_t_5 = (__pyx_v_suboffsets[__pyx_v_dim]);
     } else {
       __pyx_t_5 = -1L;
     }
     (__pyx_v_dst->suboffsets[__pyx_v_dim]) = __pyx_t_5;
   }
 
@@ -14923,15 +15367,14 @@
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst) noexcept:             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":1080
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
@@ -14942,15 +15385,15 @@
   __Pyx_memviewslice __pyx_v_memviewslice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_copy", 0);
+  __Pyx_RefNannySetupContext("memoryview_copy", 1);
 
   /* "View.MemoryView":1083
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
@@ -15006,15 +15449,15 @@
   int __pyx_t_1;
   PyObject *(*__pyx_t_2)(char *);
   int (*__pyx_t_3)(char *, PyObject *);
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
+  __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 1);
 
   /* "View.MemoryView":1094
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
@@ -15121,23 +15564,25 @@
  *     return -arg if arg < 0 else arg
  * 
  */
 
 static Py_ssize_t abs_py_ssize_t(Py_ssize_t __pyx_v_arg) {
   Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
+  int __pyx_t_2;
 
   /* "View.MemoryView":1110
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) noexcept nogil:
  *     return -arg if arg < 0 else arg             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_get_best_slice_order')
  */
-  if ((__pyx_v_arg < 0)) {
+  __pyx_t_2 = (__pyx_v_arg < 0);
+  if (__pyx_t_2) {
     __pyx_t_1 = (-__pyx_v_arg);
   } else {
     __pyx_t_1 = __pyx_v_arg;
   }
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
@@ -16271,22 +16716,20 @@
  * cdef int _err_no_memory() except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise MemoryError
  * 
  */
 
 static int __pyx_memoryview_err_no_memory(void) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("_err_no_memory", 0);
 
   /* "View.MemoryView":1261
  * @cname('__pyx_memoryview_err_no_memory')
  * cdef int _err_no_memory() except -1 with gil:
  *     raise MemoryError             # <<<<<<<<<<<<<<
  * 
  * 
@@ -16301,15 +16744,14 @@
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_AddTraceback("View.MemoryView._err_no_memory", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
-  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
 /* "View.MemoryView":1265
@@ -16453,15 +16895,16 @@
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_3 = __pyx_v_dst_ndim;
   __pyx_t_4 = __pyx_v_src_ndim;
-  if ((__pyx_t_3 > __pyx_t_4)) {
+  __pyx_t_2 = (__pyx_t_3 > __pyx_t_4);
+  if (__pyx_t_2) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_ndim = __pyx_t_5;
 
   /* "View.MemoryView":1288
@@ -17055,19 +17498,17 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
-  __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
-  __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
   /* "View.MemoryView":1368
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
@@ -17079,15 +17520,14 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) noexcept with gil:
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
 /* "View.MemoryView":1371
  * 
@@ -17096,20 +17536,18 @@
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   CYTHON_UNUSED Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_stride;
-  __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
-  __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
   /* "View.MemoryView":1374
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(shape[0]):
@@ -17215,15 +17653,14 @@
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc) noexcept:
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
-  __Pyx_RefNannyFinishContext();
 }
 
 /* "View.MemoryView":1391
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
@@ -17423,26 +17860,34 @@
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[3] = {0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
-    PyObject* values[3] = {0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -17450,27 +17895,36 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_type)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_type)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_checksum)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Enum", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Enum", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
@@ -17483,25 +17937,39 @@
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
     __pyx_v___pyx_type = values[0];
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_Enum", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 1, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("View.MemoryView.__pyx_unpickle_Enum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
@@ -17511,15 +17979,15 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 1);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0x82a3537, 0x6ae9995, 0xb068931):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
@@ -17537,15 +18005,15 @@
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  *     __pyx_result = Enum.__new__(__pyx_type)
  */
     __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError)) __PYX_ERR(1, 5, __pyx_L1_error);
     __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_t_1);
     __pyx_v___pyx_PickleError = __pyx_t_1;
@@ -17584,24 +18052,26 @@
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  */
   __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   __pyx_t_5 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
+  #if CYTHON_UNPACK_METHODS
+  if (likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_5 = 1;
     }
   }
+  #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v___pyx_type};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -17691,15 +18161,15 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 0);
+  __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 1);
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  *     __pyx_result.name = __pyx_state[0]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[1])
@@ -17722,15 +18192,15 @@
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
  *         __pyx_result.__dict__.update(__pyx_state[1])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 13, __pyx_L1_error)
   }
-  __pyx_t_3 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
   __pyx_t_4 = (__pyx_t_3 > 1);
   if (__pyx_t_4) {
   } else {
     __pyx_t_2 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_4 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
@@ -17752,24 +18222,26 @@
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(1, 14, __pyx_L1_error)
     }
     __pyx_t_5 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_7 = NULL;
     __pyx_t_8 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+    #if CYTHON_UNPACK_METHODS
+    if (likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
         __Pyx_INCREF(__pyx_t_7);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_8 = 1;
       }
     }
+    #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_t_5};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
@@ -17805,292 +18277,292 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
-  __Pyx_RefNannySetupContext("descr", 0);
+  __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18101,46 +18573,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18151,46 +18623,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18201,46 +18673,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18251,46 +18723,46 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18301,220 +18773,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
+  __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18528,17 +18997,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
+  __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18546,68 +19015,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18615,15 +19084,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18638,15 +19107,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18660,17 +19129,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
+  __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18678,68 +19147,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18747,15 +19216,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18770,15 +19239,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18792,17 +19261,17 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
+  __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18810,68 +19279,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18879,15 +19348,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18902,176 +19371,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19086,16 +19549,14 @@
  *         cdef inline double real(self):             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("real", 0);
 
   /* "cpython/complex.pxd":20
  *         @property
  *         cdef inline double real(self):
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
@@ -19109,30 +19570,27 @@
  *         cdef inline double real(self):             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
  *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("imag", 0);
 
   /* "cpython/complex.pxd":24
  *         @property
  *         cdef inline double imag(self):
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
@@ -19146,15 +19604,14 @@
  *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/contextvars.pxd":112
  * 
  * 
  * cdef inline object get_value(var, default_value=None):             # <<<<<<<<<<<<<<
@@ -19170,15 +19627,15 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_value", 0);
+  __Pyx_RefNannySetupContext("get_value", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default_value = __pyx_optional_args->default_value;
     }
   }
 
   /* "cpython/contextvars.pxd":117
@@ -19300,15 +19757,15 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("get_value_no_default", 0);
+  __Pyx_RefNannySetupContext("get_value_no_default", 1);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_default_value = __pyx_optional_args->default_value;
     }
   }
 
   /* "cpython/contextvars.pxd":135
@@ -19404,26 +19861,34 @@
 #endif
 ) {
   PyObject *__pyx_v_cursor = 0;
   double __pyx_v_mzmin;
   double __pyx_v_mzmax;
   size_t __pyx_v_n_bins;
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[4] = {0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_sample_peaks (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cursor,&__pyx_n_s_mzmin,&__pyx_n_s_mzmax,&__pyx_n_s_n_bins,0};
-    PyObject* values[4] = {0,0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -19433,34 +19898,46 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cursor)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cursor)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mzmin)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mzmin)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_peaks", 1, 4, 4, 1); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mzmax)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mzmax)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_peaks", 1, 4, 4, 2); __PYX_ERR(0, 29, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_bins)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_n_bins)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 29, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_peaks", 1, 4, 4, 3); __PYX_ERR(0, 29, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
@@ -19475,25 +19952,39 @@
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
     __pyx_v_cursor = values[0];
     __pyx_v_mzmin = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_mzmin == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 32, __pyx_L3_error)
     __pyx_v_mzmax = __pyx_PyFloat_AsDouble(values[2]); if (unlikely((__pyx_v_mzmax == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 32, __pyx_L3_error)
     __pyx_v_n_bins = __Pyx_PyInt_As_size_t(values[3]); if (unlikely((__pyx_v_n_bins == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 32, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_sample_peaks", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 29, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_AddTraceback("emzed_gui.optimized.optimized._sample_peaks", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9emzed_gui_9optimized_9optimized__sample_peaks(__pyx_self, __pyx_v_cursor, __pyx_v_mzmin, __pyx_v_mzmax, __pyx_v_n_bins);
 
   /* function exit code */
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9emzed_gui_9optimized_9optimized__sample_peaks(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_cursor, double __pyx_v_mzmin, double __pyx_v_mzmax, size_t __pyx_v_n_bins) {
   __Pyx_memviewslice __pyx_v_peaks = { 0, 0, { 0 }, { 0 }, { 0 } };
   double *__pyx_v_mzp;
@@ -19529,15 +20020,15 @@
   PyObject *__pyx_t_15 = NULL;
   __Pyx_memviewslice __pyx_t_16 = { 0, 0, { 0 }, { 0 }, { 0 } };
   size_t __pyx_t_17;
   Py_ssize_t __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_sample_peaks", 0);
+  __Pyx_RefNannySetupContext("_sample_peaks", 1);
 
   /* "emzed_gui/optimized/optimized.pyx":48
  *     cdef int mz_bin
  * 
  *     cdef double * i_sums = <double * > calloc(sizeof(double), n_bins)             # <<<<<<<<<<<<<<
  *     if i_sums == NULL:
  *         return None
@@ -19683,37 +20174,50 @@
  *         return None
  * 
  *     for spec in cursor:             # <<<<<<<<<<<<<<
  * 
  *         assert PyObject_GetBuffer(spec[0], &mz_buffer, 0) == 0, "get buffer failed"
  */
   if (likely(PyList_CheckExact(__pyx_v_cursor)) || PyTuple_CheckExact(__pyx_v_cursor)) {
-    __pyx_t_2 = __pyx_v_cursor; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_2 = __pyx_v_cursor; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
     __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_cursor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 61, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 61, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 61, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 61, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 61, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 61, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -19912,15 +20416,16 @@
  *             mz_i_sums[mz_bin] += mz * ii
  *             i_max[mz_bin] = max(i_max[mz_bin], ii)             # <<<<<<<<<<<<<<
  * 
  *         PyBuffer_Release(&mz_buffer)
  */
       __pyx_t_10 = __pyx_v_ii;
       __pyx_t_11 = (__pyx_v_i_max[__pyx_v_mz_bin]);
-      if ((__pyx_t_10 > __pyx_t_11)) {
+      __pyx_t_1 = (__pyx_t_10 > __pyx_t_11);
+      if (__pyx_t_1) {
         __pyx_t_12 = __pyx_t_10;
       } else {
         __pyx_t_12 = __pyx_t_11;
       }
       (__pyx_v_i_max[__pyx_v_mz_bin]) = __pyx_t_12;
       __pyx_L8_continue:;
     }
@@ -19967,23 +20472,23 @@
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_FromSize_t(__pyx_v_n_bins); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_13 = PyTuple_New(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_2);
-  PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
-  PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_int_2);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_int_2)) __PYX_ERR(0, 86, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_13);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_13);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_13)) __PYX_ERR(0, 86, __pyx_L1_error);
   __pyx_t_13 = 0;
   __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_float64); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
@@ -20130,18 +20635,18 @@
   __Pyx_GOTREF(__pyx_t_15);
   __pyx_t_13 = PySlice_New(Py_None, __pyx_t_15, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = PyTuple_New(2); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_13);
-  PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_13);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_13)) __PYX_ERR(0, 101, __pyx_L1_error);
   __Pyx_INCREF(__pyx_slice__5);
   __Pyx_GIVEREF(__pyx_slice__5);
-  PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_slice__5);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_slice__5)) __PYX_ERR(0, 101, __pyx_L1_error);
   __pyx_t_13 = 0;
   __pyx_t_13 = __Pyx_PyObject_GetItem(__pyx_v_result, __pyx_t_15); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_r = __pyx_t_13;
   __pyx_t_13 = 0;
   goto __pyx_L0;
@@ -20203,26 +20708,34 @@
   double __pyx_v_mzmin;
   double __pyx_v_mzmax;
   CYTHON_UNUSED int __pyx_v_ms_level;
   size_t __pyx_v_width;
   size_t __pyx_v_height;
   __Pyx_memviewslice __pyx_v_img_view = { 0, 0, { 0 }, { 0 }, { 0 } };
   #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
+  PyObject* values[9] = {0,0,0,0,0,0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_sample_image (wrapper)", 0);
+  #if !CYTHON_METH_FASTCALL
+  #if CYTHON_ASSUME_SAFE_MACROS
+  __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #else
+  __pyx_nargs = PyTuple_Size(__pyx_args); if (unlikely(__pyx_nargs < 0)) return NULL;
+  #endif
+  #endif
+  __pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   {
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_cursor,&__pyx_n_s_rtmin,&__pyx_n_s_rtmax,&__pyx_n_s_mzmin,&__pyx_n_s_mzmax,&__pyx_n_s_ms_level,&__pyx_n_s_width,&__pyx_n_s_height,&__pyx_n_s_img_view,0};
-    PyObject* values[9] = {0,0,0,0,0,0,0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
         case  9: values[8] = __Pyx_Arg_FASTCALL(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = __Pyx_Arg_FASTCALL(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
@@ -20242,69 +20755,96 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cursor)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_cursor)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_rtmin)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_rtmin)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, 1); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_rtmax)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_rtmax)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, 2); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mzmin)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mzmin)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, 3); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
-        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mzmax)) != 0)) kw_args--;
+        if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mzmax)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, 4); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
-        if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ms_level)) != 0)) kw_args--;
+        if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ms_level)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, 5); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
-        if (likely((values[6] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_width)) != 0)) kw_args--;
+        if (likely((values[6] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_width)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[6]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, 6); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
-        if (likely((values[7] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_height)) != 0)) kw_args--;
+        if (likely((values[7] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_height)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[7]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, 7); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
-        if (likely((values[8] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_img_view)) != 0)) kw_args--;
+        if (likely((values[8] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_img_view)) != 0)) {
+          (void)__Pyx_Arg_NewRef_FASTCALL(values[8]);
+          kw_args--;
+        }
         else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
           __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, 8); __PYX_ERR(0, 105, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
@@ -20329,27 +20869,41 @@
     __pyx_v_mzmin = __pyx_PyFloat_AsDouble(values[3]); if (unlikely((__pyx_v_mzmin == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L3_error)
     __pyx_v_mzmax = __pyx_PyFloat_AsDouble(values[4]); if (unlikely((__pyx_v_mzmax == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L3_error)
     __pyx_v_ms_level = __Pyx_PyInt_As_int(values[5]); if (unlikely((__pyx_v_ms_level == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L3_error)
     __pyx_v_width = __Pyx_PyInt_As_size_t(values[6]); if (unlikely((__pyx_v_width == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L3_error)
     __pyx_v_height = __Pyx_PyInt_As_size_t(values[7]); if (unlikely((__pyx_v_height == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L3_error)
     __pyx_v_img_view = __Pyx_PyObject_to_MemoryviewSlice_dsds_nn___pyx_t_5numpy_float32_t(values[8], PyBUF_WRITABLE); if (unlikely(!__pyx_v_img_view.memview)) __PYX_ERR(0, 110, __pyx_L3_error)
   }
-  goto __pyx_L4_argument_unpacking_done;
+  goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("_sample_image", 1, 9, 9, __pyx_nargs); __PYX_ERR(0, 105, __pyx_L3_error)
+  __pyx_L6_skip:;
+  goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_img_view, 1);
   __Pyx_AddTraceback("emzed_gui.optimized.optimized._sample_image", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_9emzed_gui_9optimized_9optimized_2_sample_image(__pyx_self, __pyx_v_cursor, __pyx_v_rtmin, __pyx_v_rtmax, __pyx_v_mzmin, __pyx_v_mzmax, __pyx_v_ms_level, __pyx_v_width, __pyx_v_height, __pyx_v_img_view);
 
   /* function exit code */
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_img_view, 1);
+  {
+    Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
+      __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
+    }
+  }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_9emzed_gui_9optimized_9optimized_2_sample_image(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_cursor, double __pyx_v_rtmin, double __pyx_v_rtmax, double __pyx_v_mzmin, double __pyx_v_mzmax, CYTHON_UNUSED int __pyx_v_ms_level, size_t __pyx_v_width, size_t __pyx_v_height, __Pyx_memviewslice __pyx_v_img_view) {
   size_t __pyx_v_rt_bin;
   size_t __pyx_v_mz_bin;
@@ -20375,15 +20929,15 @@
   size_t __pyx_t_9;
   size_t __pyx_t_10;
   size_t __pyx_t_11;
   size_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("_sample_image", 0);
+  __Pyx_RefNannySetupContext("_sample_image", 1);
 
   /* "emzed_gui/optimized/optimized.pyx":113
  * 
  *     # avoid zero division later
  *     assert mzmax > mzmin             # <<<<<<<<<<<<<<
  *     assert rtmax > rtmin
  * 
@@ -20423,37 +20977,50 @@
  *     cdef Py_buffer mz_buffer, ii_buffer
  * 
  *     for spec in cursor:             # <<<<<<<<<<<<<<
  * 
  *         rt = spec[0]
  */
   if (likely(PyList_CheckExact(__pyx_v_cursor)) || PyTuple_CheckExact(__pyx_v_cursor)) {
-    __pyx_t_2 = __pyx_v_cursor; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
+    __pyx_t_2 = __pyx_v_cursor; __Pyx_INCREF(__pyx_t_2);
+    __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
     __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_cursor); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
-        if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 121, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 121, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
-        if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
+        {
+          Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
+          #if !CYTHON_ASSUME_SAFE_MACROS
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 121, __pyx_L1_error)
+          #endif
+          if (__pyx_t_3 >= __pyx_temp) break;
+        }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely((0 < 0))) __PYX_ERR(0, 121, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 121, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
@@ -20752,15 +21319,22 @@
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
     __pyx_array___dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->mode);
   Py_CLEAR(p->_format);
+  #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
   (*Py_TYPE(o)->tp_free)(o);
+  #else
+  {
+    freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+    if (tp_free) tp_free(o);
+  }
+  #endif
 }
 static PyObject *__pyx_sq_item_array(PyObject *o, Py_ssize_t i) {
   PyObject *r;
   PyObject *x = PyInt_FromSsize_t(i); if(!x) return 0;
   r = Py_TYPE(o)->tp_as_mapping->mp_subscript(o, x);
   Py_DECREF(x);
   return r;
@@ -20993,15 +21567,22 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_Enum) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
+  #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
   (*Py_TYPE(o)->tp_free)(o);
+  #else
+  {
+    freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+    if (tp_free) tp_free(o);
+  }
+  #endif
 }
 
 static int __pyx_tp_traverse_Enum(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   if (p->name) {
     e = (*v)(p->name, a); if (e) return e;
@@ -21175,15 +21756,22 @@
     __pyx_memoryview___dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->obj);
   Py_CLEAR(p->_size);
   Py_CLEAR(p->_array_interface);
+  #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
   (*Py_TYPE(o)->tp_free)(o);
+  #else
+  {
+    freefunc tp_free = (freefunc)PyType_GetSlot(Py_TYPE(o), Py_tp_free);
+    if (tp_free) tp_free(o);
+  }
+  #endif
 }
 
 static int __pyx_tp_traverse_memoryview(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   if (p->obj) {
     e = (*v)(p->obj, a); if (e) return e;
@@ -21845,15 +22433,15 @@
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
   __pyx_tuple__4 = PyTuple_New(1); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 582, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__4, 0, __pyx_int_neg_1);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_tuple__4, 0, __pyx_int_neg_1)) __PYX_ERR(1, 582, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
   /* "View.MemoryView":679
  *     tup = <tuple>index if isinstance(index, tuple) else (index,)
  * 
  *     result = [slice(None)] * ndim             # <<<<<<<<<<<<<<
  *     have_slices = False
@@ -21870,26 +22458,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../../tmp/build-env-69ggvoht/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../../tmp/build-env-mqpdpvo5/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 989, __pyx_L1_error)
@@ -22042,27 +22630,27 @@
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   /* AssertionsEnabled.init */
-  __Pyx_init_assertions_enabled();
+  if (likely(__Pyx_init_assertions_enabled() == 0)); else
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* NumpyImportArray.init */
   /*
  * Cython has automatically inserted a call to _import_array since
  * you didn't include one when you cimported numpy. To disable this
  * add the line
  *   <void>numpy._import_array
  */
 #ifdef NPY_FEATURE_VERSION
-#if !NO_IMPORT_ARRAY
+#ifndef NO_IMPORT_ARRAY
 if (unlikely(_import_array() == -1)) {
     PyErr_SetString(PyExc_ImportError, "numpy.core.multiarray failed to import "
     "(auto-generated because you didn't call 'numpy.import_array()' after cimporting numpy; "
     "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
 }
 #endif
 #endif
@@ -22275,49 +22863,49 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_4(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(4, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_4(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(5, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_4(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(6, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 865, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_4); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_4); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_4); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_4); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_4); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_4(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_4(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_4); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 865, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -22556,15 +23144,15 @@
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
   __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_optimized(void)", 0);
-  if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_check_binary_version(__PYX_LIMITED_VERSION_HEX, __Pyx_get_runtime_version(), CYTHON_COMPILING_IN_LIMITED_API) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
@@ -22798,28 +23386,28 @@
  *     try:
  *         count = __pyx_collections_abc_Sequence.count             # <<<<<<<<<<<<<<
  *         index = __pyx_collections_abc_Sequence.index
  *     except:
  */
       __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_collections_abc_Sequence, __pyx_n_s_count); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 242, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_array_type->tp_dict, __pyx_n_s_count, __pyx_t_7) < 0) __PYX_ERR(1, 242, __pyx_L11_error)
+      if (__Pyx_SetItemOnTypeDict(__pyx_array_type, __pyx_n_s_count, __pyx_t_7) < 0) __PYX_ERR(1, 242, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       PyType_Modified(__pyx_array_type);
 
       /* "View.MemoryView":243
  *     try:
  *         count = __pyx_collections_abc_Sequence.count
  *         index = __pyx_collections_abc_Sequence.index             # <<<<<<<<<<<<<<
  *     except:
  *         pass
  */
       __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_collections_abc_Sequence, __pyx_n_s_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 243, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_array_type->tp_dict, __pyx_n_s_index, __pyx_t_7) < 0) __PYX_ERR(1, 243, __pyx_L11_error)
+      if (__Pyx_SetItemOnTypeDict(__pyx_array_type, __pyx_n_s_index, __pyx_t_7) < 0) __PYX_ERR(1, 243, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       PyType_Modified(__pyx_array_type);
 
       /* "View.MemoryView":241
  * 
  * 
  *     try:             # <<<<<<<<<<<<<<
@@ -22972,28 +23560,28 @@
  *     try:
  *         count = __pyx_collections_abc_Sequence.count             # <<<<<<<<<<<<<<
  *         index = __pyx_collections_abc_Sequence.index
  *     except:
  */
       __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_collections_abc_Sequence, __pyx_n_s_count); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 983, __pyx_L17_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_count, __pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L17_error)
+      if (__Pyx_SetItemOnTypeDict(__pyx_memoryviewslice_type, __pyx_n_s_count, __pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L17_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       PyType_Modified(__pyx_memoryviewslice_type);
 
       /* "View.MemoryView":984
  *     try:
  *         count = __pyx_collections_abc_Sequence.count
  *         index = __pyx_collections_abc_Sequence.index             # <<<<<<<<<<<<<<
  *     except:
  *         pass
  */
       __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_collections_abc_Sequence, __pyx_n_s_index); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 984, __pyx_L17_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_index, __pyx_t_7) < 0) __PYX_ERR(1, 984, __pyx_L17_error)
+      if (__Pyx_SetItemOnTypeDict(__pyx_memoryviewslice_type, __pyx_n_s_index, __pyx_t_7) < 0) __PYX_ERR(1, 984, __pyx_L17_error)
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       PyType_Modified(__pyx_memoryviewslice_type);
 
       /* "View.MemoryView":982
  * 
  * 
  *     try:             # <<<<<<<<<<<<<<
@@ -23320,14 +23908,16 @@
         if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
         #endif
             PyException_SetTraceback(value, tb);
     }
     tmp_value = tstate->current_exception;
     tstate->current_exception = value;
     Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
 #else
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     tmp_type = tstate->curexc_type;
     tmp_value = tstate->curexc_value;
     tmp_tb = tstate->curexc_traceback;
     tstate->curexc_type = type;
     tstate->curexc_value = value;
@@ -23675,37 +24265,70 @@
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
     int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
     while (1) {
+        Py_XDECREF(key); key = NULL;
+        Py_XDECREF(value); value = NULL;
         if (kwds_is_tuple) {
-            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            Py_ssize_t size;
+#if CYTHON_ASSUME_SAFE_MACROS
+            size = PyTuple_GET_SIZE(kwds);
+#else
+            size = PyTuple_Size(kwds);
+            if (size < 0) goto bad;
+#endif
+            if (pos >= size) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            key = __Pyx_PySequence_ITEM(kwds, pos);
+            if (!key) goto bad;
+#elif CYTHON_ASSUME_SAFE_MACROS
             key = PyTuple_GET_ITEM(kwds, pos);
+#else
+            key = PyTuple_GetItem(kwds, pos);
+            if (!key) goto bad;
+#endif
             value = kwvalues[pos];
             pos++;
         }
         else
         {
             if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(key);
+#endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_INCREF(value); // transfer ownership of value to values
+            Py_DECREF(key);
+#endif
+            key = NULL;
+            value = NULL;
             continue;
         }
+#if !CYTHON_AVOID_BORROWED_REFS
+        Py_INCREF(key);
+#endif
+        Py_INCREF(value);
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL;  // ownership transferred to values
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -23727,14 +24350,17 @@
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
+#if CYTHON_AVOID_BORROWED_REFS
+                    value = NULL; // ownership transferred to values
+#endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
@@ -23753,14 +24379,16 @@
             goto invalid_keyword_type;
         if (kwds2) {
             if (unlikely(PyDict_SetItem(kwds2, key, value))) goto bad;
         } else {
             goto invalid_keyword;
         }
     }
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return 0;
 arg_passed_twice:
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
@@ -23772,14 +24400,16 @@
         function_name, PyString_AsString(key));
     #else
     PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
+    Py_XDECREF(key);
+    Py_XDECREF(value);
     return -1;
 }
 
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
     __Pyx_TypeName type_name;
@@ -24105,66 +24735,57 @@
 #endif
 
 /* PyObjectCallMethO */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
     PyObject *self, *result;
     PyCFunction cfunc;
-    cfunc = PyCFunction_GET_FUNCTION(func);
-    self = PyCFunction_GET_SELF(func);
+    cfunc = __Pyx_CyOrPyCFunction_GET_FUNCTION(func);
+    self = __Pyx_CyOrPyCFunction_GET_SELF(func);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = cfunc(self, arg);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
         PyErr_SetString(
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
 /* PyObjectFastCall */
+#if PY_VERSION_HEX < 0x03090000 || CYTHON_COMPILING_IN_LIMITED_API
 static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
     PyObject *argstuple;
-    PyObject *result;
+    PyObject *result = 0;
     size_t i;
     argstuple = PyTuple_New((Py_ssize_t)nargs);
     if (unlikely(!argstuple)) return NULL;
     for (i = 0; i < nargs; i++) {
         Py_INCREF(args[i]);
-        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+        if (__Pyx_PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]) < 0) goto bad;
     }
     result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+  bad:
     Py_DECREF(argstuple);
     return result;
 }
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
     Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
 #if CYTHON_COMPILING_IN_CPYTHON
     if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_NOARGS))
+            return __Pyx_PyObject_CallMethO(func, NULL);
     }
     else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+        if (__Pyx_CyOrPyCFunction_Check(func) && likely( __Pyx_CyOrPyCFunction_GET_FLAGS(func) & METH_O))
+            return __Pyx_PyObject_CallMethO(func, args[0]);
     }
 #endif
     #if PY_VERSION_HEX < 0x030800B1
     #if CYTHON_FAST_PYCCALL
     if (PyCFunction_Check(func)) {
         if (kwargs) {
             return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
@@ -24180,29 +24801,39 @@
     #endif
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
     }
     #endif
     #endif
-    #if CYTHON_VECTORCALL
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    if (kwargs == NULL) {
+        #if CYTHON_VECTORCALL
+        #if Py_VERSION_HEX < 0x03090000
+        vectorcallfunc f = _PyVectorcall_Function(func);
+        #else
+        vectorcallfunc f = PyVectorcall_Function(func);
+        #endif
+        if (f) {
+            return f(func, args, (size_t)nargs, NULL);
+        }
+        #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+        if (__Pyx_CyFunction_CheckExact(func)) {
+            __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+            if (f) return f(func, args, (size_t)nargs, NULL);
+        }
+        #endif
     }
-    #endif
     if (nargs == 0) {
         return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
     }
+    #if PY_VERSION_HEX >= 0x03090000 && !CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_VectorcallDict(func, args, (size_t)nargs, kwargs);
+    #else
     return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
+    #endif
 }
 
 /* RaiseUnexpectedTypeError */
 static int
 __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
 {
     __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
@@ -24497,15 +25128,17 @@
         if (unlikely((PY_SSIZE_T_MAX >> kind_shift) - ulength < char_pos))
             goto overflow;
         ukind = __Pyx_PyUnicode_KIND(uval);
         udata = __Pyx_PyUnicode_DATA(uval);
         if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
             memcpy((char *)result_udata + (char_pos << kind_shift), udata, (size_t) (ulength << kind_shift));
         } else {
-            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            #if PY_VERSION_HEX >= 0x030D0000
+            if (unlikely(PyUnicode_CopyCharacters(result_uval, char_pos, uval, 0, ulength) < 0)) goto bad;
+            #elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
             _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
             #else
             Py_ssize_t j;
             for (j=0; j < ulength; j++) {
                 Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
                 __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
             }
@@ -24699,23 +25332,40 @@
     Py_ssize_t pos = 0;
 #if CYTHON_COMPILING_IN_PYPY
     if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
         goto invalid_keyword;
     return 1;
 #else
     if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
-        if (unlikely(PyTuple_GET_SIZE(kw) == 0))
+        Py_ssize_t kwsize;
+#if CYTHON_ASSUME_SAFE_MACROS
+        kwsize = PyTuple_GET_SIZE(kw);
+#else
+        kwsize = PyTuple_Size(kw);
+        if (kwsize < 0) return 0;
+#endif
+        if (unlikely(kwsize == 0))
             return 1;
         if (!kw_allowed) {
+#if CYTHON_ASSUME_SAFE_MACROS
             key = PyTuple_GET_ITEM(kw, 0);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
             goto invalid_keyword;
         }
 #if PY_VERSION_HEX < 0x03090000
-        for (pos = 0; pos < PyTuple_GET_SIZE(kw); pos++) {
+        for (pos = 0; pos < kwsize; pos++) {
+#if CYTHON_ASSUME_SAFE_MACROS
             key = PyTuple_GET_ITEM(kw, pos);
+#else
+            key = PyTuple_GetItem(kw, pos);
+            if (!key) return 0;
+#endif
             if (unlikely(!PyUnicode_Check(key)))
                 goto invalid_keyword_type;
         }
 #endif
         return 1;
     }
     while (PyDict_Next(kw, &pos, &key, 0)) {
@@ -25136,22 +25786,17 @@
     #endif
     empty_dict = PyDict_New();
     if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                #if CYTHON_COMPILING_IN_LIMITED_API
-                module = PyImport_ImportModuleLevelObject(
-                    name, empty_dict, empty_dict, from_list, 1);
-                #else
+            if (strchr(__Pyx_MODULE_NAME, '.') != NULL) {
                 module = PyImport_ImportModuleLevelObject(
                     name, __pyx_d, empty_dict, from_list, 1);
-                #endif
                 if (unlikely(!module)) {
                     if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
@@ -25162,22 +25807,17 @@
             PyObject *py_level = PyInt_FromLong(level);
             if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
                 name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
-            #if CYTHON_COMPILING_IN_LIMITED_API
-            module = PyImport_ImportModuleLevelObject(
-                name, empty_dict, empty_dict, from_list, level);
-            #else
             module = PyImport_ImportModuleLevelObject(
                 name, __pyx_d, empty_dict, from_list, level);
             #endif
-            #endif
         }
     }
 bad:
     Py_XDECREF(empty_dict);
     Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
@@ -25309,24 +25949,14 @@
     } else if (PyErr_Occurred()) {
         PyErr_Clear();
     }
 #endif
     return __Pyx__ImportDottedModule(name, parts_tuple);
 }
 
-/* ssize_strlen */
-static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
-    size_t len = strlen(s);
-    if (unlikely(len > PY_SSIZE_T_MAX)) {
-        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
-        return -1;
-    }
-    return (Py_ssize_t) len;
-}
-
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
         a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
@@ -25715,16 +26345,16 @@
 #endif
     return 0;
 }
 #endif
 
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg = NULL;
-    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+    PyObject *arg[2] = {NULL, NULL};
+    return __Pyx_PyObject_FastCall(func, arg + 1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectGetMethod */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
     PyObject *attr;
 #if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
     __Pyx_TypeName type_name;
@@ -25839,48 +26469,91 @@
 bad:
     return result;
 }
 
 /* ValidateBasesTuple */
 #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
 static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
-    Py_ssize_t i, n = PyTuple_GET_SIZE(bases);
+    Py_ssize_t i, n;
+#if CYTHON_ASSUME_SAFE_MACROS
+    n = PyTuple_GET_SIZE(bases);
+#else
+    n = PyTuple_Size(bases);
+    if (n < 0) return -1;
+#endif
     for (i = 1; i < n; i++)
     {
+#if CYTHON_AVOID_BORROWED_REFS
+        PyObject *b0 = PySequence_GetItem(bases, i);
+        if (!b0) return -1;
+#elif CYTHON_ASSUME_SAFE_MACROS
         PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+#else
+        PyObject *b0 = PyTuple_GetItem(bases, i);
+        if (!b0) return -1;
+#endif
         PyTypeObject *b;
 #if PY_MAJOR_VERSION < 3
         if (PyClass_Check(b0))
         {
             PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
                          PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
             return -1;
         }
 #endif
         b = (PyTypeObject*) b0;
         if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
         {
             __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
             PyErr_Format(PyExc_TypeError,
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
+            return -1;
+        }
+#if !CYTHON_USE_TYPE_SLOTS
+        if (dictoffset == 0) {
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%s.200s': "
+                "unable to validate whether bases have a __dict__ "
+                "when CYTHON_USE_TYPE_SLOTS is off "
+                "(likely because you are building in the limited API). "
+                "Therefore, all extension types with multiple bases "
+                "must add 'cdef dict __dict__' in this compilation mode",
+                type_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
             return -1;
         }
+#else
         if (dictoffset == 0 && b->tp_dictoffset)
         {
             __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
             PyErr_Format(PyExc_TypeError,
                 "extension type '%.200s' has no __dict__ slot, "
                 "but base type '" __Pyx_FMT_TYPENAME "' has: "
                 "either add 'cdef dict __dict__' to the extension type "
                 "or add '__slots__ = [...]' to the base type",
                 type_name, b_name);
             __Pyx_DECREF_TypeName(b_name);
+#if CYTHON_AVOID_BORROWED_REFS
+            Py_DECREF(b0);
+#endif
             return -1;
         }
+#endif
+#if CYTHON_AVOID_BORROWED_REFS
+        Py_DECREF(b0);
+#endif
     }
     return 0;
 }
 #endif
 
 /* PyType_Ready */
 static int __Pyx_PyType_Ready(PyTypeObject *t) {
@@ -26163,18 +26836,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_3_0_0
-#define __PYX_HAVE_RT_ImportType_3_0_0
-static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_3_0_4
+#define __PYX_HAVE_RT_ImportType_3_0_4
+static PyTypeObject *__Pyx_ImportType_3_0_4(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_4 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -26220,23 +26893,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_4 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_4 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -26408,42 +27081,61 @@
         return vc(func, args, nargs, NULL);
     }
     return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
 }
 #endif
 
 /* CythonFunctionShared */
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    if (__Pyx_CyFunction_Check(func)) {
+        return PyCFunction_GetFunction(((__pyx_CyFunctionObject*)func)->func) == (PyCFunction) cfunc;
+    } else if (PyCFunction_Check(func)) {
+        return PyCFunction_GetFunction(func) == (PyCFunction) cfunc;
+    }
+    return 0;
+}
+#else
+static CYTHON_INLINE int __Pyx__IsSameCyOrCFunction(PyObject *func, void *cfunc) {
+    return __Pyx_CyOrPyCFunction_Check(func) && __Pyx_CyOrPyCFunction_GET_FUNCTION(func) == (PyCFunction) cfunc;
+}
+#endif
 static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     __Pyx_Py_XDECREF_SET(
         __Pyx_CyFunction_GetClassObj(f),
             ((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #else
     __Pyx_Py_XDECREF_SET(
         ((PyCMethodObject *) (f))->mm_class,
         (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
 #endif
 }
 static PyObject *
 __Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
 {
     CYTHON_UNUSED_VAR(closure);
     if (unlikely(op->func_doc == NULL)) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_doc = PyObject_GetAttrString(op->func, "__doc__");
+        if (unlikely(!op->func_doc)) return NULL;
+#else
         if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
 #if PY_MAJOR_VERSION >= 3
             op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
 #else
             op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
 #endif
             if (unlikely(op->func_doc == NULL))
                 return NULL;
         } else {
             Py_INCREF(Py_None);
             return Py_None;
         }
+#endif
     }
     Py_INCREF(op->func_doc);
     return op->func_doc;
 }
 static int
 __Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
 {
@@ -26456,15 +27148,17 @@
     return 0;
 }
 static PyObject *
 __Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
 {
     CYTHON_UNUSED_VAR(context);
     if (unlikely(op->func_name == NULL)) {
-#if PY_MAJOR_VERSION >= 3
+#if CYTHON_COMPILING_IN_LIMITED_API
+        op->func_name = PyObject_GetAttrString(op->func, "__name__");
+#elif PY_MAJOR_VERSION >= 3
         op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
 #else
         op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
 #endif
         if (unlikely(op->func_name == NULL))
             return NULL;
     }
@@ -26575,18 +27269,18 @@
         return -1;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
     Py_INCREF(op->defaults_tuple);
     op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
     Py_INCREF(op->defaults_kwdict);
     #else
-    op->defaults_tuple = PySequence_ITEM(res, 0);
+    op->defaults_tuple = __Pyx_PySequence_ITEM(res, 0);
     if (unlikely(!op->defaults_tuple)) result = -1;
     else {
-        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        op->defaults_kwdict = __Pyx_PySequence_ITEM(res, 1);
         if (unlikely(!op->defaults_kwdict)) result = -1;
     }
     #endif
     Py_DECREF(res);
     return result;
 }
 static int
@@ -26687,15 +27381,23 @@
     is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
 #if PY_VERSION_HEX >= 0x03050000
     if (is_coroutine) {
         PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
         fromlist = PyList_New(1);
         if (unlikely(!fromlist)) return NULL;
         Py_INCREF(marker);
+#if CYTHON_ASSUME_SAFE_MACROS
         PyList_SET_ITEM(fromlist, 0, marker);
+#else
+        if (unlikely(PyList_SetItem(fromlist, 0, marker) < 0)) {
+            Py_DECREF(marker);
+            Py_DECREF(fromlist);
+            return NULL;
+        }
+#endif
         module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
         Py_DECREF(fromlist);
         if (unlikely(!module)) goto ignore;
         op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
         Py_DECREF(module);
         if (likely(op->func_is_coroutine)) {
             return __Pyx_NewRef(op->func_is_coroutine);
@@ -26703,14 +27405,26 @@
 ignore:
         PyErr_Clear();
     }
 #endif
     op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
     return __Pyx_NewRef(op->func_is_coroutine);
 }
+#if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *
+__Pyx_CyFunction_get_module(__pyx_CyFunctionObject *op, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_GetAttrString(op->func, "__module__");
+}
+static int
+__Pyx_CyFunction_set_module(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    return PyObject_SetAttrString(op->func, "__module__", value);
+}
+#endif
 static PyGetSetDef __pyx_CyFunction_getsets[] = {
     {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
     {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
     {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
     {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
     {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
     {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
@@ -26722,28 +27436,35 @@
     {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
     {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
     {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
     {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
     {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
     {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
     {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+#if CYTHON_COMPILING_IN_LIMITED_API
+    {"__module__", (getter)__Pyx_CyFunction_get_module, (setter)__Pyx_CyFunction_set_module, 0, 0},
+#endif
     {0, 0, 0, 0, 0}
 };
 static PyMemberDef __pyx_CyFunction_members[] = {
+#if !CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#endif
 #if CYTHON_USE_TYPE_SPECS
     {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
 #if CYTHON_METH_FASTCALL
 #if CYTHON_BACKPORT_VECTORCALL
     {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
 #else
+#if !CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
 #endif
 #endif
-#if PY_VERSION_HEX < 0x030500A0
+#endif
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
     {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
 #else
     {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
 #endif
 #endif
     {0, 0, 0,  0, 0}
 };
@@ -26758,38 +27479,48 @@
     return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
 #endif
 }
 static PyMethodDef __pyx_CyFunction_methods[] = {
     {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
     {0, 0, 0, 0}
 };
-#if PY_VERSION_HEX < 0x030500A0
+#if PY_VERSION_HEX < 0x030500A0 || CYTHON_COMPILING_IN_LIMITED_API
 #define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
 #else
 #define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
 #endif
 static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
                                        PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+#if !CYTHON_COMPILING_IN_LIMITED_API
     PyCFunctionObject *cf = (PyCFunctionObject*) op;
+#endif
     if (unlikely(op == NULL))
         return NULL;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    op->func = PyCFunction_NewEx(ml, (PyObject*)op, module);
+    if (unlikely(!op->func)) return NULL;
+#endif
     op->flags = flags;
     __Pyx_CyFunction_weakreflist(op) = NULL;
+#if !CYTHON_COMPILING_IN_LIMITED_API
     cf->m_ml = ml;
     cf->m_self = (PyObject *) op;
+#endif
     Py_XINCREF(closure);
     op->func_closure = closure;
+#if !CYTHON_COMPILING_IN_LIMITED_API
     Py_XINCREF(module);
     cf->m_module = module;
+#endif
     op->func_dict = NULL;
     op->func_name = NULL;
     Py_INCREF(qualname);
     op->func_qualname = qualname;
     op->func_doc = NULL;
-#if PY_VERSION_HEX < 0x030900B1
+#if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     op->func_classobj = NULL;
 #else
     ((PyCMethodObject*)op)->mm_class = NULL;
 #endif
     op->func_globals = globals;
     Py_INCREF(op->func_globals);
     Py_XINCREF(code);
@@ -26827,30 +27558,36 @@
 #endif
     return (PyObject *) op;
 }
 static int
 __Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
 {
     Py_CLEAR(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_CLEAR(m->func);
+#else
     Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+#endif
     Py_CLEAR(m->func_dict);
     Py_CLEAR(m->func_name);
     Py_CLEAR(m->func_qualname);
     Py_CLEAR(m->func_doc);
     Py_CLEAR(m->func_globals);
     Py_CLEAR(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
 #if PY_VERSION_HEX < 0x030900B1
     Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
 #else
     {
         PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
         ((PyCMethodObject *) (m))->mm_class = NULL;
         Py_XDECREF(cls);
     }
 #endif
+#endif
     Py_CLEAR(m->defaults_tuple);
     Py_CLEAR(m->defaults_kwdict);
     Py_CLEAR(m->func_annotations);
     Py_CLEAR(m->func_is_coroutine);
     if (m->defaults) {
         PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
         int i;
@@ -26872,22 +27609,28 @@
 {
     PyObject_GC_UnTrack(m);
     __Pyx__CyFunction_dealloc(m);
 }
 static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
 {
     Py_VISIT(m->func_closure);
+#if CYTHON_COMPILING_IN_LIMITED_API
+    Py_VISIT(m->func);
+#else
     Py_VISIT(((PyCFunctionObject*)m)->m_module);
+#endif
     Py_VISIT(m->func_dict);
     Py_VISIT(m->func_name);
     Py_VISIT(m->func_qualname);
     Py_VISIT(m->func_doc);
     Py_VISIT(m->func_globals);
     Py_VISIT(m->func_code);
+#if !CYTHON_COMPILING_IN_LIMITED_API
     Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+#endif
     Py_VISIT(m->defaults_tuple);
     Py_VISIT(m->defaults_kwdict);
     Py_VISIT(m->func_is_coroutine);
     if (m->defaults) {
         PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
         int i;
         for (i = 0; i < m->defaults_pyobjects; i++)
@@ -26903,67 +27646,123 @@
                                 op->func_qualname, (void *)op);
 #else
     return PyString_FromFormat("<cyfunction %s at %p>",
                                PyString_AsString(op->func_qualname), (void *)op);
 #endif
 }
 static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+    PyObject *f = ((__pyx_CyFunctionObject*)func)->func;
+    PyObject *py_name = NULL;
+    PyCFunction meth;
+    int flags;
+    meth = PyCFunction_GetFunction(f);
+    if (unlikely(!meth)) return NULL;
+    flags = PyCFunction_GetFlags(f);
+    if (unlikely(flags < 0)) return NULL;
+#else
     PyCFunctionObject* f = (PyCFunctionObject*)func;
     PyCFunction meth = f->m_ml->ml_meth;
+    int flags = f->m_ml->ml_flags;
+#endif
     Py_ssize_t size;
-    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    switch (flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
     case METH_VARARGS:
         if (likely(kw == NULL || PyDict_Size(kw) == 0))
             return (*meth)(self, arg);
         break;
     case METH_VARARGS | METH_KEYWORDS:
         return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
     case METH_NOARGS:
         if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
             size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
             if (likely(size == 0))
                 return (*meth)(self, NULL);
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
             PyErr_Format(PyExc_TypeError,
                 "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
                 f->m_ml->ml_name, size);
+#endif
             return NULL;
         }
         break;
     case METH_O:
         if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+#if CYTHON_ASSUME_SAFE_MACROS
             size = PyTuple_GET_SIZE(arg);
+#else
+            size = PyTuple_Size(arg);
+            if (unlikely(size < 0)) return NULL;
+#endif
             if (likely(size == 1)) {
                 PyObject *result, *arg0;
                 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
                 arg0 = PyTuple_GET_ITEM(arg, 0);
                 #else
-                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                arg0 = __Pyx_PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
                 #endif
                 result = (*meth)(self, arg0);
                 #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
                 Py_DECREF(arg0);
                 #endif
                 return result;
             }
+#if CYTHON_COMPILING_IN_LIMITED_API
+            py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+            if (!py_name) return NULL;
+            PyErr_Format(PyExc_TypeError,
+                "%.200S() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                py_name, size);
+            Py_DECREF(py_name);
+#else
             PyErr_Format(PyExc_TypeError,
                 "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
                 f->m_ml->ml_name, size);
+#endif
             return NULL;
         }
         break;
     default:
         PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
         return NULL;
     }
+#if CYTHON_COMPILING_IN_LIMITED_API
+    py_name = __Pyx_CyFunction_get_name((__pyx_CyFunctionObject*)func, NULL);
+    if (!py_name) return NULL;
+    PyErr_Format(PyExc_TypeError, "%.200S() takes no keyword arguments",
+                 py_name);
+    Py_DECREF(py_name);
+#else
     PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
                  f->m_ml->ml_name);
+#endif
     return NULL;
 }
 static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+    PyObject *self, *result;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    self = PyCFunction_GetSelf(((__pyx_CyFunctionObject*)func)->func);
+    if (unlikely(!self) && PyErr_Occurred()) return NULL;
+#else
+    self = ((PyCFunctionObject*)func)->m_self;
+#endif
+    result = __Pyx_CyFunction_CallMethod(func, self, arg, kw);
+    return result;
 }
 static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
     PyObject *result;
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
 #if CYTHON_METH_FASTCALL
      __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
     if (vc) {
@@ -26975,15 +27774,20 @@
 #endif
     }
 #endif
     if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
         Py_ssize_t argc;
         PyObject *new_args;
         PyObject *self;
+#if CYTHON_ASSUME_SAFE_MACROS
         argc = PyTuple_GET_SIZE(args);
+#else
+        argc = PyTuple_Size(args);
+        if (unlikely(!argc) < 0) return NULL;
+#endif
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
 #if PY_MAJOR_VERSION > 2
@@ -27188,15 +27992,15 @@
     0,
     0,
     0,
     0,
 #ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
     Py_TPFLAGS_METHOD_DESCRIPTOR |
 #endif
-#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+#if defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL
     _Py_TPFLAGS_HAVE_VECTORCALL |
 #endif
     Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
     0,
     (traverseproc) __Pyx_CyFunction_traverse,
     (inquiry) __Pyx_CyFunction_clear,
     0,
@@ -27420,28 +28224,99 @@
 }
 #endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
+#if PY_VERSION_HEX >= 0x030b00a6 && !CYTHON_COMPILING_IN_LIMITED_API
   #ifndef Py_BUILD_CORE
     #define Py_BUILD_CORE 1
   #endif
   #include "internal/pycore_frame.h"
 #endif
 #if CYTHON_COMPILING_IN_LIMITED_API
+static PyObject *__Pyx_PyCode_Replace_For_AddTraceback(PyObject *code, PyObject *scratch_dict,
+                                                       PyObject *firstlineno, PyObject *name) {
+    PyObject *replace = NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_firstlineno", firstlineno))) return NULL;
+    if (unlikely(PyDict_SetItemString(scratch_dict, "co_name", name))) return NULL;
+    replace = PyObject_GetAttrString(code, "replace");
+    if (likely(replace)) {
+        PyObject *result;
+        result = PyObject_Call(replace, __pyx_empty_tuple, scratch_dict);
+        Py_DECREF(replace);
+        return result;
+    }
+    #if __PYX_LIMITED_VERSION_HEX < 0x030780000
+    PyErr_Clear();
+    {
+        PyObject *compiled = NULL, *result = NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "code", code))) return NULL;
+        if (unlikely(PyDict_SetItemString(scratch_dict, "type", (PyObject*)(&PyType_Type)))) return NULL;
+        compiled = Py_CompileString(
+            "out = type(code)(\n"
+            "  code.co_argcount, code.co_kwonlyargcount, code.co_nlocals, code.co_stacksize,\n"
+            "  code.co_flags, code.co_code, code.co_consts, code.co_names,\n"
+            "  code.co_varnames, code.co_filename, co_name, co_firstlineno,\n"
+            "  code.co_lnotab)\n", "<dummy>", Py_file_input);
+        if (!compiled) return NULL;
+        result = PyEval_EvalCode(compiled, scratch_dict, scratch_dict);
+        Py_DECREF(compiled);
+        if (!result) PyErr_Print();
+        Py_DECREF(result);
+        result = PyDict_GetItemString(scratch_dict, "out");
+        if (result) Py_INCREF(result);
+        return result;
+    }
+    #endif
+}
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
+    PyObject *code_object = NULL, *py_py_line = NULL, *py_funcname = NULL, *dict = NULL;
+    PyObject *replace = NULL, *getframe = NULL, *frame = NULL;
+    PyObject *exc_type, *exc_value, *exc_traceback;
+    int success = 0;
     if (c_line) {
         (void) __pyx_cfilenm;
         (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
     }
-    _PyTraceback_Add(funcname, filename, py_line);
+    PyErr_Fetch(&exc_type, &exc_value, &exc_traceback);
+    code_object = Py_CompileString("_getframe()", filename, Py_eval_input);
+    if (unlikely(!code_object)) goto bad;
+    py_py_line = PyLong_FromLong(py_line);
+    if (unlikely(!py_py_line)) goto bad;
+    py_funcname = PyUnicode_FromString(funcname);
+    if (unlikely(!py_funcname)) goto bad;
+    dict = PyDict_New();
+    if (unlikely(!dict)) goto bad;
+    {
+        PyObject *old_code_object = code_object;
+        code_object = __Pyx_PyCode_Replace_For_AddTraceback(code_object, dict, py_py_line, py_funcname);
+        Py_DECREF(old_code_object);
+    }
+    if (unlikely(!code_object)) goto bad;
+    getframe = PySys_GetObject("_getframe");
+    if (unlikely(!getframe)) goto bad;
+    if (unlikely(PyDict_SetItemString(dict, "_getframe", getframe))) goto bad;
+    frame = PyEval_EvalCode(code_object, dict, dict);
+    if (unlikely(!frame) || frame == Py_None) goto bad;
+    success = 1;
+  bad:
+    PyErr_Restore(exc_type, exc_value, exc_traceback);
+    Py_XDECREF(code_object);
+    Py_XDECREF(py_py_line);
+    Py_XDECREF(py_funcname);
+    Py_XDECREF(dict);
+    Py_XDECREF(replace);
+    if (success) {
+        PyTraceBack_Here(
+            (struct _frame*)frame);
+    }
+    Py_XDECREF(frame);
 }
 #else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
     PyCodeObject *py_code = NULL;
     PyObject *py_funcname = NULL;
@@ -27978,56 +28853,62 @@
       }
     }
   } while (ctx->enc_count);
   ctx->enc_type = 0;
   ctx->is_complex = 0;
   return 0;
 }
-static PyObject *
+static int
 __pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
 {
     const char *ts = *tsp;
     int i = 0, number, ndim;
     ++ts;
     if (ctx->new_count != 1) {
         PyErr_SetString(PyExc_ValueError,
                         "Cannot handle repeated arrays in format string");
-        return NULL;
+        return -1;
     }
-    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return -1;
     ndim = ctx->head->field->type->ndim;
     while (*ts && *ts != ')') {
         switch (*ts) {
             case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
             default:  break;
         }
         number = __Pyx_BufFmt_ExpectNumber(&ts);
-        if (number == -1) return NULL;
-        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
-            return PyErr_Format(PyExc_ValueError,
+        if (number == -1) return -1;
+        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i]) {
+            PyErr_Format(PyExc_ValueError,
                         "Expected a dimension of size %zu, got %d",
                         ctx->head->field->type->arraysize[i], number);
-        if (*ts != ',' && *ts != ')')
-            return PyErr_Format(PyExc_ValueError,
+            return -1;
+        }
+        if (*ts != ',' && *ts != ')') {
+            PyErr_Format(PyExc_ValueError,
                                 "Expected a comma in format string, got '%c'", *ts);
+            return -1;
+        }
         if (*ts == ',') ts++;
         i++;
     }
-    if (i != ndim)
-        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
+    if (i != ndim) {
+        PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
                             ctx->head->field->type->ndim, i);
+        return -1;
+    }
     if (!*ts) {
         PyErr_SetString(PyExc_ValueError,
                         "Unexpected end of format string, expected ')'");
-        return NULL;
+        return -1;
     }
     ctx->is_valid_array = 1;
     ctx->new_count = 1;
     *tsp = ++ts;
-    return Py_None;
+    return 0;
 }
 static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
   int got_Z = 0;
   while (1) {
     switch(*ts) {
       case 0:
         if (ctx->enc_type != 0 && ctx->head == NULL) {
@@ -28145,15 +29026,15 @@
         break;
       case ':':
         ++ts;
         while(*ts != ':') ++ts;
         ++ts;
         break;
       case '(':
-        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
+        if (__pyx_buffmt_parse_array(ctx, &ts) < 0) return NULL;
         break;
       default:
         {
           int number = __Pyx_BufFmt_ExpectNumber(&ts);
           if (number == -1) return NULL;
           ctx->new_count = (size_t)number;
         }
@@ -29515,16 +30396,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(long));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        kwds = PyDict_New();
+        if (!kwds) goto limited_bad;
+        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(from_bytes);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(order_str);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(kwds);
+        return result;
+#endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
@@ -29826,16 +30731,40 @@
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
+#if !CYTHON_COMPILING_IN_LIMITED_API
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
+#else
+        PyObject *from_bytes, *result = NULL;
+        PyObject *py_bytes = NULL, *arg_tuple = NULL, *kwds = NULL, *order_str = NULL;
+        from_bytes = PyObject_GetAttrString((PyObject*)&PyInt_Type, "from_bytes");
+        if (!from_bytes) return NULL;
+        py_bytes = PyBytes_FromStringAndSize((char*)bytes, sizeof(int));
+        if (!py_bytes) goto limited_bad;
+        order_str = PyUnicode_FromString(little ? "little" : "big");
+        if (!order_str) goto limited_bad;
+        arg_tuple = PyTuple_Pack(2, py_bytes, order_str);
+        if (!arg_tuple) goto limited_bad;
+        kwds = PyDict_New();
+        if (!kwds) goto limited_bad;
+        if (PyDict_SetItemString(kwds, "signed", __Pyx_NewRef(!is_unsigned ? Py_True : Py_False))) goto limited_bad;
+        result = PyObject_Call(from_bytes, arg_tuple, kwds);
+        limited_bad:
+        Py_XDECREF(from_bytes);
+        Py_XDECREF(py_bytes);
+        Py_XDECREF(order_str);
+        Py_XDECREF(arg_tuple);
+        Py_XDECREF(kwds);
+        return result;
+#endif
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
@@ -30113,56 +31042,66 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__26));
+        Py_XDECREF(name);
+        name = __Pyx_NewRef(__pyx_n_s__26);
     }
     return name;
 }
 #endif
 
 /* CheckBinaryVersion */
-  static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
+  static unsigned long __Pyx_get_runtime_version() {
+#if __PYX_LIMITED_VERSION_HEX >= 0x030B00A4
+    return Py_Version & ~0xFFUL;
+#else
+    const char* rt_version = Py_GetVersion();
+    unsigned long version = 0;
+    unsigned long factor = 0x01000000UL;
+    unsigned int digit = 0;
+    int i = 0;
+    while (factor) {
+        while ('0' <= rt_version[i] && rt_version[i] <= '9') {
+            digit = digit * 10 + (unsigned int) (rt_version[i] - '0');
+            ++i;
         }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
+        version += factor * digit;
+        if (rt_version[i] != '.')
             break;
-        }
+        digit = 0;
+        factor >>= 8;
+        ++i;
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    return version;
+#endif
+}
+static int __Pyx_check_binary_version(unsigned long ct_version, unsigned long rt_version, int allow_newer) {
+    const unsigned long MAJOR_MINOR = 0xFFFF0000UL;
+    if ((rt_version & MAJOR_MINOR) == (ct_version & MAJOR_MINOR))
+        return 0;
+    if (likely(allow_newer && (rt_version & MAJOR_MINOR) > (ct_version & MAJOR_MINOR)))
+        return 1;
+    {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
-                      "does not match runtime version %s",
-                      ctversion, __Pyx_MODULE_NAME, rtversion);
+                      "compile time Python version %d.%d "
+                      "of module '%.100s' "
+                      "%s "
+                      "runtime version %d.%d",
+                       (int) (ct_version >> 24), (int) ((ct_version >> 16) & 0xFF),
+                       __Pyx_MODULE_NAME,
+                       (allow_newer) ? "was newer than" : "does not match",
+                       (int) (rt_version >> 24), (int) ((rt_version >> 16) & 0xFF)
+       );
         return PyErr_WarnEx(NULL, message, 1);
     }
-    return 0;
 }
 
 /* InitStrings */
   #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
@@ -30200,16 +31139,32 @@
             return -1;
         #endif
         ++t;
     }
     return 0;
 }
 
+#include <string.h>
+static CYTHON_INLINE Py_ssize_t __Pyx_ssize_strlen(const char *s) {
+    size_t len = strlen(s);
+    if (unlikely(len > (size_t) PY_SSIZE_T_MAX)) {
+        PyErr_SetString(PyExc_OverflowError, "byte string is too long");
+        return -1;
+    }
+    return (Py_ssize_t) len;
+}
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
-    return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return __Pyx_PyUnicode_FromStringAndSize(c_str, len);
+}
+static CYTHON_INLINE PyObject* __Pyx_PyByteArray_FromString(const char* c_str) {
+    Py_ssize_t len = __Pyx_ssize_strlen(c_str);
+    if (unlikely(len < 0)) return NULL;
+    return PyByteArray_FromStringAndSize(c_str, len);
 }
 static CYTHON_INLINE const char* __Pyx_PyObject_AsString(PyObject* o) {
     Py_ssize_t ignore;
     return __Pyx_PyObject_AsStringAndSize(o, &ignore);
 }
 #if __PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT
 #if !CYTHON_PEP393_ENABLED
```

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/optimized/optimized.pyx` & `emzed_gui-3.0.0a9/src/emzed_gui/optimized/optimized.pyx`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/peakmap_explorer/__init__.py` & `emzed_gui-3.0.0a9/src/emzed_gui/peakmap_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/peakmap_explorer/peakmap_explorer.py` & `emzed_gui-3.0.0a9/src/emzed_gui/peakmap_explorer/peakmap_explorer.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/resources/__init__.py` & `emzed_gui-3.0.0a9/src/emzed_gui/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/resources/icon64.png` & `emzed_gui-3.0.0a9/src/emzed_gui/resources/icon64.png`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/simple_dialogs.py` & `emzed_gui-3.0.0a9/src/emzed_gui/simple_dialogs.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/__init__.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/_debug.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/_debug.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/_table_explorer_dialog.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/_table_explorer_dialog.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/ask_value.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/ask_value.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/async_runner.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/async_runner.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/button_delegate.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/button_delegate.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/image_dialog.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/image_dialog.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/inspect.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/inspect.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # You should have received a copy of the GNU General Public License along with this
 # program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import guidata
 from emzed import Table
 from PyQt5.QtCore import Qt
+from PyQt5.QtGui import QFont, QFontDatabase
 
 from .table_explorer import TableExplorer
 
 
 def inspect(
     what,
     offerAbortOption=False,
@@ -34,14 +35,20 @@
     allows the inspection and editing of simple or multiple
     tables.
 
     """
     if isinstance(what, Table):
         what = [what]
     app = guidata.qapplication()  # singleton!
+    if sys.platform == "darwin":
+        # setting fonts in table does not work on Mac, but setting the font for the app
+        # does. now everything is in typewriter mode, but this is better than before:
+        monospace = QFont("monospace")
+        monospace.setStyleHint(QFont.Typewriter)
+        app.setFont(monospace)
     explorer = TableExplorer(
         what,
         offerAbortOption,
         parent=parent,
         close_callback=close_callback,
         custom_buttons_config=custom_buttons_config,
     )
```

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_explorer.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_explorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -857,15 +857,14 @@
 
         group_by_idx = self.chooseGroupColumn.currentIndex()
         if group_by_idx > 0:
             self.select_rows_in_group(widget_row_idx, group_by_idx)
             return
 
         self.select_row()
-        print("update")
         self.tableView.viewport().update()
 
     def select_row(self):
 
         start = time.time()
         process_events = guidata.qapplication().processEvents
 
@@ -940,33 +939,29 @@
                     self,
                     "Warning",
                     "multiselect would mark %d lines. "
                     "reduced number of lines to %d" % (len(to_select), N),
                 )
                 to_select = to_select[:N]
 
-            # self.setEnabled(False)   # did not work.
             self.tableView.blockSignals(True)
-            # self.setCursor(Qt.WaitCursor)
             try:
                 mode_before = self.tableView.selectionMode()
                 scrollbar_before = self.tableView.verticalScrollBar().value()
 
                 self.tableView.setSelectionMode(QAbstractItemView.MultiSelection)
                 for i in to_select:
-                    # avoid "double click !" wich de-selects current row
+                    # avoid "double click!" wich de-selects current row
                     if i != widget_row_idx:
                         self.tableView.selectRow(i)
                 self.tableView.setSelectionMode(mode_before)
                 self.tableView.verticalScrollBar().setValue(scrollbar_before)
 
                 self.model.set_selected_widget_rows(to_select)
 
-                n = len(to_select)
-
                 self.model.set_row_header_colors(to_select)
 
                 if not self.eic_only_mode:
                     self.choose_spec.blockSignals(True)
                     try:
                         self.setup_spectrum_chooser()
                     finally:
```

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_explorer_layout.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_explorer_layout.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_explorer_model.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_explorer_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,31 +22,25 @@
 import re
 import warnings
 from datetime import datetime
 
 import guidata
 from emzed import PeakMap
 from emzed.config import folders
+from emzed_gui.configs import get_color
+from emzed_gui.helpers import timethis
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import QMenuBar
 
-from emzed_gui.configs import get_color
-from emzed_gui.helpers import timethis
-
 from .table_explorer_model_actions import *
 
 ROWS_BATCH_SIZE = 100
 
 
-# https://stackoverflow.com/questions/1468022
-MONOSPACE = QFont("Monospace")
-MONOSPACE.setStyleHint(QFont.TypeWriter)
-
-
 def supported_postfixes(t, names):
     result = []
     if all(name in t.col_names for name in names):
         result.append("")
 
     postfixes = set(
         "__" + name.split("__", 1)[1] for name in t.col_names if "__" in name
@@ -251,15 +245,15 @@
     def row(self, index):
         ridx, cidx = self.table_index(index)
         return self._get_table_row(ridx)
 
     DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
     def font(self, index):
-        font = MONOSPACE
+        font = self.monospace
         content = self.data(index, Qt.DisplayRole)
         font.setUnderline(isUrl(content))
         return font
 
     def check_state_data(self, index, role):
         if role == Qt.CheckStateRole:
             value = self.cell_value(index)
@@ -280,29 +274,30 @@
             raise IndexError(
                 "invalid access of row %d of table of length %d"
                 % (ridx, len(self.table))
             )
         # fill cache for given row
         color = row["color"]
         if color is None:
-            for cidx_ in range(len(self.widgetColToDataCol)):
+            for cidx_ in range(len(row)):
                 self._color_cache[ridx, cidx_] = None
         elif isinstance(color, str):
-            for cidx_ in range(len(self.widgetColToDataCol)):
+            for cidx_ in range(len(row)):
                 self._color_cache[ridx, cidx_] = parse_color(color)
         elif isinstance(color, dict):
-            for cidx_ in range(len(self.widgetColToDataCol)):
+            for cidx_ in range(len(row)):
                 name = self.table.col_names[cidx_]
                 column_color = color.get(name)
                 if column_color is not None:
                     self._color_cache[ridx, cidx_] = parse_color(column_color)
                 else:
                     self._color_cache[ridx, cidx_] = None
         else:
             return
+
         return self._color_cache[ridx, cidx]
 
     def data(self, index, role=Qt.DisplayRole):
         if not index.isValid():
             return QVariant()
 
         if role == Qt.FontRole:
@@ -329,15 +324,15 @@
             else:
                 try:
                     shown = fmter(value)
                 except Exception:
                     shown = value.strftime(self.DATE_FORMAT)
         else:
             shown = fmter(value)
-        return QVariant(shown)
+        return shown
 
     def headerData(self, section, orientation, role=Qt.DisplayRole):
         if role == Qt.ForegroundRole and orientation == Qt.Vertical:
             color = self.colors_selected_rows.get(section)
             if color is not None:
                 return QBrush(QColor(color))
         if role != Qt.DisplayRole:
@@ -784,14 +779,16 @@
             return TableModel(table, parent)
 
 
 class MutableTableModel(TableModel):
     def __init__(self, table, parent):
         super(MutableTableModel, self).__init__(table, parent)
         self.nonEditables = set()
+        self.monospace = QFont("monospace")
+        self.monospace.setStyleHint(QFont.Typewriter)
 
     def data(self, index, role=Qt.DisplayRole):
         if role == Qt.EditRole:
             shown = super(MutableTableModel, self).data(index, Qt.DisplayRole)
             return str(shown)
         else:
             return super(MutableTableModel, self).data(index, role)
```

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_explorer_model_actions.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_explorer_model_actions.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/table_view.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/table_view.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/table_explorer/text_delegate.py` & `emzed_gui-3.0.0a9/src/emzed_gui/table_explorer/text_delegate.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/__init__.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_ask_value_dialog.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_ask_value_dialog.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_choose_range.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_choose_range.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_choose_spectra_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_choose_spectra_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_choose_value.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_choose_value.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_column_selection_dialog.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_column_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_filter_criteria_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_filter_criteria_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_image_scaling_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_image_scaling_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_integration_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_integration_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_spectra_selector_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_spectra_selector_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_string_filter.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_string_filter.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/_view_range_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/_view_range_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/ask_value_dialogs.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/ask_value_dialogs.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/choose_spectra_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/choose_spectra_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/column_selection_dialog.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/column_selection_dialog.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/config.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/config.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/eic_plotting_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/eic_plotting_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,15 @@
         return self.current_peak
 
     def plot_eics(self, peak_data, models, titles, background):
 
         if not peak_data:
             return
 
-        background_curves = []
+        background_curves = [None] * len(peak_data)
         rtmins = []
         rtmaxs = []
         iimaxs = []
 
         if not models:
             models = [None] * len(peak_data)
 
@@ -492,15 +492,15 @@
             else:
                 title = ""
 
             if background:
                 background_curve = make_unselectable_curve(
                     [], [], linewidth=1, color=config["color"], linestyle="DotLine"
                 )
-                background_curves.append(background_curve)
+                background_curves[i] = background_curve
                 self.add_item(background_curve)
 
             curve = make_unselectable_curve(rts, iis, title=title, **config)
             self.add_item(curve)
             yield
 
             model = models[i]
@@ -543,15 +543,16 @@
     def update_background_curves(self, rtmin, rtmax):
         if not self.current_peak_data or not self.background_curves:
             return
 
         for i, (pm, _, _, mzmin, mzmax) in enumerate(self.current_peak_data):
             ms_level = min(pm.ms_levels())
             rts, iis = pm.chromatogram(mzmin, mzmax, rtmin, rtmax, ms_level)
-            self.background_curves[i].set_data(rts, iis)
+            if self.background_curves[i] is not None:
+                self.background_curves[i].set_data(rts, iis)
 
 
 class SnappingRangeSelection(XRangeSelection):
 
     """modification:
     - only limit bars can be moved
     - snaps to given rt-values which are in general not equally spaced
```

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/filter_criteria_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/filter_criteria_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/image_scaling_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/image_scaling_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/integration_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/integration_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/modified_guiqwt.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/modified_guiqwt.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/mz_plotting_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/mz_plotting_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/peakmap_plotting_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/peakmap_plotting_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/spectra_selector_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/spectra_selector_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/ts_plotting_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/ts_plotting_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui/widgets/view_range_widget.py` & `emzed_gui-3.0.0a9/src/emzed_gui/widgets/view_range_widget.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/src/emzed_gui.egg-info/SOURCES.txt` & `emzed_gui-3.0.0a9/src/emzed_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/tests/test_import.py` & `emzed_gui-3.0.0a9/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `emzed_gui-3.0.0a8/tests/test_peak_map_optimizations.py` & `emzed_gui-3.0.0a9/tests/test_peak_map_optimizations.py`

 * *Files identical despite different names*

