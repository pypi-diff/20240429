# Comparing `tmp/spinesUtils-0.4.0.tar.gz` & `tmp/spinesutils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinesUtils-0.4.0.tar", last modified: Fri Jan 19 08:55:32 2024, max compression
+gzip compressed data, was "spinesutils-0.4.1.tar", last modified: Mon Apr 29 03:42:07 2024, max compression
```

## Comparing `spinesUtils-0.4.0.tar` & `spinesutils-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.673944 spinesUtils-0.4.0/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 spinesUtils-0.4.0/LICENSE
--rw-r--r--   0 guobingming   (501) staff       (20)    38528 2024-01-19 08:55:32.673719 spinesUtils-0.4.0/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    37692 2024-01-19 08:50:48.000000 spinesUtils-0.4.0/README.md
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-01-19 08:55:32.673987 spinesUtils-0.4.0/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1101 2024-01-19 08:54:59.000000 spinesUtils-0.4.0/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.670104 spinesUtils-0.4.0/spinesUtils/
--rw-r--r--   0 guobingming   (501) staff       (20)      882 2024-01-19 08:54:59.000000 spinesUtils-0.4.0/spinesUtils/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.671500 spinesUtils-0.4.0/spinesUtils/asserts/
--rw-r--r--   0 guobingming   (501) staff       (20)      360 2024-01-03 03:11:40.000000 spinesUtils-0.4.0/spinesUtils/asserts/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3117 2024-01-19 05:47:23.000000 spinesUtils-0.4.0/spinesUtils/asserts/_func_params.py
--rw-r--r--   0 guobingming   (501) staff       (20)    10435 2024-01-18 08:09:06.000000 spinesUtils-0.4.0/spinesUtils/asserts/_inspect.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3887 2024-01-19 05:48:56.000000 spinesUtils-0.4.0/spinesUtils/asserts/_type_and_exceptions.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.671733 spinesUtils-0.4.0/spinesUtils/data_insight/
--rw-r--r--   0 guobingming   (501) staff       (20)      108 2023-09-19 11:00:45.000000 spinesUtils-0.4.0/spinesUtils/data_insight/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     9218 2024-01-18 10:31:20.000000 spinesUtils-0.4.0/spinesUtils/data_insight/_df_preview.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4943 2024-01-19 03:52:35.000000 spinesUtils-0.4.0/spinesUtils/decorators.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.672008 spinesUtils-0.4.0/spinesUtils/feature_tools/
--rw-r--r--   0 guobingming   (501) staff       (20)      166 2024-01-19 03:52:35.000000 spinesUtils-0.4.0/spinesUtils/feature_tools/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     6001 2024-01-19 03:48:12.000000 spinesUtils-0.4.0/spinesUtils/feature_tools/_feature_tools.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.672253 spinesUtils-0.4.0/spinesUtils/io/
--rw-r--r--   0 guobingming   (501) staff       (20)       27 2023-09-21 08:48:07.000000 spinesUtils-0.4.0/spinesUtils/io/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4429 2024-01-19 03:52:35.000000 spinesUtils-0.4.0/spinesUtils/io/_data.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5074 2024-01-19 06:03:40.000000 spinesUtils-0.4.0/spinesUtils/logging.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.672503 spinesUtils-0.4.0/spinesUtils/models/
--rw-r--r--   0 guobingming   (501) staff       (20)       63 2024-01-18 07:47:17.000000 spinesUtils-0.4.0/spinesUtils/models/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     6796 2024-01-19 03:49:27.000000 spinesUtils-0.4.0/spinesUtils/models/imbalanced_classifier.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.672986 spinesUtils-0.4.0/spinesUtils/preprocessing/
--rw-r--r--   0 guobingming   (501) staff       (20)      406 2023-10-26 03:06:51.000000 spinesUtils-0.4.0/spinesUtils/preprocessing/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    16423 2024-01-19 03:52:35.000000 spinesUtils-0.4.0/spinesUtils/preprocessing/_compress_memory.py
--rw-r--r--   0 guobingming   (501) staff       (20)     3064 2024-01-18 11:02:56.000000 spinesUtils-0.4.0/spinesUtils/preprocessing/_data_shape.py
--rw-r--r--   0 guobingming   (501) staff       (20)     9620 2024-01-19 08:28:41.000000 spinesUtils-0.4.0/spinesUtils/preprocessing/_split_tools.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5051 2024-01-19 08:49:16.000000 spinesUtils-0.4.0/spinesUtils/timer.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.673262 spinesUtils-0.4.0/spinesUtils/utils/
--rw-r--r--   0 guobingming   (501) staff       (20)      225 2024-01-19 03:49:27.000000 spinesUtils-0.4.0/spinesUtils/utils/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     9182 2024-01-19 03:52:35.000000 spinesUtils-0.4.0/spinesUtils/utils/_utils.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-01-19 08:55:32.673472 spinesUtils-0.4.0/spinesUtils.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    38528 2024-01-19 08:55:32.000000 spinesUtils-0.4.0/spinesUtils.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)      982 2024-01-19 08:55:32.000000 spinesUtils-0.4.0/spinesUtils.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-01-19 08:55:32.000000 spinesUtils-0.4.0/spinesUtils.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2023-09-19 15:24:48.000000 spinesUtils-0.4.0/spinesUtils.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      120 2024-01-19 08:55:32.000000 spinesUtils-0.4.0/spinesUtils.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       12 2024-01-19 08:55:32.000000 spinesUtils-0.4.0/spinesUtils.egg-info/top_level.txt
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.247060 spinesutils-0.4.1/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 spinesutils-0.4.1/LICENSE
+-rw-r--r--   0 guobingming   (501) staff       (20)    34307 2024-04-29 03:42:07.246834 spinesutils-0.4.1/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    33442 2024-04-29 03:40:46.000000 spinesutils-0.4.1/README.md
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-29 03:42:07.247098 spinesutils-0.4.1/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1126 2024-04-29 03:40:46.000000 spinesutils-0.4.1/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.240494 spinesutils-0.4.1/spinesUtils/
+-rw-r--r--   0 guobingming   (501) staff       (20)       23 2024-04-29 03:40:23.000000 spinesutils-0.4.1/spinesUtils/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.242438 spinesutils-0.4.1/spinesUtils/asserts/
+-rw-r--r--   0 guobingming   (501) staff       (20)      360 2024-01-03 03:11:40.000000 spinesutils-0.4.1/spinesUtils/asserts/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3117 2024-01-19 05:47:23.000000 spinesutils-0.4.1/spinesUtils/asserts/_func_params.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    10435 2024-01-18 08:09:06.000000 spinesutils-0.4.1/spinesUtils/asserts/_inspect.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3887 2024-01-19 05:48:56.000000 spinesutils-0.4.1/spinesUtils/asserts/_type_and_exceptions.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.242968 spinesutils-0.4.1/spinesUtils/data_insight/
+-rw-r--r--   0 guobingming   (501) staff       (20)      108 2023-09-19 11:00:45.000000 spinesutils-0.4.1/spinesUtils/data_insight/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     9222 2024-04-29 03:40:23.000000 spinesutils-0.4.1/spinesUtils/data_insight/_df_preview.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4943 2024-01-19 03:52:35.000000 spinesutils-0.4.1/spinesUtils/decorators.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.243525 spinesutils-0.4.1/spinesUtils/feature_tools/
+-rw-r--r--   0 guobingming   (501) staff       (20)      166 2024-01-19 03:52:35.000000 spinesutils-0.4.1/spinesUtils/feature_tools/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6001 2024-01-19 03:48:12.000000 spinesutils-0.4.1/spinesUtils/feature_tools/_feature_tools.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.244111 spinesutils-0.4.1/spinesUtils/io/
+-rw-r--r--   0 guobingming   (501) staff       (20)       27 2023-09-21 08:48:07.000000 spinesutils-0.4.1/spinesUtils/io/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4429 2024-01-19 03:52:35.000000 spinesutils-0.4.1/spinesUtils/io/_data.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     5074 2024-01-19 06:03:40.000000 spinesutils-0.4.1/spinesUtils/logging.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.244737 spinesutils-0.4.1/spinesUtils/models/
+-rw-r--r--   0 guobingming   (501) staff       (20)       63 2024-01-18 07:47:17.000000 spinesutils-0.4.1/spinesUtils/models/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6796 2024-01-19 03:49:27.000000 spinesutils-0.4.1/spinesUtils/models/imbalanced_classifier.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.245581 spinesutils-0.4.1/spinesUtils/preprocessing/
+-rw-r--r--   0 guobingming   (501) staff       (20)      327 2024-04-29 03:40:23.000000 spinesutils-0.4.1/spinesUtils/preprocessing/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    16423 2024-01-19 03:52:35.000000 spinesutils-0.4.1/spinesUtils/preprocessing/_compress_memory.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     9620 2024-01-19 08:28:41.000000 spinesutils-0.4.1/spinesUtils/preprocessing/_split_tools.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     5051 2024-01-19 08:49:16.000000 spinesutils-0.4.1/spinesUtils/timer.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.246253 spinesutils-0.4.1/spinesUtils/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)      225 2024-01-19 03:49:27.000000 spinesutils-0.4.1/spinesUtils/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     9182 2024-01-19 03:52:35.000000 spinesutils-0.4.1/spinesUtils/utils/_utils.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-29 03:42:07.246573 spinesutils-0.4.1/spinesUtils.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    34307 2024-04-29 03:42:07.000000 spinesutils-0.4.1/spinesUtils.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)      941 2024-04-29 03:42:07.000000 spinesutils-0.4.1/spinesUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-29 03:42:07.000000 spinesutils-0.4.1/spinesUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2023-09-19 15:24:48.000000 spinesutils-0.4.1/spinesUtils.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      134 2024-04-29 03:42:07.000000 spinesutils-0.4.1/spinesUtils.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       12 2024-04-29 03:42:07.000000 spinesutils-0.4.1/spinesUtils.egg-info/top_level.txt
```

### Comparing `spinesUtils-0.4.0/LICENSE` & `spinesutils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/PKG-INFO` & `spinesutils-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spinesUtils
-Version: 0.4.0
+Version: 0.4.1
 Summary: spinesUtils is a user-friendly toolkit for the machine learning ecosystem.
 Home-page: https://github.com/BirchKwok/spinesUtils
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: machine learning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,17 +14,18 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn>=1.0.2
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: dask>=2023.6.0
-Requires-Dist: pyarrow>=11.0.0
+Requires-Dist: pyarrow>=14.0.1
 Requires-Dist: polars>=0.19.3
 Requires-Dist: pytz>=2021.1
