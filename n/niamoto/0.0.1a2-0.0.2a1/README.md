# Comparing `tmp/niamoto-0.0.1a2.tar.gz` & `tmp/niamoto-0.0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niamoto-0.0.1a2.tar", max compression
+gzip compressed data, was "niamoto-0.0.2a1.tar", max compression
```

## Comparing `niamoto-0.0.1a2.tar` & `niamoto-0.0.2a1.tar`

### file list

```diff
@@ -1,34 +1,60 @@
--rw-r--r--   0        0        0    35149 2023-12-18 18:49:51.068568 niamoto-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     5469 2024-01-24 10:16:49.397477 niamoto-0.0.1a2/README.md
--rw-r--r--   0        0        0     7523 2024-01-24 10:53:39.705413 niamoto-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899456 niamoto-0.0.1a2/src/niamoto/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899544 niamoto-0.0.1a2/src/niamoto/api/__init__.py
--rw-r--r--   0        0        0     1936 2023-12-18 18:47:14.899731 niamoto-0.0.1a2/src/niamoto/api/import_api.py
--rw-r--r--   0        0        0      580 2023-12-18 18:47:14.899859 niamoto-0.0.1a2/src/niamoto/api/site_generator_api.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899932 niamoto-0.0.1a2/src/niamoto/api_creator/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900005 niamoto-0.0.1a2/src/niamoto/cli/__init__.py
--rw-r--r--   0        0        0     9934 2023-12-18 18:47:14.900187 niamoto-0.0.1a2/src/niamoto/cli/commands.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900231 niamoto-0.0.1a2/src/niamoto/common/__init__.py
--rw-r--r--   0        0        0      848 2023-12-18 18:47:14.900386 niamoto-0.0.1a2/src/niamoto/common/config_manager.py
--rw-r--r--   0        0        0     1422 2023-12-18 18:47:14.900498 niamoto-0.0.1a2/src/niamoto/common/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900566 niamoto-0.0.1a2/src/niamoto/config/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900634 niamoto-0.0.1a2/src/niamoto/data_importer/__init__.py
--rw-r--r--   0        0        0     2081 2023-12-18 18:47:14.900781 niamoto-0.0.1a2/src/niamoto/data_importer/data_importer.py
--rw-r--r--   0        0        0     1302 2023-12-18 18:47:14.900891 niamoto-0.0.1a2/src/niamoto/data_importer/data_reader.py
--rw-r--r--   0        0        0      721 2023-12-18 18:47:14.901007 niamoto-0.0.1a2/src/niamoto/data_importer/data_validator.py
--rw-r--r--   0        0        0     1181 2023-12-18 18:47:14.901126 niamoto-0.0.1a2/src/niamoto/data_importer/data_writer.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.901167 niamoto-0.0.1a2/src/niamoto/data_processor/__init__.py
--rw-r--r--   0        0        0    23359 2024-01-24 10:55:38.719616 niamoto-0.0.1a2/src/niamoto/data_processor/taxon/processor.py
--rw-r--r--   0        0        0        1 2023-12-18 18:47:14.901500 niamoto-0.0.1a2/src/niamoto/data_processor/taxon/utils.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.901540 niamoto-0.0.1a2/src/niamoto/db/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.901641 niamoto-0.0.1a2/src/niamoto/db/models/__init__.py
--rw-r--r--   0        0        0     5589 2024-01-24 10:55:38.718795 niamoto-0.0.1a2/src/niamoto/db/models/models.py
--rw-r--r--   0        0        0     2908 2023-12-18 18:47:14.901935 niamoto-0.0.1a2/src/niamoto/db/niamoto_repository.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.901972 niamoto-0.0.1a2/src/niamoto/db/utils/__init__.py
--rw-r--r--   0        0        0     3692 2024-01-24 10:27:17.305204 niamoto-0.0.1a2/src/niamoto/db/utils/database.py
--rw-r--r--   0        0        0      174 2023-12-18 18:47:14.902253 niamoto-0.0.1a2/src/niamoto/main.py
--rw-r--r--   0        0        0        0 2023-12-18 18:47:14.902296 niamoto-0.0.1a2/src/niamoto/static_site_generator/__init__.py
--rw-r--r--   0        0        0     5615 2023-12-18 18:47:14.902453 niamoto-0.0.1a2/src/niamoto/static_site_generator/page_generator.py
--rw-r--r--   0        0        0    18146 2023-12-18 20:58:31.222251 niamoto-0.0.1a2/src/niamoto/static_site_generator/static/js/index.js
--rw-r--r--   0        0        0     9901 2023-12-18 18:47:14.902831 niamoto-0.0.1a2/src/niamoto/static_site_generator/templates/taxon_template.html
--rw-r--r--   0        0        0     7580 1970-01-01 00:00:00.000000 niamoto-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-12-18 18:49:51.068568 niamoto-0.0.2a1/LICENSE
+-rw-r--r--   0        0        0    12572 2024-04-29 09:35:50.501361 niamoto-0.0.2a1/README.md
+-rw-r--r--   0        0        0     7608 2024-04-26 16:21:56.378658 niamoto-0.0.2a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899456 niamoto-0.0.2a1/src/niamoto/__init__.py
+-rw-r--r--   0        0        0      176 2024-03-17 11:30:55.790624 niamoto-0.0.2a1/src/niamoto/api/__init__.py
+-rw-r--r--   0        0        0      638 2024-04-29 08:55:57.427623 niamoto-0.0.2a1/src/niamoto/api/generator.py
+-rw-r--r--   0        0        0     3404 2024-04-26 16:01:49.245020 niamoto-0.0.2a1/src/niamoto/api/importer.py
+-rw-r--r--   0        0        0     2172 2024-04-26 16:01:49.248356 niamoto-0.0.2a1/src/niamoto/api/mapper.py
+-rw-r--r--   0        0        0     2994 2024-04-29 08:38:58.672070 niamoto-0.0.2a1/src/niamoto/api/statistics.py
+-rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900005 niamoto-0.0.2a1/src/niamoto/cli/__init__.py
+-rw-r--r--   0        0        0    23392 2024-04-29 08:55:57.428067 niamoto-0.0.2a1/src/niamoto/cli/commands.py
+-rw-r--r--   0        0        0        0 2023-12-18 18:47:14.900231 niamoto-0.0.2a1/src/niamoto/common/__init__.py
+-rw-r--r--   0        0        0     6722 2024-04-26 16:01:49.247937 niamoto-0.0.2a1/src/niamoto/common/config.py
+-rw-r--r--   0        0        0     7679 2024-04-26 16:01:49.246735 niamoto-0.0.2a1/src/niamoto/common/database.py
+-rw-r--r--   0        0        0     1419 2024-03-17 11:30:55.792426 niamoto-0.0.2a1/src/niamoto/common/environment.py
+-rw-r--r--   0        0        0     1422 2024-03-17 11:30:55.791898 niamoto-0.0.2a1/src/niamoto/common/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-14 20:33:15.957328 niamoto-0.0.2a1/src/niamoto/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 16:56:57.129500 niamoto-0.0.2a1/src/niamoto/core/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 16:56:57.125946 niamoto-0.0.2a1/src/niamoto/core/components/importers/__init__.py
+-rw-r--r--   0        0        0     9811 2024-04-26 16:01:49.248390 niamoto-0.0.2a1/src/niamoto/core/components/importers/occurrences.py
+-rw-r--r--   0        0        0     1608 2024-04-26 15:09:01.953631 niamoto-0.0.2a1/src/niamoto/core/components/importers/plots.py
+-rw-r--r--   0        0        0     3900 2024-04-26 16:01:49.246868 niamoto-0.0.2a1/src/niamoto/core/components/importers/taxonomy.py
+-rw-r--r--   0        0        0        0 2024-02-26 16:58:28.941202 niamoto-0.0.2a1/src/niamoto/core/components/mappers/__init__.py
+-rw-r--r--   0        0        0    12822 2024-04-29 08:55:57.427862 niamoto-0.0.2a1/src/niamoto/core/components/mappers/mapping_manager.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:26:08.724363 niamoto-0.0.2a1/src/niamoto/core/components/statistics/__init__.py
+-rw-r--r--   0        0        0     2312 2024-04-29 08:45:10.824735 niamoto-0.0.2a1/src/niamoto/core/components/statistics/plot_stats_calculator.py
+-rw-r--r--   0        0        0    11234 2024-04-29 08:55:57.428251 niamoto-0.0.2a1/src/niamoto/core/components/statistics/statistics_calculator.py
+-rw-r--r--   0        0        0     3637 2024-04-26 16:01:49.245261 niamoto-0.0.2a1/src/niamoto/core/components/statistics/taxonomy_stats_calculator.py
+-rw-r--r--   0        0        0      107 2024-04-29 08:58:01.228690 niamoto-0.0.2a1/src/niamoto/core/models/__init__.py
+-rw-r--r--   0        0        0     3094 2024-04-29 08:55:57.427544 niamoto-0.0.2a1/src/niamoto/core/models/models.py
+-rw-r--r--   0        0        0        0 2024-02-26 09:35:39.100463 niamoto-0.0.2a1/src/niamoto/core/repositories/__init__.py
+-rw-r--r--   0        0        0     2729 2024-04-26 16:16:39.970756 niamoto-0.0.2a1/src/niamoto/core/repositories/niamoto_repository.py
+-rw-r--r--   0        0        0        0 2024-02-26 16:59:11.340255 niamoto-0.0.2a1/src/niamoto/core/services/__init__.py
+-rw-r--r--   0        0        0     1556 2024-03-22 10:17:01.014526 niamoto-0.0.2a1/src/niamoto/core/services/importer.py
+-rw-r--r--   0        0        0     1083 2024-04-26 16:01:49.247159 niamoto-0.0.2a1/src/niamoto/core/services/mapper.py
+-rw-r--r--   0        0        0    23730 2024-04-29 09:04:50.758432 niamoto-0.0.2a1/src/niamoto/core/services/processor.py
+-rw-r--r--   0        0        0     1899 2024-04-26 16:01:49.245968 niamoto-0.0.2a1/src/niamoto/core/services/statistics.py
+-rw-r--r--   0        0        0        0 2024-02-26 09:35:12.975166 niamoto-0.0.2a1/src/niamoto/core/utils/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-26 16:01:49.176772 niamoto-0.0.2a1/src/niamoto/core/utils/csv_utils.py
+-rw-r--r--   0        0        0      174 2024-03-17 09:40:18.006381 niamoto-0.0.2a1/src/niamoto/main.py
+-rw-r--r--   0        0        0       78 2024-03-14 22:19:33.109529 niamoto-0.0.2a1/src/niamoto/publish/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-18 18:47:14.899932 niamoto-0.0.2a1/src/niamoto/publish/api_creator/__init__.py
+-rw-r--r--   0        0        0       71 2024-03-14 21:27:58.003471 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/__init__.py
+-rw-r--r--   0        0        0     5997 2024-04-29 09:12:19.969907 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/page_generator.py
+-rw-r--r--   0        0        0     8892 2024-04-28 21:29:58.212701 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/index.js
+-rw-r--r--   0        0        0   205488 2024-04-26 17:33:58.572179 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/chart/4.4.2_chart.js
+-rw-r--r--   0        0        0   586923 2024-04-26 17:34:20.924377 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/d3/7.8.5_d3.js
+-rw-r--r--   0        0        0   288580 2024-04-26 17:34:26.124154 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/jquery/3.6.0_jquery.js
+-rw-r--r--   0        0        0    47635 2024-04-26 17:34:15.492610 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/justgage/1.6.1_justgage.js
+-rw-r--r--   0        0        0    14806 2024-04-26 17:32:44.478066 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.css
+-rw-r--r--   0        0        0   147552 2024-04-26 17:34:31.191623 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/1.9.4_leaflet.js
+-rw-r--r--   0        0        0     1259 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers-2x.png
+-rw-r--r--   0        0        0      696 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/layers.png
+-rw-r--r--   0        0        0     2464 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0        0        0     1466 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-icon.png
+-rw-r--r--   0        0        0      618 2023-05-18 11:01:45.000000 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/leaflet/images/marker-shadow.png
+-rw-r--r--   0        0        0   310628 2024-04-26 17:34:08.014141 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/raphael/2.3.0_raphael.js
+-rw-r--r--   0        0        0  3642321 2024-04-26 17:26:39.465386 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/static/js/vendor/tailwindcss/2.2.19_dist_tailwind.css
+-rw-r--r--   0        0        0     5514 2024-04-29 07:50:15.272656 niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/templates/taxon_template.html
+-rw-r--r--   0        0        0    14692 1970-01-01 00:00:00.000000 niamoto-0.0.2a1/PKG-INFO
```

### Comparing `niamoto-0.0.1a2/LICENSE` & `niamoto-0.0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.1a2/pyproject.toml` & `niamoto-0.0.2a1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "niamoto"
-version = "0.0.1a2"
+version = "0.0.2a1"
 description = ""
 authors = ["Julien Barbe <julien.barbe@me.com>"]
 readme = "README.md"
 license= "GPL-3.0-or-later"
 packages = [{include = "niamoto", from = "src"}]
 homepage = "https://github.com/niamoto/niamoto"
 repository= "https://github.com/niamoto/niamoto"
