# Comparing `tmp/timepulse-0.2.0.tar.gz` & `tmp/timepulse-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timepulse-0.2.0.tar", last modified: Fri Dec 15 13:43:49 2023, max compression
+gzip compressed data, was "timepulse-0.3.0.tar", last modified: Mon Apr 29 12:00:20 2024, max compression
```

## Comparing `timepulse-0.2.0.tar` & `timepulse-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.727013 timepulse-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-15 13:43:38.000000 timepulse-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-12-15 13:43:49.727013 timepulse-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2023-12-15 13:43:38.000000 timepulse-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.723013 timepulse-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:38.000000 timepulse-0.2.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-15 13:43:49.727013 timepulse-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2023-12-15 13:43:38.000000 timepulse-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.723013 timepulse-0.2.0/timepulse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.723013 timepulse-0.2.0/timepulse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/data/data_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.723013 timepulse-0.2.0/timepulse/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.727013 timepulse-0.2.0/timepulse/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/models/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7776 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/models/nbeats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/models/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/models/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.727013 timepulse-0.2.0/timepulse/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/processing/min_max_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/processing/standard_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.727013 timepulse-0.2.0/timepulse/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2023-12-15 13:43:38.000000 timepulse-0.2.0/timepulse/utils/splits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 13:43:49.723013 timepulse-0.2.0/timepulse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2023-12-15 13:43:49.000000 timepulse-0.2.0/timepulse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-12-15 13:43:49.000000 timepulse-0.2.0/timepulse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 13:43:49.000000 timepulse-0.2.0/timepulse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-15 13:43:49.000000 timepulse-0.2.0/timepulse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 13:43:49.000000 timepulse-0.2.0/timepulse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-12-15 13:43:49.000000 timepulse-0.2.0/timepulse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-15 13:43:49.000000 timepulse-0.2.0/timepulse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.956143 timepulse-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-29 12:00:04.000000 timepulse-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-29 12:00:20.956143 timepulse-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-04-29 12:00:04.000000 timepulse-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.952143 timepulse-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:04.000000 timepulse-0.3.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-29 12:00:20.956143 timepulse-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-29 12:00:04.000000 timepulse-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.952143 timepulse-0.3.0/timepulse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.956143 timepulse-0.3.0/timepulse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/data/data_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.956143 timepulse-0.3.0/timepulse/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.956143 timepulse-0.3.0/timepulse/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/models/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/models/nbeats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/models/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/models/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.956143 timepulse-0.3.0/timepulse/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/processing/min_max_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/processing/standard_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.956143 timepulse-0.3.0/timepulse/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-29 12:00:04.000000 timepulse-0.3.0/timepulse/utils/splits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:00:20.956143 timepulse-0.3.0/timepulse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-29 12:00:20.000000 timepulse-0.3.0/timepulse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-29 12:00:20.000000 timepulse-0.3.0/timepulse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:00:20.000000 timepulse-0.3.0/timepulse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 12:00:20.000000 timepulse-0.3.0/timepulse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:00:20.000000 timepulse-0.3.0/timepulse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-29 12:00:20.000000 timepulse-0.3.0/timepulse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 12:00:20.000000 timepulse-0.3.0/timepulse.egg-info/top_level.txt
```

### Comparing `timepulse-0.2.0/LICENSE.md` & `timepulse-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `timepulse-0.2.0/setup.py` & `timepulse-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="timepulse",
-    version="0.2.0",
-    description="A set of tools to help with timeseries flow",
+    version="0.3.0",
+    description="A set of algorithms to help with timeseries flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="SQUAREDEV BV",
     author_email="hello@squaredev.io",
     url="https://github.com/squaredev-io/timepulse",
     packages=find_packages(exclude=("tests", "docs")),
     install_requires=[
@@ -35,15 +35,15 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",  # Specify which py version you support
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     python_requires=">=3.9",  # Minimum version requirement of the package
-    keywords="timeseries tools ml flow python machine learning",  # Short descriptors for your package
+    keywords="timeseries algorithms ml flow ai python machine learning",  # Short descriptors for your package
     package_data={},
     entry_points={
         "console_scripts": [
             "timepulse_cli=timepulse.cli:main",  # This allows you to create a command-line script
         ],
     },
     include_package_data=True,
```

### Comparing `timepulse-0.2.0/timepulse/data/data_collection.py` & `timepulse-0.3.0/timepulse/data/data_collection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,95 @@
 import pandas as pd
 import re, os
 import holidays
 from typing import Literal, List
 
 
