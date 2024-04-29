# Comparing `tmp/cesnet-datazoo-0.1.3.tar.gz` & `tmp/cesnet_datazoo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet-datazoo-0.1.3.tar", last modified: Tue Apr  9 16:44:29 2024, max compression
+gzip compressed data, was "cesnet_datazoo-0.1.4.tar", last modified: Mon Apr 29 08:35:20 2024, max compression
```

## Comparing `cesnet-datazoo-0.1.3.tar` & `cesnet_datazoo-0.1.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.850830 cesnet-datazoo-0.1.3/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-datazoo-0.1.3/LICENCE
--rw-rw-rw-   0        0        0    12953 2024-04-09 16:44:29.849830 cesnet-datazoo-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    11374 2024-04-09 14:38:48.000000 cesnet-datazoo-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.808037 cesnet-datazoo-0.1.3/cesnet_datazoo/
--rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/__init__.py
--rw-rw-rw-   0        0        0    38035 2024-04-08 12:52:42.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/config.py
--rw-rw-rw-   0        0        0     1294 2024-03-26 11:19:49.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.834150 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/
--rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/__init__.py
--rw-rw-rw-   0        0        0    46458 2024-04-05 09:42:58.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/cesnet_dataset.py
--rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/datasets.py
--rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/datasets_constants.py
--rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/loaders.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.837155 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/
--rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/__init__.py
--rw-rw-rw-   0        0        0     1608 2024-03-13 16:30:28.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/dataset_metadata.py
--rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/metadata.csv
--rw-rw-rw-   0        0        0    15137 2024-03-14 10:55:15.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/statistics.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.839156 cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/
--rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/__init__.py
--rw-rw-rw-   0        0        0     4038 2024-04-08 10:03:47.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/classification_report.py
--rw-rw-rw-   0        0        0     1303 2024-03-13 15:46:01.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/provider_metrics.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.842522 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/
--rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/__init__.py
--rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/apps_split.py
--rw-rw-rw-   0        0        0     5083 2024-03-19 14:07:14.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/data_scalers.py
--rw-rw-rw-   0        0        0    13011 2024-03-26 09:58:57.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/indices_setup.py
--rw-rw-rw-   0        0        0    17881 2024-04-05 09:43:19.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/pytables_dataset.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.847443 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/__init__.py
--rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/class_info.py
--rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/download.py
--rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/fileutils.py
--rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet-datazoo-0.1.3/cesnet_datazoo/utils/random.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:44:29.848825 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/
--rw-rw-rw-   0        0        0    12953 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      238 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-09 16:44:29.000000 cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1792 2024-04-09 16:43:51.000000 cesnet-datazoo-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 16:44:29.850830 cesnet-datazoo-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.306340 cesnet_datazoo-0.1.4/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_datazoo-0.1.4/LICENCE
+-rw-rw-rw-   0        0        0    12953 2024-04-29 08:35:20.305333 cesnet_datazoo-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    11374 2024-04-09 14:38:48.000000 cesnet_datazoo-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.263486 cesnet_datazoo-0.1.4/cesnet_datazoo/
+-rw-rw-rw-   0        0        0        0 2023-09-04 15:14:00.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/__init__.py
+-rw-rw-rw-   0        0        0    38406 2024-04-26 10:09:35.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/config.py
+-rw-rw-rw-   0        0        0     1481 2024-04-26 10:10:11.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.289841 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/
+-rw-rw-rw-   0        0        0      443 2023-10-09 14:50:14.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/__init__.py
+-rw-rw-rw-   0        0        0    46635 2024-04-26 12:29:44.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/cesnet_dataset.py
+-rw-rw-rw-   0        0        0     3617 2024-03-13 15:20:57.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/datasets.py
+-rw-rw-rw-   0        0        0    29154 2024-03-13 15:20:40.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/datasets_constants.py
+-rw-rw-rw-   0        0        0     1854 2024-03-14 10:53:21.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/loaders.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.292010 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/
+-rw-rw-rw-   0        0        0        0 2023-08-21 14:08:44.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/__init__.py
+-rw-rw-rw-   0        0        0     1623 2024-04-26 12:35:59.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/dataset_metadata.py
+-rw-rw-rw-   0        0        0     2175 2024-03-19 11:54:21.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/metadata.csv
+-rw-rw-rw-   0        0        0    15137 2024-04-26 12:36:13.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/statistics.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.294530 cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/
+-rw-rw-rw-   0        0        0        0 2023-08-17 21:32:34.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/__init__.py
+-rw-rw-rw-   0        0        0     3981 2024-04-26 10:13:11.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/classification_report.py
+-rw-rw-rw-   0        0        0     1374 2024-04-17 16:35:50.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/provider_metrics.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.298903 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/
+-rw-rw-rw-   0        0        0        0 2023-09-01 14:24:29.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/__init__.py
+-rw-rw-rw-   0        0        0     1411 2023-10-30 20:40:56.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/apps_split.py
+-rw-rw-rw-   0        0        0     5083 2024-03-19 14:07:14.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/data_scalers.py
+-rw-rw-rw-   0        0        0    13717 2024-04-26 12:13:42.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/indices_setup.py
+-rw-rw-rw-   0        0        0    19413 2024-04-26 12:33:06.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/pytables_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.303312 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:35:45.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/__init__.py
+-rw-rw-rw-   0        0        0     2462 2024-04-04 20:29:42.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/class_info.py
+-rw-rw-rw-   0        0        0     1441 2024-02-20 11:51:54.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/download.py
+-rw-rw-rw-   0        0        0      642 2023-09-01 13:43:06.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/fileutils.py
+-rw-rw-rw-   0        0        0      575 2023-09-26 08:58:11.000000 cesnet_datazoo-0.1.4/cesnet_datazoo/utils/random.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:35:20.303827 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/
+-rw-rw-rw-   0        0        0    12953 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      238 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-29 08:35:20.000000 cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1792 2024-04-26 13:30:41.000000 cesnet_datazoo-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:35:20.306340 cesnet_datazoo-0.1.4/setup.cfg
```

### Comparing `cesnet-datazoo-0.1.3/LICENCE` & `cesnet_datazoo-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/PKG-INFO` & `cesnet_datazoo-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.3
+Version: 0.1.4
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
```

### Comparing `cesnet-datazoo-0.1.3/README.md` & `cesnet_datazoo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/config.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 from enum import Enum
 from typing import TYPE_CHECKING, Callable, Literal, Optional
 
 import yaml
 from pydantic import model_validator
 from pydantic.dataclasses import dataclass
 
