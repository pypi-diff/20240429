# Comparing `tmp/lukasdata-1.2.5.tar.gz` & `tmp/lukasdata-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.2.5.tar", last modified: Mon Apr 29 11:50:53 2024, max compression
+gzip compressed data, was "lukasdata-1.2.6.tar", last modified: Mon Apr 29 18:18:19 2024, max compression
```

## Comparing `lukasdata-1.2.5.tar` & `lukasdata-1.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 11:50:53.240481 lukasdata-1.2.5/
--rw-rw-rw-   0        0        0      128 2024-04-29 11:50:53.237483 lukasdata-1.2.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 11:50:53.210510 lukasdata-1.2.5/lukasdata/
--rw-rw-rw-   0        0        0        0 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/change_directory.py
--rw-rw-rw-   0        0        0      198 2024-04-23 22:24:46.000000 lukasdata-1.2.5/lukasdata/concat_dfs.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/count_nans.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/create_mask.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/dict_to_json.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.2.5/lukasdata/drop_column_with_na.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.2.5/lukasdata/get_list_intersection.py
--rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/get_number_columns.py
--rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/json_to_dict.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/list_to_string.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.2.5/lukasdata/mean_impute.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.2.5/lukasdata/na_counts.py
--rw-rw-rw-   0        0        0     1182 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/plot_metric_history.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2.5/lukasdata/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-04-29 11:50:53.236482 lukasdata-1.2.5/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-04-29 11:50:53.000000 lukasdata-1.2.5/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      640 2024-04-29 11:50:53.000000 lukasdata-1.2.5/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 11:50:53.000000 lukasdata-1.2.5/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-29 11:50:53.000000 lukasdata-1.2.5/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-29 11:50:53.000000 lukasdata-1.2.5/lukasdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 11:50:53.240481 lukasdata-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-04-29 11:50:47.000000 lukasdata-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:18:19.549135 lukasdata-1.2.6/
+-rw-rw-rw-   0        0        0      128 2024-04-29 18:18:19.544809 lukasdata-1.2.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 18:18:19.519819 lukasdata-1.2.6/lukasdata/
+-rw-rw-rw-   0        0        0        0 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/change_directory.py
+-rw-rw-rw-   0        0        0      198 2024-04-23 22:24:46.000000 lukasdata-1.2.6/lukasdata/concat_dfs.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/count_nans.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/create_mask.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/dict_to_json.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.2.6/lukasdata/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.2.6/lukasdata/get_list_intersection.py
+-rw-rw-rw-   0        0        0      447 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/get_number_columns.py
+-rw-rw-rw-   0        0        0      255 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/json_to_dict.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/list_to_string.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.2.6/lukasdata/mean_impute.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.2.6/lukasdata/na_counts.py
+-rw-rw-rw-   0        0        0     1182 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/plot_metric_history.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.2.6/lukasdata/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-04-29 18:18:19.542810 lukasdata-1.2.6/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-04-29 18:18:19.000000 lukasdata-1.2.6/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2024-04-29 18:18:19.000000 lukasdata-1.2.6/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 18:18:19.000000 lukasdata-1.2.6/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-29 18:18:19.000000 lukasdata-1.2.6/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 18:18:19.000000 lukasdata-1.2.6/lukasdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 18:18:19.550131 lukasdata-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-04-29 18:18:12.000000 lukasdata-1.2.6/setup.py
```

### Comparing `lukasdata-1.2.5/lukasdata/change_directory.py` & `lukasdata-1.2.6/lukasdata/change_directory.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.2.5/lukasdata/plot_metric_history.py` & `lukasdata-1.2.6/lukasdata/plot_metric_history.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.2.5/lukasdata.egg-info/SOURCES.txt` & `lukasdata-1.2.6/lukasdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

