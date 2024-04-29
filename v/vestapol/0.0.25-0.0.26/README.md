# Comparing `tmp/vestapol-0.0.25.tar.gz` & `tmp/vestapol-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vestapol-0.0.25.tar", max compression
+gzip compressed data, was "vestapol-0.0.26.tar", max compression
```

## Comparing `vestapol-0.0.25.tar` & `vestapol-0.0.26.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11355 2024-03-08 07:42:10.765828 vestapol-0.0.25/LICENSE
--rw-r--r--   0        0        0     3015 2024-03-08 07:42:10.765828 vestapol-0.0.25/README.md
--rw-r--r--   0        0        0     1011 2024-03-08 07:42:10.765828 vestapol-0.0.25/pyproject.toml
--rw-r--r--   0        0        0      209 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/api/__init__.py
--rw-r--r--   0        0        0      798 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/api/api.py
--rw-r--r--   0        0        0        0 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/destinations/__init__.py
--rw-r--r--   0        0        0      579 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/destinations/base_destination.py
--rw-r--r--   0        0        0     3095 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/destinations/gcp_destination.py
--rw-r--r--   0        0        0      957 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/destinations/local_destination.py
--rw-r--r--   0        0        0     2783 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/external_tables.py
--rw-r--r--   0        0        0        0 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/py.typed
--rw-r--r--   0        0        0        0 2024-03-08 07:42:10.765828 vestapol-0.0.25/vestapol/web_resources/__init__.py
--rw-r--r--   0        0        0     4079 2024-03-08 07:42:10.769828 vestapol-0.0.25/vestapol/web_resources/base_resource.py
--rw-r--r--   0        0        0     2182 2024-03-08 07:42:10.769828 vestapol-0.0.25/vestapol/web_resources/csv_resource.py
--rw-r--r--   0        0        0      588 2024-03-08 07:42:10.769828 vestapol-0.0.25/vestapol/web_resources/github_resource.py
--rw-r--r--   0        0        0     2775 2024-03-08 07:42:10.769828 vestapol-0.0.25/vestapol/web_resources/json_resource.py
--rw-r--r--   0        0        0        0 2024-03-08 07:42:10.769828 vestapol-0.0.25/vestapol/writers/__init__.py
--rw-r--r--   0        0        0      620 2024-03-08 07:42:10.769828 vestapol-0.0.25/vestapol/writers/json_writer.py
--rw-r--r--   0        0        0      184 2024-03-08 07:42:10.769828 vestapol-0.0.25/vestapol/writers/text_writer.py
--rw-r--r--   0        0        0     3880 1970-01-01 00:00:00.000000 vestapol-0.0.25/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-04-29 15:42:11.878409 vestapol-0.0.26/LICENSE
+-rw-r--r--   0        0        0     3015 2024-04-29 15:42:11.878409 vestapol-0.0.26/README.md
+-rw-r--r--   0        0        0     1011 2024-04-29 15:42:11.878409 vestapol-0.0.26/pyproject.toml
+-rw-r--r--   0        0        0      209 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/api/__init__.py
+-rw-r--r--   0        0        0      798 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/api/api.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/destinations/__init__.py
+-rw-r--r--   0        0        0      579 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/destinations/base_destination.py
+-rw-r--r--   0        0        0     3095 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/destinations/gcp_destination.py
+-rw-r--r--   0        0        0      957 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/destinations/local_destination.py
+-rw-r--r--   0        0        0     2783 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/external_tables.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/py.typed
+-rw-r--r--   0        0        0        0 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/web_resources/__init__.py
+-rw-r--r--   0        0        0     4006 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/web_resources/base_resource.py
+-rw-r--r--   0        0        0     2182 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/web_resources/csv_resource.py
+-rw-r--r--   0        0        0      588 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/web_resources/github_resource.py
+-rw-r--r--   0        0        0     2755 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/web_resources/json_resource.py
+-rw-r--r--   0        0        0        0 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/writers/__init__.py
+-rw-r--r--   0        0        0      620 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/writers/json_writer.py
+-rw-r--r--   0        0        0      184 2024-04-29 15:42:11.882409 vestapol-0.0.26/vestapol/writers/text_writer.py
+-rw-r--r--   0        0        0     3880 1970-01-01 00:00:00.000000 vestapol-0.0.26/PKG-INFO
```

### Comparing `vestapol-0.0.25/LICENSE` & `vestapol-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/README.md` & `vestapol-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/pyproject.toml` & `vestapol-0.0.26/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vestapol"
-version = "0.0.25"
+version = "0.0.26"
 description = "Python package that loads data from the web and deploys a corresponding external table definition, so that the data can be queried using standard SQL."
 authors = ["Brian Waligorski <bwaligorski@inquirer.com>"]
 license = "Apache License 2.0"
 readme = "README.md"  # Markdown files are supported
 repository = "https://github.com/phillymedia/vestapol"
 homepage = "https://github.com/phillymedia/vestapol"