+Requires-Dist: numba>=0.58.1
 
 # spinesUtils 
 *Dedicated to helping users do more in less time.*
 
 <big><i><b>spinesUtils</b></i></big>
  is a user-friendly toolkit for the machine learning ecosystem, offering ready-to-use features such as
 
@@ -236,90 +237,14 @@
     turbo_method='polars',  # use turbo_method to speed up load time
     chunk_size=None,  # it can be integer if you want to use pandas backend
     transform2low_mem=True,  # it can compresses file to save more memory
     verbose=False
 )
 ```
 
-
-    ---------------------------------------------------------------------------
-
-    FileNotFoundError                         Traceback (most recent call last)
-
-    /var/folders/4m/8hmtzcr17x94h4cmzhc0zrgh0000gn/T/ipykernel_701/737171132.py in ?()
-          1 from spinesUtils import read_csv
-          2 
-    ----> 3 your_df = read_csv(
-          4     fp='/path/to/your/file.csv',
-          5     sep=',',  # equal to pandas read_csv.sep
-          6     turbo_method='polars',  # use turbo_method to speed up load time
-
-
-    ~/projects/spinesUtils/spinesUtils/asserts/_inspect.py in ?(*args, **kwargs)
-        194             if mismatched_params:
-        195                 error_msg = self.build_type_error_msg(mismatched_params)
-        196                 raise ParametersTypeError(error_msg)
-        197 
-    --> 198             return func(**kwargs)
-    
-
-    ~/projects/spinesUtils/spinesUtils/asserts/_inspect.py in ?(*args, **kwargs)
-        256             if mismatched_params:
-        257                 error_msg = self.build_values_error_msg(mismatched_params)
-        258                 raise ParametersValueError(error_msg)
-        259 
-    --> 260             return func(**kwargs)
-    
-
-    ~/projects/spinesUtils/spinesUtils/io/_data.py in ?(fp, sep, chunk_size, transform2low_mem, turbo_method, encoding, verbose, **read_csv_kwargs)
-        100 
-        101     if chunk_size:
-        102         df = read_text(fp)
-        103     else:
-    --> 104         df = turbo_reader(fp, turbo_method)
-        105 
-        106     if transform2low_mem:
-        107         from ..preprocessing import transform_dtypes_low_mem
-
-
-    ~/projects/spinesUtils/spinesUtils/io/_data.py in ?(fpath, tm)
-         65     def turbo_reader(fpath, tm):
-         66         if tm == 'polars':
-         67             from polars import read_csv
-    ---> 68             return read_csv(fpath, separator=sep, encoding=encoding, **read_csv_kwargs).to_pandas()
-         69 
-         70         if tm == 'pyarrow':
-         71             from pyarrow.csv import read_csv, ParseOptions, ReadOptions
-
-
-    ~/miniconda3/envs/dev/lib/python3.11/site-packages/polars/io/csv/functions.py in ?(source, has_header, columns, new_columns, separator, comment_char, quote_char, skip_rows, dtypes, schema, null_values, missing_utf8_is_empty_string, ignore_errors, try_parse_dates, n_threads, infer_schema_length, batch_size, n_rows, encoding, low_memory, rechunk, use_pyarrow, storage_options, skip_rows_after_header, row_count_name, row_count_offset, sample_size, eol_char, raise_if_empty, truncate_ragged_lines)
-        362         use_pyarrow=False,
-        363         raise_if_empty=raise_if_empty,
-        364         **storage_options,
-        365     ) as data:
-    --> 366         df = pl.DataFrame._read_csv(
-        367             data,
-        368             has_header=has_header,
-        369             columns=columns if columns else projection,
-
-
-    ~/miniconda3/envs/dev/lib/python3.11/site-packages/polars/dataframe/frame.py in ?(cls, source, has_header, columns, separator, comment_char, quote_char, skip_rows, dtypes, schema, null_values, missing_utf8_is_empty_string, ignore_errors, try_parse_dates, n_threads, infer_schema_length, batch_size, n_rows, encoding, low_memory, rechunk, skip_rows_after_header, row_count_name, row_count_offset, sample_size, eol_char, raise_if_empty, truncate_ragged_lines)
-        766                 )
-        767 
-        768         projection, columns = handle_projection_columns(columns)
-        769 
-    --> 770         self._df = PyDataFrame.read_csv(
-        771             source,
-        772             infer_schema_length,
-        773             batch_size,
-
-
-    FileNotFoundError: No such file or directory: /path/to/your/file.csv
-
-
 ## Classifiers for imbalanced data
 
 
 ```python
 from spinesUtils.models import MultiClassBalanceClassifier
 ```
 
@@ -527,27 +452,14 @@
 df_insight
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>total</th>
       <th>na</th>
       <th>naPercent</th>
@@ -1193,27 +1105,14 @@
     (8000000, 26) (1000000, 26) (1000000, 26)
 
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>b</th>
       <th>c</th>
       <th>d</th>
```