@@ -37,85 +37,85 @@
 
 # ---------------------
 # Database dependencies
 # ---------------------
 
 # SQLAlchemy - Comprehensive database toolkit for Python.
 # Documentation: https://www.sqlalchemy.org/
-sqlalchemy = "^2.0.23"
+sqlalchemy = {extras = ["mypy"], version = "^2.0.29"}
 
 # alembic - Database migration tool for SQLAlchemy.
 # Documentation: https://alembic.sqlalchemy.org/en/latest/
 alembic = "^1.12.1"
 # geoalchemy2 - Extensions to SQLAlchemy for working with spatial databases.
 # Documentation: https://geoalchemy-2.readthedocs.io/
-geoalchemy2 = "^0.14.2"
+geoalchemy2 = "^0.15.0"
 
 # sqlite-utils - Utilities for manipulating SQLite databases.
 # Documentation: https://sqlite-utils.datasette.io/en/stable/
 
 # duckdb - In-process SQL OLAP Database Management System.
 # Documentation: https://duckdb.org/docs/api/python
 # Note: DuckDB is a new database management system that is designed to be used as an embedded database.
 # It is designed to be robust against corrupt data, supports both static and dynamic typing, comes with a
 # powerful query optimizer and can execute SQL queries in parallel.
 # References : https://geog-414.gishub.org/book/duckdb/01_duckdb_intro.html
 #              https://medium.com/@dipeit/researchers-please-replace-sqlite-with-duckdb-now-f038044a2702
 #              http://duckdb.org/docs/archive/0.9.1/api/python/overview
