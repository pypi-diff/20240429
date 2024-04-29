# Comparing `tmp/novum_api_client-1.1.1.tar.gz` & `tmp/novum_api_client-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novum_api_client-1.1.1.tar", max compression
+gzip compressed data, was "novum_api_client-2.0.0.tar", max compression
```

## Comparing `novum_api_client-1.1.1.tar` & `novum_api_client-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2023-07-05 06:53:04.093748 novum_api_client-1.1.1/LICENSE
--rw-r--r--   0        0        0      737 2024-04-11 08:34:58.578504 novum_api_client-1.1.1/README.md
--rw-r--r--   0        0        0        0 2024-01-02 08:51:00.098131 novum_api_client-1.1.1/novum_api_client/__init__.py
--rw-r--r--   0        0        0    12736 2024-04-11 08:16:47.635780 novum_api_client-1.1.1/novum_api_client/api_type.py
--rw-r--r--   0        0        0    10916 2024-04-11 08:16:44.323742 novum_api_client-1.1.1/novum_api_client/base_client.py
--rw-r--r--   0        0        0    25382 2024-04-11 08:16:47.635780 novum_api_client-1.1.1/novum_api_client/client.py
--rw-r--r--   0        0        0        0 2024-01-02 08:51:00.102131 novum_api_client-1.1.1/novum_api_client/tests/__init__.py
--rw-r--r--   0        0        0    10245 2024-04-11 08:16:44.323742 novum_api_client-1.1.1/novum_api_client/tests/test_api_base.py
--rw-r--r--   0        0        0    25868 2024-04-11 08:16:47.635780 novum_api_client-1.1.1/novum_api_client/tests/test_api_public.py
--rw-r--r--   0        0        0      537 2024-04-11 08:45:51.268680 novum_api_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 novum_api_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-05 06:53:04.093748 novum_api_client-2.0.0/LICENSE
+-rw-r--r--   0        0        0      958 2024-04-29 14:48:00.934082 novum_api_client-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-01-02 08:51:00.098131 novum_api_client-2.0.0/novum_api_client/__init__.py
+-rw-r--r--   0        0        0    16121 2024-04-29 14:48:00.934082 novum_api_client-2.0.0/novum_api_client/api_type.py
+-rw-r--r--   0        0        0    11062 2024-04-29 14:48:00.934082 novum_api_client-2.0.0/novum_api_client/base_client.py
+-rw-r--r--   0        0        0    29588 2024-04-29 14:48:00.938082 novum_api_client-2.0.0/novum_api_client/client.py
+-rw-r--r--   0        0        0        0 2024-01-02 08:51:00.102131 novum_api_client-2.0.0/novum_api_client/tests/__init__.py
+-rw-r--r--   0        0        0    10832 2024-04-29 14:48:00.938082 novum_api_client-2.0.0/novum_api_client/tests/test_api_base.py
+-rw-r--r--   0        0        0    33112 2024-04-29 14:48:00.938082 novum_api_client-2.0.0/novum_api_client/tests/test_api_public.py
+-rw-r--r--   0        0        0      598 2024-04-29 14:48:00.938082 novum_api_client-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 novum_api_client-2.0.0/PKG-INFO
```

### Comparing `novum_api_client-1.1.1/LICENSE` & `novum_api_client-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `novum_api_client-1.1.1/README.md` & `novum_api_client-2.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -11,30 +11,36 @@
 Use pip to install:
 
 ```shell
 pip install novum_api_client
 ```
 
 
-
 # Release Notes
 
-## Version 1.1.1
-- Release Date: 2024-04-11
+## Version 2.0.0
+- Release Date: 2024-04-12
 
 ### Enhancements
-- Add new functions (get_user_documents and get_user_document_by_id).
-- Force typing for Reports.
-
+- Added dataclass_json to easy the types.
+- Rename types.
+- Added Docstring.
+- Rename functions "get_capacity_measurement" and "get_capacity_measurement_count".
+- API Client available for Python > 3.8.1
 
 
 # Changelog
 
+## [1.1.1] - 2024-04-11
+- Added new functions (get_user_documents and get_user_document_by_id).
+- Forced typing for Reports.
+
+
 ## [1.0.1] - 2023-12-12
 - Prettier added
 - Most of the function have "fields" as an argument.
-- Reports are now available in our library. 
-- Add Error/Exception messages.
+- Made Reports Section available. 
+- Added Error/Exception messages.
 
 
 ## [1.0.0] - 2023-12-12
-- First release of the library.
+- First release of the library.
```

### Comparing `novum_api_client-1.1.1/novum_api_client/base_client.py` & `novum_api_client-2.0.0/novum_api_client/base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # pylint: disable=C0103
-# pylint: disable=C0115
-# pylint: disable=C0116
 # flake8: noqa
 
 from dataclasses import asdict, dataclass
 import json
 import time
 import base64
 import hashlib
@@ -16,67 +14,77 @@
 from .api_type import TChargeTypes, TUser, TUserEssentials
 
 TOKEN_REFRESH_INTERVAL_SCALE = 0.9
 PRODUCTION_API_HOST: str = "https://novum-batteries.com"
 
 
 class DateTimeEncoder(json.JSONEncoder):
+    "DateTimeEncoder"
+
     def default(self, o):
         if isinstance(o, datetime):
             return o.isoformat() + "Z"
         if isinstance(o, TChargeTypes):
             return o.value
         return super().default(o)
 
 
 class NovumAPIError(Exception):
+    "NovumAPIError class"
+
     def __init__(self, message: str, status_code: int):
         self.message = message
         self.status_code = status_code
 
         super().__init__(message)
 
 
 def get_sha_256(to_hash: str) -> str:
+    "get hash"
     to_hash_bytes = to_hash.encode("utf-8")
     sha256_hash = hashlib.sha256(to_hash_bytes)
     return sha256_hash.hexdigest()
 
 
 def user_name(user: TUserEssentials) -> str:
+    "return user name"
     if user.profile is not None and user.profile.name is not None:
         return str(user.profile.name)
-    else:
-        raise ValueError("No user defined.")
+    raise ValueError("No user defined.")
 
 
 def full_name(user: TUser) -> str:
+    "return name"
     if (
         user.profile is not None
         and user.profile.first_name is not None
         and user.profile.family_name is not None
     ):
-        return str(user.profile.first_name) + " " + str(user.profile.family_name)
-    else:
-        raise ValueError("No user name defined.")
+        name = str(user.profile.first_name)
+        surname = str(user.profile.family_name)
+        name_and_surname = name + " " + surname
+        return name_and_surname
+    raise ValueError("No user name defined.")
 
 
 def parse_jwt(token: str) -> dict:
+    "parse token"
     base64_input = token.split(".")[1]
     base64_bytes = base64_input.encode("utf-8")
-    # Replace '-' with '+' and '_' with '/' as base64url is different than base64
+    # Replace '-' with '+' and '_' with '/' as base64url
     base64_bytes += b"=" * (4 - len(base64_bytes) % 4)
     base64_string = base64_bytes.decode("utf-8").replace("-", "+").replace("_", "/")
     json_payload = unquote(base64.b64decode(base64_string).decode("utf-8"))
     return json.loads(json_payload)
 
 
 @dataclass
 class BaseAPIClient:
-    user: TUser | None = None
+    "BaseAPIClient class"
+    user: Optional[TUser] = None
     host: str = PRODUCTION_API_HOST
     refresh_token_warning: bool = True
     refresh_interval_scale: float = TOKEN_REFRESH_INTERVAL_SCALE
     _relogin_timer_handle = None
     _authenticated: bool = False
 
     def __post_init__(self):
@@ -90,14 +98,15 @@
                 "Authorization": "Bearer " + self.user.jwt,
             }
         else:
             self.headers = None
 
     @classmethod
     def from_window_location(cls, origin):
+        "frontend window"
         return cls(origin)
 
     def _clear_user(self):
         self.user = None
         self._remove_relogin_timer_handle()
 
     def _remove_relogin_timer_handle(self):
@@ -203,16 +212,15 @@
             headers=headers,
             params=params_json,
             timeout=timeout,
         )
 
         if response.status_code == requests.codes.get("ok"):
             return response.json()
-        else:
-            raise NovumAPIError(response.text, response.status_code)
+        raise NovumAPIError(response.text, response.status_code)
 
     def _post_file(self, path: str, file: str):
         options = {"upload_file": open(file)}  # investigate how to close that
         return self._post_by_path(path, options=options)
 
     def _post_json(
         self,
@@ -242,17 +250,15 @@
             params=params_json,
             data=data,
             timeout=timeout,
         )
 
         if response.status_code == requests.codes.get("ok"):
             return response.json()
-
-        else:
-            raise NovumAPIError(response.text, response.status_code)
+        raise NovumAPIError(response.text, response.status_code)
 
     def _put_json(
         self,
         url: str,
         input_data: Any,
         filter_json: Optional[dict] = None,
         option: Optional[dict] = None,
@@ -275,16 +281,15 @@
             params=params_json,
             data=data_json,
             timeout=timeout,
         )
 
         if response.status_code == requests.codes.get("ok"):
             return response.json()
-        else:
-            raise NovumAPIError(response.text, response.status_code)
+        raise NovumAPIError(response.text, response.status_code)
 
     def _delete_json(
         self,
         url: str,
         filter_json: Optional[dict] = None,
         option: Optional[dict] = None,
         timeout: float = 4.0,
@@ -302,16 +307,15 @@
             url=full_url,
             headers=headers,
             params=params_json,
             timeout=timeout,
         )
         if response.status_code <= 204:
             return response
-        else:
-            raise NovumAPIError(response.text, response.status_code)
+        raise NovumAPIError(response.text, response.status_code)
 
     def _get_text(
         self,
         path: str,
         headers: Optional[dict] = None,
     ) -> dict:
         if headers is not None:
@@ -328,11 +332,13 @@
         content = response["content"]
         return [int(i) for i in content]
 
     def _host(self) -> str:
         return self.host
 
     def authenticated(self) -> bool:
+        "authenticated"
         return self._authenticated
 
     def set_new_endpoint(self, new_end_point: str):
+        "set_new_endpoint"
         self.host = new_end_point
```

### Comparing `novum_api_client-1.1.1/novum_api_client/client.py` & `novum_api_client-2.0.0/novum_api_client/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,71 @@
-# pylint: disable=C0115
-# pylint: disable=C0116
+# pylint: disable=C0103
 # flake8: noqa
 
 import json
 from typing import Optional, List
-import requests
 from dataclasses import dataclass
+import warnings
+import requests
 from .base_client import BaseAPIClient, NovumAPIError
 from .api_type import (
     TUser,
     TReport,
-    TDataset,
-    TBattery,
-    TBatteryType,
+    TVersion,
     TUserDocument,
+    TBatteryReading,
+    TDatasetReading,
+    TDeviceMeasurement,
     TReportEssentials,
+    TAPIInfoEssentials,
     TDatasetEssentials,
     TBatteryEssentials,
-    TAPIInfoEssentials,
-    TVersionEssentials,
-    TDeviceMeasurement,
-    TCapacityMeasurement,
+    TBatteryTypeReading,
     TBatteryTypeEssentials,
     TDeviceMeasurementsResult,
+    TCapacityMeasurementReading,
     TCapacityMeasurementEssentials,
 )
 
 PRODUCTION_API_HOST: str = "https://novum-batteries.com"
 
 
 @dataclass
 class NovumAPIClient(BaseAPIClient):
