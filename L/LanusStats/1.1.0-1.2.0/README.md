# Comparing `tmp/LanusStats-1.1.0.tar.gz` & `tmp/LanusStats-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LanusStats-1.1.0.tar", last modified: Sat Apr 13 23:21:00 2024, max compression
+gzip compressed data, was "LanusStats-1.2.0.tar", last modified: Mon Apr 29 03:45:13 2024, max compression
```

## Comparing `LanusStats-1.1.0.tar` & `LanusStats-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 23:21:00.414178 LanusStats-1.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-13 23:21:00.394147 LanusStats-1.1.0/LanusStats/
--rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.1.0/LanusStats/__init__.py
--rw-rw-rw-   0        0        0      234 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/config.py
--rw-rw-rw-   0        0        0     1759 2024-04-04 03:40:59.000000 LanusStats-1.1.0/LanusStats/exceptions.py
--rw-rw-rw-   0        0        0    14779 2024-04-07 03:01:27.000000 LanusStats-1.1.0/LanusStats/fbref.py
--rw-rw-rw-   0        0        0    11508 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/fotmob.py
--rw-rw-rw-   0        0        0    16566 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/functions.py
--rw-rw-rw-   0        0        0      303 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/sofascore.py
--rw-rw-rw-   0        0        0     6605 2024-04-13 23:20:47.000000 LanusStats-1.1.0/LanusStats/threesixfivescores.py
--rw-rw-rw-   0        0        0     8640 2024-04-07 03:10:29.000000 LanusStats-1.1.0/LanusStats/visualizations.py
-drwxrwxrwx   0        0        0        0 2024-04-13 23:21:00.409850 LanusStats-1.1.0/LanusStats.egg-info/
--rw-rw-rw-   0        0        0     4858 2024-04-13 23:20:59.000000 LanusStats-1.1.0/LanusStats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2024-04-13 23:21:00.000000 LanusStats-1.1.0/LanusStats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 23:20:59.000000 LanusStats-1.1.0/LanusStats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-04-13 23:20:59.000000 LanusStats-1.1.0/LanusStats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-13 23:20:59.000000 LanusStats-1.1.0/LanusStats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4858 2024-04-13 23:21:00.412848 LanusStats-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4476 2024-04-07 16:05:01.000000 LanusStats-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-13 23:21:00.415053 LanusStats-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-04-13 23:20:47.000000 LanusStats-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:45:13.707935 LanusStats-1.2.0/
+drwxrwxrwx   0        0        0        0 2024-04-29 03:45:13.684503 LanusStats-1.2.0/LanusStats/
+-rw-rw-rw-   0        0        0      222 2024-04-07 03:06:19.000000 LanusStats-1.2.0/LanusStats/__init__.py
+-rw-rw-rw-   0        0        0      234 2024-04-13 23:20:47.000000 LanusStats-1.2.0/LanusStats/config.py
+-rw-rw-rw-   0        0        0     1759 2024-04-04 03:40:59.000000 LanusStats-1.2.0/LanusStats/exceptions.py
+-rw-rw-rw-   0        0        0    14960 2024-04-29 02:16:12.000000 LanusStats-1.2.0/LanusStats/fbref.py
+-rw-rw-rw-   0        0        0    11508 2024-04-13 23:20:47.000000 LanusStats-1.2.0/LanusStats/fotmob.py
+-rw-rw-rw-   0        0        0    17922 2024-04-14 02:10:59.000000 LanusStats-1.2.0/LanusStats/functions.py
+-rw-rw-rw-   0        0        0     3984 2024-04-14 02:31:00.000000 LanusStats-1.2.0/LanusStats/sofascore.py
+-rw-rw-rw-   0        0        0     9140 2024-04-29 03:44:07.000000 LanusStats-1.2.0/LanusStats/threesixfivescores.py
+-rw-rw-rw-   0        0        0     8640 2024-04-07 03:10:29.000000 LanusStats-1.2.0/LanusStats/visualizations.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:45:13.702464 LanusStats-1.2.0/LanusStats.egg-info/
+-rw-rw-rw-   0        0        0     8177 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 03:45:13.000000 LanusStats-1.2.0/LanusStats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8177 2024-04-29 03:45:13.706219 LanusStats-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7795 2024-04-29 02:16:12.000000 LanusStats-1.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 03:45:13.708721 LanusStats-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-29 03:44:17.000000 LanusStats-1.2.0/setup.py
```

### Comparing `LanusStats-1.1.0/LanusStats/exceptions.py` & `LanusStats-1.2.0/LanusStats/exceptions.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.1.0/LanusStats/fbref.py` & `LanusStats-1.2.0/LanusStats/fbref.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,24 +126,26 @@
         return df, df_vs
     
     def concatenate_teams_df(self, df, df_vs, axis=1):
         df_total = pd.concat([df, df_vs], axis=axis)
 
         return df_total
         
