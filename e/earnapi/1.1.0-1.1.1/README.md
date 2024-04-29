# Comparing `tmp/earnapi-1.1.0.tar.gz` & `tmp/earnapi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earnapi-1.1.0.tar", last modified: Sun Apr 28 18:01:33 2024, max compression
+gzip compressed data, was "earnapi-1.1.1.tar", last modified: Sun Apr 28 19:51:30 2024, max compression
```

## Comparing `earnapi-1.1.0.tar` & `earnapi-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:01:33.157587 earnapi-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 18:01:26.000000 earnapi-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-28 18:01:33.157587 earnapi-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-28 18:01:26.000000 earnapi-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:01:33.157587 earnapi-1.1.0/earnapi/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-28 18:01:26.000000 earnapi-1.1.0/earnapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-28 18:01:26.000000 earnapi-1.1.0/earnapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-28 18:01:26.000000 earnapi-1.1.0/earnapi/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-28 18:01:26.000000 earnapi-1.1.0/earnapi/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:01:33.157587 earnapi-1.1.0/earnapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 18:01:33.000000 earnapi-1.1.0/earnapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-28 18:01:26.000000 earnapi-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 18:01:33.157587 earnapi-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-28 18:01:26.000000 earnapi-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:51:30.790880 earnapi-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 19:51:22.000000 earnapi-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-28 19:51:30.790880 earnapi-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-28 19:51:22.000000 earnapi-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:51:30.790880 earnapi-1.1.1/earnapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-28 19:51:22.000000 earnapi-1.1.1/earnapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-28 19:51:22.000000 earnapi-1.1.1/earnapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-28 19:51:22.000000 earnapi-1.1.1/earnapi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-28 19:51:22.000000 earnapi-1.1.1/earnapi/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 19:51:30.790880 earnapi-1.1.1/earnapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-28 19:51:30.000000 earnapi-1.1.1/earnapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-28 19:51:30.000000 earnapi-1.1.1/earnapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 19:51:30.000000 earnapi-1.1.1/earnapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 19:51:30.000000 earnapi-1.1.1/earnapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-28 19:51:30.000000 earnapi-1.1.1/earnapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-28 19:51:22.000000 earnapi-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 19:51:30.790880 earnapi-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-28 19:51:22.000000 earnapi-1.1.1/setup.py
```

### Comparing `earnapi-1.1.0/LICENSE` & `earnapi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `earnapi-1.1.0/PKG-INFO` & `earnapi-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earnapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous EarnApp API wrapper written in Python using asyncio.
 Home-page: https://github.com/Vinchethescript/earnapi
 Author: Vinche.zsh
 Author-email: 
 License: GPL-3.0
 Keywords: python,earnapi,python earnapp api,python earnapp api wrapper,earnapp api wrapper,earnapp,passive income,earnapp api,earnapp dashboard,requests,python earnapp
 Requires-Python: >=3.7
```

### Comparing `earnapi-1.1.0/README.md` & `earnapi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `earnapi-1.1.0/earnapi/client.py` & `earnapi-1.1.1/earnapi/client.py`

 * *Files identical despite different names*

### Comparing `earnapi-1.1.0/earnapi/errors.py` & `earnapi-1.1.1/earnapi/errors.py`

 * *Files identical despite different names*

### Comparing `earnapi-1.1.0/earnapi/models.py` & `earnapi-1.1.1/earnapi/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from urllib.parse import urljoin
 from datetime import datetime
 from dataclasses import dataclass
+from typing import Optional
 
 
 class Endpoint:  # there are still a lot to be implemented
     BASE_URL = "https://earnapp.com/dashboard/api/"
 
     # users
     USER = urljoin(BASE_URL, "user")
@@ -45,33 +46,38 @@
     XSRF = urljoin(BASE_URL, "sec/rotate_xsrf")
     IP_CHECK = urljoin(BASE_URL, "check_ip/")
     LOGOUT = urljoin(BASE_URL, "logout")
 
 
 class Model:
     def __init__(self, kwargs) -> None:
-        self.___kwargs = kwargs
+        self._kwargs = kwargs
         for k, v in kwargs.items():
             if callable(getattr(self, f"_transform_{k}", None)):
-                kwargs[k] = getattr(self, f"_transform_{k}")(v)
+                self._kwargs[k] = getattr(self, f"_transform_{k}")(v)
+
 
     def __dir__(self):
         ret = dir(super())
-        ret += self.___kwargs.keys()
+        ret += self._kwargs.keys()
         return ret
 
-    def __getattr__(self, item):
-        return self.___kwargs.get(item, None)
+    def __getattribute__(self, item):
+        get = super().__getattribute__
+        if item.startswith("_"):
+            return get(item)
+        
+        return self._kwargs.get(item, None)
 
     def __getitem__(self, item):
-        return self.___kwargs.get(item)
+        return self._kwargs.get(item)
 
     def __repr__(self):
         args = []
-        for key, value in self.___kwargs.items():
+        for key, value in self._kwargs.items():
             args.append(f"{key}={value!r}")
         return f"{self.__class__.__name__} <{' '.join(args)}>"
 
     @classmethod
     def create_list(cls, items: list) -> list:
         return [cls(item) for item in items]
 
@@ -106,18 +112,19 @@
     promo_bonuses: float
     promo_bonuses_total: float
     ref_bvpn: float
     ref_bvpn_total: float
     ref_hola_browser: float
     ref_hola_browser_total: float
     referral_part: int
-    redeem_details: RedeemDetails
+    redeem_details: Optional[RedeemDetails] = None
 
-    def _transform_redeem_details(self, value: dict):
-        return RedeemDetails(value)
+    def _transform_redeem_details(self, value: Optional[dict]):
+        if value:
+            return RedeemDetails(value)
 
     def _transform_referral_part(self, value: str):
         return float(value.rstrip("%")) / 100
 
     @property
     def referral_bonus(self):
         return self.ref_bonuses
```

### Comparing `earnapi-1.1.0/earnapi.egg-info/PKG-INFO` & `earnapi-1.1.1/earnapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earnapi
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asynchronous EarnApp API wrapper written in Python using asyncio.
 Home-page: https://github.com/Vinchethescript/earnapi
 Author: Vinche.zsh
 Author-email: 
 License: GPL-3.0
 Keywords: python,earnapi,python earnapp api,python earnapp api wrapper,earnapp api wrapper,earnapp,passive income,earnapp api,earnapp dashboard,requests,python earnapp
 Requires-Python: >=3.7
```

### Comparing `earnapi-1.1.0/setup.py` & `earnapi-1.1.1/setup.py`

 * *Files identical despite different names*