+    """NovumAPIClient class"""
+
     def __init__(self, user=None, host=PRODUCTION_API_HOST):
         super().__init__(user, host)
 
     # ********************************************************
     # Section for the Service Center info
     # ********************************************************
 
     def ping(self) -> dict:
+        """Ping API."""
         return self._get_json("/api/batman/v1/")
 
     def get_info(self) -> TAPIInfoEssentials:
+        """Get info."""
         info = self._get_json("/api/batman/v1/info")
         return TAPIInfoEssentials(**info)
 
-    def get_version(self) -> TVersionEssentials:
+    def get_version(self) -> TVersion:
+        """Check version."""
         version = self._get_json("/api/batman/v1/version")
-        return TVersionEssentials(**version)
+        return TVersion(**version)
 
     # ********************************************************
     # Section for the users
     # ********************************************************
 
     def login(
         self, email: str, password: str, store_user=True, timeout: float = 4
-    ) -> TUser | None:
+    ) -> Optional[TUser]:
+        """Login."""
         header = {"authorization": "auth", "content-type": "application/json"}
         payload = {"username": email, "password": password}
         response = requests.post(
             self.host + "/api/batman/v1/login",
             data=json.dumps(payload),
             headers=header,
             timeout=timeout,
@@ -74,264 +80,293 @@
                         "Content-Type": "application/json",
                         "Authorization": "Bearer " + str(self.user.jwt),
                     }
                 )
 
             return self.user
 
-        else:
-            raise NovumAPIError(response.text, response.status_code)
+        raise NovumAPIError(response.text, response.status_code)
 
     def logout(self):
+        """Log out."""
         return self._get_json("/api/batman/v1/logout")
 
     def check_current_user_still_authenticated(self) -> dict:
+        """Check authentication."""
+
         return self._get_json("/api/batman/v1/check_token")
 
     # ********************************************************
     # Section for the Battery Types
     # ********************************************************
 
     def get_battery_types(
         self,
         filter_types: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TBatteryType]:
+    ) -> List[TBatteryTypeReading]:
+        """Get battery types."""
         battery_types_list = self._get_json(
             "/api/batman/v1/batteryTypes",
             filter_json=filter_types,
             option=option,
             fields=fields,
             timeout=timeout,
         )
 
         battery_types = [
-            TBatteryType(**battery_type) for battery_type in battery_types_list
+            TBatteryTypeReading(**battery_type) for battery_type in battery_types_list
         ]
 
         return battery_types
 
     def get_battery_types_count(
         self,
         filter_types: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> int:
+    ) -> dict:
+        """Get amount of battery types."""
         return self._get_json(
             "/api/batman/v1/batteryTypes/count",
             filter_json=filter_types,
             option=option,
             fields=fields,
             timeout=timeout,
         )  # type: ignore
 
     def get_battery_types_by_id(
         self, battery_type_id: str, timeout: float = 4.0
-    ) -> TBatteryType:
+    ) -> TBatteryTypeReading:
+        """Get battery type by id."""
         battery_type = self._get_json(
             f"/api/batman/v1/batteryTypes/{battery_type_id}", timeout=timeout
         )
-        return TBatteryType(**battery_type)
+        return TBatteryTypeReading(**battery_type)
 
     def remove_battery_types_by_id(self, battery_type_id: str, timeout: float = 4.0):
+        """Delete battery type by id."""
         self._delete_json(
             f"/api/batman/v1/batteryTypes/{battery_type_id}", timeout=timeout
         )
         return "The battery type was removed."
 
     def create_battery_type(
         self,
         battery_type: TBatteryTypeEssentials,
         timeout: float = 4.0,
-    ) -> TBatteryType:
+    ) -> TBatteryTypeEssentials:
+        """Create battery type."""
         created_battery_type = self._post_json(
             "/api/batman/v1/batteryTypes", input_data=battery_type, timeout=timeout
         )
-        return TBatteryType(**created_battery_type)
+        return TBatteryTypeEssentials(**created_battery_type)
 
     def update_battery_type_by_id(
         self,
         battery_type_id: str,
-        battery_type_update: TBatteryTypeEssentials,
+        battery_type_update: TBatteryTypeReading,
         timeout: float = 4.0,
-    ) -> TBatteryType:
+    ) -> TBatteryTypeEssentials:
+        """Update battery type by id."""
         updated_battery_type = self._put_json(
             f"/api/batman/v1/batteryTypes/{battery_type_id}",
             input_data=battery_type_update,
             timeout=timeout,
         )
-        return TBatteryType(**updated_battery_type)
+        return TBatteryTypeEssentials(**updated_battery_type)
 
     # ********************************************************
     # Section for the Datasets
     # ********************************************************
 
     def dataset_exists_on_remote(self, dataset_id: str, timeout: float = 4.0) -> bool:
+        """Check remote data."""
         response = self._get_json(
             f"/api/batman/v1/datasets/{dataset_id}", timeout=timeout
         )
         try:
             if len(response["measured"]["measurement_cycles"]) != 0:
                 return True
             else:
                 return False
         except KeyError:
             return False
 
     def create_dataset(
         self, dataset: TDatasetEssentials, timeout: float = 4.0
-    ) -> TDataset:
+    ) -> TDatasetEssentials:
+        """Create EIS measurement."""
         created_dataset = self._post_json(
             "/api/batman/v1/datasets", input_data=dataset, timeout=timeout
         )
-        return TDataset(**created_dataset)
+        return TDatasetEssentials(**created_dataset)
 
-    def get_dataset_by_id(self, dataset_id: str, timeout: float = 4.0) -> TDataset:
+    def get_dataset_by_id(
+        self, dataset_id: str, timeout: float = 4.0
+    ) -> TDatasetReading:
+        """Get EIS measurement by id."""
         dataset = self._get_json(
             f"/api/batman/v1/datasets/{dataset_id}", timeout=timeout
         )
-        return TDataset(**dataset)
+        return TDatasetReading(**dataset)
 
     def get_datasets(
         self,
         filter_datasets: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TDataset]:
+    ) -> List[TDatasetReading]:
+        """Get EIS measurements."""
         dataset_list = self._get_json(
             "/api/batman/v1/datasets",
             filter_json=filter_datasets,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        datasets = [TDataset(**dataset) for dataset in dataset_list]
+        datasets = [TDatasetReading(**dataset) for dataset in dataset_list]
 
         return datasets
 
     def get_datasets_count(
         self,
         filter_datasets: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
     ) -> int:
+        """Get amount of EIS measurements."""
         return self._get_json(
             "/api/batman/v1/datasets/count",
             filter_json=filter_datasets,
             option=option,
             fields=fields,
             timeout=timeout,
         )  # type: ignore
 
     def get_datasets_count_by_battery(
         self,
-        battery: TBattery,
+        battery: TBatteryReading,
         filter_datasets: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
     ) -> int:
+        """Get amount of EIS measurements by battery."""
         filter_with_id = {"meta.battery._id": battery.id}
         if filter_datasets is not None:
             filter_with_id.update(filter_datasets)
         response = self._get_json(
             "/api/batman/v1/datasets/count",
             filter_json=filter_with_id,
             option=option,
             fields=fields,
             timeout=timeout,
         )
         return response  # type: ignore
 
     def update_dataset_by_id(
-        self, dataset_id: str, dataset: TDatasetEssentials, timeout: float = 4.0
-    ) -> TDataset:
+        self, dataset_id: str, dataset: TDatasetReading, timeout: float = 4.0
+    ) -> TDatasetEssentials:
+        """Update EIS measurement by id."""
         updated_dataset = self._put_json(
             f"/api/batman/v1/datasets/{dataset_id}",
             input_data=dataset,
             timeout=timeout,
         )
-        return TDataset(**updated_dataset)
+        return TDatasetEssentials(**updated_dataset)
 
     def remove_dataset_by_id(self, dataset_id: str, timeout: float = 4.0):
+        """Delete EIS measurement by id."""
         self._delete_json(f"/api/batman/v1/datasets/{dataset_id}", timeout=timeout)
         return "The data set was removed."
 
     # ********************************************************
     # Section for the Battery
     # ********************************************************
 
     def create_battery(
         self, battery: TBatteryEssentials, timeout: float = 4.0
-    ) -> TBattery:
+    ) -> TBatteryEssentials:
+        """Create a battery."""
         created_battery = self._post_json(
             "/api/batman/v1/batteries", input_data=battery, timeout=timeout
         )
-        return TBattery(**created_battery)
+        return TBatteryEssentials(**created_battery)
 
-    def get_battery_by_id(self, battery_id: str, timeout: float = 4.0) -> TBattery:
+    def get_battery_by_id(
+        self, battery_id: str, timeout: float = 4.0
+    ) -> TBatteryReading:
+        """Get battery by id."""
         battery = self._get_json(
             f"/api/batman/v1/batteries/{battery_id}", timeout=timeout
         )
 
-        return TBattery(**battery)
+        return TBatteryReading(**battery)
 
-    def update_battery(self, battery: TBattery, timeout: float = 4.0) -> TBattery:
+    def update_battery(
+        self, battery: TBatteryReading, timeout: float = 4.0
+    ) -> TBatteryEssentials:
+        """Update a battery."""
         updated_battery = self._put_json(
             f"/api/batman/v1/batteries/{battery.id}",
             input_data=battery,
             timeout=timeout,
         )
 
-        return TBattery(**updated_battery)
+        return TBatteryEssentials(**updated_battery)
 
     def update_battery_by_id(
-        self, battery_id: str, battery_update: TBatteryEssentials, timeout: float = 4.0
-    ) -> TBattery:
+        self, battery_id: str, battery_update: TBatteryReading, timeout: float = 4.0
+    ) -> TBatteryEssentials:
+        """Update a battery by id."""
         updated_battery = self._put_json(
             f"/api/batman/v1/batteries/{battery_id}",
             input_data=battery_update,
             timeout=timeout,
         )
-        return TBattery(**updated_battery)
+        return TBatteryEssentials(**updated_battery)
 
     def remove_battery_by_id(self, battery_id: str, timeout: float = 4.0) -> str:
+        """Delete a battery by id."""
         self._delete_json(f"/api/batman/v1/batteries/{battery_id}", timeout=timeout)
         return "The battery was removed."
 
     def get_batteries(
         self,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TBattery]:
