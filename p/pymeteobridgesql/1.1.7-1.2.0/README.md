# Comparing `tmp/pymeteobridgesql-1.1.7.tar.gz` & `tmp/pymeteobridgesql-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeteobridgesql-1.1.7.tar", last modified: Sat Apr 27 13:58:11 2024, max compression
+gzip compressed data, was "pymeteobridgesql-1.2.0.tar", last modified: Mon Apr 29 13:10:23 2024, max compression
```

## Comparing `pymeteobridgesql-1.1.7.tar` & `pymeteobridgesql-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:11.673203 pymeteobridgesql-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-27 13:58:07.000000 pymeteobridgesql-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-27 13:58:11.673203 pymeteobridgesql-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-27 13:58:07.000000 pymeteobridgesql-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:11.673203 pymeteobridgesql-1.1.7/pymeteobridgesql/
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-27 13:58:07.000000 pymeteobridgesql-1.1.7/pymeteobridgesql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-27 13:58:07.000000 pymeteobridgesql-1.1.7/pymeteobridgesql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10541 2024-04-27 13:58:07.000000 pymeteobridgesql-1.1.7/pymeteobridgesql/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 13:58:11.673203 pymeteobridgesql-1.1.7/pymeteobridgesql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-27 13:58:11.000000 pymeteobridgesql-1.1.7/pymeteobridgesql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-27 13:58:11.000000 pymeteobridgesql-1.1.7/pymeteobridgesql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 13:58:11.000000 pymeteobridgesql-1.1.7/pymeteobridgesql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 13:58:11.000000 pymeteobridgesql-1.1.7/pymeteobridgesql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 13:58:11.673203 pymeteobridgesql-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-27 13:58:07.000000 pymeteobridgesql-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/pymeteobridgesql/
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/pymeteobridgesql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/pymeteobridgesql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/pymeteobridgesql/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-29 13:10:23.000000 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-29 13:10:23.000000 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:10:23.000000 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 13:10:23.000000 pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:10:23.359673 pymeteobridgesql-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-29 13:10:19.000000 pymeteobridgesql-1.2.0/setup.py
```

### Comparing `pymeteobridgesql-1.1.7/LICENSE` & `pymeteobridgesql-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeteobridgesql-1.1.7/PKG-INFO` & `pymeteobridgesql-1.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.1.7
+Version: 1.2.0
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.1.7/pymeteobridgesql/api.py` & `pymeteobridgesql-1.2.0/pymeteobridgesql/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains the code to get weather data from an MYSQL Table."""
 from __future__ import annotations
 
 import logging
 import mysql.connector
 
-from .data import ForecastDaily, ForecastHourly, RealtimeData, StationData
+from .data import ForecastDaily, ForecastHourly, MinuteData, MonthlyData, RealtimeData, StationData
 
 _LOGGER = logging.getLogger(__name__)
 
 class MeteobridgeSQLDatabaseConnectionError(Exception):
     """Cannot connect to database."""
 
 
@@ -109,7 +109,40 @@
                 for row in result:
                     result_array.append(ForecastDaily(*row))
             except mysql.connector.Error as err:
                 raise MeteobridgeSQLDataError(f"Failed to lookup daily forecast in the database: {err.msg}")
 
         return result_array
 
+
+    async def async_get_minute_data(self, interval: str = '24') -> any:
+        """Get data from the Minute Data table."""
+
+        result_array = []
+        try:
+            self._weather_cursor.execute(
+                f"SELECT * FROM minute_data WHERE `logdate` > NOW() - INTERVAL {interval} HOUR;"
+            )
+            result = self._weather_cursor.fetchall()
+            for row in result:
+                result_array.append(MinuteData(*row))
+        except mysql.connector.Error as err:
+            raise MeteobridgeSQLDataError(f"Failed to lookup data from the minute_data table in the database: {err.msg}")
+
+        return result_array
+
+    async def async_get_monthly_data(self, interval: str = '1') -> any:
+        """Get data from the Monthly Data table."""
+
+        result_array = []
+        try:
+            self._weather_cursor.execute(
+                f"SELECT * FROM monthly_data WHERE `logdate` > NOW() - INTERVAL {interval} YEAR;"
+            )
+            result = self._weather_cursor.fetchall()
+            for row in result:
+                result_array.append(MonthlyData(*row))
+        except mysql.connector.Error as err:
+            raise MeteobridgeSQLDataError(f"Failed to lookup data from the monthly_data table in the database: {err.msg}")
+
+        return result_array
+
```

### Comparing `pymeteobridgesql-1.1.7/pymeteobridgesql/data.py` & `pymeteobridgesql-1.2.0/pymeteobridgesql/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -302,14 +302,95 @@
     mb_ip: str
     mb_swversion: str
     mb_buildnum: str
     mb_platform: str
     mb_station: str
     mb_stationname: str
 
+
+@dataclass(frozen=True)
+class MinuteData:
+    logdate: datetime.datetime
+    temperature: float
+    wind_chill: float
+    air_Quality_pm1: float
+    air_Quality_pm10: float
+    air_Quality_pm25: float
+    heat_index: float
+    humidity: int
+    dewpoint: float
+    rain_rate: float
+    rain_day: float
+    wind_speed: float
+    wind_gust: float
+    wind_bearing: int
+    pressure: float
+    pressure_trend: float
+    uv: float
+    solar_radiation: float
+
+    def to_dict(self):
+        return {
+            "logdate": self.logdate,
+            "temperature": self.temperature,
+            "wind_chill": self.wind_chill,
+            "air_Quality_pm1": self.air_Quality_pm1,
+            "air_Quality_pm10": self.air_Quality_pm10,
+            "air_Quality_pm25": self.air_Quality_pm25,
+            "heat_index": self.heat_index,
+            "humidity": self.humidity,
+            "dewpoint": self.dewpoint,
+            "rain_rate": self.rain_rate,
+            "rain_day": self.rain_day,
+            "wind_speed": self.wind_speed,
+            "wind_gust": self.wind_gust,
+            "wind_bearing": self.wind_bearing,
+            "pressure": self.pressure,
+            "pressure_trend": self.pressure_trend,
+            "uv": self.uv,
+            "solar_radiation": self.solar_radiation,
+        }
+
+@dataclass(frozen=True)
+class MonthlyData:
+    logdate: datetime.date
+    temperature_low: float
+    temperature_high: float
+    humidity_low: int
+    humidity_high: int
+    rain_total: float
+    wind_speed_max: float
+    wind_speed_avg: float
+    wind_direction_avg: int
+    uvindex_max: float
+    solar_radiation_max: float
+    pressure_low: float
+    pressure_high: float
+    air_quality_low: float
+    air_quality_high: float
+
+    def to_dict(self):
+        return {
+            "logdate": self.logdate,
+            "temperature_low": self.temperature_low,
+            "temperature_high": self.temperature_high,
+            "humidity_low": self.humidity_low,
+            "humidity_high": self.humidity_high,
+            "rain_total": self.rain_total,
+            "wind_speed_max": self.wind_speed_max,
+            "wind_speed_avg": self.wind_speed_avg,
+            "wind_direction_avg": self.wind_direction_avg,
+            "uvindex_max": self.uvindex_max,
+            "solar_radiation_max": self.solar_radiation_max,
+            "pressure_low": self.pressure_low,
+            "pressure_high": self.pressure_high,
+            "air_quality_low": self.air_quality_low,
+            "air_quality_high": self.air_quality_high,
+        }
+
 def aqi_from_pm25(pm25: float) -> int:
     """Calculate the Air Quality Index from the PM2.5 value."""
     if pm25 is None:
         return None
 
     if pm25 > 500:
         return 500
@@ -338,8 +419,7 @@
         return None
 
     _val1 = (ih - il)
     _val2 = (bph - bpl)
     _val3 = (pm25 - bpl)
     return float(_val1 / _val2 * _val3 + il)
 
-
```

### Comparing `pymeteobridgesql-1.1.7/pymeteobridgesql.egg-info/PKG-INFO` & `pymeteobridgesql-1.2.0/pymeteobridgesql.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeteobridgesql
-Version: 1.1.7
+Version: 1.2.0
 Summary: Gets weather data from a MySQL table
 Home-page: https://github.com/briis/pymeteobridgesql
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymeteobridgesql-1.1.7/setup.py` & `pymeteobridgesql-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymeteobridgesql",
-    version="1.1.7",
+    version="1.2.0",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets weather data from a MySQL table",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pymeteobridgesql",
```

