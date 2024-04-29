# Comparing `tmp/twinlab-2.5.0.tar.gz` & `tmp/twinlab-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinlab-2.5.0.tar", max compression
+gzip compressed data, was "twinlab-2.6.0.tar", max compression
```

## Comparing `twinlab-2.5.0.tar` & `twinlab-2.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1031 2024-03-11 09:16:22.945659 twinlab-2.5.0/LICENSE
--rw-r--r--   0        0        0      555 2024-03-18 13:45:32.588743 twinlab-2.5.0/README.md
--rw-r--r--   0        0        0     1802 2024-04-15 09:02:01.144244 twinlab-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1486 2024-04-11 10:18:35.345552 twinlab-2.5.0/twinlab/__init__.py
--rw-r--r--   0        0        0      171 2024-03-12 11:24:16.616707 twinlab-2.5.0/twinlab/_version.py
--rw-r--r--   0        0        0    13517 2024-03-20 17:24:42.877209 twinlab-2.5.0/twinlab/api.py
--rw-r--r--   0        0        0    44109 2024-04-11 10:18:35.345728 twinlab-2.5.0/twinlab/client.py
--rw-r--r--   0        0        0    10034 2024-04-11 10:18:35.345916 twinlab-2.5.0/twinlab/core.py
--rw-r--r--   0        0        0     8676 2024-04-11 10:18:35.346087 twinlab-2.5.0/twinlab/dataset.py
--rw-r--r--   0        0        0      829 2024-04-11 10:18:35.346314 twinlab-2.5.0/twinlab/distributions.py
--rw-r--r--   0        0        0    61723 2024-04-15 08:15:42.021188 twinlab-2.5.0/twinlab/emulator.py
--rw-r--r--   0        0        0     4876 2024-04-11 10:18:35.346907 twinlab-2.5.0/twinlab/helper.py
--rw-r--r--   0        0        0    29491 2024-04-11 10:18:35.347178 twinlab-2.5.0/twinlab/params.py
--rw-r--r--   0        0        0     1862 2024-04-09 17:31:34.286104 twinlab-2.5.0/twinlab/plotting.py
--rw-r--r--   0        0        0      668 2024-04-11 10:18:35.347422 twinlab-2.5.0/twinlab/prior.py
--rw-r--r--   0        0        0     1926 2024-04-11 10:18:35.347716 twinlab-2.5.0/twinlab/sampling.py
--rw-r--r--   0        0        0     1637 2024-03-12 11:24:16.626252 twinlab-2.5.0/twinlab/settings.py
--rw-r--r--   0        0        0     5233 2024-04-11 10:18:35.347832 twinlab-2.5.0/twinlab/utils.py
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 twinlab-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1031 2023-09-19 13:29:40.794269 twinlab-2.6.0/LICENSE
+-rw-r--r--   0        0        0     2657 2024-04-29 09:55:28.721775 twinlab-2.6.0/README.md
+-rw-r--r--   0        0        0     1759 2024-04-29 09:55:28.722058 twinlab-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1486 2024-04-25 10:08:03.722392 twinlab-2.6.0/twinlab/__init__.py
+-rw-r--r--   0        0        0      171 2023-09-19 13:29:40.807103 twinlab-2.6.0/twinlab/_version.py
+-rw-r--r--   0        0        0    14702 2024-04-29 09:55:28.777944 twinlab-2.6.0/twinlab/api.py
+-rw-r--r--   0        0        0    40736 2024-04-29 09:55:28.778517 twinlab-2.6.0/twinlab/client.py
+-rw-r--r--   0        0        0     9608 2024-04-29 09:55:28.778655 twinlab-2.6.0/twinlab/core.py
+-rw-r--r--   0        0        0     9256 2024-04-29 09:55:28.778932 twinlab-2.6.0/twinlab/dataset.py
+-rw-r--r--   0        0        0      843 2024-04-29 09:55:28.779188 twinlab-2.6.0/twinlab/distributions.py
+-rw-r--r--   0        0        0    66335 2024-04-29 09:55:28.779451 twinlab-2.6.0/twinlab/emulator.py
+-rw-r--r--   0        0        0     4876 2024-04-15 15:01:48.559474 twinlab-2.6.0/twinlab/helper.py
+-rw-r--r--   0        0        0    29378 2024-04-29 09:55:28.779621 twinlab-2.6.0/twinlab/params.py
+-rw-r--r--   0        0        0     1862 2024-03-13 15:41:11.184579 twinlab-2.6.0/twinlab/plotting.py
+-rw-r--r--   0        0        0      659 2024-04-29 09:55:28.779734 twinlab-2.6.0/twinlab/prior.py
+-rw-r--r--   0        0        0     1926 2024-04-15 15:01:48.560048 twinlab-2.6.0/twinlab/sampling.py
+-rw-r--r--   0        0        0     1637 2024-01-11 11:15:46.668160 twinlab-2.6.0/twinlab/settings.py
+-rw-r--r--   0        0        0     5669 2024-04-29 09:55:28.779852 twinlab-2.6.0/twinlab/utils.py
+-rw-r--r--   0        0        0     4081 1970-01-01 00:00:00.000000 twinlab-2.6.0/PKG-INFO
```

### Comparing `twinlab-2.5.0/LICENSE` & `twinlab-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twinlab-2.5.0/pyproject.toml` & `twinlab-2.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "twinlab"
-version = "2.5.0"
-description = "Python interface for twinLab machine-learning in the cloud."
+version = "2.6.0"
+description = "twinLab - Probabilistic Machine Learning for Engineers"
 license = "MIT"