+    ) -> List[TBatteryReading]:
+        """Get batteries."""
         battery_list = self._get_json(
             "/api/batman/v1/batteries",
             filter_json=filter_batteries,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        batteries = [TBattery(**battery) for battery in battery_list]
+        batteries = [TBatteryReading(**battery) for battery in battery_list]
 
         return batteries
 
     def get_batteries_count(
         self,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
     ) -> int:
+        """Get amount of batteries."""
         return self._get_json(
             "/api/batman/v1/batteries/count",
             filter_json=filter_batteries,
             option=option,
             fields=fields,
             timeout=timeout,
         )  # type: ignore
@@ -339,37 +374,39 @@
     def get_children_of_battery_by_id(
         self,
         parent_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TBattery]:
+    ) -> List[TBatteryReading]:
+        """Get children of a battery using the id."""
         filter_with_id = {"tree.parent": parent_battery_id}
         if filter_batteries is not None:
             filter_with_id.update(filter_batteries)
         battery_list = self._get_json(
             "/api/batman/v1/batteries",
             filter_json=filter_with_id,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        batteries = [TBattery(**battery) for battery in battery_list]
+        batteries = [TBatteryReading(**battery) for battery in battery_list]
 
         return batteries
 
     def get_children_of_battery_by_id_count(
         self,
         parent_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
     ) -> int:
+        """Get amount of children by battery id."""
         filter_with_id = {"tree.parent": parent_battery_id}
         if filter_batteries is not None:
             filter_with_id.update(filter_batteries)
         response = self._get_json(
             "/api/batman/v1/batteries/count",
             filter_json=filter_with_id,
             option=option,
@@ -381,226 +418,283 @@
     def get_leaves_of_battery_by_id(
         self,
         ancestor_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TBattery]:
+    ) -> List[TBatteryReading]:
+        """Get all leaves of a tree of battery."""
         filter_with_id = {"tree.is_leaf": True, "tree.ancestors": ancestor_battery_id}
         if filter_batteries is not None:
             filter_with_id.update(filter_batteries)
         battery_list = self._get_json(
             "/api/batman/v1/batteries",
             filter_json=filter_with_id,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        batteries = [TBattery(**battery) for battery in battery_list]
+        batteries = [TBatteryReading(**battery) for battery in battery_list]
         return batteries
 
     def get_leaves_of_battery_by_id_count(
         self,
         ancestor_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TBattery]:
+    ) -> List[TBatteryReading]:
+        """Get amount of leaves of a level top(accordingly on a tree) battery."""
         filter_with_id = {"tree.is_leaf": True, "tree.ancestors": ancestor_battery_id}
         if filter_batteries is not None:
             filter_with_id.update(filter_batteries)
         battery_list = self._get_json(
             "/api/batman/v1/batteries/count",
             filter_json=filter_with_id,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        batteries = [TBattery(**battery) for battery in battery_list]
+        batteries = [TBatteryReading(**battery) for battery in battery_list]
         return batteries
 
     def get_descendants_of_battery_by_id(
         self,
         ancestor_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TBattery]:
+    ) -> List[TBatteryReading]:
+        """Get all descendants on the tree by battery id."""
         filter_with_id = {"tree.ancestors": ancestor_battery_id}
         if filter_batteries is not None:
             filter_with_id.update(filter_batteries)
         battery_list = self._get_json(
             "/api/batman/v1/batteries",
             filter_json=filter_with_id,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        batteries = [TBattery(**battery) for battery in battery_list]
+        batteries = [TBatteryReading(**battery) for battery in battery_list]
         return batteries
 
     def get_descendants_of_battery_by_id_count(
         self,
         ancestor_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TBattery]:
+    ) -> List[TBatteryReading]:
+        """Get amount of descendants on the tree by battery id."""
         filter_with_id = {"tree.ancestors": ancestor_battery_id}
         if filter_batteries is not None:
             filter_with_id.update(filter_batteries)
         battery_list = self._get_json(
             "/api/batman/v1/batteries/count",
             filter_json=filter_with_id,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        batteries = [TBattery(**battery) for battery in battery_list]
+        batteries = [TBatteryReading(**battery) for battery in battery_list]
         return batteries
 
     # ********************************************************
     # Section for the CapacityMeasurement
     # ********************************************************
 
     def create_capacity_measurement(
         self, capacity_measurement: TCapacityMeasurementEssentials, timeout: float = 4.0
-    ) -> TCapacityMeasurement:
+    ) -> TCapacityMeasurementEssentials:
+        """Create a capacity measurement."""
         response = self._post_json(
             "/api/batman/v1/capacityMeasurements",
             input_data=capacity_measurement,
             timeout=timeout,
         )
 
-        return TCapacityMeasurement(**response)
+        return TCapacityMeasurementEssentials(**response)
 
     def update_capacity_measurement_by_id(
         self,
         capacity_measurement_id: str,
-        capacity_measurement: TCapacityMeasurementEssentials,
+        capacity_measurement: TCapacityMeasurementReading,
         timeout: float = 4.0,
-    ) -> TCapacityMeasurement:
+    ) -> TCapacityMeasurementEssentials:
+        """Update a capacity measurement by id."""
         updated_capacity_measurement = self._put_json(
             f"/api/batman/v1/capacityMeasurements/{capacity_measurement_id}",
             input_data=capacity_measurement,
             timeout=timeout,
         )
-        return TCapacityMeasurement(**updated_capacity_measurement)
+        return TCapacityMeasurementEssentials(**updated_capacity_measurement)
 
     def remove_capacity_measurement_by_id(
         self, capacity_measurement_id: str, timeout: float = 4.0
     ):
+        """Delete capacity measurement by id."""
         self._delete_json(
             f"/api/batman/v1/capacityMeasurements/{capacity_measurement_id}",
             timeout=timeout,
         )
         return "Capacity measurement was removed."
 
     def get_capacity_measurement(
         self,
         filter_measurements: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> List[TCapacityMeasurement]:
+    ) -> List[TCapacityMeasurementReading]:
+        """Get capacity measurements (deprecated)."""
+        warnings.warn(
+            "Function get_capacity_measurement is deprecated, use get_capacity_measurements instead.",
+            DeprecationWarning,
+        )
+
+        capacity_measurements = self.get_capacity_measurements(
+            filter_measurements=filter_measurements,
+            option=option,
+            fields=fields,
+            timeout=timeout,
+        )
+
+        return capacity_measurements
+
+    def get_capacity_measurements(
+        self,
+        filter_measurements: Optional[dict] = None,
+        option: Optional[dict] = None,
+        fields: Optional[dict] = None,
+        timeout: float = 4.0,
+    ) -> List[TCapacityMeasurementReading]:
+        """Get capacity measurements."""
         capacity_measurement_list = self._get_json(
             "/api/batman/v1/capacityMeasurements",
             filter_json=filter_measurements,
             option=option,
             fields=fields,
             timeout=timeout,
         )
 
         capacity_measurements = [
-            TCapacityMeasurement(**capacity_measurement)
-            for capacity_measurement in capacity_measurement_list
+            TCapacityMeasurementReading(**capa) for capa in capacity_measurement_list
         ]
 
         return capacity_measurements
 
     def get_capacity_measurement_count(
         self,
         filter_measurements: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
     ) -> int:
+        """Get amount of capacity measurements (deprecated)."""
+        warnings.warn(
+            "Function get_capacity_measurement_count is deprecated, use get_capacity_measurements_count instead.",
+            DeprecationWarning,
+        )
+        capacity_measurements_count = self.get_capacity_measurement_count(
+            filter_measurements=filter_measurements,
+            option=option,
+            fields=fields,
+            timeout=timeout,
+        )
+
+        return capacity_measurements_count
+
+    def get_capacity_measurements_count(
+        self,
+        filter_measurements: Optional[dict] = None,
+        option: Optional[dict] = None,
+        fields: Optional[dict] = None,
+        timeout: float = 4.0,
+    ) -> int:
+        """Get amount of capacity measurements."""
         response = self._get_json(
             "/api/batman/v1/capacityMeasurements/count",
             filter_json=filter_measurements,
             option=option,
             fields=fields,
             timeout=timeout,
         )
         return response  # type: ignore
 
     def get_capacity_measurement_by_id(
         self, capacity_measurement_id: str, timeout: float = 4.0
-    ) -> TCapacityMeasurement:
+    ) -> TCapacityMeasurementEssentials:
+        """Get capacity measurement by id."""
         capacity_measurement = self._get_json(
             f"/api/batman/v1/capacityMeasurements/{capacity_measurement_id}",
             timeout=timeout,
         )
-        return TCapacityMeasurement(**capacity_measurement)
+        return TCapacityMeasurementEssentials(**capacity_measurement)
 
     def get_capacity_measurements_count_by_battery(
         self, battery_id: str, timeout: float = 4.0
     ) -> int:
+        """Get amount of capacity measurement per battery using battery id."""
         filter_by_id = {"battery._id": battery_id}
         response = self._get_json(
             "/api/batman/v1/capacityMeasurements/count",
             filter_json=filter_by_id,
             timeout=timeout,
         )
         return response  # type: ignore
 
     def capacity_measurement_exists_on_remote(
         self, capacity_measurement_id: str, timeout: float = 4.0
     ) -> bool:
+        """Check capacity measurement on remote."""
         response = self._get_json(
             f"/api/batman/v1/capacityMeasurements/{capacity_measurement_id}",
             timeout=timeout,
         )
         return response["id"] == capacity_measurement_id
 
     # ********************************************************
     # Section for the Measurements
     # ********************************************************
 
     def get_latests_measurements(
         self, device_id: str, count: int = 1, timeout: float = 4.0
     ) -> TDeviceMeasurementsResult:
+        """Get latest live measurement."""
         measurements_list = self._get_json(
             f"/api/time-series/v1/devices/{device_id}/measurements/last/{count}",
             timeout=timeout,
         )
 
         return measurements_list  # type: ignore
 
     def write_device_measurements(
         self, device_measurements: List[TDeviceMeasurement], timeout: float = 4.0
     ) -> TDeviceMeasurementsResult:
+        """Write time series live measurement."""
         write_measurement = self._post_json(
             "/api/time-series/v1/measurements",
             input_data=device_measurements,
             timeout=timeout,
         )
         return write_measurement  # type: ignore
 
     def read_device_measurements(
         self,
         device_filter: Optional[dict],
         option=None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
     ) -> TDeviceMeasurementsResult:
+        """Get time series live measurement."""
         read_measurements = self._get_json(
             "/api/time-series/v1/measurements",
             filter_json=device_filter,
             option=option,
             fields=fields,
             timeout=timeout,
         )
@@ -609,45 +703,49 @@
     def read_device_measurements_by_id(
         self,
         battery_id,
         device_filter: Optional[dict],
         fields: Optional[dict] = None,
         timeout: float = 4.0,
     ) -> TDeviceMeasurementsResult:
+        """Get time series live measurement by battery id."""
         read_measurements_by_battery_id = self._get_json(
             f"/api/time-series/v1/measurements/{battery_id}",
             filter_json=device_filter,
             fields=fields,
             timeout=timeout,
         )
         return read_measurements_by_battery_id  # type: ignore
 
     # ********************************************************
     # Section for the Reports
     # ********************************************************
 
     def create_report(self, report: TReportEssentials, timeout: float = 4.0) -> TReport:
+        """Create report."""
         report_post = self._post_json("/api/batman/v1/reports", report, timeout=timeout)
         return TReport(**report_post)
 
     def update_report_by_id(
         self, report_id: str, report: TReportEssentials, timeout: float = 4
     ) -> TReport:
