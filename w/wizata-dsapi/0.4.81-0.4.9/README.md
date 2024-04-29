# Comparing `tmp/wizata-dsapi-0.4.81.tar.gz` & `tmp/wizata-dsapi-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.4.81.tar", last modified: Mon Apr 29 07:42:41 2024, max compression
+gzip compressed data, was "wizata-dsapi-0.4.9.tar", last modified: Sat Mar  2 10:17:15 2024, max compression
```

## Comparing `wizata-dsapi-0.4.81.tar` & `wizata-dsapi-0.4.9.tar`

### file list

```diff
@@ -1,43 +1,39 @@
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-04-29 07:42:41.794190 wizata-dsapi-0.4.81/
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.81/LICENSE.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      170 2024-04-29 07:42:41.794066 wizata-dsapi-0.4.81/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.81/README.rst
--rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-04-29 07:42:41.794241 wizata-dsapi-0.4.81/setup.cfg
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1450 2024-04-16 13:41:39.000000 wizata-dsapi-0.4.81/setup.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-04-29 07:42:41.793159 wizata-dsapi-0.4.81/wizata_dsapi/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1531 2024-03-20 11:49:55.000000 wizata-dsapi-0.4.81/wizata_dsapi/__init__.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3875 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/api_config.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1172 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/api_dto.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     9270 2024-04-24 13:52:28.000000 wizata-dsapi-0.4.81/wizata_dsapi/api_interface.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4151 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/business_label.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10084 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/context.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     6503 2024-03-20 11:49:55.000000 wizata-dsapi-0.4.81/wizata_dsapi/dataframe_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10822 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/datapoint.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2089 2024-03-06 07:51:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/ds_dataframe.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.81/wizata_dsapi/dsapi_json_encoder.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12777 2024-04-29 07:42:28.000000 wizata-dsapi-0.4.81/wizata_dsapi/execution.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4355 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/experiment.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      807 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/ilogger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    14587 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/mlmodel.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1551 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/model_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1150 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/paged_query_result.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    28788 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/pipeline.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2355 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/plot.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    19308 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12710 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/script.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     7625 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/solution_component.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12451 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/template.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4769 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/trigger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     6291 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/twin.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12865 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/twinregistration.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)       23 2024-04-29 07:42:28.000000 wizata-dsapi-0.4.81/wizata_dsapi/version.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      942 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/wizard_function.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3762 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/wizard_request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    68678 2024-04-24 07:58:32.000000 wizata-dsapi-0.4.81/wizata_dsapi/wizata_dsapi_client.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1535 2024-03-20 11:49:55.000000 wizata-dsapi-0.4.81/wizata_dsapi/words.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-04-29 07:42:41.793886 wizata-dsapi-0.4.81/wizata_dsapi.egg-info/
--rw-r--r--   0 wizata.jph   (502) staff       (20)      170 2024-04-29 07:42:41.000000 wizata-dsapi-0.4.81/wizata_dsapi.egg-info/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1037 2024-04-29 07:42:41.000000 wizata-dsapi-0.4.81/wizata_dsapi.egg-info/SOURCES.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-04-29 07:42:41.000000 wizata-dsapi-0.4.81/wizata_dsapi.egg-info/dependency_links.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      591 2024-04-29 07:42:41.000000 wizata-dsapi-0.4.81/wizata_dsapi.egg-info/requires.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-04-29 07:42:41.000000 wizata-dsapi-0.4.81/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-03-02 10:17:15.210280 wizata-dsapi-0.4.9/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-03-02 10:17:15.210150 wizata-dsapi-0.4.9/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-03-02 10:17:15.210339 wizata-dsapi-0.4.9/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1444 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-03-02 10:17:15.208738 wizata-dsapi-0.4.9/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1375 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1340 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     6270 2024-02-28 18:32:59.000000 wizata-dsapi-0.4.9/wizata_dsapi/api_interface.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3092 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/business_label.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7101 2024-02-20 13:36:21.000000 wizata-dsapi-0.4.9/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8370 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2194 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19290 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4155 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      311 2023-11-24 08:24:01.000000 wizata-dsapi-0.4.9/wizata_dsapi/ilogger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11814 2024-03-02 10:16:09.000000 wizata-dsapi-0.4.9/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      761 2023-11-24 08:24:01.000000 wizata-dsapi-0.4.9/wizata_dsapi/paged_query_result.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19316 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2464 2024-02-28 18:33:10.000000 wizata-dsapi-0.4.9/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19133 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8874 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5080 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/solution_component.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11723 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5917 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12376 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-03-02 10:16:49.000000 wizata-dsapi-0.4.9/wizata_dsapi/version.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    63507 2024-02-28 18:32:59.000000 wizata-dsapi-0.4.9/wizata_dsapi/wizata_dsapi_client.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-03-02 10:17:15.209967 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      933 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      585 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.4.81/LICENSE.txt` & `wizata-dsapi-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.81/setup.py` & `wizata-dsapi-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
     author_email='info@wizata.com',
     packages=['wizata_dsapi'],
     install_requires=[
         'dill==0.3.6',
         'pandas==1.5.3',
         'numpy==1.23.5',
         'matplotlib==3.7.1',
-        'protobuf==3.20.3',
-        "tensorflow==2.15.0; sys_platform != 'darwin' or platform_machine != 'arm64'",
-        "tensorflow-macos==2.15.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
-        "keras==2.15.0; sys_platform != 'darwin' or platform_machine != 'arm64'",
-        "keras==2.15.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
+        'protobuf==3.19.6',
+        "tensorflow==2.7; sys_platform != 'darwin' or platform_machine != 'arm64'",
+        "tensorflow-macos==2.11.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
+        "keras==2.7; sys_platform != 'darwin' or platform_machine != 'arm64'",
+        "keras==2.11.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
         'tensorflow_probability==0.15.0',
         'scikit-learn==1.2.2',
         'plotly==5.13.1',
         'adtk==0.6.2',
         'scipy==1.10.1',
         'xgboost==1.7.4',
         'joblib==1.2.0',
@@ -36,12 +36,12 @@
         'explainerdashboard==0.4.2.1',
         'ipywidgets==8.0.4',
         'kaleido==0.2.1',
         'pytest==7.2.2',
         'pytest-cov==4.0.0',
         'shapely==2.0.1',
         'pyodbc==4.0.35',
-        'msal>=1.24.0',
+        'msal==1.21.0',
         'u8darts==0.25.0',
         'optuna==3.3.0'
     ]
 )
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/__init__.py` & `wizata-dsapi-0.4.9/wizata_dsapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # Api Entities (Dto)
 from .version import __version__
 from .api_dto import ApiDto
 from .paged_query_result import PagedQueryResult
 from .plot import Plot
-from .mlmodel import MLModel, MLModelConfig
+from .mlmodel import MLModel, MLModelConfig, ModelKeyType
 from .request import Request, filter_map
 from .execution import Execution, ExecutionStatus, ExecutionStepLog, AbortedException
 from .experiment import Experiment
 from .ds_dataframe import DSDataFrame
 from .script import Script, ScriptConfig
 from .template import Template, TemplateProperty
 from .solution_component import SolutionComponent, SolutionType
 from .business_label import BusinessLabel
 from .twinregistration import TwinRegistration, TwinRegistrationProperty
-from .trigger import Trigger
 
 # Sql Entities (Dto)
 from .twin import Twin, TwinBlockType
 from .datapoint import DataPoint, BusinessType, Label, Unit, Category, InputModeType
 
 # Api
 from .api_interface import ApiInterface
-from .api_config import _registry
 from .wizata_dsapi_client import api
 from .wizata_dsapi_client import WizataDSAPIClient
-from .dataframe_toolkit import df_to_json, df_to_csv, df_from_json, df_from_csv, validate, generate_epoch, \
-    verify_relative_datetime, generate_unique_key
+from .dataframe_toolkit import df_to_json, df_to_csv, df_from_json, df_from_csv, validate, generate_epoch
 from .model_toolkit import predict
 
 # Legacy
 from .dsapi_json_encoder import DSAPIEncoder
 from .wizard_function import WizardStep, WizardFunction
-from .wizard_request import WizardRequest
 
 # Pipeline Entities (Dto)
-from .pipeline import Pipeline, PipelineStep, StepType, WriteConfig, VarType, PipelineIO
+from .pipeline import Pipeline, PipelineStep, StepType, WriteConfig, VarType
 from .context import Context
 from .ilogger import ILogger
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.4.9/wizata_dsapi/dataframe_toolkit.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import pandas
 import io
 from datetime import datetime, timedelta, timezone
 import re
-import random
-from .words import animals, colors
 
 
 def validate(df: pandas.DataFrame) -> pandas.DataFrame:
     """
     validate dataframe format to match supported Wizata format.
     :param df: dataframe to validate.
     :return: validated and formatted df - raise error if not valid.
@@ -113,29 +111,14 @@
         if col != 'Timestamp':
             df_json[col] = list(df[col].values.astype(float))
         else:
             df_json[col] = list(df[col].values)
     return df_json
 
 
-def verify_relative_datetime(formatted_string: str) -> bool:
-    """
-    verify format of a relative datetime str
-    """
-    if not isinstance(formatted_string, str):
-        raise ValueError(f'please provide a string as relative datetime')
-
-    pattern = r'^now([+-]\d+([yMwdHhms]{1,2}))?$'
-    match = re.match(pattern, formatted_string)
-    if not match:
-        raise ValueError(f"invalid time delay format {formatted_string}")
-
-    return True
-
-
 def generate_epoch(formatted_string: str, now=None):
     """
     generate an epoch based on a formatted string (e.g. now+6h) - see documentation.
     * now = datetime.utcnow() can be override
     * units = 'y' = 365d, 'M'=30d , 'w'=7d , 'd'=24h , 'h'=60m, 'm'=60s , 's'=1000'ms'
     * operators = '+' or '-'
     :param formatted_string: formatted epoch representation using relative time.
@@ -186,19 +169,7 @@
             raise ValueError("invalid time delay format")
     else:
         timestamp = now
 
     epoch = datetime.utcfromtimestamp(0)
     timestamp_ms = int((timestamp - epoch).total_seconds() * 1000)
     return timestamp_ms
-
-
-def generate_unique_key() -> str:
-    """
-    generate a unique key for experiment, pipeline, model, template, ...
-        - 7 char reserved for 'date_'
-        - 11 char for 'color_'
-        - 11 char for 'animal_'
-        - 3 car for number XXX
-    """
-    return f"{datetime.now().strftime('%y%m%d')}_{random.choice(colors).lower()}_" \
-           f"{random.choice(animals).lower()}_{random.randint(1, 999)}"
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.4.9/wizata_dsapi/mlmodel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,309 +1,297 @@
+import json
 import uuid
-from enum import Enum
 from .api_dto import ApiDto
