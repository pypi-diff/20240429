# Comparing `tmp/aau_ais_dipaal-0.1.0.tar.gz` & `tmp/aau_ais_dipaal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aau_ais_dipaal-0.1.0.tar", last modified: Wed Apr 24 12:49:43 2024, max compression
+gzip compressed data, was "aau_ais_dipaal-0.1.1.tar", last modified: Mon Apr 29 09:53:01 2024, max compression
```

## Comparing `aau_ais_dipaal-0.1.0.tar` & `aau_ais_dipaal-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      139 2024-04-18 10:19:07.540695 aau_ais_dipaal-0.1.0/README.md
--rw-r--r--   0        0        0      615 2024-04-24 12:49:43.184783 aau_ais_dipaal-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 11:59:12.781590 aau_ais_dipaal-0.1.0/src/dipaal/__init__.py
--rw-r--r--   0        0        0      244 2024-04-17 14:41:48.579028 aau_ais_dipaal-0.1.0/src/dipaal/convert/__init__.py
--rw-r--r--   0        0        0     1565 2024-04-17 13:58:07.085801 aau_ais_dipaal-0.1.0/src/dipaal/convert/callsign.py
--rw-r--r--   0        0        0     1489 2024-04-24 10:14:42.730209 aau_ais_dipaal-0.1.0/src/dipaal/convert/converter.py
--rw-r--r--   0        0        0     1113 2024-04-17 13:58:07.077796 aau_ais_dipaal-0.1.0/src/dipaal/convert/imo.py
--rw-r--r--   0        0        0     1125 2024-04-17 13:58:07.073624 aau_ais_dipaal-0.1.0/src/dipaal/convert/mmsi.py
--rw-r--r--   0        0        0      152 2024-04-23 11:19:37.881658 aau_ais_dipaal-0.1.0/src/dipaal/export/__init__.py
--rw-r--r--   0        0        0     5913 2024-04-24 11:38:06.792730 aau_ais_dipaal-0.1.0/src/dipaal/export/exporter.py
--rw-r--r--   0        0        0     4077 2024-04-24 12:04:56.635681 aau_ais_dipaal-0.1.0/src/dipaal/export/map_exporter.py
--rw-r--r--   0        0        0        0 2024-04-23 14:21:24.000145 aau_ais_dipaal-0.1.0/src/dipaal/export/sql/map_exporter/exists/enc.sql
--rw-r--r--   0        0        0        0 2024-04-23 14:21:52.095786 aau_ais_dipaal-0.1.0/src/dipaal/export/sql/map_exporter/exists/ship_type.sql
--rw-r--r--   0        0        0      413 2024-04-24 12:29:04.207404 aau_ais_dipaal-0.1.0/src/dipaal/settings.py
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      139 2024-04-18 10:19:07.540695 aau_ais_dipaal-0.1.1/README.md
+-rw-r--r--   0        0        0      670 2024-04-29 09:53:01.166226 aau_ais_dipaal-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:59:12.781590 aau_ais_dipaal-0.1.1/src/dipaal/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-17 14:41:48.579028 aau_ais_dipaal-0.1.1/src/dipaal/convert/__init__.py
+-rw-r--r--   0        0        0     1207 2024-04-25 09:28:54.746754 aau_ais_dipaal-0.1.1/src/dipaal/convert/callsign.py
+-rw-r--r--   0        0        0     1544 2024-04-29 09:09:13.050378 aau_ais_dipaal-0.1.1/src/dipaal/convert/converter.py
+-rw-r--r--   0        0        0     1177 2024-04-25 09:28:54.789569 aau_ais_dipaal-0.1.1/src/dipaal/convert/imo.py
+-rw-r--r--   0        0        0     1187 2024-04-25 09:28:54.736736 aau_ais_dipaal-0.1.1/src/dipaal/convert/mmsi.py
+-rw-r--r--   0        0        0      152 2024-04-23 11:19:37.881658 aau_ais_dipaal-0.1.1/src/dipaal/export/__init__.py
+-rw-r--r--   0        0        0     5913 2024-04-24 11:38:06.792730 aau_ais_dipaal-0.1.1/src/dipaal/export/exporter.py
+-rw-r--r--   0        0        0     4077 2024-04-24 12:04:56.635681 aau_ais_dipaal-0.1.1/src/dipaal/export/map_exporter.py
+-rw-r--r--   0        0        0        0 2024-04-23 14:21:24.000145 aau_ais_dipaal-0.1.1/src/dipaal/export/sql/map_exporter/exists/enc.sql
+-rw-r--r--   0        0        0        0 2024-04-23 14:21:52.095786 aau_ais_dipaal-0.1.1/src/dipaal/export/sql/map_exporter/exists/ship_type.sql
+-rw-r--r--   0        0        0      401 2024-04-29 09:31:48.467158 aau_ais_dipaal-0.1.1/src/dipaal/settings.py
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 aau_ais_dipaal-0.1.1/PKG-INFO
```

### Comparing `aau_ais_dipaal-0.1.0/pyproject.toml` & `aau_ais_dipaal-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [project]
 name = "aau-ais-dipaal"