-from cesnet_datazoo.constants import (PHIST_BIN_COUNT, PPI_MAX_LEN, SELECTED_TCP_FLAGS,
-                                      TCP_PPI_CHANNELS, UDP_PPI_CHANNELS)
+from cesnet_datazoo.constants import (PHIST_BIN_COUNT, PPI_MAX_LEN, QUIC_SNI_COLUMN,
+                                      SELECTED_TCP_FLAGS, TCP_PPI_CHANNELS, TLS_SNI_COLUMN,
+                                      UDP_PPI_CHANNELS)
 
 if TYPE_CHECKING:
     from cesnet_datazoo.datasets.cesnet_dataset import CesnetDataset
 
 
 class Protocol(Enum):
     TLS = "TLS"
@@ -124,14 +125,15 @@
         database_filename: Taken from the dataset instance.
         database_path: Taken from the dataset instance.
         servicemap_path: Taken from the dataset instance.
         flowstats_features: Taken from `dataset.metadata.flowstats_features`.
         flowstats_features_boolean: Taken from `dataset.metadata.flowstats_features_boolean`.
         flowstats_features_phist: Taken from `dataset.metadata.packet_histograms` if `use_packet_histograms` is true, otherwise an empty list.
         other_fields: Taken from `dataset.metadata.other_fields` if `return_other_fields` is true, otherwise an empty list.
+        sni_column: Database column with SNI domains, can be None for datasets without SNI domains.
 
     # Configuration options
 
     Attributes:
         need_train_set: Use to disable the train set. `Default: True`
         need_val_set: Use to disable the validation set. `Default: True`
         need_test_set: Use to disable the test set. `Default: True`
@@ -339,14 +341,16 @@
             if len(train_dates) > 0 and min(val_dates) <= max(train_dates):
                 warnings.warn(f"Some validation dates ({min(val_dates).strftime('%Y%m%d')}) are before or equal to the last train date ({max(train_dates).strftime('%Y%m%d')}). This might lead to improper evaluation and should be avoided.")
             if len(test_dates) > 0 and min(test_dates) <= max(val_dates):
                 warnings.warn(f"Some test dates ({min(test_dates).strftime('%Y%m%d')}) are before or equal to the last validation date ({max(val_dates).strftime('%Y%m%d')}). This might lead to improper evaluation and should be avoided.")
         # Configure features
         self.flowstats_features = dataset.metadata.flowstats_features
         self.flowstats_features_boolean = dataset.metadata.flowstats_features_boolean
+        sni_column = TLS_SNI_COLUMN if dataset.metadata.protocol == Protocol.TLS else QUIC_SNI_COLUMN
+        self.sni_column = sni_column if sni_column in dataset.metadata.other_fields else None
         self.other_fields = dataset.metadata.other_fields if self.return_other_fields else []
         if self.use_packet_histograms:
             if len(dataset.metadata.packet_histograms) == 0:
                 raise ValueError("This dataset does not support use_packet_histograms")
             self.flowstats_features_phist = dataset.metadata.packet_histograms
         else:
             self.flowstats_features_phist = []
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/constants.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,10 +35,12 @@
 
 # Class labels
 UNKNOWN_STR_LABEL = "_unknown"
 DEFAULT_BACKGROUND_CLASS = "default-background"
 GOOGLE_BACKGROUND_CLASS = "google-background"
 
 # Indices
-INDICES_TABLE_POS = 0
-INDICES_INDEX_POS = 1
-INDICES_LABEL_POS = 2
+INDICES_TABLE_FIELD = "TABLE"
+INDICES_INDEX_FIELD = "INDEX"
+INDICES_APP_FIELD = "APP"
+INDICES_SNI_FIELD = "SNI"
+INDICES_DTYPE = [(INDICES_TABLE_FIELD, "int32"), (INDICES_INDEX_FIELD, "int32"), (INDICES_APP_FIELD, "int32"), (INDICES_SNI_FIELD, "U50")]
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/cesnet_dataset.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/cesnet_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import torch
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import LabelEncoder
 from torch.utils.data import BatchSampler, DataLoader, RandomSampler, Sampler, SequentialSampler
 from typing_extensions import assert_never
 
 from cesnet_datazoo.config import AppSelection, DataLoaderOrder, DatasetConfig, ValidationApproach
-from cesnet_datazoo.constants import (APP_COLUMN, CATEGORY_COLUMN, DATASET_SIZES, INDICES_LABEL_POS,
+from cesnet_datazoo.constants import (APP_COLUMN, CATEGORY_COLUMN, DATASET_SIZES, INDICES_APP_FIELD,
                                       SERVICEMAP_FILE, UNKNOWN_STR_LABEL)
 from cesnet_datazoo.datasets.loaders import collate_fn_simple, create_df_from_dataloader
 from cesnet_datazoo.datasets.metadata.dataset_metadata import DatasetMetadata, load_metadata
 from cesnet_datazoo.datasets.statistics import compute_dataset_statistics
 from cesnet_datazoo.pytables_data.apps_split import is_background_app
 from cesnet_datazoo.pytables_data.data_scalers import fit_scalers
 from cesnet_datazoo.pytables_data.indices_setup import (IndicesTuple, compute_known_app_counts,
@@ -551,15 +551,15 @@
                                                                                                  unknown_apps=unknown_apps,
                                                                                                  tables_app_enum=self._tables_app_enum,
                                                                                                  disable_indices_cache=disable_indices_cache,)
             elif dataset_config.val_approach == ValidationApproach.SPLIT_FROM_TRAIN:
                 train_val_rng = get_fresh_random_generator(dataset_config=dataset_config, section=RandomizedSection.TRAIN_VAL_SPLIT)
                 val_data_path = dataset_config._get_train_data_path()
                 val_unknown_indices = train_unknown_indices
-                train_labels = train_indices[:, INDICES_LABEL_POS]
+                train_labels = train_indices[INDICES_APP_FIELD]
                 if dataset_config.train_dates_weigths is not None:
                     assert dataset_config.val_known_size != "all"
                     # When weight sampling is used, val_known_size is kept but the resulting train size can be smaller due to no enough samples in some train dates
                     if dataset_config.val_known_size > len(train_indices):
                         raise ValueError(f"Requested validation size ({dataset_config.val_known_size}) is larger than the number of available train samples after weight sampling ({len(train_indices)})")
                     train_indices, val_known_indices = train_test_split(train_indices, test_size=dataset_config.val_known_size, stratify=train_labels, shuffle=True, random_state=train_val_rng)
                     dataset_config.train_size = len(train_indices)
@@ -622,14 +622,15 @@
                 indices=dataset_indices.train_indices,
                 tables_app_enum=self._tables_app_enum,
                 tables_cat_enum=self._tables_cat_enum,
                 flowstats_features=dataset_config.flowstats_features,
                 flowstats_features_boolean=dataset_config.flowstats_features_boolean,
                 flowstats_features_phist=dataset_config.flowstats_features_phist,
                 other_fields=self.dataset_config.other_fields,
+                sni_column=self.dataset_config.sni_column,
                 ppi_channels=dataset_config.get_ppi_channels(),
                 ppi_transform=dataset_config.ppi_transform,
                 flowstats_transform=dataset_config.flowstats_transform,
                 flowstats_phist_transform=dataset_config.flowstats_phist_transform,
                 target_transform=encode_labels_with_unknown_fn,
                 return_tensors=dataset_config.return_tensors,)
         if dataset_config.need_val_set:
