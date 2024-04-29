# Comparing `tmp/avoca-0.2.0.tar.gz` & `tmp/avoca-0.3.0.tar.gz`

## Comparing `avoca-0.2.0.tar` & `avoca-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 avoca-0.2.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/export_nas.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/flags.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/io.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/logging.py
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/manager.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/requirements.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/settings.py
--rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/bindings/ebas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/__init__.py
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/abstract.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/concs.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/generate_classes_doc.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/rt.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/test.py
--rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/qa_class/zscore.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/testing/__init__.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/testing/df.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.2.0/avoca/utils/torch_models.py
--rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.2.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
--rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.2.0/data/voc_jan2jun_2023.csv
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.2.0/data/.avoca/config.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/make.bat
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/conf.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/index.rst
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/quickstart.ipynb
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/bindings/ebas.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/bindings/gcwerks.md
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.2.0/docs/source/bindings/index.rst
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.2.0/examples/config.yaml
--rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.2.0/examples/data_qa.ipynb
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.2.0/examples/read_nas.ipynb
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 avoca-0.2.0/tests/test_io.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 avoca-0.2.0/.gitignore
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.2.0/LICENCE.txt
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 avoca-0.2.0/README.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 avoca-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 avoca-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 avoca-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/export_nas.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/flags.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/io.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/logging.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/manager.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/requirements.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/bindings/__init__.py
+-rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/bindings/ebas.py
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/bindings/gcwerks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/__init__.py
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/abstract.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/concs.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/generate_classes_doc.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/rt.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/test.py
+-rw-r--r--   0        0        0    15856 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/qa_class/zscore.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/testing/__init__.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/testing/df.py
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 avoca-0.3.0/avoca/utils/torch_models.py
+-rw-r--r--   0        0        0   152471 2020-02-02 00:00:00.000000 avoca-0.3.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas
+-rw-r--r--   0        0        0   499755 2020-02-02 00:00:00.000000 avoca-0.3.0/data/voc_jan2jun_2023.csv
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 avoca-0.3.0/data/.avoca/config.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/make.bat
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/conf.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/index.rst
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/quickstart.ipynb
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/bindings/ebas.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/bindings/gcwerks.md
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 avoca-0.3.0/docs/source/bindings/index.rst
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 avoca-0.3.0/examples/config.yaml
+-rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 avoca-0.3.0/examples/data_qa.ipynb
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 avoca-0.3.0/examples/read_nas.ipynb
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 avoca-0.3.0/tests/test_io.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 avoca-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 avoca-0.3.0/LICENCE.txt
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 avoca-0.3.0/README.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 avoca-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 avoca-0.3.0/PKG-INFO
```

### Comparing `avoca-0.2.0/.gitlab-ci.yml` & `avoca-0.3.0/.gitlab-ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -46,11 +46,12 @@
     - python -m pytest
     - echo "Test done"
 
 
 deploy-job:      # This job runs in the deploy stage.
   stage: deploy  # It only runs when *both* jobs in the test stage complete successfully.
   environment: production
