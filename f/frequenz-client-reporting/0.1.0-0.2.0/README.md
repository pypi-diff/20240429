# Comparing `tmp/frequenz-client-reporting-0.1.0.tar.gz` & `tmp/frequenz-client-reporting-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-client-reporting-0.1.0.tar", last modified: Fri Apr 12 14:04:06 2024, max compression
+gzip compressed data, was "frequenz-client-reporting-0.2.0.tar", last modified: Mon Apr 29 14:30:54 2024, max compression
```

## Comparing `frequenz-client-reporting-0.1.0.tar` & `frequenz-client-reporting-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:06.109189 frequenz-client-reporting-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-12 14:04:06.105189 frequenz-client-reporting-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:06.105189 frequenz-client-reporting-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/examples/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5431 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:04:06.109189 frequenz-client-reporting-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:06.105189 frequenz-client-reporting-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:06.105189 frequenz-client-reporting-0.1.0/src/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:06.105189 frequenz-client-reporting-0.1.0/src/frequenz/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:06.105189 frequenz-client-reporting-0.1.0/src/frequenz/client/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/src/frequenz/client/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9732 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/src/frequenz/client/reporting/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/src/frequenz/client/reporting/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 14:03:58.000000 frequenz-client-reporting-0.1.0/src/frequenz/client/reporting/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:04:06.105189 frequenz-client-reporting-0.1.0/src/frequenz_client_reporting.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-12 14:04:06.000000 frequenz-client-reporting-0.1.0/src/frequenz_client_reporting.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-12 14:04:06.000000 frequenz-client-reporting-0.1.0/src/frequenz_client_reporting.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:04:06.000000 frequenz-client-reporting-0.1.0/src/frequenz_client_reporting.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-12 14:04:06.000000 frequenz-client-reporting-0.1.0/src/frequenz_client_reporting.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 14:04:06.000000 frequenz-client-reporting-0.1.0/src/frequenz_client_reporting.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/examples/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.808779 frequenz-client-reporting-0.2.0/src/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.808779 frequenz-client-reporting-0.2.0/src/frequenz/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11327 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:47.000000 frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:30:54.812779 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 14:30:54.000000 frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/top_level.txt
```

### Comparing `frequenz-client-reporting-0.1.0/LICENSE` & `frequenz-client-reporting-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-client-reporting-0.1.0/PKG-INFO` & `frequenz-client-reporting-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-reporting
-Version: 0.1.0
+Version: 0.2.0
 Summary: Reporting API client for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-reporting-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-reporting-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-reporting-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-reporting-python