-version = "0.1.0"
+version = "0.1.1"
 description = "TODO: Add a description of your project."
 authors = [
     { name = "Mikael Vind Mikkelsen", email = "mvmi@cs.aau.dk" },
 ]
 dependencies = [
     "aau-ais-utilities==0.1.*",
     "pydantic==2.7.*",
+    "pydantic-settings==2.2.*",
+    "jinjasql==0.1.*",
 ]
 requires-python = "==3.12.*"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `aau_ais_dipaal-0.1.0/src/dipaal/convert/callsign.py` & `aau_ais_dipaal-0.1.1/src/dipaal/convert/imo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,45 @@
-from convert.converter import Converter
+from .converter import Converter
+from dipaal.settings import get_dipaal_engine
 from sqlalchemy import Engine
 
 
-class CallsignConverter(Converter):
-    """Convert callsigns to other formats.
+class IMOConverter(Converter):
+    """Convert IMO numbers to other formats.
 
     This class requires a connection to a database containing the relevant data.
     """
 
-    def __init__(self, engine: Engine) -> None:
+    def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
         super().__init__(engine)
 
-    def to_mmsi(self, callsign: str) -> str:
-        """Convert a callsign to an MMSI number.
+    def to_mmsi(self, imo: str) -> str:
+        """Convert an IMO number to an MMSI number.
 
         Args:
-            callsign: The callsign to convert.
+            imo: The IMO number to convert.
 
         Returns:
             The MMSI number.
         """
 
         return self.convert_within_table(
-            from_format="callsign",
+            from_format="imo",
             to_format="mmsi",
             table="public.dim_ship",
-            value=callsign)
+            value=imo)
 
-
-    def to_imo(self, callsign: str) -> str:
-        """Convert a callsign to an IMO number.
+    def to_callsign(self, imo: str) -> str:
+        """Convert an IMO number to a callsign.
 
         Args:
-            callsign: The callsign to convert.
+            imo: The IMO number to convert.
 
         Returns:
-            The IMO number.
+            The callsign.
         """
 
         return self.convert_within_table(
-            from_format="callsign",
-            to_format="imo",
+            from_format="imo",
+            to_format="callsign",
             table="public.dim_ship",
-            value=callsign)
-
-
-# Example usage:
-if __name__ == "__main__":
-
-    from sqlalchemy import create_engine
-
-    user = "jupyter"
-    password = "thick40ice43"
-    host = "s1.dipaal.dk"
-    port = "30036"
-    database = "dipaal2"
-
-    engine = create_engine(f'postgresql+psycopg://{user}:{password}@{host}:{port}/{database}')
-
-    callsign_converter = CallsignConverter(engine)
-    print(callsign_converter.to_mmsi("VRES3"))
+            value=imo)
```