-import json
+from enum import Enum
 
 
-class Category(ApiDto):
-    """
-    Category groups unit into what they represent.
-    e.g. Temperature, Distance, Speed, Pressure, ...
-    :ivar uuid.UUID category_id: Technical id of the category.
-    :ivar str name: Category name.
+def get_bool(obj, name: str):
+    if isinstance(obj[name], str) and obj[name].lower() == "false":
+        return False
+    else:
+        return bool(obj[name])
+
+
+class MLModelConfig(ApiDto):
+    """
+    a model config defines execution properties for a specific model.
+    usually to define how a pipeline should train and predict your model.
+
+    :ivar train_script: name of function referencing the script to train the model.
+    :ivar train_test_split_pct: percentage repartition to split the data for training and scoring.
+    :ivar target_feat: target feature name if existing.
+    :ivar features: filter list of datapoint columns if necessary.
+    :ivar train_test_split_type: name of function referencing the script to train the model.
+    :ivar model_key: key of the model to store (or use story property if dynamic).
+    :ivar output_property: name of dataframe column where to store results (or template property).
     """
 
     def __init__(self,
-                 category_id: uuid.UUID = None,
-                 name: str = None):
-        if category_id is None:
-            self.category_id = uuid.uuid4()
-        else:
-            self.category_id = category_id
-        self.name = name
+                 train_script=None,
+                 train_test_split_pct: float = 1.0,
+                 train_test_split_type: str = "ignore",
+                 function: str = "predict",
+                 target_feat: str = None,
+                 output_property: str = "result",
+                 features: list = None,
+                 model_key: str = None,
+                 by_twin: bool = False,
+                 by_property: bool = True,
+                 property_name: str = None,
+                 source: str = "wizata"
+                 ):
+
+        # training
+        self.train_script = train_script
+        self.train_test_split_pct = train_test_split_pct
+        self.train_test_split_type = train_test_split_type
+        self.function = function
+
+        # features management
+        self.target_feat = target_feat
+        self.features = features
+        self.output_property = output_property
+
+        # key and identification
+        self.model_key = model_key
+        self.by_twin = by_twin
+        self.by_property = by_property
+        self.property_name = property_name
 
-    def api_id(self) -> str:
-        return str(self.category_id).upper()
-
-    def endpoint(self) -> str:
-        return "Categories"
+        # source
+        self.source = source
 
     def from_json(self, obj):
-        if "id" in obj.keys():
-            self.category_id = uuid.UUID(obj["id"])
-
-        if "name" in obj.keys():
-            self.name = obj["name"]
-
-    def to_json(self):
-        obj = {
-            "id": str(self.category_id)
-        }
-        if self.name is not None and self.name != '':
-            obj["name"] = self.name
-        return obj
 
-
-class Label(ApiDto):
-    """
-    Label is a custom tag defining a time-series value.
-    :ivar uuid.UUID label_id: Technical id of the label.
-    :ivar str name: Label name.
-    """
-
-    def __init__(self,
-                 label_id: uuid.UUID = None,
-                 name: str = None):
-        if label_id is None:
-            self.label_id = uuid.uuid4()
-        else:
-            self.label_id = label_id
-        self.name = name
-
-    def api_id(self) -> str:
-        return str(self.label_id).upper()
-
-    def endpoint(self) -> str:
-        return "Labels"
-
-    def from_json(self, obj):
-        if "id" in obj.keys():
-            self.label_id = uuid.UUID(obj["id"])
-
-        if "name" in obj.keys():
-            self.name = obj["name"]
+        # blocking old configs
+        if "store_property" in obj.keys():
+            raise ValueError("deprecated and unsupported configuration 'store_property'")
+        if "model_key_type" in obj.keys():
+            raise ValueError("deprecated and unsupported configuration 'model_key_type'")
+
+        # training info
+        if "train_script" in obj.keys() and obj["train_script"] is not None:
+            self.train_script = obj["train_script"]
+        if "train_test_split_pct" in obj.keys() and obj["train_test_split_pct"] is not None:
+            self.train_test_split_pct = float(obj["train_test_split_pct"])
+        if "train_test_split_type" in obj.keys() and obj["train_test_split_type"] is not None:
+            self.train_test_split_type = obj["train_test_split_type"]
+        if "function" in obj.keys() and obj["function"] is not None:
+            self.function = obj["function"]
+
+        # features info
+        if "target_feat" in obj.keys() and obj["target_feat"] is not None:
+            self.target_feat = obj["target_feat"]
+        if "features" in obj.keys() and obj["features"] is not None:
+            self.features = obj["features"]
+        if "output_property" in obj.keys() and obj["output_property"] is not None:
+            self.output_property = obj["output_property"]
+
+        # source
+        if "source" in obj.keys() and obj["source"] is not None:
+            self.source = obj["source"]
+            if self.source not in ["wizata", "mlflow"]:
+                raise ValueError("source must be wizata or mlflow")
+
+        # key and target
+        if "model_key" not in obj.keys() or obj["model_key"] is None:
+            raise KeyError('model_key must be declared in the config.')
+        self.model_key = obj["model_key"]
+        if "by_twin" in obj.keys():
+            self.by_twin = get_bool(obj, name="by_twin")
+        if "by_property" in obj.keys():
+            self.by_property = get_bool(obj, name="by_property")
+        if "property_name" in obj.keys() and obj["property_name"] is not None:
+            self.property_name = obj["property_name"]
 
     def to_json(self, target: str = None):
         obj = {
-            "id": str(self.label_id)
+            "source": self.source
         }
-        if self.name is not None and self.name != '':
-            obj["name"] = self.name
-        return obj
-
-
-class Unit(ApiDto):
-    """
-    Unit defines how a time-series value is expressed.
-    :ivar uuid.UUID unit_id: Technical id of the unit.
-    :ivar str short_name: Short Display Name of the unit.
-    """
-
-    def __init__(self,
-                 unit_id: uuid.UUID = None,
-                 short_name: str = None):
-        if unit_id is None:
-            self.unit_id = uuid.uuid4()
-        else:
-            self.unit_id = unit_id
-        self.short_name = short_name
-
-    def api_id(self) -> str:
-        return str(self.unit_id).upper()
-
-    def endpoint(self) -> str:
-        return "Units"
-
-    def from_json(self, obj):
-        """
-        Load the datapoint entity from a dictionary.
-
-        :param obj: Dict version of the datapoint.
-        """
-        if "id" in obj.keys():
-            self.unit_id = uuid.UUID(obj["id"])
 
-        if "shortName" in obj.keys():
-            self.short_name = obj["shortName"]
+        # training info
+        if self.train_script is not None:
+            obj["train_script"] = str(self.train_script)
+        if self.train_test_split_pct is not None:
+            obj["train_test_split_pct"] = float(self.train_test_split_pct)
+        if self.train_test_split_type is not None:
+            obj["train_test_split_type"] = str(self.train_test_split_type)
+        if self.features is not None:
+            obj["features"] = self.features
+
+        # features info
+        if self.target_feat is not None:
+            obj["target_feat"] = str(self.target_feat)
+        if self.output_property is not None:
+            obj["output_property"] = self.output_property
+        if self.function is not None:
+            obj["function"] = self.function
+
+        # key and target
+        if self.model_key is not None:
+            obj["model_key"] = self.model_key
+        if self.by_twin is not None:
+            obj["by_twin"] = str(self.by_twin)
+        if self.by_property is not None:
+            obj["by_property"] = str(self.by_property)
+        if self.property_name is not None:
+            obj["property_name"] = self.property_name
 
-    def to_json(self, target: str = None):
-        obj = {
-            "id": str(self.unit_id)
-        }
-        if self.short_name is not None and self.short_name != '':
-            obj["shortName"] = self.short_name
         return obj
 
 
-class BusinessType(Enum):
-    """
-    BusinessType represents business usage of a datapoint, enumeration:
-        - "telemetry" represents a time-series emitted by a hardware device as an information (one direction).
-        - "setPoint" is used for time-series signals bidirectional used to set hardware configuration.
-        - "logical" represents a time-series calculated from others or third-party solution.
-        - "measurement" represents a logical time-series manually inputted by a human.
-    """
-    TELEMETRY = "telemetry"
-    SET_POINTS = "setPoint"
-    LOGICAL = "logical"
-    MEASUREMENT = "measurement"
-
-
-class InputModeType(Enum):
-    """
-    InputModeType defines authorization or not to write value on a time-series datapoint.
-        - "none" datapoint cannot be written from Wizata.
-        - "manual" datapoint can be written by a human.
-        - "automatic" datapoint can only be written through automatic computation.
-        - "manualAndAutomatic" authorize both manual and automatic.
-    """
-    NONE = "none"
-    MANUAL = "manual"
-    AUTOMATIC = "automatic"
-    MANUAL_AND_AUTOMATIC = "manualAndAutomatic"
-
-
-class DataPoint(ApiDto):
+class MLModel(ApiDto):
     """
-    A datapoint reference a time-series tag stored on DB.
+    A trained Machine Learning Model stored to be executed on demand.
+    Can contain also a scaler, both object are stored as pickled file.
 
-    :ivar uuid.UUID datapoint_id: Unique datapoint identifier (technical id).
-    :ivar str hardware_id: The unique datapoint logical hardware id corresponding to time-series tag name.
-    :ivar wizata_dsapi.BusinessType business_type: Business type of a datapoint defining usage.
-    :ivar str name: Display name used in the user interface.
-    :ivar uuid.UUID twin_id: Set parent twin id on which datapoint is attached.
-    :ivar uuid.UUID unit_id: Unit on which the time-series is expressed (e.g. Celsius Degree).
-    :ivar uuid.UUID category_id: Defines the Unit category (e.g Temperature).
-    :ivar str description: Additional information to help user understand the datapoint.
-    :ivar float min_value: Set manufacturer specification for hardware logical minimum values.
-    :ivar float max_value: Set manufacturer specification for hardware logical maximum values.
-    :ivar int frequency: Set frequency in milliseconds at which this data point should theoretically emit data.
-    :ivar wizata_dsapi.InputModeType input_mode: Set if time-series can or not be manually/automatically written in Wizata.
-    :ivar dict extra_properties: Add any custom properties to your datapoints as a key/value pair dictionary.
+    :ivar model_id: The UUID of the ML Model.
+    :ivar key: Logical String ID of the Model
+    :ivar generatedById: The UUID of the Execution from which the ML Model was created.
+    :ivar status: 'draft', 'valid' or 'invalid' - When generated model are tested by API, only valid model can be used.
+    :ivar needExactColumnNumbers: True by default, define if the model requires exact columns numbers to be executed.
+    :ivar needExactColumnNames: True by default, define if the model requires exact columns names to be executed.
+    :ivar has_anomalies: False by default, define if a model generate potential anomalies.
+    :ivar has_target_feat: False by default, define if a model requires a target features to be trained or executed.
+    :ivar input_columns: list of all columns used to trained the model.
+    :ivar output_columns: list of all columns generated by the model.
+    :ivar label_counts: Count of labels generated by the model.
+    :ivar trained_model: The Trained model
+    :ivar scaler: The scaler
     """
 
     @classmethod
     def route(cls):
-        return "datapoints"
+        return "mlmodels"
 
     @classmethod
     def from_dict(cls, data):
-        obj = DataPoint()
+        obj = MLModel()
         obj.from_json(data)
         return obj
 
-    def __init__(self,
-                 datapoint_id: uuid.UUID = None,
-                 hardware_id: str = None,
-                 business_type: BusinessType = None,
-                 name: str = None,
-                 twin_id: uuid.UUID = None,
-                 unit_id: uuid.UUID = None,
-                 category_id: uuid.UUID = None,
-                 description: str = None,
-                 min_value: float = None,
-                 max_value: float = None,
-                 frequency: int = None,
-                 input_mode: InputModeType = None,
-                 extra_properties: dict = None):
-        if datapoint_id is None:
-            self.datapoint_id = uuid.uuid4()
-        else:
-            self.datapoint_id = datapoint_id
-        self.hardware_id = hardware_id
-        self.name = name
-        self.business_type = business_type
-        self.twin_id = twin_id
-        self.unit_id = unit_id
-        self.category_id = category_id
-        self.description = description
-        self.min_value = min_value
-        self.max_value = max_value
-        self.frequency = frequency
-        self.input_mode = input_mode
-        self.extra_properties = extra_properties
+    @classmethod
+    def operations(cls):
+        return ['lists', 'get_by_id', 'get_by_key', 'delete']
+
+    @classmethod
+    def get_type(cls):
+        return "pickle"
+
+    def __init__(self, model_id=None, generated_by_id=None,
+                 exact_names=True, exact_numbers=True,
+                 key=None):
+        if model_id is None:
+            model_id = uuid.uuid4()
+        self.model_id = model_id
+        self.key = key
+
+        self.generatedById = generated_by_id
+
+        self.status = 'draft'
+        self.input_columns = []
+        self.output_columns = []
+
+        self.needExactColumnNumbers = exact_numbers
+        self.needExactColumnNames = exact_names
+        self.has_anomalies = False
+        self.label_counts = 0
+        self.has_target_feat = False
+
+        self.trained_model = None
+        self.scaler = None
+
+        self.experimentId = None
 
     def api_id(self) -> str:
         """
-        formatted id of the datapoint (datapoint_id)
-        :return: string formatted UUID of the DataPoint.
+        Id of the ML Model (model_id)
+
+        :return: string formatted UUID of the Model ID.
         """
-        return str(self.datapoint_id).upper()
+        return str(self.model_id).upper()
 
     def endpoint(self) -> str:
         """
-        endpoint name used to manipulate datapoint on backend.
-        :return: endpoint name.
+        Name of the endpoints used to manipulate ML Models.
+        :return: Endpoint name.
         """
-        return "DataPoints"
+        return "MLModels"
+
+    def to_json(self, target: str = None):
+        obj = {"id": str(self.model_id),
+               "status": str(self.status),
+               "needExactColumnNames": str(self.needExactColumnNames),
+               "needExactColumnNumbers": str(self.needExactColumnNumbers),
+               "hasAnomalies": str(self.has_anomalies),
+               "hasTargetFeat": str(self.has_target_feat),
+               "labelCount": str(self.label_counts)
+               }
+        if self.key is not None:
+            obj["key"] = str(self.key)
+        if self.generatedById is not None:
+            obj["generatedById"] = str(self.generatedById)
+        if self.input_columns is not None:
+            obj["inputColumns"] = json.dumps(list(self.input_columns))
+        if self.output_columns is not None:
+            obj["outputColumns"] = json.dumps(list(self.output_columns))
+        if self.experimentId is not None:
+            obj["experimentId"] = str(self.experimentId)
+        return obj
 
     def from_json(self, obj):
         """