+        """Update report by id."""
         update_report = self._put_json(
             f"/api/batman/v1/reports/{report_id}", report, timeout=timeout
         )
         return TReport(**update_report)
 
     def get_reports(
         self,
         report_filter: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4,
     ) -> List[TReport]:
+        """Get reports."""
         report_list = self._get_json(
             "/api/batman/v1/reports",
             filter_json=report_filter,
             fields=fields,
             option=option,
             timeout=timeout,
         )
@@ -657,46 +755,50 @@
     def get_reports_count(
         self,
         report_filter: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4,
     ) -> int:
+        """Get amount of reports."""
         response = self._get_json(
             "/api/batman/v1/reports/count",
             report_filter,
             option=option,
             fields=fields,
             timeout=timeout,
         )
         return response  # type: ignore
 
     def get_reports_count_by_battery(
-        self, battery: TBattery, timeout: float = 4
+        self, battery: TBatteryReading, timeout: float = 4
     ) -> int:
+        """Get amount of reports by battery."""
         response = self._get_json(
             "/api/batman/v1/reports/count",
             filter_json={"origin_id": battery.id},
             timeout=timeout,
         )
 
         return response  # type: ignore
 
     def get_report_by_id(self, report_id: str, timeout: float = 4) -> TReport:
+        """Get reports by id."""
         report = self._get_json(f"/api/batman/v1/reports/{report_id}", timeout=timeout)
         return TReport(**report)
 
     def get_reports_by_origin_id(
         self,
         origin_id: str,
         report_filter: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4,
     ) -> List[TReport]:
+        """Get reports by origin id."""
         report_list = self._get_json(
             f"/api/batman/v1/reports/byOriginId/{origin_id}",
             report_filter,
             option=option,
             fields=fields,
             timeout=timeout,
         )
@@ -709,27 +811,29 @@
         self,
         origin_id: str,
         report_filter: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4,
     ) -> int:
+        """Get amount of reports by origin id."""
         reports_count = self._get_json(
             f"/api/batman/v1/reports/byOriginId/{origin_id}/count",
             report_filter,
             option,
             fields=fields,
             timeout=timeout,
         )
         return reports_count  # type: ignore
 
     def remove_report_by_id(
         self, report_id: str, report_filter=None, option=None, timeout: float = 4
     ):