-duckdb = "^0.9.1"
+duckdb = "^0.10.1"
 
 # duckdb-engine - SQLAlchemy dialect for DuckDB.
 # Documentation: https://pypi.org/project/duckdb-engine/
-duckdb-engine = "^0.9.2"
+duckdb-engine = "^0.12.0"
 
 # ---------------------
 # Geospatial libraries
 # ---------------------
 # leafmap - Interactive mapping library with ease of use for geospatial analysis.
 # Documentation: https://leafmap.org/#key-features
-leafmap = "^0.28.1"
+leafmap = "^0.31.5"
 
 # geopandas - Extends pandas for spatial data operations.
 # Documentation: https://geopandas.org/
 geopandas = "^0.14.1"
 
 # rasterio - Library for reading and writing raster datasets (e.g., images, geospatial rasters).
 # Documentation: https://rasterio.readthedocs.io/
 rasterio = "^1.3.9"
 
 # shapely - Manipulation and analysis of planar geometric objects.
 # Documentation: https://shapely.readthedocs.io/
-shapely = "^2.0.2"
+shapely = "^2.0.3"
 
 # -------------------------
 # Data Processing libraries
 # -------------------------
 
 # pandas - Essential library for data manipulation and analysis.
 # Documentation: https://pandas.pydata.org/
-pandas = "^2.1.3"
+pandas = "^2.2.1"
 
 # pyarrow - Python bindings for Apache Arrow. required by pandas.
 # Documentation: https://arrow.apache.org/docs/python/
-pyarrow = "^15.0.0"
+pyarrow = "16.0.0"
 
 # numpy - Fundamental package for scientific computing in Python.
 # Documentation: https://numpy.org/
 numpy = "^1.26.1"
 
 # ---------------------------
 # Command Line Interface (CLI)
 # ---------------------------
 
 # click - Create beautiful command line interfaces in a composable way.
 # Documentation: https://click.palletsprojects.com/en/8.0.x/
 click = "^8.1.7"
 
 # rich - Python library for rich text and beautiful formatting in the terminal.
-rich = "^13.7.0"
+rich = "^13.7.1"
 
 # trogon - Auto-generate friendly terminal user interfaces for command line apps.
 # Documentation: https://github.com/Textualize/trogon
 
 # tabulate - Pretty-print tabular data within Python.
 # Documentation: https://pypi.org/project/tabulate/
 tabulate = "^0.9.0"
@@ -134,19 +134,16 @@
 
 # pyproj - Python interface to PROJ (cartographic projections and coordinate transformations library).
 pyproj = "^3.6.1"
 
 # rjsmin - JavaScript minifier written in Python.
 rjsmin = "^1.2.2"
 
-# toml - Python Library for Tom's Obvious, Minimal Language.
-toml = "^0.10.2"
-
-
-
+# prompt-toolkit - Library for building powerful interactive command line applications in Python.
+prompt-toolkit = "^3.0.43"
 
 
 [tool.poetry.group.dev.dependencies]
 # -------------
 # Testing Tools
 # -------------
 
@@ -183,15 +180,15 @@
 # mypy - Optional static type checker for Python, aiming to combine the benefits of dynamic and static typing.
 # Documentation: http://mypy-lang.org/
 mypy = "^1.7.0"
 types-click = "^7.1.8"
 types-tabulate = "^0.9.0.3"
 types-pluggy = "^1.2.0.2"
 pandas-stubs = "^2.1.1.230928"