-        load the datapoint entity from a dictionary.
-        :param obj: dict version of the datapoint.
+        Load the ML Model entity from a dictionary representation of the ML Model.
+
+        :param obj: Dict version of the ML Model.
         """
         if "id" in obj.keys():
-            self.datapoint_id = uuid.UUID(obj["id"])
-
-        if "hardwareId" in obj.keys():
-            self.hardware_id = obj["hardwareId"]
-
-        if "name" in obj.keys():
-            self.name = obj["name"]
-
-        if "businessType" in obj.keys():
-            self.business_type = BusinessType(str(obj["businessType"]))
-
-        if "twinId" in obj.keys() and obj["twinId"] is not None:
-            self.twin_id = uuid.UUID(obj["twinId"])
-
-        if "unitId" in obj.keys() and obj["unitId"] is not None:
-            self.unit_id = uuid.UUID(obj["unitId"])
-
-        if "categoryId" in obj.keys() and obj["categoryId"] is not None:
-            self.category_id = uuid.UUID(obj["categoryId"])
-
-        if "description" in obj.keys() and obj["description"] is not None:
-            self.description = obj["description"]
-
-        if "minValue" in obj.keys() and obj["minValue"] is not None:
-            self.min_value = float(obj["minValue"])
-
-        if "maxValue" in obj.keys() and obj["maxValue"] is not None:
-            self.max_value = float(obj["maxValue"])
-
-        if "frequency" in obj.keys() and obj["frequency"] is not None:
-            self.frequency = int(obj["frequency"])
-
-        if "inputMode" in obj.keys():
-            self.input_mode = InputModeType(str(obj["inputMode"]))
-
-        if "extraProperties" in obj.keys():
-            if isinstance(obj["extraProperties"], str):
-                self.extra_properties = json.loads(obj["extraProperties"])
+            self.model_id = obj["id"]
+        if "key" in obj.keys() and obj["key"] is not None:
+            self.key = obj["key"]
+        if "generatedById" in obj.keys() and obj["generatedById"] is not None:
+            self.generatedById = uuid.UUID(obj["generatedById"])
+        if "experimentId" in obj.keys() and obj["experimentId"] is not None:
+            self.experimentId = uuid.UUID(obj["experimentId"])
+        if "status" in obj.keys():
+            self.status = str(obj["status"]).lower()
+        if "inputColumns" in obj.keys():
+            self.input_columns = json.loads(obj["inputColumns"])
+        if "outputColumns" in obj.keys():
+            self.output_columns = json.loads(obj["outputColumns"])
+        if "labelCount" in obj.keys():
+            self.label_counts = int(obj["labelCount"])
+        if "hasAnomalies" in obj.keys():
+            if isinstance(obj["hasAnomalies"], str) and obj["hasAnomalies"].lower() == "false":
+                self.has_anomalies = False
+            else:
+                self.has_anomalies = bool(obj["hasAnomalies"])
+        if "hasTargetFeat" in obj.keys():
+            if isinstance(obj["hasTargetFeat"], str) and obj["hasTargetFeat"].lower() == "false":
+                self.has_target_feat = False
+            else:
+                self.has_target_feat = bool(obj["hasTargetFeat"])
+        if "needExactColumnNumbers" in obj.keys():
+            if isinstance(obj["needExactColumnNumbers"], str) and obj["needExactColumnNumbers"].lower() == "false":
+                self.needExactColumnNumbers = False
             else:
-                self.extra_properties = obj["extraProperties"]
+                self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
+        if "needExactColumnNames" in obj.keys():
+            if isinstance(obj["needExactColumnNames"], str) and obj["needExactColumnNames"].lower() == "false":
+                self.needExactColumnNames = False
+            else:
+                self.needExactColumnNames = bool(obj["needExactColumnNames"])
 
-    def to_json(self, target: str = None):
+    def get_sample_payload(self):
         """
-        convert the datapoint to a dictionary compatible with JSON format.
-        :return: dictionary representation of the datapoint object.
+        Get a JSON formatted sample payload to call the ML Model.
+        :return: JSON formatted sample payload.
         """
-        obj = {
-            "id": str(self.datapoint_id),
-            "hardwareId": str(self.hardware_id)
+        pl_columns = {"timestamp": "[timestamp]"}
+        for hardwareId in self.input_columns:
+            pl_columns[hardwareId] = "[" + hardwareId + "]"
+        pl_json = {
+            "id": str(self.model_id),
+            "dataset": pl_columns
         }
-        if self.business_type is not None and isinstance(self.business_type, BusinessType):
-            obj["businessType"] = self.business_type.value
-        if self.input_mode is not None and isinstance(self.input_mode, InputModeType):
-            obj["inputMode"] = self.input_mode.value
-        if self.twin_id is not None:
-            obj["twinId"] = str(self.twin_id)
-        if self.unit_id is not None:
-            obj["unitId"] = str(self.unit_id)
-        if self.category_id is not None:
-            obj["categoryId"] = str(self.category_id)
-        if self.description is not None and self.description != "":
-            obj["description"] = self.description
-        if self.name is not None and self.name != "":
-            obj["name"] = self.name
-        if self.max_value is not None:
-            obj["maxValue"] = self.max_value
-        if self.min_value is not None:
-            obj["minValue"] = self.min_value
-        if self.frequency is not None:
-            obj["frequency"] = self.frequency
-        if self.extra_properties is not None:
-            if not isinstance(self.extra_properties, dict):
-                raise ValueError('on datapoint extra properties must be None or a JSON serializable dict')
-            obj["extraProperties"] = json.dumps(self.extra_properties)
-        return obj
+        return pl_json
+
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.4.9/wizata_dsapi/ds_dataframe.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,18 @@
     @classmethod
     def from_dict(cls, data):
         obj = DSDataFrame()
         obj.from_json(data)
         return obj
 
     @classmethod
+    def operations(cls):
+        return ['lists', 'get_by_id', 'get_by_key', 'delete']
+
+    @classmethod
     def get_type(cls):
         return "pickle"
 
     def __init__(self, df_id=None, dataframe=None):
         if df_id is None:
             self.df_id = uuid.uuid4()
         else:
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.4.9/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/execution.py` & `wizata-dsapi-0.4.9/wizata_dsapi/template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,327 +1,320 @@
-import json
 import uuid
-from enum import Enum
-
-from .api_dto import ApiDto
-from .pipeline import Pipeline
-from .experiment import Experiment
-
-
-class AbortedException(Exception):
-    """
-    exception to trigger within a custom script to 'abort' a pipeline instead of failing it.
-    """
-    pass
+import json
 
+import wizata_dsapi
 
-class ExecutionStatus(Enum):
-    """
-    ExecutionStatus defines different status possible for an execution.
-        - "received" default status when execution is created initially.
-        - "queued" execution have been put in the queue.
-        - "started" a runner have started processing the execution.
-        - "completed" execution finished processing as expected.
-        - "failed" execution finished with errors.
-        - "aborted" execution was cancelled from expected or manual conditions.
-        - "abortrequested" set on an execution queued to force its abortion as soon as a runner start processing it.
-    """
-    RECEIVED = "received"
-    QUEUED = "queued"
-    STARTED = "started"
-    COMPLETED = "completed"
-    FAILED = "failed"
-    ABORTED = "aborted"
-    ABORT_REQUESTED = "abortrequested"
+from .api_dto import ApiDto
+from .pipeline import VarType
 
 
-class ExecutionStepLog(ApiDto):
-    """
-    execution Step Log defines result of a specific step processing (only for execution in experiment mode).
-    :ivar uuid.UUID execution_step_log_id: technical id of an execution step log.
-    :ivar str content: str representing result of this execution.
-    :ivar uuid.UUID execution_id: parent execution id.
-    :ivar wizata_dsapi.ExecutionStatus status: status of this execution step log.
-    :ivar uuid.UUID step_id: technical id of the pipeline step.
-    :ivar uuid.UUID createdById: unique identifier of creating user.
-    :ivar int createdDate: timestamp of created date.
-    :ivar uuid.UUID updatedById: unique identifier of updating user.
-    :ivar int updatedDate: timestamp of updated date.
-    """
+class TemplateProperty(ApiDto):
 
-    def __init__(self, execution_step_log_id=None, step_id=None, execution_id=None, content=None, status=None):
-        if execution_step_log_id is None:
-            execution_step_log_id = uuid.uuid4()
-        self.execution_step_log_id = execution_step_log_id
-        self.execution_id = execution_id
-        self.step_id = step_id
-        self.content = content
-        self.status = status
+    def __init__(self,
+                 template_property_id: uuid.UUID = None,
+                 name: str = None,
+                 description: str = None,
+                 p_type: VarType = None,
+                 required: bool = True,
+                 template_id: uuid.UUID = None):
+        if template_property_id is None:
+            self.template_property_id = uuid.uuid4()
+        else:
+            self.template_property_id = template_property_id
+        self.description = description
+        self.template_id = template_id
+        self.name = name
+        self.p_type = p_type
+        self.required = required
         self.createdById = None
         self.createdDate = None
         self.updatedById = None
         self.updatedDate = None
 
     def api_id(self) -> str:
         """
-        formatted id of the expected_step_log (execution_step_log_id)
-        :return: string formatted UUID of the ExecutionStepLog.
+        Id of the Template Property (template_property_id)
+
+        :return: string formatted UUID of the template property.
         """
-        return str(self.execution_step_log_id).upper()
+        return str(self.template_property_id).upper()
 
     def endpoint(self) -> str:
         """
-        endpoint name used to manipulate execution step log on backend.
-        :return: endpoint name.
+        Name of the endpoints used to manipulate template properties.
+        :return: Endpoint name.
         """
-        return "ExecutionStepLogs"
-
-    def to_json(self, target: str = None):
-        """
-        convert the execution step log to a dictionary compatible with JSON format.
-        :return: dictionary representation of the execution step log object.
-        """
-        obj = {
-            "id": str(self.execution_step_log_id)
-        }
-        if self.execution_id is not None:
-            obj["executionId"] = str(self.execution_id)
-        if self.step_id is not None:
-            obj["stepId"] = str(self.step_id)
-        if self.content is not None:
-            obj["content"] = json.dumps(self.content)
-        if self.createdById is not None:
-            obj["createdById"] = self.createdById
-        if self.createdDate is not None:
-            obj["createdDate"] = self.createdDate
-        if self.updatedById is not None:
-            obj["updatedById"] = self.updatedById
-        if self.updatedDate is not None:
-            obj["updatedDate"] = self.updatedDate
-        if self.status is not None and isinstance(self.status, ExecutionStatus):
-            obj["status"] = self.status.value
-        return obj
+        return "TemplateProperties"
 
     def from_json(self, obj):
-        """
-        load the execution step log entity from a dictionary.
-        :param obj: dict version of the datapoint.
-        """
         if "id" in obj.keys():
-            self.execution_step_log_id = uuid.UUID(obj["id"])
-        if "executionId" in obj.keys() and obj["executionId"] is not None:
-            self.execution_id = uuid.UUID(obj["executionId"])
-        if "stepId" in obj.keys() and obj["stepId"] is not None:
-            self.step_id = uuid.UUID(obj["stepId"])
-        if "content" in obj.keys() and obj["content"] is not None:
-            if isinstance(obj["content"], str):
-                self.content = json.loads(obj["content"])
-            else:
-                self.content = obj["content"]
-        if "status" in obj.keys():
-            self.status = ExecutionStatus(str(obj["status"]))
+            self.template_property_id = uuid.UUID(obj["id"])
+        if "name" in obj.keys():
+            self.name = obj["name"]
+        if "type" in obj.keys() and obj["type"] is not None:
+            self.p_type = VarType(obj["type"])
+        if "required" in obj.keys() and obj["required"] is not None:
+            if not isinstance(obj["required"], bool):
+                raise TypeError(f'template property field "required" should be a valid boolean')
+            self.required = obj["required"]
+        else:
+            self.required = True
+        if "description" in obj.keys():
+            self.description = obj["description"]
+        if "templateId" in obj.keys():
+            self.template_id = uuid.UUID(obj["templateId"])
         if "createdById" in obj.keys() and obj["createdById"] is not None:
             self.createdById = obj["createdById"]
         if "createdDate" in obj.keys() and obj["createdDate"] is not None:
             self.createdDate = obj["createdDate"]
         if "updatedById" in obj.keys() and obj["updatedById"] is not None:
             self.updatedById = obj["updatedById"]
         if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
             self.updatedDate = obj["updatedDate"]
 
+    def to_json(self, target: str = None):
+        """
+        Convert the template to a dictionary compatible to JSON format.
 