-        response = self._delete_json(
+        """Delete reports by id."""
+        self._delete_json(
             f"/api/batman/v1/reports/{report_id}",
             filter_json=report_filter,
             option=option,
             timeout=timeout,
         )
         return "The report was removed."
 
@@ -740,23 +844,25 @@
     def get_user_documents(
         self,
         document_filter: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
     ) -> List[TUserDocument]:
+        """Gest user documents"""
         user_documents_list = self._get_json(
             "/api/batman/v1/userDocuments",
             filter_json=document_filter,
             option=option,
             fields=fields,
             timeout=timeout,
         )
 
         user_documents = [TUserDocument(**document) for document in user_documents_list]
 
         return user_documents
 
     def get_user_document_by_id(self, user_document_id: str) -> TUserDocument:
+        """Get user document by document id."""
         document = self._get_json(f"/api/batman/v1/userDocuments/{user_document_id}")
 
         return TUserDocument(**document)
```

### Comparing `novum_api_client-1.1.1/novum_api_client/tests/test_api_base.py` & `novum_api_client-2.0.0/novum_api_client/tests/test_api_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,109 +8,115 @@
 
 from ..api_type import TProfile, TUserEssentials, TUserSettings
 from ..base_client import user_name, get_sha_256, full_name, parse_jwt, BaseAPIClient
 
 PRODUCTION_API_HOST: str = "https://novum-batteries.com"
 
 
-@pytest.fixture
-def user_mage():
-    return TUserEssentials(
-        jwt="SuperSecret123!",
-        refresh_token="MagicToken123",
-        auth0_id="EnchantedWizard123",
-        meta_data={"user_type": "MysticalBeing"},
-        roles=["sorcerer", "enchanter"],
-        scope="arcane_magic",
-        stats=None,
-        permissions=["granted", "enchanted"],
-        profile=TProfile(
-            name="Gandalf the Grey",
-            first_name="Gandalf",
-            last_name="Grey",
-            given_name="The Enchanter",
-            email="wizard@fantasyrealm.com",
-            family_name="Grey",
-            email_verified=True,
-            picture="magical_staff.jpg",
-        ),
-        settings=TUserSettings(ServiceCenterSettings=None),
-    )
-
-
-def test_get_sha_256():
-    assert get_sha_256("hello world") == hashlib.sha256(b"hello world").hexdigest()
-    assert get_sha_256("test") == hashlib.sha256(b"test").hexdigest()
-
-
-def test_user_name(user_mage):
-    result = user_name(user_mage)
-    expected_name = "Gandalf the Grey"
-    assert result == expected_name
-
-
-def test_full_name(user_mage):
-    result = full_name(user_mage)
-    expected_result = "Gandalf Grey"
-    assert result == expected_result
+class TestBaseAPIClient:
+    # auxiliar functions
+    @pytest.fixture
+    def user_sample_mage(self):
+        """Fixture: sample of user."""
+        user_sample = TUserEssentials(
+            jwt="SuperSecret123!",
+            refresh_token="MagicToken123",
+            auth0_id="EnchantedWizard123",
+            meta_data={"user_type": "MysticalBeing"},
+            roles=["sorcerer", "enchanter"],
+            scope="arcane_magic",
+            stats=None,
+            permissions=["granted", "enchanted"],
+            profile=TProfile(
+                name="Gandalf the Grey",
+                first_name="Gandalf",
+                last_name="Grey",
+                given_name="The Enchanter",
+                email="wizard@fantasyrealm.com",
+                family_name="Grey",
+                email_verified=True,
+                picture="magical_staff.jpg",
+            ),
+            settings=TUserSettings(ServiceCenterSettings=None),
+        )
+        return user_sample
 
+    def test_get_sha_256(self):
+        """Check sha_256."""
+        assert get_sha_256("hello world") == hashlib.sha256(b"hello world").hexdigest()
+        assert get_sha_256("test") == hashlib.sha256(b"test").hexdigest()
+
+    def test_user_name(self, user_sample_mage):
+        """Check user name fetch."""
+        result = user_name(user_sample_mage)
+        expected_name = "Gandalf the Grey"
+        assert result == expected_name
+
+    def test_full_name(self, user_sample_mage):
+        """Check full name check."""
+        result = full_name(user_sample_mage)
+        expected_result = "Gandalf Grey"
+        assert result == expected_result
 
-def test_parse_jwt():
-    sample_token = "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Im9Ma1Ridm93cnFndXdoN3lPaUttTCJ9.eyJodHRwczovL25vdnVtLWJhdHRlcmllcy5jb20vcm9sZXMiOlsidXNlciIsImludm9pY2VDcmVhdG9yIiwibm92dW1FeHBlcnQiXSwiaHR0cHM6Ly9ub3Z1bS1iYXR0ZXJpZXMuY29tL3NldHRpbmdzIjp7ImludmVydEF4aXMiOnRydWUsInNlcnZpY2VDZW50ZXIiOnsic2hvd0FkdmFuY2VkT3B0aW9ucyI6dHJ1ZSwiaW52ZXJ0QXhpcyI6dHJ1ZSwiZmF2b3JpdGVCYXR0ZXJpZXNJZHMiOlsiOW94SHZjNnlOWld1VzNzRWsiLCIyRUdFTjd1TU40YWg4ckRGWiIsIkRUQUhIRFR1SkJEQ3ZRRlNKIiwiOVJBU0VIZHZxRW9odlBFU1oiLCJkenBEd3NoUEFHc2N5NkJHaCIsIkFjY3lxSGdvR25IU0F3ZTlHIiwiczdNU1g0ZjNIcWpDcHZ1TEoiLCI1YzdlYkJTekNXNFJuckYzNCIsIkhQZ0RLVFRUSjNEUUhGZ0FEIl0sImJhdHRlcnlUYWJsZUNvbHVtbnMiOlsibmFtZSIsInN0YXRlLnN0YXRlX29mX2NoYXJnZS52YWx1ZSIsInN0YXRlLnN0YXRlX29mX2hlYWx0aC52YWx1ZSIsIm1ldHJpY3Muc3RhdGVfb2ZfaGVhbHRoIiwiaW50ZXJuYWxfY2FwYWNpdHlfY291bnQiLCJpbnRlcm5hbF9kYXRhc2V0X2NvdW50IiwiY3JlYXRvcl9pZCIsImxpZmV0aW1lX2luZGljYXRvciIsImludGVybmFsX2FjdGlvbnMiXSwiZGFzaGJvYXJkVGFibGVDb2x1bW5zIjpbIm5hbWUiLCJiYXR0ZXJ5X3R5cGUubmFtZSIsInN0YXRlLnN0YXRlX29mX2NoYXJnZS52YWx1ZSIsInN0YXRlLnN0YXRlX29mX2hlYWx0aC52YWx1ZSIsImxpZmV0aW1lX2luZGljYXRvciIsImludGVybmFsX2FjdGlvbnMiXSwiZWlzRGF0YXNldFRhYmxlQ29sdW1ucyI6WyJpZCIsIm1ldGEuYmF0dGVyeS5uYW1lIiwiYW5hbHlzaXMuc3RhdGVfb2ZfY2hhcmdlIiwiYW5hbHlzaXMuc3RhdGVfb2ZfaGVhbHRoIiwiaW50ZXJuYWxfYWN0aW9ucyIsImFuYWx5c2lzLmdyYWRlIiwiY3JlYXRvcl9pZCIsImNvbnRleHRfaWQiLCJjcmVhdGVkX2F0Il0sImNhcGFjaXR5TWVhc3VyZW1lbnRUYWJsZUNvbHVtbnMiOlsiaWQiLCJiYXR0ZXJ5Lm5hbWUiLCJzdGF0ZV9vZl9oZWFsdGgiLCJjcmVhdGVkX2F0IiwiaW50ZXJuYWxfYWN0aW9ucyIsImdyYWRlIiwiY3JlYXRvcl9pZCIsImNvbnRleHRfaWQiLCJzdGFydF90aW1lIiwiZW5kX3RpbWUiXX19LCJnaXZlbl9uYW1lIjoiTGVvbmFyZG8iLCJmYW1pbHlfbmFtZSI6IkJpeiIsIm5pY2tuYW1lIjoibC5iaXoiLCJuYW1lIjoiTGVvIEJpeiIsInBpY3R1cmUiOiJodHRwczovL3MuZ3JhdmF0YXIuY29tL2F2YXRhci8yZTRiYTE2Y2U0MzY4NTE0NDVmMzcxNDM1M2QyNzAwNz9zPTQ4MCZyPXBnJmQ9aHR0cHMlM0ElMkYlMkZjZG4uYXV0aDAuY29tJTJGYXZhdGFycyUyRmwucG5nIiwidXBkYXRlZF9hdCI6IjIwMjMtMTEtMDFUMTE6NDc6NTYuMjE3WiIsImVtYWlsIjoibC5iaXpAbm92dW0tZW5naW5lZXJpbmcuY29tIiwiZW1haWxfdmVyaWZpZWQiOnRydWUsImlzcyI6Imh0dHBzOi8vZGV2LW5vdnVtLmV1LmF1dGgwLmNvbS8iLCJhdWQiOiJwN0pSSEI3bVlvOGt5RXVlVWt2VnhTWFo5YllXSWZSbCIsImlhdCI6MTY5ODg0Nzk2MywiZXhwIjoxNjk4ODgzOTYzLCJzdWIiOiJhdXRoMHw2MjMzM2RiNGJjNzgzNDAwNjhjMzdjOTEiLCJzaWQiOiIwOHVGV09oX3V2N3J2Z0p3dy1HMVhMQ0F1QTNsUUFjQyIsIm5vbmNlIjoiV0hvd1NXTnlORmhpUkdGdmEwWnViSFJtUTBGUVdGcEdaRXRRTlM1bU1WVnVUa2hHZVMwdVlqVXRRdz09In0.YtOCMsRWNQIbt_XxKdyLr7Y4IP60FQea3T5KKtLJ2V753A91DbTYYGxvCdwsrGtyoXge1_8Yp7_6_bAbGKkr5K1RLSGzbUEkgqe9KvbBSI8uDvDM8hPOPGAUYq5-XyL4j2I36NWQqsT1i32d6ozf_fJqXHurfvXASfXHK7Wp6moTAV7HtqvYhcwfC9ZbV9hqplldLCkxYPe2lkzky0H-EfJqLh1X-g8hLCnn_9TW2d1LFIxHbciIaYaAqhjtU01KveDKyu3imi4m5z2pxa3hW6T_nYKB1utXUHacvMX89zMuGGSOZrNa9Ww9zhmzVgA4NG-SFCKQFNMThGkMdPdKqA"
-    result = parse_jwt(sample_token)
-    assert result is not None
-    assert "user" in result["https://novum-batteries.com/roles"]
+    def test_parse_jwt(self):
+        """Check jwt."""
+        sample_token = "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Im9Ma1Ridm93cnFndXdoN3lPaUttTCJ9.eyJodHRwczovL25vdnVtLWJhdHRlcmllcy5jb20vcm9sZXMiOlsidXNlciIsImludm9pY2VDcmVhdG9yIiwibm92dW1FeHBlcnQiXSwiaHR0cHM6Ly9ub3Z1bS1iYXR0ZXJpZXMuY29tL3NldHRpbmdzIjp7ImludmVydEF4aXMiOnRydWUsInNlcnZpY2VDZW50ZXIiOnsic2hvd0FkdmFuY2VkT3B0aW9ucyI6dHJ1ZSwiaW52ZXJ0QXhpcyI6dHJ1ZSwiZmF2b3JpdGVCYXR0ZXJpZXNJZHMiOlsiOW94SHZjNnlOWld1VzNzRWsiLCIyRUdFTjd1TU40YWg4ckRGWiIsIkRUQUhIRFR1SkJEQ3ZRRlNKIiwiOVJBU0VIZHZxRW9odlBFU1oiLCJkenBEd3NoUEFHc2N5NkJHaCIsIkFjY3lxSGdvR25IU0F3ZTlHIiwiczdNU1g0ZjNIcWpDcHZ1TEoiLCI1YzdlYkJTekNXNFJuckYzNCIsIkhQZ0RLVFRUSjNEUUhGZ0FEIl0sImJhdHRlcnlUYWJsZUNvbHVtbnMiOlsibmFtZSIsInN0YXRlLnN0YXRlX29mX2NoYXJnZS52YWx1ZSIsInN0YXRlLnN0YXRlX29mX2hlYWx0aC52YWx1ZSIsIm1ldHJpY3Muc3RhdGVfb2ZfaGVhbHRoIiwiaW50ZXJuYWxfY2FwYWNpdHlfY291bnQiLCJpbnRlcm5hbF9kYXRhc2V0X2NvdW50IiwiY3JlYXRvcl9pZCIsImxpZmV0aW1lX2luZGljYXRvciIsImludGVybmFsX2FjdGlvbnMiXSwiZGFzaGJvYXJkVGFibGVDb2x1bW5zIjpbIm5hbWUiLCJiYXR0ZXJ5X3R5cGUubmFtZSIsInN0YXRlLnN0YXRlX29mX2NoYXJnZS52YWx1ZSIsInN0YXRlLnN0YXRlX29mX2hlYWx0aC52YWx1ZSIsImxpZmV0aW1lX2luZGljYXRvciIsImludGVybmFsX2FjdGlvbnMiXSwiZWlzRGF0YXNldFRhYmxlQ29sdW1ucyI6WyJpZCIsIm1ldGEuYmF0dGVyeS5uYW1lIiwiYW5hbHlzaXMuc3RhdGVfb2ZfY2hhcmdlIiwiYW5hbHlzaXMuc3RhdGVfb2ZfaGVhbHRoIiwiaW50ZXJuYWxfYWN0aW9ucyIsImFuYWx5c2lzLmdyYWRlIiwiY3JlYXRvcl9pZCIsImNvbnRleHRfaWQiLCJjcmVhdGVkX2F0Il0sImNhcGFjaXR5TWVhc3VyZW1lbnRUYWJsZUNvbHVtbnMiOlsiaWQiLCJiYXR0ZXJ5Lm5hbWUiLCJzdGF0ZV9vZl9oZWFsdGgiLCJjcmVhdGVkX2F0IiwiaW50ZXJuYWxfYWN0aW9ucyIsImdyYWRlIiwiY3JlYXRvcl9pZCIsImNvbnRleHRfaWQiLCJzdGFydF90aW1lIiwiZW5kX3RpbWUiXX19LCJnaXZlbl9uYW1lIjoiTGVvbmFyZG8iLCJmYW1pbHlfbmFtZSI6IkJpeiIsIm5pY2tuYW1lIjoibC5iaXoiLCJuYW1lIjoiTGVvIEJpeiIsInBpY3R1cmUiOiJodHRwczovL3MuZ3JhdmF0YXIuY29tL2F2YXRhci8yZTRiYTE2Y2U0MzY4NTE0NDVmMzcxNDM1M2QyNzAwNz9zPTQ4MCZyPXBnJmQ9aHR0cHMlM0ElMkYlMkZjZG4uYXV0aDAuY29tJTJGYXZhdGFycyUyRmwucG5nIiwidXBkYXRlZF9hdCI6IjIwMjMtMTEtMDFUMTE6NDc6NTYuMjE3WiIsImVtYWlsIjoibC5iaXpAbm92dW0tZW5naW5lZXJpbmcuY29tIiwiZW1haWxfdmVyaWZpZWQiOnRydWUsImlzcyI6Imh0dHBzOi8vZGV2LW5vdnVtLmV1LmF1dGgwLmNvbS8iLCJhdWQiOiJwN0pSSEI3bVlvOGt5RXVlVWt2VnhTWFo5YllXSWZSbCIsImlhdCI6MTY5ODg0Nzk2MywiZXhwIjoxNjk4ODgzOTYzLCJzdWIiOiJhdXRoMHw2MjMzM2RiNGJjNzgzNDAwNjhjMzdjOTEiLCJzaWQiOiIwOHVGV09oX3V2N3J2Z0p3dy1HMVhMQ0F1QTNsUUFjQyIsIm5vbmNlIjoiV0hvd1NXTnlORmhpUkdGdmEwWnViSFJtUTBGUVdGcEdaRXRRTlM1bU1WVnVUa2hHZVMwdVlqVXRRdz09In0.YtOCMsRWNQIbt_XxKdyLr7Y4IP60FQea3T5KKtLJ2V753A91DbTYYGxvCdwsrGtyoXge1_8Yp7_6_bAbGKkr5K1RLSGzbUEkgqe9KvbBSI8uDvDM8hPOPGAUYq5-XyL4j2I36NWQqsT1i32d6ozf_fJqXHurfvXASfXHK7Wp6moTAV7HtqvYhcwfC9ZbV9hqplldLCkxYPe2lkzky0H-EfJqLh1X-g8hLCnn_9TW2d1LFIxHbciIaYaAqhjtU01KveDKyu3imi4m5z2pxa3hW6T_nYKB1utXUHacvMX89zMuGGSOZrNa9Ww9zhmzVgA4NG-SFCKQFNMThGkMdPdKqA"
+        result = parse_jwt(sample_token)
+        assert result is not None
+        assert "user" in result["https://novum-batteries.com/roles"]
 
+    # Base API tests
 
-class TestBaseAPIClient:
     @pytest.fixture
     def base_api_client(self):
-        return BaseAPIClient()
+        """Fixture: Base API Client."""
+        base_api = BaseAPIClient()
+        return base_api
 
-    # Test the from_window_location class method
     def test_from_window_location(self):
+        """# Check from_window_location class method."""
         origin = "https://novum-batteries.com"
         client = BaseAPIClient.from_window_location(origin)
         assert client.host == origin
 
-    # Test the _clear_user method
     def test_clear_user(self, base_api_client):
-        base_api_client.user = user_mage
+        """Check clear user info method."""
+        base_api_client.user = self.user_sample_mage
         base_api_client._clear_user()
         assert base_api_client.user is None
 
-    # Test the _remove_relogin_timer_handle method
     def test_remove_relogin_timer_handle(self, base_api_client):
+        """Check _remove_relogin_timer_handle method."""
         base_api_client._relogin_timer_handle = 3
         base_api_client._remove_relogin_timer_handle()
         assert base_api_client._relogin_timer_handle is None
 
-    # Test the _get_expire_time_from_token_in_unix_time_millis method
     def test_get_expire_time_from_token_in_unix_time_millis(self, base_api_client):
+        """Check  _get_expire_time_from_token_in_unix_time_millis method."""
         sample_token = "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6Im9Ma1Ridm93cnFndXdoN3lPaUttTCJ9.eyJodHRwczovL25vdnVtLWJhdHRlcmllcy5jb20vcm9sZXMiOlsidXNlciIsImludm9pY2VDcmVhdG9yIiwibm92dW1FeHBlcnQiXSwiaHR0cHM6Ly9ub3Z1bS1iYXR0ZXJpZXMuY29tL3NldHRpbmdzIjp7ImludmVydEF4aXMiOnRydWUsInNlcnZpY2VDZW50ZXIiOnsic2hvd0FkdmFuY2VkT3B0aW9ucyI6dHJ1ZSwiaW52ZXJ0QXhpcyI6dHJ1ZSwiZmF2b3JpdGVCYXR0ZXJpZXNJZHMiOlsiOW94SHZjNnlOWld1VzNzRWsiLCIyRUdFTjd1TU40YWg4ckRGWiIsIkRUQUhIRFR1SkJEQ3ZRRlNKIiwiOVJBU0VIZHZxRW9odlBFU1oiLCJkenBEd3NoUEFHc2N5NkJHaCIsIkFjY3lxSGdvR25IU0F3ZTlHIiwiczdNU1g0ZjNIcWpDcHZ1TEoiLCI1YzdlYkJTekNXNFJuckYzNCIsIkhQZ0RLVFRUSjNEUUhGZ0FEIl0sImJhdHRlcnlUYWJsZUNvbHVtbnMiOlsibmFtZSIsInN0YXRlLnN0YXRlX29mX2NoYXJnZS52YWx1ZSIsInN0YXRlLnN0YXRlX29mX2hlYWx0aC52YWx1ZSIsIm1ldHJpY3Muc3RhdGVfb2ZfaGVhbHRoIiwiaW50ZXJuYWxfY2FwYWNpdHlfY291bnQiLCJpbnRlcm5hbF9kYXRhc2V0X2NvdW50IiwiY3JlYXRvcl9pZCIsImxpZmV0aW1lX2luZGljYXRvciIsImludGVybmFsX2FjdGlvbnMiXSwiZGFzaGJvYXJkVGFibGVDb2x1bW5zIjpbIm5hbWUiLCJiYXR0ZXJ5X3R5cGUubmFtZSIsInN0YXRlLnN0YXRlX29mX2NoYXJnZS52YWx1ZSIsInN0YXRlLnN0YXRlX29mX2hlYWx0aC52YWx1ZSIsImxpZmV0aW1lX2luZGljYXRvciIsImludGVybmFsX2FjdGlvbnMiXSwiZWlzRGF0YXNldFRhYmxlQ29sdW1ucyI6WyJpZCIsIm1ldGEuYmF0dGVyeS5uYW1lIiwiYW5hbHlzaXMuc3RhdGVfb2ZfY2hhcmdlIiwiYW5hbHlzaXMuc3RhdGVfb2ZfaGVhbHRoIiwiaW50ZXJuYWxfYWN0aW9ucyIsImFuYWx5c2lzLmdyYWRlIiwiY3JlYXRvcl9pZCIsImNvbnRleHRfaWQiLCJjcmVhdGVkX2F0Il0sImNhcGFjaXR5TWVhc3VyZW1lbnRUYWJsZUNvbHVtbnMiOlsiaWQiLCJiYXR0ZXJ5Lm5hbWUiLCJzdGF0ZV9vZl9oZWFsdGgiLCJjcmVhdGVkX2F0IiwiaW50ZXJuYWxfYWN0aW9ucyIsImdyYWRlIiwiY3JlYXRvcl9pZCIsImNvbnRleHRfaWQiLCJzdGFydF90aW1lIiwiZW5kX3RpbWUiXX19LCJnaXZlbl9uYW1lIjoiTGVvbmFyZG8iLCJmYW1pbHlfbmFtZSI6IkJpeiIsIm5pY2tuYW1lIjoibC5iaXoiLCJuYW1lIjoiTGVvIEJpeiIsInBpY3R1cmUiOiJodHRwczovL3MuZ3JhdmF0YXIuY29tL2F2YXRhci8yZTRiYTE2Y2U0MzY4NTE0NDVmMzcxNDM1M2QyNzAwNz9zPTQ4MCZyPXBnJmQ9aHR0cHMlM0ElMkYlMkZjZG4uYXV0aDAuY29tJTJGYXZhdGFycyUyRmwucG5nIiwidXBkYXRlZF9hdCI6IjIwMjMtMTEtMDFUMTE6NDc6NTYuMjE3WiIsImVtYWlsIjoibC5iaXpAbm92dW0tZW5naW5lZXJpbmcuY29tIiwiZW1haWxfdmVyaWZpZWQiOnRydWUsImlzcyI6Imh0dHBzOi8vZGV2LW5vdnVtLmV1LmF1dGgwLmNvbS8iLCJhdWQiOiJwN0pSSEI3bVlvOGt5RXVlVWt2VnhTWFo5YllXSWZSbCIsImlhdCI6MTY5ODg0Nzk2MywiZXhwIjoxNjk4ODgzOTYzLCJzdWIiOiJhdXRoMHw2MjMzM2RiNGJjNzgzNDAwNjhjMzdjOTEiLCJzaWQiOiIwOHVGV09oX3V2N3J2Z0p3dy1HMVhMQ0F1QTNsUUFjQyIsIm5vbmNlIjoiV0hvd1NXTnlORmhpUkdGdmEwWnViSFJtUTBGUVdGcEdaRXRRTlM1bU1WVnVUa2hHZVMwdVlqVXRRdz09In0.YtOCMsRWNQIbt_XxKdyLr7Y4IP60FQea3T5KKtLJ2V753A91DbTYYGxvCdwsrGtyoXge1_8Yp7_6_bAbGKkr5K1RLSGzbUEkgqe9KvbBSI8uDvDM8hPOPGAUYq5-XyL4j2I36NWQqsT1i32d6ozf_fJqXHurfvXASfXHK7Wp6moTAV7HtqvYhcwfC9ZbV9hqplldLCkxYPe2lkzky0H-EfJqLh1X-g8hLCnn_9TW2d1LFIxHbciIaYaAqhjtU01KveDKyu3imi4m5z2pxa3hW6T_nYKB1utXUHacvMX89zMuGGSOZrNa9Ww9zhmzVgA4NG-SFCKQFNMThGkMdPdKqA"
         result = base_api_client._get_expire_time_from_token_in_unix_time_millis(
             sample_token
         )
         assert isinstance(result, str)
 
-    # TODO def test_install_token_refresh_procedure(self, user_mage):
+    # TODO def test_install_token_refresh_procedure(self, user_sample_mage):
 
     @pytest.mark.parametrize(
         "ok_value, status_code, expected_error",
         [
             (True, 200, None),
             (
                 False,
                 400,
                 f"Failed to load resource {PRODUCTION_API_HOST} -> Status:400",
             ),
         ],
     )
     def test_fetch_by_URL(self, base_api_client, ok_value, status_code, expected_error):
-        # Mock the _get_json method to return a response
+        """Mock the _get_json method to return a response."""
         response = {"ok": ok_value, "status": status_code}
         base_api_client._get_json = Mock(return_value=response)
 
         url = PRODUCTION_API_HOST
         options = {}
 
         if expected_error:
@@ -129,15 +135,15 @@
                 False,
                 400,
                 f"('Failed to load resource {PRODUCTION_API_HOST} -> Status:400'",
             ),
         ],
     )
     def test_post_by_URL(self, base_api_client, ok_value, status_code, expected_error):