-def fetch_stringency_index(country: Literal["Italy", "Spain"], period: Literal["D", "M"] = "M") -> pd.DataFrame:
+def fetch_stringency_index(
+    country: str, period: Literal["D", "M"] = "M"
+) -> pd.DataFrame:
     """
     Fetches and processes stringency index data for the specified country and period.
 
     Parameters:
-    - country (Literal["Italy", "Spain"]): The name of the country for which the stringency index data is fetched.
-    - period (Literal["D", "M"], optional): The time period for data resampling, either "D" for daily or "M" for monthly.
-                                             Defaults to "M".
+    - country (str): The name of the country for which the
+    stringency index data is fetched.
+    - period (Literal["D", "M"], optional): The time period for data resampling,
+    either "D" for daily or "M" for monthly. Defaults to "M".
 
     Returns:
     - pd.DataFrame: Processed DataFrame containing the stringency index data with date-wise categories.
 
     Example:
     >>> fetch_stringency_index("Italy")
     """
-    stringency_index_avg_url = (
-        "https://raw.githubusercontent.com/OxCGRT/covid-policy-tracker/master/data/timeseries/stringency_index_avg.csv"
-    )
+    stringency_index_avg_url = "https://raw.githubusercontent.com/OxCGRT/covid-policy-tracker/master/data/timeseries/stringency_index_avg.csv"
     strigency_index_df = pd.read_csv(stringency_index_avg_url)
-    strigency_index_df = strigency_index_df[strigency_index_df["country_name"] == country]
+    strigency_index_df = strigency_index_df[
+        strigency_index_df["country_name"] == country
+    ]
 
     # Define a regular expression pattern to match the date format
     date_pattern = r"(\d{2})([A-Za-z]{3})(\d{4})"
-    date_columns = [col for col in strigency_index_df.columns if re.fullmatch(date_pattern, col)]
+    date_columns = [
+        col for col in strigency_index_df.columns if re.fullmatch(date_pattern, col)
+    ]
 
     strigency_index_df = strigency_index_df[date_columns]
     strigency_index_df = strigency_index_df.fillna(0)
 
-    strigency_index_df = pd.melt(strigency_index_df, id_vars=None, var_name="Date", value_name="stringency_index")
+    strigency_index_df = pd.melt(
+        strigency_index_df, id_vars=None, var_name="Date", value_name="stringency_index"
+    )
 
-    strigency_index_df["Date"] = pd.to_datetime(strigency_index_df["Date"], format="%d%b%Y").dt.strftime("%Y-%m-%d")
+    strigency_index_df["Date"] = pd.to_datetime(
+        strigency_index_df["Date"], format="%d%b%Y"
+    ).dt.strftime("%Y-%m-%d")
     strigency_index_df["Date"] = pd.to_datetime(strigency_index_df["Date"])
 
     strigency_index_df = strigency_index_df.sort_values(by="Date")
     strigency_index_df = strigency_index_df.set_index("Date")
 
     # Define bin edges and labels
     bin_edges = [-1, 33.0, 66.0, 110.0]  # Example boundaries for low, medium, high
     bin_labels = [0, 1, 2]
 
     strigency_index_df["stringency_category"] = pd.cut(
         strigency_index_df["stringency_index"], bins=bin_edges, labels=bin_labels
     )
 
-    strigency_index_df = strigency_index_df.resample(period).agg({"stringency_category": lambda x: x.mode().iloc[0]})
+    strigency_index_df = strigency_index_df.resample(period).agg(
+        {"stringency_category": lambda x: x.mode().iloc[0]}
+    )
     strigency_index_df = strigency_index_df.fillna(0)
 
     return strigency_index_df
 
 
-def fetch_holidays(years: List, country_code: Literal["IT", "ES"], period: Literal["D", "M"] = "M") -> pd.DataFrame:
+def fetch_holidays(
+    years: List[int], country_code: str, period: Literal["D", "M"] = "M"
+) -> pd.DataFrame:
     """
     Fetches and processes holidays data for the specified country and period.
 
     Parameters:
     - years (List): A list of years for which holidays data is fetched.
-    - country_code (Literal["IT", "ES"]): The country code for the country of interest.
+    - country_code (str): The country code for the country of interest.
     - period (Literal["D", "M"], optional): The time period for data resampling, either "D" for daily or "M" for monthly.
                                              Defaults to "M".
 
     Returns:
     - pd.DataFrame: Processed DataFrame containing the total number of holidays for each date.
 
     Example:
     >>> fetch_holidays([2021, 2022], "IT")
     """
     holidays_dict = holidays.country_holidays(country_code, years=years)
     holidays_df = pd.DataFrame(
-        {"total_holidays": [1 for _ in range(len(holidays_dict.keys()))]}, index=holidays_dict.keys()
+        {"total_holidays": [1 for _ in range(len(holidays_dict.keys()))]},
+        index=holidays_dict.keys(),
     )
     holidays_df.index.name = "Date"
     holidays_df.index = pd.to_datetime(holidays_df.index)
     holidays_df = holidays_df.resample(period).agg({"total_holidays": "sum"})
     holidays_df = holidays_df.fillna(0)
     return holidays_df
