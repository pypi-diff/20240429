# Comparing `tmp/pydolarvenezuela-1.5.1.tar.gz` & `tmp/pydolarvenezuela-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydolarvenezuela-1.5.1.tar", last modified: Sun Apr 28 16:04:46 2024, max compression
+gzip compressed data, was "pydolarvenezuela-1.5.2.tar", last modified: Mon Apr 29 16:13:07 2024, max compression
```

## Comparing `pydolarvenezuela-1.5.1.tar` & `pydolarvenezuela-1.5.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.640573 pydolarvenezuela-1.5.1/
--rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     7209 2024-04-28 16:04:46.635504 pydolarvenezuela-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     4818 2024-04-28 12:19:05.000000 pydolarvenezuela-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.513172 pydolarvenezuela-1.5.1/pyDolarVenezuela/
--rw-rw-rw-   0        0        0     2712 2024-04-28 16:02:13.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.546367 pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/
--rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.546367 pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/icons/
--rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/icons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.563226 pydolarvenezuela-1.5.1/pyDolarVenezuela/data/
--rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/data/__init__.py
--rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/data/redis.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.581247 pydolarvenezuela-1.5.1/pyDolarVenezuela/models/
--rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/models/__init__.py
--rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/models/database.py
--rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/models/pages.py
--rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/network.py
--rw-rw-rw-   0        0        0      740 2024-04-28 11:38:43.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/pages.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.611897 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/
--rw-rw-rw-   0        0        0     5149 2024-04-28 15:09:31.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/__init__.py
--rw-rw-rw-   0        0        0     2141 2024-04-28 15:44:15.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/bcv.py
--rw-rw-rw-   0        0        0     1846 2024-04-28 12:10:50.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/criptodolar.py
--rw-rw-rw-   0        0        0     2315 2024-04-28 12:10:54.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/exchangemonitor.py
--rw-rw-rw-   0        0        0     1037 2024-04-28 12:10:58.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/italcambio.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.618121 pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/
--rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/__init__.py
--rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/calculator.py
--rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/time.py
--rw-rw-rw-   0        0        0     2236 2024-04-28 11:49:26.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-28 16:04:46.632505 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/
--rw-rw-rw-   0        0        0     7209 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      897 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-28 16:04:46.000000 pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-04-28 16:02:26.000000 pydolarvenezuela-1.5.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 16:04:46.640573 pydolarvenezuela-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1488 2024-04-28 16:02:19.000000 pydolarvenezuela-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.896654 pydolarvenezuela-1.5.2/
+-rw-rw-rw-   0        0        0     1094 2023-10-12 04:26:29.000000 pydolarvenezuela-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0     7221 2024-04-29 16:13:07.893655 pydolarvenezuela-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4830 2024-04-28 21:36:23.000000 pydolarvenezuela-1.5.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.782611 pydolarvenezuela-1.5.2/pyDolarVenezuela/
+-rw-rw-rw-   0        0        0     2712 2024-04-29 16:12:38.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.811276 pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/
+-rw-rw-rw-   0        0        0       20 2023-11-22 01:27:36.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.815278 pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/icons/
+-rw-rw-rw-   0        0        0      927 2023-11-22 01:28:58.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/icons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.831659 pydolarvenezuela-1.5.2/pyDolarVenezuela/data/
+-rw-rw-rw-   0        0        0        0 2024-04-25 17:18:32.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/data/__init__.py
+-rw-rw-rw-   0        0        0      684 2024-04-26 15:20:21.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/data/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.847609 pydolarvenezuela-1.5.2/pyDolarVenezuela/models/
+-rw-rw-rw-   0        0        0        0 2024-04-25 22:38:51.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/models/__init__.py
+-rw-rw-rw-   0        0        0      364 2024-04-26 04:56:19.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/models/database.py
+-rw-rw-rw-   0        0        0      312 2024-04-28 07:05:31.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/models/pages.py
+-rw-rw-rw-   0        0        0      453 2024-04-27 21:40:31.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/network.py
+-rw-rw-rw-   0        0        0      740 2024-04-28 16:11:30.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/pages.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.872898 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/
+-rw-rw-rw-   0        0        0     5145 2024-04-29 16:08:34.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-04-28 15:44:15.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/bcv.py
+-rw-rw-rw-   0        0        0     1762 2024-04-29 16:09:28.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/criptodolar.py
+-rw-rw-rw-   0        0        0     2315 2024-04-28 12:10:54.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/exchangemonitor.py
+-rw-rw-rw-   0        0        0     1282 2024-04-28 21:32:57.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/italcambio.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.884889 pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/
+-rw-rw-rw-   0        0        0      104 2024-04-02 19:26:40.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/__init__.py
+-rw-rw-rw-   0        0        0      670 2024-03-07 02:06:16.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/calculator.py
+-rw-rw-rw-   0        0        0     2187 2024-04-02 19:26:31.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/time.py
+-rw-rw-rw-   0        0        0     2236 2024-04-28 11:49:26.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-29 16:13:07.890658 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/
+-rw-rw-rw-   0        0        0     7221 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      897 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-29 16:13:07.000000 pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-04-29 16:12:24.000000 pydolarvenezuela-1.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 16:13:07.897657 pydolarvenezuela-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2024-04-29 16:12:30.000000 pydolarvenezuela-1.5.2/setup.py
```

### Comparing `pydolarvenezuela-1.5.1/LICENSE` & `pydolarvenezuela-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/PKG-INFO` & `pydolarvenezuela-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.1
+Version: 1.5.2
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
@@ -130,15 +130,15 @@
 
 print(valor_dolar)
 ```
 
 La función `currency_converter` convierte una cantidad de dinero de una moneda a otra utilizando los datos de un monitor específico.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 from pyDolarVenezuela import currency_converter
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 
 information_dolar = monitor.get_value_monitors("enparalelovzla")
 price_in_dolares = currency_converter(
```