### Comparing `spinesUtils-0.4.0/README.md` & `spinesutils-0.4.1/spinesUtils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: spinesUtils
+Version: 0.4.1
+Summary: spinesUtils is a user-friendly toolkit for the machine learning ecosystem.
+Home-page: https://github.com/BirchKwok/spinesUtils
+Author: Birch Kwok
+Author-email: birchkwok@gmail.com
+Keywords: machine learning
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: scikit-learn>=1.0.2
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: tqdm>=4.65.0
+Requires-Dist: dask>=2023.6.0
+Requires-Dist: pyarrow>=14.0.1
+Requires-Dist: polars>=0.19.3
+Requires-Dist: pytz>=2021.1
+Requires-Dist: numba>=0.58.1
+
 # spinesUtils 
 *Dedicated to helping users do more in less time.*
 
 <big><i><b>spinesUtils</b></i></big>
  is a user-friendly toolkit for the machine learning ecosystem, offering ready-to-use features such as
 
 - [x] Logging functionality
@@ -212,90 +237,14 @@
     turbo_method='polars',  # use turbo_method to speed up load time
     chunk_size=None,  # it can be integer if you want to use pandas backend
     transform2low_mem=True,  # it can compresses file to save more memory
     verbose=False
 )
 ```
 
-
-    ---------------------------------------------------------------------------
-
-    FileNotFoundError                         Traceback (most recent call last)
-
-    /var/folders/4m/8hmtzcr17x94h4cmzhc0zrgh0000gn/T/ipykernel_701/737171132.py in ?()
-          1 from spinesUtils import read_csv
-          2 
-    ----> 3 your_df = read_csv(
-          4     fp='/path/to/your/file.csv',
-          5     sep=',',  # equal to pandas read_csv.sep
-          6     turbo_method='polars',  # use turbo_method to speed up load time
-
-
-    ~/projects/spinesUtils/spinesUtils/asserts/_inspect.py in ?(*args, **kwargs)
-        194             if mismatched_params:
-        195                 error_msg = self.build_type_error_msg(mismatched_params)
-        196                 raise ParametersTypeError(error_msg)
-        197 
-    --> 198             return func(**kwargs)
-    
-
-    ~/projects/spinesUtils/spinesUtils/asserts/_inspect.py in ?(*args, **kwargs)
-        256             if mismatched_params:
-        257                 error_msg = self.build_values_error_msg(mismatched_params)
-        258                 raise ParametersValueError(error_msg)
-        259 
-    --> 260             return func(**kwargs)
-    
-
-    ~/projects/spinesUtils/spinesUtils/io/_data.py in ?(fp, sep, chunk_size, transform2low_mem, turbo_method, encoding, verbose, **read_csv_kwargs)
-        100 
-        101     if chunk_size:
-        102         df = read_text(fp)
-        103     else:
-    --> 104         df = turbo_reader(fp, turbo_method)
-        105 
-        106     if transform2low_mem:
-        107         from ..preprocessing import transform_dtypes_low_mem
-
-
-    ~/projects/spinesUtils/spinesUtils/io/_data.py in ?(fpath, tm)
-         65     def turbo_reader(fpath, tm):
-         66         if tm == 'polars':
-         67             from polars import read_csv
-    ---> 68             return read_csv(fpath, separator=sep, encoding=encoding, **read_csv_kwargs).to_pandas()
-         69 
-         70         if tm == 'pyarrow':
-         71             from pyarrow.csv import read_csv, ParseOptions, ReadOptions
-
-
-    ~/miniconda3/envs/dev/lib/python3.11/site-packages/polars/io/csv/functions.py in ?(source, has_header, columns, new_columns, separator, comment_char, quote_char, skip_rows, dtypes, schema, null_values, missing_utf8_is_empty_string, ignore_errors, try_parse_dates, n_threads, infer_schema_length, batch_size, n_rows, encoding, low_memory, rechunk, use_pyarrow, storage_options, skip_rows_after_header, row_count_name, row_count_offset, sample_size, eol_char, raise_if_empty, truncate_ragged_lines)
-        362         use_pyarrow=False,
-        363         raise_if_empty=raise_if_empty,
-        364         **storage_options,
-        365     ) as data:
-    --> 366         df = pl.DataFrame._read_csv(
-        367             data,
-        368             has_header=has_header,
-        369             columns=columns if columns else projection,
-
-
-    ~/miniconda3/envs/dev/lib/python3.11/site-packages/polars/dataframe/frame.py in ?(cls, source, has_header, columns, separator, comment_char, quote_char, skip_rows, dtypes, schema, null_values, missing_utf8_is_empty_string, ignore_errors, try_parse_dates, n_threads, infer_schema_length, batch_size, n_rows, encoding, low_memory, rechunk, skip_rows_after_header, row_count_name, row_count_offset, sample_size, eol_char, raise_if_empty, truncate_ragged_lines)
-        766                 )
-        767 
-        768         projection, columns = handle_projection_columns(columns)
-        769 
-    --> 770         self._df = PyDataFrame.read_csv(
-        771             source,
-        772             infer_schema_length,
-        773             batch_size,
-
-
-    FileNotFoundError: No such file or directory: /path/to/your/file.csv
-
-
 ## Classifiers for imbalanced data
 
 
 ```python
 from spinesUtils.models import MultiClassBalanceClassifier
 ```
 
@@ -503,27 +452,14 @@
 df_insight
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>total</th>
       <th>na</th>
       <th>naPercent</th>
@@ -1169,27 +1105,14 @@
     (8000000, 26) (1000000, 26) (1000000, 26)
 
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>b</th>
       <th>c</th>
       <th>d</th>
```

