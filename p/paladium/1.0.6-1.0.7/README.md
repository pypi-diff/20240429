# Comparing `tmp/paladium-1.0.6.tar.gz` & `tmp/paladium-1.0.7.tar.gz`

## Comparing `paladium-1.0.6.tar` & `paladium-1.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 paladium-1.0.6/example.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/__init__.py
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/faction.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/paladium.py
--rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/player.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 paladium-1.0.6/src/paladium/rank.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paladium-1.0.6/tests/.gitkeep
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 paladium-1.0.6/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 paladium-1.0.6/README.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 paladium-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 paladium-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 paladium-1.0.7/example.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 paladium-1.0.7/src/paladium/__init__.py
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 paladium-1.0.7/src/paladium/faction.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 paladium-1.0.7/src/paladium/paladium.py
+-rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 paladium-1.0.7/src/paladium/player.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 paladium-1.0.7/src/paladium/rank.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paladium-1.0.7/tests/.gitkeep
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 paladium-1.0.7/.gitignore
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 paladium-1.0.7/README.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 paladium-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 paladium-1.0.7/PKG-INFO
```

### Comparing `paladium-1.0.6/example.py` & `paladium-1.0.7/example.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from paladium import Paladium
-from rank import Leaderboard
 
 def test():
     # main tests
     api = Paladium()
 
     # example player
     player = api.get_player('aureliancnx')
```

### Comparing `paladium-1.0.6/src/paladium/faction.py` & `paladium-1.0.7/src/paladium/faction.py`

 * *Files identical despite different names*

### Comparing `paladium-1.0.6/src/paladium/paladium.py` & `paladium-1.0.7/src/paladium/paladium.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 from typing import List, Dict
 from .player import Player
 from .faction import Faction, FactionLeaderboard
 from .rank import PlayerRank, Leaderboard, PlayerLeaderboard
 import uuid
 
-PALADIUM_API_URL = 'https://api.paladium-pvp.fr/'
+PALADIUM_API_URL = 'https://api.paladium.games/v1/paladium/'
 
 class Paladium:
     def __init__(self, key: str = None):
         self.key = key
     
     """
     Represents the Paladium API.
```

### Comparing `paladium-1.0.6/src/paladium/player.py` & `paladium-1.0.7/src/paladium/player.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         self.uuid = uuid.UUID(json_data.get('uuid'))
         self.faction = json_data.get('faction')
         self.first_join = datetime.fromtimestamp(json_data.get('firstJoin') / 1000)
         self.friends = [Friend(friend) for friend in json_data.get('friends')]
         self.money = json_data.get('money')
         self.time_played = timedelta(minutes=json_data.get('timePlayed'))
         self.jobs = {job: PlayerJob.from_dict(job, json_data.get('jobs').get(job)) for job in json_data.get('jobs')}
+        self.rank = json_data.get('rank')
 
     def __str__(self):
         return f'Player: {self.username}, UUID: {self.uuid}, Faction: {self.faction}, Time Played: {self.time_played}'
 
     @staticmethod
     def from_uuid(id: str) -> 'Player':
         """
@@ -125,7 +126,13 @@
         return self.time_played
     
     def get_jobs(self) -> Dict[str, PlayerJob]:
         """
         Returns a dictionary of jobs of the player.
         """
         return self.jobs
+
+    def get_rank(self) -> str:
+        """
+        Returns the rank of the player.
+        """
+        return self.rank
```

### Comparing `paladium-1.0.6/src/paladium/rank.py` & `paladium-1.0.7/src/paladium/rank.py`

 * *Files identical despite different names*