@@ -640,14 +641,15 @@
                 indices=dataset_indices.val_known_indices,
                 tables_app_enum=self._tables_app_enum,
                 tables_cat_enum=self._tables_cat_enum,
                 flowstats_features=dataset_config.flowstats_features,
                 flowstats_features_boolean=dataset_config.flowstats_features_boolean,
                 flowstats_features_phist=dataset_config.flowstats_features_phist,
                 other_fields=self.dataset_config.other_fields,
+                sni_column=self.dataset_config.sni_column,
                 ppi_channels=dataset_config.get_ppi_channels(),
                 ppi_transform=dataset_config.ppi_transform,
                 flowstats_transform=dataset_config.flowstats_transform,
                 flowstats_phist_transform=dataset_config.flowstats_phist_transform,
                 target_transform=encode_labels_with_unknown_fn,
                 return_tensors=dataset_config.return_tensors,
                 preload=dataset_config.preload_val,
@@ -660,14 +662,15 @@
                 indices=test_combined_indices,
                 tables_app_enum=self._tables_app_enum,
                 tables_cat_enum=self._tables_cat_enum,
                 flowstats_features=dataset_config.flowstats_features,
                 flowstats_features_boolean=dataset_config.flowstats_features_boolean,
                 flowstats_features_phist=dataset_config.flowstats_features_phist,
                 other_fields=self.dataset_config.other_fields,
+                sni_column=self.dataset_config.sni_column,
                 ppi_channels=dataset_config.get_ppi_channels(),
                 ppi_transform=dataset_config.ppi_transform,
                 flowstats_transform=dataset_config.flowstats_transform,
                 flowstats_phist_transform=dataset_config.flowstats_phist_transform,
                 target_transform=encode_labels_with_unknown_fn,
                 return_tensors=dataset_config.return_tensors,
                 preload=dataset_config.preload_test,
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/datasets.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/datasets_constants.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/datasets_constants.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/loaders.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/loaders.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/dataset_metadata.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/dataset_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,9 +35,9 @@
     def parse_string_to_list(cls, v: str, info: ValidationInfo) -> list[str]:
         l = list(map(str.strip, v.split(","))) if v else []
         return l
 
 metadata_df = pd.read_csv(os.path.join(os.path.dirname(__file__), "metadata.csv"), index_col="Name", keep_default_na=False)
 def load_metadata(dataset_name: str) -> DatasetMetadata:
     d = metadata_df.loc[dataset_name].to_dict()
