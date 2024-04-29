# Comparing `tmp/parcllabs-0.1.7.tar.gz` & `tmp/parcllabs-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parcllabs-0.1.7.tar", last modified: Fri Apr 26 20:33:19 2024, max compression
+gzip compressed data, was "parcllabs-0.1.8.tar", last modified: Mon Apr 29 00:09:16 2024, max compression
```

## Comparing `parcllabs-0.1.7.tar` & `parcllabs-0.1.8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.440753 parcllabs-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-26 20:32:45.000000 parcllabs-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 20:33:19.436753 parcllabs-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-04-26 20:32:45.000000 parcllabs-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/parcllabs/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/plabs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/parcllabs/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/search/metros.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/search/top_markets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/parcllabs/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-26 20:33:16.000000 parcllabs-0.1.7/parcllabs/services/base_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/for_sale_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/investor_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/portfolio_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-26 20:32:45.000000 parcllabs-0.1.7/parcllabs/services/rental_market_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/parcllabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 20:33:19.000000 parcllabs-0.1.7/parcllabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:33:19.440753 parcllabs-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-26 20:32:45.000000 parcllabs-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:33:19.436753 parcllabs-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-26 20:32:45.000000 parcllabs-0.1.7/tests/test_for_sale_market_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-26 20:32:45.000000 parcllabs-0.1.7/tests/test_parcl_labs_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-26 20:32:45.000000 parcllabs-0.1.7/tests/test_parcl_labs_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.425693 parcllabs-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 00:08:33.000000 parcllabs-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-29 00:09:16.425693 parcllabs-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-04-29 00:08:33.000000 parcllabs-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.417693 parcllabs-0.1.8/parcllabs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-29 00:09:12.000000 parcllabs-0.1.8/parcllabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-29 00:09:13.000000 parcllabs-0.1.8/parcllabs/plabs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.421693 parcllabs-0.1.8/parcllabs/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/search/metros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/search/top_markets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.421693 parcllabs-0.1.8/parcllabs/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-29 00:09:13.000000 parcllabs-0.1.8/parcllabs/services/base_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/for_sale_market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10276 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/investor_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13414 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/portfolio_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-29 00:08:33.000000 parcllabs-0.1.8/parcllabs/services/rental_market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-29 00:09:13.000000 parcllabs-0.1.8/parcllabs/services/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.421693 parcllabs-0.1.8/parcllabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 00:09:16.000000 parcllabs-0.1.8/parcllabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 00:09:16.425693 parcllabs-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-29 00:08:33.000000 parcllabs-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 00:09:16.421693 parcllabs-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-29 00:08:33.000000 parcllabs-0.1.8/tests/test_for_sale_market_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-29 00:08:33.000000 parcllabs-0.1.8/tests/test_parcl_labs_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 00:08:33.000000 parcllabs-0.1.8/tests/test_parcl_labs_service.py
```

### Comparing `parcllabs-0.1.7/LICENSE` & `parcllabs-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/PKG-INFO` & `parcllabs-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parcllabs
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SDK for ParclLabs API
 Home-page: https://github.com/ParclLabs/parcllabs-python
 Author: ParclLabs
 Author-email: team@parcllabs.com
 Keywords: parcllabs api real estate analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `parcllabs-0.1.7/README.md` & `parcllabs-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,50 @@
 ![Logo](img/labs.jpg)
 # parcllabs-python
 
 ## Sign Up for an API Key
 
-To use the ParclLabs API, you need an API key. To get an API key, sign up at [ParclLabs](https://dashboard.parcllabs.com/signup).
+To use the Parcl Labs API, you need an API key. To get an API key, sign up at [ParclLabs](https://dashboard.parcllabs.com/signup).
 
 ## Installation
 
 You can install the package via pip:
 
 ```bash
 pip install parcllabs
 ```
 
+### Search
+Search is your entry point into finding one or many of over 70,000 markets in the United States. You can search for markets by name, state, region, fips, or zip code. You can also search for markets by their Parcl ID.
+
+#### Search Markets
+```python
+import os
+
+from parcllabs import ParclLabsClient
+
+
+api_key = os.getenv('PARCLLABS_API_KEY')
+client = ParclLabsClient(api_key)
+
+# all cities in EAST_NORTH_CENTRAL census region
+results = client.search.markets.retrieve_many(
+    location_type='CITY',
+    region='EAST_NORTH_CENTRAL',
+    as_dataframe=True
+)
+print(results.head())
+#     parcl_id country    geoid state_fips_code             name state_abbreviation              region location_type
+# 0    5333443     USA  5500100              55  Abbotsford City                 WI  EAST_NORTH_CENTRAL          CITY
+# 1    5387920     USA  1700113              17    Abingdon City                 IL  EAST_NORTH_CENTRAL          CITY
+# 2    5403368     USA  5500275              55       Adams City                 WI  EAST_NORTH_CENTRAL          CITY
+# 3    5278505     USA  2600440              26      Adrian City                 MI  EAST_NORTH_CENTRAL          CITY
+# 4    5332624     USA  3901000              39       Akron City                 OH  EAST_NORTH_CENTRAL          CITY
+```
+
 ### Rental Market Metrics
 
 #### Gross Yield
 Gets the percent gross yield for a specified <parcl_id>. At the market level, identified by <parcl_id>, gross yield is calculated by dividing the annual median rental income—derived from multiplying the monthly median new rental listing price by 12—by its median new listings for sale price.
 
 #### Rental Units Concentration
 Gets the number of rental units, total units, and percent rental unit concentration for a specified <parcl_id>.
```

