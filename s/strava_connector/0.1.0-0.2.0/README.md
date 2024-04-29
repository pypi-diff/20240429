# Comparing `tmp/strava_connector-0.1.0.tar.gz` & `tmp/strava_connector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strava_connector-0.1.0.tar", max compression
+gzip compressed data, was "strava_connector-0.2.0.tar", max compression
```

## Comparing `strava_connector-0.1.0.tar` & `strava_connector-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2024-04-29 09:03:24.918761 strava_connector-0.1.0/LICENSE
--rw-r--r--   0        0        0     1108 2024-04-29 17:22:13.004695 strava_connector-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1438 2024-04-29 17:01:42.375758 strava_connector-0.1.0/strava_connector/__init__.py
--rw-r--r--   0        0        0     3600 2024-04-29 10:33:43.309077 strava_connector-0.1.0/strava_connector/authenticator.py
--rw-r--r--   0        0        0    13433 2024-04-29 17:19:47.401419 strava_connector-0.1.0/strava_connector/connector.py
--rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 strava_connector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-29 09:03:24.918761 strava_connector-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1108 2024-04-29 18:10:20.657421 strava_connector-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1438 2024-04-29 17:01:42.375758 strava_connector-0.2.0/strava_connector/__init__.py
+-rw-r--r--   0        0        0     3600 2024-04-29 10:33:43.309077 strava_connector-0.2.0/strava_connector/authenticator.py
+-rw-r--r--   0        0        0    15144 2024-04-29 18:06:29.122919 strava_connector-0.2.0/strava_connector/connector.py
+-rw-r--r--   0        0        0      407 1970-01-01 00:00:00.000000 strava_connector-0.2.0/PKG-INFO
```

### Comparing `strava_connector-0.1.0/LICENSE` & `strava_connector-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strava_connector-0.1.0/pyproject.toml` & `strava_connector-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strava_connector"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 requests = "^2.31.0"
```

### Comparing `strava_connector-0.1.0/strava_connector/__init__.py` & `strava_connector-0.2.0/strava_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `strava_connector-0.1.0/strava_connector/authenticator.py` & `strava_connector-0.2.0/strava_connector/authenticator.py`

 * *Files identical despite different names*

### Comparing `strava_connector-0.1.0/strava_connector/connector.py` & `strava_connector-0.2.0/strava_connector/connector.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Literal, overload
+
 import requests
 
 from strava_connector.authenticator import Authenticator
 
 
 class Connector:
     def __init__(
@@ -18,30 +20,52 @@
 
     @property
     def access_token(self) -> str:
         """Append the credentials to the request."""
         self.authenticator.update_token()
         return str(self.authenticator.strava_tokens["access_token"])
 
+    @overload
     def get_request(
         self,
         route: str,
         print_query: bool,
         params: dict,
-    ) -> dict:
+        to_json: Literal[True],
+    ) -> dict: ...
+
+    @overload
+    def get_request(
+        self,
+        route: str,
+        print_query: bool,
+        params: dict,
+        to_json: Literal[False],
+    ) -> requests.Response: ...
+
+    def get_request(
+        self,
+        route: str,
+        print_query: bool,
+        params: dict,
+        to_json: bool,
+    ) -> dict | requests.Response:
         """GET request against strava's API."""
         params["access_token"] = self.access_token
         params_str = "&".join(
             [f"{k}={v}" for k, v in params.items() if v is not None]
         )
         url = f"{self.api_url}/{route}?{params_str}"
         if print_query:
             print(url)
         result = requests.get(url, timeout=self.authenticator._timeout)
-        return result.json()
+        if to_json:
+            return result.json()
+        else:
+            return result
 
     def getActivityById(
         self,
         id: int,
         include_all_efforts: bool | None = None,
         print_query: bool = False,
     ) -> dict:
