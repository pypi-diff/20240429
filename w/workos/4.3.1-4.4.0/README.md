# Comparing `tmp/workos-4.3.1.tar.gz` & `tmp/workos-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workos-4.3.1.tar", last modified: Wed Apr 10 20:22:45 2024, max compression
+gzip compressed data, was "workos-4.4.0.tar", last modified: Mon Apr 29 17:14:22 2024, max compression
```

## Comparing `workos-4.3.1.tar` & `workos-4.4.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:22:45.086060 workos-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-10 20:22:31.000000 workos-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-10 20:22:45.086060 workos-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-10 20:22:31.000000 workos-4.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 20:22:45.086060 workos-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-10 20:22:31.000000 workos-4.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:22:45.082060 workos-4.3.1/workos/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-10 20:22:31.000000 workos-4.3.1/workos/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-10 20:22:31.000000 workos-4.3.1/workos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-10 20:22:31.000000 workos-4.3.1/workos/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-10 20:22:31.000000 workos-4.3.1/workos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-04-10 20:22:31.000000 workos-4.3.1/workos/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-10 20:22:31.000000 workos-4.3.1/workos/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-10 20:22:31.000000 workos-4.3.1/workos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7510 2024-04-10 20:22:31.000000 workos-4.3.1/workos/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-10 20:22:31.000000 workos-4.3.1/workos/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-10 20:22:31.000000 workos-4.3.1/workos/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-10 20:22:31.000000 workos-4.3.1/workos/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:22:45.082060 workos-4.3.1/workos/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/audit_logs_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-10 20:22:31.000000 workos-4.3.1/workos/resources/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-10 20:22:31.000000 workos-4.3.1/workos/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-04-10 20:22:31.000000 workos-4.3.1/workos/user_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:22:45.086060 workos-4.3.1/workos/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 20:22:31.000000 workos-4.3.1/workos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-10 20:22:31.000000 workos-4.3.1/workos/utils/connection_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-10 20:22:31.000000 workos-4.3.1/workos/utils/pagination_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-10 20:22:31.000000 workos-4.3.1/workos/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-10 20:22:31.000000 workos-4.3.1/workos/utils/sso_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-10 20:22:31.000000 workos-4.3.1/workos/utils/um_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 20:22:31.000000 workos-4.3.1/workos/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-10 20:22:31.000000 workos-4.3.1/workos/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 20:22:45.082060 workos-4.3.1/workos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-10 20:22:45.000000 workos-4.3.1/workos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-10 20:22:45.000000 workos-4.3.1/workos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:22:45.000000 workos-4.3.1/workos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 20:22:43.000000 workos-4.3.1/workos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-10 20:22:45.000000 workos-4.3.1/workos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 20:22:45.000000 workos-4.3.1/workos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.314670 workos-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 17:14:15.000000 workos-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-29 17:14:22.314670 workos-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-29 17:14:15.000000 workos-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:14:22.314670 workos-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-29 17:14:15.000000 workos-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.310670 workos-4.4.0/workos/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-29 17:14:15.000000 workos-4.4.0/workos/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-29 17:14:15.000000 workos-4.4.0/workos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-29 17:14:15.000000 workos-4.4.0/workos/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-29 17:14:15.000000 workos-4.4.0/workos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-04-29 17:14:15.000000 workos-4.4.0/workos/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-29 17:14:15.000000 workos-4.4.0/workos/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-29 17:14:15.000000 workos-4.4.0/workos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7713 2024-04-29 17:14:15.000000 workos-4.4.0/workos/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-29 17:14:15.000000 workos-4.4.0/workos/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-29 17:14:15.000000 workos-4.4.0/workos/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-29 17:14:15.000000 workos-4.4.0/workos/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.314670 workos-4.4.0/workos/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/audit_logs_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-29 17:14:15.000000 workos-4.4.0/workos/resources/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-29 17:14:15.000000 workos-4.4.0/workos/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39319 2024-04-29 17:14:15.000000 workos-4.4.0/workos/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.314670 workos-4.4.0/workos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/connection_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/pagination_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/sso_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/um_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-29 17:14:15.000000 workos-4.4.0/workos/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-29 17:14:15.000000 workos-4.4.0/workos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:14:22.310670 workos-4.4.0/workos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:14:20.000000 workos-4.4.0/workos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:14:22.000000 workos-4.4.0/workos.egg-info/top_level.txt
```

### Comparing `workos-4.3.1/LICENSE` & `workos-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/PKG-INFO` & `workos-4.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.3.1
+Version: 4.4.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,27 @@
 workos.client_id = "client_1234"
 ```
 
 ## SDK Versioning
 
 For our SDKs WorkOS follows a Semantic Versioning ([SemVer](https://semver.org/)) process where all releases will have a version X.Y.Z (like 1.0.0) pattern wherein Z would be a bug fix (e.g., 1.0.1), Y would be a minor release (1.1.0) and X would be a major release (2.0.0). We permit any breaking changes to only be released in major versions and strongly recommend reading changelogs before making any major version upgrades.
 
+## Beta Releases
+
+WorkOS has features in Beta that can be accessed via Beta releases. We would love for you to try these
+and share feedback with us before these features reach general availability (GA). To install a Beta version,
+please follow the [installation steps](#installation) above using the Beta release version.
+
+> Note: there can be breaking changes between Beta versions. Therefore, we recommend pinning the package version to a
+> specific version. This way you can install the same version each time without breaking changes unless you are
+> intentionally looking for the latest Beta version.
+
+We highly recommend keeping an eye on when the Beta feature you are interested in goes from Beta to stable so that you
+can move to using the stable version.
+
 ## More Information
 
 - [Single Sign-On Guide](https://workos.com/docs/sso/guide)
 - [Directory Sync Guide](https://workos.com/docs/directory-sync/guide)
 - [Admin Portal Guide](https://workos.com/docs/admin-portal/guide)
 - [Magic Link Guide](https://workos.com/docs/magic-link/guide)
```