```

### Comparing `timepulse-0.2.0/timepulse/metrics/regression_metrics.py` & `timepulse-0.3.0/timepulse/metrics/regression_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,8 +88,16 @@
     mse = calculate_mse(y_true, y_pred)
     rmse = calculate_rmse(y_true, y_pred)
     mape = calculate_mape(y_true, y_pred)
     smape = calculate_smape(y_true, y_pred)
     mase = calculate_mase(y_true, y_pred)
     r2 = calculate_r2(y_true, y_pred)
 
-    return {"mae": mae, "mse": mse, "rmse": rmse, "mape": mape, "smape": smape, "mase": mase, "r2_score": r2}
+    return {
+        "mae": mae,
+        "mse": mse,
+        "rmse": rmse,
+        "mape": mape,
+        "smape": smape,
+        "mase": mase,
+        "r2_score": r2,
+    }
```

### Comparing `timepulse-0.2.0/timepulse/models/lstm.py` & `timepulse-0.3.0/timepulse/models/lstm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from timepulse.utils.models import create_early_stopping
 from timepulse.processing.min_max_scaler import MinMaxScalerWrapper
 import tensorflow as tf
-import pandas as pd
 import numpy as np
 from typing import List, Optional, Tuple, Type
 
 
 class LSTM:
     def __init__(
         self,
@@ -35,21 +34,35 @@
             [
                 tf.keras.layers.LSTM(self.n_neurons, input_shape=self.input_shape),
                 tf.keras.layers.Dropout(self.dropout_rate),
                 tf.keras.layers.Dense(self.horizon),
             ]
         )
 
-    def compile(self, loss: str = "mean_squared_error", learning_rate: float = 0.001) -> None:
-        self.model.compile(loss=loss, optimizer=tf.keras.optimizers.legacy.Adam(learning_rate=learning_rate))
+    def compile(
+        self, loss: str = "mean_squared_error", learning_rate: float = 0.001
+    ) -> None:
+        self.model.compile(
+            loss=loss,
+            optimizer=tf.keras.optimizers.legacy.Adam(learning_rate=learning_rate),
+        )
 
-    def fit(self, X_train: np.array, y_train: np.array, X_val: np.array, y_val: np.array, verbose: int = 0) -> None:
+    def fit(
+        self,
+        X_train: np.array,
+        y_train: np.array,
+        X_val: np.array,
+        y_val: np.array,
+        verbose: int = 0,
+    ) -> None:
         if self.scaler_X is not None:
             X_train = self.scaler_X.fit_transform_X(X_train)
-            y_train = self.scaler_y.fit_transform_y(y_train.reshape(len(y_train), 1)).flatten()
+            y_train = self.scaler_y.fit_transform_y(
+                y_train.reshape(len(y_train), 1)
+            ).flatten()
             X_val = self.scaler_X.transform_X(X_val)
             y_val = self.scaler_y.transform_y(y_val.reshape(len(y_val), 1)).flatten()
         X_train_reshaped = np.reshape(X_train, (X_train.shape[0], 1, X_train.shape[1]))
         X_val_reshaped = np.reshape(X_val, (X_val.shape[0], 1, X_val.shape[1]))
         self.model.fit(
             X_train_reshaped,
             y_train,
```

### Comparing `timepulse-0.2.0/timepulse/models/nbeats.py` & `timepulse-0.3.0/timepulse/models/nbeats.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,16 +50,20 @@
     ) -> None:
         super().__init__(**kwargs)
         self.input_size = input_size
         self.theta_size = theta_size
         self.horizon = horizon
         self.n_neurons = n_neurons
         self.n_layers = n_layers