```

### Comparing `vestapol-0.0.25/vestapol/api/api.py` & `vestapol-0.0.26/vestapol/api/api.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/vestapol/destinations/base_destination.py` & `vestapol-0.0.26/vestapol/destinations/base_destination.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/vestapol/destinations/gcp_destination.py` & `vestapol-0.0.26/vestapol/destinations/gcp_destination.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/vestapol/destinations/local_destination.py` & `vestapol-0.0.26/vestapol/destinations/local_destination.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/vestapol/external_tables.py` & `vestapol-0.0.26/vestapol/external_tables.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/vestapol/web_resources/base_resource.py` & `vestapol-0.0.26/vestapol/web_resources/base_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,15 +59,14 @@
             the destinations module for supported destination types.
 
         Returns:
             list: a list of data rows
         """
         data = self.request_data()
         self.write_data(data, destination)
-        return data  # TODO: I think we can remove this return statement
 
     def request_data(self):
         """Method that encapsulates the call to an API or other web resource. It
         returns a raw representation of the response may be further transformed
         so that it can be parsed by external object tables. In most instances,
         this method will be overridden when creating a subclass of BaseResource.
```

### Comparing `vestapol-0.0.25/vestapol/web_resources/csv_resource.py` & `vestapol-0.0.26/vestapol/web_resources/csv_resource.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/vestapol/web_resources/github_resource.py` & `vestapol-0.0.26/vestapol/web_resources/github_resource.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/vestapol/web_resources/json_resource.py` & `vestapol-0.0.26/vestapol/web_resources/json_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Any
 from typing import Dict
+from typing import Generator
 from typing import List
 from typing import Optional
 from typing import Tuple
-from typing import Generator
 from typing import TYPE_CHECKING
 
 from vestapol.web_resources import base_resource
 from vestapol.writers import json_writer
 
 if TYPE_CHECKING:
     from vestapol.destinations.base_destination import BaseDestination
@@ -51,15 +51,14 @@
             self.manual_schema,
         )
 
     def load(self, destination: BaseDestination):
         data = self.request_data()
         self.write_data(data, destination)
         self.unnest_data(data, destination)
-        return data
 
     def write_data(self, api_data, destination: BaseDestination):
         json_writer.write_json(
             api_data, self.response_target_prefix / self.response_filename, destination
         )
 
     @abstractmethod
```

### Comparing `vestapol-0.0.25/vestapol/writers/json_writer.py` & `vestapol-0.0.26/vestapol/writers/json_writer.py`

 * *Files identical despite different names*

### Comparing `vestapol-0.0.25/PKG-INFO` & `vestapol-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vestapol
-Version: 0.0.25
+Version: 0.0.26
 Summary: Python package that loads data from the web and deploys a corresponding external table definition, so that the data can be queried using standard SQL.
 Home-page: https://github.com/phillymedia/vestapol
 License: Apache-2.0
 Author: Brian Waligorski
 Author-email: bwaligorski@inquirer.com
 Requires-Python: >=3.8.12,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