### Comparing `spinesUtils-0.4.0/setup.py` & `spinesutils-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='spinesUtils',
-    version="0.4.0",
+    version="0.4.1",
     description='spinesUtils is a user-friendly toolkit for the machine learning ecosystem.',
     keywords='machine learning',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
@@ -23,14 +23,15 @@
     author_email='birchkwok@gmail.com',
     install_requires=[
         'scikit-learn>=1.0.2',
         'numpy>=1.17.0',
         'pandas>=2.0.0',
         'tqdm>=4.65.0',
         'dask>=2023.6.0',
-        'pyarrow>=11.0.0',
+        "pyarrow>=14.0.1",
         'polars>=0.19.3',
-        'pytz>=2021.1'
+        'pytz>=2021.1',
+        'numba>=0.58.1'
     ],
     zip_safe=False,
     include_package_data=True
 )
```

### Comparing `spinesUtils-0.4.0/spinesUtils/asserts/_func_params.py` & `spinesutils-0.4.1/spinesUtils/asserts/_func_params.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/asserts/_inspect.py` & `spinesutils-0.4.1/spinesUtils/asserts/_inspect.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/asserts/_type_and_exceptions.py` & `spinesutils-0.4.1/spinesUtils/asserts/_type_and_exceptions.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/data_insight/_df_preview.py` & `spinesutils-0.4.1/spinesUtils/data_insight/_df_preview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
 import numpy as np