@@ -51,14 +75,15 @@
         """
         return self.get_request(
             route=f"activities/{id}",
             print_query=print_query,
             params={
                 "include_all_efforts": include_all_efforts,
             },
+            to_json=True,
         )
 
     def getCommentsByActivityId(
         self,
         id: int,
         page: int | None = None,
         per_page: int | None = None,
@@ -75,14 +100,15 @@
             print_query=print_query,
             params={
                 "page": page,
                 "per_page": per_page,
                 "page_size": page_size,
                 "after_cursor": after_cursor,
             },
+            to_json=True,
         )
 
     def getKudoersByActivityId(
         self,
         id: int,
         page: int | None = None,
         per_page: int | None = None,
@@ -95,14 +121,15 @@
         return self.get_request(
             route=f"activities/{id}/kudos",
             print_query=print_query,
             params={
                 "page": page,
                 "per_page": per_page,
             },
+            to_json=True,
         )
 
     def getLapsByActivityId(
         self,
         id: int,
         print_query: bool = False,
     ) -> dict:
@@ -110,14 +137,15 @@
 
         https://developers.strava.com/docs/reference/#api-Activities-getLapsByActivityId
         """
         return self.get_request(
             route=f"activities/{id}/laps",
             print_query=print_query,
             params={},
+            to_json=True,
         )
 
     def getLoggedInAthleteActivities(
         self,
         page: int,
         per_page: int | None = None,
         print_query: bool = False,
@@ -129,14 +157,15 @@
         return self.get_request(
             route="athlete/activities",
             print_query=print_query,
             params={
                 "page": page,
                 "per_page": per_page,
             },
+            to_json=True,
         )
 
     def getZonesByActivityId(
         self,
         id: int,
         print_query: bool = False,
     ) -> dict:
@@ -144,42 +173,42 @@
 
         https://developers.strava.com/docs/reference/#api-Activities-getZonesByActivityId
         """
         return self.get_request(
             route=f"activities/{id}/zones",
             print_query=print_query,
             params={},
+            to_json=True,
         )
 
     def getLoggedInAthlete(
         self,
         print_query: bool = False,
     ) -> dict:
         """Get Athlete.
 
         https://developers.strava.com/docs/reference/#api-Athletes-getLoggedInAthlete
         """
         return self.get_request(
-            route="athlete",
-            print_query=print_query,
-            params={},
+            route="athlete", print_query=print_query, params={}, to_json=True
         )
 
     def getLoggedInAthleteZones(
         self,
         print_query: bool = False,
     ) -> dict:
         """Get Zones.
 
         https://developers.strava.com/docs/reference/#api-Athletes-getLoggedInAthleteZones
         """
         return self.get_request(
             route="athlete/zones",
             print_query=print_query,
             params={},
+            to_json=True,
         )
 
     def getStats(
         self,
         id: int,
         print_query: bool = False,
     ) -> dict:
@@ -187,14 +216,15 @@
 
         https://developers.strava.com/docs/reference/#api-Athletes-getStats
         """
         return self.get_request(
             route=f"athletes/{id}/stats",
             print_query=print_query,
             params={},
+            to_json=True,
         )
 
     def getClubActivitiesById(
         self,
         id: int,
         page: int | None = None,
         per_page: int | None = None,
@@ -207,14 +237,15 @@
         return self.get_request(
             route=f"clubs/{id}/activities",
             print_query=print_query,
             params={
                 "page": page,
                 "per_page": per_page,
             },
+            to_json=True,
         )
 
     def getClubAdminsById(
         self,
         id: int,
         page: int | None = None,
         per_page: int | None = None,
@@ -227,14 +258,15 @@
         return self.get_request(
             route=f"clubs/{id}/admins",
             print_query=print_query,
             params={
                 "page": page,
                 "per_page": per_page,
             },
+            to_json=True,
         )
 
     def getClubById(
         self,
         id: int,
         print_query: bool = False,
     ) -> dict:
@@ -242,14 +274,15 @@
 
         https://developers.strava.com/docs/reference/#api-Clubs-getClubById
         """
         return self.get_request(
             route=f"clubs/{id}",
             print_query=print_query,
             params={},
+            to_json=True,
         )
 
     def getClubMembersById(
         self,
         id: int,
         page: int | None = None,
         per_page: int | None = None,
@@ -262,14 +295,15 @@
         return self.get_request(
             route=f"clubs/{id}/members",
             print_query=print_query,
             params={
                 "page": page,
                 "per_page": per_page,
             },
+            to_json=True,
         )
 
     def getLoggedInAthleteClubs(
         self,
         page: int,
         per_page: int | None = None,
         print_query: bool = False,
@@ -281,59 +315,60 @@
         return self.get_request(
             route="athlete/clubs",
             print_query=print_query,
             params={
                 "page": page,
                 "per_page": per_page,
             },
+            to_json=True,
         )
 
     def getGearById(
         self,
         id: str,
         print_query: bool = False,
     ) -> dict:
         """Get Gear.
 
         https://developers.strava.com/docs/reference/#api-Gears-getGearById
         """
         return self.get_request(
-            route=f"gear/{id}",
-            print_query=print_query,
-            params={},
+            route=f"gear/{id}", print_query=print_query, params={}, to_json=True
         )
 
     def getRouteAsGPX(
         self,
         id: int,
         print_query: bool = False,
-    ) -> dict:
+    ) -> requests.Response:
         """Export Route GPX.
 
         https://developers.strava.com/docs/reference/#api-Routes-getRouteAsGPX
         """
         return self.get_request(
             route=f"routes/{id}/export_gpx",
             print_query=print_query,
             params={},
+            to_json=False,
         )
 
     def getRouteAsTCX(
         self,
         id: int,
         print_query: bool = False,
-    ) -> dict:
+    ) -> requests.Response:
         """Export Route TCX.
 
         https://developers.strava.com/docs/reference/#api-Routes-getRouteAsTCX
         """
         return self.get_request(
             route=f"routes/{id}/export_tcx",
             print_query=print_query,
             params={},
+            to_json=False,
         )
 
     def getRouteById(
         self,
         id: int,
         print_query: bool = False,
     ) -> dict:
@@ -341,14 +376,15 @@
 
         https://developers.strava.com/docs/reference/#api-Routes-getRouteById
         """
         return self.get_request(
             route=f"routes/{id}",
             print_query=print_query,
             params={},
+            to_json=True,
         )
 
     def getRoutesByAthleteId(
         self,
         id: int,
         page: int | None = None,
         per_page: int | None = None,
@@ -361,14 +397,15 @@
         return self.get_request(
             route=f"athletes/{id}/routes",
             print_query=print_query,
             params={
                 "page": page,
                 "per_page": per_page,
             },
+            to_json=True,
         )
 
     def getEffortsBySegmentId(
         self,
         segment_id: int,
         start_date_local: str | None = None,
         end_date_local: str | None = None,
@@ -384,14 +421,15 @@
             print_query=print_query,
             params={
                 "segment_id": segment_id,
                 "start_date_local": start_date_local,
                 "end_date_local": end_date_local,
                 "per_page": per_page,
             },
+            to_json=True,
         )
 
     def getSegmentEffortById(
         self,
         id: int,
         print_query: bool = False,
     ) -> dict:
@@ -399,14 +437,15 @@
 
         https://developers.strava.com/docs/reference/#api-SegmentEfforts-getSegmentEffortById
         """
         return self.get_request(
             route=f"segment_efforts/{id}",
             print_query=print_query,
             params={},
+            to_json=True,
         )
 
     def exploreSegments(
         self,
         bounds: str,
         activity_type: str | None = None,
         min_cat: int | None = None,
@@ -422,14 +461,35 @@
             print_query=print_query,
             params={
                 "bounds": bounds,
                 "activity_type": activity_type,
                 "min_cat": min_cat,
                 "max_cat": max_cat,
             },
+            to_json=True,
+        )
+
+    def getLoggedInAthleteStarredSegments(
+        self,
+        page: int | None = None,
+        per_page: int | None = None,
+        print_query: bool = False,
+    ) -> dict:
+        """List Athlete Starred Segments.
+
+        https://developers.strava.com/docs/reference/#api-Segments-getLoggedInAthleteStarredSegments
+        """
+        return self.get_request(
+            route="segments/starred",
+            print_query=print_query,
+            params={
+                "page": page,
+                "per_page": per_page,
+            },
+            to_json=True,
         )
 
     def getRouteStreams(
         self,
         id: int,
         print_query: bool = False,
     ) -> dict:
@@ -437,14 +497,15 @@
 
         https://developers.strava.com/docs/reference/#api-Streams-getRouteStreams
         """
         return self.get_request(
             route=f"routes/{id}/streams",
             print_query=print_query,
             params={},
+            to_json=True,
         )
 
     def getSegmentEffortStreams(
         self,
         id: int,
         keys: list[str],
         key_by_type: bool = False,
@@ -457,14 +518,15 @@
         return self.get_request(
             route=f"segment_efforts/{id}/streams",
             print_query=print_query,
             params={
                 "keys": keys,
                 "key_by_type": key_by_type,
             },
+            to_json=True,
         )
 
     def getSegmentStreams(
         self,
         id: int,
         keys: list[str],
         key_by_type: bool = False,
@@ -477,14 +539,15 @@
         return self.get_request(
             route=f"segments/{id}/streams",
             print_query=print_query,
             params={
                 "keys": keys,
                 "key_by_type": key_by_type,
             },
+            to_json=True,
         )
 
     def getUploadById(
         self,
         uploadId: int,
         print_query: bool = False,
     ) -> dict:
@@ -492,8 +555,9 @@
 
         https://developers.strava.com/docs/reference/#api-Uploads-getUploadById
         """
         return self.get_request(
             route=f"uploads/{id}",
             print_query=print_query,
             params={"uploadId": uploadId},
+            to_json=True,
         )
```