-homepage = "https://www.digilab.co.uk"
-repository = "https://github.com/digiLab-ai/twinLab-client"
-documentation = "https://digilab-ai.github.io/twinLab"
+homepage = "https://twinlab.ai"
+documentation = "https://twinlab.ai"
 authors = ["digiLab Solutions Ltd. <info@digilab.co.uk>"]
 maintainers = [
     "Alexander Mead <alexander@digilab.co.uk>",
     "Freddy Wordingham <freddy@digilab.co.uk>",
     "Michelle Fabienne Bieger <michelle@digilab.co.uk>",
     "Huy Nguyen <huy@digilab.co.uk>",
     "Joe Schaefer <joe@digiLab.co.uk>",
     "Jodeci Pugsley <jodeci@digilab.co.uk>",
     "Sai Aakash Ramesh<sai-aakash@digilab.co.uk>",
     "Sergio Chavez <sergio@digilab.co.uk>",
     "Micol Greta Giannelli <micol@digilab.co.uk>",
     "Jasper Cantwell <jasper@digilab.co.uk>",
+    "Will Denby <will@digilab.co.uk>",
 ]
 keywords = ["machine-learning", "AI", "cloud", "twinLab", "digiLab"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 matplotlib = ">=3.7"
@@ -32,22 +32,22 @@
 pandas = [
     { version = "^1.5.3", python = ">=3.8,<3.9" },
     { version = "^2.0", python = ">=3.9,<3.13" },
 ]
 python-dotenv = "^1.0.0"
 requests = "^2.28.2"
 typeguard = "^4.0.0"
-pytest = "^7.4.3"
 setuptools = "^69.0.2"
 deprecated = "^1.2.14"
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^6.22.0"
 IPython = "^8.11"
 pytest = "^7.1.2"
+pytest-timeout = "^2.3.1"
 pytest-cov = "^3.0.0"
 pytest-regtest = "^1.5.1"
 pytest-regressions = "^2.5.0"
 
 # NOTE: This allows for better collection of the pytests
 # NOTE: Allows tests that have the same name but in different folders
 [tool.pytest.ini_options]
```

### Comparing `twinlab-2.5.0/twinlab/__init__.py` & `twinlab-2.6.0/twinlab/__init__.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.5.0/twinlab/api.py` & `twinlab-2.6.0/twinlab/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,27 @@
     status = response.status_code
     body = _get_response_body(response)
     return status, body
 
 
 @typechecked
 @check_status_code
+def generate_temp_upload_url(
+    dataset_id: str, verbose: Optional[bool] = False
+) -> Tuple[int, dict]:
+    url = f"{os.getenv('TWINLAB_URL')}/temp_upload_url/{dataset_id}"
+    headers = _create_headers(verbose=verbose)
+    response = requests.get(url, headers=headers)
+    status = response.status_code
+    body = _get_response_body(response)
+    return status, body
+
+
+@typechecked
+@check_status_code
 def process_uploaded_dataset(
     dataset_id: str, verbose: Optional[bool] = False
 ) -> Tuple[int, dict]:
     url = f"{os.getenv('TWINLAB_URL')}/datasets/{dataset_id}"
     headers = _create_headers(verbose=verbose)
     response = requests.post(url, headers=headers)
     status = response.status_code
@@ -188,14 +201,27 @@
     status = response.status_code
     body = _get_response_body(response)
     return status, body
 
 
 @typechecked
 @check_status_code
+def delete_temp_dataset(
+    dataset_id: str, verbose: Optional[bool] = False
+) -> Tuple[int, dict]:
+    url = f"{os.getenv('TWINLAB_URL')}/temp_datasets/{dataset_id}"
+    headers = _create_headers(verbose=verbose)
+    response = requests.delete(url, headers=headers)
+    status = response.status_code
+    body = _get_response_body(response)
+    return status, body
+
+
+@typechecked
+@check_status_code
 def view_data_model(
     model_id: str, dataset_type: str, verbose: Optional[bool] = False
 ) -> Tuple[int, dict]:
     url = f"{os.getenv('TWINLAB_URL')}/models/{model_id}/view_data_model"
     query_params = {"dataset_type": dataset_type}
     headers = _create_headers(verbose=verbose)
     response = requests.get(url, headers=headers, params=query_params)
@@ -342,21 +368,29 @@
     return status, body
 
 
 ### Synchronous endpoints ###
 
 
 def _use_request_body(
-    data_csv: Optional[str] = None, data_std_csv: Optional[str] = None, **kwargs
+    data_csv: Optional[str] = None,
+    data_std_csv: Optional[str] = None,
+    dataset_id: Optional[str] = None,
+    dataset_std_id: Optional[str] = None,
+    **kwargs,
 ) -> dict:
     request_body = {"kwargs": kwargs}
     if data_csv is not None:
         request_body["dataset"] = data_csv
     if data_std_csv is not None:
         request_body["dataset_std"] = data_std_csv
+    if dataset_id is not None:
+        request_body["dataset_id"] = dataset_id
+    if dataset_std_id is not None:
+        request_body["dataset_std_id"] = dataset_std_id
     return request_body
 
 
 @typechecked
 @check_status_code
 def use_model(
     model_id: str,
@@ -383,22 +417,26 @@
 @typechecked
 @check_status_code
 def use_request_model(
     model_id: str,
     method: str,
     data_csv: Optional[str] = None,
     data_std_csv: Optional[str] = None,
+    dataset_id: Optional[str] = None,
+    dataset_std_id: Optional[str] = None,
     processor: str = "cpu",
     verbose: bool = False,
     **kwargs,
 ) -> Tuple[int, dict]:
     url = f"{os.getenv('TWINLAB_URL')}/models/{model_id}/async/{method}"
     headers = _create_headers(verbose=verbose)
     headers["X-Processor"] = processor
-    request_body = _use_request_body(data_csv, data_std_csv, **kwargs)
+    request_body = _use_request_body(
+        data_csv, data_std_csv, dataset_id, dataset_std_id, **kwargs
+    )
     response = requests.post(url, headers=headers, json=request_body)
     status = response.status_code
     body = _get_response_body(response)
     return status, body
 
 
 @typechecked
```

### Comparing `twinlab-2.5.0/twinlab/core.py` & `twinlab-2.6.0/twinlab/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -226,44 +226,43 @@
             ['biscuits', 'gardening', 'new-emulator', 'my-emulator']
 
     """
 
     # Get the emulators dictionary from the response
     _, response = api.list_models(verbose=DEBUG)
     emulators = utils.get_value_from_body("model_information", response)
-
-    # Standardise dictionary for failed cases
-    for emulator in emulators:
-        if "run_time" not in emulator:
-            emulator["run_time"] = "NaN"
-        if "start_time" not in emulator:
-            emulator["start_time"] = "NaN"
+    emulator_list = utils.get_value_from_body("models", response)
 
     # Create dictionary of cuddly response
     status_dict = {
         "success": "Successfully trained emulators:",
         "in_progress": "Emulators currently training:",
         "failed": "Emulators that failed to train:",
+        "no_logging": "Emualtors trained prior to logging:",
     }
 
-    # Write out nicely in verbose mode
-    verbose_keys = ("model", "start_time", "run_time")
     if verbose:
-        for status, nice_status in status_dict.items():
-            emus = [emu for emu in emulators if emu["status"] == status]
-            # Sort through dictionary via success, in_progress, failed
-            emus = [dict((key, emu[key]) for key in verbose_keys) for emu in emus]
-            emus = sorted(emus, key=lambda d: d["start_time"])
-            # List models in order from starting time
+
+        for status in status_dict.keys():
+
+            emus = []
+            for i in emulators:
+                if i.get("status") == status:
+                    i.pop("status", None)
+                    emus.append(i)
+
+            if status != "no_logging":
+                emus = sorted(emus, key=lambda d: d["start_time"])
+
             if emus:
-                # Only print list if there are available emulators to list
-                print(nice_status)
+                print(status_dict[status])
                 pprint(emus)
-    # Return a simple list of trained emulators for backwards compatability
-    return [emulator["model"] for emulator in emulators]
+                print("\n")
+
+    return emulator_list
 
 
 @typechecked
 def list_example_datasets(verbose: bool = False) -> list:
     """List example datasets that are available on the twinLab cloud.
 
     These datasets can be downloaded and used for training emulators and other operations and are used in many of the examples in the documentation.
```

### Comparing `twinlab-2.5.0/twinlab/dataset.py` & `twinlab-2.6.0/twinlab/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -74,15 +74,14 @@
                 upload_url,
                 verbose=verbose,
                 check=settings.CHECK_DATASETS,
             )
             if verbose:
                 print("Processing dataset")
             _, response = api.process_uploaded_dataset(self.id, verbose=DEBUG)
-
         else:
             csv_string = utils.get_csv_string(df)
             _, response = api.upload_dataset(self.id, csv_string, verbose=DEBUG)
         if verbose:
             message = utils.get_message(response)
             print(message)
 
@@ -115,17 +114,22 @@
                 2                     2             1.000000
 
         """
         columns_string = ",".join(columns)
         _, response = api.analyse_dataset(
             self.id, columns=columns_string, verbose=DEBUG
         )
-
-        csv_string = utils.get_value_from_body("dataframe", response)
-        csv_string = io.StringIO(csv_string)
+        if response["dataframe"] is not None:
+            csv_string = utils.get_value_from_body("dataframe", response)
+            csv_string = io.StringIO(csv_string)
+        else:
+            df_url = utils.get_value_from_body("dataframe_url", response)
+            csv_string = utils.download_dataframe_from_presigned_url(df_url)
+            dataframe_name = utils.get_value_from_body("dataframe_name", response)
+            _, response = api.delete_temp_dataset(dataframe_name)
         df = pd.read_csv(csv_string, index_col=0, sep=",")
         if verbose:
             print("Variance Analysis:")
             print(df)
         return df
 
     @deprecated(
@@ -195,17 +199,20 @@
                 6  0.980764 -0.164966
                 7  0.684830 -0.960764
                 8  0.480932  0.340115
                 9  0.392118  0.845795
 
         """
         _, response = api.view_dataset(self.id, verbose=DEBUG)
-
-        csv_string = utils.get_value_from_body("dataset", response)
-        csv_string = io.StringIO(csv_string)
+        if response["dataset"] is not None:
+            csv_string = utils.get_value_from_body("dataset", response)
+            csv_string = io.StringIO(csv_string)
+        else:
+            df_url = utils.get_value_from_body("dataset_url", response)
+            csv_string = utils.download_dataframe_from_presigned_url(df_url)
         df = pd.read_csv(csv_string, sep=",")
         if verbose:
             print("Dataset:")
             print(df)
         return df
 
     @typechecked
```

### Comparing `twinlab-2.5.0/twinlab/distributions.py` & `twinlab-2.6.0/twinlab/distributions.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 @typechecked
 class DistributionMethods(Enum):
     UNIFORM = "uniform"
 
 
 @typechecked
-class Uniform:
+class Uniform(Distribution):
     """A one-dimensional continous uniform distribution between a minimum and maximum value.
 
     Args:
         min (float): The minimum value of the distribution.
         max (float): The maximum value of the distribution.
 
     """
```

### Comparing `twinlab-2.5.0/twinlab/emulator.py` & `twinlab-2.6.0/twinlab/emulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # Standard imports
 import io
 import json
+import sys
 import time
+import uuid
+
 from pprint import pprint
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 # Third-party imports
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from typeguard import typechecked
 
 # Project imports
-from . import api, utils
+from . import api, settings, utils
 from .dataset import Dataset
 from .params import (
     BenchmarkParams,
     CalibrateParams,
     DesignParams,
     PredictParams,
     RecommendParams,
@@ -54,19 +57,57 @@
     "get_calibration_curve": "benchmark",
     "predict": "predict",
     "sample": "sample",
     "get_candidate_points": "recommend",
     "solve_inverse": "calibrate",
 }
 
+ALLOWED_DATAFRAME_SIZE = 5.5 * int(
+    1e6
+)  # 5.5MB limit to stay safely (also to allow other variables and dataframes to flow through without making a fuss) within the 6MB limit for a Lambda response payload size
+
 ### Helper functions ###
 # TODO: Should these functions all have preceeding underscores?
 
 
 @typechecked
+def _upload_large_datasets(
+    df: pd.DataFrame, csv_string: str, method_prefix: str
+) -> Optional[str]:
+    df_id = str(uuid.uuid4())
+    if sys.getsizeof(csv_string) > ALLOWED_DATAFRAME_SIZE:
+        dataset_id = method_prefix + "_data_" + df_id
+        _, response = api.generate_temp_upload_url(dataset_id, verbose=DEBUG)
+        upload_url = utils.get_value_from_body("url", response)
+        utils.upload_dataframe_to_presigned_url(
+            df,
+            upload_url,
+            check=settings.CHECK_DATASETS,
+        )
+        return dataset_id
+    else:
+        return None
+
+
+@typechecked
+def _retrieve_dataframe_from_response(
+    response: dict,
+    dataframe_key: Optional[str] = "dataframe",
+    dataframe_url_key: Optional[str] = "dataframe_url",
+) -> io.StringIO:
+    if response[dataframe_key] is not None:
+        csv = utils.get_value_from_body(dataframe_key, response)
+        csv = io.StringIO(csv)
+    else:
+        data_url = utils.get_value_from_body(dataframe_url_key, response)
+        csv = utils.download_dataframe_from_presigned_url(data_url)
+    return csv
+
+
+@typechecked
 def _calculate_ping_time(elapsed_time: float) -> float:
     # This smoothly transitions between regular pinging at the initial ping time
     # to more drawn out pinging (expoential) as time goes on
     return PING_TIME_INITIAL + elapsed_time * PING_FRACTIONAL_INCREASE
 
 
 # TODO: Combine _wait_for_training_completion and _wait_for_job_completion
@@ -126,48 +167,34 @@
     else:
         message = "No response message in body"
     return message
 
 
 @typechecked
 def _process_csv(
-    csv: io.StringIO, method: str, verbose: bool = False
+    csv: io.StringIO, method: str
 ) -> Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]:
     if method == "predict":
         df = pd.read_csv(csv, sep=",")
         n = len(df.columns)
         df_mean, df_std = df.iloc[:, : n // 2], df.iloc[:, n // 2 :]
         df_std.columns = df_std.columns.str.removesuffix(" [std_dev]")
-        if verbose:
-            print("Mean predictions:")
-            print(df_mean)
-            print("Standard deviation predictions:")
-            print(df_std)
         return df_mean, df_std
     elif method == "sample":
         df_result = pd.read_csv(csv, header=[0, 1], sep=",")
-        if verbose:
-            print("Samples:")
-            print(df_result)
         return df_result
     elif method == "get_candidate_points":
         df = pd.read_csv(csv, sep=",")
-        if verbose:
-            print("Recommended points:")
-            print(df)
         return df
     elif method == "solve_inverse":
         df = pd.read_csv(csv, sep=",")
         df = df.set_index("Unnamed: 0")
         df.index.name = None
         if "Unnamed: 0.1" in df.columns:  # TODO: This seems like a nasty hack
             df = df.drop("Unnamed: 0.1", axis=1)
-        if verbose:
-            print("Calibration summary:")
-            print(df)
         return df
     else:
         raise ValueError(f"Method {method} not recognised")
 
 
 ### ###
 
@@ -187,15 +214,15 @@
             Be sure to double check which emulators have been created using .. autofunction:: `~list_emulator`.
     """
 
     @typechecked
     def __init__(self, id: str):
         self.id = id
 
-    # @typechecked # TODO: Typecheck does not seem to work with List[Prior]??
+    @typechecked
     def design(
         self,
         priors: List[Prior],
         num_points: int,
         params: DesignParams = DesignParams(),
         verbose: bool = False,
     ) -> pd.DataFrame:
@@ -214,37 +241,42 @@
 
         Example:
             .. code-block:: python
 
                 emulator = tl.Emulator("emulator_id")
 
                 my_priors = [
-                    tl.Prior("x1", tl.distribution.Uniform(0, 12)),
-                    tl.Prior("x2", tl.distribution.Uniform(0, 0.5)),
-                    tl.Prior("x3 ", tl.distribution.Uniform(0, 10)),
+                    tl.Prior("x1", tl.distributions.Uniform(0, 12)),
+                    tl.Prior("x2", tl.distributions.Uniform(0, 0.5)),
+                    tl.Prior("x3 ", tl.distributions.Uniform(0, 10)),
                 ]
 
                 initial_design = emulator.design(my_priors, 10)
 
         """
         # Convert priors to json so they can be passed through the API
-        priors = [prior.to_json() for prior in priors]
+        serialised_priors = [prior.to_json() for prior in priors]
 
         # Call the API function
         _, response = api.get_initial_design(
-            priors,
+            serialised_priors,
             params.sampling_method.to_json(),
             num_points,
             seed=params.seed,
             verbose=verbose,
         )
-
         # Get result from body of response
-        initial_design = utils.get_value_from_body("initial_design", response)
-        initial_design = io.StringIO(initial_design)
+        initial_design = _retrieve_dataframe_from_response(
+            response, "initial_design", "initial_design_url"
+        )
+        if (
+            "dataframe_name" in response.keys()
+            and response["dataframe_name"] is not None
+        ):
+            api.delete_temp_dataset(response["dataframe_name"])
 
         # Convert result which is a numpy array to pandas dataframe with correct column names
         initial_design_df = pd.read_csv(initial_design, sep=",")
 
         if verbose:
             print("Initial design:")
             print(initial_design_df)
@@ -295,14 +327,15 @@
 
         Example:
             .. code-block:: python
 
                 df = pd.DataFrame({"X": [1, 2, 3, 4], "y": [1, 4, 9, 16]})
                 dataset = tl.Dataset("my_dataset")
                 dataset.upload(df)
+                emulator = tl.Emulator("my_emulator")
                 emulator.train(dataset, ["X"], ["y"])
 
         """
 
         # Making a dictionary from TrainParams class
         if PROCESSOR == "gpu":
             print(
@@ -437,16 +470,17 @@
                 4  0.719469 -0.832518
                 5  0.423106  0.400669
                 6  0.980764 -0.164966
                 7  0.684830 -0.960764
 
         """
         _, response = api.view_data_model(self.id, dataset_type="train", verbose=DEBUG)
-        train_csv_string = utils.get_value_from_body("training_data", response)
-        train_csv_string = io.StringIO(train_csv_string)
+        train_csv_string = _retrieve_dataframe_from_response(
+            response, "training_data", "training_data_url"
+        )
         df_train = pd.read_csv(train_csv_string, sep=",", index_col=0)
         if verbose:
             print("Training data")
             pprint(df_train)
         return df_train
 
     @typechecked
@@ -470,16 +504,17 @@
 
                           x         y
                 0  0.480932  0.340115
                 1  0.392118  0.845795
 
         """
         _, response = api.view_data_model(self.id, dataset_type="test", verbose=DEBUG)
-        test_csv_string = utils.get_value_from_body("test_data", response)
-        test_csv_string = io.StringIO(test_csv_string)
+        test_csv_string = _retrieve_dataframe_from_response(
+            response, "test_data", "test_data_url"
+        )
         df_test = pd.read_csv(test_csv_string, sep=",", index_col=0)
         if verbose:
             print("Test data")
             pprint(df_test)
         return df_test
 
     def list_processes(self, verbose: bool = False) -> Dict[str, Dict]:
@@ -573,31 +608,49 @@
                 0   -0.730114  0.474193  0.046743  1.327620
                 1   -0.656061  0.505923  0.074198  1.289113
                 2   -0.579500  0.538610  0.100665  1.247405
                 3   -0.502726  0.574996  0.128068  1.205057
                 4   -0.428691  0.614687  0.157740  1.165903
 
         """
+        method = " "  # Error generated regarding "local variable referenced before asssignment" if not included
         _, response = api.list_processes_model(model_id=self.id, verbose=DEBUG)
+        method = " "  # TODO: This is a bad way to avoid a scope error for this variable
+
         for i in range(len(response["processes"])):
             if response["processes"][i]["process_id"] == process_id:
                 method = response["processes"][i]["method"]
         _, response = api.use_response_model(
             model_id=self.id,
             method=method,
             process_id=process_id,
             verbose=DEBUG,
         )
-        csv = utils.get_value_from_body("dataframe", response)
-        csv = io.StringIO(csv)
+
+        csv = _retrieve_dataframe_from_response(response)
         if method == "predict":
-            df_mean, df_std = _process_csv(csv, method, verbose=verbose)
+            df_mean, df_std = _process_csv(csv, method)
+            if verbose:
+                print("Mean predictions:")
+                print(df_mean)
+                print("Standard deviation predictions:")
+                print(df_std)
             return df_mean, df_std
         else:
-            df = _process_csv(csv, method, verbose=verbose)
+            df = _process_csv(csv, method)
+            if verbose:
+                if method == "sample":
+                    print("Samples:")
+                elif method == "get_candidate_points":
+                    print("Recommended points:")
+                elif method == "solve_inverse":
+                    print("Calibration summary:")
+                else:
+                    print("Process results:")
+                print(df)
             return df
 
     @typechecked
     def summarise(self, verbose: bool = False) -> dict:
         """Get a summary of a trained emulator on the twinLab cloud.
 
         This summary returns transformer diagnostics, with details about the input/output decomposition.
@@ -731,14 +784,15 @@
             if not params.combined_score:  # DataFrame
                 score = pd.read_csv(score, sep=",")
             if verbose:
                 print("Emulator Score:")
                 print(score)  # Could be pd.DataFrame or float
             return score
         else:
+            # TODO: Convert to warning!
             print(
                 "No test data was available for this emulator, so it cannot be scored."
             )
 
     @typechecked
     def benchmark(
         self,
@@ -795,14 +849,15 @@
         if csv is not None:
             df = pd.read_csv(csv, sep=",")
             if verbose:
                 print("Calibration curve:")
                 pprint(df)
             return df
         else:
+            # TODO: Convert to warning!
             print(
                 "No test data was available for this emulator, so it cannot be benchmarked."
             )
 
     @typechecked
     def predict(
         self,
@@ -861,33 +916,42 @@
             csv = self._use_method(
                 method=API_METHOD,
                 df=df,
                 **params.unpack_parameters(),
                 verbose=verbose,
             )
         else:
+            data_csv = utils.get_csv_string(df)
+            dataset_id = _upload_large_datasets(df, data_csv, API_METHOD)
+            if dataset_id is not None:
+                data_csv = None
             _, response = api.use_request_model(
                 model_id=self.id,
                 method=API_METHOD,
-                data_csv=utils.get_csv_string(df),
+                dataset_id=dataset_id,
+                data_csv=data_csv,
                 **params.unpack_parameters(),
                 processor=PROCESSOR,
                 verbose=DEBUG,
             )
             process_id = utils.get_value_from_body("process_id", response)
             if verbose:
                 print(f"Job {PROCESS_MAP[API_METHOD]} process ID: {process_id}")
             if not wait:
                 return process_id
             _, response = _wait_for_job_completion(
                 self.id, API_METHOD, process_id, verbose=verbose
             )
-            csv = utils.get_value_from_body("dataframe", response)
-            csv = io.StringIO(csv)
-        df_mean, df_std = _process_csv(csv, API_METHOD, verbose=verbose)
+            csv = _retrieve_dataframe_from_response(response)
+        df_mean, df_std = _process_csv(csv, API_METHOD)
+        if verbose:
+            print("Mean predictions:")
+            print(df_mean)
+            print("Standard deviation predictions:")
+            print(df_std)
         return df_mean, df_std
 
     @typechecked
     def sample(
         self,
         df: pd.DataFrame,
         num_samples: int,
@@ -944,34 +1008,41 @@
                 method=API_METHOD,
                 df=df,
                 num_samples=num_samples,
                 **params.unpack_parameters(),
                 verbose=verbose,
             )
         else:
+            data_csv = utils.get_csv_string(df)
+            dataset_id = _upload_large_datasets(df, data_csv, API_METHOD)
+            if dataset_id is not None:
+                data_csv = None
             _, response = api.use_request_model(
                 model_id=self.id,
                 method=API_METHOD,
-                data_csv=utils.get_csv_string(df),
+                dataset_id=dataset_id,
+                data_csv=data_csv,
                 num_samples=num_samples,
                 **params.unpack_parameters(),
                 processor=PROCESSOR,
                 verbose=DEBUG,
             )
             process_id = utils.get_value_from_body("process_id", response)
             if verbose:
                 print(f"Job {PROCESS_MAP[API_METHOD]} process ID: {process_id}")
             if not wait:
                 return process_id
             _, response = _wait_for_job_completion(
                 self.id, API_METHOD, process_id, verbose=verbose
             )
-            csv = utils.get_value_from_body("dataframe", response)
-            csv = io.StringIO(csv)
-        df = _process_csv(csv, API_METHOD, verbose=verbose)
+            csv = _retrieve_dataframe_from_response(response)
+        df = _process_csv(csv, API_METHOD)
+        if verbose:
+            print("Samples:")
+            print(df)
         return df
 
     @typechecked
     def recommend(
         self,
         num_points: int,
         acq_func: str,
@@ -991,15 +1062,15 @@
         A classic use case for this would be a user trying to reduce overally uncertainty.
         For example, a user trying to reduce the uncertainty in the strength of a pipe across all design parameters.
         The number of requested data points can be specified by the user, and if this is greater than one then then recommendations are all suggested at once, and are designed to be the optmial set, as a group, to achieve the user outcome.
         twinLab optimises which specific acquisition function within the chosen category will be used, prioritising numerical stability based on the number of points requested.
 
         The value of the acquisition function is also returned to the user.
         While this is of limited value in isolation, the trend of the acquisition function value over multiple iterations of ``Recommend`` can be used to understand the performance of the emulator.
-        The ``Emualtor.learn`` method can be used to improve the performance of an emulator iteratively.
+        The ``Emulator.learn`` method can be used to improve the performance of an emulator iteratively.
 
         Args:
             num_points (int): The number of samples to draw for each row of the evaluation data.
             acq_func (str): Specifies the acquisition function to be used when recommending new points.
                 The acquisition function can be either ``"explore"`` or ``"optimise"``.
             params (RecommendParams, optional): A parameter configuration that contains all of the optional recommendation parameters.
             wait (bool, optional): If ``True`` wait for the job to complete, otherwise return the process ID and exit.
@@ -1029,15 +1100,15 @@
                 -0.00553509
 
         Example:
 
             .. code-block:: python
 
                 emulator = tl.Emulator("quickstart")
-                emulator.recommend(3, "optimisation")
+                emulator.recommend(3, "optimise")
 
             .. code-block:: console
 
                           x
                 0  0.273920
                 1  0.306423
                 2  0.226851
@@ -1061,22 +1132,14 @@
                 method=API_METHOD,
                 num_points=num_points,
                 acq_func=ACQ_FUNC_DICT[acq_func],
                 **params.unpack_parameters(),
                 verbose=verbose,
             )
 
-            df = _process_csv(csv, API_METHOD, verbose=verbose)
-
-            if verbose:
-                print("Recommended samples:")
-                print(df)
-
-            return df, acq_func_value
-
         else:
             _, response = api.use_request_model(
                 model_id=self.id,
                 method=API_METHOD,
                 num_points=num_points,
                 acq_func=ACQ_FUNC_DICT[acq_func],
                 **params.unpack_parameters(),
@@ -1087,29 +1150,26 @@
             if verbose:
                 print(f"Job {PROCESS_MAP[API_METHOD]} process ID: {process_id}")
             if not wait:
                 return process_id
             _, response = _wait_for_job_completion(
                 self.id, API_METHOD, process_id, verbose=verbose
             )
-            csv = utils.get_value_from_body("dataframe", response)
+            csv = _retrieve_dataframe_from_response(response)
             acq_func_value = float(
                 utils.get_value_from_body("acq_func_value", response)
             )
-            csv = io.StringIO(csv)
-
-            df = _process_csv(csv, API_METHOD, verbose=verbose)
-
-            if verbose:
-                print("Recommended samples:")
-                print(df)
-                print("Acquisition function value:")
-                print(acq_func_value)
 
-            return df, acq_func_value
+        df = _process_csv(csv, API_METHOD)
+        if verbose:
+            print("Recommended points:")
+            print(df)
+            print("Acquisition function value:")
+            print(acq_func_value)
+        return df, acq_func_value
 
     @typechecked
     def calibrate(
         self,
         df_obs: pd.DataFrame,
         df_std: pd.DataFrame,
         params: CalibrateParams = CalibrateParams(),
@@ -1159,124 +1219,162 @@
                 df=df_obs,
                 df_std=df_std,
                 **params.unpack_parameters(),
                 verbose=verbose,
             )
             df = pd.read_csv(csv, sep=",")
         else:
+            data_csv = utils.get_csv_string(df_obs)
+            data_std_csv = utils.get_csv_string(df_std)
+            dataset_id = _upload_large_datasets(df_obs, data_csv, API_METHOD)
+            dataset_std_id = _upload_large_datasets(
+                df_std, data_std_csv, API_METHOD + "_std"
+            )
+            if dataset_id is not None:
+                data_csv = None
+            if dataset_std_id is not None:
+                data_std_csv = None
             _, response = api.use_request_model(
                 model_id=self.id,
                 method=API_METHOD,
-                data_csv=utils.get_csv_string(df_obs),
-                data_std_csv=utils.get_csv_string(df_std),
+                data_csv=data_csv,
+                data_std_csv=data_std_csv,
+                dataset_id=dataset_id,
+                dataset_std_id=dataset_std_id,
                 **params.unpack_parameters(),
                 processor=PROCESSOR,
                 verbose=DEBUG,
             )
             process_id = utils.get_value_from_body("process_id", response)
             if verbose:
                 print(f"Job {PROCESS_MAP[API_METHOD]} process ID: {process_id}")
             if not wait:
                 return process_id
             _, response = _wait_for_job_completion(
                 self.id, API_METHOD, process_id, verbose=verbose
             )
-            csv = utils.get_value_from_body("dataframe", response)
-            csv = io.StringIO(csv)
-            df = _process_csv(csv, API_METHOD, verbose=verbose)
+            csv = _retrieve_dataframe_from_response(response)
+            df = _process_csv(csv, API_METHOD)
+        if verbose:
+            print("Calibration summary:")
+            print(df)
         return df
 
     @typechecked
     def learn(
         self,
         dataset: Dataset,
         inputs: List[str],
         outputs: List[str],
         num_loops: int,
         num_points_per_loop: int,
         acq_func: str,
         simulation: Callable,  # A function that ingests X and returns y
         train_params: TrainParams = TrainParams(),
         recommend_params: RecommendParams = RecommendParams(),
-        verbose: bool = False,
+        verbose: bool = True,
     ) -> None:
         """Perform active learning to improve an emulator on the twinLab cloud.
 
         Active learning is a method that can identify and utilise the most informative data points to add to an emulator in order to reduce the number of measurements to be taken or simulations that are required.
         Using active learning can result in a more accurate model, trained with less data.
-        The primary difference between this method and ``Emulator.recommend`` is that in this method the emulator is trained on the new data points that are suggested in an active loop.
-        This way, new data can be used to update an emulator until the desired level of accuracy is achieved.
+        The primary difference between this method and ``Emulator.recommend`` is that in this method, the emulator is trained, new data points are suggested, and then training occurs continuously in an active loop.
+        This way, new data can be used to train and update an emulator until the desired level of accuracy is achieved.
         This can be done using either the ``"optmise"`` or ``"explore"`` acquisition functions.
-        The emulator can therefore be updated with the objective of either finding the point of maximum output or reducing the overall uncertainty in the emulator.
+        The emulator is therefore updated on the twinLab cloud with the objective of either finding the point of maximum output or reducing the overall uncertainty in the emulator.
+        This method does not return anything to the user directly, but instead updates the ``Dataset`` and ``Emulator`` in the cloud.
 
         Args:
             dataset (Dataset): twinLab dataset object which contains the initial training data for the emulator.
             inputs (list[str]): List of input column names in the training dataset.
             outputs (list[str]): List of output column names in the training dataset.
-            num_loops (int): Number of loops to run the learning process.
+            num_loops (int): Number of loops to run of the learning process. This must be a positive integer. Note that in this method, the emulator is trained and then re-trained on new suggested data points, so setting ``num_loops=1`` here will mean that ``Emulator.train`` is run _twice_, and ``Emulator.recommend`` is run once.
             num_points_per_loop (int): Number of points to sample in each loop.
             acq_func (str): Specifies the acquisition function to be used when recommending new points: either ``"explore"`` or ``"optimise"``.
             simulation (Callable): A function that takes in a set of inputs and generates the outputs (for example, a simulator for the data generating process).
-            train_params (TrainParams, optional): A parameter configuration that contains optional training parameters.
+            train_params (TrainParams, optional): A parameter configuration that contains optional training parameters. Note that currently we only support the case when ``"test_train_ratio=1"`` when running a learning loop.
             recommend_params (RecommendParams, optional): A parameter configuration that contains optional recommendation parameters.
-            verbose (bool, optional): Display detailed information about the operation while running.
+            verbose (bool, optional): Display detailed information about the operation while running. If ``True``, the requested candidate points will be printed to the screen while running. If ``False`` the emulator will be updated on the cloud while the method runs silently.
 
         Examples:
             .. code-block:: python
 
-                emulator = tl.Emulator(id=emulator_id)
-                dataset = tl.Dataset(dataset_id)
+                emulator = tl.Emulator("quickstart")
+                dataset = tl.Dataset("quickstart")
                 emulator.learn(
                     dataset=dataset,
-                    inputs=["X"],
+                    inputs=["x"],
                     outputs=["y"],
                     num_loops=3,
                     num_points_per_loop=5,
                     acq_func="explore",
                     simulation=my_simulator,
                 )
 
         """
 
+        if train_params.train_test_ratio != 1:
+            raise ValueError(
+                f"The test_train_ratio must be set to 1, not {train_params.train_test_ratio}, for this method to work."
+            )
+
+        if num_loops <= 0:
+            raise ValueError(
+                f"num_loops must be set to an integer value of 1 or more, not {num_loops}, for this method to work."
+            )
+
+        # Train model initially
+        self.train(
+            dataset=dataset,
+            inputs=inputs,
+            outputs=outputs,
+            params=train_params,
+            verbose=False,
+        )
+
         # Loop over iterations of learning
         for i in range(num_loops):
 
+            # Compute optimal sample location(s)
+            candidate_points, acq_func_value = self.recommend(
+                num_points=num_points_per_loop,
+                acq_func=acq_func,
+                params=recommend_params,
+                verbose=False,
+            )
+
+            # Evaluating the candidate points
+            candidate_points[outputs] = pd.DataFrame(
+                simulation(candidate_points[inputs].values)
+            )
+
             # Train model
             self.train(
                 dataset=dataset,
                 inputs=inputs,
                 outputs=outputs,
                 params=train_params,
-                verbose=verbose,
+                verbose=False,
             )
 
-            # Get recommendations on all but final iteration
-            if i < num_loops - 1:
+            # Download current training data, append new data, and reupload
+            df_train = self.view_train_data()
+            df_train = pd.concat([df_train, candidate_points], ignore_index=True)
+            dataset.upload(df_train)
 
-                # Compute optimal sample location(s)
-                candidate_points, _ = self.recommend(
-                    num_points=num_points_per_loop,
-                    acq_func=acq_func,
-                    params=recommend_params,
-                    verbose=verbose,
-                )
+            if verbose:
                 print(f"Iteration: {i}")
                 print("Suggested candidate point(s):")
-                print(candidate_points)
-                print()
-
-                # Evaluating the candidate points
-                candidate_points[outputs] = pd.DataFrame(
-                    simulation(candidate_points[inputs].values)
-                )
-
-                # Download current training data, append new data, and reupload
-                df_train = self.view_train_data()
-                df_train = pd.concat([df_train, candidate_points], ignore_index=True)
-                dataset.upload(df_train)
+                pprint(candidate_points)
+                print("Acquisition function value:")
+                print(acq_func_value)
+        if verbose:
+            print(
+                f"The candidate points have been uploaded in the Dataset {dataset.id}, alongside the emulator training data, on twinLab cloud."
+            )
 
     @typechecked
     def delete(self, verbose: bool = False) -> None:
         """Delete emulator from the twinLab cloud.
 
         It can be useful to delete an emulator to keep a cloud account tidy, or if an emulator is no longer necessary.
 
@@ -1380,14 +1478,15 @@
     @typechecked
     def heatmap(
         self,
         x1_axis: str,
         x2_axis: str,
         y_axis: str,
         x_fixed: Dict[str, float] = {},
+        mean_or_std: str = "mean",
         params: PredictParams = PredictParams(),
         x1_lim: Optional[Tuple[float, float]] = None,
         x2_lim: Optional[Tuple[float, float]] = None,
         n_points: int = 25,
         cmap=digilab_cmap,
         verbose: bool = False,
     ) -> plt.plot:
@@ -1401,19 +1500,20 @@
         Args:
             x1_axis (str): The name of the x1-axis variable (horizonal axis).
             x2_axis (str): The name of the x2-axis variable (vertical axis).
             y_axis (str): The name of the plotted variable (heatmap).
             x_fixed (dict, optional): A dictionary of fixed values for the other ``X`` variables.
                 Note that all ``X`` variables of an emulator must either be specified as ``x1_axis``, ``x2_axis`` or appear as keys in ``x_fixed``.
                 Passing an empty dictionary (the default) will fix none of the variables.
+            mean_or_std (str, optional): A string determining whether to plot the mean (``"mean"``) or standard deviation (``"std"``) of the emulator. Defaults to ``"mean"``.
             params: (PredictParams, optional). A parameter configuration that contains optional prediction parameters.
             x1_lim (tuple[float, float], optional): The limits of the x1-axis.
-                If not provided. the limits will be taken directly from the emulator.
+                If not provided, the limits will be taken directly from the emulator.
             x2_lim (tuple[float, float], optional): The limits of the x2-axis.
-                If not provided. the limits will be taken directly from the emulator.
+                If not provided, the limits will be taken directly from the emulator.
             n_points (int, optional): The number of points to sample in each dimension.
                 The default is 25, which will create a 25x25 grid.
             cmap (str, optional): The color of the plot. Defaults to a digiLab palette.
                 Can be any valid matplotlib color (https://matplotlib.org/stable/users/explain/colors/colormaps.html).
             verbose (bool, optional): Display detailed information about the operation while running.
 
         Returns:
@@ -1466,19 +1566,26 @@
         if x_fixed is not None:
             for x_col, x_val in x_fixed.items():
                 X[x_col] = x_val * np.ones(n_points**2)
         df_X = pd.DataFrame(X)
 
         # Predict using the emulator
         # NOTE: Uncertainty is discarded here
-        df_mean, _ = self.predict(df_X, params=params, verbose=verbose)
+        df_mean, df_std = self.predict(df_X, params=params, verbose=verbose)
+
+        if mean_or_std == "mean":
+            df = df_mean
+        elif mean_or_std == "std":
+            df = df_std
+        else:
+            raise ValueError("mean_or_std must be either 'mean' or 'std'")
 
         # Plot the results
         plt = heatmap(
             x1_axis,
             x2_axis,
             y_axis,
             df_X,
-            df_mean,
+            df,
             cmap,
         )
         return plt  # Return the plot
```

### Comparing `twinlab-2.5.0/twinlab/helper.py` & `twinlab-2.6.0/twinlab/helper.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.5.0/twinlab/params.py` & `twinlab-2.6.0/twinlab/params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Standard imports
 from abc import ABC, abstractmethod
-from typing import List, Optional, Set, Union
+from typing import Dict, List, Optional, Set, Tuple, Union
 
-# Third-party imports
 import pandas as pd
+
+# Third-party imports
+from deprecated import deprecated
 from typeguard import typechecked
 
 from .dataset import Dataset
 from .sampling import LatinHypercube, Sampling
 
 # Project imports
 from .utils import remove_none_values
@@ -64,14 +66,15 @@
     """Abstract base class for all parameter classes"""
 
     @abstractmethod
     def unpack_parameters(self):
         pass
 
 
+@typechecked
 class EstimatorParams(Params):
     """Parameter configuration for the Gaussian Process emulator (estimator).
 
     Attributes:
         detrend (bool, optional): Should the linear trend in the data be removed (detrended) before training the emulator?
             The defaults is ``False``.
         covar_module (Union[str, None], optional): Specifies the functions that build up the kernel (covariance matrix) of the Gaussian Process.
@@ -122,14 +125,15 @@
             "covar_module": self.covar_module,
             "estimator_type": self.estimator_type,
         }
         params = remove_none_values(params)
         return params
 
 
+@typechecked
 class ModelSelectionParams(Params):
     """Parameter configuration for the Bayesian model selection process.
 
     Attributes:
         seed (Union[int, None], optional): Specifies the seed for the random number generator for every trial of the model selection process.
             Setting to an integer is necessary for reproducible results.
             The default value is ``None``, which means the seed is randomly generated each time.
@@ -192,14 +196,15 @@
             "depth": self.depth,
             "beam": self.beam,
         }
         params = remove_none_values(params)
         return params
 
 
+@typechecked
 class TrainParams(Params):
     """Parameter configuration for training an emulator.
 
     This includes parameters that pertain directly to the training of the model,
     such as the ratio of training to testing data,
     as well as parameters that pertain to the setup of the model such as the number of dimensions to retain after decomposition.
 
@@ -313,55 +318,47 @@
         train_params = remove_none_values(train_params)
         if self.dataset_std is not None:
             train_params["dataset_std_id"] = self.dataset_std.id
         params = {**setup_params, **train_params}
         return params
 
 
-### ###
-
-
-### Score ###
+@typechecked
 class ScoreParams(Params):
     """Parameter configuration for scoring a trained emulator.
 
     Attributes:
         metric (str, optional): Metric used for scoring the performance of an emulator.
             Can be either:
             • ``"MSE"``: Mean Squared Error, which only compared the mean emulator prediction to the test data.
             • ``"MSLL"``: Mean Squared Log Loss, which compares the distribution of the emulator prediction to the test data.
-            The default is ``"MSE"``.
+            The default is ``"MSLL"``.
         combined_score (bool, optional): Determining whether to combined (average) the emulator score across output dimensions.
             If ``False`` a dataframe of scores will be returned, with the score for each output dimension, even if there is only a single emulator output dimension.
             If ``True`` a single number will be returned, which is the average score across all output dimensions.
             The default is ``False``.
 
     """
 
     def __init__(
         self,
-        metric: str = "MSE",
+        metric: str = "MSLL",
         combined_score: bool = False,
     ):
         self.metric = metric
         self.combined_score = combined_score
 
     def unpack_parameters(self):
         params = {
             "metric": self.metric,
             "combined_score": self.combined_score,
         }
         return params
 
 
-### ###
-
-### Benchmark ###
-
-
 class BenchmarkParams(Params):
     """Parameter configuration for benchmarking a trained emulator.
 
     Attributes:
         type (str, optional): Specifies the type of emulator benchmark to be performed.
             Can be either:
 
@@ -381,19 +378,15 @@
         self.type = type
 
     def unpack_parameters(self):
         params = {"type": self.type}
         return params
 
 
-### ###
-
-### Predict ###
-
-
+@typechecked
 class PredictParams(Params):
     """Parameter configuration for making predictions using a trained emulator.
 
     Attributes:
         observation_noise (bool, optional): Whether or not to include the noise term in the standard deviation of the prediction.
             Setting this to ``False`` can be a good idea if the training data is noisy but the underlying trend of the trained model is smooth.
             In this case, the predictions would correspond to the underlying trend.
@@ -410,19 +403,15 @@
         self.observation_noise = observation_noise
 
     def unpack_parameters(self):
         params = {"kwargs": {"observation_noise": self.observation_noise}}
         return params
 
 
-### ###
-
-### Sample ###
-
-
+@typechecked
 class SampleParams(Params):
     """Parameter configuration for sampling from a trained emulator.
 
     Attributes:
         seed (Union[int, None], optional): Specifies the seed used by the random number generator to generate a set of samples.
             Setting this to an integer is useful for the reproducibility of results.
             The default value is ``None``, which means the seed is randomly generated each time.
@@ -448,119 +437,98 @@
         if "fidelity" in params["kwargs"]:
             params["kwargs"]["fidelity"] = _convert_dataframe_to_dict(
                 params["kwargs"], "fidelity"
             )
         return params
 
 
-### ###
+@deprecated(
+    version="2.6.0",
+    reason="AcqFuncParams is deprecated and will be removed in a future release. The functionality can be found in the RecommendParams class henceforth.",
+)
+class AcqFuncParams(Params):
+    def __init__():
+        pass
 
-### Recommend ###
 
+@deprecated(
+    version="2.6.0",
+    reason="OptimiserParams is deprecated and will be removed in a future release. The functionality can be found in the RecommendParams class henceforth.",
+)
+class OptimiserParams(Params):
+    def __init__():
+        pass
 
-# TODO: Combine AcqFuncParams with the RecommendParams class
-class AcqFuncParams(Params):
-    """Parameter configuration for the acquisition function used in the Bayesian-optimisation routine.
+
+@typechecked
+class RecommendParams(Params):
+    """Parameter configuration for recommending new points to sample using the Bayesian-optimisation routine.
 
     Attributes:
         weights (Union[list[float], None], optional):
             A list of weighting values that are used to scalarise the objective function in the case of a multi-output model.
             The default value is ``None``, which applies equal weight to each output dimension.
-
-    """
-
-    def __init__(
-        self,
-        weights: Optional[List[float]] = None,
-        # mc_points: Optional[int] = None, # TODO: Cannot be included because tensor
-    ):
-        self.weights = weights
-        self.mc_points = None
-
-    def unpack_parameters(self):
-        params = {"weights": self.weights, "mc_points": self.mc_points}
-        params = remove_none_values(params)
-        return params
-
-
-# TODO: Combine OptimiserParams with the RecommendParams class
-class OptimiserParams(Params):
-    """Parameter configuration for the optimiser used in the Bayesian-optimisation routine.
-
-    Attributes:
         num_restarts (int, optional): The number of random restarts for optimisation.
             The default value is ``5``.
         raw_samples (int, optional): The number of samples for initialization.
             The default value is ``128``.
+        bounds (Union[Tuple, None], optional): The bounds of the input space.
+            If this is set to `None` then the bounds are inferred from the range of the training data.
+            Otherwise, this must be a dictionary mapping column names to a tuple of lower and upper bounds.
+            For example, ``{"x0": (0, 1), "x1": (0, 2)}`` to set boundaries on two input variables ``x0`` and ``x1``.
+        seed (Union[int, None], optional): Specifies the seed used by the random number generator to start the optimiser to discover the recommendations.
+            Setting this to an integer is good for reproducibility.
+            The default value is ``None``, which means the seed is randomly generated each time.
 
     """
 
     def __init__(
         self,
+        weights: Optional[List[float]] = None,
+        # mc_points: Optional[int] = None, # TODO: Cannot be included because tensor
         num_restarts: int = 5,
         raw_samples: int = 128,
-        # bounds: Optional[pd.DataFrame] = None, # TODO: Commented-out as pandas types hard to serialise
+        bounds: Optional[Dict[str, Tuple[float, float]]] = None,
+        seed: Optional[int] = None,
     ):
+        self.weights = weights
+        self.mc_points = None
         self.num_restarts = num_restarts
         self.raw_samples = raw_samples
-        self.bounds = None
+        self.bounds = bounds
+        self.seed = seed
+
+        if self.bounds is not None:
+            self.bounds = pd.DataFrame(self.bounds)
+            self.bounds.rename(
+                index={0: "lower_bounds", 1: "upper_bounds"}, inplace=True
+            )
 
     def unpack_parameters(self):
-        params = {
+        acq_kwargs = {"weights": self.weights, "mc_points": self.mc_points}
+        opt_kwargs = {
             "num_restarts": self.num_restarts,
             "raw_samples": self.raw_samples,
             "bounds": self.bounds,
         }
-        params = remove_none_values(params)
-        if "bounds" in params:
-            params["bounds"] = _convert_dataframe_to_dict(params, "bounds")
-        return params
-
-
-# TODO: Merge AcqFuncParams and OptimiserParams into RecommendParams!
-class RecommendParams(Params):
-    """Parameter configuration for recommending new points to sample using the Bayesian-optimisation routine.
-
-    Attributes:
-        acq_kwargs (AcqFuncParams, optional): An `AcqFuncParams` object for customising the acquisition function.
-        opt_kwargs (OptimiserParams, optional): An `OptimiserParams` object for customising the optimisation routine.
-        seed (Union[int, None], optional): Specifies the seed used by the random number generator to start the optimiser to discover the recommendations.
-            Setting this to an integer is good for reproducibility.
-            The default value is ``None``, which means the seed is randomly generated each time.
-
-    """
-
-    def __init__(
-        self,
-        acq_kwargs: AcqFuncParams = AcqFuncParams(),
-        opt_kwargs: OptimiserParams = OptimiserParams(),
-        seed: Optional[int] = None,
-    ):
-        self.acq_kwargs = acq_kwargs
-        self.opt_kwargs = opt_kwargs
-        self.seed = seed
-
-    def unpack_parameters(self):
+        if "bounds" in opt_kwargs and opt_kwargs["bounds"] is not None:
+            opt_kwargs["bounds"] = _convert_dataframe_to_dict(opt_kwargs, "bounds")
         params = {
-            "acq_kwargs": self.acq_kwargs.unpack_parameters(),
-            "opt_kwargs": self.opt_kwargs.unpack_parameters(),
+            "acq_kwargs": acq_kwargs,
+            "opt_kwargs": opt_kwargs,
             "kwargs": {
                 "return_acq_func_value": True,  # This is fixed to be true here!
                 "seed": self.seed,
             },
         }
         params = remove_none_values(params)
         return params
 
 
-### ###
-
-### Calibrate ###
-
-
+@typechecked
 class CalibrateParams(Params):
     """Parameter configuration for inverting a trained emulator to estimate the input parameters that generated a given output.
 
     Attributes:
         y_std_model (Union[bool, pd.DataFrame], optional): Whether to include model noise covariance in the likelihood.
 
             - If ``True`` TODO ...
@@ -626,17 +594,15 @@
         if (
             "y_std_model" in params
         ):  # TODO: y_std_model is not affected by remove_none_values because default is set to False. If we change that (which seems to be the case), we need to update the API in a similar way of get_candidate_points with bounds.
             params["y_std_model"] = _convert_dataframe_to_dict(params, "y_std_model")
         return params
 
 
-### ###
-
-
+@typechecked
 class DesignParams:
     """Parameter configuration to setup an initial experimental or simulations design structure.
 
     Attributes:
         sampling_method (Sampling, optional): The sampling method to use for the initial design.
             Options are either:
```

### Comparing `twinlab-2.5.0/twinlab/plotting.py` & `twinlab-2.6.0/twinlab/plotting.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.5.0/twinlab/prior.py` & `twinlab-2.6.0/twinlab/prior.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import json
 
 from typeguard import typechecked
 
+
 from .distributions import Distribution
 
 
 @typechecked
 class Prior:
     """A prior probability distribution
 
     Attributes:
         name (str): This is the name given to the prior, usually corresponding to the parameter it represents.
         distribution (Distribution): The one-dimensional probability distribution for the prior.
 
     """
 
-    def __init__(self, name: str, distribution):  # TODO: Typehint here!
+    def __init__(self, name: str, distribution: Distribution):
         self.name = name
         self.distribution = distribution
 
     def to_json(self):
         return json.dumps(
             {"name": self.name, "distribution": self.distribution.to_json()}
         )
```

### Comparing `twinlab-2.5.0/twinlab/sampling.py` & `twinlab-2.6.0/twinlab/sampling.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.5.0/twinlab/settings.py` & `twinlab-2.6.0/twinlab/settings.py`

 * *Files identical despite different names*

### Comparing `twinlab-2.5.0/twinlab/utils.py` & `twinlab-2.6.0/twinlab/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,31 @@
         else:
             print(f"File upload failed")
             print(f"Status code: {response.status_code}")
             print(f"Reason: {response.text}")
 
 
 @typechecked
+def download_dataframe_from_presigned_url(url: str) -> io.StringIO:
+    """
+    Download a `pandas.DataFrame` from the specified pre-signed URL.
+
+    Args:
+        url (str): The pre-signed URL generated for downloading the file.
+
+    Returns:
+        io.StringIO: The dataframe in string format downloaded from the URL.
+
+    """
+    response = requests.get(url)
+    buffer = io.StringIO(response.text)
+    return buffer
+
+
+@typechecked
 def get_csv_string(df: pd.DataFrame) -> str:
     buffer = io.StringIO()
     df.to_csv(buffer, index=False)
     return buffer.getvalue()
 
 
 @typechecked
```