-        self.hidden = [tf.keras.layers.Dense(n_neurons, activation="relu") for _ in range(n_layers)]
-        self.theta_layer = tf.keras.layers.Dense(theta_size, activation="linear", name="theta")
+        self.hidden = [
+            tf.keras.layers.Dense(n_neurons, activation="relu") for _ in range(n_layers)
+        ]
+        self.theta_layer = tf.keras.layers.Dense(
+            theta_size, activation="linear", name="theta"
+        )
 
     def call(self, inputs: np.array) -> Tuple[np.array, np.array]:
         """
         Forward pass through the NBeatsBlock.
 
         Parameters
         ----------
@@ -151,16 +155,20 @@
         n_neurons: int = 512,
         n_layers: int = 4,
         n_stacks: int = 30,
         epochs: int = 5000,
         batch_size: int = 1024,
         scaler_class: Type = MinMaxScalerWrapper(),
         callbacks: List = [
-            tf.keras.callbacks.ReduceLROnPlateau(monitor="val_loss", patience=100, verbose=0),
-            create_early_stopping(monitor="val_loss", patience=200, restore_best_weights=True),
+            tf.keras.callbacks.ReduceLROnPlateau(
+                monitor="val_loss", patience=100, verbose=0
+            ),
+            create_early_stopping(
+                monitor="val_loss", patience=200, restore_best_weights=True
+            ),
         ],
         **kwargs: Dict,
     ) -> None:
         super().__init__(**kwargs)
         self.input_size = window_size * horizon
         self.theta_size = window_size * horizon + horizon
         self.window_size = window_size
@@ -183,35 +191,59 @@
             n_layers=n_layers,
             name="InitialBlock",
         )
 
     def build(self) -> None:
         stack_input = tf.keras.layers.Input(shape=(self.input_size), name="stack_input")
         backcast, forecast = self.initial_block(stack_input)
-        residuals = tf.keras.layers.subtract([stack_input, backcast], name="subtract_00")
+        residuals = tf.keras.layers.subtract(
+            [stack_input, backcast], name="subtract_00"
+        )
         for i in range(self.n_stacks - 1):
             backcast, block_forecast = NBeatsBlock(
                 input_size=self.input_size,
                 theta_size=self.theta_size,
                 horizon=self.horizon,
                 n_neurons=self.n_neurons,
                 n_layers=self.n_layers,
                 name=f"NBeatsBlock_{i}",
             )(residuals)
-            residuals = tf.keras.layers.subtract([residuals, backcast], name=f"subtract_{i}")
+            residuals = tf.keras.layers.subtract(
+                [residuals, backcast], name=f"subtract_{i}"
+            )
             forecast = tf.keras.layers.add([forecast, block_forecast], name=f"add_{i}")
-        self.model = tf.keras.Model(inputs=stack_input, outputs=forecast, name=self.model_name)
+        self.model = tf.keras.Model(
+            inputs=stack_input, outputs=forecast, name=self.model_name
+        )
 
-    def compile(self, loss: str = "mae", learning_rate: float = 0.001, metrics: List = ["mae", "mse"]) -> None:
-        self.model.compile(loss=loss, optimizer=tf.keras.optimizers.legacy.Adam(learning_rate), metrics=metrics)
+    def compile(
+        self,
+        loss: str = "mae",
+        learning_rate: float = 0.001,
+        metrics: List = ["mae", "mse"],
+    ) -> None:
+        self.model.compile(
+            loss=loss,
+            optimizer=tf.keras.optimizers.legacy.Adam(learning_rate),
+            metrics=metrics,
+        )
 
-    def fit(self, X_train: np.array, y_train: np.array, X_val: np.array, y_val: np.array, verbose: int = 0) -> None:
+    def fit(
+        self,
+        X_train: np.array,
+        y_train: np.array,
+        X_val: np.array,
+        y_val: np.array,
+        verbose: int = 0,
+    ) -> None:
         if self.scaler_X is not None:
             X_train = self.scaler_X.fit_transform_X(X_train)
-            y_train = self.scaler_y.fit_transform_y(y_train.reshape(len(y_train), 1)).flatten()
+            y_train = self.scaler_y.fit_transform_y(
+                y_train.reshape(len(y_train), 1)
+            ).flatten()
             X_val = self.scaler_X.transform_X(X_val)
             y_val = self.scaler_y.transform_y(y_val.reshape(len(y_val), 1)).flatten()
         self.model.fit(
             X_train,
             y_train,
             epochs=self.epochs,
             validation_data=(X_val, y_val),
```

### Comparing `timepulse-0.2.0/timepulse/models/nn.py` & `timepulse-0.3.0/timepulse/models/nn.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,31 @@
         if self.n_neurons1 is not None:
             layers.append(tf.keras.layers.Dropout(self.dropout_rate))
             layers.append(tf.keras.layers.Dense(self.n_neurons1, activation="relu"))
         layers.append(tf.keras.layers.Dense(self.horizon))
         self.model = tf.keras.Sequential(layers, name=self.model_name)
 
     def compile(self, loss: str = "mae", learning_rate: float = 0.001) -> None:
-        self.model.compile(loss=loss, optimizer=tf.keras.optimizers.legacy.Adam(learning_rate))
+        self.model.compile(
+            loss=loss, optimizer=tf.keras.optimizers.legacy.Adam(learning_rate)
+        )
 
-    def fit(self, X_train: np.array, y_train: np.array, X_val: np.array, y_val: np.array, verbose: int = 0) -> None:
+    def fit(
+        self,
+        X_train: np.array,
+        y_train: np.array,
+        X_val: np.array,
+        y_val: np.array,
+        verbose: int = 0,
+    ) -> None:
         if self.scaler_X is not None:
             X_train = self.scaler_X.fit_transform_X(X_train)
-            y_train = self.scaler_y.fit_transform_y(y_train.reshape(len(y_train), 1)).flatten()
+            y_train = self.scaler_y.fit_transform_y(
+                y_train.reshape(len(y_train), 1)
+            ).flatten()
             X_val = self.scaler_X.transform_X(X_val)
             y_val = self.scaler_y.transform_y(y_val.reshape(len(y_val), 1)).flatten()
         self.model.fit(
             X_train,
             y_train,
             epochs=self.epochs,
             batch_size=self.batch_size,
```

### Comparing `timepulse-0.2.0/timepulse/models/xgboost.py` & `timepulse-0.3.0/timepulse/models/xgboost.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,50 @@
 import numpy as np
 import joblib
 import os
 from typing import Type, Dict
 
 
 class XGBoostRegressor:
-    def __init__(self, scaler_class: Type = MinMaxScalerWrapper(), **kwargs: Dict) -> None:
+    def __init__(
+        self, scaler_class: Type = MinMaxScalerWrapper(), **kwargs: Dict
+    ) -> None:
         self.params = kwargs
         self.scaler_X = scaler_class
         self.scaler_y = scaler_class
         self.model_name = f"xgboost_model"
         self.model = None
 
     def build(self) -> None:
         if self.params:
             self.model = XGBRegressor()
         else:
             self.model = XGBRegressor(**self.params)
 
-    def fit(self, X_train: np.array, y_train: np.array, X_val: np.array, y_val: np.array, verbose: int = 0) -> None:
+    def fit(
+        self,
+        X_train: np.array,
+        y_train: np.array,
+        X_val: np.array,
+        y_val: np.array,
+        verbose: int = 0,
+    ) -> None:
         if self.scaler_X is not None:
             X_train = self.scaler_X.fit_transform_X(X_train)
-            y_train = self.scaler_y.fit_transform_y(y_train.reshape(len(y_train), 1)).flatten()
+            y_train = self.scaler_y.fit_transform_y(
+                y_train.reshape(len(y_train), 1)
+            ).flatten()
             X_val = self.scaler_X.transform_X(X_val)
             y_val = self.scaler_y.transform_y(y_val.reshape(len(y_val), 1)).flatten()
-        self.model.fit(X_train, y_train, eval_set=[(X_train, y_train), (X_val, y_val)], verbose=verbose)
+        self.model.fit(
+            X_train,
+            y_train,
+            eval_set=[(X_train, y_train), (X_val, y_val)],
+            verbose=verbose,
+        )
 
     def predict(self, X_test: np.array) -> None:
         if self.scaler_X is not None:
             X_test = self.scaler_X.transform_X(X_test)
             y_pred = self.model.predict(X_test)
             y_pred = self.scaler_y.inverse_transform_y(y_pred.reshape(-1, 1))
         else:
```

### Comparing `timepulse-0.2.0/timepulse/processing/min_max_scaler.py` & `timepulse-0.3.0/timepulse/processing/min_max_scaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from sklearn.preprocessing import MinMaxScaler
 import numpy as np
 
+
 class MinMaxScalerWrapper:
     def __init__(self) -> None:
         self.scaler_X = MinMaxScaler()
         self.scaler_y = MinMaxScaler()
 
     def fit_transform_X(self, data: np.array) -> np.array:
         return self.scaler_X.fit_transform(data)
```

### Comparing `timepulse-0.2.0/timepulse/processing/standard_scaler.py` & `timepulse-0.3.0/timepulse/processing/standard_scaler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from sklearn.preprocessing import StandardScaler
 import numpy as np
 
+
 class StandardScalerWrapper:
     def __init__(self) -> None:
         self.scaler_X = StandardScaler()
         self.scaler_y = StandardScaler()
 
     def fit_transform_X(self, data: np.array) -> np.array:
         return self.scaler_X.fit_transform(data)
```

### Comparing `timepulse-0.2.0/timepulse/utils/models.py` & `timepulse-0.3.0/timepulse/utils/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import tensorflow as tf
 import os
 import numpy as np
 from typing import Tuple, Dict, Type
 from timepulse.metrics.regression_metrics import evaluate_preds
 
 
-def create_model_checkpoint(model_name: str, save_path: str = "storage") -> tf.keras.callbacks.ModelCheckpoint:
+def create_model_checkpoint(
+    model_name: str, save_path: str = "storage"
+) -> tf.keras.callbacks.ModelCheckpoint:
     """
     Creates a ModelCheckpoint callback for saving the best model during training.
 
     Parameters
     ----------
     model_name : str
         Name of the model.