-        # Mock the _post_json method to return a response
+        """Check the _post_json method to return a response."""
         response = {"ok": ok_value, "status": status_code}
         base_api_client._post_json = Mock(return_value=response)
 
         url = PRODUCTION_API_HOST
         options = {}
 
         if expected_error:
```

### Comparing `novum_api_client-1.1.1/novum_api_client/tests/test_api_public.py` & `novum_api_client-2.0.0/novum_api_client/tests/test_api_public.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,222 +7,275 @@
 from datetime import datetime
 import json
 import pytest
 
 from ..base_client import NovumAPIError
 from ..client import NovumAPIClient
 from ..api_type import (
-    ReportStates,
+    TUser,
+    TReport,
+    TVersion,
     TAnalysis,
-    TBattery,
-    TBatteryEssentials,
-    TBatteryType,
-    TBatteryTypeEssentials,
-    TCapacityMeasurement,
-    TCapacityMeasurementEssentials,
+    TEISSetup,
+    TMeasured,
     TChargeCycle,
     TChargeTypes,
-    TDataset,
-    TDatasetEssentials,
     TDatasetMeta,
-    TDeviceMetaParticle,
-    TEISSetup,
-    TMeasured,
+    ReportStates,
+    TTimedMeasure,
     TMeasurementCycle,
-    TReport,
     TReportEssentials,
-    TTimedMeasure,
-    TUser,
     TAPIInfoEssentials,
-    TVersion,
-    TVersionEssentials,
+    TDatasetEssentials,
+    TBatteryEssentials,
+    TDeviceMetaParticle,
+    TBatteryTypeEssentials,
+    TCapacityMeasurementEssentials,
 )
 
 
 class TestNovumAPIClient:
     @pytest.fixture(scope="class")
     def unauthenticated_api_client(self):
+        """Check if authenticated before login."""
         api_client = NovumAPIClient()
         yield api_client
 
     @pytest.fixture(scope="class")
     def ada_logged_client(self):
+        """Fixture API client logged in."""
         client = NovumAPIClient()
         client.login(
             email="ada.lovelace@novum-engineering.com", password="5TkbQuVEx4v2GVqJ"
         )
         yield client
 
     def test_ping(self, unauthenticated_api_client: NovumAPIClient):
+        """Check ping message."""
         response = unauthenticated_api_client.ping()
 
         assert (
             response["message"]
             == "Hello user this is the Novum batman API server. All routes begin with /api/{api_type}/{api_version}/{resource}. You have to identify using your credentials and /api/batman/v1/login to obtain a token"
         )
 
     def test_get_info(self, unauthenticated_api_client: NovumAPIClient):
+        """Check info root."""
         info = unauthenticated_api_client.get_info()
 
         assert isinstance(info, TAPIInfoEssentials)
         assert info.name == "Novum Base API"
         assert info.dbName == "batman"
 
     def test_get_version(self, unauthenticated_api_client: NovumAPIClient):
+        """Check version"""
         version = unauthenticated_api_client.get_version()
 
-        assert isinstance(version, TVersionEssentials)
+        assert isinstance(version, TVersion)
         assert version.name == "novum-api"
         assert version.branch == "master"
 
     def test_login_ada(self, unauthenticated_api_client: NovumAPIClient):
+        """Check Ada login."""
         response = unauthenticated_api_client.login(
             email="ada.lovelace@novum-engineering.com", password="5TkbQuVEx4v2GVqJ"
         )
         assert isinstance(response, TUser)
         assert "user" in response.roles
 
     def test_login_ada_with_wrong_credentials(
         self, unauthenticated_api_client: NovumAPIClient
     ):