-class Execution(ApiDto):
+        :return: dictionary representation of the Template object.
+        """
+        obj = {
+            "id": str(self.template_property_id)
+        }
+        if self.name is not None:
+            obj["name"] = str(self.name)
+        if self.description is not None:
+            obj["description"] = str(self.description)
+        if self.p_type is not None:
+            obj["type"] = str(self.p_type.value)
+        if self.required is not None:
+            if not isinstance(self.required, bool):
+                raise TypeError(f'template property field "required" should be a valid boolean')
+            obj["required"] = self.required
+        if self.template_id is not None:
+            obj["templateId"] = str(self.template_id)
+        if self.createdById is not None:
+            obj["createdById"] = str(self.createdById)
+        if self.createdDate is not None:
+            obj["createdDate"] = str(self.createdDate)
+        if self.updatedById is not None:
+            obj["updatedById"] = str(self.updatedById)
+        if self.updatedDate is not None:
+            obj["updatedDate"] = str(self.updatedDate)
+        return obj
+
+
+class Template(ApiDto):
     """
-    execution keeps all information on time, status and results of a specific pipeline manual or automatic run.
+    Template of a solution and/or asset.
 
-    :ivar uuid.UUID execution_id: technical id of execution.
-    :ivar int execution_time: duration of the execution from started.
-    :ivar uuid.UUID experiment_id: experiment id used in experiment mode.
-    :ivar uuid.UUID pipeline_id: pipeline id executed or to execute.
-    :ivar dict properties: configuration, parameters and variables (only accessible from front-end to DS api).
-    :ivar int queued_date: timestamp on which execution is queued, if none use createdDate
-    :ivar int started_date: timestamp on which execution is started.
-    :ivar wizata_dsapi.ExecutionStatus status: execution status.
-    :ivar uuid.UUID template_id: template id linked to the pipeline.
-    :ivar uuid.UUID trigger_id: trigger id used if automatic run.
-    :ivar uuid.UUID twin_id: twin id registered on the template to run pipeline on.
-    :ivar int waiting_time: duration of the waiting time in the queue.
-    :ivar list warnings: list of error and/or warning messages.
+    :ivar template_id: UUID of the Template.
+    :ivar key: str unique id identifying the Template.
+    :ivar name: logical display name of the Template.
+    :ivar properties: list of Property { type , name } of the solution.
+
+    Properties only support type 'datapoint', 'float', 'integer', 'json', 'datetime', 'relative' or 'string'
     """
 
     @classmethod
     def route(cls):
-        return "execute"
+        return "templates"
 
     @classmethod
     def from_dict(cls, data):
-        obj = Execution()
+        obj = Template()
         obj.from_json(data)
         return obj
 
-    def __init__(self,
-                 execution_id=None,
-                 properties: dict = None,
-                 pipeline: Pipeline = None,
-                 pipeline_id: uuid.UUID = None,
-                 experiment: Experiment = None,
-                 experiment_id: uuid.UUID = None,
-                 twin_id: uuid.UUID = None,
-                 template_id: uuid.UUID = None,
-                 trigger_id: uuid.UUID = None):
-
-        # Id
-        if execution_id is None:
-            execution_id = uuid.uuid4()
-        self.execution_id = execution_id
-
-        # Experiment
-        if experiment is not None:
-            self.experiment_id = experiment.experiment_id
-        else:
-            self.experiment_id = experiment_id
-
-        # Trigger
-        self.trigger_id = trigger_id
-        self.twin_id = twin_id
-        self.template_id = template_id
+    @classmethod
+    def operations(cls):
+        return ['lists', 'get_by_id', 'get_by_key', 'create', 'update', 'delete']
 
-        # Pipeline
-        if pipeline is not None:
-            self.pipeline_id = pipeline.pipeline_id
+    def __init__(self, template_id=None, key=None, name=None, properties=None):
+        if template_id is None:
+            self.template_id = uuid.uuid4()
         else:
-            self.pipeline_id = pipeline_id
-
-        # Status and info
-        self.status = None
-        self.queued_date = None
-        self.started_date = None
-        self.execution_time = None
-        self.waiting_time = None
-        self.warnings = None
-
-        # Only accessible between Front-End and DS API (not backend)
+            self.template_id = template_id
+        self.key = key
+        self.name = name
         if properties is None:
-            properties = {}
+            properties = []
         self.properties = properties
-
-        # created/updated
         self.createdById = None
         self.createdDate = None
         self.updatedById = None
         self.updatedDate = None
 
-        # outputs (only accessible within runners)
-        self.models = []
-        self.plots = []
-        self.dataframes = []
-
     def api_id(self) -> str:
-        return str(self.execution_id).upper()
-
-    def endpoint(self) -> str:
-        return "Executions"
-
-    def to_json(self, target: str = None):
-        obj = {
-            "id": str(self.execution_id)
-        }
-
-        # Experiment
-        if self.experiment_id is not None:
-            obj["experimentId"] = str(self.experiment_id)
-
-        # Pipeline
-        if self.pipeline_id is not None:
-            obj["pipelineId"] = str(self.pipeline_id)
-
-        # Trigger , Twin & Template
-        if self.trigger_id is not None:
-            obj["executionTriggerId"] = str(self.trigger_id)
-        if self.template_id is not None:
-            obj["templateId"] = str(self.template_id)
-        if self.twin_id is not None:
-            obj["twinId"] = str(self.twin_id)
-
-        # Status and info
-        if self.queued_date is not None:
-            obj["queuedDate"] = self.queued_date
-        if self.started_date is not None:
-            obj["startedDate"] = self.started_date
-        if self.execution_time is not None:
-            obj["executionTime"] = self.execution_time
-        if self.waiting_time is not None:
-            obj["waitingTime"] = self.waiting_time
-        if self.warnings is not None:
-            obj["warnings"] = self.warnings
-        if self.status is not None and isinstance(self.status, ExecutionStatus):
-            obj["status"] = self.status.value
-
-        # Properties (DS API/Front-End only)
-        if self.properties is not None and target is None:
-            obj["properties"] = json.dumps(self.properties)
+        """
+        Id of the Template (template_id)
 
-        # created/updated
-        if self.createdById is not None:
-            obj["createdById"] = self.createdById
-        if self.createdDate is not None:
-            obj["createdDate"] = self.createdDate
-        if self.updatedById is not None:
-            obj["updatedById"] = self.updatedById
-        if self.updatedDate is not None:
-            obj["updatedDate"] = self.updatedDate
+        :return: string formatted UUID of the template.
+        """
+        return str(self.template_id).upper()
 
-        return obj
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate templates.
+        :return: Endpoint name.
+        """
+        return "Templates"
 
     def from_json(self, obj):
-        if "id" in obj.keys():
-            self.execution_id = uuid.UUID(obj["id"])
-
-        # Experiment
-        if "experimentId" in obj.keys() and obj["experimentId"] is not None:
-            self.experiment_id = uuid.UUID(obj["experimentId"])
-
-        # Pipeline
-        if "pipelineId" in obj.keys() and obj["pipelineId"] is not None:
-            self.pipeline_id = uuid.UUID(obj["pipelineId"])
-
-        # Trigger , Twin & Template
-        if "twinId" in obj.keys() and obj["twinId"] is not None:
-            self.twin_id = uuid.UUID(obj["twinId"])
-        if "templateId" in obj.keys() and obj["templateId"] is not None:
-            self.template_id = uuid.UUID(obj["templateId"])
-        if "executionTriggerId" in obj.keys() and obj["executionTriggerId"] is not None:
-            self.trigger_id = uuid.UUID(obj["executionTriggerId"])
-
-        # Status and Info
-        if "queuedDate" in obj.keys() and obj["queuedDate"] is not None:
-            self.queued_date = int(obj["queuedDate"])
-        if "startedDate" in obj.keys() and obj["startedDate"] is not None:
-            self.started_date = int(obj["startedDate"])
-        if "waitingTime" in obj.keys() and obj["waitingTime"] is not None:
-            self.waiting_time = int(obj["waitingTime"])
-        if "executionTime" in obj.keys() and obj["executionTime"] is not None:
-            self.execution_time = int(obj["executionTime"])
-        if "warnings" in obj.keys() and obj["warnings"] is not None:
-            self.warnings = obj["warnings"]
-        if "status" in obj.keys():
-            self.status = ExecutionStatus(str(obj["status"]))
+        """
+        Load the Template entity from a dictionary.
 
-        # Properties
+        :param obj: Dict version of the Template.
+        """
+        if "id" in obj.keys():
+            self.template_id = uuid.UUID(obj["id"])
+        if "key" in obj.keys() and obj["key"] is not None:
+            self.key = obj["key"]
+        if "name" in obj.keys() and obj["name"] is not None:
+            self.name = obj["name"]
         if "properties" in obj.keys() and obj["properties"] is not None:
             if isinstance(obj["properties"], str):
-                if obj["properties"] == '':
-                    self.properties = {}
-                self.properties = json.loads(obj["properties"])
+                properties = json.loads(obj["properties"])
             else:
-                self.properties = obj["properties"]
-
-        # created/updated
+                properties = obj["properties"]
+            # add properties to add method to ensure unicity of name and validity of type
+            for to_add in properties:
+                self.add_property(to_add)
         if "createdById" in obj.keys() and obj["createdById"] is not None:
             self.createdById = obj["createdById"]
         if "createdDate" in obj.keys() and obj["createdDate"] is not None:
             self.createdDate = obj["createdDate"]
         if "updatedById" in obj.keys() and obj["updatedById"] is not None:
             self.updatedById = obj["updatedById"]
         if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
             self.updatedDate = obj["updatedDate"]
 
+    def to_json(self, target: str = None):
+        """
+        Convert the template to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Template object.
+        """
+        obj = {
+            "id": str(self.template_id)
+        }
+        if self.key is not None:
+            obj["key"] = str(self.key)
+        if self.name is not None:
+            obj["name"] = str(self.name)
+        if self.properties is not None:
+            obj_properties = []
+            template_property: TemplateProperty
+            for template_property in self.properties:
+                obj_properties.append(template_property.to_json())
+            obj["properties"] = json.dumps(obj_properties)
+        if self.createdById is not None:
+            obj["createdById"] = str(self.createdById)
+        if self.createdDate is not None:
+            obj["createdDate"] = str(self.createdDate)
+        if self.updatedById is not None:
+            obj["updatedById"] = str(self.updatedById)
+        if self.updatedDate is not None:
+            obj["updatedDate"] = str(self.updatedDate)
+        return obj
+
+    def add(self, name: str, p_type: VarType, required: bool = True,
+            template_property_id: uuid.UUID = None, description: str = None):
+        """
+        add a property from detailed information.
+        """
+
+        if self.properties is None:
+            self.properties = []
+
+        if name is None or p_type is None:
+            raise ValueError('please set a name and a type for property')
+
+        property_value = TemplateProperty(
+            template_property_id=template_property_id,
+            name=name,
+            p_type=p_type,
+            required=required,
+            description=description
+        )
+        property_value.template_id = self.template_id
+
+        existing_property: TemplateProperty
+        for existing_property in self.properties:
+            if existing_property.name == property_value.name:
+                raise ValueError(f'property {property_value.name} already exists in template.')
+
+        self.properties.append(property_value)
+
+    def get_property(self, property_name) -> TemplateProperty:
+        """
+        get a property from its name.
+        :param property_name: name of the property.
+        """
+        for t_property in self.properties:
+            if t_property.name == property_name:
+                return t_property
+
+    def add_property(self, property_value):
+        """
+        add a property in list of properties
+        by default - a property is required
+        :param property_value: dict or TemplateProperty
+        """
+        if isinstance(property_value, dict):
+            if "type" not in property_value:
+                raise KeyError("property must have a type.")
+            p_type = VarType(property_value['type'])
+
+            if "name" not in property_value:
+                raise KeyError("property must have a name")
+            name = property_value["name"]
+
+            template_property_id = None
+            if "id" in property_value:
+                if isinstance(property_value['id'], str):
+                    template_property_id = uuid.UUID(property_value['id'])
+                elif isinstance(property_value['id'], uuid.UUID):
+                    template_property_id = property_value['id']
+                else:
+                    raise ValueError('id must be a valid str or UUID')
+
+            required = True
+            if "required" in property_value:
+                required = property_value["required"]
+
+            description = None
+            if "description" in property_value:
+                description = property_value["description"]
+
+            self.add(template_property_id=template_property_id,
+                     name=name,
+                     p_type=p_type,
+                     required=required,
+                     description=description)
+        elif isinstance(property_value, TemplateProperty):
+            property_value.template_id = self.template_id
+
+            for existing_property in self.properties:
+                if existing_property.name == property_value.name:
+                    raise ValueError(f'property {property_value.name} already exists in template.')
+
+            self.properties.append(property_value)
+        else:
+            raise ValueError('property must be a dict or a TemplateProperty')
+
+    def remove_property(self, name: str):
+        """
+        remove a property from the list based on its name
+        :param name: property to remove
+        """
+        found_property = None
+
+        existing_property: TemplateProperty
+        for existing_property in self.properties:
+            if existing_property.name == name:
+                found_property = existing_property
+
+        if self.properties is not None and found_property is not None:
+            self.properties.remove(found_property)
+
+
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.4.9/wizata_dsapi/model_toolkit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pandas
 from .mlmodel import MLModel
 
 
 def predict(df: pandas.DataFrame, ml_model: MLModel, mapping_table=None):
     """
     Execute a Machine Learning models locally.
+
     :param df: dataframe to use as input.
     :param ml_model: trained machine learning model.
     :param mapping_table: Optional mapping table.
     :return: output dataframe with predicted values.
     """
     if ml_model is None or ml_model.trained_model is None or ml_model.input_columns is None:
         raise ValueError("Please download your model from DS API before using it.")
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/plot.py` & `wizata-dsapi-0.4.9/wizata_dsapi/plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import uuid
 from .api_dto import ApiDto
 
 
 class Plot(ApiDto):
     """
     A plot is a definition of a Plotly figure that can be stored and shared on Wizata.
+
     :ivar plot_id: The UUID of the plot.
     :ivar generatedById: The UUID of the Execution from which the plot was created.
     :ivar name: A simple name helping the user identifying the plot.
     :ivar figure: Plotly figure defining the plot itself.
     """
 
     @classmethod