-types-toml = "^0.10.8.7"
+types-pyyaml = "^6.0.12.20240311"
 # pydantic - Data validation and settings management using Python type hinting.
 pydantic = "^2.5.0"
 
 # ----------------------------
 # Development Utilities
 # ----------------------------
```

### Comparing `niamoto-0.0.1a2/src/niamoto/common/config_manager.py` & `niamoto-0.0.2a1/src/niamoto/api/generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-import os
-import toml
+from typing import List, Optional, Any, Dict
 
-from typing import Any, Dict, Optional
+from niamoto.core.models import TaxonRef
+from niamoto.common.config import Config
+from niamoto.publish import PageGenerator
 
 
-class ConfigManager:
-    def __init__(self) -> None:
-        self.config: Dict[str, Any] = self.load_config()
+class StaticContentGenerator:
+    def __init__(self, config: Config) -> None:
+        self.page_generator = PageGenerator(config)
 
-    def load_config(self) -> Dict[str, Any]:
-        config_path: str = os.path.join(os.getcwd(), "config", "niamoto_config.toml")
-        if os.path.exists(config_path):
-            with open(config_path, "r") as config_file:
-                return toml.load(config_file)
-        else:
-            raise FileNotFoundError("Configuration file not found.")
+    def generate_page_for_taxon(
+        self, taxon: TaxonRef, stats: Optional[Any], mapping: Dict[Any, Any]
+    ) -> str:
+        return self.page_generator.generate_taxon_page(taxon, stats, mapping)
 
