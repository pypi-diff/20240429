# Comparing `tmp/corkus.py-3.0.1.tar.gz` & `tmp/corkus_py-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corkus.py-3.0.1.tar", last modified: Fri Dec  2 12:19:26 2022, max compression
+gzip compressed data, was "corkus_py-3.1.0.tar", last modified: Mon Apr 29 17:33:27 2024, max compression
```

## Comparing `corkus.py-3.0.1.tar` & `corkus_py-3.1.0.tar`

### file list

```diff
@@ -1,101 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:19:26.052920 corkus.py-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2022-12-02 12:19:05.000000 corkus.py-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-02 12:19:05.000000 corkus.py-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2022-12-02 12:19:26.052920 corkus.py-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2022-12-02 12:19:05.000000 corkus.py-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:19:26.024919 corkus.py-3.0.1/corkus/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:19:26.028920 corkus.py-3.0.1/corkus/data/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/data/ids_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/data/major_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:19:26.032920 corkus.py-3.0.1/corkus/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/ingredient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/leaderboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/endpoints/territory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:19:26.048920 corkus.py-3.0.1/corkus/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/armour_defense.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/base_guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/base_partial_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/base_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/base_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/dungeon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/guild_banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/identification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/identification_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/ingredient.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/ingredient_comsumable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/ingredient_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/ingredient_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/ingredient_sprite.py
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/leaderboard_guild.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/leaderboard_partial_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/leaderboard_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/level_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/major_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/mojang_skin_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/online_players.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_guild.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_ingredient.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_online_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/partial_teritories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/player.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/player_character.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/player_gamemodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/player_profession.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/player_ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/player_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/player_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/playtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/quest.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/raid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/search_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/skill_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/territory.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/territory_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/objects/weapon_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:19:26.052920 corkus.py-3.0.1/corkus/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/utils/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/utils/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-02 12:19:05.000000 corkus.py-3.0.1/corkus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-02 12:19:26.028920 corkus.py-3.0.1/corkus.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2022-12-02 12:19:25.000000 corkus.py-3.0.1/corkus.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2022-12-02 12:19:25.000000 corkus.py-3.0.1/corkus.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-02 12:19:25.000000 corkus.py-3.0.1/corkus.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2022-12-02 12:19:25.000000 corkus.py-3.0.1/corkus.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-02 12:19:25.000000 corkus.py-3.0.1/corkus.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-02 12:19:05.000000 corkus.py-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-02 12:19:26.052920 corkus.py-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2022-12-02 12:19:05.000000 corkus.py-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:27.086398 corkus_py-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 17:33:13.000000 corkus_py-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-29 17:33:13.000000 corkus_py-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-29 17:33:27.086398 corkus_py-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-29 17:33:13.000000 corkus_py-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:27.070399 corkus_py-3.1.0/corkus/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:27.074399 corkus_py-3.1.0/corkus/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/data/ids_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/data/major_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:27.074399 corkus_py-3.1.0/corkus/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/endpoints/territory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:27.082399 corkus_py-3.1.0/corkus/objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/armour_defense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/base_guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/base_partial_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/base_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/base_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/dungeon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/guild_banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/identification_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/identification_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/ingredient_comsumable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/ingredient_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/ingredient_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/ingredient_sprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13812 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/leaderboard_guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/leaderboard_partial_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/leaderboard_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/level_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/major_identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/mojang_skin_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/online_players.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_online_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/partial_teritories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/player.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/player_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/player_gamemodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/player_profession.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/player_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/player_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/player_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/playtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/quest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/raid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/search_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/skill_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/territory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/territory_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/objects/weapon_damage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:27.086398 corkus_py-3.1.0/corkus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/utils/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/utils/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 17:33:13.000000 corkus_py-3.1.0/corkus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:27.086398 corkus_py-3.1.0/corkus.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-29 17:33:27.000000 corkus_py-3.1.0/corkus.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-29 17:33:27.000000 corkus_py-3.1.0/corkus.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:33:27.000000 corkus_py-3.1.0/corkus.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:33:27.000000 corkus_py-3.1.0/corkus.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 17:33:27.000000 corkus_py-3.1.0/corkus.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 17:33:13.000000 corkus_py-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:33:27.086398 corkus_py-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-29 17:33:13.000000 corkus_py-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:33:27.086398 corkus_py-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_corkus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6326 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_leaderboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_player.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_playtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_territory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 17:33:13.000000 corkus_py-3.1.0/tests/test_uuid.py
```

### Comparing `corkus.py-3.0.1/LICENSE` & `corkus_py-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/PKG-INFO` & `corkus_py-3.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,28 @@
-Metadata-Version: 2.1
-Name: corkus.py
-Version: 3.0.1
-Summary: Asynchronous, feature-rich and easy to use Python wrapper for Public Wynncraft API
-Home-page: https://github.com/MrBartusek/corkus.py
-Author: MrBartusek
-License: MIT
-Project-URL: Documentation, https://corkuspy.readthedocs.io/en/stable/
-Project-URL: Issue tracker, https://github.com/MrBartusek/corkus.py/issues
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![corkus banner](https://i.imgur.com/8FjYte1.gif)
 
 [![pypi](https://img.shields.io/pypi/v/corkus.py)](https://pypi.org/project/corkus.py/)
-[![build](https://img.shields.io/github/workflow/status/MrBartusek/corkus.py/build)](https://github.com/MrBartusek/corkus.py/actions)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/MrBartusek/corkus.py/main.yml)](https://github.com/MrBartusek/corkus.py/actions)
 [![docs build](https://img.shields.io/readthedocs/corkuspy)](https://corkuspy.readthedocs.io/en/stable)
 [![Codecov](https://img.shields.io/codecov/c/github/MrBartusek/corkus.py)](https://app.codecov.io/gh/MrBartusek/corkus.py)
 [![python version](https://img.shields.io/pypi/pyversions/corkus.py)](https://pypi.org/project/corkus.py/)
 ![downloads](https://img.shields.io/pypi/dm/corkus.py?color=sucess)
 
 # Corkus.py ⚙️
 
+> [!CAUTION]
+> **Corkus.py is no longer maintained**
+>
+> Due to recent changes in the Wynncraft API, Corkus.py is no longer working and will not receive further updates or support. Some endpoints based on the v2 API may still be operational, but those relying on the now-removed v1 API and new v3 API are no longer functioning. Additionally, more features may become broken in the future.
+>
+> I'm unable to recommend any other Python-based wrapper for the Wynncraft API - I don't see any good alternatives. It is strongly advised to not use this project anymore due to its outdated and non-functional state.
+>
+> Thank you to all users and contributors for your support and feedback throughout the lifespan of this project.
+
+
 Asynchronous, feature-rich and easy to use Python wrapper for [Public Wynncraft API](https://docs.wynncraft.com).
 
 ## Key Features
 
 - Modern asynchronous API using `async`/`await` syntax.
 - Easy to use with an object oriented design using `fetch` and helper functions.
 - 100% coverage of the Wynncraft API.
```

### Comparing `corkus.py-3.0.1/corkus/client.py` & `corkus_py-3.1.0/corkus/client.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/data/ids_convert.py` & `corkus_py-3.1.0/corkus/data/ids_convert.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/data/major_ids.py` & `corkus_py-3.1.0/corkus/data/major_ids.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/guild.py` & `corkus_py-3.1.0/corkus/endpoints/guild.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/ingredient.py` & `corkus_py-3.1.0/corkus/endpoints/ingredient.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/item.py` & `corkus_py-3.1.0/corkus/endpoints/item.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/leaderboard.py` & `corkus_py-3.1.0/corkus/endpoints/leaderboard.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/network.py` & `corkus_py-3.1.0/corkus/endpoints/network.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/player.py` & `corkus_py-3.1.0/corkus/endpoints/player.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/recipe.py` & `corkus_py-3.1.0/corkus/endpoints/recipe.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/search.py` & `corkus_py-3.1.0/corkus/endpoints/search.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/endpoints/territory.py` & `corkus_py-3.1.0/corkus/endpoints/territory.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/errors.py` & `corkus_py-3.1.0/corkus/errors.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/__init__.py` & `corkus_py-3.1.0/corkus/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/armour_defense.py` & `corkus_py-3.1.0/corkus/objects/armour_defense.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/base_guild.py` & `corkus_py-3.1.0/corkus/objects/base_guild.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/base_partial_member.py` & `corkus_py-3.1.0/corkus/objects/base_partial_member.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/base_player.py` & `corkus_py-3.1.0/corkus/objects/base_player.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/base_server.py` & `corkus_py-3.1.0/corkus/objects/base_server.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/color.py` & `corkus_py-3.1.0/corkus/objects/color.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/dungeon.py` & `corkus_py-3.1.0/corkus/objects/dungeon.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/enums.py` & `corkus_py-3.1.0/corkus/objects/enums.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/guild.py` & `corkus_py-3.1.0/corkus/objects/guild.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/guild_banner.py` & `corkus_py-3.1.0/corkus/objects/guild_banner.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/identification.py` & `corkus_py-3.1.0/corkus/objects/identification.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/identification_type.py` & `corkus_py-3.1.0/corkus/objects/identification_type.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/identification_values.py` & `corkus_py-3.1.0/corkus/objects/identification_values.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/ingredient.py` & `corkus_py-3.1.0/corkus/objects/ingredient.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/ingredient_comsumable.py` & `corkus_py-3.1.0/corkus/objects/ingredient_comsumable.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/ingredient_item.py` & `corkus_py-3.1.0/corkus/objects/ingredient_item.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/ingredient_position.py` & `corkus_py-3.1.0/corkus/objects/ingredient_position.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/ingredient_sprite.py` & `corkus_py-3.1.0/corkus/objects/ingredient_sprite.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/item.py` & `corkus_py-3.1.0/corkus/objects/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,17 +296,17 @@
             return None
 
     @property
     def item_id(self) -> str:
         """Minecraft `block`_/`item`_ ID + optional `data value`_,
         pre-flattening. Format: ``ID:DV``
 
-        .. _block: https://minecraft.fandom.com/wiki/Java_Edition_data_values/Pre-flattening/Block_IDs
-        .. _item: https://minecraft.fandom.com/wiki/Java_Edition_data_values/Pre-flattening/Item_IDs
-        .. _data value: https://minecraft.fandom.com/wiki/Java_Edition_data_values/Pre-flattening"""
+        .. _block: https://minecraft.wiki/w/Java_Edition_data_values/Pre-flattening/Block_IDs
+        .. _item: https://minecraft.wiki/w/Java_Edition_data_values/Pre-flattening/Item_IDs
+        .. _data value: https://minecraft.wiki/w/Java_Edition_data_values/Pre-flattening"""
         if self.skin is not None:
             return "397:3"
 
         return self._attributes.get("material") or self._generate_id()
 
     def _generate_id(self) -> str:
         if self.armour_type == ArmourType.LEATHER:
```

### Comparing `corkus.py-3.0.1/corkus/objects/leaderboard_guild.py` & `corkus_py-3.1.0/corkus/objects/leaderboard_guild.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/leaderboard_partial_member.py` & `corkus_py-3.1.0/corkus/objects/leaderboard_partial_member.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/leaderboard_player.py` & `corkus_py-3.1.0/corkus/objects/leaderboard_player.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/level_range.py` & `corkus_py-3.1.0/corkus/objects/level_range.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/major_identification.py` & `corkus_py-3.1.0/corkus/objects/major_identification.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/material.py` & `corkus_py-3.1.0/corkus/objects/material.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/member.py` & `corkus_py-3.1.0/corkus/objects/member.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/mojang_skin_response.py` & `corkus_py-3.1.0/corkus/objects/mojang_skin_response.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/online_players.py` & `corkus_py-3.1.0/corkus/objects/online_players.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/partial_guild.py` & `corkus_py-3.1.0/corkus/objects/partial_guild.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/partial_ingredient.py` & `corkus_py-3.1.0/corkus/objects/partial_ingredient.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/partial_member.py` & `corkus_py-3.1.0/corkus/objects/partial_member.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/partial_online_player.py` & `corkus_py-3.1.0/corkus/objects/partial_online_player.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/partial_player.py` & `corkus_py-3.1.0/corkus/objects/partial_player.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/partial_recipe.py` & `corkus_py-3.1.0/corkus/objects/partial_recipe.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/partial_server.py` & `corkus_py-3.1.0/corkus/objects/partial_server.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/partial_teritories.py` & `corkus_py-3.1.0/corkus/objects/partial_teritories.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/player.py` & `corkus_py-3.1.0/corkus/objects/player.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/player_character.py` & `corkus_py-3.1.0/corkus/objects/player_character.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/player_gamemodes.py` & `corkus_py-3.1.0/corkus/objects/player_gamemodes.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/player_profession.py` & `corkus_py-3.1.0/corkus/objects/player_profession.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/player_ranking.py` & `corkus_py-3.1.0/corkus/objects/player_ranking.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/player_statistics.py` & `corkus_py-3.1.0/corkus/objects/player_statistics.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/player_status.py` & `corkus_py-3.1.0/corkus/objects/player_status.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/playtime.py` & `corkus_py-3.1.0/corkus/objects/playtime.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/quest.py` & `corkus_py-3.1.0/corkus/objects/quest.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/raid.py` & `corkus_py-3.1.0/corkus/objects/raid.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/recipe.py` & `corkus_py-3.1.0/corkus/objects/recipe.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/search_result.py` & `corkus_py-3.1.0/corkus/objects/search_result.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/server.py` & `corkus_py-3.1.0/corkus/objects/server.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/skill_points.py` & `corkus_py-3.1.0/corkus/objects/skill_points.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/territory.py` & `corkus_py-3.1.0/corkus/objects/territory.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/territory_location.py` & `corkus_py-3.1.0/corkus/objects/territory_location.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/uuid.py` & `corkus_py-3.1.0/corkus/objects/uuid.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/objects/weapon_damage.py` & `corkus_py-3.1.0/corkus/objects/weapon_damage.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/utils/cache.py` & `corkus_py-3.1.0/corkus/utils/cache.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/utils/enum.py` & `corkus_py-3.1.0/corkus/utils/enum.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/utils/ratelimit.py` & `corkus_py-3.1.0/corkus/utils/ratelimit.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/utils/request.py` & `corkus_py-3.1.0/corkus/utils/request.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus/utils/utils.py` & `corkus_py-3.1.0/corkus/utils/utils.py`

 * *Files identical despite different names*

### Comparing `corkus.py-3.0.1/corkus.py.egg-info/SOURCES.txt` & `corkus_py-3.1.0/corkus.py.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -85,8 +85,24 @@
 corkus/objects/uuid.py
 corkus/objects/weapon_damage.py
 corkus/utils/__init__.py
 corkus/utils/cache.py
 corkus/utils/enum.py
 corkus/utils/ratelimit.py
 corkus/utils/request.py
-corkus/utils/utils.py
+corkus/utils/utils.py
+tests/test_cache.py
+tests/test_corkus.py
+tests/test_enum.py
+tests/test_guild.py
+tests/test_ingredient.py
+tests/test_item.py
+tests/test_leaderboard.py
+tests/test_network.py
+tests/test_player.py
+tests/test_playtime.py
+tests/test_ratelimit.py
+tests/test_recipe.py
+tests/test_request.py
+tests/test_search.py
+tests/test_territory.py
+tests/test_uuid.py
```

### Comparing `corkus.py-3.0.1/setup.py` & `corkus_py-3.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     description='Asynchronous, feature-rich and easy to use Python wrapper for Public Wynncraft API',
     long_description=readme,
     long_description_content_type="text/markdown",
     include_package_data=True,
     install_requires=requirements,
     python_requires='>=3.8.0',
     classifiers=[
-    'Development Status :: 5 - Production/Stable',
+    'Development Status :: 7 - Inactive',
     'License :: OSI Approved :: MIT License',
     'Intended Audience :: Developers',
     'Natural Language :: English',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
```

