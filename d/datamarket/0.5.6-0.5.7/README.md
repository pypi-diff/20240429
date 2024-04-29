# Comparing `tmp/datamarket-0.5.6.tar.gz` & `tmp/datamarket-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.5.6.tar", last modified: Mon Apr 29 14:56:20 2024, max compression
+gzip compressed data, was "datamarket-0.5.7.tar", last modified: Mon Apr 29 15:23:23 2024, max compression
```

## Comparing `datamarket-0.5.6.tar` & `datamarket-0.5.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.159464 datamarket-0.5.6/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)    35149 2024-04-29 13:44:53.000000 datamarket-0.5.6/LICENSE
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1692 2024-04-29 14:56:20.158464 datamarket-0.5.6/PKG-INFO
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      934 2024-04-29 13:44:53.000000 datamarket-0.5.6/README.md
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       38 2024-04-29 14:56:20.159464 datamarket-0.5.6/setup.cfg
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1080 2024-04-29 14:55:33.000000 datamarket-0.5.6/setup.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.150464 datamarket-0.5.6/src/
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.152464 datamarket-0.5.6/src/datamarket/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       12 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/__init__.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.156464 datamarket-0.5.6/src/datamarket/interfaces/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/__init__.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     4214 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/alchemy.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1252 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/aws.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2915 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/drive.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1344 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/ftp.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     3002 2024-04-29 14:48:37.000000 datamarket-0.5.6/src/datamarket/interfaces/nominatim.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2913 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/proxy.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2565 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/tinybird.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.156464 datamarket-0.5.6/src/datamarket/params/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/params/__init__.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1143 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/params/nominatim.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.157464 datamarket-0.5.6/src/datamarket/utils/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       20 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/__init__.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      635 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/alchemy.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2270 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/main.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2499 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/selenium.py
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      941 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/soda.py
-drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.158464 datamarket-0.5.6/src/datamarket.egg-info/
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1692 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/PKG-INFO
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      755 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/SOURCES.txt
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        1 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/dependency_links.txt
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       86 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/requires.txt
--rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       11 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/top_level.txt
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 15:23:23.710522 datamarket-0.5.7/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)    35149 2024-04-29 13:44:53.000000 datamarket-0.5.7/LICENSE
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1692 2024-04-29 15:23:23.710522 datamarket-0.5.7/PKG-INFO
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      934 2024-04-29 13:44:53.000000 datamarket-0.5.7/README.md
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       38 2024-04-29 15:23:23.711521 datamarket-0.5.7/setup.cfg
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1080 2024-04-29 15:22:50.000000 datamarket-0.5.7/setup.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 15:23:23.699522 datamarket-0.5.7/src/
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 15:23:23.701521 datamarket-0.5.7/src/datamarket/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       12 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/__init__.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 15:23:23.706522 datamarket-0.5.7/src/datamarket/interfaces/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/interfaces/__init__.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     4214 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/interfaces/alchemy.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1252 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/interfaces/aws.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2915 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/interfaces/drive.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1344 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/interfaces/ftp.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     3147 2024-04-29 15:22:05.000000 datamarket-0.5.7/src/datamarket/interfaces/nominatim.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2913 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/interfaces/proxy.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2565 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/interfaces/tinybird.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 15:23:23.707522 datamarket-0.5.7/src/datamarket/params/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/params/__init__.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1143 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/params/nominatim.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 15:23:23.709522 datamarket-0.5.7/src/datamarket/utils/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       20 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/utils/__init__.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      635 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/utils/alchemy.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2270 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/utils/main.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2499 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/utils/selenium.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      941 2024-04-29 13:44:53.000000 datamarket-0.5.7/src/datamarket/utils/soda.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 15:23:23.709522 datamarket-0.5.7/src/datamarket.egg-info/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1692 2024-04-29 15:23:23.000000 datamarket-0.5.7/src/datamarket.egg-info/PKG-INFO
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      755 2024-04-29 15:23:23.000000 datamarket-0.5.7/src/datamarket.egg-info/SOURCES.txt
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        1 2024-04-29 15:23:23.000000 datamarket-0.5.7/src/datamarket.egg-info/dependency_links.txt
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       86 2024-04-29 15:23:23.000000 datamarket-0.5.7/src/datamarket.egg-info/requires.txt
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       11 2024-04-29 15:23:23.000000 datamarket-0.5.7/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.5.6/LICENSE` & `datamarket-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/PKG-INFO` & `datamarket-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.6
+Version: 0.5.7
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.5.6/README.md` & `datamarket-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/setup.py` & `datamarket-0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "undetected_chromedriver",
     "pendulum",
     "boto3",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.5.6",
+    version="0.5.7",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.5.6/src/datamarket/interfaces/alchemy.py` & `datamarket-0.5.7/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/interfaces/aws.py` & `datamarket-0.5.7/src/datamarket/interfaces/aws.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/interfaces/drive.py` & `datamarket-0.5.7/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/interfaces/ftp.py` & `datamarket-0.5.7/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/interfaces/nominatim.py` & `datamarket-0.5.7/src/datamarket/interfaces/nominatim.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,17 @@
     @staticmethod
     def get_province_from_postcode(postcode):
         if postcode:
             return POSTCODES[postcode[:2]]
 
 
 class Nominatim:
-    def __init__(self, endpoint : str, geonames : GeoNames):
-        self.endpoint = endpoint
-        self.geonames = geonames
+    def __init__(self, nominatim_endpoint, geonames_endpoint):
+        self.endpoint = nominatim_endpoint
+        self.geonames = GeoNames(geonames_endpoint)
     
     @staticmethod
     def get_attribute(raw_json, keys):
         for key in keys:
             if key in raw_json:
                 return raw_json[key]
 
@@ -81,13 +81,14 @@
 
 
 class NominatimInterface(Nominatim):
     def __init__(self, config):
         if "osm" in config:
             self.config = config["osm"]
 
-            self.endpoint = self.config["nominatim_endpoint"]
+            self.nominatim_endpoint = self.config["nominatim_endpoint"]
+            self.geonames_endpoint = self.config["geonames_endpoint"]
 
         else:
             logger.warning("no osm section in config")
 
-        super().__init__(self.endpoint)
+        super().__init__(self.nominatim_endpoint, self.geonames_endpoint)
```

### Comparing `datamarket-0.5.6/src/datamarket/interfaces/proxy.py` & `datamarket-0.5.7/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/interfaces/tinybird.py` & `datamarket-0.5.7/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/params/nominatim.py` & `datamarket-0.5.7/src/datamarket/params/nominatim.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/utils/alchemy.py` & `datamarket-0.5.7/src/datamarket/utils/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/utils/main.py` & `datamarket-0.5.7/src/datamarket/utils/main.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/utils/selenium.py` & `datamarket-0.5.7/src/datamarket/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket/utils/soda.py` & `datamarket-0.5.7/src/datamarket/utils/soda.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.6/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.5.7/src/datamarket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.6
+Version: 0.5.7
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.5.6/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.5.7/src/datamarket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