### Comparing `pydolarvenezuela-1.5.1/README.md` & `pydolarvenezuela-1.5.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 print(valor_dolar)
 ```
 
 La función `currency_converter` convierte una cantidad de dinero de una moneda a otra utilizando los datos de un monitor específico.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 from pyDolarVenezuela import currency_converter
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 
 information_dolar = monitor.get_value_monitors("enparalelovzla")
 price_in_dolares = currency_converter(
```

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/__init__.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from . import network
 from .models.pages import Page
 from .data.redis import Redis
 from .tools import get_time_zone as getdate, currency_converter
 from .provider import select_monitor
 
-version = '1.5.1'
+version = '1.5.2'
 """
 Versión actual de la biblioteca    
 """
 
 class CheckVersion:
     """
     Verificar actualización de la biblioteca
```

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/assets/icons/__init__.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/assets/icons/__init__.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/data/redis.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/data/redis.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/pages.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/pages.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/__init__.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             change  = round(float(new_price - price), 2)
             percent = float(f'{round(float((change / new_price) * 100 if price != 0 else 0), 2)}'.replace('-', ' '))
             symbol  = "" if change == 0 else "▲" if change >= 0 else "▼"
             color   = "red" if symbol == '▼' else "green" if symbol == '▲' else "neutral"
             last_update = last_data[i].get('last_update', None)
             change = float(str(change).replace('-', ' '))
 
-            if not last_update:
+            if last_update:
                 existing_data_dict[i].update({
                     'price': new_price,
                     'change': change,
                     'percent': percent,
                     'color': color,
                     'symbol': symbol,
                     'last_update': last_update
```

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/bcv.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/bcv.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/criptodolar.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/criptodolar.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
         for monitor in self.json_response:
             if monitor['type'] in ['bolivar', 'bancove']:
                 data = {
                     'title': _convert_dollar_name_to_monitor_name(monitor['name']),
                     'price': round(monitor['price'], 2),
                     'price_old': monitor['priceOld'],
-                    'type': 'bank' if monitor['type'] == 'bancove' else 'monitor',
                     'last_update': time.get_time_standard(monitor['updatedAt']),
                 }
 
                 self.data[_convert_specific_format(data['title'])] = data
     
     def get_values(self):
         self._load()
```

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/exchangemonitor.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/exchangemonitor.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/provider/italcambio.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/provider/italcambio.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+from datetime import datetime
+from bs4 import BeautifulSoup
 from ..network import get
+from ..tools.time import standard_time_zone
 from ..utils import code_currencies
-from bs4 import BeautifulSoup
 
 class Italcambio:
     def __init__(self, url: str, **kwargs) -> None:
         response = get(url)
         self.soup = BeautifulSoup(response, 'html.parser')
 
     def _load(self):
@@ -13,17 +15,20 @@
 
         self.rates = {}
         for i in range(len(monitors_amounts)):
             if i%2 == 0:
                 title = code_currencies[monitors_amounts[i]]
                 price_old = float(str(monitors_amounts[i-1]).split()[-1])
                 price = round(price_old, 2)
+                dt = datetime.now(standard_time_zone)
+                dt_tostring = dt.strftime('%d/%m/%Y, %I:%M %p')
     
                 self.rates[monitors_amounts[i].lower()] = {
                     'title': title,
                     'price': price,
-                    'price_old': price_old
+                    'price_old': price_old,
+                    'last_update': dt_tostring
                 }
     
     def get_values(self):
         self._load()
         return self.rates
```

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/calculator.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/tools/time.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/tools/time.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela/utils.py` & `pydolarvenezuela-1.5.2/pyDolarVenezuela/utils.py`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/PKG-INFO` & `pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDolarVenezuela
-Version: 1.5.1
+Version: 1.5.2
 Summary: Esta librería en Python consulta los precios del dólar y/o euro en diversos monitores en Venezuela, además de la tasa de cambio oficial BCV.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Francisco Griman
@@ -130,15 +130,15 @@
 
 print(valor_dolar)
 ```
 
 La función `currency_converter` convierte una cantidad de dinero de una moneda a otra utilizando los datos de un monitor específico.
 
 ```python
-from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor
+from pyDolarVenezuela.pages import BCV, CriptoDolar, ExchangeMonitor, Italcambio
 from pyDolarVenezuela import Monitor
 from pyDolarVenezuela import currency_converter
 
 monitor = Monitor(ExchangeMonitor, 'USD')
 
 information_dolar = monitor.get_value_monitors("enparalelovzla")
 price_in_dolares = currency_converter(
```

### Comparing `pydolarvenezuela-1.5.1/pyDolarVenezuela.egg-info/SOURCES.txt` & `pydolarvenezuela-1.5.2/pyDolarVenezuela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydolarvenezuela-1.5.1/pyproject.toml` & `pydolarvenezuela-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyDolarVenezuela"
-version = "1.5.1"
+version = "1.5.2"
 dependencies = [
   "requests",
   "curl_cffi",
   "beautifulsoup4",
   "babel",
   "pytz",
   "colorama",
```

### Comparing `pydolarvenezuela-1.5.1/setup.py` & `pydolarvenezuela-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.5.1'
+VERSION = '1.5.2'
 PACKAGE_NAME = 'pyDolarVenezuela' 
 AUTHOR = 'Francisco Griman'
 AUTHOR_EMAIL = 'grihardware@gmail.com'
 URL = 'https://github.com/fcoagz/pydolarvenezuela'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'esta es una librería en python que te permite consultar los precios del dólar en diferentes monitores en Venezuela y el dolar oficial BCV.'
```