### Comparing `parcllabs-0.1.7/parcllabs/__init__.py` & `parcllabs-0.1.8/parcllabs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,7 +30,8 @@
 
 from parcllabs.services.rental_market_metrics import (
     RentalMarketMetricsRentalUnitsConcentration,
     RentalMarketMetricsGrossYield,
 )
 
 from parcllabs.services.portfolio_metrics import PortfolioMetricsSFHousingStockOwnership
+from parcllabs.services.search import SearchMarkets
```

### Comparing `parcllabs-0.1.7/parcllabs/plabs_client.py` & `parcllabs-0.1.8/parcllabs/plabs_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 from parcllabs.services.rental_market_metrics import (
     RentalMarketMetricsRentalUnitsConcentration,
     RentalMarketMetricsGrossYield,
 )
 
 from parcllabs.services.portfolio_metrics import PortfolioMetricsSFHousingStockOwnership
+from parcllabs.services.search import SearchMarkets
 
 
 class ParclLabsClient:
     def __init__(self, api_key: str):
         if api_key is None:
             raise ValueError("api_key is required")
         self.api_key = api_key
@@ -66,14 +67,15 @@
         )
         self.rental_market_metrics_gross_yield = RentalMarketMetricsGrossYield(
             client=self
         )
         self.portfolio_metrics_sf_housing_stock_ownership = (
             PortfolioMetricsSFHousingStockOwnership(client=self)
         )
+        self.search_markets = SearchMarkets(client=self)
 
     def get(self, url: str, params: dict = None):
         """
         Send a GET request to the specified URL with the given parameters.
 
         Args:
             url (str): The URL endpoint to request.
```

### Comparing `parcllabs-0.1.7/parcllabs/search/metros.py` & `parcllabs-0.1.8/parcllabs/search/metros.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/parcllabs/services/base_service.py` & `parcllabs-0.1.8/parcllabs/services/base_service.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/parcllabs/services/for_sale_market_metrics.py` & `parcllabs-0.1.8/parcllabs/services/for_sale_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/parcllabs/services/investor_metrics.py` & `parcllabs-0.1.8/parcllabs/services/investor_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/parcllabs/services/market_metrics.py` & `parcllabs-0.1.8/parcllabs/services/market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/parcllabs/services/portfolio_metrics.py` & `parcllabs-0.1.8/parcllabs/services/portfolio_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/parcllabs/services/rental_market_metrics.py` & `parcllabs-0.1.8/parcllabs/services/rental_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/parcllabs.egg-info/PKG-INFO` & `parcllabs-0.1.8/parcllabs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parcllabs
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python SDK for ParclLabs API
 Home-page: https://github.com/ParclLabs/parcllabs-python
 Author: ParclLabs
 Author-email: team@parcllabs.com
 Keywords: parcllabs api real estate analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `parcllabs-0.1.7/parcllabs.egg-info/SOURCES.txt` & `parcllabs-0.1.8/parcllabs.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,10 +15,11 @@
 parcllabs/services/__init__.py
 parcllabs/services/base_service.py
 parcllabs/services/for_sale_market_metrics.py
 parcllabs/services/investor_metrics.py
 parcllabs/services/market_metrics.py
 parcllabs/services/portfolio_metrics.py
 parcllabs/services/rental_market_metrics.py
+parcllabs/services/search.py
 tests/test_for_sale_market_metrics.py
 tests/test_parcl_labs_clients.py
 tests/test_parcl_labs_service.py
```

### Comparing `parcllabs-0.1.7/setup.py` & `parcllabs-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/tests/test_for_sale_market_metrics.py` & `parcllabs-0.1.8/tests/test_for_sale_market_metrics.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/tests/test_parcl_labs_clients.py` & `parcllabs-0.1.8/tests/test_parcl_labs_clients.py`

 * *Files identical despite different names*

### Comparing `parcllabs-0.1.7/tests/test_parcl_labs_service.py` & `parcllabs-0.1.8/tests/test_parcl_labs_service.py`

 * *Files identical despite different names*

