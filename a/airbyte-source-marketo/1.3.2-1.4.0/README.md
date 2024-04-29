# Comparing `tmp/airbyte_source_marketo-1.3.2.tar.gz` & `tmp/airbyte_source_marketo-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_marketo-1.3.2.tar", max compression
+gzip compressed data, was "airbyte_source_marketo-1.4.0.tar", max compression
```

## Comparing `airbyte_source_marketo-1.3.2.tar` & `airbyte_source_marketo-1.4.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     4514 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/README.md
--rw-r--r--   0        0        0      776 2024-04-24 19:29:40.282623 airbyte_source_marketo-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     1171 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/__init__.py
--rw-r--r--   0        0        0      233 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/run.py
--rw-r--r--   0        0        0     1542 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/activity_types.json
--rw-r--r--   0        0        0     1471 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/campaigns.json
--rw-r--r--   0        0        0    11717 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/leads.json
--rw-r--r--   0        0        0     1158 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/lists.json
--rw-r--r--   0        0        0     2254 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/programs.json
--rw-r--r--   0        0        0     1620 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/schemas/segmentations.json
--rw-r--r--   0        0        0    23327 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/source.py
--rw-r--r--   0        0        0     1803 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/spec.json
--rw-r--r--   0        0        0     2069 2024-04-24 19:26:18.579111 airbyte_source_marketo-1.3.2/source_marketo/utils.py
--rw-r--r--   0        0        0     5220 1970-01-01 00:00:00.000000 airbyte_source_marketo-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/README.md
+-rw-r--r--   0        0        0      772 2024-04-29 18:17:32.035382 airbyte_source_marketo-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1171 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/__init__.py
+-rw-r--r--   0        0        0     5854 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/manifest.yaml
+-rw-r--r--   0        0        0      233 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/run.py
+-rw-r--r--   0        0        0     1542 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/activity_types.json
+-rw-r--r--   0        0        0     1471 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/campaigns.json
+-rw-r--r--   0        0        0    11717 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/leads.json
+-rw-r--r--   0        0        0     1158 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/lists.json
+-rw-r--r--   0        0        0     2254 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/programs.json
+-rw-r--r--   0        0        0     1620 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/schemas/segmentations.json
+-rw-r--r--   0        0        0    19219 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/source.py
+-rw-r--r--   0        0        0     1803 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/spec.json
+-rw-r--r--   0        0        0     2069 2024-04-29 17:04:46.000000 airbyte_source_marketo-1.4.0/source_marketo/utils.py
+-rw-r--r--   0        0        0     5223 1970-01-01 00:00:00.000000 airbyte_source_marketo-1.4.0/PKG-INFO
```

### Comparing `airbyte_source_marketo-1.3.2/README.md` & `airbyte_source_marketo-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-marketo spec
 poetry run source-marketo check --config secrets/config.json
 poetry run source-marketo discover --config secrets/config.json
-poetry run source-marketo read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-marketo read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

### Comparing `airbyte_source_marketo-1.3.2/pyproject.toml` & `airbyte_source_marketo-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.3.2"
+version = "1.4.0"
 name = "airbyte-source-marketo"
 description = "Source implementation for Marketo."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_marketo" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "0.80.0"
+airbyte-cdk = "^0"
 
 [tool.poetry.scripts]
 source-marketo = "source_marketo.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.1"
 requests-mock = "^1.11.0"