### Comparing `aau_ais_dipaal-0.1.0/src/dipaal/convert/converter.py` & `aau_ais_dipaal-0.1.1/src/dipaal/convert/converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from abc import ABC
 from sqlalchemy import Engine
-from aau_ais_core import PostgreSQLConnection, dipaal_engine
+from aau_ais_utilities.connections import PostgreSQLConnection
+from dipaal.settings import get_dipaal_engine
 
 
 class Converter(ABC):
 
-    def __init__(self, engine: Engine = dipaal_engine) -> None:
+    def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
         self.connection = PostgreSQLConnection(engine)
 
     def convert_within_table(self, *, from_format: str, to_format: str, table: str, value: str) -> str:
         """Convert a value from one format to another within the context of a single database table.
 
         Args:
             from_format: The format of the value to convert.
```

### Comparing `aau_ais_dipaal-0.1.0/src/dipaal/convert/imo.py` & `aau_ais_dipaal-0.1.1/src/dipaal/convert/callsign.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-from convert.converter import Converter
+from .converter import Converter
 from sqlalchemy import Engine
+from dipaal.settings import get_dipaal_engine
 
-class IMOConverter(Converter):
-    """Convert IMO numbers to other formats.
+
+class CallsignConverter(Converter):
+    """Convert callsigns to other formats.
 
     This class requires a connection to a database containing the relevant data.
     """
 
-    def __init__(self, engine: Engine) -> None:
+    def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
         super().__init__(engine)
 
-    def to_mmsi(self, imo: str) -> str:
-        """Convert an IMO number to an MMSI number.
+    def to_mmsi(self, callsign: str) -> str:
+        """Convert a callsign to an MMSI number.
 
         Args:
-            imo: The IMO number to convert.
+            callsign: The callsign to convert.
 
         Returns:
             The MMSI number.
         """
 
         return self.convert_within_table(
-            from_format="imo",
+            from_format="callsign",
             to_format="mmsi",
             table="public.dim_ship",
-            value=imo)
+            value=callsign)
+
 
-    def to_callsign(self, imo: str) -> str:
-        """Convert an IMO number to a callsign.
+    def to_imo(self, callsign: str) -> str:
+        """Convert a callsign to an IMO number.
 
         Args:
-            imo: The IMO number to convert.
+            callsign: The callsign to convert.
 
         Returns:
-            The callsign.
+            The IMO number.
         """
 
         return self.convert_within_table(
-            from_format="imo",
-            to_format="callsign",
+            from_format="callsign",
+            to_format="imo",
             table="public.dim_ship",
-            value=imo)
+            value=callsign)
```

### Comparing `aau_ais_dipaal-0.1.0/src/dipaal/convert/mmsi.py` & `aau_ais_dipaal-0.1.1/src/dipaal/convert/mmsi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from convert.converter import Converter
+from .converter import Converter
+from dipaal.settings import get_dipaal_engine
 from sqlalchemy import Engine
 
 
 class MMSIConverter(Converter):
     """Convert MMSI numbers to other formats.
 
     This class requires a connection to a database containing the relevant data.
     """
 
-    def __init__(self, engine: Engine) -> None:
+    def __init__(self, engine: Engine = get_dipaal_engine()) -> None:
         super().__init__(engine)
 
     def to_imo(self, mmsi: str) -> str:
         """Convert an MMSI number to an IMO number.
 
         Args:
             mmsi: The MMSI number to convert.
```

### Comparing `aau_ais_dipaal-0.1.0/src/dipaal/export/exporter.py` & `aau_ais_dipaal-0.1.1/src/dipaal/export/exporter.py`

 * *Files identical despite different names*

### Comparing `aau_ais_dipaal-0.1.0/src/dipaal/export/map_exporter.py` & `aau_ais_dipaal-0.1.1/src/dipaal/export/map_exporter.py`

 * *Files identical despite different names*