@@ -17,55 +18,62 @@
 
     @classmethod
     def from_dict(cls, data):
         obj = Plot()
         obj.from_json(data)
         return obj
 
+    @classmethod
+    def operations(cls):
+        return ['lists', 'get_by_id', 'get_by_key', 'delete']
+
     def __init__(self, plot_id=None, name=None, generated_by_id=None, figure=None):
         if plot_id is None:
             self.plot_id = uuid.uuid4()
         else:
             self.plot_id = plot_id
         self.name = name
         self.generatedById = generated_by_id # Execution
         # Step Id
         self.figure = figure
 
     def api_id(self) -> str:
         """
         Id of the plot (plot_id)
+
         :return: string formatted UUID of the plot.
         """
         return str(self.plot_id).upper()
 
     def endpoint(self) -> str:
         """
         Name of the endpoints used to manipulate plots.
         :return: Endpoint name.
         """
         return "Plots"
 
     def from_json(self, obj):
         """
         Load the Plot entity from a dictionary representation of the Plot.
+
         :param obj: Dict version of the Plot.
         """
         if "id" in obj.keys():
             self.plot_id = uuid.UUID(obj["id"])
         if "name" in obj.keys():
             self.name = obj["name"]
         if "figure" in obj.keys():
             self.figure = obj["figure"]
         if "generatedById" in obj.keys():
             self.generatedById = obj["generatedById"]
 
     def to_json(self, target: str = None):
         """
         Convert the plot to a dictionary compatible to JSON format.
+
         :return: dictionary representation of the Plot object.
         """
         obj = {
             "id": str(self.plot_id)
         }
         if self.name is not None:
             obj["name"] = self.name
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/request.py` & `wizata-dsapi-0.4.9/wizata_dsapi/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,49 @@
     '==':'eq',
     '!=':'neq'
 }
 
 
 class Request(ApiDto):
     """
-    request defines how to fetch data from time-series database.
+    A Request to fetch dataframes from Wizata App.
 
-    :ivar list datapoints: list of str pointing to hardware ids of datapoint or template properties name.
-    :ivar datetime|str start: start range to fetch set as a datetime, a @parameter or str relative format (e.g. 'now-1d')
-    :ivar datetime|str end: start range to fetch set as a datetime, a @parameter or str relative format (e.g. 'now')
-    :ivar str aggregation: aggregation method ("mean", "stddev", "mode", "median", "count", "sum", "first", "last", "max", "min").
-    :ivar int interval: interval passed in seconds at __init__ (stored as milliseconds).
-    :ivar uuid.UUID template_id: use technical id of wizata_dsapi.Template to fetch data based on a template.
-    :ivar uuid.UUID twin_id: technical id of wizata_dsapi.Twin registered on template_id.
-    :ivar dict filters: filters to apply to the query pre-aggregation. nested dictionary using as first key=datapoint then value=another dictionary with key=operator (gt,lt,gte,lte,eq,neq) and value is the float value to compare too).
-    :ivar dict options: dict representing query options.
+    To execute the request please use a DS API client.
+
+    :ivar equipments: List of Equipments containing Digital Twin item and datapoints to fetch.
+
+    :ivar template_id: UUID of the template.
+    :ivar template: str unique id of the template.
+    :ivar twin_id: UUID of the Digital Twin.
+    :ivar twin: str hardware id of the Digital Twin.
+
+    :ivar start: Datetime defining beginning of period.
+    :ivar end: Datetime defining end of period.
+    :ivar aggregation: Aggregation method to fetch, accept "mean" and "stddev".
+    :ivar interval: Interval in seconds between each aggregation.
+    :ivar filters: Filter to apply on the query (not yet fully implemented).
+    :ivar connections: Connections rules between equipment to align data in time (not yet fully implemented).
+    :ivar null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
     """
 
     @classmethod
     def route(cls):
         return "data"
 
     @classmethod
     def from_dict(cls, data):
         obj = Request()
         obj.from_json(data)
         return obj
 
     @classmethod