-    d = {k.replace(" ", "_").lower(): v for k, v in d.items()}
+    d = {k.replace(" ", "_").lower(): v for k, v in d.items()} # type: ignore
     return DatasetMetadata(**d)
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/metadata/metadata.csv` & `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/metadata/metadata.csv`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/datasets/statistics.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/datasets/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     table_paths = list_all_tables(database_path)
     stats_dataset = PyTablesDataset(database_path=database_path,
                                     tables_app_enum=tables_app_enum,
                                     tables_cat_enum=tables_cat_enum,
                                     tables_paths=table_paths,
                                     indices=None,
                                     disabled_apps=disabled_apps,
-                                    return_all_fields=True,
+                                    return_raw_fields=True,
                                     flowstats_features=[],
                                     flowstats_features_boolean=[],
                                     flowstats_features_phist=[],
                                     other_fields=[],
                                     ppi_channels=UDP_PPI_CHANNELS,)
     if num_samples != "all":
         subset_indices = np.random.randint(low=0, high=len(stats_dataset.indices), size=num_samples)
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/classification_report.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/classification_report.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import numpy as np
 from sklearn.metrics import accuracy_score, precision_recall_fscore_support
 
-from cesnet_datazoo.metrics.provider_metrics import (per_app_provider_metrics,
-                                                       provider_accuracies)
+from cesnet_datazoo.metrics.provider_metrics import per_app_provider_metrics, provider_accuracies
 from cesnet_datazoo.utils.class_info import ClassInfo
 
 
-def better_classification_report(y_true: np.ndarray, y_pred: np.ndarray, cm: np.ndarray, labels: list[int], class_info: ClassInfo, digits: int = 2, zero_division: int = 0) -> tuple[str, dict[str, float]]:
-    p, r, f1, s  = precision_recall_fscore_support(y_true, y_pred,
+def better_classification_report(test_labels: np.ndarray, preds: np.ndarray, cm: np.ndarray, labels: list[int], class_info: ClassInfo, digits: int = 2, zero_division: int = 0) -> tuple[str, dict[str, float]]:
+    p, r, f1, s  = precision_recall_fscore_support(test_labels, preds,
                                                    labels=labels,
                                                    zero_division=zero_division)
     sc_p, sc_r, sc_f1 = per_app_provider_metrics(cm, class_info=class_info)
     predicted_unknown = cm[:, -1]
     with np.errstate(divide="ignore", invalid="ignore"):
         predicted_unknown_perc = predicted_unknown / s
         predicted_unknown_perc = np.nan_to_num(predicted_unknown_perc)
@@ -42,24 +41,24 @@
 
     headers_avg = ["precision (pr)", "recall (pr)", "f1-score (pr)", "pred unknown", "support"]
     row_fmt_avg = "{:>{width}} " + 3 * " {:>6.{digits}} ({:.{digits}f}) " + "{:>15} " + "{:>9}\n"
     digits = 3 # show more precise averages
     report += headers_fmt.format("", *headers_avg, width=width)
     report += row_fmt_avg.format("macro avg", *row_avg, width=width, digits=digits)
 
-    acc = accuracy_score(y_true, y_pred)
-    provider_acc, failed_provider_acc = provider_accuracies(y_true, y_pred, class_info=class_info)
+    acc = accuracy_score(test_labels, preds)
+    provider_acc, failed_provider_acc = provider_accuracies(test_labels, preds, class_info=class_info)
 
     row_fmt_acc = "{:>{width}} {:>15} {:>15} {:>7.{digits}f}\n"
     report += row_fmt_acc.format("acc", "", "", acc, width=width, digits=digits)
     report += row_fmt_acc.format("provider acc", "", "", provider_acc, width=width, digits=digits)
     report += row_fmt_acc.format("failed provider acc", "", "", failed_provider_acc, width=width, digits=digits)
     metrics = {
-        "Test/Accuracy": acc,
-        "Test/Provider Accuracy": provider_acc,
-        "Test/Failed Provider Accuracy": failed_provider_acc,
-        "Test/Fscore": avg_f1,
-        "Test/Provider Fscore": avg_sc_f1,
-        "Test/Recall": avg_r,
-        "Test/Provider Recall": avg_sc_r,
+        "test/acc": acc,
+        "test/provider-acc": provider_acc,
+        "test/failed-provider-acc": failed_provider_acc,
+        "test/fscore": avg_f1,
+        "test/provider-fscore": avg_sc_f1,
+        "test/recall": avg_r,
+        "test/provider-recall": avg_sc_r,
     }
     return report, metrics
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/metrics/provider_metrics.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/metrics/provider_metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 
 from cesnet_datazoo.utils.class_info import ClassInfo
 
 
-def provider_accuracies(y_true: np.ndarray, y_pred: np.ndarray, class_info: ClassInfo) -> tuple[float, float]:
+def provider_accuracies(true_labels: np.ndarray, preds: np.ndarray, class_info: ClassInfo) -> tuple[float, float]:
     provider_mapping_arr = np.array(list(class_info.provider_mapping.values()))
-    y_true_sc = provider_mapping_arr[y_true]
-    y_pred_sc = provider_mapping_arr[y_pred]
-    mistakes = y_true != y_pred
-    provider_acc = (y_true_sc == y_pred_sc).sum() / len(y_true_sc)
-    failed_provider_acc = (y_true_sc[mistakes] == y_pred_sc[mistakes]).sum() / mistakes.sum()
+    true_labels_provider = provider_mapping_arr[true_labels]
+    preds_provider = provider_mapping_arr[preds]
+    mistakes = true_labels != preds
+    provider_acc = (true_labels_provider == preds_provider).sum() / len(true_labels_provider)
+    failed_provider_acc = (true_labels_provider[mistakes] == preds_provider[mistakes]).sum() / mistakes.sum()
     return provider_acc, failed_provider_acc
 
 def per_app_provider_metrics(cm, class_info: ClassInfo):
     metrics = []
     for i, app in enumerate(class_info.target_names):
         if not class_info.has_provider[app]:
             metrics.append((None, None, None))
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/apps_split.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/apps_split.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/data_scalers.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/data_scalers.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/indices_setup.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/indices_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 import dataclasses
 import logging
 import os
+import time
 import warnings
 from collections import namedtuple
 from enum import Enum
 
 import numpy as np
 import pandas as pd
 
 from cesnet_datazoo.config import DatasetConfig
-from cesnet_datazoo.constants import INDICES_INDEX_POS, INDICES_LABEL_POS, INDICES_TABLE_POS
+from cesnet_datazoo.constants import (INDICES_APP_FIELD, INDICES_DTYPE, INDICES_INDEX_FIELD,
+                                      INDICES_TABLE_FIELD)
 from cesnet_datazoo.pytables_data.pytables_dataset import init_test_indices, init_train_indices
 from cesnet_datazoo.utils.fileutils import yaml_dump, yaml_load
 from cesnet_datazoo.utils.random import RandomizedSection, get_fresh_random_generator
 
 log = logging.getLogger(__name__)
 TRAIN_DATA_PARAMS_FILE = "train_data_params.yaml"
 TEST_DATA_PARAMS_FILE = "test_data_params.yaml"
 IndicesTuple = namedtuple("IndicesTuple", ["train_indices", "val_known_indices", "val_unknown_indices", "test_known_indices", "test_unknown_indices"])
 
 
 def sort_indices(indices: np.ndarray) -> np.ndarray:
-    idxs = np.argsort(indices[:, INDICES_INDEX_POS])
-    res = idxs[np.argsort(indices[idxs, INDICES_TABLE_POS], kind="stable")]
+    idxs = np.argsort(indices[INDICES_INDEX_FIELD])
+    res = idxs[np.argsort(indices[idxs][INDICES_TABLE_FIELD], kind="stable")]
     return indices[res]
 
 def subset_and_sort_indices(dataset_config: DatasetConfig, dataset_indices: IndicesTuple) -> IndicesTuple:
     if dataset_config.train_size == "all":
         dataset_config.train_size = len(dataset_indices.train_indices)
     if dataset_config.val_known_size == "all":
         dataset_config.val_known_size = len(dataset_indices.val_known_indices)
@@ -57,15 +59,15 @@
         warnings.warn(f"Requested test unknown size {dataset_config.test_unknown_size} is larger than the number of available samples {len(test_unknown_indices)}.")
         dataset_config.test_unknown_size = len(test_unknown_indices)
     dataset_indices = IndicesTuple(train_indices=train_indices, val_known_indices=val_known_indices, val_unknown_indices=val_unknown_indices, test_known_indices=test_known_indices, test_unknown_indices=test_unknown_indices)
     return dataset_indices
 
 def date_weight_sample_train_indices(dataset_config: DatasetConfig, train_indices: np.ndarray, num_samples: int) -> np.ndarray:
     rng = get_fresh_random_generator(dataset_config=dataset_config, section=RandomizedSection.DATE_WEIGHT_SAMPLING)
-    indices_per_date = [train_indices[train_indices[:, INDICES_TABLE_POS] == i] for i in np.unique(train_indices[:, INDICES_TABLE_POS])]
+    indices_per_date = [train_indices[train_indices[INDICES_TABLE_FIELD] == i] for i in np.unique(train_indices[INDICES_TABLE_FIELD])]
     weights = np.array(dataset_config.train_dates_weigths)
     weights = weights / weights.sum()
     samples_per_date = np.ceil((weights * (num_samples))).astype(int)
     samples_per_date_clipped = np.clip(samples_per_date, a_max=list(map(len, indices_per_date)), a_min=0)
     df = pd.DataFrame(data={"Dates": dataset_config.train_dates, "Weights": dataset_config.train_dates_weigths, "Requested Samples": samples_per_date, "Available Samples": samples_per_date_clipped})
     log.info(f"Weight sampling per date with requsted total number of samples {num_samples} (train_size + val_known_size when using the split-from-train validation approach; train_size otherwise)")
     for l in df.to_string(index=False).splitlines():
@@ -73,15 +75,15 @@
     if not all(samples_per_date == samples_per_date_clipped):
         warnings.warn("Some dates have not enough samples, resulting train size will be smaller")
     sampled_indicies_per_date = [indices[rng.choice(len(indices), size=n, replace=False)] for indices, n in zip(indices_per_date, samples_per_date_clipped)]
     sampled_train_indices = np.concatenate(sampled_indicies_per_date)
     return sampled_train_indices
 
 def indices_to_app_counts(indices: np.ndarray, tables_app_enum: dict[int, str]) -> pd.Series:
-    app_counts = pd.Series(indices[:, INDICES_LABEL_POS]).value_counts()
+    app_counts = pd.Series(indices[INDICES_APP_FIELD]).value_counts()
     app_counts.index = app_counts.index.map(lambda x: tables_app_enum[x])
     return app_counts
 
 def compute_known_app_counts(dataset_indices: IndicesTuple, tables_app_enum: dict[int, str]) -> pd.DataFrame:
     train_app_counts = indices_to_app_counts(dataset_indices.train_indices, tables_app_enum)
     val_known_app_counts = indices_to_app_counts(dataset_indices.val_known_indices, tables_app_enum)
     test_known_app_counts = indices_to_app_counts(dataset_indices.test_known_indices, tables_app_enum)
@@ -95,73 +97,82 @@
     return df
 
 def init_or_load_train_indices(dataset_config: DatasetConfig, tables_app_enum: dict[int, str], servicemap: pd.DataFrame, disable_indices_cache: bool) -> tuple[np.ndarray, np.ndarray, list[str], list[str]]:
     train_data_path = dataset_config._get_train_data_path()
     init_train_data(train_data_path)
     if not os.path.isfile(os.path.join(train_data_path, TRAIN_DATA_PARAMS_FILE)):
         log.info("Processing train indices")
+        start_time = time.time()
         train_data_params = dataset_config._get_train_data_params()
         train_known_indices, train_unknown_indices, known_apps, unknown_apps = init_train_indices(train_data_params=train_data_params,
                                                                                                   database_path=dataset_config.database_path,
                                                                                                   tables_app_enum=tables_app_enum,
+                                                                                                  sni_column=dataset_config.sni_column,
                                                                                                   servicemap=servicemap,
                                                                                                   rng=get_fresh_random_generator(dataset_config=dataset_config, section=RandomizedSection.INIT_TRAIN_INDICES))
         if not disable_indices_cache:
             yaml_dump({k: str(v) if isinstance(v, Enum) else list(v) if isinstance(v, tuple) else v for k, v in dataclasses.asdict(train_data_params).items()}, os.path.join(train_data_path, TRAIN_DATA_PARAMS_FILE))
             yaml_dump(known_apps, os.path.join(train_data_path, "known_apps.yaml"))
             yaml_dump(unknown_apps, os.path.join(train_data_path, "unknown_apps.yaml"))
-            np.save(os.path.join(train_data_path, "train_known_indices.npy"), train_known_indices)
-            np.save(os.path.join(train_data_path, "train_unknown_indices.npy"), train_unknown_indices)
+            np.savez_compressed(os.path.join(train_data_path, "train_indices.npz"), train_known_indices=train_known_indices, train_unknown_indices=train_unknown_indices)
+        log.info(f"Processing indices took {time.time() - start_time:.2f} seconds")
     else:
         known_apps = yaml_load(os.path.join(train_data_path, "known_apps.yaml"))
         unknown_apps = yaml_load(os.path.join(train_data_path, "unknown_apps.yaml"))
-        train_known_indices = np.load(os.path.join(train_data_path, "train_known_indices.npy"))
-        train_unknown_indices = np.load(os.path.join(train_data_path, "train_unknown_indices.npy"))
+        loaded = np.load(os.path.join(train_data_path, "train_indices.npz"))
+        train_known_indices = loaded["train_known_indices"]
+        train_unknown_indices = loaded["train_unknown_indices"]
     return train_known_indices, train_unknown_indices, known_apps, unknown_apps
 
 def init_or_load_val_indices(dataset_config: DatasetConfig, known_apps: list[str], unknown_apps: list[str], tables_app_enum: dict[int, str], disable_indices_cache: bool) -> tuple[np.ndarray, np.ndarray, str]:
     val_data_params, val_data_path = dataset_config._get_val_data_params_and_path(known_apps=known_apps, unknown_apps=unknown_apps)
     init_test_data(val_data_path)
     if not os.path.isfile(os.path.join(val_data_path, TEST_DATA_PARAMS_FILE)):
         log.info("Processing validation indices")
+        start_time = time.time()
         val_known_indices, val_unknown_indices = init_test_indices(test_data_params=val_data_params,
                                                                    database_path=dataset_config.database_path,
                                                                    tables_app_enum=tables_app_enum,
+                                                                   sni_column=dataset_config.sni_column,
                                                                    rng=get_fresh_random_generator(dataset_config=dataset_config, section=RandomizedSection.INIT_VAL_INIDICES))
         if not disable_indices_cache:
             yaml_dump(dataclasses.asdict(val_data_params), os.path.join(val_data_path, TEST_DATA_PARAMS_FILE))
-            np.save(os.path.join(val_data_path, "val_known_indices.npy"), val_known_indices)
-            np.save(os.path.join(val_data_path, "val_unknown_indices.npy"), val_unknown_indices)
+            np.savez_compressed(os.path.join(val_data_path, "val_indices.npz"), val_known_indices=val_known_indices, val_unknown_indices=val_unknown_indices)
+        log.info(f"Processing indices took {time.time() - start_time:.2f} seconds")
     else:
-        val_known_indices = np.load(os.path.join(val_data_path, "val_known_indices.npy"))
-        val_unknown_indices = np.load(os.path.join(val_data_path, "val_unknown_indices.npy"))
+        loaded = np.load(os.path.join(val_data_path, "val_indices.npz"))
+        val_known_indices = loaded["val_known_indices"]
+        val_unknown_indices = loaded["val_unknown_indices"]
     return val_known_indices, val_unknown_indices, val_data_path
 
 def init_or_load_test_indices(dataset_config: DatasetConfig, known_apps: list[str], unknown_apps: list[str], tables_app_enum: dict[int, str], disable_indices_cache: bool) -> tuple[np.ndarray, np.ndarray, str]:
     test_data_params, test_data_path = dataset_config._get_test_data_params_and_path(known_apps=known_apps, unknown_apps=unknown_apps)
     init_test_data(test_data_path)
     if not os.path.isfile(os.path.join(test_data_path, TEST_DATA_PARAMS_FILE)):
         log.info("Processing test indices")
+        start_time = time.time()
         test_known_indices, test_unknown_indices = init_test_indices(test_data_params=test_data_params,
                                                                      database_path=dataset_config.database_path,
                                                                      tables_app_enum=tables_app_enum,
+                                                                     sni_column=dataset_config.sni_column,
                                                                      rng=get_fresh_random_generator(dataset_config=dataset_config, section=RandomizedSection.INIT_TEST_INDICES))
         if not disable_indices_cache:
             yaml_dump(dataclasses.asdict(test_data_params), os.path.join(test_data_path, TEST_DATA_PARAMS_FILE))
-            np.save(os.path.join(test_data_path, "test_known_indices.npy"), test_known_indices)
-            np.save(os.path.join(test_data_path, "test_unknown_indices.npy"), test_unknown_indices)
+            np.savez_compressed(os.path.join(test_data_path, "test_indices.npz"), test_known_indices=test_known_indices, test_unknown_indices=test_unknown_indices)
+        log.info(f"Processing indices took {time.time() - start_time:.2f} seconds")
     else:
-        test_known_indices = np.load(os.path.join(test_data_path, "test_known_indices.npy"))
-        test_unknown_indices = np.load(os.path.join(test_data_path, "test_unknown_indices.npy"))
+        loaded = np.load(os.path.join(test_data_path, "test_indices.npz"))
+        test_known_indices = loaded["test_known_indices"]
+        test_unknown_indices = loaded["test_unknown_indices"]
     return test_known_indices, test_unknown_indices, test_data_path
 
 def init_train_data(train_data_path: str):
     os.makedirs(train_data_path, exist_ok=True)
     os.makedirs(os.path.join(train_data_path, "transforms"), exist_ok=True)
     os.makedirs(os.path.join(train_data_path, "preload"), exist_ok=True)
 
 def init_test_data(test_data_path: str):
     os.makedirs(test_data_path, exist_ok=True)
     os.makedirs(os.path.join(test_data_path, "preload"), exist_ok=True)
 
 def no_indices() -> np.ndarray:
-    return np.zeros((0,3), dtype=np.int64)
+    return np.empty(shape=(0,), dtype=INDICES_DTYPE)
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/pytables_data/pytables_dataset.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/pytables_data/pytables_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import torch
 from numpy.lib.recfunctions import structured_to_unstructured
 from torch.utils.data import Dataset
 from typing_extensions import assert_never
 
 from cesnet_datazoo.config import (AppSelection, MinTrainSamplesCheck, TestDataParams,
                                    TrainDataParams)
-from cesnet_datazoo.constants import (APP_COLUMN, INDICES_INDEX_POS, INDICES_TABLE_POS, PPI_COLUMN,
-                                      QUIC_SNI_COLUMN, TLS_SNI_COLUMN)
+from cesnet_datazoo.constants import (APP_COLUMN, INDICES_DTYPE, INDICES_INDEX_FIELD,
+                                      INDICES_TABLE_FIELD, PPI_COLUMN)
 from cesnet_datazoo.pytables_data.apps_split import (is_background_app,
                                                      split_apps_topx_with_provider_groups)
 
 log = logging.getLogger(__name__)
 
 
 class PyTablesDataset(Dataset):
@@ -32,20 +32,21 @@
                  tables_app_enum: dict[int, str],
                  tables_cat_enum: dict[int, str],
                  flowstats_features: list[str],
                  flowstats_features_boolean: list[str],
                  flowstats_features_phist: list[str],
                  other_fields: list[str],
                  ppi_channels: list[int],
+                 sni_column: Optional[str] = None,
                  ppi_transform: Optional[Callable] = None,
                  flowstats_transform: Optional[Callable] = None,
                  flowstats_phist_transform: Optional[Callable] = None,
                  target_transform: Optional[Callable] = None,
                  return_tensors: bool = False,
-                 return_all_fields: bool = False,
+                 return_raw_fields: bool = False,
                  preload: bool = False,
                  preload_blob: Optional[str] = None,
                  disabled_apps: Optional[list[str]] = None,):
         self.database_path = database_path
         self.tables_paths = tables_paths
         self.tables = {}
         self.tables_app_enum = tables_app_enum
@@ -56,33 +57,33 @@
         else:
             self.indices = indices
 
         self.flowstats_features = flowstats_features
         self.flowstats_features_boolean = flowstats_features_boolean
         self.flowstats_features_phist = flowstats_features_phist
         self.other_fields = other_fields
+        self.sni_column = sni_column
         self.ppi_channels = ppi_channels
         self.ppi_transform = ppi_transform
         self.flowstats_transform = flowstats_transform
         self.flowstats_phist_transform = flowstats_phist_transform
         self.target_transform = target_transform
         self.return_tensors = return_tensors
-        self.return_all_fields = return_all_fields
-        self.sni_column = TLS_SNI_COLUMN if TLS_SNI_COLUMN in self.other_fields else QUIC_SNI_COLUMN if QUIC_SNI_COLUMN in self.other_fields else None
+        self.return_raw_fields = return_raw_fields
 
         self.preload = preload
         self.preload_blob = preload_blob
 
     def __getitem__(self, batch_idx):
         # log.debug(f"worker {self.worker_id}: __getitem__")
         if self.preload:
             batch_data = self.data[batch_idx]
         else:
             batch_data = load_data_from_tables(tables=self.tables, indices=self.indices[batch_idx], data_dtype=self.data_dtype)
-        if self.return_all_fields:
+        if self.return_raw_fields:
             return (batch_data, batch_idx)
 
         # Prepare data
         x_ppi = batch_data[PPI_COLUMN].astype("float32")
         x_ppi = x_ppi[:, self.ppi_channels, :]
         x_flowstats = structured_to_unstructured(batch_data[self.flowstats_features], dtype="float32")
         if self.flowstats_features_boolean:
@@ -169,24 +170,29 @@
         self.database.close()
 
 def worker_init_fn(worker_id):
     worker_info = torch.utils.data.get_worker_info() # type: ignore
     dataset = worker_info.dataset
     dataset.pytables_worker_init(worker_id)
 
-def init_train_indices(train_data_params: TrainDataParams, database_path: str, tables_app_enum: dict[int, str], servicemap: pd.DataFrame, rng: np.random.RandomState) -> tuple[np.ndarray, np.ndarray, list[str], list[str]]:
+def init_train_indices(train_data_params: TrainDataParams, database_path: str, tables_app_enum: dict[int, str], sni_column: Optional[str], servicemap: pd.DataFrame, rng: np.random.RandomState) -> tuple[np.ndarray, np.ndarray, list[str], list[str]]:
     database, train_tables = load_database(database_path, tables_paths=train_data_params.train_tables_paths)
     inverted_tables_app_enum = {v: k for k, v in tables_app_enum.items()}
-    all_app_labels = {}
+    all_labels = {}
+    all_sni_domains = {}
     app_counts = pd.Series(dtype="int64")
     start_time = time.time()
     for i, table_path in enumerate(train_data_params.train_tables_paths):
-        all_app_labels[i] = train_tables[i].read(field=APP_COLUMN)
-        log.info(f"Reading app column for table {table_path} took {time.time() - start_time:.2f} seconds"); start_time = time.time()
-        app_counts = app_counts.add(pd.Series(all_app_labels[i]).value_counts(), fill_value=0)
+        all_labels[i] = train_tables[i].read(field=APP_COLUMN)
+        if sni_column is not None:
+            all_sni_domains[i] = train_tables[i].read(field=sni_column)
+        else:
+            all_sni_domains[i] = np.full_like(all_labels[i], "", dtype="U1")
+        log.info(f"Reading app and SNI columns for table {table_path} took {time.time() - start_time:.2f} seconds"); start_time = time.time()
+        app_counts = app_counts.add(pd.Series(all_labels[i]).value_counts(), fill_value=0)
     database.close()
     # Handle disabled apps and apps with less than min_samples_per_app samples
     if len(train_data_params.disabled_apps) > 0:
         log.info(f"Disabled applications in dataset config: {sorted(train_data_params.disabled_apps)}")
     disabled_apps_ids = [inverted_tables_app_enum[app] for app in train_data_params.disabled_apps]
     min_samples_apps_ids = set(app_counts[app_counts<train_data_params.min_train_samples_per_app].index.tolist())
     if len(min_samples_apps_ids) > 0:
@@ -198,16 +204,17 @@
         elif train_data_params.min_train_samples_check == MinTrainSamplesCheck.DISABLE_APPS:
             log.info(f"Found applications with less than {train_data_params.min_train_samples_per_app} train samples: {min_samples_apps_names}. " +
                        "Disabling these applications")
             disabled_apps_ids.extend(min_samples_apps_ids)
     # Base indices are indices of samples that are not disabled and have enough samples
     base_indices = {}
     for i, table_path in enumerate(train_data_params.train_tables_paths):
-        base_indices[i] = np.nonzero(np.isin(all_app_labels[i], disabled_apps_ids, invert=True))[0]
-    base_labels = {table_id: arr[base_indices[table_id]] for table_id, arr in all_app_labels.items()}
+        base_indices[i] = np.nonzero(np.isin(all_labels[i], disabled_apps_ids, invert=True))[0]
+    base_labels = {table_id: arr[base_indices[table_id]] for table_id, arr in all_labels.items()}
+    base_sni_domains = {table_id: arr[base_indices[table_id]] for table_id, arr in all_sni_domains.items()}
     # Apps selection
     if train_data_params.apps_selection != AppSelection.FIXED:
         app_counts = app_counts[[app for app in app_counts.index.tolist() if app not in disabled_apps_ids]]
         app_counts.index = app_counts.index.map(tables_app_enum)
         app_counts = app_counts.sort_values(ascending=False).astype("int64")
         sorted_apps = app_counts.index.to_list()
         if train_data_params.apps_selection == AppSelection.ALL_KNOWN:
@@ -226,34 +233,46 @@
         known_apps = train_data_params.apps_selection_fixed_known
         unknown_apps = train_data_params.apps_selection_fixed_unknown
     known_apps = sorted(known_apps)
     unknown_apps = sorted(unknown_apps)
     known_apps_ids = [inverted_tables_app_enum[app] for app in known_apps]
     unknown_apps_ids = [inverted_tables_app_enum[app] for app in unknown_apps]
 
-    train_known_indices, train_unknown_indices = convert_dict_indices(base_indices=base_indices, base_labels=base_labels, known_apps_ids=known_apps_ids, unknown_apps_ids=unknown_apps_ids)
+    train_known_indices, train_unknown_indices = convert_dict_indices(base_indices=base_indices,
+                                                                      base_labels=base_labels,
+                                                                      base_sni_domains=base_sni_domains,
+                                                                      known_apps_ids=known_apps_ids,
+                                                                      unknown_apps_ids=unknown_apps_ids)
     rng.shuffle(train_known_indices)
     rng.shuffle(train_unknown_indices)
-    log.info(f"Processing indices took {time.time() - start_time:.2f} seconds"); start_time = time.time()
     return train_known_indices, train_unknown_indices, known_apps, unknown_apps
 
-def init_test_indices(test_data_params: TestDataParams, database_path: str, tables_app_enum: dict[int, str], rng: np.random.RandomState) -> tuple[np.ndarray, np.ndarray]:
+def init_test_indices(test_data_params: TestDataParams, database_path: str, tables_app_enum: dict[int, str], sni_column: Optional[str], rng: np.random.RandomState) -> tuple[np.ndarray, np.ndarray]:
     database, test_tables = load_database(database_path, tables_paths=test_data_params.test_tables_paths)
     inverted_tables_app_enum = {v: k for k, v in tables_app_enum.items()}
     base_labels = {}
+    base_sni_domains = {}
     base_indices = {}
     start_time = time.time()
     for i, table_path in enumerate(test_data_params.test_tables_paths):
         base_labels[i] = test_tables[i].read(field=APP_COLUMN)
-        log.info(f"Reading app column for table {table_path} took {time.time() - start_time:.2f} seconds"); start_time = time.time()
+        if sni_column is not None:
+            base_sni_domains[i] = test_tables[i].read(field=sni_column)
+        else:
+            base_sni_domains[i] = np.full_like(base_labels[i], "", dtype="U1")
+        log.info(f"Reading app and SNI columns for table {table_path} took {time.time() - start_time:.2f} seconds"); start_time = time.time()
         base_indices[i] = np.arange(len(test_tables[i]))
     database.close()
     known_apps_ids = [inverted_tables_app_enum[app] for app in test_data_params.known_apps]
     unknown_apps_ids = [inverted_tables_app_enum[app] for app in test_data_params.unknown_apps]
-    test_known_indices, test_unknown_indices = convert_dict_indices(base_indices=base_indices, base_labels=base_labels, known_apps_ids=known_apps_ids, unknown_apps_ids=unknown_apps_ids)
+    test_known_indices, test_unknown_indices = convert_dict_indices(base_indices=base_indices,
+                                                                    base_labels=base_labels,
+                                                                    base_sni_domains=base_sni_domains,
+                                                                    known_apps_ids=known_apps_ids,
+                                                                    unknown_apps_ids=unknown_apps_ids)
     rng.shuffle(test_known_indices)
     rng.shuffle(test_unknown_indices)
     log.info(f"Processing indices took {time.time() - start_time:.2f} seconds"); start_time = time.time()
     return test_known_indices, test_unknown_indices
 
 def load_database(database_path: str, tables_paths: Optional[list[str]] = None, mode: str = "r") -> tuple[tb.File, dict[int, Any]]: # dict[int, tb.Table]
     database = tb.open_file(database_path, mode=mode)
@@ -267,32 +286,36 @@
         raise e
     return database, tables
 
 def list_all_tables(database_path: str) -> list[str]:
     with tb.open_file(database_path, mode="r") as database:
         return list(map(lambda x: x._v_pathname, iter(database.get_node(f"/flows"))))
 
-def convert_dict_indices(base_indices: dict[int, np.ndarray], base_labels: dict[int, np.ndarray], known_apps_ids: list[int], unknown_apps_ids: list[int]) -> tuple[np.ndarray, np.ndarray]:
+def convert_dict_indices(base_indices: dict[int, np.ndarray], base_labels: dict[int, np.ndarray], base_sni_domains: dict[int, np.ndarray], known_apps_ids: list[int], unknown_apps_ids: list[int]) -> tuple[np.ndarray, np.ndarray]:
     is_known = {table_id: np.isin(table_arr, known_apps_ids) for table_id, table_arr in base_labels.items()}
     is_unknown = {table_id: np.isin(table_arr, unknown_apps_ids) for table_id, table_arr in base_labels.items()}
     known_indices_dict = {table_id: table_arr[is_known[table_id]] for table_id, table_arr in base_indices.items()}
     unknown_indices_dict = {table_id: table_arr[is_unknown[table_id]] for table_id, table_arr in base_indices.items()}
     known_labels_dict = {table_id: table_arr[is_known[table_id]] for table_id, table_arr in base_labels.items()}
     unknown_labels_dict = {table_id: table_arr[is_unknown[table_id]] for table_id, table_arr in base_labels.items()}
-    known_indices = np.column_stack((
+    known_sni_domains_dict = {table_id: table_arr[is_known[table_id]] for table_id, table_arr in base_sni_domains.items()}
+    unknown_sni_domains_dict = {table_id: table_arr[is_unknown[table_id]] for table_id, table_arr in base_sni_domains.items()}
+    known_indices = np.array(list(zip(
         np.concatenate([[table_id] * table_arr.sum() for table_id, table_arr in is_known.items()]),
         np.concatenate(list(known_indices_dict.values())),
-        np.concatenate(list(known_labels_dict.values()))))
-    unknown_indices = np.column_stack((
+        np.concatenate(list(known_labels_dict.values())),
+        np.concatenate(list(known_sni_domains_dict.values())))), dtype=INDICES_DTYPE)
+    unknown_indices = np.array(list(zip(
         np.concatenate([[table_id] * table_arr.sum() for table_id, table_arr in is_unknown.items()]),
         np.concatenate(list(unknown_indices_dict.values())),
-        np.concatenate(list(unknown_labels_dict.values()))))
+        np.concatenate(list(unknown_labels_dict.values())),
+        np.concatenate(list(unknown_sni_domains_dict.values())))), dtype=INDICES_DTYPE)
     return known_indices, unknown_indices
 
 def load_data_from_tables(tables, indices: np.ndarray, data_dtype: np.dtype) -> np.ndarray:
-    sorted_indices = indices[indices[:, INDICES_TABLE_POS].argsort(kind="stable")]
-    unique_tables, split_bounderies = np.unique(sorted_indices[:, INDICES_TABLE_POS], return_index=True)
+    sorted_indices = indices[indices[INDICES_TABLE_FIELD].argsort(kind="stable")]
+    unique_tables, split_bounderies = np.unique(sorted_indices[INDICES_TABLE_FIELD], return_index=True)
     indices_per_table = np.split(sorted_indices, split_bounderies[1:])
     data = np.zeros(len(indices), dtype=data_dtype)
     for table_id, table_indices in zip(unique_tables, indices_per_table):
-        data[np.where(indices[:, INDICES_TABLE_POS] == table_id)[0]] = tables[table_id].read_coordinates(table_indices[:, INDICES_INDEX_POS])
+        data[np.where(indices[INDICES_TABLE_FIELD] == table_id)[0]] = tables[table_id].read_coordinates(table_indices[INDICES_INDEX_FIELD])
     return data
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/utils/class_info.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/utils/class_info.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/utils/download.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/utils/download.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/utils/fileutils.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo/utils/random.py` & `cesnet_datazoo-0.1.4/cesnet_datazoo/utils/random.py`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/PKG-INFO` & `cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-datazoo
-Version: 0.1.3
+Version: 0.1.4
 Summary: A toolkit for large network traffic datasets
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-datazoo
 Project-URL: Documentation, https://cesnet.github.io/cesnet-datazoo/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-datazoo/issues
```

### Comparing `cesnet-datazoo-0.1.3/cesnet_datazoo.egg-info/SOURCES.txt` & `cesnet_datazoo-0.1.4/cesnet_datazoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cesnet-datazoo-0.1.3/pyproject.toml` & `cesnet_datazoo-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-datazoo"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