### Comparing `workos-4.3.1/setup.py` & `workos-4.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/audit_logs.py` & `workos-4.4.0/workos/audit_logs.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/client.py` & `workos-4.4.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/directory_sync.py` & `workos-4.4.0/workos/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/events.py` & `workos-4.4.0/workos/events.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,22 +24,24 @@
             self._request_helper = RequestHelper()
         return self._request_helper
 
     def list_events(
         self,
         events=None,
         limit=None,
+        organization_id=None,
         after=None,
         range_start=None,
         range_end=None,
     ):
         """Gets a list of Events .
         Kwargs:
             events (list): Filter to only return events of particular types. (Optional)
             limit (int): Maximum number of records to return. (Optional)
+            organization_id(str): Organization ID limits scope of events to a single organization. (Optional)
             after (str): Pagination cursor to receive records after a provided Event ID. (Optional)
             range_start (str): Date range start for stream of events. (Optional)
             range_end (str): Date range end for stream of events. (Optional)
 
 
         Returns:
             dict: Events response from WorkOS.
@@ -49,14 +51,15 @@
             limit = RESPONSE_LIMIT
             default_limit = True
 
         params = {
             "events": events,
             "limit": limit,
             "after": after,
+            "organization_id": organization_id,
             "range_start": range_start,
             "range_end": range_end,
         }
 
         response = self.request_helper.request(
             "events",
             method=REQUEST_METHOD_GET,
```

### Comparing `workos-4.3.1/workos/exceptions.py` & `workos-4.4.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/mfa.py` & `workos-4.4.0/workos/mfa.py`

 * *Files 7% similar despite different names*

```diff
@@ -102,16 +102,17 @@
         Returns: Dict containing the authentication factor information.
         """
 
         if authentication_factor_id is None:
             raise ValueError("Incomplete arguments. Need to specify a factor ID")
 
         response = self.request_helper.request(
-            "auth/factors/{authentication_factor_id}".format(
-                authentication_factor_id=authentication_factor_id
+            self.request_helper.build_parameterized_url(
+                "auth/factors/{authentication_factor_id}",
+                authentication_factor_id=authentication_factor_id,
             ),
             method=REQUEST_METHOD_GET,
             token=workos.api_key,
         )
 
         if response["type"] == "totp":
             return WorkOSAuthenticationFactorTotp.construct_from_response(
@@ -133,16 +134,17 @@
         Returns: Does not provide a response.
         """
 
         if authentication_factor_id is None:
             raise ValueError("Incomplete arguments. Need to specify a factor ID.")
 
         return self.request_helper.request(
-            "auth/factors/{authentication_factor_id}".format(
-                authentication_factor_id=authentication_factor_id
+            self.request_helper.build_parameterized_url(
+                "auth/factors/{authentication_factor_id}",
+                authentication_factor_id=authentication_factor_id,
             ),
             method=REQUEST_METHOD_DELETE,
             token=workos.api_key,
         )
 
     def challenge_factor(
         self,
@@ -165,16 +167,16 @@
 
         if authentication_factor_id is None:
             raise ValueError(
                 "Incomplete arguments: 'authentication_factor_id' is a required parameter"
             )
 
         response = self.request_helper.request(
-            "auth/factors/{factor_id}/challenge".format(
-                factor_id=authentication_factor_id
+            self.request_helper.build_parameterized_url(
+                "auth/factors/{factor_id}/challenge", factor_id=authentication_factor_id
             ),
             method=REQUEST_METHOD_POST,
             params=params,
             token=workos.api_key,
         )
 
         return WorkOSChallenge.construct_from_response(response).to_dict()
@@ -224,16 +226,17 @@
 
         if authentication_challenge_id is None or code is None:
             raise ValueError(
                 "Incomplete arguments: 'authentication_challenge_id' and 'code' are required parameters"
             )
 
         response = self.request_helper.request(
-            "auth/challenges/{challenge_id}/verify".format(
-                challenge_id=authentication_challenge_id
+            self.request_helper.build_parameterized_url(
+                "auth/challenges/{challenge_id}/verify",
+                challenge_id=authentication_challenge_id,
             ),
             method=REQUEST_METHOD_POST,
             params=params,
             token=workos.api_key,
         )
 
         return WorkOSChallengeVerification.construct_from_response(response).to_dict()
```

### Comparing `workos-4.3.1/workos/organizations.py` & `workos-4.4.0/workos/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/passwordless.py` & `workos-4.4.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/portal.py` & `workos-4.4.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/audit_logs_export.py` & `workos-4.4.0/workos/resources/audit_logs_export.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/base.py` & `workos-4.4.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/directory_sync.py` & `workos-4.4.0/workos/resources/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/event.py` & `workos-4.4.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/list.py` & `workos-4.4.0/workos/resources/list.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/mfa.py` & `workos-4.4.0/workos/resources/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/organizations.py` & `workos-4.4.0/workos/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/passwordless.py` & `workos-4.4.0/workos/resources/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/sso.py` & `workos-4.4.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/resources/user_management.py` & `workos-4.4.0/workos/resources/user_management.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/sso.py` & `workos-4.4.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/user_management.py` & `workos-4.4.0/workos/user_management.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/utils/connection_types.py` & `workos-4.4.0/workos/utils/connection_types.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/utils/request.py` & `workos-4.4.0/workos/utils/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import platform
 
 import requests
+import urllib
 
 import workos
 from workos.exceptions import (
     AuthorizationException,
     AuthenticationException,
     BadRequestException,
     NotFoundException,
@@ -41,14 +42,18 @@
             base_api_url (str): Base URL for api requests (Should end with a /)
         """
         self.base_api_url = "{}{{}}".format(base_api_url)
 
     def generate_api_url(self, path):
         return self.base_api_url.format(path)
 
+    def build_parameterized_url(self, url, **params):
+        escaped_params = {k: urllib.parse.quote(str(v)) for k, v in params.items()}
+        return url.format(**escaped_params)
+
     def request(
         self,
         path,
         method=REQUEST_METHOD_GET,
         params=None,
         headers=None,
         token=None,
```

### Comparing `workos-4.3.1/workos/utils/validation.py` & `workos-4.4.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos/webhooks.py` & `workos-4.4.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-4.3.1/workos.egg-info/PKG-INFO` & `workos-4.4.0/workos.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.3.1
+Version: 4.4.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,27 @@
 workos.client_id = "client_1234"
 ```
 
 ## SDK Versioning
 
 For our SDKs WorkOS follows a Semantic Versioning ([SemVer](https://semver.org/)) process where all releases will have a version X.Y.Z (like 1.0.0) pattern wherein Z would be a bug fix (e.g., 1.0.1), Y would be a minor release (1.1.0) and X would be a major release (2.0.0). We permit any breaking changes to only be released in major versions and strongly recommend reading changelogs before making any major version upgrades.
 
+## Beta Releases
+
+WorkOS has features in Beta that can be accessed via Beta releases. We would love for you to try these
+and share feedback with us before these features reach general availability (GA). To install a Beta version,
+please follow the [installation steps](#installation) above using the Beta release version.
+
+> Note: there can be breaking changes between Beta versions. Therefore, we recommend pinning the package version to a
+> specific version. This way you can install the same version each time without breaking changes unless you are
+> intentionally looking for the latest Beta version.
+
+We highly recommend keeping an eye on when the Beta feature you are interested in goes from Beta to stable so that you
+can move to using the stable version.
+
 ## More Information
 
 - [Single Sign-On Guide](https://workos.com/docs/sso/guide)
 - [Directory Sync Guide](https://workos.com/docs/directory-sync/guide)
 - [Admin Portal Guide](https://workos.com/docs/admin-portal/guide)
 - [Magic Link Guide](https://workos.com/docs/magic-link/guide)
```

### Comparing `workos-4.3.1/workos.egg-info/SOURCES.txt` & `workos-4.4.0/workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