+    def operations(cls):
+        return ['query']
+
+    @classmethod
     def get_type(cls):
         return "pickle"
 
     def __init__(self,
                  datapoints=None,
                  start=None,
                  end=None,
@@ -94,16 +105,17 @@
         self.connections = None
         self.name = None
 
         self.null = null
 
     def prepare(self):
         """
-        prepare analyse the query and produce a dict with query information.
-        :return: dict
+        prepare a dict JSON compatible only for the QUERY part of the request.
+
+        :return: a dict JSON compatible
         """
         query = {}
         if self.request_id is not None:
             query["id"] = str(self.request_id)
         if self.equipments is not None:
             query["equipments_list"] = self.equipments
         else:
@@ -150,58 +162,57 @@
             millisec = dt_to_format.timestamp() * 1000
             return int(millisec)
         else:
             raise TypeError("date is not a valid datetime")
 
     def start_time(self, now=None) -> datetime:
         """
-        convert a relative start time to a datetime based on a now parameter.
+        get start time
         :param now: override now value for relative datetime
         :return: start datetime
         """
         if self.start is None:
             raise ValueError('missing start datetime')
         elif isinstance(self.start, str):
             return datetime.fromtimestamp(generate_epoch(self.start, now=now) / 1000, timezone.utc)
         elif isinstance(self.start, datetime):
             return self.start
         else:
             raise TypeError(f'unsupported start datetime type {self.start.__class__.__name__}')
 
     def end_time(self, now=None) -> datetime:
         """
-        convert a relative end time to a datetime based on a now parameter.
+        get end time
         :param now: override now value for relative datetime
-        :return: end datetime
+        :return: start datetime
         """
         if self.end is None:
             raise ValueError('missing end datetime')
         elif isinstance(self.end, str):
             return datetime.fromtimestamp(generate_epoch(self.end, now=now) / 1000, timezone.utc)
         elif isinstance(self.end, datetime):
             return self.end
         else:
             raise TypeError(f'unsupported end datetime type {self.end.__class__.__name__}')
 
     def add_datapoints(self, datapoints, shift: int = 0):
         """
-        add datapoints to existing list of datapoints in the query.
-        :param datapoints:  datapoints to fetch identified by hardware id or template property name.
-        :param shift: shift to apply in seconds on timestamp, by default 0.
+        Add datapoints to fetch without defining its equipments.
+        :param datapoints: List(str) of datapoints to fetch identified by Hardware ID.
+        :param shift: Shift to apply in seconds on timestamp, by default 0.
         """
         self.equipments.append({
             "id": None,
             "datapoints": list(datapoints),
             "shift": str(shift) + "s"
         })
 
     def get_datapoints(self) -> list:
         """
-        get datapoints
-        :return: list of declared datapoints.
+        return list of declared datapoints.
         """
         datapoints = []
 
         if self.equipments is not None:
             for equipment in self.equipments:
                 if "datapoints" not in equipment.keys():
                     raise KeyError("No 'data points' have been provided for equipment with id '" +
@@ -222,15 +233,15 @@
         """
         self.equipments = []
         if datapoints is not None:
             self.add_datapoints(datapoints)
 
     def add_equipment(self, equipment_id: uuid.UUID, datapoints, shift=0):
         """
-        add datapoints to fetch with a digital twin id identification.
+        Add datapoints to fetch with a Digital Twin ID identification.
         :param equipment_id: UUID of the Digital Twin ID to which the datapoints are linked.
         :param datapoints: List(str) of datapoints to fetch identified by Hardware ID.
         :param shift: Shift to apply in seconds on timestamp, by default 0.
         """
         if not isinstance(equipment_id, uuid.UUID):
             raise TypeError("equipment_id must be of type uuid.UUID")
         for equipment in self.equipments:
@@ -238,56 +249,57 @@
                 raise ValueError("equipment_id is already in the request please remove it before adding datapoints.")
         self.equipments.append({
             "id": str(equipment_id),
             "datapoints": list(datapoints),
             "shift": str(shift) + "s"
         })
 
+    # attempt to remove equipment from the query if exists
     def remove_equipment(self, equipment_id: uuid.UUID):
         """
-        remove equipment from the list including all its listed datapoints.
+        Remove an equipment from the list including all its listed datapoints.
         :param equipment_id: UUID of the Digital Twin item.
         """
         if equipment_id is not None and not isinstance(equipment_id, uuid.UUID):
             raise TypeError("equipment_id must be None or of type uuid.UUID")
         found = None
         for equipment in self.equipments:
             if "id" in equipment.keys() and equipment["id"] == str(equipment_id):
                 found = equipment
         if found is not None:
             self.equipments.remove(equipment)
 
     def set_aggregation(self, method, interval):
         """
-        specifies aggregation properties
-        :param method: "mean", "stddev", "mode", "median", "count", "sum", "first", "last", "max" or "min"
+        Specifies aggregation properties
+        :param method: 'mean' or 'stddev'
         :param interval: interval in ms (will be stored in seconds)
         """
         if method not in self.list_agg_methods():
             raise KeyError(f'unsupported agg_method {method}.')
         self.aggregation = method
         if interval is not None:
             self.interval = int(interval) / 1000
 
     def list_agg_methods(self) -> list:
         """
         get a list of all authorized methods.
-        :return: list with "mean", "stddev", "mode", "median", "count", "sum", "first", "last", "max" or "min"
+        :return: list of all authorized methods.
         """
         return [
             "mean", "stddev", "mode", "median", "count", "sum", "first", "last", "max", "min"
         ]
 
     def select_template(self,
                         template_id=None,
                         template_key=None,
                         twin_id=None,
                         twin_hardware_id=None):
         """
-        select a template and its registration.
+        Select a template and its registration.
         :param template_id: template UUID
         :param template_key: template key ( ignored if template_id specified )
         :param twin_id: Digital Twin UUID
         :param twin_hardware_id: hardware ID of Digital Twin ( ignored if twin_id specified )
         """
         if template_id is None and template_key is None and twin_id is None and twin_hardware_id is None:
             self.template = None
@@ -311,15 +323,14 @@
 
             elif twin_hardware_id is not None:
                 self.template['twin_hardware_id'] = str(twin_hardware_id)
 
     def get_params(self):
         """
         get a list of all parameters.
-        :return: list of parameters
         """
         params = []
 
         if self.start is not None and isinstance(self.start, str) and self.start.startswith("@"):
             params.append(self.start[1:])
 
         if self.end is not None and isinstance(self.end, str) and self.end.startswith("@"):
@@ -346,19 +357,49 @@
             self.end = value
             assigned = True
 
         if not assigned:
             raise KeyError(f'parameter {name} not found in request.')
 
     def to_json(self, target: str = None):
+        """
+        convert to a dict JSON compatible for all properties. For query only, use prepare().
+
+        :return: a dict JSON compatible
+        """
+
+        # Prepare is 'to_json' without future obsolete properties
         obj = self.prepare()
-        self.set_extra_data(obj)
+
+        if self.target_feat is not None:
+            obj["target_feat"] = {
+                "sensor": self.target_feat["sensor"],
+                "operator": self.target_feat["operator"],
+                "threshold": self.target_feat["threshold"]
+            }
+        if self.on_off_sensor is not None and self.restart_time is not None:
+            obj["restart_filter"] = {
+                "on_off_sensor": self.on_off_sensor,
+                "stop_restart_time": self.restart_time
+            }
+
+        if self.sensitivity is not None:
+            obj["sensitivity"] = self.sensitivity
+
+        if self.extra_data is not None:
+            obj["extra_data"] = self.extra_data
+
         return obj
 
     def from_json(self, json_data):
+        """
+        load a request based on dict from a JSON file.
+
+        :param json_data: JSON formatted dictionnary object representing a query.
+        """
         if "id" in json_data.keys():
             self.request_id = uuid.UUID(json_data["id"])
 
         if "name" in json_data.keys():
             self.name = json_data["name"]
 
         found_dps = False
@@ -458,32 +499,8 @@
 
         if "sensitivity" in json_data.keys():
             self.sensitivity = json_data["sensitivity"]
 
         if "extra_data" in json_data.keys():
             self.extra_data = json_data["extra_data"]
 
-    def set_extra_data(self, obj) -> dict:
-        """
-        deprecated - set additional data to query used as post-processing
-        """
-        if obj is None:
-            obj = {}
-        if self.target_feat is not None:
-            obj["target_feat"] = {
-                "sensor": self.target_feat["sensor"],
-                "operator": self.target_feat["operator"],
-                "threshold": self.target_feat["threshold"]
-            }
-        if self.on_off_sensor is not None and self.restart_time is not None:
-            obj["restart_filter"] = {
-                "on_off_sensor": self.on_off_sensor,
-                "stop_restart_time": self.restart_time
-            }
-
-        if self.sensitivity is not None:
-            obj["sensitivity"] = self.sensitivity
-
-        if self.extra_data is not None:
-            obj["extra_data"] = self.extra_data
-        return obj
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/twin.py` & `wizata-dsapi-0.4.9/wizata_dsapi/twin.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,58 +10,44 @@
     if match is None:
         raise ValueError('color is not a proper hexadecimal color : e.g. #E64600')
     else:
         return True
 
 
 class TwinBlockType(Enum):
-    """
-    digital twin block type
-        - area
-        - machine
-        - equipment
-        - flow
-    """
     AREA = "area"
     MACHINE = "machine"
     EQUIPMENT = "equipment"
     FLOW = "flow"
 
 
 class Twin(ApiDto):
     """
-    digital twin item representing an asset, machine, equipment.
+    Digital Twin item/asset declared and managed on Wizata.
 
-    :ivar uuid.UUID twin_id: technical id of the twin.
-    :ivar uuid.UUID hardware_id: unique str hardware id (e.g. required in template and ml models 'by_twin').
-    :ivar str name: logical display name of the Asset.
-    :ivar uuid.UUID parent_id: technical id of the parent twin item.
-    :ivar wizata_dsapi.TwinBlockType type: type (area, machine, equipment or flow).
-    :ivar float latitude: fixed latitude of the twin item.
-    :ivar float longitude: fixed longitude of the twin item.
-    :ivar uuid.UUID latitude_id: technical id of a datapoint specifying dynamic latitude of twin.
-    :ivar uuid.UUID longitude_id: technical id of a datapoint specifying dynamic longitude of twin.
-    :ivar str color: hexadecimal code of the color to associate with this twin item.
-    :ivar str icon: logical id of the icon or svg schema to associate with this twin item.
-    :ivar uuid.UUID createdById: unique identifier of creating user.
-    :ivar int createdDate: timestamp of created date.
-    :ivar uuid.UUID updatedById: unique identifier of updating user.
-    :ivar int updatedDate: timestamp of updated date.
+    :ivar twin_id: UUID of the Digital Twin.
+    :ivar hardware_id: str hardware id identifying the Asset.
+    :ivar name: logical display name of the Asset.
+    :ivar type: type (area, machine, equipment or flow).
     """
 
     @classmethod
     def route(cls):
         return "twins"
 
     @classmethod
     def from_dict(cls, data):
         obj = Twin()
         obj.from_json(data)
         return obj
 
+    @classmethod
+    def operations(cls):
+        return ['lists', 'get_by_id', 'get_by_key', 'create', 'update', 'delete']
+
     def __init__(self, twin_id=None, hardware_id=None, name=None, parent_id=None, ttype=TwinBlockType.MACHINE,
                  latitude_id: uuid.UUID = None, longitude_id: uuid.UUID = None, color: str = None, icon: str = None,
                  latitude: float = None, longitude: float = None):
         if twin_id is None:
             self.twin_id = uuid.uuid4()
         else:
             self.twin_id = twin_id
@@ -79,20 +65,34 @@
         self.icon = icon
         self.createdById = None
         self.createdDate = None
         self.updatedById = None
         self.updatedDate = None
 
     def api_id(self) -> str:
+        """
+        Id of the experiment (experiment_id)
+
+        :return: string formatted UUID of the Experiment.
+        """
         return str(self.twin_id).upper()
 
     def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate execution.
+        :return: Endpoint name.
+        """
         return "Twins"
 
     def from_json(self, obj):
+        """
+        Load the Twin entity from a dictionary.
+
+        :param obj: Dict version of the Twin.
+        """
         if "id" in obj.keys():
             self.twin_id = uuid.UUID(obj["id"])
         if "hardwareId" in obj.keys() and obj["hardwareId"] is not None:
             self.hardware_id = obj["hardwareId"]
         if "name" in obj.keys() and obj["name"] is not None:
             self.name = obj["name"]
         if "parentId" in obj.keys() and obj["parentId"] is not None:
@@ -118,31 +118,36 @@
             self.createdDate = obj["createdDate"]
         if "updatedById" in obj.keys() and obj["updatedById"] is not None:
             self.updatedById = obj["updatedById"]
         if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
             self.updatedDate = obj["updatedDate"]
 
     def to_json(self, target: str = None):
+        """
+        Convert the twin to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Twin object.
+        """
         obj = {
             "id": str(self.twin_id)
         }
         if self.hardware_id is not None:
             obj["hardwareId"] = str(self.hardware_id)
         if self.name is not None:
             obj["name"] = str(self.name)
         if self.parent_id is not None:
             obj["parentId"] = str(self.parent_id)
         if self.type is not None and isinstance(self.type, TwinBlockType):
             obj["type"] = self.type.value
         if self.color is not None:
             obj["color"] = str(self.color)
         if self.latitude is not None:
-            obj["latitude"] = float(self.latitude)
+            obj["latitude"] = str(self.latitude)
         if self.longitude is not None:
-            obj["longitude"] = float(self.longitude)
+            obj["longitude"] = str(self.longitude)
         if self.latitude_id is not None:
             obj["latitudeSensorId"] = str(self.latitude_id)
         if self.longitude_id is not None:
             obj["longitudeSensorId"] = str(self.longitude_id)
         if self.icon is not None:
             obj["icon"] = str(self.icon)
         if self.createdById is not None:
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.4.9/wizata_dsapi/twinregistration.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,14 @@
 from .api_dto import ApiDto
 from .pipeline import VarType
 from .datapoint import DataPoint
 from .template import TemplateProperty
 
 
 class TwinRegistrationProperty(ApiDto):
-    """
-    define a property mapping between template and registration.
-    :ivar uuid.UUID twin_registration_property_id: technical id of the twin registration property.
-    :ivar uuid.UUID twin_registration_id: technical id of the twin registration.
-    :ivar wizata_dsapi.TemplateProperty template_property: template property associated.
-    :ivar wizata_dsapi.VarType p_type: type associate to this registration - equal the one on template_property.
-    :ivar value: value of the registration property, type is depending upon p_type.
-    :ivar uuid.UUID createdById: unique identifier of creating user.
-    :ivar int createdDate: timestamp of created date.
-    :ivar uuid.UUID updatedById: unique identifier of updating user.
-    :ivar int updatedDate: timestamp of updated date.
-    """
-
-    @classmethod
-    def route(cls):
-        return "registrationproperties"
-
-    @classmethod
-    def from_dict(cls, data):
-        obj = TwinRegistrationProperty()
-        obj.from_json(data)
-        return obj
 
     def __init__(self,
                  twin_registration_property_id: uuid.UUID = None,
                  twin_registration_id: uuid.UUID = None,
                  template_property: TemplateProperty = None,
                  value=None,
                  p_type: VarType = None):
@@ -46,20 +24,32 @@
         self.p_type = p_type
         self.createdById = None
         self.createdDate = None
         self.updatedById = None
         self.updatedDate = None
 
     def api_id(self) -> str:
+        """
+        Id
+        :return: string formatted UUID of the template.
+        """
         return str(self.twin_registration_property_id).upper()
 
     def endpoint(self) -> str:
+        """
+        Name of the endpoints.
+        :return: Endpoint name.
+        """
         return "TwinRegistrationProperties"
 
     def from_json(self, obj):
+        """
+        Load the property from a dictionary.
+        :param obj: Dict version of the Property.
+        """
         if "id" in obj.keys():
             self.twin_registration_property_id = uuid.UUID(obj["id"])
         if "templatePropertyId" in obj.keys() and obj["templatePropertyId"] is not None:
             self.template_property = TemplateProperty(obj["templatePropertyId"])
         if "twinRegistrationId" in obj.keys() and obj["twinRegistrationId"] is not None:
             self.twin_registration_id = obj["twinRegistrationId"]
 
@@ -94,14 +84,19 @@
             self.value = obj["float"]
             self.p_type = VarType.FLOAT
         elif "string" in obj.keys() and obj["string"] is not None:
             self.value = obj["string"]
             self.p_type = VarType.STRING
 
     def to_json(self, target: str = None):
+        """
+        Convert the registration to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Registration object.
+        """
         obj = {
             "id": str(self.twin_registration_property_id)
         }
         if self.template_property is not None:
             obj["templatePropertyId"] = str(self.template_property.template_property_id)
         if self.twin_registration_id is not None:
             obj["twinRegistrationId"] = str(self.twin_registration_id)
@@ -147,35 +142,23 @@
         if self.updatedDate is not None:
             obj["updatedDate"] = str(self.updatedDate)
         return obj
 
 
 class TwinRegistration(ApiDto):
     """
-    registration of a digital twin item on a template.
+    Registration of a Digital Twin on a solution Template.
 
-    :ivar uuid.UUID twin_registration_id: technical id of the registration.
-    :ivar uuid.UUID twin_id: technical id of the twin item.
-    :ivar uuid.UUID template_id: technical id of the template.
-    :ivar list properties: list of wizata_dsapi.TwinRegistrationProperty or dict { name , datapoint, float, integer, string }
-    :ivar uuid.UUID createdById: unique identifier of creating user.
-    :ivar int createdDate: timestamp of created date.
-    :ivar uuid.UUID updatedById: unique identifier of updating user.
-    :ivar int updatedDate: timestamp of updated date.
-    """
+    :ivar twin_registration_id: UUID of the registration
+    :ivar twin_id: UUID of registered Digital Twin
+    :ivar template_id: UUID of the solution template.
+    :ivar properties: list of Properties { name , datapoint, float, integer, string }
 
-    @classmethod
-    def route(cls):
-        return "registrations"
-
-    @classmethod
-    def from_dict(cls, data):
-        obj = TwinRegistration()
-        obj.from_json(data)
-        return obj
+    A property must contains a name and the hardwareId of the datapoint or the value corresponding to the right type.
+    """
 
     def __init__(self, twin_registration_id=None, twin_id=None, template_id=None, properties=None):
         if twin_registration_id is None:
             self.twin_registration_id = uuid.uuid4()
         else:
             self.twin_registration_id = twin_registration_id
         self.twin_id = twin_id
@@ -191,26 +174,40 @@
 
         self.createdById = None
         self.createdDate = None
         self.updatedById = None
         self.updatedDate = None
 
     def api_id(self) -> str:
+        """
+        Id of the TwinRegistrations (twin_registration_id)
+
+        :return: string formatted UUID of the template.
+        """
         return str(self.twin_registration_id).upper()
 
     def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate templates.
+        :return: Endpoint name.
+        """
         return "TwinRegistration"
 
     def from_json(self, obj):
+        """
+        Load the Registration entity from a dictionary.
+
+        :param obj: Dict version of the Registration.
+        """
         if "id" in obj.keys():
             self.twin_registration_id = uuid.UUID(obj["id"])
         if "twinId" in obj.keys() and obj["twinId"] is not None:
-            self.twin_id = uuid.UUID(obj["twinId"])
+            self.twin_id = obj["twinId"]
         if "templateId" in obj.keys() and obj["templateId"] is not None:
-            self.template_id = uuid.UUID(obj["templateId"])
+            self.template_id = obj["templateId"]
         if "properties" in obj.keys() and obj["properties"] is not None:
             if isinstance(obj["properties"], str):
                 self.properties = json.loads(obj["properties"])
             else:
                 self.properties = obj["properties"]
             self._properties = []
             for dict_property in self.properties:
@@ -227,14 +224,19 @@
             self.createdDate = obj["createdDate"]
         if "updatedById" in obj.keys() and obj["updatedById"] is not None:
             self.updatedById = obj["updatedById"]
         if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
             self.updatedDate = obj["updatedDate"]
 
     def to_json(self, target: str = None):
+        """
+        Convert the registration to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Registration object.
+        """
         obj = {
             "id": str(self.twin_registration_id)
         }
         if self.twin_id is not None:
             obj["twinId"] = str(self.twin_id)
         if self.template_id is not None:
             obj["templateId"] = str(self.template_id)
@@ -255,15 +257,14 @@
         if self.updatedDate is not None:
             obj["updatedDate"] = str(self.updatedDate)
         return obj
 
     def append(self, registration_property: TwinRegistrationProperty):
         """
         append a twin registration property.
-        :param wizata_dsapi.TwinRegistrationProperty registration_property: append a property.
         """
 
         if registration_property.twin_registration_id is None:
             registration_property.twin_registration_id = self.twin_registration_id
         elif registration_property.twin_registration_id != self.twin_registration_id:
             raise ValueError('mismatch between registration id and property id')
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/wizard_request.py` & `wizata-dsapi-0.4.9/wizata_dsapi/experiment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,104 +1,116 @@
 import uuid
-import json
-from .request import Request
+from .api_dto import ApiDto
 
 
-class WizardRequest:
+class Experiment(ApiDto):
     """
-    represents a wizard request to generate automatically a pipeline through an experimentation.
-    :ivar uuid.UUID execution_id: execution id at origin of this request.
-    :ivar str name: name of the request.
-    :ivar bool is_anomaly_detection: true if request concerns an anomaly detection.
-    :ivar str function: name of the function.
-    :ivar dict properties: dictionary of properties defining the request.
+    An experiment is a container to track all executions made in the same context.
+
+    :ivar experiment_id: The UUID of the Experiment.
+    :ivar key: Logical String ID of the Experiment
+    :ivar name: A simple name helping the user identifying the experiment.
     """
 
-    def __init__(self,
-                 execution_id: uuid.UUID = None,
-                 name: str = None,
-                 request: Request = None,
-                 properties: dict = None
-                 ):
-        if execution_id is None:
-            execution_id = uuid.uuid4()
-        self.execution_id = execution_id
+    @classmethod
+    def route(cls):
+        return "experiments"
+
+    @classmethod
+    def from_dict(cls, data):
+        obj = Experiment()
+        obj.from_json(data)
+        return obj
+
+    @classmethod
+    def operations(cls):
+        return ['lists', 'get_by_id', 'get_by_key', 'create', 'update', 'delete']
+
+    def __init__(self, experiment_id=None, key=None, name=None, description=None):
+        if experiment_id is None:
+            self.experiment_id = uuid.uuid4()
+        else:
+            self.experiment_id = experiment_id
+        self.key = key
         self.name = name
-        self.request = request
-        self.is_anomaly_detection = False
-        self.function = None
-        self.properties = properties
+        self.description = description
+        self.templateId = None
+        self.twinId = None
+        self.twinGraphId = None
+        self.createdById = None
+        self.createdDate = None
+        self.updatedById = None
+        self.updatedDate = None
+
+    def api_id(self) -> str:
+        """
+        Id of the experiment (experiment_id)
+
+        :return: string formatted UUID of the Experiment.
+        """
+        return str(self.experiment_id).upper()
 
-    def to_json(self):
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate execution.
+        :return: Endpoint name.
+        """
+        return "Experiments"
+
+    def to_json(self, target: str = None):
+        """
+        Convert to a json version of Experiment definition.
+        """
         obj = {
-            "id": str(self.execution_id),
-            "name": str(self.name)
+            "id": str(self.experiment_id)
         }
-        if self.request is not None:
-            obj["request"] = json.dumps(self.request.to_json())
-
-        if self.function is not None:
-            obj["function"] = self.function
-        if self.is_anomaly_detection:
-            obj["isAnomalyDetection"] = True
-        else:
-            obj["isAnomalyDetection"] = False
-        if self.properties is not None:
-            obj["properties"] = json.dumps(self.properties)
+        if self.key is not None:
+            if len(self.key) > 16:
+                raise ValueError('experiment key is limited to 16 char.')
+            obj["key"] = str(self.key)
+        if self.name is not None:
+            obj["name"] = str(self.name)
+        if self.description is not None:
+            obj["description"] = str(self.description)
+        if self.templateId is not None:
+            obj["templateId"] = str(self.templateId)
+        if self.twinId is not None:
+            obj["twinId"] = str(self.twinId)
+        if self.twinGraphId is not None:
+            obj["twinGraphId"] = str(self.twinGraphId)
+        if self.createdById is not None:
+            obj["createdById"] = str(self.createdById)
+        if self.createdDate is not None:
+            obj["createdDate"] = str(self.createdDate)
+        if self.updatedById is not None:
+            obj["updatedById"] = str(self.updatedById)
+        if self.updatedDate is not None:
+            obj["updatedDate"] = str(self.updatedDate)
         return obj
 
     def from_json(self, obj):
+        """
+        Load an experiment from a stored JSON object.
+        """
         if "id" in obj.keys():
-            self.execution_id = uuid.UUID(obj["id"])
-        if "name" in obj.keys():
+            self.experiment_id = uuid.UUID(obj["id"])
+        if "key" in obj.keys() and obj["key"] is not None:
+            self.key = obj["key"]
+        if "name" in obj.keys() and obj["name"] is not None:
             self.name = obj["name"]
-        else:
-            raise ValueError("please set a name on the request")
-        if "request" in obj.keys() and obj["request"] is not None:
-            self.request = Request()
-            if isinstance(obj["request"], str):
-                self.request.from_json(json.loads(obj["request"]))
-                self.copy_properties(json.loads(obj["request"]))
-            else:
-                self.request.from_json(obj["request"])
-                self.copy_properties(obj["request"])
-        if "properties" in obj.keys() and obj["properties"] is not None:
-            if isinstance(obj["properties"], str):
-                self.add_properties(json.loads(obj["properties"]))
-            else:
-                self.add_properties(obj["properties"])
-
-        if "function" in obj.keys() and obj["function"] is not None:
-            self.function = obj["function"]
-        if "isAnomalyDetection" in obj.keys() and obj["isAnomalyDetection"] is not None:
-            if isinstance(obj["isAnomalyDetection"], bool):
-                self.is_anomaly_detection = obj["isAnomalyDetection"]
-            else:
-                self.is_anomaly_detection = obj["isAnomalyDetection"] == 'True'
-
-    def copy_properties(self, obj: dict):
-        """
-        copy all properties from a dict to another.
-        :param dict obj: new dict
-        """
-        keys = [
-            'target_feat',
-            'sensitivity',
-            'aggregations',
-            'restart_filter',
-            'interval'
-        ]
-        for key in keys:
-            if key in obj:
-                if self.properties is None:
-                    self.properties = {}
-                self.properties[key] = obj[key]
-
-    def add_properties(self, obj: dict):
-        """
-        add all properties from a dict to current properties.
-        :param dict obj: properties to add.
-        """
-        for key in obj.keys():
-            if self.properties is None:
-                self.properties = {}
-            self.properties[key] = obj[key]
+        if "description" in obj.keys() and obj["description"] is not None:
+            self.description = obj["description"]
+        if "templateId" in obj.keys() and obj["templateId"] is not None:
+            self.templateId = obj["templateId"]
+        if "twinId" in obj.keys() and obj["twinId"] is not None:
+            self.twinId = obj["twinId"]
+        if "twinGraphId" in obj.keys() and obj["twinGraphId"] is not None:
+            self.twinGraphId = obj["twinGraphId"]
+        if "createdById" in obj.keys() and obj["createdById"] is not None:
+            self.createdById = obj["createdById"]
+        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
+            self.createdDate = obj["createdDate"]
+        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
+            self.updatedById = obj["updatedById"]
+        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
+            self.updatedDate = obj["updatedDate"]
+
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.4.9/wizata_dsapi/wizata_dsapi_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,68 +24,49 @@
 from .api_dto import ApiDto
 from .business_label import BusinessLabel
 from .plot import Plot
 from .request import Request
 from .mlmodel import MLModel
 from .experiment import Experiment
 from .script import Script
-from .execution import Execution, ExecutionStatus
+from .execution import Execution
 from .dsapi_json_encoder import DSAPIEncoder
 from .ds_dataframe import DSDataFrame
 from .model_toolkit import predict
 from .template import Template, TemplateProperty
 from .twinregistration import TwinRegistration
-from .trigger import Trigger
 from .twin import Twin
 from .datapoint import DataPoint, BusinessType, Label, Category
 from .pipeline import Pipeline, PipelineStep, VarType
 from .solution_component import SolutionComponent, SolutionType
 from .paged_query_result import PagedQueryResult
 from .api_interface import ApiInterface
 from .version import __version__
 
-from .api_config import _registry
-
 
 def sanitize_url_parameter(param_value):
     illegal_characters = set(c for c in param_value if not (c.isalnum() or c in '-_., '))
     if illegal_characters:
         raise ValueError(f"illegal characters found in parameter {param_value}: {', '.join(illegal_characters)}")
     encoded_param_value = urllib.parse.quote(param_value)
     return encoded_param_value
 
 
 class WizataDSAPIClient(ApiInterface):
-    """
-    client wrapper to cloud data science API
-
-    accessible preferably through wizata_dsapi.api() using os variables, you can also create an instance using __init__()
-    please contact your administrator to receive configuration and connection details
-
-    :ivar str domain: URL of data science API
-    :ivar str client_id: azure authentication - client id
-    :ivar str client_secret: azure authentication - your client secret API key
-    :ivar str scope: azure authentication - scope
-    :ivar str tenant_id: azure authentication - tenant
-    :ivar str protocol: default - https
-    :ivar str username: azure authentication - deprecated - username
-    :ivar str password: azure authentication - deprecated - password
-    """
 
     def __init__(self,
                  client_id=None,
                  scope=None,
                  tenant_id=None,
                  username=None,
                  password=None,
                  domain="localhost",
                  protocol="https",
                  client_secret=None):
         super().__init__()
-        super()._set_registry("cloud_dsapi", _registry)
 
         # properties
         self.domain = domain
         self.protocol = protocol
 
         # authentication
         self.__username = username
@@ -109,18 +90,30 @@
             )
 
         self.__app = msal.PublicClientApplication(
             client_id=self.__client_id,
             authority=self.__authority
         )
 
+        self._dto_registry = {
+            "business_labels": BusinessLabel,
+            "dataframes": DSDataFrame,
+            "datapoints": DataPoint,
+            "executions": Execution,
+            "experiments": Experiment,
+            "mlmodels": MLModel,
+            "pipelines": Pipeline,
+            "plots": Plot,
+            "request": Request,
+            "scripts": Script,
+            "templates": Template,
+            "twins": Twin
+        }
+
     def authenticate(self):
-        """
-        perform authentication on client side
-        """
         result = self.__app.acquire_token_interactive(
             scopes=self.__scopes,
             success_template="""<html><body>You are authenticated and your code is running, you can close this page.<script>setTimeout(function(){window.close()}, 3000);</script></body></html> """
         )
         self.__daemon = False
         self.__interactive_token = result["access_token"]
 
@@ -177,23 +170,20 @@
         }
 
     def __raise_error(self, response):
         """
         raise a formatted error from an API response.
         :param response: response from the server.
         """
-        if 'Content-Type' in response.headers and response.headers['Content-Type'] == 'application/json':
-            json_content = response.json()
-            if "errors" in json_content.keys():
-                message = json_content["errors"][0]["message"]
-                return RuntimeError(str(response.status_code) + " - " + message)
-            else:
-                return RuntimeError(str(response.status_code) + " - " + response.reason)
+        json_content = response.json()
+        if "errors" in json_content.keys():
+            message = json_content["errors"][0]["message"]
+            return RuntimeError(str(response.status_code) + " - " + message)
         else:
-            raise RuntimeError(str(response.status_code) + " - " + response.reason)
+            return RuntimeError(str(response.status_code) + " - " + response.reason)
 
     def _process_request(self,
                          method: str,
                          route: str,
                          dto_class=None,
                          result_type: str = None,
                          params: dict = None,
@@ -233,20 +223,14 @@
             response = requests.delete(
                 self.__url() + route,
                 headers=self.__header(),
                 params=params
             )
         if response is None:
             raise ValueError('Method not supported')
-        if "Wizata-Version" in response.headers:
-            server_version = response.headers["Wizata-Version"]
-            if server_version != wizata_dsapi.__version__:
-                print(f' * Warning - version mismatch - server {server_version} vs local {wizata_dsapi.__version__}')
-                print(f'        python -m pip install --upgrade pip')
-                print(f'        pip install wizata_dsapi=={server_version}')
         if response.status_code == 200:
             if result_type == "list":
                 obj_list = []
                 for obj_json in response.json():
                     obj_list.append(dto_class.from_dict(obj_json))
                 return obj_list
             elif result_type == "json":
@@ -275,20 +259,17 @@
 
     def info(self):
         """
         print insights regarding version and supported operations
         """
         print(f"")
         print(f"version: {__version__} ")
-        for class_name in _registry:
-            print(f'Entity {class_name}')
-            print(f' * Class    {_registry[class_name]["class"]} - ')
-            print(f' * DS API   {_registry[class_name]["cloud_dsapi"]} - ')
-            print(f' * Context  {_registry[class_name]["cloud_context"]}')
-            print(f"")
+        print(f'operations: ')
+        for class_name in self._dto_registry:
+            print(f'    {class_name} - {self._dto_registry[class_name].operations()} - {self._dto_registry[class_name].get_type()}')
         print(f"")
 
     def lists(self, entity):
         """
         lists all elements of a specific entity.
         :param entity: plural name of the entity or class (e.g. scripts, plots, mlmodels, dataframes...)
         :return: list of all elements with at least the id property.
@@ -383,32 +364,24 @@
                 route=dto_class.route() + "/" + str(id) + "/",
                 dto_class=dto_class,
                 result_type=dto_class.get_type()
             )
 
         # get_by_key
         elif operation == "get_by_key":
-            if dto_class == Script:
-                return self._process_request(
+            results = self._process_request(
                     method="GET",
-                    route=dto_class.route() + "/" + str(key) + "/",
+                    route=dto_class.route() + "/",
                     dto_class=dto_class,
-                    result_type=dto_class.get_type()
+                    result_type="list",
+                    params={'key': key}
                 )
-            else:
-                results = self._process_request(
-                        method="GET",
-                        route=dto_class.route() + "/",
-                        dto_class=dto_class,
-                        result_type="list",
-                        params={'key': key}
-                    )
-                for result in results:
-                    return result
-                return None
+            for result in results:
+                return result
+            return None
 
     def create(self, obj) -> uuid.UUID:
         """
         create and save an object on the server
         :param obj: object from any supported entity (see info()) or python callable function (Script)
         :return: id of created object
         """
@@ -728,26 +701,28 @@
             elif isinstance(experiment, Experiment):
                 execution.experiment_id = experiment.experiment_id
         if properties is not None and isinstance(properties, dict):
             execution.properties = properties
 
         if pipeline is not None:
             if isinstance(pipeline, uuid.UUID) or (isinstance(pipeline, str) and is_valid_uuid(pipeline)):
-                execution.pipeline_id = pipeline
+                execution.pipeline = Pipeline(pipeline_id=uuid.UUID(pipeline))
             elif isinstance(pipeline, str):
-                execution.pipeline_id = self.get(pipeline_key=pipeline).pipeline_id
+                execution.pipeline = self.get(pipeline_key=pipeline)
             elif isinstance(pipeline, Pipeline):
-                execution.pipeline_id = pipeline.pipeline_id
+                execution.pipeline = pipeline
         if twin is not None:
+            if execution.properties is None:
+                execution.properties = {}
             if isinstance(twin, uuid.UUID) or (isinstance(twin, str) and is_valid_uuid(twin)):
-                execution.twin_id = twin
+                execution.properties["twinId"] = str(twin)
             elif isinstance(twin, str):
-                execution.twin_id = self.get(twin_hardware_id=twin).twin_id
+                execution.properties["twinId"] = str(self.get(twin_hardware_id=twin).twin_id)
             elif isinstance(twin, Twin):
-                execution.twin_id = twin.twin_id
+                execution.properties["twinId"] = str(twin.twin_id)
 
         # Execute
         if isinstance(execution, Execution):
             response = requests.post(f"{self.__url()}execute/?mode={mode}",
                                      headers=self.__header(),
                                      data=json.dumps(execution.to_json(), cls=DSAPIEncoder))
 
@@ -760,24 +735,25 @@
                     for plot in obj["plots"]:
                         result_execution.plots.append(self.get(Plot(plot_id=plot["id"])))
                 if "models" in obj.keys():
                     for mlmodel in obj["models"]:
                         result_execution.models.append(self.get(MLModel(model_id=mlmodel["id"])))
                 if "resultDataframe" in obj.keys() and obj["resultDataframe"]["id"] is not None:
                     result_execution.output_ds_dataframe = self.get(DSDataFrame(df_id=obj["resultDataframe"]["id"]))
-
+                if "anomaliesList" in obj.keys() and isinstance(obj["anomaliesList"], str):
+                    result_execution.anomalies = json.loads(obj["anomaliesList"])
                 return result_execution
             else:
                 raise self.__raise_error(response)
         else:
             raise TypeError("No execution have been loaded from parameters.")
 
     def experiment(self,
+                   experiment,
                    pipeline,
-                   experiment=None,
                    twin=None,
                    properties: dict = None,
                    train: bool = True,
                    plot: bool = True,
                    write: bool = False) -> Execution:
         """
         experiment and train models with a pipeline.
@@ -1562,105 +1538,14 @@
                 twin = Twin()
                 twin.from_json(obj)
                 query.results.append(twin)
             return query
         else:
             raise self.__raise_error(response)
 
-    def search_executions(self,
-                          page: int = 1,
-                          size: int = 20,
-                          sort: str = "id",
-                          direction: str = "asc",
-                          pipeline_id: uuid.UUID = None,
-                          twin_id:  uuid.UUID = None,
-                          template_id: uuid.UUID = None,
-                          status: ExecutionStatus = None) -> PagedQueryResult:
-        """
-        get executions with a paged query.
-        :param page: numero of the page - default 1.
-        :param size: quantity per page - default 20 max 100.
-        :param sort: column to sort results - default id.
-        :param direction: sorting direction by default asc, accept also desc.
-        :param pipeline_id: filter on a specific pipeline.
-        :param twin_id: filter on a specific twin.
-        :param template_id: filter on a specific template.
-        :param status: filter on a specific status.
-        :return: PagedQueryResults, check total for number of potential results and results for the list of entity.
-        """
-        query = PagedQueryResult(
-            page=page,
-            size=size,
-            sort=sort,
-            direction=direction
-        )
-
-        if sort not in ["id", "pipelineId", "twinId", "templateId",
-                        "createdDate" , "createdById",
-                        "updatedDate", "updatedById",
-                        "status"]:
-            raise ValueError("invalid sort column")
-
-        parameter_str = "?page=" + str(page) + "&size=" + str(size) + "&sort=" + str(sort) + "&direction=" + str(direction)
-
-        if pipeline_id is not None:
-            parameter_str += "&pipelineId=" + sanitize_url_parameter(str(pipeline_id))
-
-        if twin_id is not None:
-            parameter_str += "&twinId=" + sanitize_url_parameter(str(twin_id))
-
-        if template_id is not None:
-            parameter_str += "&templateId=" + sanitize_url_parameter(str(template_id))
-
-        if status is not None:
-            if not isinstance(status, ExecutionStatus):
-                raise ValueError(f'status is not a valid ExecutionStatus')
-            parameter_str += "&status=" + sanitize_url_parameter(status.value)
-
-        response = requests.request("GET",
-                                    self.__url() + "execute/filter" + parameter_str,
-                                    headers=self.__header()
-                                    )
-        if response.status_code == 200:
-            response_obj = response.json()
-            query.total = int(response_obj["total"])
-            query.results = []
-            for obj in response_obj["results"]:
-                execution = Execution()
-                execution.from_json(obj)
-                query.results.append(execution)
-            return query
-        else:
-            raise self.__raise_error(response)
-
-    def abort(self, executions: list) -> str:
-        """
-        send an abort request for executions and return a result message
-        :param executions: must be a list containing uuid or Execution.
-        """
-        if executions is None or len(executions) == 0:
-            raise ValueError(f'please provide at list one execution to abort')
-
-        payload = {
-            'ids': []
-        }
-        for execution in executions:
-            if isinstance(execution, uuid.UUID):
-                payload['ids'].append(str(execution))
-            if isinstance(execution, str):
-                payload['ids'].append(str(uuid.UUID(execution)))
-            if isinstance(execution, Execution):
-                payload['ids'].append(str(execution.execution_id))
-        response = requests.post(
-            self.__url() + "execute/abort",
-            headers=self.__header(),
-            data=json.dumps(payload)
-        )
-        return response.text
-
 
 def api() -> WizataDSAPIClient:
     """
     Create a WizataDSAPIClient from environment variables.
     :return: client
     """
     protocol = 'https'
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.4.9/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE.txt
 README.rst
 setup.py
 wizata_dsapi/__init__.py
-wizata_dsapi/api_config.py
 wizata_dsapi/api_dto.py
 wizata_dsapi/api_interface.py
 wizata_dsapi/business_label.py
 wizata_dsapi/context.py
 wizata_dsapi/dataframe_toolkit.py
 wizata_dsapi/datapoint.py
 wizata_dsapi/ds_dataframe.py
@@ -19,20 +18,17 @@
 wizata_dsapi/paged_query_result.py
 wizata_dsapi/pipeline.py
 wizata_dsapi/plot.py
 wizata_dsapi/request.py
 wizata_dsapi/script.py
 wizata_dsapi/solution_component.py
 wizata_dsapi/template.py
-wizata_dsapi/trigger.py
 wizata_dsapi/twin.py
 wizata_dsapi/twinregistration.py
 wizata_dsapi/version.py
 wizata_dsapi/wizard_function.py
-wizata_dsapi/wizard_request.py
 wizata_dsapi/wizata_dsapi_client.py
-wizata_dsapi/words.py
 wizata_dsapi.egg-info/PKG-INFO
 wizata_dsapi.egg-info/SOURCES.txt
 wizata_dsapi.egg-info/dependency_links.txt
 wizata_dsapi.egg-info/requires.txt
 wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.4.81/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.4.9/wizata_dsapi.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 dill==0.3.6
 pandas==1.5.3
 numpy==1.23.5
 matplotlib==3.7.1
-protobuf==3.20.3
+protobuf==3.19.6
 tensorflow_probability==0.15.0
 scikit-learn==1.2.2
 plotly==5.13.1
 adtk==0.6.2
 scipy==1.10.1
 xgboost==1.7.4
 joblib==1.2.0
@@ -15,18 +15,18 @@
 explainerdashboard==0.4.2.1
 ipywidgets==8.0.4
 kaleido==0.2.1
 pytest==7.2.2
 pytest-cov==4.0.0
 shapely==2.0.1
 pyodbc==4.0.35
-msal>=1.24.0
+msal==1.21.0
 u8darts==0.25.0
 optuna==3.3.0
 
 [:sys_platform != "darwin" or platform_machine != "arm64"]
-tensorflow==2.15.0
-keras==2.15.0
+tensorflow==2.7
+keras==2.7
 
 [:sys_platform == "darwin" and platform_machine == "arm64"]
-tensorflow-macos==2.15.0
-keras==2.15.0
+tensorflow-macos==2.11.0
+keras==2.11.0
```