-from numba import jit
 
 from spinesUtils.feature_tools import select_numeric_cols
 from spinesUtils.asserts import ParameterTypeAssert
 
 
 @ParameterTypeAssert({'df': pd.DataFrame, 'target_col': str, 'groupby': (None, str)})
 def classify_samples_dist(df, target_col, groupby=None):
@@ -131,14 +130,15 @@
     --------
     >>> df = pd.DataFrame({'A': [1, 2, 3], 'B': [4, 5, 6]})
     >>> df_preview(df, indicators=['mean', 'std'])
        mean   std
     A   2.0   1.0
     B   5.0   1.0
     """
+    from numba import jit
 
     @jit(nopython=True, fastmath=True)
     def calculate_skewness_kurtosis(data, mean, std):
         var = std ** 2
         # std = np.sqrt(var)
 
         # 计算三阶和四阶中心矩
```

### Comparing `spinesUtils-0.4.0/spinesUtils/decorators.py` & `spinesutils-0.4.1/spinesUtils/decorators.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/feature_tools/_feature_tools.py` & `spinesutils-0.4.1/spinesUtils/feature_tools/_feature_tools.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/io/_data.py` & `spinesutils-0.4.1/spinesUtils/io/_data.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/logging.py` & `spinesutils-0.4.1/spinesUtils/logging.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/models/imbalanced_classifier.py` & `spinesutils-0.4.1/spinesUtils/models/imbalanced_classifier.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/preprocessing/_compress_memory.py` & `spinesutils-0.4.1/spinesUtils/preprocessing/_compress_memory.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/preprocessing/_split_tools.py` & `spinesutils-0.4.1/spinesUtils/preprocessing/_split_tools.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/timer.py` & `spinesutils-0.4.1/spinesUtils/timer.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils/utils/_utils.py` & `spinesutils-0.4.1/spinesUtils/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `spinesUtils-0.4.0/spinesUtils.egg-info/PKG-INFO` & `spinesutils-0.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: spinesUtils
-Version: 0.4.0
-Summary: spinesUtils is a user-friendly toolkit for the machine learning ecosystem.
-Home-page: https://github.com/BirchKwok/spinesUtils
-Author: Birch Kwok
-Author-email: birchkwok@gmail.com
-Keywords: machine learning
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: scikit-learn>=1.0.2
-Requires-Dist: numpy>=1.17.0
-Requires-Dist: pandas>=2.0.0
-Requires-Dist: tqdm>=4.65.0
-Requires-Dist: dask>=2023.6.0
-Requires-Dist: pyarrow>=11.0.0
-Requires-Dist: polars>=0.19.3
-Requires-Dist: pytz>=2021.1
-
 # spinesUtils 
 *Dedicated to helping users do more in less time.*
 
 <big><i><b>spinesUtils</b></i></big>
  is a user-friendly toolkit for the machine learning ecosystem, offering ready-to-use features such as
 
 - [x] Logging functionality
@@ -236,90 +212,14 @@
     turbo_method='polars',  # use turbo_method to speed up load time
     chunk_size=None,  # it can be integer if you want to use pandas backend
     transform2low_mem=True,  # it can compresses file to save more memory
     verbose=False
 )
 ```
 
-
-    ---------------------------------------------------------------------------
-
-    FileNotFoundError                         Traceback (most recent call last)
-
-    /var/folders/4m/8hmtzcr17x94h4cmzhc0zrgh0000gn/T/ipykernel_701/737171132.py in ?()
-          1 from spinesUtils import read_csv
-          2 
-    ----> 3 your_df = read_csv(
-          4     fp='/path/to/your/file.csv',
-          5     sep=',',  # equal to pandas read_csv.sep
-          6     turbo_method='polars',  # use turbo_method to speed up load time
-
-
-    ~/projects/spinesUtils/spinesUtils/asserts/_inspect.py in ?(*args, **kwargs)
-        194             if mismatched_params:
-        195                 error_msg = self.build_type_error_msg(mismatched_params)
-        196                 raise ParametersTypeError(error_msg)
-        197 
-    --> 198             return func(**kwargs)
-    
-
-    ~/projects/spinesUtils/spinesUtils/asserts/_inspect.py in ?(*args, **kwargs)
-        256             if mismatched_params:
-        257                 error_msg = self.build_values_error_msg(mismatched_params)
-        258                 raise ParametersValueError(error_msg)
-        259 
-    --> 260             return func(**kwargs)
-    
-
-    ~/projects/spinesUtils/spinesUtils/io/_data.py in ?(fp, sep, chunk_size, transform2low_mem, turbo_method, encoding, verbose, **read_csv_kwargs)
-        100 
-        101     if chunk_size:
-        102         df = read_text(fp)
-        103     else:
-    --> 104         df = turbo_reader(fp, turbo_method)
-        105 
-        106     if transform2low_mem:
-        107         from ..preprocessing import transform_dtypes_low_mem
-
-
-    ~/projects/spinesUtils/spinesUtils/io/_data.py in ?(fpath, tm)
-         65     def turbo_reader(fpath, tm):
-         66         if tm == 'polars':
-         67             from polars import read_csv
-    ---> 68             return read_csv(fpath, separator=sep, encoding=encoding, **read_csv_kwargs).to_pandas()
-         69 
-         70         if tm == 'pyarrow':
-         71             from pyarrow.csv import read_csv, ParseOptions, ReadOptions
-
-
-    ~/miniconda3/envs/dev/lib/python3.11/site-packages/polars/io/csv/functions.py in ?(source, has_header, columns, new_columns, separator, comment_char, quote_char, skip_rows, dtypes, schema, null_values, missing_utf8_is_empty_string, ignore_errors, try_parse_dates, n_threads, infer_schema_length, batch_size, n_rows, encoding, low_memory, rechunk, use_pyarrow, storage_options, skip_rows_after_header, row_count_name, row_count_offset, sample_size, eol_char, raise_if_empty, truncate_ragged_lines)
-        362         use_pyarrow=False,
-        363         raise_if_empty=raise_if_empty,
-        364         **storage_options,
-        365     ) as data:
-    --> 366         df = pl.DataFrame._read_csv(
-        367             data,
-        368             has_header=has_header,
-        369             columns=columns if columns else projection,
-
-
-    ~/miniconda3/envs/dev/lib/python3.11/site-packages/polars/dataframe/frame.py in ?(cls, source, has_header, columns, separator, comment_char, quote_char, skip_rows, dtypes, schema, null_values, missing_utf8_is_empty_string, ignore_errors, try_parse_dates, n_threads, infer_schema_length, batch_size, n_rows, encoding, low_memory, rechunk, skip_rows_after_header, row_count_name, row_count_offset, sample_size, eol_char, raise_if_empty, truncate_ragged_lines)
-        766                 )
-        767 
-        768         projection, columns = handle_projection_columns(columns)
-        769 
-    --> 770         self._df = PyDataFrame.read_csv(
-        771             source,
-        772             infer_schema_length,
-        773             batch_size,
-
-
-    FileNotFoundError: No such file or directory: /path/to/your/file.csv
-
-
 ## Classifiers for imbalanced data
 
 
 ```python
 from spinesUtils.models import MultiClassBalanceClassifier
 ```
 
@@ -527,27 +427,14 @@
 df_insight
 ```
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>total</th>
       <th>na</th>
       <th>naPercent</th>
@@ -1193,27 +1080,14 @@
     (8000000, 26) (1000000, 26) (1000000, 26)
 
 
 
 
 
 <div>
-<style scoped>
-    .dataframe tbody tr th:only-of-type {
-        vertical-align: middle;
-    }
-
-    .dataframe tbody tr th {
-        vertical-align: top;
-    }
-
-    .dataframe thead th {
-        text-align: right;
-    }
-</style>
 <table border="1" class="dataframe">
   <thead>
     <tr style="text-align: right;">
       <th></th>
       <th>b</th>
       <th>c</th>
       <th>d</th>
```

### Comparing `spinesUtils-0.4.0/spinesUtils.egg-info/SOURCES.txt` & `spinesutils-0.4.1/spinesUtils.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,11 +21,10 @@
 spinesUtils/feature_tools/_feature_tools.py
 spinesUtils/io/__init__.py
 spinesUtils/io/_data.py
 spinesUtils/models/__init__.py
 spinesUtils/models/imbalanced_classifier.py
 spinesUtils/preprocessing/__init__.py
 spinesUtils/preprocessing/_compress_memory.py
-spinesUtils/preprocessing/_data_shape.py
 spinesUtils/preprocessing/_split_tools.py
 spinesUtils/utils/__init__.py
 spinesUtils/utils/_utils.py
```