-    def get_all_teams_season_stats(self, league, save_csv=False, stats_vs=False, change_columns_names=False, add_page_name=False):
+    def get_all_teams_season_stats(self, league, season, save_csv=False, stats_vs=False, change_columns_names=False, add_page_name=False):
         
         today = datetime.now().strftime('%Y-%m-%d')
         data = pd.DataFrame()
         for stat in self.possible_stats:
-            placeholder = self.get_teams_season_stats(f'{stat}',league, False, stats_vs, change_columns_names, add_page_name)
+            placeholder = self.get_teams_season_stats(f'{stat}',league, season, False, stats_vs, change_columns_names, add_page_name)
             data = pd.concat([data, placeholder], axis=1)
         
-        if save_csv:
-              data.to_csv(f'{league} - {stat} - {today}.csv')
+        if save_csv and stats_vs:
+            data.to_csv(f'{league} - {stat} - team vs stats - {today}.csv')
+        elif save_csv: 
+            data.to_csv(f'{league} - {stat} - team stats - {today}.csv')
 
         return data
 
     def get_table(self, soup):
         return soup.find_all('table')[0]
 
     def parse_row(self, row):
@@ -227,15 +229,15 @@
                 df_data.columns = new_columns
 
         if save_csv:
               df_data.to_csv(f'{league} - {stat} - {today}.csv')
         
         return df_data
 
-    def get_all_player_season_stats(self, league, save_csv=False):
+    def get_all_player_season_stats(self, league, season, save_csv=False):
         """Gets a table of ALL the stats in a players page.
 
         Args:
             league (str): Possible leagues in get_available_leagues("Fbref")
             save_csv (bool, optional): If true, it saves the tables as a csv. Defaults to False.
 
         Returns:
@@ -245,28 +247,28 @@
         
         today = datetime.now().strftime('%Y-%m-%d')
         data = pd.DataFrame()
         gk_data = pd.DataFrame()
         for stat in self.possible_stats:
             print(stat)
             if stat in ['keepers', 'keepersadv']:
-                placeholder = self.get_player_season_stats(f'{stat}',league, False, True)
+                placeholder = self.get_player_season_stats(f'{stat}',league, season, False, True)
                 if len(gk_data) == 0:
                     gk_data = pd.concat([gk_data, placeholder], axis=1)
                 else:
                     gk_data = gk_data.merge(placeholder, on='Player', how='left')
             else:
-                placeholder = self.get_player_season_stats(f'{stat}',league, False, True)
+                placeholder = self.get_player_season_stats(f'{stat}',league, season, False, True)
                 if len(data) == 0:
                     data = pd.concat([data, placeholder], axis=1)
                 else:
                     data = data.merge(placeholder, on='Player', how='left')
         
         if save_csv:
-              data.to_csv(f'{league} - {stat} - {today}.csv')
+              data.to_csv(f'{league} - {stat} - player stats - {today}.csv')
 
         #To avoid duplicates of players that played for two clubs in the same competition
         data = data.drop_duplicates(subset=['Player', 'stats_Squad']).reset_index(drop=True)
         gk_data = gk_data.drop_duplicates(subset=['Player', 'keepers_Squad']).reset_index(drop=True)
 
         return data, gk_data
```

### Comparing `LanusStats-1.1.0/LanusStats/fotmob.py` & `LanusStats-1.2.0/LanusStats/fotmob.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.1.0/LanusStats/functions.py` & `LanusStats-1.2.0/LanusStats/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 from .exceptions import *
+from IPython.display import clear_output
+import pandas as pd
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+import random
+import numpy as np
+import undetected_chromedriver as uc
 
 def get_possible_leagues(league, season, page):
     """Dictionary with all the possible pages, leagues and season for the scraper.
     Also contains some exception to prevent errors such as a league or page that is not a part of the scraper.
 
     Args:
         league (str): League to scrape