@@ -36,16 +36,14 @@
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-client-reporting)](https://pypi.org/project/frequenz-client-reporting/)
 [![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-client-reporting-python/)
 
 ## Introduction
 
 Reporting API client for Python
 
-TODO(cookiecutter): Improve the README file
-
 ## Supported Platforms
 
 The following platforms are officially supported (tested):
 
 - **Python:** 3.11
 - **Operating System:** Ubuntu Linux 20.04
 - **Architectures:** amd64, arm64
```

### Comparing `frequenz-client-reporting-0.1.0/README.md` & `frequenz-client-reporting-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-client-reporting)](https://pypi.org/project/frequenz-client-reporting/)
 [![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-client-reporting-python/)
 
 ## Introduction
 
 Reporting API client for Python
 
-TODO(cookiecutter): Improve the README file
-
 ## Supported Platforms
 
 The following platforms are officially supported (tested):
 
 - **Python:** 3.11
 - **Operating System:** Ubuntu Linux 20.04
 - **Architectures:** amd64, arm64
```

### Comparing `frequenz-client-reporting-0.1.0/examples/client.py` & `frequenz-client-reporting-0.2.0/examples/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 from pprint import pprint
 from typing import AsyncIterator
 
 import pandas as pd
 from frequenz.client.common.metric import Metric
 
-from frequenz.client.reporting import ReportingClient
+from frequenz.client.reporting import ReportingApiClient
 
 # Experimental import
 from frequenz.client.reporting._client import MetricSample
 
 
 def main() -> None:
     """Parse arguments and run the client."""
@@ -75,42 +75,42 @@
     metric_names: list[str],
     start_dt: datetime,
     end_dt: datetime,
     page_size: int,
     service_address: str,
     display: str,
 ) -> None:
-    """Test the ReportingClient.
+    """Test the ReportingApiClient.
 
     Args:
         microgrid_id: microgrid ID
         component_id: component ID
         metric_names: list of metric names
         start_dt: start datetime
         end_dt: end datetime
         page_size: page size
         service_address: service address
         display: display format
 
     Raises:
         ValueError: if display format is invalid
     """
-    client = ReportingClient(service_address)
+    client = ReportingApiClient(service_address)
 
     metrics = [Metric[mn] for mn in metric_names]
 
     def data_iter() -> AsyncIterator[MetricSample]:
         """Iterate over single metric.
 
         Just a wrapper around the client method for readability.
 
         Returns:
             Iterator over single metric samples
         """
-        return client.iterate_single_component(
+        return client.list_single_component_data(
             microgrid_id=microgrid_id,
             component_id=component_id,
             metrics=metrics,
             start_dt=start_dt,
             end_dt=end_dt,
             page_size=page_size,
         )
```

### Comparing `frequenz-client-reporting-0.1.0/pyproject.toml` & `frequenz-client-reporting-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,35 @@
 
 [project]
 name = "frequenz-client-reporting"
 description = "Reporting API client for Python"
 readme = "README.md"
 license = { text = "MIT" }
 keywords = ["frequenz", "python", "lib", "library", "client-reporting", "client", "reporting", "api"]
-# TODO(cookiecutter): Remove and add more classifiers if appropriate
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Software Development :: Libraries",
   "Typing :: Typed",
 ]
 requires-python = ">= 3.11, < 4"
-# TODO(cookiecutter): Remove and add more dependencies if appropriate
 dependencies = [
   "typing-extensions >= 4.5.0, < 5",
-  "frequenz-api-reporting >= 0.1.1, < 1",
+  "frequenz-api-reporting >= 0.1.1, < 0.2",
   "frequenz-client-common == 0.1.0",
 ]
 dynamic = ["version"]
 
 [[project.authors]]
 name = "Frequenz Energy-as-a-Service GmbH"
 email = "floss@frequenz.com"
 
-# TODO(cookiecutter): Remove and add more optional dependencies if appropriate
 [project.optional-dependencies]
 dev-flake8 = [
   "flake8 == 6.1.0",
   "flake8-docstrings == 1.7.0",
   "flake8-pyproject == 1.2.3",  # For reading the flake8 config from pyproject.toml
   "pydoclint == 0.3.2",
   "pydocstyle == 6.3.0",
```

### Comparing `frequenz-client-reporting-0.1.0/src/frequenz/client/reporting/_client.py` & `frequenz-client-reporting-0.2.0/src/frequenz/client/reporting/_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright © 2024 Frequenz Energy-as-a-Service GmbH
 
 """Client for requests to the Reporting API."""
 
 from collections import namedtuple
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Any, AsyncIterator, Awaitable, Generator, Type, cast
+from typing import Any, AsyncIterator, Awaitable, Iterator, Type, cast
 
 import grpc.aio as grpcaio
 
 # pylint: disable=no-name-in-module
 from frequenz.api.common.v1.metrics.metric_sample_pb2 import Metric as PBMetric
 from frequenz.api.common.v1.microgrid.microgrid_pb2 import (
     MicrogridComponentIDs as PBMicrogridComponentIDs,
@@ -30,15 +30,20 @@
 from google.protobuf.timestamp_pb2 import Timestamp as PBTimestamp
 
 # pylint: enable=no-name-in-module
 
 MetricSample = namedtuple(
     "MetricSample", ["timestamp", "microgrid_id", "component_id", "metric", "value"]
 )
-"""Type for a sample of a time series incl. metric type, microgrid and component ID"""
+"""Type for a sample of a time series incl. metric type, microgrid and component ID
+
+A named tuple was chosen to allow safe access to the fields while keeping the
+simplicity of a tuple. This data type can be easily used to create a numpy array
+or a pandas DataFrame.
+"""
 
 
 @dataclass(frozen=True)
 class ComponentsDataPage:
     """A page of microgrid components data returned by the Reporting service."""
 
     _data_pb: PBListMicrogridComponentsDataResponse
@@ -54,15 +59,15 @@
             return True
         if not self._data_pb.microgrids[0].components:
             return True
         if not self._data_pb.microgrids[0].components[0].metric_samples:
             return True
         return False
 
-    def iterate_metric_samples(self) -> Generator[MetricSample, None, None]:
+    def __iter__(self) -> Iterator[MetricSample]:
         """Get generator that iterates over all values in the page.
 
         Note: So far only `SimpleMetricSample` in the `MetricSampleVariant`
         message is supported.
 
 
         Yields:
@@ -100,28 +105,28 @@
 
         Returns:
             The token for the next page of data.
         """
         return self._data_pb.pagination_info.next_page_token
 
 
-class ReportingClient:
+class ReportingApiClient:
     """A client for the Reporting service."""
 
     def __init__(self, service_address: str):
         """Create a new Reporting client.
 
         Args:
             service_address: The address of the Reporting service.
         """
         self._grpc_channel = grpcaio.insecure_channel(service_address)
         self._stub = ReportingStub(self._grpc_channel)
 
     # pylint: disable=too-many-arguments
-    async def iterate_single_component(
+    async def list_single_component_data(
         self,
         *,
         microgrid_id: int,
         component_id: int,
         metrics: Metric | list[Metric],
         start_dt: datetime,
         end_dt: datetime,
@@ -138,26 +143,64 @@
             page_size: The page size.
 
         Yields:
             A named tuple with the following fields:
             * timestamp: The timestamp of the metric sample.
             * value: The metric value.
         """
-        async for page in self._iterate_components_data_pages(
+        async for page in self._list_microgrid_components_data_pages(
             microgrid_components=[(microgrid_id, [component_id])],
             metrics=[metrics] if isinstance(metrics, Metric) else metrics,
             start_dt=start_dt,
             end_dt=end_dt,
             page_size=page_size,
         ):
-            for entry in page.iterate_metric_samples():
+            for entry in page:
+                yield entry
+
+    # pylint: disable=too-many-arguments
+    async def list_microgrid_components_data(
+        self,
+        *,
+        microgrid_components: list[tuple[int, list[int]]],
+        metrics: Metric | list[Metric],
+        start_dt: datetime,
+        end_dt: datetime,
+        page_size: int = 1000,
+    ) -> AsyncIterator[MetricSample]:
+        """Iterate over the data for multiple microgrids and components.
+
+        Args:
+            microgrid_components: List of tuples where each tuple contains
+                                  microgrid ID and corresponding component IDs.
+            metrics: The metric name or list of metric names.
+            start_dt: The start date and time.
+            end_dt: The end date and time.
+            page_size: The page size.
+
+        Yields:
+            A named tuple with the following fields:
+            * microgrid_id: The microgrid ID.
+            * component_id: The component ID.
+            * metric: The metric name.
+            * timestamp: The timestamp of the metric sample.
+            * value: The metric value.
+        """
+        async for page in self._list_microgrid_components_data_pages(
+            microgrid_components=microgrid_components,
+            metrics=[metrics] if isinstance(metrics, Metric) else metrics,
+            start_dt=start_dt,
+            end_dt=end_dt,
+            page_size=page_size,
+        ):
+            for entry in page:
                 yield entry
 
     # pylint: disable=too-many-arguments
-    async def _iterate_components_data_pages(
+    async def _list_microgrid_components_data_pages(
         self,
         *,
         microgrid_components: list[tuple[int, list[int]]],
         metrics: list[Metric],
         start_dt: datetime,
         end_dt: datetime,
         page_size: int = 1000,
@@ -255,15 +298,15 @@
             return None
         return ComponentsDataPage(response)
 
     async def close(self) -> None:
         """Close the client and cancel any pending requests immediately."""
         await self._grpc_channel.close(grace=None)
 
-    async def __aenter__(self) -> "ReportingClient":
+    async def __aenter__(self) -> "ReportingApiClient":
         """Enter the async context."""
         return self
 
     async def __aexit__(
         self,
         _exc_type: Type[BaseException] | None,
         _exc_val: BaseException | None,
```

### Comparing `frequenz-client-reporting-0.1.0/src/frequenz_client_reporting.egg-info/PKG-INFO` & `frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-client-reporting
-Version: 0.1.0
+Version: 0.2.0
 Summary: Reporting API client for Python
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Documentation, https://frequenz-floss.github.io/frequenz-client-reporting-python/
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-client-reporting-python/releases
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-client-reporting-python/issues
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-client-reporting-python
@@ -36,16 +36,14 @@
 [![PyPI Package](https://img.shields.io/pypi/v/frequenz-client-reporting)](https://pypi.org/project/frequenz-client-reporting/)
 [![Docs](https://img.shields.io/badge/docs-latest-informational)](https://frequenz-floss.github.io/frequenz-client-reporting-python/)
 
 ## Introduction
 
 Reporting API client for Python
 
-TODO(cookiecutter): Improve the README file
-
 ## Supported Platforms
 
 The following platforms are officially supported (tested):
 
 - **Python:** 3.11
 - **Operating System:** Ubuntu Linux 20.04
 - **Architectures:** amd64, arm64
```

### Comparing `frequenz-client-reporting-0.1.0/src/frequenz_client_reporting.egg-info/requires.txt` & `frequenz-client-reporting-0.2.0/src/frequenz_client_reporting.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 typing-extensions<5,>=4.5.0
-frequenz-api-reporting<1,>=0.1.1
+frequenz-api-reporting<0.2,>=0.1.1
 frequenz-client-common==0.1.0
 
 [dev]
 frequenz-client-reporting[dev-flake8,dev-formatting,dev-mkdocs,dev-mypy,dev-noxfile,dev-pylint,dev-pytest]
 
 [dev-flake8]
 flake8==6.1.0
```

