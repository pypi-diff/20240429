# Comparing `tmp/skodaconnect-1.3.8.tar.gz` & `tmp/skodaconnect-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skodaconnect-1.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skodaconnect-1.3.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skodaconnect-1.3.8.tar` & `skodaconnect-1.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      502 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/.github/dependabot.yml
--rw-r--r--   0        0        0      127 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/.gitignore
--rw-r--r--   0        0        0       34 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/.settings/.gitignore
--rw-r--r--   0        0        0    11357 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/LICENSE
--rw-r--r--   0        0        0     8218 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/README.md
--rw-r--r--   0        0        0    14972 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/example/example.py
--rw-r--r--   0        0        0      984 2023-11-05 21:25:20.468701 skodaconnect-1.3.8/pyproject.toml
--rw-r--r--   0        0        0       47 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/requirements.txt
--rw-r--r--   0        0        0      290 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/skodaconnect/__init__.py
--rw-r--r--   0        0        0      226 2023-11-05 21:21:33.749179 skodaconnect-1.3.8/skodaconnect/__version__.py
--rw-r--r--   0        0        0    99894 2023-11-05 21:21:33.753179 skodaconnect-1.3.8/skodaconnect/connection.py
--rw-r--r--   0        0        0    10026 2023-11-05 21:21:33.753179 skodaconnect-1.3.8/skodaconnect/const.py
--rw-r--r--   0        0        0    50241 2023-11-05 21:21:33.753179 skodaconnect-1.3.8/skodaconnect/dashboard.py
--rw-r--r--   0        0        0     3209 2023-11-05 21:21:33.753179 skodaconnect-1.3.8/skodaconnect/exceptions.py
--rw-r--r--   0        0        0     2565 2023-11-05 21:21:33.753179 skodaconnect-1.3.8/skodaconnect/utilities.py
--rw-r--r--   0        0        0   164132 2023-11-05 21:21:33.753179 skodaconnect-1.3.8/skodaconnect/vehicle.py
--rw-r--r--   0        0        0     9102 1970-01-01 00:00:00.000000 skodaconnect-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0      502 2023-10-25 18:53:50.980473 skodaconnect-1.3.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      127 2023-04-06 19:41:48.072390 skodaconnect-1.3.9/.gitignore
+-rw-r--r--   0        0        0       34 2023-04-06 19:41:31.182390 skodaconnect-1.3.9/.settings/.gitignore
+-rw-r--r--   0        0        0    11357 2023-04-06 19:41:31.182390 skodaconnect-1.3.9/LICENSE
+-rw-r--r--   0        0        0     8218 2023-10-25 18:53:50.980473 skodaconnect-1.3.9/README.md
+-rw-r--r--   0        0        0    14972 2023-12-11 15:26:57.086214 skodaconnect-1.3.9/example/example.py
+-rw-r--r--   0        0        0      984 2023-12-11 15:27:39.826214 skodaconnect-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-12-11 15:27:39.826214 skodaconnect-1.3.9/requirements.txt
+-rw-r--r--   0        0        0      290 2023-04-06 19:41:48.072390 skodaconnect-1.3.9/skodaconnect/__init__.py
+-rw-r--r--   0        0        0      226 2023-12-11 16:05:04.836214 skodaconnect-1.3.9/skodaconnect/__version__.py
+-rw-r--r--   0        0        0    99885 2023-12-11 15:27:39.836214 skodaconnect-1.3.9/skodaconnect/connection.py
+-rw-r--r--   0        0        0    10026 2023-12-11 15:45:15.746214 skodaconnect-1.3.9/skodaconnect/const.py
+-rw-r--r--   0        0        0    50241 2023-10-25 18:53:50.980473 skodaconnect-1.3.9/skodaconnect/dashboard.py
+-rw-r--r--   0        0        0     3209 2023-04-06 19:41:48.072390 skodaconnect-1.3.9/skodaconnect/exceptions.py
+-rw-r--r--   0        0        0     2565 2023-04-06 19:41:48.072390 skodaconnect-1.3.9/skodaconnect/utilities.py
+-rw-r--r--   0        0        0   164132 2023-12-11 16:05:04.836214 skodaconnect-1.3.9/skodaconnect/vehicle.py
+-rw-r--r--   0        0        0     9102 1970-01-01 00:00:00.000000 skodaconnect-1.3.9/PKG-INFO
```

### Comparing `skodaconnect-1.3.8/LICENSE` & `skodaconnect-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.8/README.md` & `skodaconnect-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.8/example/example.py` & `skodaconnect-1.3.9/example/example.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.8/pyproject.toml` & `skodaconnect-1.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.8/skodaconnect/connection.py` & `skodaconnect-1.3.9/skodaconnect/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -928,15 +928,15 @@
         try:
             await self.set_token('connect')
             _LOGGER.debug("Attempting extraction of jwt subject from identity token.")
             atoken = self._session_tokens['connect']['access_token']
             subject = self.decode_token(atoken).get('sub', None)
 
             response = await self.get(
-                f'https://customer-profile.apps.emea.vwapps.io/v2/customers/{subject}/realCarData'
+                f'https://customer-profile.vwgroup.io/v2/customers/{subject}/realCarData'
             )
             if response.get('realCars', False):
                 data = {
                     'realCars': response.get('realCars', {})
                 }
                 return data
             elif response.get('status_code', {}):
```

### Comparing `skodaconnect-1.3.8/skodaconnect/const.py` & `skodaconnect-1.3.9/skodaconnect/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 #XCLIENT_ID = 'a83d7e44-c8b7-42b7-b8ca-e478270d2091'                                    # Used in Android app 4.x.x
 XCLIENT_ID = 'fef89b3d-a6e0-4525-91eb-a9436e6e469a'                                     # Used in Android app 5.2.7
 XAPPVERSION = '5.2.7'
 XAPPNAME = 'cz.skodaauto.connect'
 # IOS App UA
 # USER_AGENT = 'MySkoda/230629002 CFNetwork/1474 Darwin/23.0.0'
 # Android App UA
-USER_AGENT = 'OneConnect/000000148 CFNetwork/1485 Darwin/23.1.0'
+USER_AGENT = 'OneConnect/000000157 CFNetwork/1485 Darwin/23.1.0'
 APP_URI = 'skodaconnect://oidc.login/'
 
 # Used when fetching data
 HEADERS_SESSION = {
     'Connection': 'keep-alive',
     'Content-Type': 'application/json',
     'Accept-charset': 'UTF-8',
```

### Comparing `skodaconnect-1.3.8/skodaconnect/dashboard.py` & `skodaconnect-1.3.9/skodaconnect/dashboard.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.8/skodaconnect/exceptions.py` & `skodaconnect-1.3.9/skodaconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.8/skodaconnect/utilities.py` & `skodaconnect-1.3.9/skodaconnect/utilities.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.8/skodaconnect/vehicle.py` & `skodaconnect-1.3.9/skodaconnect/vehicle.py`

 * *Files identical despite different names*

### Comparing `skodaconnect-1.3.8/PKG-INFO` & `skodaconnect-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skodaconnect
-Version: 1.3.8
+Version: 1.3.9
 Summary: skodaconnect - A Python 3 library for interacting with Skoda Connect and Smartlink services.
 Author-email: lendy007 <lendik@gmail.com>, FarFar <faekie@hotmail.com>, dvx76 <fabrice.devaux@gmail.com>, WebSpider <bacardicoke@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: POSIX
```