+        """Check if login with wrong password gets authenticated."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.login(
                 email="ada.lovelace@novum-engineering.com", password="WrongPassword"
             )
 
         error_details = json.loads(str(excinfo.value))
 
         expected_error_message = "Wrong email or password."
         assert expected_error_message in error_details["details"]
 
     def test_check_current_user_still_authenticated(
         self, ada_logged_client: NovumAPIClient
     ):
+        """Check authentication."""
         response = ada_logged_client.check_current_user_still_authenticated()
         assert response["authenticated"] is True
 
     def test_logout(self, ada_logged_client: NovumAPIClient):
+        """Check logout function."""
         response = ada_logged_client.logout()
         assert response == {"message": "Logout successful"}
 
     # ********************************************************
     # Section for the Battery Type
     # ********************************************************
 
     @pytest.fixture
     def sample_battery_type(self):
-        return TBatteryTypeEssentials(
+        """Fixture: Battery Type"""
+        sample_battery_type = TBatteryTypeEssentials(
             name="Test Battery Type",
             manufacturer="The Tester",
             nominal_voltage=3.7,
             nominal_capacity=2500,
         )
+        return sample_battery_type
 
     @pytest.fixture
     def created_battery_type(
         self,
         ada_logged_client: NovumAPIClient,
         sample_battery_type: TBatteryTypeEssentials,
     ):
+        """Fixture: sample of battery type."""
         response = ada_logged_client.create_battery_type(sample_battery_type)
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_battery_types_by_id(response.id)
 
     def test_get_battery_type(
-        self, ada_logged_client: NovumAPIClient, created_battery_type: TBatteryType
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery_type: TBatteryTypeEssentials,
     ):
+        """Check if the created battery type can be fetched."""
         response = ada_logged_client.get_battery_types()
 
         assert response[0].id == created_battery_type.id
 
+    def test_get_battery_type_with_fields(
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery_type: TBatteryTypeEssentials,
+    ):
+        """Check if the created battery type can be fetched with fields."""
+        fields = {"name": 1}
+        response = ada_logged_client.get_battery_types(fields=fields)
+
+        assert response[0].id == created_battery_type.id
+        assert response[0].name == created_battery_type.name
+        assert response[0].manufacturer is None
+
+    def test_get_battery_type_without_fields(
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery_type: TBatteryTypeEssentials,
+    ):
+        """Check if the created battery type can be fetched without fields."""
+        fields = {"name": 0}
+        response = ada_logged_client.get_battery_types(fields=fields)
+
+        assert response[0].id == created_battery_type.id
+        assert response[0].name is None
+
     def test_get_battery_type_count(self, ada_logged_client: NovumAPIClient):
+        """Check number of battery types created."""
         response = ada_logged_client.get_battery_types_count()
         assert response == 6
 
     def test_get_battery_type_by_id(
-        self, ada_logged_client: NovumAPIClient, created_battery_type: TBatteryType
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery_type: TBatteryTypeEssentials,
     ):
+        """Check fetching battery type by id"""
         response = ada_logged_client.get_battery_types_by_id(created_battery_type.id)
         assert response.id == created_battery_type.id
 
-    def test_create_battery_type(self, created_battery_type: TBatteryType):
-
+    def test_create_battery_type(self, created_battery_type: TBatteryTypeEssentials):
+        """Check info of created battery type."""
         assert created_battery_type.name == "Test Battery Type"
         assert created_battery_type.nominal_voltage == 3.7
         assert created_battery_type.nominal_capacity == 2500
 
     @pytest.fixture
     def sample_battery_type_without_name(
         self, sample_battery_type: TBatteryTypeEssentials
     ):
+        """Fixture: battery type without name."""
         sample_battery_type.name = None  # type: ignore
         return sample_battery_type
 
     def test_create_battery_type_missing_required_field_name(
         self,
         unauthenticated_api_client: NovumAPIClient,
-        sample_battery_type_without_name: TBatteryType,
+        sample_battery_type_without_name: TBatteryTypeEssentials,
     ):
+        """Check if attempt to create a battery type without name raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_battery_type(
                 sample_battery_type_without_name
             )
 
         assert '{"error":"Failed to validate battery type data","details":' in str(
             excinfo.value
         )
 
     @pytest.fixture
     def sample_battery_type_without_manufacturer(
         self, sample_battery_type: TBatteryTypeEssentials
     ):
+        """Fixture: battery type without manufacturer."""
         sample_battery_type.manufacturer = None  # type: ignore
         return sample_battery_type
 
     def test_create_battery_type_missing_required_field_manufacturer(
         self,
         unauthenticated_api_client: NovumAPIClient,
-        sample_battery_type_without_manufacturer: TBatteryType,
+        sample_battery_type_without_manufacturer: TBatteryTypeEssentials,
     ):
+        """Check if attempt to create a battery type without manufacturer raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_battery_type(
                 sample_battery_type_without_manufacturer
             )
 
         assert (
             '{"error":"Failed to validate battery type data","details":"Key: \'BatteryType.Manufacturer\''
             in str(excinfo.value)
         )
 
     @pytest.fixture
-    def sample_battery_type_without_capacity(self, sample_battery_type: TBatteryType):
+    def sample_battery_type_without_capacity(
+        self, sample_battery_type: TBatteryTypeEssentials
+    ):
+        """Fixture: battery type without nominal capacity."""
         sample_battery_type.nominal_capacity = ""  # type: ignore
         return sample_battery_type
 
     def test_create_battery_type_missing_required_field_capacity(
         self,
         ada_logged_client: NovumAPIClient,
-        sample_battery_type_without_capacity: TBatteryType,
+        sample_battery_type_without_capacity: TBatteryTypeEssentials,
     ):
+        """Check if attempt to create a battery type without nominal capacity raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             ada_logged_client.create_battery_type(sample_battery_type_without_capacity)
 
         assert '{"error":"Failed to decode battery type data"' in str(excinfo.value)
 
     @pytest.fixture
-    def sample_battery_type_without_voltage(self, sample_battery_type: TBatteryType):
+    def sample_battery_type_without_voltage(
+        self, sample_battery_type: TBatteryTypeEssentials
+    ):
+        """Fixture: battery type without nominal voltage."""
         sample_battery_type.nominal_voltage = ""  # type: ignore
         return sample_battery_type
 
     def test_update_battery_type(
-        self, ada_logged_client: NovumAPIClient, created_battery_type: TBatteryType
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery_type: TBatteryTypeEssentials,
     ):
+        """Check if attempt to create a battery type without nominal voltage raises an error."""
         update_data = TBatteryTypeEssentials(
             name="Updated Battery Type",
             manufacturer="Updated",
             nominal_voltage=3.8,
             nominal_capacity=3200,
             description="There is an update",
         )
@@ -236,95 +289,141 @@
         assert updated_response.nominal_voltage == 3.8
         assert updated_response.nominal_capacity == 3200
         assert updated_response.description == "There is an update"
 
     def test_delete_battery_type_from_another_user(
         self, ada_logged_client: NovumAPIClient
     ):
+        """Check if attempt to delete a battery type from another uses raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             ada_logged_client.remove_battery_types_by_id("dpgtbPhcnt5oH685D")
 
         assert '{"error":"Forbidden","details":""}' in str(excinfo.value)
 
     def test_delete_battery_type(
         self, ada_logged_client: NovumAPIClient, sample_battery_type
     ):
+        """Check battery type deletion."""
         sample_battery_type.name = "to be deleted"
         to_be_deleted_sample = sample_battery_type
         to_be_deleted = ada_logged_client.create_battery_type(to_be_deleted_sample)
 
         response = ada_logged_client.remove_battery_types_by_id(to_be_deleted.id)
 
         assert "was removed" in response
 
     # # ********************************************************
     # # Section for the Battery
     # # ********************************************************
 
     @pytest.fixture
-    def sample_battery(self, created_battery_type: TBatteryType):
+    def sample_battery(self, created_battery_type: TBatteryTypeEssentials):
+        """Fixture: sample of battery."""
         return TBatteryEssentials(
             name="Test Battery", battery_type=created_battery_type
         )
 
     @pytest.fixture
     def created_battery(
         self, ada_logged_client: NovumAPIClient, sample_battery: TBatteryEssentials
     ):
+        """Fixture: sample of battery."""
 
         response = ada_logged_client.create_battery(sample_battery)
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_battery_by_id(response.id)
 
-    def test_create_battery(self, created_battery: TBattery):
+    def test_create_battery(self, created_battery: TBatteryEssentials):
+        """Check battery creation."""
 
         assert created_battery.name == "Test Battery"
 
+    def test_get_battery(
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery: TBatteryEssentials,
+    ):
+        """Check if the created battery can be fetched."""
+        response = ada_logged_client.get_batteries()
+
+        assert response[0].id == created_battery.id
+
+    def test_get_battery_with_fields(
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery: TBatteryEssentials,
+    ):
+        """Check if the created battery can be fetched with fields."""
+        fields = {"name": 1}
+        response = ada_logged_client.get_batteries(fields=fields)
+
+        assert response[0].id == created_battery.id
+        assert response[0].name == created_battery.name
+        assert response[0].description is None
+
+    def test_get_battery_without_fields(
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery: TBatteryEssentials,
+    ):
+        """Check if the created battery can be fetched without fields."""
+        fields = {"name": 0}
+        response = ada_logged_client.get_batteries(fields=fields)
+
+        assert response[0].id == created_battery.id
+        assert response[0].name is None
+        assert response[0].description is None
+
     @pytest.fixture
     def sample_battery_without_name(self, sample_battery: TBatteryEssentials):
+        """Fixture: battery without name."""
         sample_battery.name = None  # type: ignore
 
         return sample_battery
 
     def test_create_battery_missing_required_field_name(
         self,
         unauthenticated_api_client: NovumAPIClient,
         sample_battery_without_name: TBatteryEssentials,
     ):
+        """Check if attempt to create a battery without name raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_battery(sample_battery_without_name)
 
         assert '{"error":"Failed to validate ' in str(excinfo.value)
 
     def test_update_battery(
         self,
         ada_logged_client: NovumAPIClient,
-        created_battery: TBattery,
-        created_battery_type: TBatteryType,
+        created_battery: TBatteryEssentials,
+        created_battery_type: TBatteryTypeEssentials,
     ):
+        """Check battery updating."""
         update_data = TBatteryEssentials(
             name="Updated Battery",
             battery_type=created_battery_type,
             description="There is an update",
         )
 
         updated_response = ada_logged_client.update_battery_by_id(
             created_battery.id, update_data
         )
 
         assert updated_response.name == "Updated Battery"
         assert updated_response.description == "There is an update"
 
     def test_delete_battery(
-        self, ada_logged_client: NovumAPIClient, created_battery_type: TBatteryType
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_battery_type: TBatteryTypeEssentials,
     ):
-
+        """Check battery deletion."""
         to_be_deleted_sample = TBatteryEssentials(
             name="Test Battery Delete", battery_type=created_battery_type
         )
         to_be_deleted = ada_logged_client.create_battery(to_be_deleted_sample)
 
         response = ada_logged_client.remove_battery_by_id(to_be_deleted.id)
 
@@ -332,14 +431,15 @@
 
     # ********************************************************
     # Section for the DataSet
     # ********************************************************
 
     @pytest.fixture
     def sample_eis_dataset(self):
