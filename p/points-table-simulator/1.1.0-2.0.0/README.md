# Comparing `tmp/points_table_simulator-1.1.0.tar.gz` & `tmp/points_table_simulator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "points_table_simulator-1.1.0.tar", last modified: Thu Apr 25 07:00:26 2024, max compression
+gzip compressed data, was "points_table_simulator-2.0.0.tar", last modified: Mon Apr 29 15:43:51 2024, max compression
```

## Comparing `points_table_simulator-1.1.0.tar` & `points_table_simulator-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.696224 points_table_simulator-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.github/scripts/quality_checks.sh
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.github/scripts/setup_environment.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.github/workflows/quality_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/create_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.696224 points_table_simulator-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/src/points_table_simulator/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/src/points_table_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/src/points_table_simulator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/src/points_table_simulator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25624 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/src/points_table_simulator/points_table_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 07:00:26.000000 points_table_simulator-1.1.0/src/points_table_simulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.700224 points_table_simulator-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/tests/points_table_simulator_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/points_table_simulator_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 07:00:26.704224 points_table_simulator-1.1.0/tests/points_table_simulator_tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/points_table_simulator_tests/error_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-25 07:00:18.000000 points_table_simulator-1.1.0/tests/points_table_simulator_tests/success_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.075955 points_table_simulator-2.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.github/scripts/quality_checks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.github/scripts/setup_environment.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.github/workflows/quality_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/create_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.075955 points_table_simulator-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/src/points_table_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/src/points_table_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/src/points_table_simulator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/src/points_table_simulator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27066 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/src/points_table_simulator/points_table_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/tests/points_table_simulator_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/points_table_simulator_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/tests/points_table_simulator_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/points_table_simulator_tests/error_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/points_table_simulator_tests/success_tests.py
```

### Comparing `points_table_simulator-1.1.0/.github/workflows/publish.yml` & `points_table_simulator-2.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/.github/workflows/quality_check.yml` & `points_table_simulator-2.0.0/.github/workflows/quality_check.yml`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/.gitignore` & `points_table_simulator-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/LICENSE` & `points_table_simulator-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/PKG-INFO` & `points_table_simulator-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: points-table-simulator
-Version: 1.1.0
+Version: 2.0.0
 Summary: This package will simulate the points table based on different possible results in a sports tournament
 Home-page: https://github.com/NishanthMuruganantham/points-table-simulator
 Author: Nishanth Muruganantham
 Author-email: nishanthmurugananth10@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `points_table_simulator-1.1.0/README.md` & `points_table_simulator-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/pyproject.toml` & `points_table_simulator-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/setup.cfg` & `points_table_simulator-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/src/points_table_simulator/exceptions.py` & `points_table_simulator-2.0.0/src/points_table_simulator/exceptions.py`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/src/points_table_simulator/points_table_simulator.py` & `points_table_simulator-2.0.0/src/points_table_simulator/points_table_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,14 +252,28 @@
         current_points_table = pd.DataFrame(team_points_data)
         current_points_table.sort_values(by="points", ascending=False, inplace=True)
         current_points_table.reset_index(drop=True, inplace=True)
 
         return current_points_table
 
     @property
+    def number_of_completed_matches(self) -> int:
+        """
+        Returns the number of completed matches in the tournament schedule.
+
+        Returns:
+            int: The number of completed matches in the tournament schedule.
+        """
+        return len(self.tournament_schedule) - len(self.remaining_matches)
+
+    @property
+    def remaining_schedule_df(self) -> pd.DataFrame:
+        return self.tournament_schedule.iloc[self.number_of_completed_matches:, :]
+
+    @property
     def remaining_matches(self) -> List[Tuple[str, str]]:
         """
         Returns a list of tuples containing the remaining fixture matches in the tournament schedule.
 
         Returns:
             List[Tuple[str, str]]: List of tuples containing the remaining matches in the tournament schedule.
         """
@@ -317,18 +331,19 @@
 
         self._validate_the_inputs_for_simulate_qualification_scenarios(
             team_name, top_x_position_in_the_table, desired_number_of_scenarios
         )
         self._check_for_minimal_tournament_completion()
         list_of_points_tables_for_qualification_scenarios = []
         list_of_remaining_match_result_for_qualification_scenarios = []
+        current_points_dict: Dict[str, int] = self.current_points_table.set_index("team")["points"].to_dict()   # pylint: disable=unsubscriptable-object
 
-        for tuple_of_remaining_match_results in self.various_probable_outcomes_for_remaining_matches:
+        for remaining_matches_winning_teams in self.various_probable_outcomes_for_remaining_matches:
             _is_favourable_scenario = self._check_the_given_scenario_for_favourable_outcome(
-                team_name, top_x_position_in_the_table, tuple_of_remaining_match_results
+                current_points_dict.copy(), remaining_matches_winning_teams, team_name, top_x_position_in_the_table
             )
             if _is_favourable_scenario:
                 updated_points_table, temporary_schedule_df = _is_favourable_scenario
                 list_of_points_tables_for_qualification_scenarios.append(updated_points_table)
                 list_of_remaining_match_result_for_qualification_scenarios.append(temporary_schedule_df)
 
             if len(list_of_points_tables_for_qualification_scenarios) >= desired_number_of_scenarios:
@@ -349,65 +364,77 @@
         tournament_completion_percentage = (
             (len(self.tournament_schedule) - len(self.remaining_matches)) / len(self.tournament_schedule)
         ) * 100
         if tournament_completion_percentage < TOURNAMENT_COMPLETION_CUTOFF_PERCENTAGE:
             raise TournamentCompletionBelowCutoffError(TOURNAMENT_COMPLETION_CUTOFF_PERCENTAGE, round(tournament_completion_percentage, 2))
 
     def _check_the_given_scenario_for_favourable_outcome(
-        self, team_name: str, top_x_position_in_the_table:int, tuple_of_remaining_match_results: Tuple[str]
+        self, current_points_dict: Dict[str, int], remaining_matches_winning_teams: Tuple[str], team_name: str, top_x_position_in_the_table:int
     ) -> Union[Tuple[pd.DataFrame, pd.DataFrame], None]:
         """
         Checks if the given scenario is favourable for the specified team.
 
         This function iterates through all possible combinations of match results for the remaining matches
         in the tournament schedule. For each combination, it calculates the updated points table and checks
         if the specified team qualifies within the top X positions. Once enough qualifying scenarios are found
         based on the desired number of scenarios, the function stops iterating and returns the results.
 
         Returns:
             Union[Tuple[pd.DataFrame, pd.DataFrame], None]: A tuple containing two dataframes:
                 - The updated points table for the given scenario.
                 - The remaining match outcome for the given scenario.
         """
-        number_of_completed_matches: int = len(self.tournament_schedule) - len(self.remaining_matches)
-        remaining_schedule_df: pd.DataFrame = self.tournament_schedule.iloc[
-            number_of_completed_matches:, :
-        ]
-        initial_points_table = self.current_points_table
+        updated_points_dict = self._update_winning_team_points_dict(current_points_dict, remaining_matches_winning_teams)
+        top_x_positions_teams = list(updated_points_dict.keys())[:top_x_position_in_the_table]
 
-        temporary_schedule_df = remaining_schedule_df.copy()
-        updated_points_table = initial_points_table.copy()
+        if team_name in top_x_positions_teams:
+            remaining_outcome_df = self.remaining_schedule_df.copy()
+            udpated_points_table = self.current_points_table.copy()
+
+            for match_number, possible_winning_team in enumerate(remaining_matches_winning_teams):
+                home_team, away_team = self.remaining_matches[match_number]
+                remaining_outcome_df.loc[
+                    self.number_of_completed_matches + match_number,
+                    self.tournament_schedule_winning_team_column_name
+                ] = possible_winning_team
+                udpated_points_table = self._update_points_table(
+                    udpated_points_table, home_team, away_team, possible_winning_team
+                )
+            udpated_points_table.sort_values(by="points", ascending=False, inplace=True)
+            udpated_points_table.reset_index(drop=True, inplace=True)
 
-        for match_number, possible_winning_team in enumerate(tuple_of_remaining_match_results):
-            home_team, away_team = self.remaining_matches[match_number]
-            temporary_schedule_df.loc[
-                number_of_completed_matches + match_number,
-                self.tournament_schedule_winning_team_column_name
-            ] = possible_winning_team
-            updated_points_table = self._update_points_table(
-                updated_points_table, home_team, away_team, possible_winning_team
-            )
-
-        updated_points_table.sort_values(by="points", ascending=False, inplace=True)
-        updated_points_table.reset_index(drop=True, inplace=True)
-
-        if team_name in updated_points_table["team"].values[:top_x_position_in_the_table]:
-            return updated_points_table, temporary_schedule_df
+            return udpated_points_table, remaining_outcome_df
 
         return None
 
     def _update_points_table(
         self, points_table: pd.DataFrame, home_team: str, away_team: str, winning_team: str
     ) -> pd.DataFrame:
         points_table.loc[points_table["team"] == winning_team, "matches_won"] += 1
         points_table.loc[points_table['team'] == winning_team, 'points'] += self.points_for_a_win
         points_table.loc[points_table['team'] == home_team, 'matches_played'] += 1
         points_table.loc[points_table['team'] == away_team, 'matches_played'] += 1
         return points_table
 
+    def _update_winning_team_points_dict(self, current_points_dict: Dict[str, int], remaining_matches_winning_teams: Tuple[str]) -> Dict[str, int]:
+        """
+        Updates the points dictionary for the winning teams in the remaining matches.
+
+        Args:
+            current_points_dict (Dict[str, int]): The current points dictionary.
+            remaining_matches_winning_teams (Tuple[str]): The winning teams in the remaining matches.
+
+        Returns:
+            Dict[str, int]: The updated points dictionary.
+        """
+        for team in remaining_matches_winning_teams:
+            current_points_dict[team] += self.points_for_a_win
+        updated_points_dict = dict(sorted(current_points_dict.items(), key=lambda item: item[1], reverse=True))
+        return updated_points_dict
+
     @staticmethod
     def _validate_input_types(
         tournament_schedule: pd.DataFrame,
         points_for_a_win: int,
         points_for_a_no_result: int,
         points_for_a_draw: int,
         **kwargs
```

### Comparing `points_table_simulator-1.1.0/src/points_table_simulator.egg-info/PKG-INFO` & `points_table_simulator-2.0.0/src/points_table_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: points-table-simulator
-Version: 1.1.0
+Version: 2.0.0
 Summary: This package will simulate the points table based on different possible results in a sports tournament
 Home-page: https://github.com/NishanthMuruganantham/points-table-simulator
 Author: Nishanth Muruganantham
 Author-email: nishanthmurugananth10@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `points_table_simulator-1.1.0/src/points_table_simulator.egg-info/SOURCES.txt` & `points_table_simulator-2.0.0/src/points_table_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv` & `points_table_simulator-2.0.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/tests/points_table_simulator_tests/error_tests.py` & `points_table_simulator-2.0.0/tests/points_table_simulator_tests/error_tests.py`

 * *Files identical despite different names*

### Comparing `points_table_simulator-1.1.0/tests/points_table_simulator_tests/success_tests.py` & `points_table_simulator-2.0.0/tests/points_table_simulator_tests/success_tests.py`

 * *Files identical despite different names*