```

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/__init__.py` & `airbyte_source_marketo-1.4.0/source_marketo/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/schemas/activity_types.json` & `airbyte_source_marketo-1.4.0/source_marketo/schemas/activity_types.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/schemas/campaigns.json` & `airbyte_source_marketo-1.4.0/source_marketo/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/schemas/leads.json` & `airbyte_source_marketo-1.4.0/source_marketo/schemas/leads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/schemas/lists.json` & `airbyte_source_marketo-1.4.0/source_marketo/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/schemas/programs.json` & `airbyte_source_marketo-1.4.0/source_marketo/schemas/programs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/schemas/segmentations.json` & `airbyte_source_marketo-1.4.0/source_marketo/schemas/segmentations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/source.py` & `airbyte_source_marketo-1.4.0/source_marketo/source.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 import csv
-import datetime
 import json
 import re
 from abc import ABC
 from time import sleep
 from typing import Any, Iterable, List, Mapping, MutableMapping, Optional, Tuple
 
 import pendulum
 import requests
 from airbyte_cdk.models import SyncMode
-from airbyte_cdk.sources import AbstractSource
+from airbyte_cdk.sources.declarative.exceptions import ReadException
+from airbyte_cdk.sources.declarative.yaml_declarative_source import YamlDeclarativeSource
 from airbyte_cdk.sources.streams import Stream
 from airbyte_cdk.sources.streams.availability_strategy import AvailabilityStrategy
 from airbyte_cdk.sources.streams.http import HttpStream
 from airbyte_cdk.sources.streams.http.auth import Oauth2Authenticator
 from airbyte_cdk.utils import AirbyteTracedException
 from airbyte_protocol.models import FailureType
 
@@ -130,30 +130,25 @@
 
         # use the lowest date between start_date and self.end_date, otherwise API fails if start_date is in future
         start_date = min(start_date, pendulum.now())
         date_slices = []
 
         end_date = pendulum.parse(self.end_date) if self.end_date else pendulum.now()
         while start_date < end_date:
-            # the amount of days for each data-chunk begining from start_date
+            # the amount of days for each data-chunk beginning from start_date
             end_date_slice = start_date.add(days=self.window_in_days)
 
             date_slice = {"startAt": to_datetime_str(start_date), "endAt": to_datetime_str(end_date_slice)}
 
             date_slices.append(date_slice)
             start_date = end_date_slice
 
         return date_slices
 
 
-class SemiIncrementalMarketoStream(IncrementalMarketoStream):
-    def stream_slices(self, sync_mode, stream_state: Mapping[str, Any] = None, **kwargs) -> Iterable[Optional[MutableMapping[str, any]]]:
-        return [None]
-
-
 class MarketoExportBase(IncrementalMarketoStream):
     """
     Base class for all the streams which support bulk extract.
     """
 
     # Polling Job Status - https://developers.marketo.com/rest-api/bulk-extract/bulk-lead-extract/
     # The status is only updated once every 60 seconds
@@ -439,126 +434,14 @@
             "additionalProperties": True,
             "properties": properties,
         }
 
         return schema
 
 
-class ActivityTypes(MarketoStream):
-    """
-    Return list of all activity types.
-    API Docs: https://developers.marketo.com/rest-api/lead-database/activities/#describe
-    """
-
-    def path(self, stream_slice: Mapping[str, Any] = None, **kwargs) -> str:
-        return "rest/v1/activities/types.json"
-
-
-class Programs(IncrementalMarketoStream):
-    """
-    Return list of all programs.
-    API Docs: https://developers.marketo.com/rest-api/assets/programs/#by_date_range
-    """
-
-    cursor_field = "updatedAt"
-    page_size = 200
-
-    def __init__(self, config: Mapping[str, Any]):
-        super().__init__(config)
-        self.offset = 0
-
-    def path(self, **kwargs) -> str:
-        return f"rest/asset/v1/{self.name}.json"
-
-    def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
-        data = response.json().get(self.data_field)
-
-        if data:
-            self.offset += self.page_size + 1
-            return {"offset": self.offset}
-
-    def request_params(
-        self,
-        stream_state: Mapping[str, Any],
-        stream_slice: Mapping[str, Any] = None,
-        next_page_token: Mapping[str, Any] = None,
-    ) -> MutableMapping[str, Any]:
-        """
-        Programs are queryable via their updatedAt time but require and
-        end date as well. As there is no max time range for the query,
-        query from the bookmark value until current.
-        """
-
-        params = super().request_params(next_page_token, stream_state=stream_state, stream_slice=stream_slice)
-        params.update(
-            {
-                "maxReturn": self.page_size,
-                "earliestUpdatedAt": stream_slice["startAt"],
-                "latestUpdatedAt": stream_slice["endAt"],
-            }
-        )
-
-        return params
-
-    def normalize_datetime(self, dt: str, format="%Y-%m-%dT%H:%M:%SZ%z"):
-        """
-        Convert '2018-09-07T17:37:18Z+0000' -> '2018-09-07T17:37:18Z'
-        """
-        try:
-            res = datetime.datetime.strptime(dt, format)
-        except ValueError:
-            self.logger.warning("date-time field in unexpected format: '%s'", dt)
-            return dt
-        return to_datetime_str(res)
-
-    def parse_response(self, response: requests.Response, stream_state: Mapping[str, Any], **kwargs) -> Iterable[MutableMapping]:
-        for record in super().parse_response(response, stream_state, **kwargs):
-            # delete +00:00 part from the end of createdAt and updatedAt
-            record["updatedAt"] = self.normalize_datetime(record["updatedAt"])
-            record["createdAt"] = self.normalize_datetime(record["createdAt"])
-            yield record
-
-
-class Campaigns(SemiIncrementalMarketoStream):
-    """
-    Return list of all campaigns.
-    API Docs: https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Campaigns/getCampaignsUsingGET
-    """
-
-
-class Lists(SemiIncrementalMarketoStream):
-    """
-    Return list of all lists.
-    API Docs: https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Static_Lists/getListsUsingGET
-    """
-
-
-class Segmentations(MarketoStream):
-    """
-    This stream is similar to Programs but don't support to filter using created or update at parameters
-    API Docs: https://developers.marketo.com/rest-api/endpoint-reference/asset-endpoint-reference/#!/Segments/getSegmentationUsingGET
-    """
-
-    page_size = 200
-    offset = 0
-
-    def __init__(self, config: Mapping[str, Any]):
-        super().__init__(config)
-
-    def path(self, **kwargs) -> str:
-        return "rest/asset/v1/segmentation.json"
-
-    def next_page_token(self, response: requests.Response) -> Optional[Mapping[str, Any]]:
-        data = response.json().get(self.data_field)
-
-        if data:
-            self.offset += self.page_size + 1
-            return {"offset": self.offset}
-
-
 class MarketoAuthenticator(Oauth2Authenticator):
     def __init__(self, config):
         super().__init__(
             token_refresh_endpoint=f"{config['domain_url']}/identity/oauth/token",
             client_id=config["client_id"],
             client_secret=config["client_secret"],
             refresh_token=None,
@@ -582,45 +465,38 @@
             response.raise_for_status()
             response_json = response.json()
             return response_json["access_token"], response_json["expires_in"]
         except Exception as e:
             raise Exception(f"Error while refreshing access token: {e}") from e
 
 
-class SourceMarketo(AbstractSource):
+class SourceMarketo(YamlDeclarativeSource):
     """
-    Source Marketo fetch data of personalized multi-channel programs and campaigns to prospects and customers.
+    Source Marketo fetch data of personalized multichannel programs and campaigns to prospects and customers.
     """
 
-    def check_connection(self, logger, config) -> Tuple[bool, any]:
-        """
-        Testing connection availability for the connector by granting the credentials.
-        """
-
-        try:
-            url = f"{config['domain_url']}/rest/v1/leads/describe"
-
-            authenticator = MarketoAuthenticator(config)
+    def __init__(self) -> None:
+        super().__init__(**{"path_to_yaml": "manifest.yaml"})
 
-            session = requests.get(url, headers=authenticator.get_auth_header())
-            session.raise_for_status()
-
-            return True, None
-        except requests.exceptions.RequestException as e:
-            return False, repr(e)
+    def _get_declarative_streams(self, config: Mapping[str, Any]) -> List[Stream]:
+        return super().streams(config)
 
     def streams(self, config: Mapping[str, Any]) -> List[Stream]:
         config["authenticator"] = MarketoAuthenticator(config)
 
-        streams = [ActivityTypes(config), Segmentations(config), Campaigns(config), Leads(config), Lists(config), Programs(config)]
-
-        # create dynamically activities by activity type id
-        for activity in ActivityTypes(config).read_records(sync_mode=None):
-            stream_name = f"activities_{clean_string(activity['name'])}"
+        streams = self._get_declarative_streams(config)
+        streams.append(Leads(config))
+        activity_types_stream = [stream for stream in streams if stream.name == "activity_types"][0]
 
-            stream_class = type(stream_name, (Activities,), {"activity": activity})
-
-            # instantiate a stream with config
-            stream_instance = stream_class(config)
-            streams.append(stream_instance)
+        # dynamically create activities by activity type id
+        try:
+            for activity in activity_types_stream.read_records(sync_mode=None):
+                stream_name = f"activities_{clean_string(activity['name'])}"
+                stream_class = type(stream_name, (Activities,), {"activity": activity})
+
+                # instantiate a stream with config
+                stream_instance = stream_class(config)
+                streams.append(stream_instance)
+        except ReadException as e:
+            self.logger.warning(f"An error occurred while creating activity streams: {repr(e)}")
 
         return streams
```

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/spec.json` & `airbyte_source_marketo-1.4.0/source_marketo/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/source_marketo/utils.py` & `airbyte_source_marketo-1.4.0/source_marketo/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_marketo-1.3.2/PKG-INFO` & `airbyte_source_marketo-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-marketo
-Version: 1.3.2
+Version: 1.4.0
 Summary: Source implementation for Marketo.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.80.0)
+Requires-Dist: airbyte-cdk (>=0,<1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/marketo
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Marketo source connector
 
 
@@ -45,15 +45,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-marketo spec
 poetry run source-marketo check --config secrets/config.json
 poetry run source-marketo discover --config secrets/config.json
-poetry run source-marketo read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-marketo read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

