# Comparing `tmp/MLB-StatsAPI-1.7.1.tar.gz` & `tmp/mlb_statsapi-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLB-StatsAPI-1.7.1.tar", last modified: Mon Dec 18 20:05:53 2023, max compression
+gzip compressed data, was "mlb_statsapi-1.7.2.tar", last modified: Mon Apr 29 12:56:37 2024, max compression
```

## Comparing `MLB-StatsAPI-1.7.1.tar` & `mlb_statsapi-1.7.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 20:05:53.350515 MLB-StatsAPI-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-18 20:05:35.000000 MLB-StatsAPI-1.7.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 20:05:53.350515 MLB-StatsAPI-1.7.1/MLB_StatsAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-12-18 20:05:53.000000 MLB-StatsAPI-1.7.1/MLB_StatsAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2023-12-18 20:05:53.000000 MLB-StatsAPI-1.7.1/MLB_StatsAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 20:05:53.000000 MLB-StatsAPI-1.7.1/MLB_StatsAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-18 20:05:53.000000 MLB-StatsAPI-1.7.1/MLB_StatsAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-18 20:05:53.000000 MLB-StatsAPI-1.7.1/MLB_StatsAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-12-18 20:05:53.350515 MLB-StatsAPI-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-12-18 20:05:35.000000 MLB-StatsAPI-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-18 20:05:53.350515 MLB-StatsAPI-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-18 20:05:35.000000 MLB-StatsAPI-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 20:05:53.350515 MLB-StatsAPI-1.7.1/statsapi/
--rw-r--r--   0 runner    (1001) docker     (127)    60910 2023-12-18 20:05:35.000000 MLB-StatsAPI-1.7.1/statsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41519 2023-12-18 20:05:35.000000 MLB-StatsAPI-1.7.1/statsapi/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-18 20:05:35.000000 MLB-StatsAPI-1.7.1/statsapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 20:05:53.350515 MLB-StatsAPI-1.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 20:05:35.000000 MLB-StatsAPI-1.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2023-12-18 20:05:35.000000 MLB-StatsAPI-1.7.1/tests/test_get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:56:37.855325 mlb_statsapi-1.7.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 12:56:21.000000 mlb_statsapi-1.7.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:56:37.855325 mlb_statsapi-1.7.2/MLB_StatsAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-29 12:56:37.000000 mlb_statsapi-1.7.2/MLB_StatsAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-29 12:56:37.000000 mlb_statsapi-1.7.2/MLB_StatsAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:56:37.000000 mlb_statsapi-1.7.2/MLB_StatsAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 12:56:37.000000 mlb_statsapi-1.7.2/MLB_StatsAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 12:56:37.000000 mlb_statsapi-1.7.2/MLB_StatsAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-29 12:56:37.855325 mlb_statsapi-1.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-29 12:56:21.000000 mlb_statsapi-1.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:56:37.855325 mlb_statsapi-1.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-29 12:56:21.000000 mlb_statsapi-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:56:37.851325 mlb_statsapi-1.7.2/statsapi/
+-rw-r--r--   0 runner    (1001) docker     (127)    61193 2024-04-29 12:56:21.000000 mlb_statsapi-1.7.2/statsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41519 2024-04-29 12:56:21.000000 mlb_statsapi-1.7.2/statsapi/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 12:56:21.000000 mlb_statsapi-1.7.2/statsapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:56:37.855325 mlb_statsapi-1.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:56:21.000000 mlb_statsapi-1.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-29 12:56:21.000000 mlb_statsapi-1.7.2/tests/test_get.py
```

### Comparing `MLB-StatsAPI-1.7.1/LICENSE` & `mlb_statsapi-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MLB-StatsAPI-1.7.1/MLB_StatsAPI.egg-info/PKG-INFO` & `mlb_statsapi-1.7.2/MLB_StatsAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLB-StatsAPI
-Version: 1.7.1
+Version: 1.7.2
 Summary: MLB Stats API Wrapper for Python
 Home-page: https://github.com/toddrob99/MLB-StatsAPI
 Author: Todd Roberts
 Author-email: todd@toddrob.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `MLB-StatsAPI-1.7.1/PKG-INFO` & `mlb_statsapi-1.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLB-StatsAPI
-Version: 1.7.1
+Version: 1.7.2
 Summary: MLB Stats API Wrapper for Python
 Home-page: https://github.com/toddrob99/MLB-StatsAPI
 Author: Todd Roberts
 Author-email: todd@toddrob.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `MLB-StatsAPI-1.7.1/setup.py` & `mlb_statsapi-1.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `MLB-StatsAPI-1.7.1/statsapi/__init__.py` & `mlb_statsapi-1.7.2/statsapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,24 +148,28 @@
                     game_info["national_broadcasts"].append("MLB.tv Free Game")
                 if game_info["status"] in ["Final", "Game Over"]:
                     if game.get("isTie"):
                         game_info.update({"winning_team": "Tie", "losing_Team": "Tie"})
                     else:
                         game_info.update(
                             {
-                                "winning_team": game["teams"]["away"]["team"].get(
-                                    "name", "???"
-                                )
-                                if game["teams"]["away"].get("isWinner")
-                                else game["teams"]["home"]["team"].get("name", "???"),
-                                "losing_team": game["teams"]["home"]["team"].get(
-                                    "name", "???"
-                                )
-                                if game["teams"]["away"].get("isWinner")
-                                else game["teams"]["away"]["team"].get("name", "???"),
+                                "winning_team": (
+                                    game["teams"]["away"]["team"].get("name", "???")
+                                    if game["teams"]["away"].get("isWinner")
+                                    else game["teams"]["home"]["team"].get(
+                                        "name", "???"
+                                    )
+                                ),
+                                "losing_team": (
+                                    game["teams"]["home"]["team"].get("name", "???")
+                                    if game["teams"]["away"].get("isWinner")
+                                    else game["teams"]["away"]["team"].get(
+                                        "name", "???"
+                                    )
+                                ),
                                 "winning_pitcher": game.get("decisions", {})
                                 .get("winner", {})
                                 .get("fullName", ""),
                                 "losing_pitcher": game.get("decisions", {})
                                 .get("loser", {})
                                 .get("fullName", ""),
                                 "save_pitcher": game.get("decisions", {})
@@ -612,18 +616,22 @@
                         "ops"
                     ]
                 ),
                 "personId": batterId_int,
                 "battingOrder": str(
                     boxData[side]["players"]["ID" + batterId]["battingOrder"]
                 ),
-                "substitution": False
-                if str(boxData[side]["players"]["ID" + batterId]["battingOrder"])[-1]
-                == "0"
-                else True,
+                "substitution": (
+                    False
+                    if str(boxData[side]["players"]["ID" + batterId]["battingOrder"])[
+                        -1
+                    ]
+                    == "0"
+                    else True
+                ),
                 "note": boxData[side]["players"]["ID" + batterId]["stats"][
                     "batting"
                 ].get("note", ""),
                 "name": boxData["playerInfo"]["ID" + batterId]["boxscoreName"],
                 "position": boxData[side]["players"]["ID" + batterId]["position"][
                     "abbreviation"
                 ],
@@ -1215,15 +1223,15 @@
     )
 
 
 def lookup_player(lookup_value, gameType=None, season=None, sportId=1):
     """Get data about players based on first, last, or full name."""
     params = {
         "sportId": sportId,
-        "fields": "people,id,fullName,firstName,lastName,primaryNumber,currentTeam,id,primaryPosition,code,abbreviation,useName,boxscoreName,nickName,mlbDebutDate,nameFirstLast,firstLastName,lastFirstName,lastInitName,initLastName,fullFMLName,fullLFMName",
+        "fields": "people,id,fullName,firstName,lastName,primaryNumber,currentTeam,id,primaryPosition,code,abbreviation,useName,boxscoreName,nickName,mlbDebutDate,nameFirstLast,firstLastName,lastFirstName,lastInitName,initLastName,fullFMLName,fullLFMName,nameSlug",
     }
     if gameType:
         params.update(
             {
                 "gameType": gameType,
             }
         )
```

### Comparing `MLB-StatsAPI-1.7.1/statsapi/endpoints.py` & `mlb_statsapi-1.7.2/statsapi/endpoints.py`

 * *Files identical despite different names*

### Comparing `MLB-StatsAPI-1.7.1/tests/test_get.py` & `mlb_statsapi-1.7.2/tests/test_get.py`

 * *Files identical despite different names*