-    def get(self, section: str, key: Optional[str] = None) -> Any:
-        if key:
-            # Returns a specific value in the section
-            return self.config[section].get(key)
-        else:
-            # Returns the entire section if no specific key is provided
-            return self.config.get(section)
+    def generate_taxonomy_tree(self, taxons: List[TaxonRef]) -> None:
+        self.page_generator.generate_taxonomy_tree_js(taxons)
```

### Comparing `niamoto-0.0.1a2/src/niamoto/common/exceptions.py` & `niamoto-0.0.2a1/src/niamoto/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `niamoto-0.0.1a2/src/niamoto/data_processor/taxon/processor.py` & `niamoto-0.0.2a1/src/niamoto/core/services/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 import os
 import re
 import time
-from rich.console import Console
-from rich.progress import track
-from pyproj import Transformer, ProjError  # type: ignore
+from typing import Any, Callable, Dict, List, Union
+
+import pandas as pd
 import rasterio  # type: ignore
+from loguru import logger
+from pyproj import Transformer, ProjError  # type: ignore
 from rasterio.errors import RasterioError  # type: ignore
+from rich.console import Console
+from rich.progress import track
 from shapely import wkt  # type: ignore
-from loguru import logger
-import pandas as pd
-from typing import Any, Callable, Dict, List, Union
-from niamoto.common.config_manager import ConfigManager
-from niamoto.db.models.models import Taxon
-from niamoto.db.utils.database import Database
+
+from niamoto.core.models import TaxonRef
+from niamoto.common.config import Config
+from niamoto.common.database import Database
 
 
 class TaxonDataProcessor:
     """
     Processor for handling taxon data operations, including reading from a DataFrame,
     processing data, and writing to a database.
     """
 
     def __init__(self, db_path: str):
         """Initialize the processor with a database name."""
         self.db = Database(db_path)
         self.console = Console()
-        self.config = ConfigManager()
+        self.config = Config()
 
     def process_and_write_taxon_data(self, data: Any) -> None:
         """Process the provided taxon data and write it to the database."""
         start_time = time.time()
         # Sort the DataFrame for easier processing
 
-        taxonomy_config = self.config.get("taxonomy")
+        taxonomy_config = {
+            "Family": {"field": "id_family", "parent": ""},
+            "Genus": {"field": "id_genus", "parent": "Family"},
+            "Species": {"field": "id_species", "parent": "Genus"},
+            "Hybrid": {"field": "id_species", "parent": "Genus"},
+            "Subspecies": {"field": "id_infra", "parent": "Species"},
+            "Variety": {"field": "id_infra", "parent": "Species"},
+            "Forma": {"field": "id_infra", "parent": "Species"},
+        }
 
         # Step 1: Create or update all taxons from the data
         # Iterate through each row of the sorted DataFrame
         self.console.print("Generating taxonomic hierarchy", style="italic blue")
-        self.generate_taxonomy_from_occurrences(data, taxonomy_config)
+        self.generate_taxonomy_from_occurrences(data, TaxonRef, taxonomy_config)
 
         # Commit the changes to ensure all taxons have been saved
         self.db.commit_session()
 
         # Step 2: Execute necessary calculations on the data
         self.console.print("Performing calculations", style="italic blue")
         self.perform_calculations(data, taxonomy_config)
@@ -56,66 +66,76 @@
         total_time = end_time - start_time
 
         self.console.print(
             f"Total processing time: {total_time:.2f} seconds", style="italic blue"
         )
 
     def generate_taxonomy_from_occurrences(
-        self, data: Any, config: Dict[str, Any]
+        self, data: Any, model: Any, config: Dict[str, Any]
     ) -> None:
         """
         Generate the taxonomy hierarchy from occurrence data.
 
         Parameters:
-            occurrences (pd.DataFrame): DataFrame containing occurrence data.
+            data: DataFrame containing the occurrence data.
+            model: The SQLAlchemy model to use for the taxon hierarchy.
+            config: Configuration defining the taxonomic ranks and their hierarchy.
         """
         sorted_df = data.sort_values(
-            by=["id_taxonref", "id_family", "id_genus", "id_species", "id_infra"]
+            by=["id_family", "id_genus", "id_species", "id_infra"]
         )
 
-        self.create_taxonomic_hierarchy(sorted_df, self.db, config)
+        self.create_taxonomic_hierarchy(sorted_df, self.db.session, model, config)
 
     def create_taxonomic_hierarchy(
-        self, data: Any, db: Any, taxonomy_config: Dict[str, Any]
+        self, data: Any, session: Any, model: Any, taxonomy_config: Dict[str, Any]
     ) -> None:
         """
         Creates a taxonomic hierarchy based on a given configuration.
 
-            :param data: DataFrame containing the taxonomic data.
-            :param session: Database session.
-            :param config: Configuration defining the taxonomic ranks and their hierarchy.
+        Parameters:
+            data: DataFrame containing the taxonomic data.
+            session: Database session.
+            model: The SQLAlchemy model to use for the taxonomic hierarchy.
+            taxonomy_config: Configuration defining the taxonomic ranks and their hierarchy.
+
         """
 
         for rank in taxonomy_config:
             self.create_taxons_for_rank(
-                data, db, rank, taxonomy_config[rank], taxonomy_config
+                data, session, model, rank, taxonomy_config[rank], taxonomy_config
             )
 
     def create_taxons_for_rank(
         self,
         data: Any,
-        db: Any,
+        session: Any,
+        model: Any,
         rank_name: str,
         rank_config: Dict[str, Any],
         taxonomy_config: Dict[str, Any],
     ) -> None:
         """
         Creates taxons for a specific rank based on the configuration.
 
-            :param data: DataFrame containing the taxonomic data.
-            :param session: Database session.
-            :param rank_name: Name of the taxonomic rank to process.
-            :param rank_config: Configuration for the current taxonomic rank.
+        Parameters:
+            data: DataFrame containing the taxonomic data.
+            session: Database session.
+            model: The SQLAlchemy model to use for the taxonomic hierarchy.
+            rank_name: The name of the taxonomic rank.
+            rank_config: Configuration for the taxonomic rank.
+            taxonomy_config: Configuration defining the taxonomic ranks and their hierarchy.
         """
         ids = data[rank_config["field"]].dropna().unique()
         for id_ in track(ids, description=f"{rank_name}"):
             id_native = int(id_) if pd.notna(id_) else None
-            query = db.session.query(Taxon).filter(Taxon.id_taxonref == id_native)
-            taxon_list = db.execute_query(query)
-            taxon = taxon_list[0] if taxon_list else None
+            taxon = session.query(TaxonRef).filter(TaxonRef.id == id_native).first()
+            # query = session.query(model).filter(model.id_taxonref == id_native)
+            # taxon_list = db.execute_query(query)
+            # taxon = taxon_list[0] if taxon_list else None
             if not taxon:
                 row = data[data[rank_config["field"]] == id_].iloc[0]
                 # Extract and verify the identifiers for the different taxonomic ranks
                 taxon_ids = {
                     "id_family": int(row.get("id_family"))
                     if pd.notna(row.get("id_family"))
                     else None,
@@ -136,47 +156,46 @@
                 )
                 parent_id = (
                     int(row[parent_id_field])
                     if parent_id_field and pd.notna(row[parent_id_field])
                     else None
                 )
                 if parent_id:
-                    query = db.session.query(Taxon).filter(
-                        Taxon.id_taxonref == parent_id
+                    parent_taxon = (
+                        session.query(TaxonRef)
+                        .filter(TaxonRef.id == parent_id)
+                        .first()
                     )
-
-                    parent_taxon_list = db.execute_query(query)
-                    parent_taxon = parent_taxon_list[0] if parent_taxon_list else None
                     parent_id = parent_taxon.id if parent_taxon else None
 
                 full_name = self.determine_full_name(row, rank_name)
-                taxon = Taxon(
+                taxon = model(
                     id_taxonref=id_native,
                     id_family=int(taxon_ids["id_family"])
                     if pd.notna(taxon_ids["id_family"])
                     else None,
                     id_genus=int(taxon_ids["id_genus"])
                     if pd.notna(taxon_ids["id_genus"])
                     else None,
                     id_species=int(taxon_ids["id_species"])
                     if pd.notna(taxon_ids["id_species"])
                     else None,
                     id_infra=int(taxon_ids["id_infra"])
                     if pd.notna(taxon_ids["id_infra"])
                     else None,
                     rank_name=row.get("rank"),
-                    id_source=int(row.get("id_source")),
                     full_name=full_name,
                     parent_id=parent_id,
                 )
 
-                db.session.add(taxon)
-        db.commit_session()
+                session.add(taxon)
+        session.commit()
 
-    def determine_full_name(self, row: Any, rank_name: str) -> Any:
+    @staticmethod
+    def determine_full_name(row: Any, rank_name: str) -> Any:
         """
         Determine the full name for a given taxon rank.
 
         Parameters:
             row (pd.Series): Data row containing taxon information.
             rank_name (str): The rank name of the taxon.
 
@@ -191,14 +210,15 @@
 
     def perform_calculations(self, data: Any, taxonomy_config: Dict[str, Any]) -> None:
         """
         Perform calculations for each taxonomic level and update the Taxon objects in the database.
 
         Parameters:
             data (pd.DataFrame): The DataFrame containing occurrence data.
+            taxonomy_config (dict): The configuration defining the taxonomic ranks and their hierarchy.
         """
 
         processed_ranks = set()
 
         # Perform calculations for each taxonomic level
         for rank_name, taxon_config in taxonomy_config.items():
             rank = taxon_config.get("field")
@@ -211,16 +231,16 @@
 
     def process_group(self, data: Any, group_by_rank: str, rank_name: str) -> None:
         """
         Process a group of data for a given taxonomic level and update the database.
 
         Parameters:
             data (pd.DataFrame): The DataFrame containing the data to process.
-            ids (List[int]): List of unique identifiers for the taxonomic level.
-            group_by_field (str): The field to group by ('id_family', 'id_genus', etc.).
+            group_by_rank (str): The field to group the data by.
+            rank_name (str): The name of the taxonomic rank to process.
         """
         # Define the calculations to perform for each field
         calculations: Dict[
             str,
             Union[List[Union[str, Callable[..., Any]]], str, Callable[..., Any]],
         ] = {
             "dbh": ["mean", "max", "median"],
@@ -270,103 +290,21 @@
 
             grouped_data["occ_um_count"] = filtered_data.groupby(group_by_rank)[
                 "in_um"
             ].apply(lambda x: (x.astype(str).str.lower() == "true").sum())
 
             # Process and update Taxon objects with the calculated metrics
             for taxon_id, metrics in grouped_data.iterrows():
-                self.update_taxon(group_by_rank, taxon_id, metrics)
+                self.update_taxon(taxon_id, metrics)
 
             # Extract the coordinates from the filtered data
             coordinates = self.extract_coordinates(filtered_data)
 
             geo_json = {"type": "MultiPoint", "coordinates": coordinates}
 
-            for taxon_id, group in filtered_data.groupby(group_by_rank):
-                taxon = (
-                    self.db.session.query(Taxon).filter_by(id_taxonref=taxon_id).first()
-                )
-                if taxon:
-                    # Perform the frequency calculations for this taxon
-                    frequencies = self.calculate_frequencies(taxon_id, group)
-                    taxon.frequencies = frequencies  # type: ignore
-                    taxon.geo_pts_pn = geo_json  # type: ignore
-
-    def update_taxon(
-        self, group_by_field: str, taxon_id: int, update_data: Dict[str, Any]
-    ) -> None:
-        """
-        Update a Taxon object in the database with provided data.
-
-        Parameters:
-            taxon_id (int): The identifier of the Taxon to be updated.
-            update_data (dict): The data to update the Taxon with.
-        """
-        # Fetch the Taxon object from the database
-        taxon = self.db.session.query(Taxon).filter_by(id_taxonref=taxon_id).first()
-
-        if taxon:
-            # Update the Taxon object with the provided data
-            for attr, value in update_data.items():
-                setattr(taxon, attr, round(value, 2))
-
-            # Commit the changes to the database
-            self.db.commit_session()
-        else:
-            logger.error(f"Taxon with id {taxon_id} not found in the database.")
-
-    def extract_coordinates(self, filtered_data: Any) -> List[List[float]]:
-        """
-        Extract geographic coordinates from the filtered data.
-
-        Parameters:
-            filtered_data (pd.DataFrame): The DataFrame containing the filtered data.
-
-        Returns:
-            list: A list of coordinates.
-        """
-
-        # This code returns a list of coordinates. For each point in the 'geo_pt' column of the filtered_data DataFrame,
-        # it removes the "POINT (" and ")" strings, splits the remaining string into a list of strings,
-        # converts each string to a float, and adds the list of floats to the outer list.
-        # It only does this if the point is not NaN.
-        return [
-            list(map(float, str(point).replace("POINT (", "").replace(")", "").split()))
-            for point in filtered_data["geo_pt"]
-            if pd.notna(point)  # Check that the point is not NaN
-        ]
-
-    def get_unique_ids(self, field_name: str) -> List[int]:
-        """
-        Retrieve unique identifiers for a specified field from the database.
-
-        Parameters:
-            field_name (str): The field name to retrieve unique identifiers for.
-
-        Returns:
-            List[int]: A list of unique identifiers.
-        """
-        query = self.db.session.query(getattr(Taxon, field_name)).distinct()
-        unique_ids = [record[0] for record in query.all() if record[0] is not None]
-        return unique_ids
-
-    def map_attributes(self, column_name: str, attr_mapping: Any) -> Any:
-        """
-        Maps the attributes of a column name based on a given attribute mapping.
-
-        Args:
-            column_name (str): The name of the column to map the attributes of.
-            attr_mapping (dict): A dictionary containing the old attribute names as keys and the new attribute names as values.
-
-        Returns:
-            str: The column name with the attributes mapped according to the attribute mapping.
-        """
-        for old_attr, new_attr in attr_mapping.items():
-            column_name = column_name.replace(old_attr, new_attr)
-        return column_name
 
     def calculate_frequencies(
         self, taxon_id: int, group_data: Any
     ) -> dict[str, dict[str, float]]:
         """
         Calculate the frequencies for various measurements for a given taxon.
         """
@@ -438,15 +376,89 @@
         else:
             frequencies["rainfall"] = self.calculate_direct_distribution(
                 group_data["rainfall"], rainfall_bins
             )
 
         return frequencies
 
-    def process_field_data(self, data: Any, bins: List[int]) -> dict[Any, Any]:
+    def update_taxon(self, taxon_id: int, update_data: Dict[str, Any]) -> None:
+        """
+        Update a Taxon object in the database with provided data.
+
+        Parameters:
+            taxon_id (int): The identifier of the Taxon to be updated.
+            update_data (dict): The data to update the Taxon with.
+        """
+        # Fetch the Taxon object from the database
+        taxon = self.db.session.query(TaxonRef).filter_by(id_taxonref=taxon_id).first()
+
+        if taxon:
+            # Update the Taxon object with the provided data
+            for attr, value in update_data.items():
+                setattr(taxon, attr, round(value, 2))
+
+            # Commit the changes to the database
+            self.db.commit_session()
+        else:
+            logger.error(f"Taxon with id {taxon_id} not found in the database.")
+
+    @staticmethod
+    def extract_coordinates(filtered_data: Any) -> List[List[float]]:
+        """
+        Extract geographic coordinates from the filtered data.
+
+        Parameters:
+            filtered_data (pd.DataFrame): The DataFrame containing the filtered data.
+
+        Returns:
+            list: A list of coordinates.
+        """
+
+        # This code returns a list of coordinates. For each point in the 'geo_pt' column of the filtered_data DataFrame,
+        # it removes the "POINT (" and ")" strings, splits the remaining string into a list of strings,
+        # converts each string to a float, and adds the list of floats to the outer list.
+        # It only does this if the point is not NaN.
+        return [
+            list(map(float, str(point).replace("POINT (", "").replace(")", "").split()))
+            for point in filtered_data["geo_pt"]
+            if pd.notna(point)  # Check that the point is not NaN
+        ]
+
+    def get_unique_ids(self, field_name: str) -> List[int]:
+        """
+        Retrieve unique identifiers for a specified field from the database.
+
+        Parameters:
+            field_name (str): The field name to retrieve unique identifiers for.
+
+        Returns:
+            List[int]: A list of unique identifiers.
+        """
+        query = self.db.session.query(getattr(TaxonRef, field_name)).distinct()
+        unique_ids = [record[0] for record in query.all() if record[0] is not None]
+        return unique_ids
+
+    @staticmethod
+    def map_attributes(column_name: str, attr_mapping: Any) -> Any:
+        """
+        Maps the attributes of a column name based on a given attribute mapping.
+
+        Args:
+            column_name (str): The name of the column to map the attributes of.
+            attr_mapping (dict): A dictionary containing the old attribute names as keys and the new attribute names as values.
+
+        Returns:
+            str: The column name with the attributes mapped according to the attribute mapping.
+        """
+        for old_attr, new_attr in attr_mapping.items():
+            column_name = column_name.replace(old_attr, new_attr)
+        return column_name
+
+    @staticmethod
+    def process_field_data(data: Any, bins: List[int]) -> dict[Any, Any]:
         """
         Categorizes the field data into specified bins and calculates the frequencies for each category.
         The frequencies are then converted to percentages and returned as a dictionary.
 
         Args:
             data (Any): The dataset containing the field data.
             bins (List[int]): The list of bins to categorize the data.
@@ -539,15 +551,16 @@
             interval_label = f"{previous_bin_edge}-{bin_edge}"
             percentages_per_interval[interval_label] = percentage
 
             previous_bin_edge = bin_edge
 
         return percentages_per_interval
 
-    def extract_raster_values(self, geo_points: Any, raster_path: str) -> Any:
+    @staticmethod
+    def extract_raster_values(geo_points: Any, raster_path: str) -> Any:
         """Extract values for given geo points from a raster file."""
         raster_values = pd.Series([None] * len(geo_points))
 
         try:
             with rasterio.open(raster_path) as raster:
                 transformer = Transformer.from_crs(
                     "epsg:4326", raster.crs, always_xy=True
```

