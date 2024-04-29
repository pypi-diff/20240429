# Comparing `tmp/smart_meter_to_openhab-0.5.1.tar.gz` & `tmp/smart_meter_to_openhab-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_meter_to_openhab-0.5.1.tar", max compression
+gzip compressed data, was "smart_meter_to_openhab-0.5.2.tar", max compression
```

## Comparing `smart_meter_to_openhab-0.5.1.tar` & `smart_meter_to_openhab-0.5.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1211 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/LICENSE
--rw-r--r--   0        0        0     4512 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/README.md
--rw-r--r--   0        0        0      793 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      475 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/.env.example
--rw-r--r--   0        0        0      349 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/__init__.py
--rw-r--r--   0        0        0     9828 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/interfaces.py
--rw-r--r--   0        0        0     5462 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/openhab.py
--rw-r--r--   0        0        0     8905 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/sml_iskra_mt175.py
--rw-r--r--   0        0        0      294 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/utils.py
--rw-r--r--   0        0        0     5489 2024-04-16 19:07:16.461630 smart_meter_to_openhab-0.5.1/smart_meter_to_openhab_scripts/main.py
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4512 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/README.md
+-rw-r--r--   0        0        0      793 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      475 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/.env.example
+-rw-r--r--   0        0        0      349 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/__init__.py
+-rw-r--r--   0        0        0    11175 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/interfaces.py
+-rw-r--r--   0        0        0     4802 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/openhab.py
+-rw-r--r--   0        0        0     8473 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/sml_iskra_mt175.py
+-rw-r--r--   0        0        0      294 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/utils.py
+-rw-r--r--   0        0        0     5729 2024-04-29 19:13:58.590913 smart_meter_to_openhab-0.5.2/smart_meter_to_openhab_scripts/main.py
+-rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.5.2/PKG-INFO
```

### Comparing `smart_meter_to_openhab-0.5.1/LICENSE` & `smart_meter_to_openhab-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.5.1/README.md` & `smart_meter_to_openhab-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.5.1/pyproject.toml` & `smart_meter_to_openhab-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smart_meter_to_openhab"
-version = "0.5.1"
+version = "0.5.2"
 description = "Pushing data of ISKRA MT175 smart meter to openhab"
 authors = ["Heiko Bauer <heiko_bauer@icloud.com>"]
 repository = "https://github.com/die-bauerei/smart-meter-to-openhab"
 readme = "README.md"
 packages = [
     {include = "smart_meter_to_openhab"},
     {include = "smart_meter_to_openhab_scripts"}
```

### Comparing `smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/interfaces.py` & `smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/interfaces.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from dataclasses import dataclass
-from typing import List, Any, Union, Tuple, ClassVar, Iterator
-from statistics import mean
-from abc import ABC
+from typing import List, Any, Union, Tuple, ClassVar, Iterator, Callable
+from statistics import mean, median
+from abc import ABC, abstractmethod
 from functools import cache
 import os
 from .utils import PersistenceValuesType
 
 @dataclass(frozen=True, eq=False)
 class OhItem():
     oh_item : str
@@ -61,20 +61,21 @@
                 if this_value.oh_item == new_value.oh_item:
                     this_value.value = new_value.value
                     break
 
     def __iter__(self) -> Iterator[OhItemAndValue]:
         return iter(self._oh_items_and_values)
     
+    @abstractmethod
     def is_invalid(self) -> bool:
-        number_values=[value for value in self.value_list() if value is not None]
-        return (not number_values) or any(value < 0 for value in number_values)
+        pass
     
+    @abstractmethod
     def is_valid(self) -> bool:
-        return not self.is_invalid()
+        pass
     
     def value_list(self) -> List[Any]:
         # consider only the values that really will be used (oh_item name not empty)
         return [oh_item_value.value for oh_item_value in self._oh_items_and_values  if oh_item_value.oh_item]
     
     def __eq__(self, other) -> bool:
         if isinstance(other, OhItemAndValueContainer):
@@ -112,49 +113,74 @@
     @property
     def overall_consumption(self) -> OhItemAndValue:
         return self._oh_items_and_values[3]
     @property
     def electricity_meter(self) -> OhItemAndValue:
         return self._oh_items_and_values[4]
     
+    def is_invalid(self) -> bool:
+        number_values=[value for value in self.value_list() if value is not None]
+        return (not number_values) or any(value < 0 for value in number_values)
+    
+    def is_valid(self) -> bool:
+        return not self.is_invalid()
+    
+    def is_inconsistent(self, prev_values : SmartMeterValues) -> bool:
+        return not self.is_consistent(prev_values)
+
+    def is_consistent(self, prev_values : SmartMeterValues) -> bool:
+        if self.electricity_meter.value is None or prev_values.electricity_meter.value is None:
+            return True
+        e_meter_unexpected_high = prev_values.electricity_meter.value > 1 and self.electricity_meter.value > prev_values.electricity_meter.value*2
+        return self.electricity_meter.value >= prev_values.electricity_meter.value and not e_meter_unexpected_high
+
     def __repr__(self) -> str:
         return f"L1={self.phase_1_consumption.value} L2={self.phase_2_consumption.value} "\
             f"L3={self.phase_3_consumption.value} Overall={self.overall_consumption.value} E={self.electricity_meter.value}"
 
     @staticmethod
     @cache
     def oh_item_names() -> SmartMeterOhItemNames:
         return SmartMeterValues._oh_item_names
 
     @staticmethod    
     def create(values : List[OhItemAndValue], user_specified_oh_item_names : Union[SmartMeterOhItemNames, None] = None) -> SmartMeterValues:
         value=SmartMeterValues(user_specified_oh_item_names=user_specified_oh_item_names)
         value.assign_values(values)
         return value
+
+    @staticmethod
+    def create_mean(values : List[SmartMeterValues], user_specified_oh_item_names : Union[SmartMeterOhItemNames, None] = None) -> SmartMeterValues:
+        return SmartMeterValues.create_avg(values, mean, user_specified_oh_item_names)
     
     @staticmethod
-    def create_avg(values : List[SmartMeterValues], user_specified_oh_item_names : Union[SmartMeterOhItemNames, None] = None) -> SmartMeterValues:
+    def create_median(values : List[SmartMeterValues], user_specified_oh_item_names : Union[SmartMeterOhItemNames, None] = None) -> SmartMeterValues:
+        return SmartMeterValues.create_avg(values, median, user_specified_oh_item_names)
+    
+    @staticmethod
+    def create_avg(values : List[SmartMeterValues], operator : Callable[[List[float]], float], 
+                   user_specified_oh_item_names : Union[SmartMeterOhItemNames, None] = None ) -> SmartMeterValues:
         smart_meter_values=SmartMeterValues(None, None, None, None, None, user_specified_oh_item_names)
         phase_1_value_list = [value.phase_1_consumption.value for value in values if value.phase_1_consumption.value is not None]
         if phase_1_value_list: 
-            smart_meter_values.phase_1_consumption.value = mean(phase_1_value_list)
+            smart_meter_values.phase_1_consumption.value = operator(phase_1_value_list)
         phase_2_value_list = [value.phase_2_consumption.value for value in values if value.phase_2_consumption.value is not None]
         if phase_2_value_list: 
-            smart_meter_values.phase_2_consumption.value = mean(phase_2_value_list)
+            smart_meter_values.phase_2_consumption.value = operator(phase_2_value_list)
         phase_3_value_list = [value.phase_3_consumption.value for value in values if value.phase_3_consumption.value is not None]
         if phase_3_value_list: 
-            smart_meter_values.phase_3_consumption.value = mean(phase_3_value_list)
+            smart_meter_values.phase_3_consumption.value = operator(phase_3_value_list)
         overall_consumption_value_list = [value.overall_consumption.value for value in values if value.overall_consumption.value is not None]
         if overall_consumption_value_list: 
-            smart_meter_values.overall_consumption.value = mean(overall_consumption_value_list)
+            smart_meter_values.overall_consumption.value = operator(overall_consumption_value_list)
         electricity_meter_value_list = [value.electricity_meter.value for value in values if value.electricity_meter.value is not None]
         if electricity_meter_value_list: 
-            smart_meter_values.electricity_meter.value = mean(electricity_meter_value_list)
+            smart_meter_values.electricity_meter.value = operator(electricity_meter_value_list)
         return smart_meter_values
-    
+
     # NOTE: Use PersistenceValuesType as input to consider that the count of values can potentially be different per item.
     # This could be some data optimization in openhab or similar. Whatever the reason is, we have to support it.
     @staticmethod
     def check_if_updated(pers_values : PersistenceValuesType) -> bool:
         # no consumption is good and considered as updated.
         electricity_meter_values=SmartMeterValues.all_values_for_item(4, pers_values)
         if len(electricity_meter_values) > 1 and all(value == electricity_meter_values[0] for value in electricity_meter_values):
```

### Comparing `smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/openhab.py` & `smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/openhab.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 import requests
 import http
 import datetime
 from logging import Logger
 from requests.auth import HTTPBasicAuth
 from requests.adapters import HTTPAdapter, Retry
 from typing import List, Tuple
-from statistics import median
 from .interfaces import *
 
 # disable warnings about insecure requests because ssl verification is disabled
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
-def _get_median(list_values : List[List[float]]) -> SmartMeterValues:
-    smart_meter_values : List[OhItemAndValue] = []
-    value_index=0
-    for item in SmartMeterValues.oh_item_names():
-        if item:
-            avg_value = median(list_values[value_index]) if len(list_values[value_index]) > 1 else None
-            smart_meter_values.append(OhItemAndValue(item, avg_value))
-            value_index+=1
-    return SmartMeterValues.create(smart_meter_values)
-
 class OpenhabConnection():
     def __init__(self, oh_host : str, oh_user : str, oh_passwd : str, logger : Logger) -> None:
         self._oh_host=oh_host
         self._session=requests.Session()
         if oh_user:
             self._session.auth=HTTPBasicAuth(oh_user, oh_passwd)
         retries=Retry(total=8,
@@ -61,14 +50,16 @@
                     self._logger.warning("Caught Exception while getting from openHAB: " + str(e))
                 values.append(oh_item_value)
         return values
 
     def get_values_from_items(self) -> SmartMeterValues:
         return SmartMeterValues.create(self.get_item_value_list_from_items(SmartMeterValues.oh_item_names()))
 
+    # NOTE: This can potentially return values, although no new values have been posted. Depending on the config: 
+    # https://www.openhab.org/docs/configuration/persistence.html
     def _get_persistence_values(self, oh_item_names : Tuple[str, ...], start_time : datetime.datetime, end_time : datetime.datetime) -> PersistenceValuesType:
         pers_values = []
         for item in oh_item_names:
             if item:
                 values=[]
                 try:
                     with self._session.get(
@@ -87,14 +78,8 @@
     def check_if_persistence_values_updated(self, start_time : datetime.datetime, end_time : datetime.datetime) -> bool:
         pers_values=self._get_persistence_values(SmartMeterValues.oh_item_names(), start_time, end_time)
         updated=SmartMeterValues.check_if_updated(pers_values)
         if not updated:
             self._logger.warning("Persistence values have not been updated.")
             for index, values in enumerate(pers_values):
                 self._logger.warning(f"Values for index {index}: {values}")
-        return updated
-
-    def get_median_from_items(self, timedelta : datetime.timedelta = datetime.timedelta(minutes=30)) -> SmartMeterValues:
-        end_time=datetime.datetime.now()
-        start_time=end_time-timedelta
-        pers_values=self._get_persistence_values(SmartMeterValues.oh_item_names(), start_time, end_time)
-        return _get_median(pers_values)
+        return updated
```

### Comparing `smart_meter_to_openhab-0.5.1/smart_meter_to_openhab/sml_iskra_mt175.py` & `smart_meter_to_openhab-0.5.2/smart_meter_to_openhab/sml_iskra_mt175.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,83 @@
 import serial
 import os
 import logging
 from datetime import timedelta, datetime
 from logging import Logger
-from typing import List, Any, Optional
+from typing import List, Optional
 from pathlib import Path
 from time import sleep
 from abc import ABC, abstractmethod
 from .interfaces import SmartMeterValues
 
-MIN_REF_VALUE_IN_WATT=50
-def _has_outlier(value_list : List[Any], ref_value_list : List[Any]) -> bool:
-    for i in range(len(value_list)):
-        if value_list[i] is not None and ref_value_list[i] is not None and value_list[i]*0.001 > max(ref_value_list[i], MIN_REF_VALUE_IN_WATT):
-            return True
-    return False
-
 class SmartMeterReader(ABC):
+    _prev_avg_values : SmartMeterValues = SmartMeterValues()
+
     def __init__(self, logger : Logger, raw_data_dump_dir : Optional[Path] = None) -> None:
         self._logger=logger
         self._latest_raw_data=''
         self._raw_data_dump_dir=raw_data_dump_dir
         self._raw_data_dump_invalid_counter=0
-        self._raw_data_dump_outlier_counter=0
+        self._raw_data_dump_inconsistent_counter=0
         self._raw_data_dump_valid_counter=0
         if self._raw_data_dump_dir:
             os.makedirs(self._raw_data_dump_dir, exist_ok=True)
             self._logger.info(f"Using directory {self._raw_data_dump_dir} for raw data dumps.")
 
-    def read_avg(self, read_count : int, ref_values : SmartMeterValues = SmartMeterValues()) -> SmartMeterValues:
+    def read_avg(self, read_count : int) -> SmartMeterValues:
         """Read average data from the smart meter
 
         Parameters
         ----------
         read_count : int
             specifies the number of performed reads that are averaged. Between each read is a sleep of 1 sec
-        ref_values : SmartMeterValues
-            Values that are used as baseline. If a new read value is 100 times higher as the given reference value, 
-            it is considered as outlier and will be ignored.
             
         Returns
         -------
         SmartMeterValues
             Contains the data read from the smart meter
         """
         all_values : List[SmartMeterValues] = []
         for i in range(read_count):
-            values=self.read(ref_values)
-            if values.is_valid():
-                 all_values.append(values)
+            all_values.append(self._read_raw())
             sleep(1)
-        if len(all_values) < read_count:
-            self._logger.warning(f"Expected {read_count} valid values but only received {len(all_values)}. Returning average value anyway.")
-        return SmartMeterValues.create_avg(all_values)
-
-    def read(self, ref_values : SmartMeterValues) -> SmartMeterValues:
-        """Read data from the smart meter and try to validate them
-
-        Parameters
-        ----------
-        ref_values : SmartMeterValues
-            Values that are used as baseline to detect outliers
-        
-        Returns
-        -------
-        SmartMeterValues
-            Contains the data read from the smart meter
-        """
-        ref_value_list=ref_values.value_list()
-        values=self._read_raw()
-        if values.is_invalid():
-            self._logger.info(f"Detected invalid values during read. Trying again")
-            if self._raw_data_dump_dir:
-                with open(self._raw_data_dump_dir / f"raw_data_dump_invalid_{self._raw_data_dump_invalid_counter}.sml", 'w') as f:
-                    f.write(self._latest_raw_data)
-                self._raw_data_dump_invalid_counter+=1
-        value_list=values.value_list()
-        if _has_outlier(value_list, ref_value_list):
-            self._logger.info(f"Detected unrealistic values during read. Trying again")
-            if self._raw_data_dump_dir:
-                with open(self._raw_data_dump_dir / f"raw_data_dump_outlier_{self._raw_data_dump_outlier_counter}.sml", 'w') as f:
-                    f.write(self._latest_raw_data)
-                self._raw_data_dump_outlier_counter+=1
-
-        if values.is_invalid() or _has_outlier(value_list, ref_value_list):
-            self._logger.warning(f"Unable to read and validate data. Ignoring following values: {values}")
-            values.reset()
-
-        if self._raw_data_dump_dir and self._logger.level == logging.DEBUG and values.is_valid():
-            with open(self._raw_data_dump_dir / f"raw_data_dump_valid_{self._raw_data_dump_valid_counter}.sml", 'w') as f:
-                f.write(self._latest_raw_data)
-            self._raw_data_dump_valid_counter+=1
 
-        return values
+        good_values : List[SmartMeterValues] = []
+        for values in all_values:
+            if values.is_invalid():
+                self._logger.warning(f"Detected invalid values during read. Ignoring following values: {values}")
+                if self._raw_data_dump_dir:
+                    with open(self._raw_data_dump_dir / f"raw_data_dump_invalid_{self._raw_data_dump_invalid_counter}.sml", 'w') as f:
+                        f.write(self._latest_raw_data)
+                    self._raw_data_dump_invalid_counter+=1
+            elif values.is_inconsistent(SmartMeterReader._prev_avg_values):
+                self._logger.warning(f"Detected inconsistent values during read. Ignoring following values: {values}")
+                if self._raw_data_dump_dir:
+                    with open(self._raw_data_dump_dir / f"raw_data_dump_inconsistent_{self._raw_data_dump_inconsistent_counter}.sml", 'w') as f:
+                        f.write(self._latest_raw_data)
+                    self._raw_data_dump_inconsistent_counter+=1
+            else:
+                if self._raw_data_dump_dir and self._logger.level == logging.DEBUG:
+                    with open(self._raw_data_dump_dir / f"raw_data_dump_valid_{self._raw_data_dump_valid_counter}.sml", 'w') as f:
+                        f.write(self._latest_raw_data)
+                    self._raw_data_dump_valid_counter+=1
+                good_values.append(values)
+
+        if len(good_values) < read_count:
+            self._logger.warning(f"Expected {read_count} valid values but only received {len(good_values)}. Returning average value anyway.")
+
+        if SmartMeterReader._prev_avg_values.is_invalid():
+            # Creating initial previous values. Implication: Consistency check (above) always returns True. 
+            # In this case it is best to return the median. This should most likely ignore possible inconsistent outlier in the first run (call of this method).
+            avg_value=SmartMeterValues.create_median(good_values)
+        else:
+            # When having a valid previous value, it is better to return the mean value since the inconsistent outliers have been removed already.
+            avg_value=SmartMeterValues.create_mean(good_values)
+        SmartMeterReader._prev_avg_values=avg_value
+        return avg_value
 
     @abstractmethod
     def _read_raw(self) -> SmartMeterValues:
         pass
 
 # supporting OBIS code 1.8.0 only
 def _decode_sml_iskra_mt175_one_way(raw_data : str) -> SmartMeterValues:
```

### Comparing `smart_meter_to_openhab-0.5.1/smart_meter_to_openhab_scripts/main.py` & `smart_meter_to_openhab-0.5.2/smart_meter_to_openhab_scripts/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,60 +45,64 @@
 
 def _exec_process(params : List[str]) -> None:
     result = subprocess.run(params, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     rc=result.returncode
     if rc != 0:
         raise Exception("Failed to execute command "+ ' '.join(params)+". Return code was: "+str(result.returncode))
 
-def _run(logger : logging.Logger, read_count : int, raw_data_dump_dir : Union[Path, None] = None) -> None:
+def _run(logger : logging.Logger, read_count : int, uhubctl : bool, raw_data_dump_dir : Union[Path, None] = None) -> None:
     from smart_meter_to_openhab.openhab import OpenhabConnection
     from smart_meter_to_openhab.sml_iskra_mt175 import SmlIskraMt175OneWay
     from smart_meter_to_openhab.utils import manage_rolling_list
 
     oh_user=os.getenv('OH_USER') if 'OH_USER' in os.environ else ''
     oh_passwd=os.getenv('OH_PASSWD') if 'OH_PASSWD' in os.environ else ''
     oh_connection = OpenhabConnection(os.getenv('OH_HOST'), oh_user, oh_passwd, logger) # type: ignore
     sml_iskra = SmlIskraMt175OneWay('/dev/ttyUSB0', logger, raw_data_dump_dir)
     logger.info("Connections established. Starting to transfer smart meter values to openhab.")
     desired_number_of_persistence_values=6
+    invalid_reads_in_a_row=0
     datetimes_before_post_to_oh : List[datetime] =[]
     while True:
         logger.info("Reading SML data")
-        ref_smart_meter_value=oh_connection.get_median_from_items()
-        values=sml_iskra.read_avg(read_count, ref_values=ref_smart_meter_value)
+        values=sml_iskra.read_avg(read_count)
+        invalid_reads_in_a_row = invalid_reads_in_a_row+1 if values.is_invalid() else 0
         logger.info(f"current values: {values}")
         datetimes_before_post_to_oh=manage_rolling_list(datetimes_before_post_to_oh, desired_number_of_persistence_values, datetime.now())
         oh_connection.post_to_items(values)
         logger.info("Values posted to openHAB")
+        if invalid_reads_in_a_row == desired_number_of_persistence_values:
+            logger.error(f"Reading values from smart meter failed {invalid_reads_in_a_row} times in a row.")
+            if uhubctl:
+                logger.error("Power off and on usb ports and exiting process")
+                # TODO: sudo reboot seems to help a lot more. But lets try this first
+                _exec_process(["sudo", "uhubctl", "-a", "cycle", "-d", "10", "-p", "1-5"])
+            else:
+                logger.error("Exiting process")
+            break
         if len(datetimes_before_post_to_oh) == desired_number_of_persistence_values:
             # NOTE: exclude the latest values since oh sometimes has not handled the post requests from above yet.
             if not oh_connection.check_if_persistence_values_updated(start_time=datetimes_before_post_to_oh[0], 
                                                                      end_time=datetimes_before_post_to_oh[-1]):
+                logger.error("openHAB items ping NOT successful.")
                 break
             logger.info("openHAB items ping successful.")
 
 def main() -> None:
     parser=create_args_parser()
     args = parser.parse_args()
     if args.dotenv_path:
         load_dotenv(dotenv_path=args.dotenv_path)
     logger=create_logger(args.logfile)
     logger.setLevel(logging.INFO)
     logger.info(f"Starting smart_meter_to_openhab version {__version__}")
     logger.setLevel(log_level_from_arg(args.verbose))
     try:
         raw_data_dump_dir=args.raw_data_dump_dir if args.raw_data_dump_dir else None
-        _run(logger, args.smart_meter_read_count, raw_data_dump_dir)
-
-        if args.uhubctl:
-            logger.error("openHAB items seem to have not been updated - Power off and on usb ports and exiting process")
-            # TODO: sudo reboot seems to help a lot more. But lets try this first
-            _exec_process(["sudo", "uhubctl", "-a", "cycle", "-d", "10", "-p", "1-5"])
-        else:
-            logger.error("openHAB items seem to have not been updated - exiting process")
+        _run(logger, args.smart_meter_read_count, args.uhubctl, raw_data_dump_dir)
     except Exception as e:
         logger.exception("Caught Exception: " + str(e))
     except:
         logger.exception("Caught unknow exception")
 
     logger.error("Unable to upload valid data to openHAB. Exiting Process with Return Code 1.")
     sys.exit(1)
```

### Comparing `smart_meter_to_openhab-0.5.1/PKG-INFO` & `smart_meter_to_openhab-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_meter_to_openhab
-Version: 0.5.1
+Version: 0.5.2
 Summary: Pushing data of ISKRA MT175 smart meter to openhab
 Home-page: https://github.com/die-bauerei/smart-meter-to-openhab
 Author: Heiko Bauer
 Author-email: heiko_bauer@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