@@ -53,15 +55,20 @@
     """
     return tf.keras.callbacks.EarlyStopping(
         monitor=monitor, patience=patience, restore_best_weights=restore_best_weights
     )
 
 
 def run_model(
-    model_instance: Type, X_train: np.array, y_train: np.array, X_test: np.array, y_test: np.array, verbose=0
+    model_instance: Type,
+    X_train: np.array,
+    y_train: np.array,
+    X_test: np.array,
+    y_test: np.array,
+    verbose=0,
 ) -> Tuple[np.array, Dict]:
     """
     Train and evaluate a Keras model.
 
     Parameters
     ----------
     model_instance : Type
```

### Comparing `timepulse-0.2.0/timepulse/utils/splits.py` & `timepulse-0.3.0/timepulse/utils/splits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 import pandas as pd
 from sklearn.model_selection import StratifiedShuffleSplit
 from typing import Union, Tuple
 
 
-def create_multivar_dataframe(base_df: pd.DataFrame, *additional_dfs: pd.DataFrame) -> pd.DataFrame:
+def create_multivar_dataframe(
+    base_df: pd.DataFrame, *additional_dfs: pd.DataFrame, interval: str = "M"
+) -> pd.DataFrame:
     """
     Create a multivariate DataFrame by merging a base DataFrame with additional DataFrames based on a date range.
 
     Parameters:
     - base_df (pd.DataFrame): The base DataFrame.
     - additional_dfs (list of pd.DataFrame): List of additional DataFrames to be merged based on the date range.
 
@@ -19,27 +21,27 @@
     - multivar_df = create_multivar_dataframe(df, monthly_strigency_index_df, monthly_holidays_df, monthly_weather_history_df)
     """
     # Find the minimum and maximum dates from the base DataFrame
     min_date = base_df.index.min()
     max_date = base_df.index.max()
 
     # Create a monthly date range with the last day of each month
-    date_range = pd.date_range(start=min_date, end=max_date, freq="M")
+    date_range = pd.date_range(start=min_date, end=max_date, freq=interval)
 
     # Create a DataFrame with the date range to ensure complete coverage
     complete_date_range_df = pd.DataFrame({"Date": date_range})
     complete_date_range_df = complete_date_range_df.set_index(["Date"])
 
     # Initialize the multivariate DataFrame with the base DataFrame
     multivar_df = base_df
 
     # Merge additional DataFrames based on the date range
     for additional_df in additional_dfs:
         # Merge with the complete date range DataFrame to ensure all dates are included
-        merged_df = pd.merge(complete_date_range_df, additional_df, on="Date", how="left")
+        merged_df = pd.merge(complete_date_range_df, additional_df, left_index=True, right_index=True, how="left")
         # Fill missing values with 0 and convert to integer
         merged_df = merged_df.fillna(0).astype(int)
         # Perform the merge with the multivariate DataFrame
         multivar_df = pd.merge(multivar_df, merged_df, left_index=True, right_index=True, how="left")
 
     return multivar_df
```

### Comparing `timepulse-0.2.0/timepulse.egg-info/SOURCES.txt` & `timepulse-0.3.0/timepulse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