### Comparing `niamoto-0.0.1a2/src/niamoto/db/niamoto_repository.py` & `niamoto-0.0.2a1/src/niamoto/core/repositories/niamoto_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import os
-from niamoto.db.utils.database import Database
-from niamoto.db.models.models import Base
 from typing import Optional, Union, Callable, Any
 
+from niamoto.core.models import Base
+from niamoto.common.database import Database
+
 
 class NiamotoRepository:
     """
     The NiamotoRepository provides a data access layer to interact with the database.
     It allows fetching of entity objects defined by the SQLAlchemy ORM.
     """
 
     def __init__(self, db_path: str) -> None:
         """
         Initializes a new instance of the NiamotoRepository with a given database path.
 
         Args:
             db_path (str): The path to the database file.
         """
-        if not os.path.exists(db_path):
-            raise ValueError("Invalid database path")
         self.db = Database(db_path)
         self.session = self.db.session
 
     def get_entities(
         self,
         entity_class: Any,
         order_by: Optional[Union[Callable[[Any], Any], Any]] = None,
@@ -42,29 +40,29 @@
                 "Invalid entity_class argument. Must be a valid SQLAlchemy ORM class."
             )
         query = self.session.query(entity_class)
         if order_by is not None:
             query = query.order_by(order_by)
         return query.all()
 