+        """Fixture: EIS measurement."""
         sample_eis = TDatasetEssentials(
             measured=TMeasured(
                 start_time="2021-03-10T17:40:44.956Z",
                 end_time="2021-03-10T17:42:43.915Z",
                 eis_setup=TEISSetup(
                     start_frequency=4000,
                     end_frequency=0.1,
@@ -371,15 +471,15 @@
                         current_raw_values=None,
                         voltage_raw_values=None,
                     )
                 ],
             ),
             analysis=TAnalysis(),
             meta=TDatasetMeta(
-                tags=["tag", "tag"],
+                tags=["tag1", "tag2"],
                 client_software=TVersion(
                     tag="test_tag",
                     name="test",
                     hash=None,
                     branch=None,
                     build_date=None,
                     error=None,
@@ -404,90 +504,122 @@
         )
         return sample_eis
 
     @pytest.fixture
     def created_eis_dataset(
         self, ada_logged_client: NovumAPIClient, sample_eis_dataset: TDatasetEssentials
     ):
+        """Fixture: created EIS measurement."""
 
         response = ada_logged_client.create_dataset(sample_eis_dataset)
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_dataset_by_id(response.id)
 
-    def test_create_eis_dataset(self, created_eis_dataset: TDataset):
+    def test_create_eis_dataset(self, created_eis_dataset: TDatasetEssentials):
+        """Check EIS creation."""
 
-        assert isinstance(created_eis_dataset, TDataset)
+        assert isinstance(created_eis_dataset, TDatasetEssentials)
 
     @pytest.fixture
     def sample_dataset_without_name(self, sample_eis_dataset: TDatasetEssentials):
+        """Fixture: EIS measurement without name"""
         sample_eis_dataset.measured.start_time = None  # type : ignore
         return sample_eis_dataset
 
     def test_create_dataset_missing_required_field_start_time(
         self,
         unauthenticated_api_client: NovumAPIClient,
         sample_dataset_without_name: TDatasetEssentials,
     ):
+        """Check if attempt to create a EIS measurement without name raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_dataset(sample_dataset_without_name)
 
         assert (
             '{"error":"Failed to validate dataset","details":"Key: \'Dataset.Measured.StartTime\' Error:'
             in str(excinfo.value)
         )
 
     def test_get_dataset(
-        self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDataset
+        self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
     ):
+        """Check created EIS measurement."""
         response = ada_logged_client.get_datasets()
 
         assert response[0].id == created_eis_dataset.id
 
+    def test_get_dataset_with_fields(
+        self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
+    ):
+        """Check created EIS measurement with fields."""
+        fields = {"context_id": 1}
+        response = ada_logged_client.get_datasets(fields=fields)
+
+        assert response[0].id == created_eis_dataset.id
+        assert response[0].context_id == created_eis_dataset.context_id
+        assert response[0].show_in_chart is None
+
+    def test_get_dataset_without_fields(
+        self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
+    ):
+        """Check created EIS measurement without fields."""
+        fields = {"context_id": 0}
+        response = ada_logged_client.get_datasets(fields=fields)
+
+        assert response[0].id == created_eis_dataset.id
+        assert response[0].context_id is None
+        assert response[0].show_in_chart is None
+
     def test_get_datasets_count(self, ada_logged_client: NovumAPIClient):
+        """Check amount of EIS measurements."""
         response = ada_logged_client.get_datasets_count()
 
         assert response == 0
 
     def test_get_dataset_by_id(
-        self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDataset
+        self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
     ):
+        """Check created dataset by id."""
         response = ada_logged_client.get_dataset_by_id(created_eis_dataset.id)
 
         assert response.id == created_eis_dataset.id
 
     def test_update_dataset(
-        self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDataset
+        self, ada_logged_client: NovumAPIClient, created_eis_dataset: TDatasetEssentials
     ):
+        """Check EIS measurement update."""
         response = ada_logged_client.get_dataset_by_id(created_eis_dataset.id)
         response.context_id = "new_context_id"
         ada_logged_client.update_dataset_by_id(created_eis_dataset.id, response)
         response_updated = ada_logged_client.get_dataset_by_id(created_eis_dataset.id)
 
         assert response_updated.context_id == "new_context_id"
 
     def test_delete_dataset(
         self, ada_logged_client: NovumAPIClient, sample_eis_dataset: TDatasetEssentials
     ):
+        """Check EIS measurement deletion."""
         to_be_deleted_sample = sample_eis_dataset
         to_be_deleted = ada_logged_client.create_dataset(to_be_deleted_sample)
 
         response = ada_logged_client.remove_dataset_by_id(to_be_deleted.id)
 
         assert "was removed" in response
 
     # ********************************************************
     # Section for the Capacity Measurement
     # ********************************************************
 
     @pytest.fixture
     def sample_capacity_measurement(self):
-        return TCapacityMeasurementEssentials(
+        """Fixture: sample capacity measurement."""
+        sample_capacity = TCapacityMeasurementEssentials(
             start_time=datetime(2023, 11, 10, 5, 5, 5),
             end_time=None,
             current_setpoint=1,
             voltage_setpoint=2,
             charge_type=TChargeTypes.CC,
             charge_cycles=[
                 TChargeCycle(
@@ -502,89 +634,123 @@
             device_name="NOVUM Testing Device",
             device_info="Firmware: v1.02",
             voltage_min=2.14,
             voltage_max=3.14,
             state_of_health=0.94,
             grade="D",
         )
+        return sample_capacity
 
     @pytest.fixture
     def created_capacity_measurement(
         self,
         ada_logged_client: NovumAPIClient,
         sample_capacity_measurement: TCapacityMeasurementEssentials,
     ):
+        """Fixture: capacity measurement creation."""
 
         response = ada_logged_client.create_capacity_measurement(
             sample_capacity_measurement
         )
 
         yield response
 
         # Add cleanup code here to delete the created battery type
         ada_logged_client.remove_capacity_measurement_by_id(response.id)
 
     def test_create_capacity_measurement(
         self, created_capacity_measurement: TCapacityMeasurementEssentials
     ):
+        """Check capacity measurement creation."""
 
         assert created_capacity_measurement.current_setpoint == 1
 
     @pytest.fixture
     def sample_capacity_measurement_without_start_time(
         self, sample_capacity_measurement: TCapacityMeasurementEssentials
     ):
+        """Fixture: sample of capacity measurement without start time."""
         sample_capacity_measurement.start_time = None  # type: ignore
         return sample_capacity_measurement
 
     def test_create_capacity_measurement_missing_required_field_start_time(
         self,
         unauthenticated_api_client: NovumAPIClient,
         sample_capacity_measurement_without_start_time: TCapacityMeasurementEssentials,
     ):
+        """Check if attempt to create a capacity measurement without start time raises an error."""
         with pytest.raises(NovumAPIError) as excinfo:
             unauthenticated_api_client.create_capacity_measurement(
                 sample_capacity_measurement_without_start_time
             )
 
         assert (
             '{"error":"Failed to validate capacity measurement","details":"Key: \'CapacityMeasurement.StartTime\' Error:Field validation for \'StartTime\' failed'
             in str(excinfo.value)
         )
 
-    def test_get_capacity_measurement(
+    def test_get_capacity_measurements(
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_capacity_measurement: TCapacityMeasurementEssentials,
+    ):
+        """Check capacity measurements fetching."""
+        response = ada_logged_client.get_capacity_measurements()
+
+        assert response[0].id == created_capacity_measurement.id
+
+    def test_get_capacity_measurements_with_fields(
+        self,
+        ada_logged_client: NovumAPIClient,
+        created_capacity_measurement: TCapacityMeasurementEssentials,
+    ):
+        """Check capacity measurements fetching with fields."""
+        fields = {"device_name": 1}
+        response = ada_logged_client.get_capacity_measurements(fields=fields)
+
+        assert response[0].id == created_capacity_measurement.id
+        assert response[0].device_name == created_capacity_measurement.device_name
+        assert response[0].grade is None
+
+    def test_get_capacity_measurements_without_fields(
         self,
         ada_logged_client: NovumAPIClient,
-        created_capacity_measurement: TCapacityMeasurement,
+        created_capacity_measurement: TCapacityMeasurementEssentials,
     ):
-        response = ada_logged_client.get_capacity_measurement()
+        """Check capacity measurements fetching without fields."""
+        fields = {"device_name": 0}
+        response = ada_logged_client.get_capacity_measurements(fields=fields)
 
         assert response[0].id == created_capacity_measurement.id
+        assert response[0].device_name is None
 
-    def test_get_capacity_measurement_count(self, ada_logged_client: NovumAPIClient):
-        response = ada_logged_client.get_capacity_measurement_count()
+    def test_get_capacity_measurements_count(self, ada_logged_client: NovumAPIClient):
+        """Check created capacity measurement."""
+        response = ada_logged_client.get_capacity_measurements_count()
 
         assert response == 0
 
     def test_get_capacity_measurement_by_id(
         self,
         ada_logged_client: NovumAPIClient,
-        created_capacity_measurement: TCapacityMeasurement,
+        created_capacity_measurement: TCapacityMeasurementEssentials,
     ):
+        """Check created capacity measurement by id."""
         response = ada_logged_client.get_capacity_measurement_by_id(
             created_capacity_measurement.id
         )
 
         assert response.id == created_capacity_measurement.id
 
     def test_update_capacity_measurement(
         self,
         ada_logged_client: NovumAPIClient,
-        created_capacity_measurement: TCapacityMeasurement,
+        created_capacity_measurement: TCapacityMeasurementEssentials,
     ):
+        """Check capacity measurement updating."""
         response = ada_logged_client.get_capacity_measurement_by_id(
             created_capacity_measurement.id
         )
         response.context_id = "new_context_id"
         ada_logged_client.update_capacity_measurement_by_id(
             created_capacity_measurement.id, response
         )
@@ -595,14 +761,15 @@
         assert response_updated.context_id == "new_context_id"
 
     def test_delete_capacity_measurement(
         self,
         ada_logged_client: NovumAPIClient,
         sample_capacity_measurement: TCapacityMeasurementEssentials,
     ):
+        """Check capacity measurement deletion."""
         to_be_deleted_sample = sample_capacity_measurement
         to_be_deleted = ada_logged_client.create_capacity_measurement(
             to_be_deleted_sample
         )
 
         response = ada_logged_client.remove_capacity_measurement_by_id(to_be_deleted.id)
```

### Comparing `novum_api_client-1.1.1/PKG-INFO` & `novum_api_client-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: novum_api_client
-Version: 1.1.1
+Version: 2.0.0
 Summary: This library contains the basic api functions for Novum Service Center.
 Author: Leonardo
 Author-email: l.biz@novum-engineering.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Description-Content-Type: text/markdown
 
 
 
 # Novum API Library
 
@@ -25,31 +27,36 @@
 Use pip to install:
 
 ```shell
 pip install novum_api_client
 ```
 
 
-
 # Release Notes
 
-## Version 1.1.1
-- Release Date: 2024-04-11
+## Version 2.0.0
+- Release Date: 2024-04-12
 
 ### Enhancements
-- Add new functions (get_user_documents and get_user_document_by_id).
-- Force typing for Reports.
-
+- Added dataclass_json to easy the types.
+- Rename types.
+- Added Docstring.
+- Rename functions "get_capacity_measurement" and "get_capacity_measurement_count".
+- API Client available for Python > 3.8.1
 
 
 # Changelog
 
+## [1.1.1] - 2024-04-11
+- Added new functions (get_user_documents and get_user_document_by_id).
+- Forced typing for Reports.
+
+
 ## [1.0.1] - 2023-12-12
 - Prettier added
 - Most of the function have "fields" as an argument.
-- Reports are now available in our library. 
-- Add Error/Exception messages.
+- Made Reports Section available. 
+- Added Error/Exception messages.
 
 
 ## [1.0.0] - 2023-12-12
 - First release of the library.
-
```