+  when: manual
   script:
     - pip install twine build
     - python -m build
     - TWINE_PASSWORD=${PYPY_TOKEN} TWINE_USERNAME=__token__ python -m twine upload dist/*
```

### Comparing `avoca-0.2.0/.readthedocs.yaml` & `avoca-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/flags.py` & `avoca-0.3.0/avoca/flags.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/manager.py` & `avoca-0.3.0/avoca/manager.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/requirements.py` & `avoca-0.3.0/avoca/requirements.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/settings.py` & `avoca-0.3.0/avoca/settings.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/bindings/ebas.py` & `avoca-0.3.0/avoca/bindings/ebas.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import logging
 import re
 from datetime import datetime, timedelta
 from enum import IntEnum
 from os import PathLike
 from pathlib import Path
 from typing import Any
-from warnings import warn
 
 import numpy as np
 import pandas as pd
 from ebas.io.file.nasa_ames import EbasNasaAmes
 from nilutility.datatypes import DataObject
 from nilutility.datetime_helper import DatetimeInterval
 
@@ -41,14 +40,17 @@
 ebas_flag_to_avoca: dict[int, QA_Flag] = {
     ebas_flag: avoca_flag for avoca_flag, ebas_flag in flags_to_ebas.items()
 }
 # Set some flags with Multiple values to the same value
 ebas_flag_to_avoca.pop(0)  # 0 is valid in avoca
 ebas_flag_to_avoca[999] = QA_Flag.MISSING
 ebas_flag_to_avoca[900] = QA_Flag.INVALIDATED_EXT
+ebas_flag_to_avoca[685] = (
+    QA_Flag.CALIBRATION
+)  #  	Invalid due to secondary standard gas measurement. Used for Level 0.
 
 missing_flags = set(QA_Flag) - set(flags_to_ebas.keys())
 if missing_flags:
     raise RuntimeError(
         f"Not all QA flags are mapped to Ebas flags. Missing: {missing_flags}"
     )
 
@@ -180,37 +182,36 @@
 
     # Find the last submited files the format is:
     last_file = None
     last_submision_time = None
     for file in directory.glob(f"*.nas"):
         try:
             time_str = file.name.split(".")[2]
-            time = datetime.datetime.strptime(time_str, "%Y%m%d%H%M%S")
+            time = datetime.strptime(time_str, "%Y%m%d%H%M%S")
             if last_submision_time is None or time > last_submision_time:
                 last_submision_time = time
                 last_file = file
         except Exception as e:
             logger.warning(f"Could not parse time from {file}: {e}")
 
     return last_file
 
 
 def get_data_level(nas: EbasNasaAmes) -> DataLevel:
     """Get the data level of the nas file."""
     data_level = nas.metadata["datalevel"]
 
-    match data_level:
-        case "1":
-            return DataLevel.CONCS
-        case "2":
-            return DataLevel.QA_CONCS
-        case "0":
-            return DataLevel.AREAS
-        case _:
-            raise ValueError(f"Data level {data_level} not recognized")
+    if data_level == "1":
+        return DataLevel.CONCS
+    elif data_level == "2":
+        return DataLevel.QA_CONCS
+    elif data_level == "0":
+        return DataLevel.AREAS
+    else:
+        raise ValueError(f"Data level {data_level} not recognized")
 
 
 def nas_to_avoca(nas: EbasNasaAmes) -> pd.DataFrame:
     """Convert the ebas file to a pandas dataframe for @voc@.
 
     To read the nas file, you can do:
 
@@ -254,16 +255,22 @@
         if "comp_name" not in metadata:
             continue
 
         values = var["values_"]
 
         title = metadata["title"]
 
-        # Split the title on the _
+        # Special variable used for calibration
+        if title == "cal":
+            calib_ids = np.array(values, dtype=float)
+            mask_nan = np.isnan(calib_ids)
+            calib_ids[mask_nan] = 0
+            clean_for_df[("-", "calib_id")] = calib_ids.astype(int)
 
+        # Split the title on the _
         title = title.split("_")
 
         if len(title) != 2:
 
             print("passing", title)
             continue
 
@@ -292,40 +299,50 @@
             clean_for_df[flag_col] |= flag_serie
 
     # Use the start of the intervals as the datetime (use 1 for the end)
     clean_for_df[("-", "datetime")] = [dt[0] for dt in nas.sample_times]
     clean_for_df[("-", "start_datetime")] = clean_for_df[("-", "datetime")]
     clean_for_df[("-", "end_datetime")] = [dt[1] for dt in nas.sample_times]
 
-    is_calibration = {
-        compound: (QA_Flag.CALIBRATION.value & clean_for_df[(compound, "flag")]).astype(
-            bool
-        )
-        for compound in compounds
-    }
-
-    # Assert all the calibration flags are the same
-    ref_calib = is_calibration[compounds[0]]
-    for compound in compounds[1:]:
-        mask_same = is_calibration[compounds[0]] == is_calibration[compound]
-        if not np.all(mask_same):
-            # Show the rows where not all have the same flag
-            mask_different = ~mask_same
-            logger.warning(
-                f"Calibration flags are not the same for all compounds: {compound} "
-                f"is different from reference compound {compounds[0]}"
-                f"at rows {np.argwhere(mask_different).reshape(-1)}"
+    df = pd.DataFrame(clean_for_df)
+    # Runtype, by default assume air samples
+    df[("-", "type")] = "air"
+
+    for calib_type, flag in {
+        "std": QA_Flag.CALIBRATION,
+        "blank": QA_Flag.BLANK,
+    }.items():
+        is_calib = {
+            compound: (flag.value & clean_for_df[(compound, "flag")]).astype(bool)
+            for compound in compounds
+        }
+
+        # Assert all the calibration flags are the same
+        ref_calib = is_calib[compounds[0]]
+        for compound in compounds[1:]:
+            mask_same = is_calib[compounds[0]] == is_calib[compound]
+            if not np.all(mask_same):
+                # Show the rows where not all have the same flag
+                mask_different = ~mask_same
+                logger.warning(
+                    f"Calibration flags for {flag} are not the same for all compounds:"
+                    f" {compound} is different from reference compound"
+                    f" {compounds[0]} at rows {np.argwhere(mask_different).reshape(-1)}"
+                )
+                # Combine the calib in both samples
+                ref_calib = ref_calib | is_calib[compound]
+        # Check that we are not overriding another flag
+        if not np.all(df.loc[ref_calib, ("-", "type")] == "air"):
+            other_types = np.unique(df.loc[ref_calib, ("-", "type")].to_numpy())
+            raise ValueError(
+                f"Calibration flag {flag} is overriding some {other_types} runs."
             )
-            # Combine the calib in both samples
-            ref_calib = ref_calib | is_calibration[compound]
+        df.loc[ref_calib, ("-", "type")] = calib_type
 
-    runtype = pd.Series(is_calibration[compounds[0]].map({True: "std", False: "air"}))
-    clean_for_df[("-", "type")] = runtype
-
-    return pd.DataFrame(clean_for_df).set_index(("-", "datetime"))
+    return df
 
 
 def read_ebas_csv(file: PathLike) -> pd.DataFrame:
     """Read the EBAS csv file and return a DataFrame.
 
     This format comes from other EBAS tools.
     """
@@ -379,28 +396,60 @@
 
 def extract_concentration_field(text: str) -> dict[str, float]:
     """Extract the concentrations from the text.
 
     This is a temporary solution that we found to communicate the concentrations
     of the standards thgrough the nas files.
     """
-    # Define the regular expression pattern to match the concentrations field
-    concentration_pattern = r"Concentrations:\s*\{([^}]*)\}"
-    # Search for the concentration field in the text
-    concentration_match = re.search(concentration_pattern, text)
-    if concentration_match:
-        # Extract the concentration substring
-        concentration_substring = concentration_match.group(1)
-        # Split the substring by comma to separate individual concentrations
-        concentration_list = concentration_substring.split(",")
-        # Initialize an empty dictionary to store concentrations
-        concentrations = {}
-        for concentration in concentration_list:
-            # Split each concentration by '=' to separate compound and value
-            compound, value = concentration.split("=")
-            # Remove leading and trailing whitespaces
-            compound = compound.strip()
-            value = float(value.strip())  # Convert value to float
-            concentrations[compound] = value
-        return concentrations
-    else:
-        return {}
+    # Check that the string starts and end with {}
+    if not text.startswith("{") or not text.endswith("}") or "{" in text[1:]:
+        raise ValueError(
+            f"Invalid concentration field: {text}. Must start and end with '{' and '}'"
+        )
+
+    text = text[1:-1]  # Remove the brackets
+
+    # Split the substring by comma to separate individual concentrations
+    concentration_list = text.split(",")
+    # Initialize an empty dictionary to store concentrations
+    concentrations = {}
+    for concentration in concentration_list:
+        # Split each concentration by '=' to separate compound and value
+        compound, value = concentration.split("=")
+        # Remove leading and trailing whitespaces
+        compound = compound.strip()
+        value = float(value.strip())  # Convert value to float
+        concentrations[compound] = value
+    return concentrations
+
+
+def read_calibrations(nas) -> dict[int, dict[str, str | dict[str, float]]]:
+    calibration_str = nas.metadata["cal_std_id"]
+    if "sec_std_id" in nas.metadata and nas.metadata["sec_std_id"] is not None:
+        calibration_str_2 = nas.metadata["sec_std_id"]
+        calibration_str += ";" + calibration_str_2
+    calib_dict = {}
+
+    calibrations = calibration_str.split(";")
+    for calibration in calibrations:
+        calibration_id = re.search(
+            r"Status calibration standard: (\d+)", calibration
+        ).group(1)
+        calib_fields = re.split(r",(?![^{}]*\})", calibration, 0)
+
+        fields_dict: dict[str, str | dict[str, float]] = {}
+        for field in calib_fields:
+            field_parts = field.strip().split(":")
+            field_name = field_parts[0].strip()
+            fields_dict[field_name] = ":".join(field_parts[1:]).strip()
+
+        calibration_id = int(calibration_id)
+        # Check if we have a concentration field
+        if "Concentrations" in fields_dict:
+            concentration_dict = extract_concentration_field(
+                fields_dict["Concentrations"]
+            )
+            fields_dict["Concentrations"] = concentration_dict
+
+        calib_dict[calibration_id] = fields_dict
+
+    return calib_dict
```

### Comparing `avoca-0.2.0/avoca/qa_class/abstract.py` & `avoca-0.3.0/avoca/qa_class/abstract.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/qa_class/concs.py` & `avoca-0.3.0/avoca/qa_class/concs.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/qa_class/generate_classes_doc.py` & `avoca-0.3.0/avoca/qa_class/generate_classes_doc.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/qa_class/rt.py` & `avoca-0.3.0/avoca/qa_class/rt.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/qa_class/test.py` & `avoca-0.3.0/avoca/qa_class/test.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/qa_class/zscore.py` & `avoca-0.3.0/avoca/qa_class/zscore.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/avoca/utils/torch_models.py` & `avoca-0.3.0/avoca/utils/torch_models.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas` & `avoca-0.3.0/data/CH0001G.20240219123300.20240307132229.online_gc.NMHC.air.16d.61mn.CH01L_Agilent_GC-MS-MEDUSA_Medusa-12_JFJ.CH01L_gc_ms.lev0.nas`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/data/voc_jan2jun_2023.csv` & `avoca-0.3.0/data/voc_jan2jun_2023.csv`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/docs/Makefile` & `avoca-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/docs/make.bat` & `avoca-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/docs/source/conf.py` & `avoca-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/docs/source/index.rst` & `avoca-0.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/docs/source/quickstart.ipynb` & `avoca-0.3.0/docs/source/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/docs/source/bindings/ebas.md` & `avoca-0.3.0/docs/source/bindings/ebas.md`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/examples/data_qa.ipynb` & `avoca-0.3.0/examples/data_qa.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/examples/read_nas.ipynb` & `avoca-0.3.0/examples/read_nas.ipynb`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/LICENCE.txt` & `avoca-0.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `avoca-0.2.0/pyproject.toml` & `avoca-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "avoca"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Lionel Constantin", email="lionel.constantin@empa.ch" },
 ]
 description = "@voc@: Quality assessement of measurement data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `avoca-0.2.0/PKG-INFO` & `avoca-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: avoca
-Version: 0.2.0
+Version: 0.3.0
 Summary: @voc@: Quality assessement of measurement data
 Project-URL: Homepage, https://gitlab.com/empa503/atmospheric-measurements/avoca
 Project-URL: Bug Tracker, https://gitlab.com/empa503/atmospheric-measurements/avoca/-/issues
 Project-URL: Documentation, http://avoca.readthedocs.io/
 Author-email: Lionel Constantin <lionel.constantin@empa.ch>
 License-File: LICENCE.txt
 Classifier: License :: OSI Approved :: MIT License
@@ -27,20 +27,21 @@
 Requires-Dist: myst-nb; extra == 'doc'
 Requires-Dist: myst-parser; extra == 'doc'
 Requires-Dist: sphinx; extra == 'doc'
 Description-Content-Type: text/markdown
 
 # avoca 
 
-Quality assessement of data.
+Python package for Quality assessement of data.
+
+Official name is `@voc@` but it is called `avoca` for simplicity.
 
 ## Documentation 
 
-Currenlty only the source code is documented.
-We plan on generating a full documentation.
+A documentation can be found at (http://avoca.readthedocs.io/)
 
 
 ## License
 
 This project is licensed under the MIT License.
 
 It is managed by the a group of researchers at [Empa](https://www.empa.ch/web/s503/climate-gases)
```