+    @staticmethod
     def build_taxonomy_tree(taxons: Any) -> Any:
         rank_order = {"Famille": 1, "Genus": 2, "Species": 3, "Variety": 4}
 
-        # Tri des taxons selon le rang (les rangs non listés seront placés à la fin)
         sorted_taxons = sorted(taxons, key=lambda x: rank_order.get(x.rank_name, 5))
 
         tree = {}
         for taxon in sorted_taxons:
             tree[taxon.id] = {
                 "name": taxon.full_name,
                 "parent_id": taxon.parent_id,
                 "children": [],
             }
 
-        for id, node in tree.items():
+        for _id, node in tree.items():
             parent_id = node["parent_id"]
             if parent_id:
                 tree[parent_id]["children"].append(node)
 
         root_nodes = [node for node in tree.values() if node["parent_id"] is None]
         return root_nodes
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `niamoto-0.0.1a2/src/niamoto/static_site_generator/page_generator.py` & `niamoto-0.0.2a1/src/niamoto/publish/static_site_generator/page_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+import json
 import os
 import shutil
-import json
-import rjsmin  # type: ignore
+from typing import Any, List, Optional, Dict
+
 import jinja2
-from niamoto.common.config_manager import ConfigManager
-from niamoto.db.models.models import Taxon
-from typing import Any, List
+import rjsmin  # type: ignore
+
+from niamoto.core.models import TaxonRef
+from niamoto.common.config import Config
 
 
 class PageGenerator:
-    def __init__(self, config: ConfigManager) -> None:
+    def __init__(self, config: Config) -> None:
         """
         Initializes the PageGenerator class with configuration settings.
 
-        :param config: An instance of ConfigManager containing configuration settings.
+        Args:
+             config (Config): An instance of ConfigManager containing configuration settings.
+
+        Returns:
+            None
 
         Sets the template directory, static source directory, output directory, and static destination directory.
         Also configures the Jinja2 template environment.
         """
 
         self.config = config
 
@@ -28,68 +34,79 @@
             os.path.dirname(os.path.abspath(__file__)), "static"
         )
         self.output_dir = self.config.get("web", "static_pages")
 
         template_loader = jinja2.FileSystemLoader(searchpath=self.template_dir)
         self.template_env = jinja2.Environment(loader=template_loader)
 
-    def generate_taxon_page(self, taxon: Taxon) -> str:
+    def generate_taxon_page(
+        self, taxon: TaxonRef, stats: Optional[Any], mapping: Dict[Any, Any]
+    ) -> str:
         """
         Generates a webpage for a given taxon object.
 
         Args:
-            taxon (Taxon): The taxon object for which the webpage is generated.
+            taxon (TaxonRef): The taxon object for which the webpage is generated.
+            stats (dict, optional): A dictionary containing statistics for the taxon.
+            mapping (dict): The mapping dictionary containing the configuration for generating the webpage.
 
         Returns:
             str: The path of the generated webpage.
         """
         template = self.template_env.get_template("taxon_template.html")
-        taxon_dict = self.taxon_to_dict(taxon)
-        html_output = template.render(taxon=taxon_dict)
+        taxon_dict = self.taxon_to_dict(taxon, stats)
 
+        html_output = template.render(taxon=taxon_dict, stats=stats, mapping=mapping)
         taxon_output_dir = os.path.join(self.output_dir, "pages", "taxon")
         os.makedirs(taxon_output_dir, exist_ok=True)
-
-        output_path = os.path.join(taxon_output_dir, f"{taxon.id_taxonref}.html")
+        output_path = os.path.join(taxon_output_dir, f"{taxon.id}.html")
         with open(output_path, "w") as file:
             file.write(html_output)
-
         self.copy_static_files()
-
         return output_path
 
-    def generate_taxonomy_tree_js(self, taxons: List[Taxon]) -> None:
+    def generate_taxonomy_tree_js(self, taxons: List[TaxonRef]) -> None:
         tree = self.build_taxonomy_tree(taxons)
         js_content = "const taxonomyData = " + json.dumps(tree, indent=4) + ";"
         minified_js = rjsmin.jsmin(js_content)
 
         js_path = os.path.join(self.output_dir, "js", "taxonomy_tree.js")
         with open(js_path, "w") as file:
             file.write(minified_js)
 
-    @staticmethod
-    def build_taxonomy_tree(taxons: List[Any]) -> Any:
-        tree = {}
+    def build_taxonomy_tree(self, taxons: List[TaxonRef]) -> List[Dict[Any, Any]]:
+        taxons_by_id = {int(taxon.id): taxon for taxon in taxons}
+        tree = []
+
         for taxon in taxons:
-            if taxon.full_name is None:
-                continue
-            tree[taxon.id] = {
-                "id": taxon.id_taxonref,
-                "name": taxon.full_name,
-                "parent_id": taxon.parent_id,
-                "children": [],
-            }
-
-        for id, node in tree.items():
-            parent_id = node["parent_id"]
-            if parent_id and parent_id in tree:
-                tree[parent_id]["children"].append(node)
+            if taxon.parent_id is None:
+                tree.append(self.build_subtree(taxon, taxons_by_id))
+
+        return tree
+
+    def build_subtree(
+        self, taxon: TaxonRef, taxons_by_id: Dict[int, TaxonRef]
+    ) -> Dict[str, Any]:
+        node: Dict[str, Any] = {
+            "id": taxon.id,
+            "name": taxon.full_name,
+            "children": [],
+        }
 
-        root_nodes = [node for node in tree.values() if node["parent_id"] is None]
-        return root_nodes
+        left = taxon.lft
+        right = taxon.rght
+
+        for child_id, child_taxon in taxons_by_id.items():
+            if (
+                child_taxon.parent_id == taxon.id
+                and left < child_taxon.lft < child_taxon.rght < right
+            ):
+                node["children"].append(self.build_subtree(child_taxon, taxons_by_id))
+
+        return node
 
     def copy_static_files(self) -> None:
         """
         Copies static files to the destination directory, overwriting existing files.
 
         The destination directory is created if it doesn't exist.
         """
@@ -103,49 +120,47 @@
 
             if os.path.isdir(src_path):
                 # shutil.copytree will overwrite files in the destination directory if dirs_exist_ok=True
                 shutil.copytree(src_path, dest_path, dirs_exist_ok=True)
             else:
                 shutil.copy2(src_path, dest_path)
 
-    @staticmethod
-    def taxon_to_dict(taxon: Taxon) -> dict[str, Any]:
+    def taxon_to_dict(self, taxon: TaxonRef, stats: Optional[Any]) -> dict[str, Any]:
         """
-        Converts a Taxon object to a dictionary.
+        Converts a TaxonRef object and its associated statistics to a dictionary.
 
         Args:
-            taxon: A Taxon object.
+            taxon (TaxonRef): A TaxonRef object.
+            stats (dict, optional): A dictionary containing statistics for the taxon.
 
         Returns:
-            A dictionary representing the taxon data.
+            dict[str, Any]: A dictionary representing the taxon data and its statistics.
         """
-        return {
+        taxon_dict = {
             "id": taxon.id,
             "full_name": taxon.full_name,
+            "authors": taxon.authors,
             "rank_name": taxon.rank_name,
-            "occ_count": taxon.occ_count,
-            "occ_um_count": taxon.occ_um_count,
-            "dbh_max": taxon.dbh_max,
-            "dbh_avg": taxon.dbh_avg,
-            "freq_max": taxon.freq_max,
-            "height_max": taxon.height_max,
-            "wood_density_avg": taxon.wood_density_avg,
-            "wood_density_min": taxon.wood_density_min,
-            "wood_density_max": taxon.wood_density_max,
-            "bark_thickness_avg": taxon.bark_thickness_avg,
-            "bark_thickness_min": taxon.bark_thickness_min,
-            "bark_thickness_max": taxon.bark_thickness_max,
-            "leaf_sla_avg": taxon.leaf_sla_avg,
-            "leaf_sla_min": taxon.leaf_sla_min,
-            "leaf_sla_max": taxon.leaf_sla_max,
-            "leaf_area_avg": taxon.leaf_area_avg,
-            "leaf_area_min": taxon.leaf_area_min,
-            "leaf_area_max": taxon.leaf_area_max,
-            "leaf_thickness_avg": taxon.leaf_thickness_avg,
-            "leaf_thickness_min": taxon.leaf_thickness_min,
-            "leaf_thickness_max": taxon.leaf_thickness_max,
-            "leaf_ldmc_avg": taxon.leaf_ldmc_avg,
-            "leaf_ldmc_min": taxon.leaf_ldmc_min,
-            "leaf_ldmc_max": taxon.leaf_ldmc_max,
-            "frequencies": taxon.frequencies,
-            "geo_pts_pn": taxon.geo_pts_pn,
+            "lft": taxon.lft,
+            "rght": taxon.rght,
+            "level": taxon.level,
+            "parent_id": taxon.parent_id,
         }
+
+        if stats:
+            frequencies = {}
+            for key, value in stats.items():
+                if key.endswith("_bins"):
+                    freq_key = key[:-5]  # Remove the "_bins" suffix
+                    freq_key = freq_key.replace(
+                        "_", "-"
+                    )  # Replace "_" with "-" for other keys
+                    if value is not None:  # Check if value is not None
+                        frequencies[freq_key] = json.loads(
+                            value.replace("'", '"')
+                        )  # Parse the JSON string
+                else:
+                    taxon_dict[key] = value
+
+            taxon_dict["frequencies"] = frequencies
+
+        return taxon_dict
```