@@ -478,8 +485,44 @@
         page (str): Page inside the array of get_available_pagues()
         league (str): League inside the array of get_available_leagues(page)
 
     Returns:
         dict: League data with the seasons inside
     """
     league_data = get_possible_leagues('Argentina Copa de la Liga', '2023', 'Fotmob')[page][league]
-    return league_data
+    return league_data
+
+def get_proxy():
+    ''' Gets a proxy address.
+
+    Code used by Owen Seymour in ScraperFC, here:
+    https://github.com/oseymour/ScraperFC/blob/main/ScraperFC/shared_functions.py#L628 
+    
+    Returns
+    -------
+    proxy : str
+        In the form <IP address>:<port>
+    '''
+    options = Options()
+    options.add_argument('--headless')
+    driver = uc.Chrome(headless=True,use_subprocess=False,option=options)
+    clear_output()
+    
+    try:
+        driver.get('https://sslproxies.org/')
+        table = driver.find_elements(By.TAG_NAME, 'table')[0]
+        df = pd.read_html(table.get_attribute('outerHTML'))[0]
+        df = df.iloc[np.where(~np.isnan(df['Port']))[0],:] # ignore nans
+
+        ips = df['IP Address'].values
+        ports = df['Port'].astype('int').values
+
+        driver.quit()
+        proxies = list()
+        for i in range(len(ips)):
+            proxies.append('{}:{}'.format(ips[i], ports[i]))
+        i = random.randint(0, len(proxies)-1)
+        return proxies[i]
+    except Exception as e:
+        driver.close()
+        driver.quit()
+        raise e
```

### Comparing `LanusStats-1.1.0/LanusStats/threesixfivescores.py` & `LanusStats-1.2.0/LanusStats/threesixfivescores.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from PIL import Image
 import re
 from io import BytesIO
 from .functions import get_possible_leagues_for_page
 from .exceptions import MatchDoesntHaveInfo
 from .config import headers
 import time
+import numpy as np
 
 class ThreeSixFiveScores:
 
     def parse_dataframe(self, objeto):
         df = pd.DataFrame(objeto['rows'])
         df_1 = df['entity'].apply(pd.Series)
         df_2 = df['stats'].apply(pd.Series)[0].apply(pd.Series)
@@ -71,14 +72,72 @@
         
         matchup_id, game_id = self.get_ids(match_url)
         response = requests.get(f'https://webws.365scores.com/web/game/?appTypeId=5&langId=29&timezoneName=America/Buenos_Aires&userCountryId=382&gameId={game_id}&matchupId={matchup_id}&topBookmaker=14', headers=headers)
         time.sleep(3)
         match_data = response.json()['game']
         return match_data
     
+    def get_requests_stats(self, match_url):
+        """Request to stats of a match
+
+        Args:
+            match_url (str): 65Scores match URL.
+
+        Returns:
+            response: JSON with the response of the request.
+        """
+        matchup_id, game_id = self.get_ids(match_url)
+        response = requests.get(f'https://webws.365scores.com/web/game/stats/?appTypeId=5&langId=29&timezoneName=America/Buenos_Aires&userCountryId=382&games={game_id}', headers=headers)
+        time.sleep(3)
+        return response
+    
+    def get_match_general_stats(self, match_url):
+        """Get data from a match and scrape it. Requests about general stats.
+
+        Args:
+            match_url (url): 365Scores match URL. Example: https://www.365scores.com/es-mx/football/match/copa-de-la-liga-profesional-7214/lanus-union-santa-fe-869-7206-7214#id=4033824
+
+        Returns:
+            match_stats: Json with game stats.
+        """
+        
+        response = self.get_requests_stats(match_url)
+        match_stats = pd.DataFrame(response.json()['statistics'])
+        
+        team1 = {
+            'id': response.json()['competitors'][0]['id'],
+            'name': response.json()['competitors'][0]['name']
+        }
+        
+        team2 = {
+            'id': response.json()['competitors'][1]['id'],
+            'name': response.json()['competitors'][1]['name']
+        }
+        
+        match_stats['team_name'] = np.where(match_stats['competitorId'] == team1['id'], team1['name'], team2['name'])
+        return match_stats
+    
+    def get_match_time_stats(self, match_url):
+        """Get time match stats
+
+        Args:
+            match_url (str): 365Scores match URL. Example: https://www.365scores.com/es-mx/football/match/copa-de-la-liga-profesional-7214/lanus-union-santa-fe-869-7206-7214#id=4033824
+
+        Returns:
+            game_statistics: JSON with various stats about time played and wasted in a match.
+        """
+        
+        response = self.get_requests_stats(match_url)
+        try:
+            game_statistics = response.json()['actualGameStatistics']
+        except KeyError:
+            raise MatchDoesntHaveInfo(match_url)
+        
+        return game_statistics
+    
     def get_match_shotmap(self, match_url):
         """Scrape shotmap from the page as a DataFrame, if the match has it.
 
         Args:
             match_url (url): 365Scores match URL. Example: https://www.365scores.com/es-mx/football/match/copa-de-la-liga-profesional-7214/lanus-union-santa-fe-869-7206-7214#id=4033824
 
         Returns:
@@ -102,22 +161,34 @@
             teams_df: Player data for a match as a DataFrame.
         """
         match_data = self.get_match_data(match_url)
         teams_json = match_data['members']
         teams_df = pd.DataFrame(teams_json)
         return teams_df
     
-    def get_team_names(self, match_url):
+    def get_team_data(self, match_url):
         values = ['home', 'away']
         names = []
+        ids = []
         match_data = self.get_match_data(match_url)
         for value in values:
             nombre = match_data[f'{value}Competitor']['name']
-            names.append(nombre)
-        home, away = names[0], names[1]
+            id = match_data[f'{value}Competitor']['id']
+            names.append(nombre), ids.append(id)
+        
+        home = {
+            'name': names[0],
+            'id': id[0]
+        }
+        
+        away = {
+            'name': names[1],
+            'id': id[1]
+        }
+        
         return home, away
     
     def get_general_match_stats(self, match_url):
         """Get general statistics for teams from a match
 
         Args:
             match_url (url): 365Scores match URL. Example: https://www.365scores.com/es-mx/football/match/copa-de-la-liga-profesional-7214/lanus-union-santa-fe-869-7206-7214#id=4033824
```

### Comparing `LanusStats-1.1.0/LanusStats/visualizations.py` & `LanusStats-1.2.0/LanusStats/visualizations.py`

 * *Files identical despite different names*

### Comparing `LanusStats-1.1.0/setup.py` & `LanusStats-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '1.1.0'
+VERSION = '1.2.0'
 PACKAGE_NAME = 'LanusStats'
 AUTHOR = 'Federico Rábanos'
 AUTHOR_EMAIL = 'lanusstats@gmail.com'
 URL = 'https://github.com/federicorabanos'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Python library for scraping football data and visualize it / Libreria de Python para scrapear data de fútbol y visualizarla'
```

