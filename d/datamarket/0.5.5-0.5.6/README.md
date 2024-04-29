# Comparing `tmp/datamarket-0.5.5.tar.gz` & `tmp/datamarket-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamarket-0.5.5.tar", last modified: Mon Apr  8 12:26:12 2024, max compression
+gzip compressed data, was "datamarket-0.5.6.tar", last modified: Mon Apr 29 14:56:20 2024, max compression
```

## Comparing `datamarket-0.5.5.tar` & `datamarket-0.5.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:26:12.677461 datamarket-0.5.5/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)    35149 2024-04-02 08:28:11.000000 datamarket-0.5.5/LICENSE
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1692 2024-04-08 12:26:12.677461 datamarket-0.5.5/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      934 2024-04-02 08:28:11.000000 datamarket-0.5.5/README.md
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       38 2024-04-08 12:26:12.677461 datamarket-0.5.5/setup.cfg
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1080 2024-04-08 12:26:08.000000 datamarket-0.5.5/setup.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:26:12.669461 datamarket-0.5.5/src/
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:26:12.669461 datamarket-0.5.5/src/datamarket/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       12 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/__init__.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:26:12.673461 datamarket-0.5.5/src/datamarket/interfaces/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/interfaces/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     4214 2024-04-08 12:15:49.000000 datamarket-0.5.5/src/datamarket/interfaces/alchemy.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1252 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/interfaces/aws.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2915 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/interfaces/drive.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1344 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/interfaces/ftp.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2730 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/interfaces/nominatim.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2913 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/interfaces/proxy.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2565 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/interfaces/tinybird.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:26:12.673461 datamarket-0.5.5/src/datamarket/params/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        0 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/params/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     1143 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/params/nominatim.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:26:12.673461 datamarket-0.5.5/src/datamarket/utils/
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       20 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/utils/__init__.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      635 2024-04-08 11:53:46.000000 datamarket-0.5.5/src/datamarket/utils/alchemy.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2270 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/utils/main.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)     2499 2024-04-02 08:28:11.000000 datamarket-0.5.5/src/datamarket/utils/selenium.py
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      941 2024-04-02 08:51:09.000000 datamarket-0.5.5/src/datamarket/utils/soda.py
-drwxrwxr-x   0 adrian    (1000) adrian    (1000)        0 2024-04-08 12:26:12.673461 datamarket-0.5.5/src/datamarket.egg-info/
--rw-r--r--   0 adrian    (1000) adrian    (1000)     1692 2024-04-08 12:26:12.000000 datamarket-0.5.5/src/datamarket.egg-info/PKG-INFO
--rw-rw-r--   0 adrian    (1000) adrian    (1000)      755 2024-04-08 12:26:12.000000 datamarket-0.5.5/src/datamarket.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)        1 2024-04-08 12:26:12.000000 datamarket-0.5.5/src/datamarket.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       86 2024-04-08 12:26:12.000000 datamarket-0.5.5/src/datamarket.egg-info/requires.txt
--rw-rw-r--   0 adrian    (1000) adrian    (1000)       11 2024-04-08 12:26:12.000000 datamarket-0.5.5/src/datamarket.egg-info/top_level.txt
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.159464 datamarket-0.5.6/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)    35149 2024-04-29 13:44:53.000000 datamarket-0.5.6/LICENSE
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1692 2024-04-29 14:56:20.158464 datamarket-0.5.6/PKG-INFO
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      934 2024-04-29 13:44:53.000000 datamarket-0.5.6/README.md
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       38 2024-04-29 14:56:20.159464 datamarket-0.5.6/setup.cfg
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1080 2024-04-29 14:55:33.000000 datamarket-0.5.6/setup.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.150464 datamarket-0.5.6/src/
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.152464 datamarket-0.5.6/src/datamarket/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       12 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/__init__.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.156464 datamarket-0.5.6/src/datamarket/interfaces/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/__init__.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     4214 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/alchemy.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1252 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/aws.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2915 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/drive.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1344 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/ftp.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     3002 2024-04-29 14:48:37.000000 datamarket-0.5.6/src/datamarket/interfaces/nominatim.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2913 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/proxy.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2565 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/interfaces/tinybird.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.156464 datamarket-0.5.6/src/datamarket/params/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/params/__init__.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1143 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/params/nominatim.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.157464 datamarket-0.5.6/src/datamarket/utils/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       20 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/__init__.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      635 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/alchemy.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2270 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/main.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     2499 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/selenium.py
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      941 2024-04-29 13:44:53.000000 datamarket-0.5.6/src/datamarket/utils/soda.py
+drwxr-xr-x   0 ajimenez  (1000) ajimenez  (1000)        0 2024-04-29 14:56:20.158464 datamarket-0.5.6/src/datamarket.egg-info/
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)     1692 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/PKG-INFO
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)      755 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/SOURCES.txt
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)        1 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/dependency_links.txt
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       86 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/requires.txt
+-rw-r--r--   0 ajimenez  (1000) ajimenez  (1000)       11 2024-04-29 14:56:20.000000 datamarket-0.5.6/src/datamarket.egg-info/top_level.txt
```

### Comparing `datamarket-0.5.5/LICENSE` & `datamarket-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/PKG-INFO` & `datamarket-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.5
+Version: 0.5.6
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.5.5/README.md` & `datamarket-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/setup.py` & `datamarket-0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "undetected_chromedriver",
     "pendulum",
     "boto3",
 ]
 
 setuptools.setup(
     name="datamarket",
-    version="0.5.5",
+    version="0.5.6",
     author="DataMarket",
     author_email="techsupport@datamarket.es",
     description="Utilities that integrate advance scraping knowledge into just one library.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Data-Market/datamarket",
     project_urls={
```

### Comparing `datamarket-0.5.5/src/datamarket/interfaces/alchemy.py` & `datamarket-0.5.6/src/datamarket/interfaces/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/interfaces/aws.py` & `datamarket-0.5.6/src/datamarket/interfaces/aws.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/interfaces/drive.py` & `datamarket-0.5.6/src/datamarket/interfaces/drive.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/interfaces/ftp.py` & `datamarket-0.5.6/src/datamarket/interfaces/ftp.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/interfaces/nominatim.py` & `datamarket-0.5.6/src/datamarket/interfaces/nominatim.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,40 @@
 from ..params.nominatim import POSTCODES
 
 ########################################################################################################################
 # CLASSES
 
 logger = logging.getLogger(__name__)
 
+class GeoNames:
+    def __init__(self, endpoint):
+        self.endpoint = endpoint
+
+    def get_postcode(self, lat, lon):
+        response = requests.get(f"{self.endpoint}/postcode?lat={lat}&lon={lon}").json()
+        postcode = str(response.get("postal_code", ""))
+        if postcode and len(postcode) == 5 and postcode[:2] in POSTCODES:
+            return postcode
+
+    @staticmethod
+    def get_province_from_postcode(postcode):
+        if postcode:
+            return POSTCODES[postcode[:2]]
+
 
 class Nominatim:
-    def __init__(self, endpoint):
+    def __init__(self, endpoint : str, geonames : GeoNames):
         self.endpoint = endpoint
+        self.geonames = geonames
+    
+    @staticmethod
+    def get_attribute(raw_json, keys):
+        for key in keys:
+            if key in raw_json:
+                return raw_json[key]
 
     def geocode(self, address):
         return requests.get(f"{self.endpoint}/?q={address}&format=json").json()
 
     def geocode_parsed(self, address):
         results = self.geocode(address)
 
@@ -28,45 +50,29 @@
 
     def reverse(self, lat, lon):
         return requests.get(f"{self.endpoint}/reverse?lat={lat}&lon={lon}&format=json").json()
 
     def reverse_parsed(self, lat, lon):
         raw_json = self.reverse(lat, lon).get("address", {})
 
-        postcode = self.validate_postcode(raw_json.get("postcode"))
+        postcode = self.geonames.get_postcode(lat, lon)
         district, quarter = self.get_district_quarter(raw_json)
         return {
             "country": raw_json.get("country"),
             "country_code": raw_json.get("country_code"),
             "state": raw_json.get("state"),
-            "province": self.get_province_from_postcode(postcode),
+            "province": self.geonames.get_province_from_postcode(postcode),
             "city": self.get_attribute(raw_json, ["city", "town", "village"]),
             "postcode": postcode,
             "district": district,
             "quarter": quarter,
             "street": raw_json.get("road"),
             "number": raw_json.get("house_number"),
         }
 
-    @staticmethod
-    def validate_postcode(postcode):
-        if postcode and len(postcode) == 5 and postcode[:2] in POSTCODES:
-            return postcode
-
-    @staticmethod
-    def get_province_from_postcode(postcode):
-        if postcode:
-            return POSTCODES[postcode[:2]]
-
-    @staticmethod
-    def get_attribute(raw_json, keys):
-        for key in keys:
-            if key in raw_json:
-                return raw_json[key]
-
     def get_district_quarter(self, raw_json):
         district = self.get_attribute(raw_json, ["city_district", "suburb", "borough"])
         quarter = self.get_attribute(raw_json, ["quarter", "neighbourhood"])
 
         if not district and quarter:
             district = quarter
             quarter = None
```

### Comparing `datamarket-0.5.5/src/datamarket/interfaces/proxy.py` & `datamarket-0.5.6/src/datamarket/interfaces/proxy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/interfaces/tinybird.py` & `datamarket-0.5.6/src/datamarket/interfaces/tinybird.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/params/nominatim.py` & `datamarket-0.5.6/src/datamarket/params/nominatim.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/utils/alchemy.py` & `datamarket-0.5.6/src/datamarket/utils/alchemy.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/utils/main.py` & `datamarket-0.5.6/src/datamarket/utils/main.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/utils/selenium.py` & `datamarket-0.5.6/src/datamarket/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket/utils/soda.py` & `datamarket-0.5.6/src/datamarket/utils/soda.py`

 * *Files identical despite different names*

### Comparing `datamarket-0.5.5/src/datamarket.egg-info/PKG-INFO` & `datamarket-0.5.6/src/datamarket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamarket
-Version: 0.5.5
+Version: 0.5.6
 Summary: Utilities that integrate advance scraping knowledge into just one library.
 Home-page: https://github.com/Data-Market/datamarket
 Author: DataMarket
 Author-email: techsupport@datamarket.es
 Project-URL: Website, https://datamarket.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `datamarket-0.5.5/src/datamarket.egg-info/SOURCES.txt` & `datamarket-0.5.6/src/datamarket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

