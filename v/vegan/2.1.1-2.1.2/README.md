# Comparing `tmp/vegan-2.1.1.tar.gz` & `tmp/vegan-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vegan-2.1.1.tar", max compression
+gzip compressed data, was "vegan-2.1.2.tar", max compression
```

## Comparing `vegan-2.1.1.tar` & `vegan-2.1.2.tar`

### file list

```diff
@@ -1,698 +1,698 @@
--rwxr-xr-x   0        0        0      978 2024-04-28 22:58:20.333449 vegan-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      105 2024-04-27 16:44:17.965844 vegan-2.1.1/venue, journal.S.HTML
--rwxr-xr-x   0        0        0     1606 2024-04-28 19:08:53.538304 vegan-2.1.1/venue.S.HTML
--rwxr-xr-x   0        0        0      527 2024-04-17 03:36:20.919517 vegan-2.1.1/venues/stages/vegan/___license/license.s.HTML
--rwxr-xr-x   0        0        0    37279 2024-04-17 03:33:22.077284 vegan-2.1.1/venues/stages/vegan/___license/list/gpl-3.0-standalone.html
--rw-r--r--   0        0        0      131 2024-04-28 20:54:59.933399 vegan-2.1.1/venues/stages/vegan/___license/list/non-commercial.S.HTML
--rwxr-xr-x   0        0        0      112 2024-04-17 03:33:22.077284 vegan-2.1.1/venues/stages/vegan/___license/list/vegan.s.HTML
--rwxr-xr-x   0        0        0      405 2024-04-17 03:33:22.073284 vegan-2.1.1/venues/stages/vegan/___objectives/book/Vitamin B.S.HTML
--rwxr-xr-x   0        0        0       63 2024-04-17 03:33:22.073284 vegan-2.1.1/venues/stages/vegan/___objectives/book/Vitamin K.S.HTML
--rw-r--r--   0        0        0      201 2024-04-28 20:53:16.850555 vegan-2.1.1/venues/stages/vegan/___objectives/objectives - elliptic.S.HTML
--rwxr-xr-x   0        0        0     1274 2024-04-28 20:51:03.764043 vegan-2.1.1/venues/stages/vegan/___objectives/objectives.S.HTML
--rwxr-xr-x   0        0        0      376 2024-04-17 03:36:20.951516 vegan-2.1.1/venues/stages/vegan/__dictionary/vegan_1
--rwxr-xr-x   0        0        0      403 2024-04-17 03:36:20.919517 vegan-2.1.1/venues/stages/vegan/__init__.py
--rwxr-xr-x   0        0        0    93154 2024-04-28 20:56:44.192241 vegan-2.1.1/venues/stages/vegan/__status/API/DB/records.json
--rwxr-xr-x   0        0        0     2094 2024-04-27 16:55:04.129273 vegan-2.1.1/venues/stages/vegan/__status/API/status.proc.py
--rwxr-xr-x   0        0        0     1172 2024-04-17 03:33:22.077284 vegan-2.1.1/venues/stages/vegan/__status/__pycache__/status_API.proc.cpython-310.pyc
--rwxr-xr-x   0        0        0       11 2024-04-23 21:56:29.284154 vegan-2.1.1/venues/stages/vegan/__status/main/.gitignore
--rwxr-xr-x   0        0        0 13330130 2024-04-28 20:56:31.644379 vegan-2.1.1/venues/stages/vegan/__status/main/DB/records.json
--rw-r--r--   0        0        0    41183 2024-04-25 01:22:42.760494 vegan-2.1.1/venues/stages/vegan/__status/main/output.json
--rwxr-xr-x   0        0        0     2106 2024-04-28 00:14:24.216317 vegan-2.1.1/venues/stages/vegan/__status/main/status.proc.py
--rwxr-xr-x   0        0        0      454 2024-04-17 03:36:21.219514 vegan-2.1.1/venues/stages/vegan/_ellipses--/__init__.py
--rwxr-xr-x   0        0        0      595 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/_ellipses--/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      891 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/_ellipses--/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1124 2024-04-24 21:00:13.657608 vegan-2.1.1/venues/stages/vegan/_essence/__init__.py
--rwxr-xr-x   0        0        0      839 2024-04-24 21:00:32.929451 vegan-2.1.1/venues/stages/vegan/_essence/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3705 2024-04-28 19:04:01.618019 vegan-2.1.1/venues/stages/vegan/_essence/build/__init__.py
--rw-r--r--   0        0        0     2530 2024-04-28 19:04:04.274021 vegan-2.1.1/venues/stages/vegan/_essence/build/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      202 2024-04-27 16:49:31.955662 vegan-2.1.1/venues/stages/vegan/_essence/essence.S.HTML
--rw-r--r--   0        0        0      475 2024-04-27 21:56:20.995877 vegan-2.1.1/venues/stages/vegan/_essence/run_script/__init__.py
--rwxr-xr-x   0        0        0      738 2024-04-23 19:31:08.382022 vegan-2.1.1/venues/stages/vegan/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0      756 2024-04-23 19:30:52.306199 vegan-2.1.1/venues/stages/vegan/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      544 2024-04-23 19:31:08.382022 vegan-2.1.1/venues/stages/vegan/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0      781 2024-04-23 19:31:08.382022 vegan-2.1.1/venues/stages/vegan/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1623 2024-04-24 00:54:42.885927 vegan-2.1.1/venues/stages/vegan/_ops/clique/__init__.py
--rwxr-xr-x   0        0        0     1591 2024-04-24 00:54:47.309876 vegan-2.1.1/venues/stages/vegan/_ops/clique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1361 2024-04-24 00:54:47.309876 vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      770 2024-04-23 22:34:43.485503 vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0      788 2024-04-23 22:34:42.625514 vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      571 2024-04-23 22:34:43.485503 vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0      807 2024-04-23 22:34:43.485503 vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      662 2024-04-24 00:54:33.574033 vegan-2.1.1/venues/stages/vegan/adventures/_ops/_clique.py
--rwxr-xr-x   0        0        0      794 2024-04-23 19:52:04.387492 vegan-2.1.1/venues/stages/vegan/adventures/_ops/monitor.py
--rwxr-xr-x   0        0        0      613 2024-04-23 22:31:52.519576 vegan-2.1.1/venues/stages/vegan/adventures/_ops/off.py
--rwxr-xr-x   0        0        0      612 2024-04-23 22:31:52.539576 vegan-2.1.1/venues/stages/vegan/adventures/_ops/on.py
--rwxr-xr-x   0        0        0      426 2024-04-23 22:31:52.551576 vegan-2.1.1/venues/stages/vegan/adventures/_ops/refresh.py
--rwxr-xr-x   0        0        0      692 2024-04-23 22:31:52.567575 vegan-2.1.1/venues/stages/vegan/adventures/_ops/status.py
--rwxr-xr-x   0        0        0      342 2024-04-24 01:44:03.440834 vegan-2.1.1/venues/stages/vegan/adventures/adventures.S.HTML
--rwxr-xr-x   0        0        0      152 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/customs/__init__.py
--rwxr-xr-x   0        0        0      601 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/customs/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      926 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/customs/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      245 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/customs/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0      345 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/customs/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0      251 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/customs/__pycache__/status.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-27 23:15:29.829818 vegan-2.1.1/venues/stages/vegan/adventures/customs/_ops/off.py
--rw-r--r--   0        0        0        0 2024-04-27 23:15:26.181863 vegan-2.1.1/venues/stages/vegan/adventures/customs/_ops/on.py
--rw-r--r--   0        0        0        2 2024-04-27 23:15:34.237762 vegan-2.1.1/venues/stages/vegan/adventures/customs/_ops/status.py
--rwxr-xr-x   0        0        0      549 2024-04-23 22:31:52.579575 vegan-2.1.1/venues/stages/vegan/adventures/customs/clique.py
--rw-r--r--   0        0        0      289 2024-04-27 23:17:27.076359 vegan-2.1.1/venues/stages/vegan/adventures/customs/configs_school/embargo.NFT
--rwxr-xr-x   0        0        0      145 2024-04-27 23:16:20.801181 vegan-2.1.1/venues/stages/vegan/adventures/customs/customs.S.HTML
--rwxr-xr-x   0        0        0       14 2024-04-24 01:06:32.184393 vegan-2.1.1/venues/stages/vegan/adventures/monetary/.gitignore
--rwxr-xr-x   0        0        0       17 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/.gitignore
--rwxr-xr-x   0        0        0      454 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__itinerary/itinerary.S.HTML
--rwxr-xr-x   0        0        0     1820 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__pycache__/clique.cpython-310.pyc
--rw-r--r--   0        0        0      748 2024-04-28 01:02:18.999830 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__pycache__/connect.cpython-310.pyc
--rw-r--r--   0        0        0      783 2024-04-28 01:02:21.999797 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/find_name.cpython-310.pyc
--rwxr-xr-x   0        0        0        4 2024-04-28 00:13:51.336698 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/insert_document.cpython-310.pyc
--rw-r--r--   0        0        0      795 2024-04-28 01:02:18.999830 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/retrieve_every.cpython-310.pyc
--rwxr-xr-x   0        0        0      196 2024-04-24 22:53:29.564774 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/_land.S.HTML
--rwxr-xr-x   0        0        0      700 2024-04-28 01:02:04.667987 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/find_name.py
--rwxr-xr-x   0        0        0      924 2024-04-28 01:06:31.349043 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/insert_document.py
--rwxr-xr-x   0        0        0      601 2024-04-28 01:02:04.735986 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/retrieve_every.py
--rwxr-xr-x   0        0        0      170 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/cautionary_ingredients/cautionary_ingredients.S.HTML
--rwxr-xr-x   0        0        0     1019 2024-04-28 01:02:06.219970 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/connect.py
--rwxr-xr-x   0        0        0      721 2024-04-24 23:09:34.366674 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/essential_nutrients/essential_nutrients.S.HTML
--rwxr-xr-x   0        0        0      401 2024-04-24 23:06:14.224847 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/glossary/glossary.S.HTML
--rw-r--r--   0        0        0     1303 2024-04-28 04:32:41.571189 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/find_ingredient.cpython-310.pyc
--rw-r--r--   0        0        0     1347 2024-04-28 01:13:28.732365 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/insert.cpython-310.pyc
--rw-r--r--   0        0        0      707 2024-04-28 01:33:42.490573 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/retrieve_one.cpython-310.pyc
--rw-r--r--   0        0        0      860 2024-04-28 02:43:34.943005 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/__pycache__/create.cpython-310.pyc
--rw-r--r--   0        0        0      887 2024-04-28 02:46:59.456565 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/__pycache__/drop_and_create.cpython-310.pyc
--rw-r--r--   0        0        0      624 2024-04-28 02:46:44.020748 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/drop_and_create.py
--rw-r--r--   0        0        0     1087 2024-04-28 04:32:39.723209 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/find_ingredient.py
--rw-r--r--   0        0        0      117 2024-04-28 02:07:02.567921 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/goals.S.HTML
--rw-r--r--   0        0        0     1304 2024-04-28 03:26:22.405607 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/insert.py
--rw-r--r--   0        0        0      606 2024-04-28 01:33:38.874614 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/retrieve_one.py
--rwxr-xr-x   0        0        0     1477 2024-04-23 20:40:34.490341 vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/ingredients.S.HTML
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__init__.py
--rwxr-xr-x   0        0        0      150 2024-04-17 03:36:48.047066 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1687 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      680 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/connect.cpython-310.pyc
--rwxr-xr-x   0        0        0      857 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1904 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1610 2024-04-23 19:31:08.342022 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0        0 2024-04-28 19:01:53.133950 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/ingredients/cautionary_ingredients/5.JSON
--rwxr-xr-x   0        0        0        0 2024-04-28 19:01:54.085950 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/ingredients/essential_nutrients/5.JSON
--rwxr-xr-x   0        0        0        0 2024-04-28 19:01:55.089950 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/ingredients/glossary/5.JSON
--rwxr-xr-x   0        0        0      118 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/1.JSON
--rwxr-xr-x   0        0        0      118 2024-04-23 22:05:34.538523 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/2.JSON
--rwxr-xr-x   0        0        0      118 2024-04-23 22:07:10.673303 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/3.JSON
--rwxr-xr-x   0        0        0      118 2024-04-27 17:35:00.336394 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/4.JSON
--rwxr-xr-x   0        0        0      118 2024-04-28 19:02:50.497975 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/5.JSON
--rwxr-xr-x   0        0        0      118 2024-04-28 19:04:10.818025 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/6.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/1.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-23 22:05:35.566512 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/2.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-23 22:07:11.713281 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/3.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-27 17:35:01.316362 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/4.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-28 19:02:51.533976 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/5.JSON
--rwxr-xr-x   0        0        0     5140 2024-04-28 19:04:11.850026 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/6.JSON
--rwxr-xr-x   0        0        0        0 2024-04-23 22:05:36.562502 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/2.JSON
--rwxr-xr-x   0        0        0        0 2024-04-23 22:07:12.697261 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/3.JSON
--rwxr-xr-x   0        0        0        0 2024-04-27 17:35:02.312330 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/4.JSON
--rwxr-xr-x   0        0        0        0 2024-04-28 19:02:52.497976 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/5.JSON
--rwxr-xr-x   0        0        0        0 2024-04-28 19:04:12.822027 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/6.JSON
--rwxr-xr-x   0        0        0     5771 2024-04-28 19:04:04.554021 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/goals/5.JSON
--rwxr-xr-x   0        0        0     5771 2024-04-28 19:04:13.826027 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/goals/6.JSON
--rwxr-xr-x   0        0        0      564 2024-04-27 23:14:58.002218 vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/saves.S.HTML
--rwxr-xr-x   0        0        0     1434 2024-04-23 20:09:59.888961 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0      868 2024-04-22 01:43:44.052692 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc
--rw-r--r--   0        0        0     1973 2024-04-28 15:55:33.174259 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1620 2024-04-23 22:34:43.293506 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1079 2024-04-23 20:09:44.305153 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/_clique.py
--rwxr-xr-x   0        0        0      865 2024-04-22 01:43:41.108724 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/off.py
--rwxr-xr-x   0        0        0     2428 2024-04-28 15:55:30.526268 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/on.py
--rw-r--r--   0        0        0     2460 2024-04-28 19:04:04.542021 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     2152 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc
--rwxr-xr-x   0        0        0     2843 2024-04-28 19:03:52.654013 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/_clique.py
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/dumps/dump.py
--rwxr-xr-x   0        0        0        2 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/dumps/restore.py
--rwxr-xr-x   0        0        0        2 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/exports/export.py
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/exports/import.py
--rwxr-xr-x   0        0        0      390 2024-04-23 20:10:51.728325 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/memories.S.HTML
--rwxr-xr-x   0        0        0     1764 2024-04-23 22:31:52.611575 vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/status.py
--rwxr-xr-x   0        0        0      453 2024-04-23 21:03:13.015179 vegan-2.1.1/venues/stages/vegan/adventures/monetary/monetary.S.HTML
--rwxr-xr-x   0        0        0       46 2024-04-27 23:28:20.716508 vegan-2.1.1/venues/stages/vegan/adventures/monetary/moves/saves/export/__init__.py
--rwxr-xr-x   0        0        0     1343 2024-04-23 22:34:43.485503 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/off.cpython-310.pyc
--rwxr-xr-x   0        0        0     1759 2024-04-23 22:34:42.625513 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1288 2024-04-23 22:34:43.489503 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1311 2024-04-23 22:34:42.629513 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0      792 2024-04-24 18:58:20.084451 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/_clique.py
--rwxr-xr-x   0        0        0      328 2024-04-24 18:58:20.096451 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/off.py
--rwxr-xr-x   0        0        0      325 2024-04-24 18:58:20.108451 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/on.py
--rwxr-xr-x   0        0        0      330 2024-04-24 18:58:20.116451 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/refresh.py
--rwxr-xr-x   0        0        0      339 2024-04-24 18:58:20.116451 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/status.py
--rwxr-xr-x   0        0        0      130 2024-04-24 18:57:58.564669 vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/redis_mix.S.HTML
--rwxr-xr-x   0        0        0      188 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/sanique/__init__.py
--rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 vegan-2.1.1/venues/stages/vegan/adventures/sanique/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1343 2024-04-23 22:34:43.485503 vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc
--rw-r--r--   0        0        0     1759 2024-04-25 21:35:38.123051 vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc
--rwxr-xr-x   0        0        0     1288 2024-04-23 22:34:43.489503 vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc
--rwxr-xr-x   0        0        0     1311 2024-04-23 22:34:42.629514 vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc
--rwxr-xr-x   0        0        0     1380 2024-04-23 22:31:52.655574 vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/off.py
--rwxr-xr-x   0        0        0     1831 2024-04-25 21:31:37.994003 vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/on.py
--rwxr-xr-x   0        0        0     1164 2024-04-23 22:31:52.683574 vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/refresh.py
--rwxr-xr-x   0        0        0     1229 2024-04-23 22:31:52.699574 vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/status.py
--rwxr-xr-x   0        0        0      781 2024-04-23 22:31:52.711573 vegan-2.1.1/venues/stages/vegan/adventures/sanique/clique.py
--rwxr-xr-x   0        0        0     6337 2024-04-28 20:50:26.408443 vegan-2.1.1/venues/stages/vegan/adventures/sanique/harbor/__init__.py
--rw-r--r--   0        0        0     5040 2024-04-28 20:50:30.200402 vegan-2.1.1/venues/stages/vegan/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      524 2024-04-17 03:36:20.947517 vegan-2.1.1/venues/stages/vegan/adventures/sanique/sanique.S.HTML
--rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 vegan-2.1.1/venues/stages/vegan/adventures/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
--rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/adventures/sanique/utilities/has_sanic_check.py
--rwxr-xr-x   0        0        0      151 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/affiliates_Amazon/affiliates.s.HTML
--rwxr-xr-x   0        0        0      176 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/besties.S.HTML
--rwxr-xr-x   0        0        0      596 2024-04-17 03:36:49.119045 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/__pycache__/source.cpython-310.pyc
--rwxr-xr-x   0        0        0      738 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/__pycache__/source.cpython-311.pyc
--rwxr-xr-x   0        0        0     1255 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/__init__.py
--rw-r--r--   0        0        0     1552 2024-04-27 17:40:11.463956 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2127 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      776 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc
--rwxr-xr-x   0        0        0      450 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/FOUNDATIONAL.cpython-311.pyc
--rw-r--r--   0        0        0      646 2024-04-27 17:40:11.499956 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc
--rwxr-xr-x   0        0        0      778 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc
--rw-r--r--   0        0        0      496 2024-04-27 17:40:11.499956 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-310.pyc
--rwxr-xr-x   0        0        0      677 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc
--rwxr-xr-x   0        0        0      508 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/branded.py
--rwxr-xr-x   0        0        0      262 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/foundational.py
--rwxr-xr-x   0        0        0      466 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/status/API_status_branded_1.py
--rwxr-xr-x   0        0        0      533 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/status/API_status_foundational_1.py
--rw-r--r--   0        0        0      739 2024-04-27 17:40:30.387524 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/status/__pycache__/API_status_branded_1.cpython-310.pyc
--rw-r--r--   0        0        0      734 2024-04-27 17:40:30.383524 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/status/__pycache__/API_status_foundational_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      370 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/source.py
--rwxr-xr-x   0        0        0      939 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/__init__.py
--rw-r--r--   0        0        0     1125 2024-04-27 17:40:11.499956 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2082 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      740 2024-04-27 17:40:12.739927 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0    37079 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON
--rwxr-xr-x   0        0        0    37079 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON
--rwxr-xr-x   0        0        0     7242 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/beet_juice_2412474.JSON
--rwxr-xr-x   0        0        0     8522 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/beet_juice_2642759.JSON
--rwxr-xr-x   0        0        0    33964 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/impossible_beef_2664238.JSON
--rwxr-xr-x   0        0        0    17926 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/problems/impossible_2468423.JSON
--rwxr-xr-x   0        0        0      104 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/problems/problems.r.HTML
--rwxr-xr-x   0        0        0    10678 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/vegan_pizza_2672996.JSON
--rwxr-xr-x   0        0        0    10670 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/walnuts_1882785.JSON
--rwxr-xr-x   0        0        0   189146 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON
--rwxr-xr-x   0        0        0      255 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/mergers.r.HTML
--rwxr-xr-x   0        0        0       88 2024-04-17 03:33:22.097283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/priorities.r.HTML
--rwxr-xr-x   0        0        0      454 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/status_1.py
--rwxr-xr-x   0        0        0     1210 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/food.s.HTML
--rwxr-xr-x   0        0        0     4580 2024-04-27 18:21:30.033645 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/__init__.py
--rw-r--r--   0        0        0     2455 2024-04-27 18:24:41.143411 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1748 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__init__.py
--rw-r--r--   0        0        0     1194 2024-04-27 17:40:11.551954 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2050 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      571 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1065 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-311.pyc
--rw-r--r--   0        0        0     1339 2024-04-27 17:40:12.659929 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      599 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__init__.py
--rwxr-xr-x   0        0        0      596 2024-04-17 03:36:50.207023 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4071 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__init__.py
--rw-r--r--   0        0        0     2918 2024-04-27 17:40:11.551954 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     5397 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1247 2024-04-27 17:40:12.671929 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_mass_1.cpython-310.pyc
--rw-r--r--   0        0        0      983 2024-04-27 17:40:12.975921 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_volume_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      421 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__init__.py
--rwxr-xr-x   0        0        0      563 2024-04-17 03:36:50.203023 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      946 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1243 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_mass_1.py
--rwxr-xr-x   0        0        0      891 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_volume_1.py
--rwxr-xr-x   0        0        0     1392 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/status_1.py
--rw-r--r--   0        0        0      614 2024-04-28 20:33:03.399922 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/API_status_found_1.py
--rw-r--r--   0        0        0      587 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/API_status_not_found_1.py
--rw-r--r--   0        0        0     1768 2024-04-27 18:21:13.609835 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__init__.py
--rw-r--r--   0        0        0      745 2024-04-27 17:18:55.070676 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_1.cpython-310.pyc
--rw-r--r--   0        0        0      836 2024-04-28 20:33:06.991881 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_found_1.cpython-310.pyc
--rw-r--r--   0        0        0      757 2024-04-27 17:40:30.383524 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_not_found_1.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2024-04-27 18:24:41.239410 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1414 2024-04-27 17:40:12.831925 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_1_description.cpython-310.pyc
--rw-r--r--   0        0        0     1823 2024-04-27 17:40:12.991921 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_2_measures.cpython-310.pyc
--rw-r--r--   0        0        0     1536 2024-04-27 17:40:12.659929 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc
--rw-r--r--   0        0        0     1594 2024-04-25 01:35:26.781309 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_4_land_essentials.cpython-310.pyc
--rw-r--r--   0        0        0     1685 2024-04-27 17:40:13.295914 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_4_lands.cpython-310.pyc
--rwxr-xr-x   0        0        0     1158 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_1_description.py
--rwxr-xr-x   0        0        0     1866 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_2_measures.py
--rwxr-xr-x   0        0        0     2071 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_3_measured_ingredients.py
--rwxr-xr-x   0        0        0     1489 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_4_lands.py
--rw-r--r--   0        0        0     2071 2024-04-27 17:40:12.231939 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1586 2024-04-27 17:40:12.667929 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0     1098 2024-04-27 17:40:12.559931 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2412474.cpython-310.pyc
--rw-r--r--   0        0        0     1437 2024-04-27 17:40:12.411935 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_3.cpython-310.pyc
--rw-r--r--   0        0        0     1201 2024-04-27 17:40:12.471933 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_loop_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2765 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_1.py
--rwxr-xr-x   0        0        0     1617 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_2.py
--rwxr-xr-x   0        0        0      708 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_2412474.py
--rwxr-xr-x   0        0        0     1080 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_3.py
--rwxr-xr-x   0        0        0      844 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_loop_1.py
--rwxr-xr-x   0        0        0     2276 2024-04-28 01:02:04.787985 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/land/__init__.py
--rw-r--r--   0        0        0     2093 2024-04-28 01:02:21.911798 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/land/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      466 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__init__.py
--rwxr-xr-x   0        0        0      568 2024-04-17 03:36:50.287021 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      957 2024-04-17 03:33:22.101283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1166 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__init__.py
--rw-r--r--   0        0        0      833 2024-04-27 17:40:12.419934 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1012 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      703 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__init__.py
--rw-r--r--   0        0        0      827 2024-04-27 17:40:12.419934 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1272 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1360 2024-04-27 17:40:12.507932 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1062 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/status_1.py
--rw-r--r--   0        0        0     1979 2024-04-27 17:40:12.447934 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_mass_1.cpython-310.pyc
--rw-r--r--   0        0        0      999 2024-04-27 17:40:12.715928 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_volume_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     2079 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/status_mass_1.py
--rwxr-xr-x   0        0        0      716 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/status_volume_1.py
--rwxr-xr-x   0        0        0     1143 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured ingredients.S.HTML
--rwxr-xr-x   0        0        0     1421 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__init__.py
--rw-r--r--   0        0        0     1109 2024-04-27 17:40:12.387935 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1591 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1606 2024-04-27 17:40:12.795926 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_IU_1.cpython-310.pyc
--rw-r--r--   0        0        0     1505 2024-04-27 17:40:12.291937 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_energy_1.cpython-310.pyc
--rw-r--r--   0        0        0     1603 2024-04-27 17:40:12.955922 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_mass_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1705 2024-04-27 17:39:04.185559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_IU_1.py
--rwxr-xr-x   0        0        0     1904 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_energy_1.py
--rwxr-xr-x   0        0        0     1608 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_mass_1.py
--rwxr-xr-x   0        0        0     1724 2024-04-17 03:36:21.175514 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__init__.py
--rwxr-xr-x   0        0        0     1435 2024-04-17 03:36:50.287021 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3142 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1232 2024-04-17 03:36:21.147514 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__init__.py
--rwxr-xr-x   0        0        0     1246 2024-04-17 03:36:50.291021 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1831 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1489 2024-04-17 03:36:21.175514 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__init__.py
--rwxr-xr-x   0        0        0     1198 2024-04-17 03:36:50.291021 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1791 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1379 2024-04-17 03:36:21.175514 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__init__.py
--rwxr-xr-x   0        0        0     1335 2024-04-17 03:36:50.291021 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1842 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      706 2024-04-17 03:36:50.291021 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc
--rwxr-xr-x   0        0        0     1040 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc
--rwxr-xr-x   0        0        0     1899 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc
--rwxr-xr-x   0        0        0      651 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc
--rwxr-xr-x   0        0        0      845 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc
--rwxr-xr-x   0        0        0      849 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc
--rwxr-xr-x   0        0        0      636 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/food_nutrient.py
--rwxr-xr-x   0        0        0      483 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/label_nutrient.py
--rwxr-xr-x   0        0        0      503 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient.r.HTML
--rwxr-xr-x   0        0        0      706 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient_prototype_1.r.HTML
--rwxr-xr-x   0        0        0     3859 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__init__.py
--rw-r--r--   0        0        0     2386 2024-04-27 17:40:12.343936 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4016 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1360 2024-04-27 17:40:12.655929 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/status_mass_1.cpython-310.pyc
--rw-r--r--   0        0        0     1391 2024-04-27 17:40:13.079919 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/status_volume_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      110 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/form.S.HTML
--rwxr-xr-x   0        0        0     1232 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/status_mass_1.py
--rwxr-xr-x   0        0        0     1175 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/status_volume_1.py
--rwxr-xr-x   0        0        0      306 2024-04-27 17:39:04.189559 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/nature_v2.S.HTML
--rwxr-xr-x   0        0        0      102 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/unmeasured_ingredients/__init__.py
--rwxr-xr-x   0        0        0      338 2024-04-17 03:36:50.291021 vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/unmeasured_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1042 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/NIH.s.HTML
--rw-r--r--   0        0        0      536 2024-04-27 16:55:09.193236 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc
--rwxr-xr-x   0        0        0      670 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc
--rwxr-xr-x   0        0        0     1131 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__init__.py
--rw-r--r--   0        0        0     1131 2024-04-27 17:40:30.767515 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1889 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      815 2024-04-27 16:55:09.193236 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc
--rwxr-xr-x   0        0        0     1399 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc
--rwxr-xr-x   0        0        0     1087 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/assertions.py
--rwxr-xr-x   0        0        0      434 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/status/API_status_1.py
--rw-r--r--   0        0        0      698 2024-04-27 17:40:30.387524 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/status/__pycache__/API_status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      316 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/source.py
--rwxr-xr-x   0        0        0      844 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/__init__.py
--rw-r--r--   0        0        0     1038 2024-04-27 17:40:15.195870 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1918 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0    44597 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/coated tablets/multivitamin_276336.JSON
--rwxr-xr-x   0        0        0    22180 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/other/chia_seeds_214893.JSON
--rwxr-xr-x   0        0        0     6430 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/powder/mane_270619.JSON
--rwxr-xr-x   0        0        0    72594 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/powder/nutritional_shake_220884.JSON
--rwxr-xr-x   0        0        0    57378 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/powder packets/multivitamin_246811.JSON
--rwxr-xr-x   0        0        0    22710 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/tablets/calcium_261967.JSON
--rwxr-xr-x   0        0        0    43725 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/tablets/multivitamin_249664.JSON
--rwxr-xr-x   0        0        0     7107 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON
--rw-r--r--   0        0        0     4047 2024-04-27 18:25:39.806722 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/__init__.py
--rw-r--r--   0        0        0     2752 2024-04-27 18:25:55.126541 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      271 2024-04-17 03:36:50.963008 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      383 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1147 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__init__.py
--rw-r--r--   0        0        0      906 2024-04-27 17:40:15.039874 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1201 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1229 2024-04-27 17:40:13.511909 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/status_powder_packets_246811.cpython-310.pyc
--rwxr-xr-x   0        0        0      931 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/status_powder_packets_246811.py
--rwxr-xr-x   0        0        0       56 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/servingSizeUnit/__init__.py
--rw-r--r--   0        0        0     1917 2024-04-27 17:48:43.182166 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_ops/retrieve/__init__.py
--rw-r--r--   0        0        0     1763 2024-04-27 17:48:48.074086 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1410 2024-04-27 17:40:14.187894 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_1_info.cpython-310.pyc
--rw-r--r--   0        0        0     1418 2024-04-27 17:40:14.083896 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_2_form.cpython-310.pyc
--rw-r--r--   0        0        0     1827 2024-04-27 17:40:13.859901 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc
--rw-r--r--   0        0        0     1236 2024-04-25 18:59:21.733410 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_essential_nutrients.cpython-310.pyc
--rw-r--r--   0        0        0     1474 2024-04-27 17:40:13.847901 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_unmeasured_ingredients.cpython-310.pyc
--rw-r--r--   0        0        0     1661 2024-04-27 17:40:14.131895 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_5_essential_nutrients.cpython-310.pyc
--rw-r--r--   0        0        0     1589 2024-04-27 17:40:13.907900 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_6_cautionary_ingredients.cpython-310.pyc
--rw-r--r--   0        0        0    28721 2024-04-28 20:56:28.872410 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/mane_270619_nature.JSON
--rw-r--r--   0        0        0   124533 2024-04-28 20:56:29.068408 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/multivitamin_249664.JSON
--rw-r--r--   0        0        0     1036 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_1_info.py
--rw-r--r--   0        0        0     1046 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_2_form.py
--rw-r--r--   0        0        0     1614 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_3_measured_ingredients.py
--rw-r--r--   0        0        0     1065 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_4_unmeasured_ingredients.py
--rw-r--r--   0        0        0     1271 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_5_essential_nutrients.py
--rw-r--r--   0        0        0     1164 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_6_cautionary_ingredients.py
--rw-r--r--   0        0        0      828 2024-04-27 17:40:12.847925 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/_loop/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      736 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/_loop/status_1.py
--rw-r--r--   0        0        0     1741 2024-04-27 17:40:13.223916 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/__pycache__/status_multivitamin_276336.cpython-310.pyc
--rwxr-xr-x   0        0        0     1557 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336.py
--rwxr-xr-x   0        0        0   136805 2024-04-28 20:56:29.368405 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336_nature.JSON
--rw-r--r--   0        0        0     1209 2024-04-27 17:40:13.147918 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/__pycache__/status_chia_seeds_214893.cpython-310.pyc
--rwxr-xr-x   0        0        0    82230 2024-04-28 20:56:28.848410 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/chia_seeds_214893_nature.JSON
--rwxr-xr-x   0        0        0      763 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/status_chia_seeds_214893.py
--rw-r--r--   0        0        0     1172 2024-04-27 17:40:12.731927 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/__pycache__/status_mane_270619.cpython-310.pyc
--rwxr-xr-x   0        0        0    28721 2024-04-28 20:56:25.788444 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/mane_270619_nature.JSON
--rwxr-xr-x   0        0        0      736 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/status_mane_270619.py
--rw-r--r--   0        0        0      568 2024-04-25 04:11:27.433921 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      672 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      665 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__init__.py
--rw-r--r--   0        0        0      860 2024-04-27 17:40:15.039874 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1333 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      767 2024-04-27 17:40:13.195917 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/status_other_214893.cpython-310.pyc
--rwxr-xr-x   0        0        0      512 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/status_other_214893.py
--rwxr-xr-x   0        0        0      512 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/form.S.HTML
--rwxr-xr-x   0        0        0     3783 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__init__.py
--rw-r--r--   0        0        0     2355 2024-04-27 17:40:15.043874 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      179 2024-04-17 03:36:51.818991 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1571 2024-04-27 17:40:13.811902 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_246811.cpython-310.pyc
--rw-r--r--   0        0        0     1546 2024-04-27 17:40:13.511909 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_276336.cpython-310.pyc
--rwxr-xr-x   0        0        0     1781 2024-04-27 17:39:04.201558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/status_246811.py
--rwxr-xr-x   0        0        0     1666 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/status_276336.py
--rwxr-xr-x   0        0        0     3221 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__init__.py
--rw-r--r--   0        0        0     2669 2024-04-27 17:40:14.991875 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1195 2024-04-27 17:40:13.007921 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_coated_tablet_276336.cpython-310.pyc
--rw-r--r--   0        0        0      998 2024-04-27 17:40:13.175917 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_gram_1.cpython-310.pyc
--rw-r--r--   0        0        0     1004 2024-04-27 17:40:13.075919 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_220884.cpython-310.pyc
--rw-r--r--   0        0        0     1037 2024-04-27 17:40:12.371935 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_270619.cpython-310.pyc
--rw-r--r--   0        0        0     1418 2024-04-27 17:40:13.091919 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_packets_246811.cpython-310.pyc
--rw-r--r--   0        0        0      947 2024-04-27 17:40:13.891900 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_tablet_261967.cpython-310.pyc
--rw-r--r--   0        0        0      981 2024-04-27 17:40:13.787903 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_vegan_capsule_248267.cpython-310.pyc
--rwxr-xr-x   0        0        0      929 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_coated_tablet_276336.py
--rwxr-xr-x   0        0        0      816 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_gram_1.py
--rwxr-xr-x   0        0        0      820 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_220884.py
--rwxr-xr-x   0        0        0      893 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_270619.py
--rwxr-xr-x   0        0        0     1333 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_packets_246811.py
--rwxr-xr-x   0        0        0      703 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_tablet_261967.py
--rwxr-xr-x   0        0        0      727 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_vegan_capsule_248267.py
--rw-r--r--   0        0        0     1881 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/land/__init__.py
--rw-r--r--   0        0        0     1983 2024-04-27 17:40:15.187871 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/land/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1613 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__init__.py
--rw-r--r--   0        0        0     1857 2024-04-27 17:40:15.043874 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2911 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1119 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__init__.py
--rw-r--r--   0        0        0     1079 2024-04-27 17:40:15.187871 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1442 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      961 2024-04-27 17:40:13.363913 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      664 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/status_1.py
--rwxr-xr-x   0        0        0      587 2024-04-27 17:39:04.193559 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__init__.py
--rw-r--r--   0        0        0      990 2024-04-27 17:40:18.015806 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1171 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1074 2024-04-27 17:40:13.119918 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_status/__pycache__/status_chia_seeds_214893.cpython-310.pyc
--rwxr-xr-x   0        0        0      801 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_status/status_chia_seeds_214893.py
--rwxr-xr-x   0        0        0     4661 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__init__.py
--rw-r--r--   0        0        0     2795 2024-04-27 17:40:15.043874 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4500 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1630 2024-04-27 17:40:13.151918 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1729 2024-04-27 17:39:04.197558 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/status_1.py
--rwxr-xr-x   0        0        0     1514 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/measured_ingredient.S.HTML
--rwxr-xr-x   0        0        0      561 2024-04-17 03:33:22.109283 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredients.S.HTML
--rw-r--r--   0        0        0        3 2024-04-25 01:50:49.197454 vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/natures_v2.S.HTML
--rw-r--r--   0        0        0       87 2024-04-27 20:03:02.828977 vegan-2.1.1/venues/stages/vegan/goals/goals.S.HTML
--rw-r--r--   0        0        0     8904 2024-04-28 01:16:44.610153 vegan-2.1.1/venues/stages/vegan/goals/umuntu/FDA.py
--rw-r--r--   0        0        0     9794 2024-03-09 19:44:16.627477 vegan-2.1.1/venues/stages/vegan/goals/umuntu/FDA_v1.py
--rw-r--r--   0        0        0     4193 2024-03-10 18:32:48.701726 vegan-2.1.1/venues/stages/vegan/goals/umuntu/FDA_v2.py
--rw-r--r--   0        0        0     7523 2024-03-12 19:40:02.502146 vegan-2.1.1/venues/stages/vegan/goals/umuntu/FDA_v3.py
--rw-r--r--   0        0        0     4337 2024-04-28 01:16:47.442121 vegan-2.1.1/venues/stages/vegan/goals/umuntu/__pycache__/FDA.cpython-310.pyc
--rw-r--r--   0        0        0     3847 2024-03-14 19:34:32.350499 vegan-2.1.1/venues/stages/vegan/goals/umuntu/__pycache__/FDA_v3.cpython-310.pyc
--rw-r--r--   0        0        0       71 2024-04-27 16:41:36.022921 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Carbohydrates.s.HTML
--rw-r--r--   0        0        0       61 2024-04-27 16:41:31.750949 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Fat.s.HTML
--rw-r--r--   0        0        0       64 2024-04-27 16:41:27.998973 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Lipids.s.HTML
--rw-r--r--   0        0        0      145 2024-04-27 16:41:20.183024 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Protein.s.HTML
--rw-r--r--   0        0        0       16 2024-01-31 21:52:02.234756 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Vitamin A.s.HTML
--rw-r--r--   0        0        0        0 2024-01-31 21:52:25.962491 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Vitamin B.s.HTML
--rw-r--r--   0        0        0       68 2024-04-27 16:40:48.275230 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Vitamin C.s.HTML
--rw-r--r--   0        0        0       65 2024-04-27 16:40:44.111256 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Vitamin D.s.HTML
--rw-r--r--   0        0        0      423 2024-04-27 16:42:29.518570 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_journal/Vitamin E.s.HTML
--rw-r--r--   0        0        0      553 2024-04-28 02:16:08.201921 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_ops/__pycache__/retrieve.cpython-310.pyc
--rw-r--r--   0        0        0      352 2024-04-28 01:52:53.553431 vegan-2.1.1/venues/stages/vegan/goals/umuntu/_ops/retrieve.py
--rw-r--r--   0        0        0        3 2024-03-10 18:23:03.506534 vegan-2.1.1/venues/stages/vegan/goals/umuntu/parse_FDA.proc.py
--rw-r--r--   0        0        0      488 2024-04-28 00:30:07.297621 vegan-2.1.1/venues/stages/vegan/goals/umuntu/umuntu.S.HTML
--rwxr-xr-x   0        0        0      799 2024-04-17 03:36:48.015066 vegan-2.1.1/venues/stages/vegan/measures/_interpret/__pycache__/status_unit_kind.cpython-310.pyc
--rwxr-xr-x   0        0        0     1469 2024-04-17 03:36:50.287021 vegan-2.1.1/venues/stages/vegan/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc
--rwxr-xr-x   0        0        0     2547 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc
--rwxr-xr-x   0        0        0       61 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/_interpret/interpret.S.HTML
--rwxr-xr-x   0        0        0      667 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/_interpret/status_unit_kind.py
--rwxr-xr-x   0        0        0     1675 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/_interpret/unit_kind.py
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/biological_activity/__init__.py
--rwxr-xr-x   0        0        0       59 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/electric_current/electric_current.S.HTML
--rwxr-xr-x   0        0        0     1142 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/energy/energy.r.HTML
--rwxr-xr-x   0        0        0     1171 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/energy/swap/__init__.py
--rwxr-xr-x   0        0        0     1016 2024-04-17 03:36:50.291021 vegan-2.1.1/venues/stages/vegan/measures/energy/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1761 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/energy/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      618 2024-04-17 03:36:48.423058 vegan-2.1.1/venues/stages/vegan/measures/energy/swap/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      383 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/energy/swap/status_1.py
--rwxr-xr-x   0        0        0       71 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/length/length.r.HTML
--rwxr-xr-x   0        0        0       95 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/mass/e_note.py
--rwxr-xr-x   0        0        0       12 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/mass/mass.r.html
--rwxr-xr-x   0        0        0     2326 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/mass/swap/__init__.py
--rwxr-xr-x   0        0        0     1724 2024-04-17 03:36:49.175043 vegan-2.1.1/venues/stages/vegan/measures/mass/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3229 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/mass/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1141 2024-04-17 03:36:47.971067 vegan-2.1.1/venues/stages/vegan/measures/mass/swap/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1150 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/mass/swap/status_1.py
--rwxr-xr-x   0        0        0     2419 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/mass/system international.r.html
--rwxr-xr-x   0        0        0      768 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/mass/us customary.r.html
--rwxr-xr-x   0        0        0      520 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__init__.py
--rwxr-xr-x   0        0        0      632 2024-04-17 03:36:56.186905 vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      945 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0      605 2024-04-17 03:36:48.239062 vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      339 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/status_1.py
--rwxr-xr-x   0        0        0      861 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/jargon.r.HTML
--rwxr-xr-x   0        0        0     2242 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/mass equivalents.r.HTML
--rwxr-xr-x   0        0        0     2428 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__init__.py
--rwxr-xr-x   0        0        0     1576 2024-04-17 03:36:49.227043 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     3068 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1138 2024-04-17 03:36:47.891069 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      845 2024-04-17 03:36:48.003067 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      913 2024-04-17 03:36:47.891069 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_3.cpython-310.pyc
--rwxr-xr-x   0        0        0      645 2024-04-17 03:36:47.839070 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_sci_note_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1425 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/status_1.py
--rwxr-xr-x   0        0        0      898 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/status_2.py
--rwxr-xr-x   0        0        0     1112 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/status_3.py
--rwxr-xr-x   0        0        0      467 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/status_sci_note_1.py
--rwxr-xr-x   0        0        0      168 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/number/fraction_point/fraction_point.s.HTML
--rwxr-xr-x   0        0        0      707 2024-04-17 03:36:47.987067 vegan-2.1.1/venues/stages/vegan/measures/number/integer/__pycache__/status_string_is_integer.cpython-310.pyc
--rwxr-xr-x   0        0        0      525 2024-04-17 03:36:51.071006 vegan-2.1.1/venues/stages/vegan/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc
--rwxr-xr-x   0        0        0      749 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc
--rwxr-xr-x   0        0        0      557 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/integer/status_string_is_integer.py
--rwxr-xr-x   0        0        0      365 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/integer/string_is_integer.py
--rwxr-xr-x   0        0        0      885 2024-04-17 03:36:53.302962 vegan-2.1.1/venues/stages/vegan/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc
--rwxr-xr-x   0        0        0     1702 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc
--rwxr-xr-x   0        0        0      738 2024-04-17 03:36:47.851070 vegan-2.1.1/venues/stages/vegan/measures/number/percentage/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      948 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/percentage/from_fraction.py
--rwxr-xr-x   0        0        0      550 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/percentage/status_1.py
--rwxr-xr-x   0        0        0     2205 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/__init__.py
--rwxr-xr-x   0        0        0     1356 2024-04-17 03:36:50.023027 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2240 2024-04-17 03:36:48.299061 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/_status/__pycache__/status_multiples_of_3_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     3221 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/_status/status_multiples_of_3_1.py
--rwxr-xr-x   0        0        0      612 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/sci_note.S.HTML
--rwxr-xr-x   0        0        0      644 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/sci_note_possibilities.S.HTML
--rwxr-xr-x   0        0        0     1339 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/sci_note_thoughts.S.HTML
--rwxr-xr-x   0        0        0      360 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note_2/__init__.py
--rwxr-xr-x   0        0        0      595 2024-04-17 03:36:49.439038 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1213 2024-04-17 03:36:47.835070 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note_2/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      933 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/measures/number/sci_note_2/status_1.py
--rwxr-xr-x   0        0        0       58 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/temperature/temperature.r.html
--rwxr-xr-x   0        0        0     2202 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/volume/swap/__init__.py
--rwxr-xr-x   0        0        0     1472 2024-04-17 03:36:49.175043 vegan-2.1.1/venues/stages/vegan/measures/volume/swap/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2595 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/volume/swap/__pycache__/__init__.cpython-311.pyc
--rwxr-xr-x   0        0        0     1683 2024-04-17 03:36:48.151064 vegan-2.1.1/venues/stages/vegan/measures/volume/swap/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1663 2024-04-17 03:36:20.927517 vegan-2.1.1/venues/stages/vegan/measures/volume/swap/status_1.py
--rwxr-xr-x   0        0        0      510 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/volume/volume.html
--rwxr-xr-x   0        0        0      911 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/measures/weight/weight.r.html
--rwxr-xr-x   0        0        0     1028 2024-04-17 03:36:50.295021 vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/equalities.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/equalities.cpython-311.pyc
--rwxr-xr-x   0        0        0      460 2024-04-17 03:36:50.651014 vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/equality.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/equality.cpython-311.pyc
--rwxr-xr-x   0        0        0      984 2024-04-17 03:36:55.934910 vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/override_print.cpython-310.pyc
--rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/override_print.cpython-311.pyc
--rwxr-xr-x   0        0        0      579 2024-04-17 03:36:48.039066 vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/status_equalitites_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1088 2024-04-17 03:36:20.919517 vegan-2.1.1/venues/stages/vegan/mixes/insure/equalities.py
--rwxr-xr-x   0        0        0      237 2024-04-17 03:36:20.919517 vegan-2.1.1/venues/stages/vegan/mixes/insure/equality.py
--rwxr-xr-x   0        0        0      781 2024-04-17 03:36:20.923517 vegan-2.1.1/venues/stages/vegan/mixes/insure/override_print.py
--rwxr-xr-x   0        0        0      377 2024-04-17 03:36:20.919517 vegan-2.1.1/venues/stages/vegan/mixes/insure/status_equalitites_1.py
--rwxr-xr-x   0        0        0      577 2024-04-17 17:15:35.007074 vegan-2.1.1/venues/stages/vegan/mixes/procedure/__init__.py
--rwxr-xr-x   0        0        0     1001 2024-04-17 17:16:22.698306 vegan-2.1.1/venues/stages/vegan/mixes/procedure/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1516 2024-04-28 22:58:05.553616 vegan-2.1.1/venues/stages/vegan/readme.md
--rwxr-xr-x   0        0        0     1872 2024-04-27 17:27:23.142884 vegan-2.1.1/venues/stages/vegan/shows_v2/goodness_certifications/certifications.py
--rwxr-xr-x   0        0        0      658 2024-04-17 03:33:22.105283 vegan-2.1.1/venues/stages/vegan/shows_v2/goodness_certifications/vegan.S.HTML
--rw-r--r--   0        0        0     1598 2024-04-26 02:57:44.344040 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/assertions/__pycache__/ingredient.cpython-310.pyc
--rw-r--r--   0        0        0     2787 2024-04-26 02:57:17.872276 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/assertions/ingredient.py
--rw-r--r--   0        0        0     1251 2024-04-27 18:04:01.749135 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/__init__.py
--rw-r--r--   0        0        0      680 2024-04-27 18:04:08.929041 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1489 2024-04-27 17:40:11.683951 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_empty/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1260 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_empty/status_1.py
--rw-r--r--   0        0        0     1781 2024-04-27 17:40:12.227939 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_0.cpython-310.pyc
--rw-r--r--   0        0        0     3633 2024-04-27 17:40:12.183940 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     2757 2024-04-27 17:40:11.855947 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0     1977 2024-04-27 17:40:11.583954 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_3.cpython-310.pyc
--rwxr-xr-x   0        0        0     2369 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_0.py
--rwxr-xr-x   0        0        0     6447 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_1.py
--rwxr-xr-x   0        0        0     3878 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_2.py
--rwxr-xr-x   0        0        0     2366 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_3.py
--rw-r--r--   0        0        0     2747 2024-04-27 17:40:12.331936 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0   200787 2024-04-28 20:56:29.644402 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.JSON
--rwxr-xr-x   0        0        0     2091 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.py
--rw-r--r--   0        0        0     2641 2024-04-27 17:40:11.763949 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0   112672 2024-04-28 20:56:28.140418 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.JSON
--rwxr-xr-x   0        0        0     1915 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.py
--rw-r--r--   0        0        0     2316 2024-04-27 17:40:11.999944 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1889 2024-04-27 17:40:11.979945 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1_supp_1.cpython-310.pyc
--rwxr-xr-x   0        0        0   109562 2024-04-28 20:56:28.332416 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.JSON
--rwxr-xr-x   0        0        0     1809 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.py
--rwxr-xr-x   0        0        0     1410 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1_supp_1.py
--rw-r--r--   0        0        0     2157 2024-04-28 17:41:08.600315 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/__init__.py
--rw-r--r--   0        0        0     1503 2024-04-28 17:45:17.079823 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      666 2024-04-27 18:36:34.414945 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/_status/API_status_1.py
--rw-r--r--   0        0        0      818 2024-04-27 18:36:39.062889 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/_status/__pycache__/API_status_1.cpython-310.pyc
--rw-r--r--   0        0        0     2680 2024-04-26 02:40:26.492343 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/land/_ops/formulate/__init__.py
--rw-r--r--   0        0        0     2140 2024-04-26 02:57:44.348040 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/land/_ops/formulate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      233 2024-04-25 19:30:22.223844 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/recipe.S.HTML
--rw-r--r--   0        0        0     2532 2024-04-28 00:40:14.210697 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/__pycache__/formulate.cpython-310.pyc
--rw-r--r--   0        0        0     1762 2024-04-28 20:36:11.453774 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/__init__.py
--rw-r--r--   0        0        0     1521 2024-04-28 20:36:14.941735 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2919 2024-04-28 20:27:58.831567 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0   214899 2024-04-28 20:56:29.776400 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.JSON
--rw-r--r--   0        0        0     2278 2024-04-28 19:16:12.004516 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.py
--rw-r--r--   0        0        0     2634 2024-04-28 19:17:33.854202 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0    58590 2024-04-28 20:56:29.628402 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.JSON
--rw-r--r--   0        0        0     1929 2024-04-28 19:17:29.690314 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.py
--rw-r--r--   0        0        0     1862 2024-04-28 19:11:33.194920 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/API_status_1.py
--rw-r--r--   0        0        0     1888 2024-04-28 20:28:26.819221 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/API_status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1880 2024-04-28 17:59:07.380196 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0    94101 2024-04-28 20:56:40.680279 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/status_1.JSON
--rw-r--r--   0        0        0     1590 2024-04-28 19:10:15.594738 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/API_status_1.py
--rw-r--r--   0        0        0     1861 2024-04-28 20:28:26.827221 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/API_status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1853 2024-04-28 17:57:44.252665 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0   214851 2024-04-28 20:56:43.624247 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/status_1.JSON
--rw-r--r--   0        0        0     1664 2024-04-28 04:43:21.416236 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     2201 2024-04-28 16:55:02.089934 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/add_goals.cpython-310.pyc
--rw-r--r--   0        0        0      576 2024-04-28 04:35:34.153314 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/find_goal.cpython-310.pyc
--rw-r--r--   0        0        0     4192 2024-04-28 16:54:48.693981 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/add_goals.py
--rw-r--r--   0        0        0      477 2024-04-28 04:35:29.457365 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/find_goal.py
--rw-r--r--   0        0        0     1421 2024-04-28 02:28:19.421723 vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/recipe_with_goals.S.HTML
--rwxr-xr-x   0        0        0      143 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/shows.S.HTML
--rwxr-xr-x   0        0        0      561 2024-04-27 18:25:31.750817 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/_assertions/__init__.py
--rw-r--r--   0        0        0      792 2024-04-27 18:25:53.262563 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/_assertions/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      224 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/FDA.s.HTML
--rwxr-xr-x   0        0        0      421 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/journal.r.HTML
--rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/calcium.r.HTML
--rwxr-xr-x   0        0        0      216 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/lipids/lipids.r.HTML
--rwxr-xr-x   0        0        0       11 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/protein/protein.r.HTML
--rwxr-xr-x   0        0        0     1351 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin a.r.HTML
--rwxr-xr-x   0        0        0      807 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin b.r.HTML
--rwxr-xr-x   0        0        0       93 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin c.r.HTML
--rwxr-xr-x   0        0        0     1298 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin d.r.HTML
--rwxr-xr-x   0        0        0      149 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin e.r.HTML
--rwxr-xr-x   0        0        0      219 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/channel/river.s.HTML
--rwxr-xr-x   0        0        0      543 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/forward channel.s.HTML
--rwxr-xr-x   0        0        0      935 2024-04-17 03:33:22.117283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/structures.s.HTML
--rwxr-xr-x   0        0        0      471 2024-04-17 03:36:50.295021 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      706 2024-04-25 00:16:33.983975 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/__pycache__/develop.cpython-310.pyc
--rw-r--r--   0        0        0     4797 2024-04-25 00:36:39.253965 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__init__.py
--rw-r--r--   0        0        0     2213 2024-04-25 00:37:22.933411 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1197 2024-04-24 23:56:39.560827 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1034 2024-04-24 23:56:09.969137 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/status_1.py
--rw-r--r--   0        0        0     1738 2024-04-24 23:56:39.788825 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1746 2024-04-24 23:56:39.488828 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_2.cpython-310.pyc
--rwxr-xr-x   0        0        0     2137 2024-04-24 23:56:04.641192 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_1.py
--rwxr-xr-x   0        0        0     2114 2024-04-24 23:55:56.809274 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_2.py
--rw-r--r--   0        0        0     2128 2024-04-25 00:03:24.840594 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     3694 2024-04-25 00:03:21.140633 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/status_1.py
--rw-r--r--   0        0        0      441 2024-04-25 01:00:06.752757 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/assertions_one/__init__.py
--rw-r--r--   0        0        0      562 2024-04-25 01:02:38.506933 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/assertions_one/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3264 2024-04-25 00:19:03.893176 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/calculate_portions/__init__.py
--rw-r--r--   0        0        0     1531 2024-04-25 01:02:38.506933 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/calculate_portions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1358 2024-04-25 01:28:21.171397 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/cultivate/__init__.py
--rw-r--r--   0        0        0     1059 2024-04-25 01:31:25.482717 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/cultivate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      796 2024-04-25 00:15:47.948849 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/develop.py
--rw-r--r--   0        0        0     2537 2024-04-25 00:17:17.051140 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__init__.py
--rw-r--r--   0        0        0     1716 2024-04-25 00:37:48.473088 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      697 2024-04-25 00:37:45.949120 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      447 2024-04-25 00:16:53.147600 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/status_1.py
--rwxr-xr-x   0        0        0     1775 2024-04-26 02:19:59.665597 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__init__.py
--rw-r--r--   0        0        0     1404 2024-04-26 02:20:21.177381 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2945 2024-04-17 03:33:22.125283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2090 2024-04-27 17:40:10.779972 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     2227 2024-04-27 17:40:10.791972 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0     1311 2024-04-27 17:40:10.963968 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_loop_1.cpython-310.pyc
--rwxr-xr-x   0        0        0      950 2024-04-17 03:33:22.125283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/multiply_measures.s.HTML
--rwxr-xr-x   0        0        0     2547 2024-04-27 17:39:04.177559 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_1.py
--rwxr-xr-x   0        0        0     2933 2024-04-27 17:39:04.177559 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_2.py
--rwxr-xr-x   0        0        0     1076 2024-04-27 17:39:04.177559 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_loop_1.py
--rwxr-xr-x   0        0        0      279 2024-04-24 21:20:53.222120 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      631 2024-04-25 00:59:04.661504 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/assertions/__init__.py
--rw-r--r--   0        0        0      788 2024-04-25 01:02:38.506933 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/assertions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5604 2024-04-25 01:10:19.889397 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__init__.py
--rw-r--r--   0        0        0     1687 2024-04-25 01:12:56.963514 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1238 2024-04-25 00:37:45.713123 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0     1109 2024-04-25 00:37:34.509265 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/status_1.py
--rw-r--r--   0        0        0      543 2024-04-25 00:28:13.396655 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__init__.py
--rw-r--r--   0        0        0      779 2024-04-25 00:29:32.087569 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      953 2024-04-25 00:29:48.903340 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      752 2024-04-25 00:29:43.999407 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/status_1.py
--rwxr-xr-x   0        0        0     2566 2024-04-28 00:13:52.540684 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__init__.py
--rw-r--r--   0        0        0     2231 2024-04-28 00:14:29.404256 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1017 2024-04-24 22:13:23.957516 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_cautionary.cpython-310.pyc
--rwxr-xr-x   0        0        0     1004 2024-04-24 21:26:22.034066 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_essentials.cpython-310.pyc
--rwxr-xr-x   0        0        0      720 2024-04-24 22:13:18.389563 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/status_cautionary.py
--rwxr-xr-x   0        0        0      700 2024-04-24 21:26:17.758155 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/status_essentials.py
--rwxr-xr-x   0        0        0     1295 2024-04-24 22:45:33.169829 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__init__.py
--rwxr-xr-x   0        0        0     1049 2024-04-24 22:45:47.549673 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1088 2024-04-24 23:20:51.223363 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/status_essentials.cpython-310.pyc
--rwxr-xr-x   0        0        0      685 2024-04-24 22:45:57.489566 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/status_essentials.py
--rwxr-xr-x   0        0        0     1357 2024-04-26 01:45:40.405817 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__init__.py
--rw-r--r--   0        0        0     1216 2024-04-26 01:45:55.765588 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      922 2024-04-24 23:20:51.611359 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_1.cpython-310.pyc
--rw-r--r--   0        0        0      906 2024-04-25 00:00:13.970586 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_2.cpython-310.pyc
--rwxr-xr-x   0        0        0      692 2024-04-24 23:19:39.112127 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_1.py
--rw-r--r--   0        0        0      681 2024-04-25 00:00:10.370624 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_2.py
--rw-r--r--   0        0        0     1021 2024-04-25 00:41:35.278255 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__init__.py
--rw-r--r--   0        0        0     1065 2024-04-25 00:41:39.946197 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1018 2024-04-25 00:37:45.877121 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      843 2024-04-25 00:25:33.730936 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/status_1.py
--rwxr-xr-x   0        0        0     1523 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/grove.S.HTML
--rwxr-xr-x   0        0        0       58 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/info/info.S.HTML
--rwxr-xr-x   0        0        0       73 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/measures/measures.S.HTML
--rwxr-xr-x   0        0        0       59 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/natures/natures.S.HTML
--rwxr-xr-x   0        0        0     1508 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/unites/unites.S.HTML
--rwxr-xr-x   0        0        0     2330 2024-04-23 19:28:57.911458 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/land.S.HTML
--rwxr-xr-x   0        0        0      395 2024-04-26 01:48:09.659641 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/__init__.py
--rw-r--r--   0        0        0      575 2024-04-26 02:00:50.941720 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0      459 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/measures.S.HTML
--rwxr-xr-x   0        0        0     1355 2024-04-26 01:57:53.387927 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__init__.py
--rw-r--r--   0        0        0     1118 2024-04-26 02:02:11.196735 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1601 2024-04-17 03:33:22.125283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      937 2024-04-26 02:02:10.948737 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_1.cpython-310.pyc
--rw-r--r--   0        0        0      935 2024-04-26 02:04:37.130957 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_2.cpython-310.pyc
--rw-r--r--   0        0        0      868 2024-04-26 02:04:37.222956 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_3.cpython-310.pyc
--rwxr-xr-x   0        0        0     1177 2024-04-26 02:02:05.356806 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_1.py
--rwxr-xr-x   0        0        0     1175 2024-04-26 02:02:49.844262 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_2.py
--rwxr-xr-x   0        0        0     1017 2024-04-26 02:03:05.508071 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_3.py
--rwxr-xr-x   0        0        0      765 2024-04-26 02:08:49.075920 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__init__.py
--rw-r--r--   0        0        0      863 2024-04-26 02:08:54.079860 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     1336 2024-04-17 03:33:22.125283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1632 2024-04-27 17:40:11.335960 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/status_1.cpython-310.pyc
--rwxr-xr-x   0        0        0     1685 2024-04-27 17:39:04.181559 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/status_1.py
--rwxr-xr-x   0        0        0      412 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/natures/natures.S.HTML
--rwxr-xr-x   0        0        0      405 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/measured_ingredients/measured_ingredients.S.HTML
--rwxr-xr-x   0        0        0     1066 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/measures/measures.S.HTML
--rwxr-xr-x   0        0        0      611 2024-04-25 19:49:42.003893 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/nature.S.HTML
--rwxr-xr-x   0        0        0      310 2024-04-25 20:29:19.933549 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/unmeasured_ingredients/UI.S.HTML
--rwxr-xr-x   0        0        0      426 2024-04-25 20:36:16.050543 vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/treasure.S.HTML
--rwxr-xr-x   0        0        0       14 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/vegan -- emojis.S.HTML
--rwxr-xr-x   0        0        0     4258 2024-04-28 22:56:51.642449 vegan-2.1.1/venues/stages/vegan/vegan.S.HTML
--rwxr-xr-x   0        0        0      632 2024-04-17 03:33:22.129283 vegan-2.1.1/venues/stages/vegan/vegan.css
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 vegan-2.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      978 2024-04-28 23:00:03.624285 vegan-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      105 2024-04-27 16:44:17.965844 vegan-2.1.2/venue, journal.S.HTML
+-rwxr-xr-x   0        0        0     1606 2024-04-28 19:08:53.538304 vegan-2.1.2/venue.S.HTML
+-rwxr-xr-x   0        0        0      527 2024-04-17 03:36:20.919517 vegan-2.1.2/venues/stages/vegan/___license/license.s.HTML
+-rwxr-xr-x   0        0        0    37279 2024-04-17 03:33:22.077284 vegan-2.1.2/venues/stages/vegan/___license/list/gpl-3.0-standalone.html
+-rw-r--r--   0        0        0      131 2024-04-28 20:54:59.933399 vegan-2.1.2/venues/stages/vegan/___license/list/non-commercial.S.HTML
+-rwxr-xr-x   0        0        0      112 2024-04-17 03:33:22.077284 vegan-2.1.2/venues/stages/vegan/___license/list/vegan.s.HTML
+-rwxr-xr-x   0        0        0      405 2024-04-17 03:33:22.073284 vegan-2.1.2/venues/stages/vegan/___objectives/book/Vitamin B.S.HTML
+-rwxr-xr-x   0        0        0       63 2024-04-17 03:33:22.073284 vegan-2.1.2/venues/stages/vegan/___objectives/book/Vitamin K.S.HTML
+-rw-r--r--   0        0        0      201 2024-04-28 20:53:16.850555 vegan-2.1.2/venues/stages/vegan/___objectives/objectives - elliptic.S.HTML
+-rwxr-xr-x   0        0        0     1274 2024-04-28 20:51:03.764043 vegan-2.1.2/venues/stages/vegan/___objectives/objectives.S.HTML
+-rwxr-xr-x   0        0        0      376 2024-04-17 03:36:20.951516 vegan-2.1.2/venues/stages/vegan/__dictionary/vegan_1
+-rwxr-xr-x   0        0        0      403 2024-04-17 03:36:20.919517 vegan-2.1.2/venues/stages/vegan/__init__.py
+-rwxr-xr-x   0        0        0    93154 2024-04-28 20:56:44.192241 vegan-2.1.2/venues/stages/vegan/__status/API/DB/records.json
+-rwxr-xr-x   0        0        0     2094 2024-04-27 16:55:04.129273 vegan-2.1.2/venues/stages/vegan/__status/API/status.proc.py
+-rwxr-xr-x   0        0        0     1172 2024-04-17 03:33:22.077284 vegan-2.1.2/venues/stages/vegan/__status/__pycache__/status_API.proc.cpython-310.pyc
+-rwxr-xr-x   0        0        0       11 2024-04-23 21:56:29.284154 vegan-2.1.2/venues/stages/vegan/__status/main/.gitignore
+-rwxr-xr-x   0        0        0 13330130 2024-04-28 20:56:31.644379 vegan-2.1.2/venues/stages/vegan/__status/main/DB/records.json
+-rw-r--r--   0        0        0    41183 2024-04-25 01:22:42.760494 vegan-2.1.2/venues/stages/vegan/__status/main/output.json
+-rwxr-xr-x   0        0        0     2106 2024-04-28 00:14:24.216317 vegan-2.1.2/venues/stages/vegan/__status/main/status.proc.py
+-rwxr-xr-x   0        0        0      454 2024-04-17 03:36:21.219514 vegan-2.1.2/venues/stages/vegan/_ellipses--/__init__.py
+-rwxr-xr-x   0        0        0      595 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/_ellipses--/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      891 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/_ellipses--/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1124 2024-04-24 21:00:13.657608 vegan-2.1.2/venues/stages/vegan/_essence/__init__.py
+-rwxr-xr-x   0        0        0      839 2024-04-24 21:00:32.929451 vegan-2.1.2/venues/stages/vegan/_essence/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3705 2024-04-28 19:04:01.618019 vegan-2.1.2/venues/stages/vegan/_essence/build/__init__.py
+-rw-r--r--   0        0        0     2530 2024-04-28 19:04:04.274021 vegan-2.1.2/venues/stages/vegan/_essence/build/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      202 2024-04-27 16:49:31.955662 vegan-2.1.2/venues/stages/vegan/_essence/essence.S.HTML
+-rw-r--r--   0        0        0      475 2024-04-27 21:56:20.995877 vegan-2.1.2/venues/stages/vegan/_essence/run_script/__init__.py
+-rwxr-xr-x   0        0        0      738 2024-04-23 19:31:08.382022 vegan-2.1.2/venues/stages/vegan/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      756 2024-04-23 19:30:52.306199 vegan-2.1.2/venues/stages/vegan/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      544 2024-04-23 19:31:08.382022 vegan-2.1.2/venues/stages/vegan/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0      781 2024-04-23 19:31:08.382022 vegan-2.1.2/venues/stages/vegan/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1623 2024-04-24 00:54:42.885927 vegan-2.1.2/venues/stages/vegan/_ops/clique/__init__.py
+-rwxr-xr-x   0        0        0     1591 2024-04-24 00:54:47.309876 vegan-2.1.2/venues/stages/vegan/_ops/clique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1361 2024-04-24 00:54:47.309876 vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      770 2024-04-23 22:34:43.485503 vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      788 2024-04-23 22:34:42.625514 vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      571 2024-04-23 22:34:43.485503 vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0      807 2024-04-23 22:34:43.485503 vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      662 2024-04-24 00:54:33.574033 vegan-2.1.2/venues/stages/vegan/adventures/_ops/_clique.py
+-rwxr-xr-x   0        0        0      794 2024-04-23 19:52:04.387492 vegan-2.1.2/venues/stages/vegan/adventures/_ops/monitor.py
+-rwxr-xr-x   0        0        0      613 2024-04-23 22:31:52.519576 vegan-2.1.2/venues/stages/vegan/adventures/_ops/off.py
+-rwxr-xr-x   0        0        0      612 2024-04-23 22:31:52.539576 vegan-2.1.2/venues/stages/vegan/adventures/_ops/on.py
+-rwxr-xr-x   0        0        0      426 2024-04-23 22:31:52.551576 vegan-2.1.2/venues/stages/vegan/adventures/_ops/refresh.py
+-rwxr-xr-x   0        0        0      692 2024-04-23 22:31:52.567575 vegan-2.1.2/venues/stages/vegan/adventures/_ops/status.py
+-rwxr-xr-x   0        0        0      342 2024-04-24 01:44:03.440834 vegan-2.1.2/venues/stages/vegan/adventures/adventures.S.HTML
+-rwxr-xr-x   0        0        0      152 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/customs/__init__.py
+-rwxr-xr-x   0        0        0      601 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/customs/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      926 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/customs/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      245 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/customs/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0      345 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/customs/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0      251 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/customs/__pycache__/status.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-27 23:15:29.829818 vegan-2.1.2/venues/stages/vegan/adventures/customs/_ops/off.py
+-rw-r--r--   0        0        0        0 2024-04-27 23:15:26.181863 vegan-2.1.2/venues/stages/vegan/adventures/customs/_ops/on.py
+-rw-r--r--   0        0        0        2 2024-04-27 23:15:34.237762 vegan-2.1.2/venues/stages/vegan/adventures/customs/_ops/status.py
+-rwxr-xr-x   0        0        0      549 2024-04-23 22:31:52.579575 vegan-2.1.2/venues/stages/vegan/adventures/customs/clique.py
+-rw-r--r--   0        0        0      289 2024-04-27 23:17:27.076359 vegan-2.1.2/venues/stages/vegan/adventures/customs/configs_school/embargo.NFT
+-rwxr-xr-x   0        0        0      145 2024-04-27 23:16:20.801181 vegan-2.1.2/venues/stages/vegan/adventures/customs/customs.S.HTML
+-rwxr-xr-x   0        0        0       14 2024-04-24 01:06:32.184393 vegan-2.1.2/venues/stages/vegan/adventures/monetary/.gitignore
+-rwxr-xr-x   0        0        0       17 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/.gitignore
+-rwxr-xr-x   0        0        0      454 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__itinerary/itinerary.S.HTML
+-rwxr-xr-x   0        0        0     1820 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__pycache__/clique.cpython-310.pyc
+-rw-r--r--   0        0        0      748 2024-04-28 01:02:18.999830 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__pycache__/connect.cpython-310.pyc
+-rw-r--r--   0        0        0      783 2024-04-28 01:02:21.999797 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/find_name.cpython-310.pyc
+-rwxr-xr-x   0        0        0        4 2024-04-28 00:13:51.336698 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/insert_document.cpython-310.pyc
+-rw-r--r--   0        0        0      795 2024-04-28 01:02:18.999830 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/retrieve_every.cpython-310.pyc
+-rwxr-xr-x   0        0        0      196 2024-04-24 22:53:29.564774 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/_land.S.HTML
+-rwxr-xr-x   0        0        0      700 2024-04-28 01:02:04.667987 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/find_name.py
+-rwxr-xr-x   0        0        0      924 2024-04-28 01:06:31.349043 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/insert_document.py
+-rwxr-xr-x   0        0        0      601 2024-04-28 01:02:04.735986 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/retrieve_every.py
+-rwxr-xr-x   0        0        0      170 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/cautionary_ingredients/cautionary_ingredients.S.HTML
+-rwxr-xr-x   0        0        0     1019 2024-04-28 01:02:06.219970 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/connect.py
+-rwxr-xr-x   0        0        0      721 2024-04-24 23:09:34.366674 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/essential_nutrients/essential_nutrients.S.HTML
+-rwxr-xr-x   0        0        0      401 2024-04-24 23:06:14.224847 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/glossary/glossary.S.HTML
+-rw-r--r--   0        0        0     1303 2024-04-28 04:32:41.571189 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/find_ingredient.cpython-310.pyc
+-rw-r--r--   0        0        0     1347 2024-04-28 01:13:28.732365 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/insert.cpython-310.pyc
+-rw-r--r--   0        0        0      707 2024-04-28 01:33:42.490573 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/retrieve_one.cpython-310.pyc
+-rw-r--r--   0        0        0      860 2024-04-28 02:43:34.943005 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/__pycache__/create.cpython-310.pyc
+-rw-r--r--   0        0        0      887 2024-04-28 02:46:59.456565 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/__pycache__/drop_and_create.cpython-310.pyc
+-rw-r--r--   0        0        0      624 2024-04-28 02:46:44.020748 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/drop_and_create.py
+-rw-r--r--   0        0        0     1087 2024-04-28 04:32:39.723209 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/find_ingredient.py
+-rw-r--r--   0        0        0      117 2024-04-28 02:07:02.567921 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/goals.S.HTML
+-rw-r--r--   0        0        0     1304 2024-04-28 03:26:22.405607 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/insert.py
+-rw-r--r--   0        0        0      606 2024-04-28 01:33:38.874614 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/retrieve_one.py
+-rwxr-xr-x   0        0        0     1477 2024-04-23 20:40:34.490341 vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/ingredients.S.HTML
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__init__.py
+-rwxr-xr-x   0        0        0      150 2024-04-17 03:36:48.047066 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1687 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      680 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/connect.cpython-310.pyc
+-rwxr-xr-x   0        0        0      857 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1904 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1610 2024-04-23 19:31:08.342022 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0        0 2024-04-28 19:01:53.133950 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/ingredients/cautionary_ingredients/5.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-28 19:01:54.085950 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/ingredients/essential_nutrients/5.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-28 19:01:55.089950 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/ingredients/glossary/5.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/1.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-23 22:05:34.538523 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/2.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-23 22:07:10.673303 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/3.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-27 17:35:00.336394 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/4.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-28 19:02:50.497975 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/5.JSON
+-rwxr-xr-x   0        0        0      118 2024-04-28 19:04:10.818025 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/cautionary_ingredients/6.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/1.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-23 22:05:35.566512 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/2.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-23 22:07:11.713281 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/3.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-27 17:35:01.316362 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/4.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-28 19:02:51.533976 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/5.JSON
+-rwxr-xr-x   0        0        0     5140 2024-04-28 19:04:11.850026 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/6.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-23 22:05:36.562502 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/2.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-23 22:07:12.697261 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/3.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-27 17:35:02.312330 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/4.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-28 19:02:52.497976 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/5.JSON
+-rwxr-xr-x   0        0        0        0 2024-04-28 19:04:12.822027 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/glossary/6.JSON
+-rwxr-xr-x   0        0        0     5771 2024-04-28 19:04:04.554021 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/goals/5.JSON
+-rwxr-xr-x   0        0        0     5771 2024-04-28 19:04:13.826027 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/goals/6.JSON
+-rwxr-xr-x   0        0        0      564 2024-04-27 23:14:58.002218 vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/saves.S.HTML
+-rwxr-xr-x   0        0        0     1434 2024-04-23 20:09:59.888961 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0      868 2024-04-22 01:43:44.052692 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc
+-rw-r--r--   0        0        0     1973 2024-04-28 15:55:33.174259 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1620 2024-04-23 22:34:43.293506 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1079 2024-04-23 20:09:44.305153 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/_clique.py
+-rwxr-xr-x   0        0        0      865 2024-04-22 01:43:41.108724 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/off.py
+-rwxr-xr-x   0        0        0     2428 2024-04-28 15:55:30.526268 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/on.py
+-rw-r--r--   0        0        0     2460 2024-04-28 19:04:04.542021 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2152 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2843 2024-04-28 19:03:52.654013 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/_clique.py
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/dumps/dump.py
+-rwxr-xr-x   0        0        0        2 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/dumps/restore.py
+-rwxr-xr-x   0        0        0        2 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/exports/export.py
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/exports/import.py
+-rwxr-xr-x   0        0        0      390 2024-04-23 20:10:51.728325 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/memories.S.HTML
+-rwxr-xr-x   0        0        0     1764 2024-04-23 22:31:52.611575 vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/status.py
+-rwxr-xr-x   0        0        0      453 2024-04-23 21:03:13.015179 vegan-2.1.2/venues/stages/vegan/adventures/monetary/monetary.S.HTML
+-rwxr-xr-x   0        0        0       46 2024-04-27 23:28:20.716508 vegan-2.1.2/venues/stages/vegan/adventures/monetary/moves/saves/export/__init__.py
+-rwxr-xr-x   0        0        0     1343 2024-04-23 22:34:43.485503 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/off.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1759 2024-04-23 22:34:42.625513 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1288 2024-04-23 22:34:43.489503 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1311 2024-04-23 22:34:42.629513 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0      792 2024-04-24 18:58:20.084451 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/_clique.py
+-rwxr-xr-x   0        0        0      328 2024-04-24 18:58:20.096451 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/off.py
+-rwxr-xr-x   0        0        0      325 2024-04-24 18:58:20.108451 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/on.py
+-rwxr-xr-x   0        0        0      330 2024-04-24 18:58:20.116451 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/refresh.py
+-rwxr-xr-x   0        0        0      339 2024-04-24 18:58:20.116451 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/status.py
+-rwxr-xr-x   0        0        0      130 2024-04-24 18:57:58.564669 vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/redis_mix.S.HTML
+-rwxr-xr-x   0        0        0      188 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/sanique/__init__.py
+-rwxr-xr-x   0        0        0      598 2024-04-17 17:46:30.800270 vegan-2.1.2/venues/stages/vegan/adventures/sanique/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1343 2024-04-23 22:34:43.485503 vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc
+-rw-r--r--   0        0        0     1759 2024-04-25 21:35:38.123051 vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1288 2024-04-23 22:34:43.489503 vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1311 2024-04-23 22:34:42.629514 vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1380 2024-04-23 22:31:52.655574 vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/off.py
+-rwxr-xr-x   0        0        0     1831 2024-04-25 21:31:37.994003 vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/on.py
+-rwxr-xr-x   0        0        0     1164 2024-04-23 22:31:52.683574 vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/refresh.py
+-rwxr-xr-x   0        0        0     1229 2024-04-23 22:31:52.699574 vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/status.py
+-rwxr-xr-x   0        0        0      781 2024-04-23 22:31:52.711573 vegan-2.1.2/venues/stages/vegan/adventures/sanique/clique.py
+-rwxr-xr-x   0        0        0     6337 2024-04-28 20:50:26.408443 vegan-2.1.2/venues/stages/vegan/adventures/sanique/harbor/__init__.py
+-rw-r--r--   0        0        0     5040 2024-04-28 20:50:30.200402 vegan-2.1.2/venues/stages/vegan/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      524 2024-04-17 03:36:20.947517 vegan-2.1.2/venues/stages/vegan/adventures/sanique/sanique.S.HTML
+-rwxr-xr-x   0        0        0      388 2024-04-17 03:36:47.855070 vegan-2.1.2/venues/stages/vegan/adventures/sanique/utilities/__pycache__/has_sanic_check.cpython-310.pyc
+-rwxr-xr-x   0        0        0      167 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/adventures/sanique/utilities/has_sanic_check.py
+-rwxr-xr-x   0        0        0      151 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/affiliates_Amazon/affiliates.s.HTML
+-rwxr-xr-x   0        0        0      176 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/besties.S.HTML
+-rwxr-xr-x   0        0        0      596 2024-04-17 03:36:49.119045 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/__pycache__/source.cpython-310.pyc
+-rwxr-xr-x   0        0        0      738 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/__pycache__/source.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1255 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/__init__.py
+-rw-r--r--   0        0        0     1552 2024-04-27 17:40:11.463956 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2127 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      776 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc
+-rwxr-xr-x   0        0        0      450 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/FOUNDATIONAL.cpython-311.pyc
+-rw-r--r--   0        0        0      646 2024-04-27 17:40:11.499956 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc
+-rwxr-xr-x   0        0        0      778 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc
+-rw-r--r--   0        0        0      496 2024-04-27 17:40:11.499956 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-310.pyc
+-rwxr-xr-x   0        0        0      677 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc
+-rwxr-xr-x   0        0        0      508 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/branded.py
+-rwxr-xr-x   0        0        0      262 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/foundational.py
+-rwxr-xr-x   0        0        0      466 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/status/API_status_branded_1.py
+-rwxr-xr-x   0        0        0      533 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/status/API_status_foundational_1.py
+-rw-r--r--   0        0        0      739 2024-04-27 17:40:30.387524 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/status/__pycache__/API_status_branded_1.cpython-310.pyc
+-rw-r--r--   0        0        0      734 2024-04-27 17:40:30.383524 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/status/__pycache__/API_status_foundational_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      370 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/source.py
+-rwxr-xr-x   0        0        0      939 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/__init__.py
+-rw-r--r--   0        0        0     1125 2024-04-27 17:40:11.499956 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2082 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      740 2024-04-27 17:40:12.739927 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0    37079 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON
+-rwxr-xr-x   0        0        0    37079 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON
+-rwxr-xr-x   0        0        0     7242 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/beet_juice_2412474.JSON
+-rwxr-xr-x   0        0        0     8522 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/beet_juice_2642759.JSON
+-rwxr-xr-x   0        0        0    33964 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/impossible_beef_2664238.JSON
+-rwxr-xr-x   0        0        0    17926 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/problems/impossible_2468423.JSON
+-rwxr-xr-x   0        0        0      104 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/problems/problems.r.HTML
+-rwxr-xr-x   0        0        0    10678 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/vegan_pizza_2672996.JSON
+-rwxr-xr-x   0        0        0    10670 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/walnuts_1882785.JSON
+-rwxr-xr-x   0        0        0   189146 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON
+-rwxr-xr-x   0        0        0      255 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/mergers.r.HTML
+-rwxr-xr-x   0        0        0       88 2024-04-17 03:33:22.097283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/priorities.r.HTML
+-rwxr-xr-x   0        0        0      454 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/status_1.py
+-rwxr-xr-x   0        0        0     1210 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/food.s.HTML
+-rwxr-xr-x   0        0        0     4580 2024-04-27 18:21:30.033645 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/__init__.py
+-rw-r--r--   0        0        0     2455 2024-04-27 18:24:41.143411 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1748 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__init__.py
+-rw-r--r--   0        0        0     1194 2024-04-27 17:40:11.551954 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2050 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      571 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1065 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-311.pyc
+-rw-r--r--   0        0        0     1339 2024-04-27 17:40:12.659929 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      599 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__init__.py
+-rwxr-xr-x   0        0        0      596 2024-04-17 03:36:50.207023 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4071 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__init__.py
+-rw-r--r--   0        0        0     2918 2024-04-27 17:40:11.551954 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     5397 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1247 2024-04-27 17:40:12.671929 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_mass_1.cpython-310.pyc
+-rw-r--r--   0        0        0      983 2024-04-27 17:40:12.975921 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_volume_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      421 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__init__.py
+-rwxr-xr-x   0        0        0      563 2024-04-17 03:36:50.203023 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      946 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1243 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_mass_1.py
+-rwxr-xr-x   0        0        0      891 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_volume_1.py
+-rwxr-xr-x   0        0        0     1392 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/status_1.py
+-rw-r--r--   0        0        0      614 2024-04-28 20:33:03.399922 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/API_status_found_1.py
+-rw-r--r--   0        0        0      587 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/API_status_not_found_1.py
+-rw-r--r--   0        0        0     1768 2024-04-27 18:21:13.609835 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-27 17:18:55.070676 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      836 2024-04-28 20:33:06.991881 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_found_1.cpython-310.pyc
+-rw-r--r--   0        0        0      757 2024-04-27 17:40:30.383524 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_not_found_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1784 2024-04-27 18:24:41.239410 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1414 2024-04-27 17:40:12.831925 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_1_description.cpython-310.pyc
+-rw-r--r--   0        0        0     1823 2024-04-27 17:40:12.991921 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_2_measures.cpython-310.pyc
+-rw-r--r--   0        0        0     1536 2024-04-27 17:40:12.659929 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc
+-rw-r--r--   0        0        0     1594 2024-04-25 01:35:26.781309 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_4_land_essentials.cpython-310.pyc
+-rw-r--r--   0        0        0     1685 2024-04-27 17:40:13.295914 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_4_lands.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1158 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_1_description.py
+-rwxr-xr-x   0        0        0     1866 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_2_measures.py
+-rwxr-xr-x   0        0        0     2071 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_3_measured_ingredients.py
+-rwxr-xr-x   0        0        0     1489 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_4_lands.py
+-rw-r--r--   0        0        0     2071 2024-04-27 17:40:12.231939 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1586 2024-04-27 17:40:12.667929 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0     1098 2024-04-27 17:40:12.559931 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2412474.cpython-310.pyc
+-rw-r--r--   0        0        0     1437 2024-04-27 17:40:12.411935 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_3.cpython-310.pyc
+-rw-r--r--   0        0        0     1201 2024-04-27 17:40:12.471933 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_loop_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2765 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_1.py
+-rwxr-xr-x   0        0        0     1617 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_2.py
+-rwxr-xr-x   0        0        0      708 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_2412474.py
+-rwxr-xr-x   0        0        0     1080 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_3.py
+-rwxr-xr-x   0        0        0      844 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_loop_1.py
+-rwxr-xr-x   0        0        0     2276 2024-04-28 01:02:04.787985 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/land/__init__.py
+-rw-r--r--   0        0        0     2093 2024-04-28 01:02:21.911798 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/land/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      466 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__init__.py
+-rwxr-xr-x   0        0        0      568 2024-04-17 03:36:50.287021 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      957 2024-04-17 03:33:22.101283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1166 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__init__.py
+-rw-r--r--   0        0        0      833 2024-04-27 17:40:12.419934 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1012 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      703 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__init__.py
+-rw-r--r--   0        0        0      827 2024-04-27 17:40:12.419934 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1272 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1360 2024-04-27 17:40:12.507932 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1062 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/status_1.py
+-rw-r--r--   0        0        0     1979 2024-04-27 17:40:12.447934 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_mass_1.cpython-310.pyc
+-rw-r--r--   0        0        0      999 2024-04-27 17:40:12.715928 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_volume_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2079 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/status_mass_1.py
+-rwxr-xr-x   0        0        0      716 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/status_volume_1.py
+-rwxr-xr-x   0        0        0     1143 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured ingredients.S.HTML
+-rwxr-xr-x   0        0        0     1421 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__init__.py
+-rw-r--r--   0        0        0     1109 2024-04-27 17:40:12.387935 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1591 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1606 2024-04-27 17:40:12.795926 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_IU_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1505 2024-04-27 17:40:12.291937 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_energy_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1603 2024-04-27 17:40:12.955922 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_mass_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1705 2024-04-27 17:39:04.185559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_IU_1.py
+-rwxr-xr-x   0        0        0     1904 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_energy_1.py
+-rwxr-xr-x   0        0        0     1608 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_mass_1.py
+-rwxr-xr-x   0        0        0     1724 2024-04-17 03:36:21.175514 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__init__.py
+-rwxr-xr-x   0        0        0     1435 2024-04-17 03:36:50.287021 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3142 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1232 2024-04-17 03:36:21.147514 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__init__.py
+-rwxr-xr-x   0        0        0     1246 2024-04-17 03:36:50.291021 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1831 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1489 2024-04-17 03:36:21.175514 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__init__.py
+-rwxr-xr-x   0        0        0     1198 2024-04-17 03:36:50.291021 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1791 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1379 2024-04-17 03:36:21.175514 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__init__.py
+-rwxr-xr-x   0        0        0     1335 2024-04-17 03:36:50.291021 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1842 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      706 2024-04-17 03:36:50.291021 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1040 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1899 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc
+-rwxr-xr-x   0        0        0      651 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc
+-rwxr-xr-x   0        0        0      845 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc
+-rwxr-xr-x   0        0        0      849 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc
+-rwxr-xr-x   0        0        0      636 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/food_nutrient.py
+-rwxr-xr-x   0        0        0      483 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/label_nutrient.py
+-rwxr-xr-x   0        0        0      503 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient.r.HTML
+-rwxr-xr-x   0        0        0      706 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient_prototype_1.r.HTML
+-rwxr-xr-x   0        0        0     3859 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__init__.py
+-rw-r--r--   0        0        0     2386 2024-04-27 17:40:12.343936 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4016 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1360 2024-04-27 17:40:12.655929 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/status_mass_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1391 2024-04-27 17:40:13.079919 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/status_volume_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      110 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/form.S.HTML
+-rwxr-xr-x   0        0        0     1232 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/status_mass_1.py
+-rwxr-xr-x   0        0        0     1175 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/status_volume_1.py
+-rwxr-xr-x   0        0        0      306 2024-04-27 17:39:04.189559 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/nature_v2.S.HTML
+-rwxr-xr-x   0        0        0      102 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/unmeasured_ingredients/__init__.py
+-rwxr-xr-x   0        0        0      338 2024-04-17 03:36:50.291021 vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/unmeasured_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1042 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/NIH.s.HTML
+-rw-r--r--   0        0        0      536 2024-04-27 16:55:09.193236 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc
+-rwxr-xr-x   0        0        0      670 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1131 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__init__.py
+-rw-r--r--   0        0        0     1131 2024-04-27 17:40:30.767515 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1889 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      815 2024-04-27 16:55:09.193236 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1399 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1087 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/assertions.py
+-rwxr-xr-x   0        0        0      434 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/status/API_status_1.py
+-rw-r--r--   0        0        0      698 2024-04-27 17:40:30.387524 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/status/__pycache__/API_status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      316 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/source.py
+-rwxr-xr-x   0        0        0      844 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/__init__.py
+-rw-r--r--   0        0        0     1038 2024-04-27 17:40:15.195870 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1918 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0    44597 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/coated tablets/multivitamin_276336.JSON
+-rwxr-xr-x   0        0        0    22180 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/other/chia_seeds_214893.JSON
+-rwxr-xr-x   0        0        0     6430 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/powder/mane_270619.JSON
+-rwxr-xr-x   0        0        0    72594 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/powder/nutritional_shake_220884.JSON
+-rwxr-xr-x   0        0        0    57378 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/powder packets/multivitamin_246811.JSON
+-rwxr-xr-x   0        0        0    22710 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/tablets/calcium_261967.JSON
+-rwxr-xr-x   0        0        0    43725 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/tablets/multivitamin_249664.JSON
+-rwxr-xr-x   0        0        0     7107 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON
+-rw-r--r--   0        0        0     4047 2024-04-27 18:25:39.806722 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/__init__.py
+-rw-r--r--   0        0        0     2752 2024-04-27 18:25:55.126541 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      271 2024-04-17 03:36:50.963008 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      383 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1147 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__init__.py
+-rw-r--r--   0        0        0      906 2024-04-27 17:40:15.039874 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1201 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1229 2024-04-27 17:40:13.511909 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/status_powder_packets_246811.cpython-310.pyc
+-rwxr-xr-x   0        0        0      931 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/status_powder_packets_246811.py
+-rwxr-xr-x   0        0        0       56 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/servingSizeUnit/__init__.py
+-rw-r--r--   0        0        0     1917 2024-04-27 17:48:43.182166 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_ops/retrieve/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-27 17:48:48.074086 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1410 2024-04-27 17:40:14.187894 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_1_info.cpython-310.pyc
+-rw-r--r--   0        0        0     1418 2024-04-27 17:40:14.083896 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_2_form.cpython-310.pyc
+-rw-r--r--   0        0        0     1827 2024-04-27 17:40:13.859901 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc
+-rw-r--r--   0        0        0     1236 2024-04-25 18:59:21.733410 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_essential_nutrients.cpython-310.pyc
+-rw-r--r--   0        0        0     1474 2024-04-27 17:40:13.847901 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_unmeasured_ingredients.cpython-310.pyc
+-rw-r--r--   0        0        0     1661 2024-04-27 17:40:14.131895 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_5_essential_nutrients.cpython-310.pyc
+-rw-r--r--   0        0        0     1589 2024-04-27 17:40:13.907900 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_6_cautionary_ingredients.cpython-310.pyc
+-rw-r--r--   0        0        0    28721 2024-04-28 20:56:28.872410 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/mane_270619_nature.JSON
+-rw-r--r--   0        0        0   124533 2024-04-28 20:56:29.068408 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/multivitamin_249664.JSON
+-rw-r--r--   0        0        0     1036 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_1_info.py
+-rw-r--r--   0        0        0     1046 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_2_form.py
+-rw-r--r--   0        0        0     1614 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_3_measured_ingredients.py
+-rw-r--r--   0        0        0     1065 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_4_unmeasured_ingredients.py
+-rw-r--r--   0        0        0     1271 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_5_essential_nutrients.py
+-rw-r--r--   0        0        0     1164 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_6_cautionary_ingredients.py
+-rw-r--r--   0        0        0      828 2024-04-27 17:40:12.847925 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/_loop/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      736 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/_loop/status_1.py
+-rw-r--r--   0        0        0     1741 2024-04-27 17:40:13.223916 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/__pycache__/status_multivitamin_276336.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1557 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336.py
+-rwxr-xr-x   0        0        0   136805 2024-04-28 20:56:29.368405 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336_nature.JSON
+-rw-r--r--   0        0        0     1209 2024-04-27 17:40:13.147918 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/__pycache__/status_chia_seeds_214893.cpython-310.pyc
+-rwxr-xr-x   0        0        0    82230 2024-04-28 20:56:28.848410 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/chia_seeds_214893_nature.JSON
+-rwxr-xr-x   0        0        0      763 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/status_chia_seeds_214893.py
+-rw-r--r--   0        0        0     1172 2024-04-27 17:40:12.731927 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/__pycache__/status_mane_270619.cpython-310.pyc
+-rwxr-xr-x   0        0        0    28721 2024-04-28 20:56:25.788444 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/mane_270619_nature.JSON
+-rwxr-xr-x   0        0        0      736 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/status_mane_270619.py
+-rw-r--r--   0        0        0      568 2024-04-25 04:11:27.433921 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      672 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      665 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__init__.py
+-rw-r--r--   0        0        0      860 2024-04-27 17:40:15.039874 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1333 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      767 2024-04-27 17:40:13.195917 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/status_other_214893.cpython-310.pyc
+-rwxr-xr-x   0        0        0      512 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/status_other_214893.py
+-rwxr-xr-x   0        0        0      512 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/form.S.HTML
+-rwxr-xr-x   0        0        0     3783 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__init__.py
+-rw-r--r--   0        0        0     2355 2024-04-27 17:40:15.043874 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      179 2024-04-17 03:36:51.818991 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1571 2024-04-27 17:40:13.811902 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_246811.cpython-310.pyc
+-rw-r--r--   0        0        0     1546 2024-04-27 17:40:13.511909 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_276336.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1781 2024-04-27 17:39:04.201558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/status_246811.py
+-rwxr-xr-x   0        0        0     1666 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/status_276336.py
+-rwxr-xr-x   0        0        0     3221 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__init__.py
+-rw-r--r--   0        0        0     2669 2024-04-27 17:40:14.991875 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1195 2024-04-27 17:40:13.007921 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_coated_tablet_276336.cpython-310.pyc
+-rw-r--r--   0        0        0      998 2024-04-27 17:40:13.175917 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_gram_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1004 2024-04-27 17:40:13.075919 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_220884.cpython-310.pyc
+-rw-r--r--   0        0        0     1037 2024-04-27 17:40:12.371935 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_270619.cpython-310.pyc
+-rw-r--r--   0        0        0     1418 2024-04-27 17:40:13.091919 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_packets_246811.cpython-310.pyc
+-rw-r--r--   0        0        0      947 2024-04-27 17:40:13.891900 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_tablet_261967.cpython-310.pyc
+-rw-r--r--   0        0        0      981 2024-04-27 17:40:13.787903 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_vegan_capsule_248267.cpython-310.pyc
+-rwxr-xr-x   0        0        0      929 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_coated_tablet_276336.py
+-rwxr-xr-x   0        0        0      816 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_gram_1.py
+-rwxr-xr-x   0        0        0      820 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_220884.py
+-rwxr-xr-x   0        0        0      893 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_270619.py
+-rwxr-xr-x   0        0        0     1333 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_packets_246811.py
+-rwxr-xr-x   0        0        0      703 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_tablet_261967.py
+-rwxr-xr-x   0        0        0      727 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_vegan_capsule_248267.py
+-rw-r--r--   0        0        0     1881 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/land/__init__.py
+-rw-r--r--   0        0        0     1983 2024-04-27 17:40:15.187871 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/land/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1613 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__init__.py
+-rw-r--r--   0        0        0     1857 2024-04-27 17:40:15.043874 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2911 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1119 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__init__.py
+-rw-r--r--   0        0        0     1079 2024-04-27 17:40:15.187871 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1442 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      961 2024-04-27 17:40:13.363913 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      664 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/status_1.py
+-rwxr-xr-x   0        0        0      587 2024-04-27 17:39:04.193559 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__init__.py
+-rw-r--r--   0        0        0      990 2024-04-27 17:40:18.015806 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1171 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1074 2024-04-27 17:40:13.119918 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_status/__pycache__/status_chia_seeds_214893.cpython-310.pyc
+-rwxr-xr-x   0        0        0      801 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_status/status_chia_seeds_214893.py
+-rwxr-xr-x   0        0        0     4661 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__init__.py
+-rw-r--r--   0        0        0     2795 2024-04-27 17:40:15.043874 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4500 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1630 2024-04-27 17:40:13.151918 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1729 2024-04-27 17:39:04.197558 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/status_1.py
+-rwxr-xr-x   0        0        0     1514 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/measured_ingredient.S.HTML
+-rwxr-xr-x   0        0        0      561 2024-04-17 03:33:22.109283 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredients.S.HTML
+-rw-r--r--   0        0        0        3 2024-04-25 01:50:49.197454 vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/natures_v2.S.HTML
+-rw-r--r--   0        0        0       87 2024-04-27 20:03:02.828977 vegan-2.1.2/venues/stages/vegan/goals/goals.S.HTML
+-rw-r--r--   0        0        0     8904 2024-04-28 01:16:44.610153 vegan-2.1.2/venues/stages/vegan/goals/umuntu/FDA.py
+-rw-r--r--   0        0        0     9794 2024-03-09 19:44:16.627477 vegan-2.1.2/venues/stages/vegan/goals/umuntu/FDA_v1.py
+-rw-r--r--   0        0        0     4193 2024-03-10 18:32:48.701726 vegan-2.1.2/venues/stages/vegan/goals/umuntu/FDA_v2.py
+-rw-r--r--   0        0        0     7523 2024-03-12 19:40:02.502146 vegan-2.1.2/venues/stages/vegan/goals/umuntu/FDA_v3.py
+-rw-r--r--   0        0        0     4337 2024-04-28 01:16:47.442121 vegan-2.1.2/venues/stages/vegan/goals/umuntu/__pycache__/FDA.cpython-310.pyc
+-rw-r--r--   0        0        0     3847 2024-03-14 19:34:32.350499 vegan-2.1.2/venues/stages/vegan/goals/umuntu/__pycache__/FDA_v3.cpython-310.pyc
+-rw-r--r--   0        0        0       71 2024-04-27 16:41:36.022921 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Carbohydrates.s.HTML
+-rw-r--r--   0        0        0       61 2024-04-27 16:41:31.750949 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Fat.s.HTML
+-rw-r--r--   0        0        0       64 2024-04-27 16:41:27.998973 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Lipids.s.HTML
+-rw-r--r--   0        0        0      145 2024-04-27 16:41:20.183024 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Protein.s.HTML
+-rw-r--r--   0        0        0       16 2024-01-31 21:52:02.234756 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Vitamin A.s.HTML
+-rw-r--r--   0        0        0        0 2024-01-31 21:52:25.962491 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Vitamin B.s.HTML
+-rw-r--r--   0        0        0       68 2024-04-27 16:40:48.275230 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Vitamin C.s.HTML
+-rw-r--r--   0        0        0       65 2024-04-27 16:40:44.111256 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Vitamin D.s.HTML
+-rw-r--r--   0        0        0      423 2024-04-27 16:42:29.518570 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_journal/Vitamin E.s.HTML
+-rw-r--r--   0        0        0      553 2024-04-28 02:16:08.201921 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_ops/__pycache__/retrieve.cpython-310.pyc
+-rw-r--r--   0        0        0      352 2024-04-28 01:52:53.553431 vegan-2.1.2/venues/stages/vegan/goals/umuntu/_ops/retrieve.py
+-rw-r--r--   0        0        0        3 2024-03-10 18:23:03.506534 vegan-2.1.2/venues/stages/vegan/goals/umuntu/parse_FDA.proc.py
+-rw-r--r--   0        0        0      488 2024-04-28 00:30:07.297621 vegan-2.1.2/venues/stages/vegan/goals/umuntu/umuntu.S.HTML
+-rwxr-xr-x   0        0        0      799 2024-04-17 03:36:48.015066 vegan-2.1.2/venues/stages/vegan/measures/_interpret/__pycache__/status_unit_kind.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1469 2024-04-17 03:36:50.287021 vegan-2.1.2/venues/stages/vegan/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2547 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc
+-rwxr-xr-x   0        0        0       61 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/_interpret/interpret.S.HTML
+-rwxr-xr-x   0        0        0      667 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/_interpret/status_unit_kind.py
+-rwxr-xr-x   0        0        0     1675 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/_interpret/unit_kind.py
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/biological_activity/__init__.py
+-rwxr-xr-x   0        0        0       59 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/electric_current/electric_current.S.HTML
+-rwxr-xr-x   0        0        0     1142 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/energy/energy.r.HTML
+-rwxr-xr-x   0        0        0     1171 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/energy/swap/__init__.py
+-rwxr-xr-x   0        0        0     1016 2024-04-17 03:36:50.291021 vegan-2.1.2/venues/stages/vegan/measures/energy/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1761 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/energy/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      618 2024-04-17 03:36:48.423058 vegan-2.1.2/venues/stages/vegan/measures/energy/swap/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      383 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/energy/swap/status_1.py
+-rwxr-xr-x   0        0        0       71 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/length/length.r.HTML
+-rwxr-xr-x   0        0        0       95 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/mass/e_note.py
+-rwxr-xr-x   0        0        0       12 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/mass/mass.r.html
+-rwxr-xr-x   0        0        0     2326 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/mass/swap/__init__.py
+-rwxr-xr-x   0        0        0     1724 2024-04-17 03:36:49.175043 vegan-2.1.2/venues/stages/vegan/measures/mass/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3229 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/mass/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1141 2024-04-17 03:36:47.971067 vegan-2.1.2/venues/stages/vegan/measures/mass/swap/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1150 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/mass/swap/status_1.py
+-rwxr-xr-x   0        0        0     2419 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/mass/system international.r.html
+-rwxr-xr-x   0        0        0      768 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/mass/us customary.r.html
+-rwxr-xr-x   0        0        0      520 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__init__.py
+-rwxr-xr-x   0        0        0      632 2024-04-17 03:36:56.186905 vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      945 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0      605 2024-04-17 03:36:48.239062 vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      339 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/status_1.py
+-rwxr-xr-x   0        0        0      861 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/jargon.r.HTML
+-rwxr-xr-x   0        0        0     2242 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/mass equivalents.r.HTML
+-rwxr-xr-x   0        0        0     2428 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__init__.py
+-rwxr-xr-x   0        0        0     1576 2024-04-17 03:36:49.227043 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3068 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1138 2024-04-17 03:36:47.891069 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      845 2024-04-17 03:36:48.003067 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      913 2024-04-17 03:36:47.891069 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0      645 2024-04-17 03:36:47.839070 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_sci_note_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1425 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/status_1.py
+-rwxr-xr-x   0        0        0      898 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/status_2.py
+-rwxr-xr-x   0        0        0     1112 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/status_3.py
+-rwxr-xr-x   0        0        0      467 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/status_sci_note_1.py
+-rwxr-xr-x   0        0        0      168 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/number/fraction_point/fraction_point.s.HTML
+-rwxr-xr-x   0        0        0      707 2024-04-17 03:36:47.987067 vegan-2.1.2/venues/stages/vegan/measures/number/integer/__pycache__/status_string_is_integer.cpython-310.pyc
+-rwxr-xr-x   0        0        0      525 2024-04-17 03:36:51.071006 vegan-2.1.2/venues/stages/vegan/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc
+-rwxr-xr-x   0        0        0      749 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc
+-rwxr-xr-x   0        0        0      557 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/integer/status_string_is_integer.py
+-rwxr-xr-x   0        0        0      365 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/integer/string_is_integer.py
+-rwxr-xr-x   0        0        0      885 2024-04-17 03:36:53.302962 vegan-2.1.2/venues/stages/vegan/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1702 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc
+-rwxr-xr-x   0        0        0      738 2024-04-17 03:36:47.851070 vegan-2.1.2/venues/stages/vegan/measures/number/percentage/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      948 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/percentage/from_fraction.py
+-rwxr-xr-x   0        0        0      550 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/percentage/status_1.py
+-rwxr-xr-x   0        0        0     2205 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/__init__.py
+-rwxr-xr-x   0        0        0     1356 2024-04-17 03:36:50.023027 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2240 2024-04-17 03:36:48.299061 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/_status/__pycache__/status_multiples_of_3_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3221 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/_status/status_multiples_of_3_1.py
+-rwxr-xr-x   0        0        0      612 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/sci_note.S.HTML
+-rwxr-xr-x   0        0        0      644 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/sci_note_possibilities.S.HTML
+-rwxr-xr-x   0        0        0     1339 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/sci_note_thoughts.S.HTML
+-rwxr-xr-x   0        0        0      360 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note_2/__init__.py
+-rwxr-xr-x   0        0        0      595 2024-04-17 03:36:49.439038 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1213 2024-04-17 03:36:47.835070 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note_2/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      933 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/measures/number/sci_note_2/status_1.py
+-rwxr-xr-x   0        0        0       58 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/temperature/temperature.r.html
+-rwxr-xr-x   0        0        0     2202 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/volume/swap/__init__.py
+-rwxr-xr-x   0        0        0     1472 2024-04-17 03:36:49.175043 vegan-2.1.2/venues/stages/vegan/measures/volume/swap/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2595 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/volume/swap/__pycache__/__init__.cpython-311.pyc
+-rwxr-xr-x   0        0        0     1683 2024-04-17 03:36:48.151064 vegan-2.1.2/venues/stages/vegan/measures/volume/swap/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1663 2024-04-17 03:36:20.927517 vegan-2.1.2/venues/stages/vegan/measures/volume/swap/status_1.py
+-rwxr-xr-x   0        0        0      510 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/volume/volume.html
+-rwxr-xr-x   0        0        0      911 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/measures/weight/weight.r.html
+-rwxr-xr-x   0        0        0     1028 2024-04-17 03:36:50.295021 vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/equalities.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/equalities.cpython-311.pyc
+-rwxr-xr-x   0        0        0      460 2024-04-17 03:36:50.651014 vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/equality.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/equality.cpython-311.pyc
+-rwxr-xr-x   0        0        0      984 2024-04-17 03:36:55.934910 vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/override_print.cpython-310.pyc
+-rwxr-xr-x   0        0        0        5 2024-04-17 03:33:22.113283 vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/override_print.cpython-311.pyc
+-rwxr-xr-x   0        0        0      579 2024-04-17 03:36:48.039066 vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/status_equalitites_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1088 2024-04-17 03:36:20.919517 vegan-2.1.2/venues/stages/vegan/mixes/insure/equalities.py
+-rwxr-xr-x   0        0        0      237 2024-04-17 03:36:20.919517 vegan-2.1.2/venues/stages/vegan/mixes/insure/equality.py
+-rwxr-xr-x   0        0        0      781 2024-04-17 03:36:20.923517 vegan-2.1.2/venues/stages/vegan/mixes/insure/override_print.py
+-rwxr-xr-x   0        0        0      377 2024-04-17 03:36:20.919517 vegan-2.1.2/venues/stages/vegan/mixes/insure/status_equalitites_1.py
+-rwxr-xr-x   0        0        0      577 2024-04-17 17:15:35.007074 vegan-2.1.2/venues/stages/vegan/mixes/procedure/__init__.py
+-rwxr-xr-x   0        0        0     1001 2024-04-17 17:16:22.698306 vegan-2.1.2/venues/stages/vegan/mixes/procedure/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1295 2024-04-28 22:59:58.612342 vegan-2.1.2/venues/stages/vegan/readme.md
+-rwxr-xr-x   0        0        0     1872 2024-04-27 17:27:23.142884 vegan-2.1.2/venues/stages/vegan/shows_v2/goodness_certifications/certifications.py
+-rwxr-xr-x   0        0        0      658 2024-04-17 03:33:22.105283 vegan-2.1.2/venues/stages/vegan/shows_v2/goodness_certifications/vegan.S.HTML
+-rw-r--r--   0        0        0     1598 2024-04-26 02:57:44.344040 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/assertions/__pycache__/ingredient.cpython-310.pyc
+-rw-r--r--   0        0        0     2787 2024-04-26 02:57:17.872276 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/assertions/ingredient.py
+-rw-r--r--   0        0        0     1251 2024-04-27 18:04:01.749135 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/__init__.py
+-rw-r--r--   0        0        0      680 2024-04-27 18:04:08.929041 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1489 2024-04-27 17:40:11.683951 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_empty/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1260 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_empty/status_1.py
+-rw-r--r--   0        0        0     1781 2024-04-27 17:40:12.227939 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_0.cpython-310.pyc
+-rw-r--r--   0        0        0     3633 2024-04-27 17:40:12.183940 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     2757 2024-04-27 17:40:11.855947 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0     1977 2024-04-27 17:40:11.583954 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2369 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_0.py
+-rwxr-xr-x   0        0        0     6447 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_1.py
+-rwxr-xr-x   0        0        0     3878 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_2.py
+-rwxr-xr-x   0        0        0     2366 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_3.py
+-rw-r--r--   0        0        0     2747 2024-04-27 17:40:12.331936 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0   200787 2024-04-28 20:56:29.644402 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.JSON
+-rwxr-xr-x   0        0        0     2091 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.py
+-rw-r--r--   0        0        0     2641 2024-04-27 17:40:11.763949 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0   112672 2024-04-28 20:56:28.140418 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.JSON
+-rwxr-xr-x   0        0        0     1915 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.py
+-rw-r--r--   0        0        0     2316 2024-04-27 17:40:11.999944 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1889 2024-04-27 17:40:11.979945 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1_supp_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0   109562 2024-04-28 20:56:28.332416 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.JSON
+-rwxr-xr-x   0        0        0     1809 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.py
+-rwxr-xr-x   0        0        0     1410 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1_supp_1.py
+-rw-r--r--   0        0        0     2157 2024-04-28 17:41:08.600315 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/__init__.py
+-rw-r--r--   0        0        0     1503 2024-04-28 17:45:17.079823 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      666 2024-04-27 18:36:34.414945 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/_status/API_status_1.py
+-rw-r--r--   0        0        0      818 2024-04-27 18:36:39.062889 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/_status/__pycache__/API_status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     2680 2024-04-26 02:40:26.492343 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/land/_ops/formulate/__init__.py
+-rw-r--r--   0        0        0     2140 2024-04-26 02:57:44.348040 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/land/_ops/formulate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      233 2024-04-25 19:30:22.223844 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/recipe.S.HTML
+-rw-r--r--   0        0        0     2532 2024-04-28 00:40:14.210697 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/__pycache__/formulate.cpython-310.pyc
+-rw-r--r--   0        0        0     1762 2024-04-28 20:36:11.453774 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/__init__.py
+-rw-r--r--   0        0        0     1521 2024-04-28 20:36:14.941735 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2919 2024-04-28 20:27:58.831567 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0   214899 2024-04-28 20:56:29.776400 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.JSON
+-rw-r--r--   0        0        0     2278 2024-04-28 19:16:12.004516 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.py
+-rw-r--r--   0        0        0     2634 2024-04-28 19:17:33.854202 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0    58590 2024-04-28 20:56:29.628402 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.JSON
+-rw-r--r--   0        0        0     1929 2024-04-28 19:17:29.690314 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.py
+-rw-r--r--   0        0        0     1862 2024-04-28 19:11:33.194920 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/API_status_1.py
+-rw-r--r--   0        0        0     1888 2024-04-28 20:28:26.819221 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/API_status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1880 2024-04-28 17:59:07.380196 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0    94101 2024-04-28 20:56:40.680279 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/status_1.JSON
+-rw-r--r--   0        0        0     1590 2024-04-28 19:10:15.594738 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/API_status_1.py
+-rw-r--r--   0        0        0     1861 2024-04-28 20:28:26.827221 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/API_status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1853 2024-04-28 17:57:44.252665 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0   214851 2024-04-28 20:56:43.624247 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/status_1.JSON
+-rw-r--r--   0        0        0     1664 2024-04-28 04:43:21.416236 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     2201 2024-04-28 16:55:02.089934 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/add_goals.cpython-310.pyc
+-rw-r--r--   0        0        0      576 2024-04-28 04:35:34.153314 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/find_goal.cpython-310.pyc
+-rw-r--r--   0        0        0     4192 2024-04-28 16:54:48.693981 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/add_goals.py
+-rw-r--r--   0        0        0      477 2024-04-28 04:35:29.457365 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/find_goal.py
+-rw-r--r--   0        0        0     1421 2024-04-28 02:28:19.421723 vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/recipe_with_goals.S.HTML
+-rwxr-xr-x   0        0        0      143 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/shows.S.HTML
+-rwxr-xr-x   0        0        0      561 2024-04-27 18:25:31.750817 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/_assertions/__init__.py
+-rw-r--r--   0        0        0      792 2024-04-27 18:25:53.262563 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/_assertions/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      224 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/FDA.s.HTML
+-rwxr-xr-x   0        0        0      421 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/journal.r.HTML
+-rwxr-xr-x   0        0        0        0 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/calcium.r.HTML
+-rwxr-xr-x   0        0        0      216 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/lipids/lipids.r.HTML
+-rwxr-xr-x   0        0        0       11 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/protein/protein.r.HTML
+-rwxr-xr-x   0        0        0     1351 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin a.r.HTML
+-rwxr-xr-x   0        0        0      807 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin b.r.HTML
+-rwxr-xr-x   0        0        0       93 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin c.r.HTML
+-rwxr-xr-x   0        0        0     1298 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin d.r.HTML
+-rwxr-xr-x   0        0        0      149 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin e.r.HTML
+-rwxr-xr-x   0        0        0      219 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/channel/river.s.HTML
+-rwxr-xr-x   0        0        0      543 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/forward channel.s.HTML
+-rwxr-xr-x   0        0        0      935 2024-04-17 03:33:22.117283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/structures.s.HTML
+-rwxr-xr-x   0        0        0      471 2024-04-17 03:36:50.295021 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      706 2024-04-25 00:16:33.983975 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/__pycache__/develop.cpython-310.pyc
+-rw-r--r--   0        0        0     4797 2024-04-25 00:36:39.253965 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__init__.py
+-rw-r--r--   0        0        0     2213 2024-04-25 00:37:22.933411 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1197 2024-04-24 23:56:39.560827 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1034 2024-04-24 23:56:09.969137 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/status_1.py
+-rw-r--r--   0        0        0     1738 2024-04-24 23:56:39.788825 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1746 2024-04-24 23:56:39.488828 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2137 2024-04-24 23:56:04.641192 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_1.py
+-rwxr-xr-x   0        0        0     2114 2024-04-24 23:55:56.809274 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_2.py
+-rw-r--r--   0        0        0     2128 2024-04-25 00:03:24.840594 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3694 2024-04-25 00:03:21.140633 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/status_1.py
+-rw-r--r--   0        0        0      441 2024-04-25 01:00:06.752757 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/assertions_one/__init__.py
+-rw-r--r--   0        0        0      562 2024-04-25 01:02:38.506933 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/assertions_one/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3264 2024-04-25 00:19:03.893176 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/calculate_portions/__init__.py
+-rw-r--r--   0        0        0     1531 2024-04-25 01:02:38.506933 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/calculate_portions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1358 2024-04-25 01:28:21.171397 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/cultivate/__init__.py
+-rw-r--r--   0        0        0     1059 2024-04-25 01:31:25.482717 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/cultivate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      796 2024-04-25 00:15:47.948849 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/develop.py
+-rw-r--r--   0        0        0     2537 2024-04-25 00:17:17.051140 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__init__.py
+-rw-r--r--   0        0        0     1716 2024-04-25 00:37:48.473088 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      697 2024-04-25 00:37:45.949120 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      447 2024-04-25 00:16:53.147600 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/status_1.py
+-rwxr-xr-x   0        0        0     1775 2024-04-26 02:19:59.665597 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__init__.py
+-rw-r--r--   0        0        0     1404 2024-04-26 02:20:21.177381 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2945 2024-04-17 03:33:22.125283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2090 2024-04-27 17:40:10.779972 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     2227 2024-04-27 17:40:10.791972 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0     1311 2024-04-27 17:40:10.963968 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_loop_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0      950 2024-04-17 03:33:22.125283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/multiply_measures.s.HTML
+-rwxr-xr-x   0        0        0     2547 2024-04-27 17:39:04.177559 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_1.py
+-rwxr-xr-x   0        0        0     2933 2024-04-27 17:39:04.177559 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_2.py
+-rwxr-xr-x   0        0        0     1076 2024-04-27 17:39:04.177559 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_loop_1.py
+-rwxr-xr-x   0        0        0      279 2024-04-24 21:20:53.222120 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      631 2024-04-25 00:59:04.661504 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/assertions/__init__.py
+-rw-r--r--   0        0        0      788 2024-04-25 01:02:38.506933 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/assertions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5604 2024-04-25 01:10:19.889397 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__init__.py
+-rw-r--r--   0        0        0     1687 2024-04-25 01:12:56.963514 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1238 2024-04-25 00:37:45.713123 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0     1109 2024-04-25 00:37:34.509265 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/status_1.py
+-rw-r--r--   0        0        0      543 2024-04-25 00:28:13.396655 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-25 00:29:32.087569 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      953 2024-04-25 00:29:48.903340 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      752 2024-04-25 00:29:43.999407 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/status_1.py
+-rwxr-xr-x   0        0        0     2566 2024-04-28 00:13:52.540684 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__init__.py
+-rw-r--r--   0        0        0     2231 2024-04-28 00:14:29.404256 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1017 2024-04-24 22:13:23.957516 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_cautionary.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1004 2024-04-24 21:26:22.034066 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_essentials.cpython-310.pyc
+-rwxr-xr-x   0        0        0      720 2024-04-24 22:13:18.389563 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/status_cautionary.py
+-rwxr-xr-x   0        0        0      700 2024-04-24 21:26:17.758155 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/status_essentials.py
+-rwxr-xr-x   0        0        0     1295 2024-04-24 22:45:33.169829 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__init__.py
+-rwxr-xr-x   0        0        0     1049 2024-04-24 22:45:47.549673 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1088 2024-04-24 23:20:51.223363 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/status_essentials.cpython-310.pyc
+-rwxr-xr-x   0        0        0      685 2024-04-24 22:45:57.489566 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/status_essentials.py
+-rwxr-xr-x   0        0        0     1357 2024-04-26 01:45:40.405817 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__init__.py
+-rw-r--r--   0        0        0     1216 2024-04-26 01:45:55.765588 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      922 2024-04-24 23:20:51.611359 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_1.cpython-310.pyc
+-rw-r--r--   0        0        0      906 2024-04-25 00:00:13.970586 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_2.cpython-310.pyc
+-rwxr-xr-x   0        0        0      692 2024-04-24 23:19:39.112127 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_1.py
+-rw-r--r--   0        0        0      681 2024-04-25 00:00:10.370624 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_2.py
+-rw-r--r--   0        0        0     1021 2024-04-25 00:41:35.278255 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__init__.py
+-rw-r--r--   0        0        0     1065 2024-04-25 00:41:39.946197 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1018 2024-04-25 00:37:45.877121 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      843 2024-04-25 00:25:33.730936 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/status_1.py
+-rwxr-xr-x   0        0        0     1523 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/grove.S.HTML
+-rwxr-xr-x   0        0        0       58 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/info/info.S.HTML
+-rwxr-xr-x   0        0        0       73 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0       59 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/natures/natures.S.HTML
+-rwxr-xr-x   0        0        0     1508 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/unites/unites.S.HTML
+-rwxr-xr-x   0        0        0     2330 2024-04-23 19:28:57.911458 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/land.S.HTML
+-rwxr-xr-x   0        0        0      395 2024-04-26 01:48:09.659641 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/__init__.py
+-rw-r--r--   0        0        0      575 2024-04-26 02:00:50.941720 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0      459 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0     1355 2024-04-26 01:57:53.387927 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__init__.py
+-rw-r--r--   0        0        0     1118 2024-04-26 02:02:11.196735 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1601 2024-04-17 03:33:22.125283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      937 2024-04-26 02:02:10.948737 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_1.cpython-310.pyc
+-rw-r--r--   0        0        0      935 2024-04-26 02:04:37.130957 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_2.cpython-310.pyc
+-rw-r--r--   0        0        0      868 2024-04-26 02:04:37.222956 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_3.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1177 2024-04-26 02:02:05.356806 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_1.py
+-rwxr-xr-x   0        0        0     1175 2024-04-26 02:02:49.844262 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_2.py
+-rwxr-xr-x   0        0        0     1017 2024-04-26 02:03:05.508071 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_3.py
+-rwxr-xr-x   0        0        0      765 2024-04-26 02:08:49.075920 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__init__.py
+-rw-r--r--   0        0        0      863 2024-04-26 02:08:54.079860 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1336 2024-04-17 03:33:22.125283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1632 2024-04-27 17:40:11.335960 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/status_1.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1685 2024-04-27 17:39:04.181559 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/status_1.py
+-rwxr-xr-x   0        0        0      412 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/natures/natures.S.HTML
+-rwxr-xr-x   0        0        0      405 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/measured_ingredients/measured_ingredients.S.HTML
+-rwxr-xr-x   0        0        0     1066 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/measures/measures.S.HTML
+-rwxr-xr-x   0        0        0      611 2024-04-25 19:49:42.003893 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/nature.S.HTML
+-rwxr-xr-x   0        0        0      310 2024-04-25 20:29:19.933549 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/unmeasured_ingredients/UI.S.HTML
+-rwxr-xr-x   0        0        0      426 2024-04-25 20:36:16.050543 vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/treasure.S.HTML
+-rwxr-xr-x   0        0        0       14 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/vegan -- emojis.S.HTML
+-rwxr-xr-x   0        0        0     4258 2024-04-28 22:56:51.642449 vegan-2.1.2/venues/stages/vegan/vegan.S.HTML
+-rwxr-xr-x   0        0        0      632 2024-04-17 03:33:22.129283 vegan-2.1.2/venues/stages/vegan/vegan.css
+-rw-r--r--   0        0        0     2474 1970-01-01 00:00:00.000000 vegan-2.1.2/PKG-INFO
```

### Comparing `vegan-2.1.1/pyproject.toml` & `vegan-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "vegan"
-version = "2.1.1"
+version = "2.1.2"
 description = "vegan health"
 authors = []
 readme = "venues/stages/vegan/readme.md"
 
 packages = [
     { include = "vegan", from = "venues/stages" }
 ]
```

### Comparing `vegan-2.1.1/venue.S.HTML` & `vegan-2.1.2/venue.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/___license/license.s.HTML` & `vegan-2.1.2/venues/stages/vegan/___license/license.s.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/___license/list/gpl-3.0-standalone.html` & `vegan-2.1.2/venues/stages/vegan/___license/list/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/___objectives/objectives.S.HTML` & `vegan-2.1.2/venues/stages/vegan/___objectives/objectives.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/__status/API/DB/records.json` & `vegan-2.1.2/venues/stages/vegan/__status/API/DB/records.json`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/__status/API/status.proc.py` & `vegan-2.1.2/venues/stages/vegan/__status/API/status.proc.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/__status/__pycache__/status_API.proc.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/__status/__pycache__/status_API.proc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/__status/main/DB/records.json` & `vegan-2.1.2/venues/stages/vegan/__status/main/DB/records.json`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/__status/main/output.json` & `vegan-2.1.2/venues/stages/vegan/__status/main/output.json`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/__status/main/status.proc.py` & `vegan-2.1.2/venues/stages/vegan/__status/main/status.proc.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_ellipses--/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/_ellipses--/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_ellipses--/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/_ellipses--/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_essence/__init__.py` & `vegan-2.1.2/venues/stages/vegan/_essence/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_essence/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/_essence/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_essence/build/__init__.py` & `vegan-2.1.2/venues/stages/vegan/_essence/build/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_essence/build/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/_essence/build/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_ops/__pycache__/off.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_ops/__pycache__/on.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_ops/__pycache__/refresh.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_ops/__pycache__/status.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_ops/clique/__init__.py` & `vegan-2.1.2/venues/stages/vegan/_ops/clique/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/_ops/clique/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/_ops/clique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/_clique.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/off.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/on.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/refresh.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/__pycache__/status.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/_clique.py` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/_clique.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/monitor.py` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/monitor.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/off.py` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/off.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/on.py` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/on.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/_ops/status.py` & `vegan-2.1.2/venues/stages/vegan/adventures/_ops/status.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/customs/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/customs/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/customs/__pycache__/clique.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/customs/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/customs/clique.py` & `vegan-2.1.2/venues/stages/vegan/adventures/customs/clique.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__pycache__/clique.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__pycache__/connect.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/__pycache__/connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/find_name.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/find_name.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/retrieve_every.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/__pycache__/retrieve_every.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/find_name.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/find_name.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/insert_document.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/insert_document.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/retrieve_every.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/_land/retrieve_every.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/connect.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/connect.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/essential_nutrients/essential_nutrients.S.HTML` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/essential_nutrients/essential_nutrients.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/find_ingredient.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/find_ingredient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/insert.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/insert.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/retrieve_one.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/__pycache__/retrieve_one.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/__pycache__/create.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/__pycache__/create.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/__pycache__/drop_and_create.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/__pycache__/drop_and_create.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/drop_and_create.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/_indexes/drop_and_create.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/find_ingredient.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/find_ingredient.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/insert.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/insert.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/retrieve_one.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/goals/retrieve_one.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/DB/vegan_tract/ingredients.S.HTML` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/DB/vegan_tract/ingredients.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/clique.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/connect.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/connect.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/off.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/on.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__pycache__/status.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/1.JSON` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/1.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/2.JSON` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/2.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/3.JSON` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/3.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/4.JSON` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/4.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/5.JSON` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/5.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/6.JSON` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/essential_nutrients/6.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/goals/5.JSON` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/goals/5.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/goals/6.JSON` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/exports/vegan_tract/goals/6.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/__saves/saves.S.HTML` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/__saves/saves.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/_clique.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/_clique.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/off.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/off.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/on.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/on.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/__pycache__/_clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/__pycache__/clique.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/saves/_clique.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/saves/_clique.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/monetary/_ops/status.py` & `vegan-2.1.2/venues/stages/vegan/adventures/monetary/_ops/status.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/off.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/on.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/refresh.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/status.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/redis_mix/_ops/_clique.py` & `vegan-2.1.2/venues/stages/vegan/adventures/redis_mix/_ops/_clique.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/__pycache__/off.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/__pycache__/on.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/__pycache__/refresh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/__pycache__/status.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/off.py` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/off.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/on.py` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/on.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/refresh.py` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/refresh.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/_ops/status.py` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/_ops/status.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/clique.py` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/clique.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/harbor/__init__.py` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/harbor/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/adventures/sanique/sanique.S.HTML` & `vegan-2.1.2/venues/stages/vegan/adventures/sanique/sanique.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/__pycache__/source.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/__pycache__/source.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/BRANDED.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/branded.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/assertions/__pycache__/foundational.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/status/API_status_foundational_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/status/API_status_foundational_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/status/__pycache__/API_status_branded_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/status/__pycache__/API_status_branded_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/deliveries/one/status/__pycache__/API_status_foundational_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/deliveries/one/status/__pycache__/API_status_foundational_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/Gardein_f'sh_2663758.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/Gardein_f'sh_2664238.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/beet_juice_2412474.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/beet_juice_2412474.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/beet_juice_2642759.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/beet_juice_2642759.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/impossible_beef_2664238.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/impossible_beef_2664238.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/problems/impossible_2468423.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/problems/impossible_2468423.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/vegan_pizza_2672996.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/vegan_pizza_2672996.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/branded/walnuts_1882785.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/branded/walnuts_1882785.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/examples/foundational/2346404_sweet_potatoes.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/food.s.HTML` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/food.s.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/assertions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/assertions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_mass_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_mass_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_volume_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/__pycache__/status_volume_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/label_splitter/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_mass_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_volume_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/interpret/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/status_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_interpret/packageWeight/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/API_status_found_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/API_status_found_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/API_status_not_found_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/API_status_not_found_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_found_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_found_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_not_found_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/API_status_not_found_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_1_description.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_1_description.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_2_measures.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_2_measures.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_4_land_essentials.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_4_land_essentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_4_lands.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/__pycache__/status_4_lands.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_1_description.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_1_description.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_2_measures.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_2_measures.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_3_measured_ingredients.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_3_measured_ingredients.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_4_lands.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status/status_4_lands.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2412474.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_2412474.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_3.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_loop_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/__pycache__/status_loop_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_2.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_2.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_2412474.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_2412474.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_3.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_3.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_loop_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/_status_v1/status_loop_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/land/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/land/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/land/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/land/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/for_each/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/status_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_ops/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_mass_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_mass_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_volume_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/__pycache__/status_volume_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/status_mass_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/status_volume_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/_status/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured ingredients.S.HTML` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured ingredients.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_IU_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_IU_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_energy_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_energy_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_mass_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_mass_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_IU_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_IU_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_energy_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_energy_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_mass_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/_status/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/biological_activity/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/energy/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/mass/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/food_nutrient_calculator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/__pycache__/label_nutrient_calculator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/food_nutrient.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/amount/per_package/food_nutrient.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient_prototype_1.r.HTML` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measured_ingredients/measured_ingredient/ingredient_prototype_1.r.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/status_mass_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/status_mass_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/status_volume_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/__pycache__/status_volume_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/status_mass_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/status_mass_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/status_volume_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/food_USDA/nature_v2/measures/form/status_volume_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/NIH.s.HTML` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/NIH.s.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/__pycache__/source.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/__pycache__/source.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/__pycache__/assertions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/assertions.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/assertions.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/deliveries/one/status/__pycache__/API_status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/deliveries/one/status/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/coated tablets/multivitamin_276336.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/coated tablets/multivitamin_276336.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/other/chia_seeds_214893.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/other/chia_seeds_214893.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/powder/mane_270619.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/powder/mane_270619.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/powder/nutritional_shake_220884.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/powder/nutritional_shake_220884.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/powder packets/multivitamin_246811.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/powder packets/multivitamin_246811.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/tablets/calcium_261967.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/tablets/calcium_261967.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/tablets/multivitamin_249664.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/tablets/multivitamin_249664.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/examples/vegan_capsules/probiotics_248267.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/status_powder_packets_246811.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/__pycache__/status_powder_packets_246811.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/status_powder_packets_246811.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_interpret/ingredientRows/for_each/status_powder_packets_246811.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_ops/retrieve/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_ops/retrieve/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_ops/retrieve/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_1_info.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_1_info.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_2_form.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_2_form.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_3_measured_ingredients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_essential_nutrients.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_essential_nutrients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_unmeasured_ingredients.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_4_unmeasured_ingredients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_5_essential_nutrients.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_5_essential_nutrients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_6_cautionary_ingredients.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/__pycache__/status_6_cautionary_ingredients.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/mane_270619_nature.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/mane_270619_nature.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/multivitamin_249664.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/multivitamin_249664.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_1_info.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_1_info.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_2_form.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_2_form.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_3_measured_ingredients.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_3_measured_ingredients.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_4_unmeasured_ingredients.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_4_unmeasured_ingredients.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_5_essential_nutrients.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_5_essential_nutrients.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_6_cautionary_ingredients.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status/status_6_cautionary_ingredients.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/_loop/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/_loop/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/_loop/status_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/_loop/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/__pycache__/status_multivitamin_276336.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/__pycache__/status_multivitamin_276336.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336_nature.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/coated_tablets/status_multivitamin_276336_nature.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/__pycache__/status_chia_seeds_214893.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/__pycache__/status_chia_seeds_214893.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/chia_seeds_214893_nature.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/chia_seeds_214893_nature.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/status_chia_seeds_214893.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/other/status_chia_seeds_214893.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/__pycache__/status_mane_270619.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/__pycache__/status_mane_270619.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/mane_270619_nature.JSON` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/mane_270619_nature.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/status_mane_270619.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/_status_v1/powder/status_mane_270619.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/status_other_214893.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/__pycache__/status_other_214893.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/status_other_214893.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/amount/status_other_214893.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/form.S.HTML` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/form.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_246811.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_246811.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_276336.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/__pycache__/status_276336.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/status_246811.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/status_246811.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/status_276336.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/serving_size/amount/status_276336.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_coated_tablet_276336.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_coated_tablet_276336.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_gram_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_gram_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_220884.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_220884.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_270619.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_270619.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_packets_246811.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_powder_packets_246811.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_tablet_261967.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_tablet_261967.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_vegan_capsule_248267.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/__pycache__/status_vegan_capsule_248267.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_coated_tablet_276336.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_coated_tablet_276336.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_gram_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_gram_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_220884.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_220884.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_270619.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_270619.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_packets_246811.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_powder_packets_246811.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_tablet_261967.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_tablet_261967.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_vegan_capsule_248267.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/form/unit/status_vegan_capsule_248267.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/land/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/land/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/land/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/land/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/status_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_ops/seek_name/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_status/__pycache__/status_chia_seeds_214893.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_status/__pycache__/status_chia_seeds_214893.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_status/status_chia_seeds_214893.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/_status/status_chia_seeds_214893.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__init__.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/status_1.py` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/_status/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/measured_ingredient.S.HTML` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredient/measured_ingredient.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredients.S.HTML` & `vegan-2.1.2/venues/stages/vegan/besties/supp_NIH/nature_v2/measured_ingredients/measured_ingredients.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/goals/umuntu/FDA.py` & `vegan-2.1.2/venues/stages/vegan/goals/umuntu/FDA.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/goals/umuntu/FDA_v1.py` & `vegan-2.1.2/venues/stages/vegan/goals/umuntu/FDA_v1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/goals/umuntu/FDA_v2.py` & `vegan-2.1.2/venues/stages/vegan/goals/umuntu/FDA_v2.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/goals/umuntu/FDA_v3.py` & `vegan-2.1.2/venues/stages/vegan/goals/umuntu/FDA_v3.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/goals/umuntu/__pycache__/FDA.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/goals/umuntu/__pycache__/FDA.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/goals/umuntu/__pycache__/FDA_v3.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/goals/umuntu/__pycache__/FDA_v3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/goals/umuntu/_ops/__pycache__/retrieve.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/goals/umuntu/_ops/__pycache__/retrieve.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/_interpret/__pycache__/status_unit_kind.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/_interpret/__pycache__/status_unit_kind.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/_interpret/__pycache__/unit_kind.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/_interpret/__pycache__/unit_kind.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/_interpret/status_unit_kind.py` & `vegan-2.1.2/venues/stages/vegan/measures/_interpret/status_unit_kind.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/_interpret/unit_kind.py` & `vegan-2.1.2/venues/stages/vegan/measures/_interpret/unit_kind.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/energy/energy.r.HTML` & `vegan-2.1.2/venues/stages/vegan/measures/energy/energy.r.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/energy/swap/__init__.py` & `vegan-2.1.2/venues/stages/vegan/measures/energy/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/energy/swap/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/energy/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/energy/swap/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/energy/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/energy/swap/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/energy/swap/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass/swap/__init__.py` & `vegan-2.1.2/venues/stages/vegan/measures/mass/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass/swap/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/mass/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass/swap/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/mass/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass/swap/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/mass/swap/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass/swap/status_1.py` & `vegan-2.1.2/venues/stages/vegan/measures/mass/swap/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass/system international.r.html` & `vegan-2.1.2/venues/stages/vegan/measures/mass/system international.r.html`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass/us customary.r.html` & `vegan-2.1.2/venues/stages/vegan/measures/mass/us customary.r.html`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__init__.py` & `vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/is_an_equivalent/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/jargon.r.HTML` & `vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/jargon.r.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/mass_equivalents/mass equivalents.r.HTML` & `vegan-2.1.2/venues/stages/vegan/measures/mass_equivalents/mass equivalents.r.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__init__.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_2.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_3.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_sci_note_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/__pycache__/status_sci_note_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/status_1.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/status_2.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/status_2.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/decimal/reduce/status_3.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/decimal/reduce/status_3.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/integer/__pycache__/status_string_is_integer.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/integer/__pycache__/status_string_is_integer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/integer/__pycache__/string_is_integer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/integer/__pycache__/string_is_integer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/integer/status_string_is_integer.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/integer/status_string_is_integer.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/percentage/__pycache__/from_fraction.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/percentage/__pycache__/from_fraction.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/percentage/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/percentage/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/percentage/from_fraction.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/percentage/from_fraction.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/percentage/status_1.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/percentage/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/__init__.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/_status/__pycache__/status_multiples_of_3_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/_status/__pycache__/status_multiples_of_3_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/_status/status_multiples_of_3_1.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/_status/status_multiples_of_3_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/sci_note.S.HTML` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/sci_note.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/sci_note_possibilities.S.HTML` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/sci_note_possibilities.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note/sci_note_thoughts.S.HTML` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note/sci_note_thoughts.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note_2/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note_2/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note_2/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/number/sci_note_2/status_1.py` & `vegan-2.1.2/venues/stages/vegan/measures/number/sci_note_2/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/volume/swap/__init__.py` & `vegan-2.1.2/venues/stages/vegan/measures/volume/swap/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/volume/swap/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/volume/swap/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/volume/swap/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/volume/swap/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/volume/swap/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/measures/volume/swap/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/volume/swap/status_1.py` & `vegan-2.1.2/venues/stages/vegan/measures/volume/swap/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/measures/weight/weight.r.html` & `vegan-2.1.2/venues/stages/vegan/measures/weight/weight.r.html`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/equalities.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/equalities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/override_print.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/override_print.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/mixes/insure/__pycache__/status_equalitites_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/mixes/insure/__pycache__/status_equalitites_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/mixes/insure/equalities.py` & `vegan-2.1.2/venues/stages/vegan/mixes/insure/equalities.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/mixes/insure/override_print.py` & `vegan-2.1.2/venues/stages/vegan/mixes/insure/override_print.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/mixes/procedure/__init__.py` & `vegan-2.1.2/venues/stages/vegan/mixes/procedure/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/mixes/procedure/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/mixes/procedure/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/readme.md` & `vegan-2.1.2/venues/stages/vegan/readme.md`

 * *Files 23% similar despite different names*

```diff
@@ -11,38 +11,32 @@
 
 You are now officially certified to include "vegan" in your practice!
 
 Encore! Encore! Encore! Encore!
 
 ******
 
-<section style="border: 2px solid black; border-radius: 6px">
-	<h1>vegan</h1>
+# vegan
 
 
-</section>
+## summary
 
-<div style="height: 1px; background: black;" ></div>	
 
-
-<h2>summary</h2>
-
-
-<div style="height: 1px; background: black;" ></div>	
 		
-<h2>obtain</h2>
-`[USD] pip install vegan`
-
+## obtain
+```
+[USD] pip install vegan
+```
 
 ---	
-<h2>on</h2>
+## on
 
 
 
-<code>
+```
 	#
 	#	vegan_essence.py
 	#
 	#
 
 	import json
 	fp = open ("/online/ridges/vegan/ridges.JSON", "r")
@@ -73,29 +67,30 @@
 		"USDA": {
 			"food": ridges ["USDA"] ["food"]
 		},
 		"NIH": {
 			"supp": ridges ["NIH"] ["supp"]
 		}
 	}
-</code>
+```
 
-<code>
+```
 	vegan adventures on
-</code>
+```
 
-<code>
+```
 	vegan adventures monetary saves import --name 5.JSON
-</code>
+```
 
 ---
 
 ## tutorial
-`[USD] vegan help`
-
+```
+[USD] vegan help
+```
 ---
 
 ## contacts
 Bryan@Status600.com
```

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/goodness_certifications/certifications.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/goodness_certifications/certifications.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/goodness_certifications/vegan.S.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/goodness_certifications/vegan.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/assertions/__pycache__/ingredient.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/assertions/__pycache__/ingredient.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/assertions/ingredient.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/assertions/ingredient.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_empty/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_empty/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_empty/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_empty/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_0.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_0.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_2.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_3.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_0.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_0.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_2.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_2.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_3.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_food/status_3.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.JSON` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_foods_and_supps/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.JSON` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_rational_amounts/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1_supp_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/__pycache__/status_1_supp_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.JSON` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1_supp_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/formulate/_status/status_supp/status_1_supp_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/_status/API_status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/_status/API_status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/_status/__pycache__/API_status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/_ops/retrieve/_status/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/land/_ops/formulate/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/land/_ops/formulate/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe/land/_ops/formulate/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe/land/_ops/formulate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/__pycache__/formulate.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/__pycache__/formulate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.JSON` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/1_3_recipe_prefomulated/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.JSON` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status/2_food/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/API_status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/API_status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/API_status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/status_1.JSON` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_1_recipe/status_1.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/API_status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/API_status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/API_status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/API_status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/status_1.JSON` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/1_2_recipe/status_1.JSON`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/_status_API/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/add_goals.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/add_goals.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/find_goal.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/__pycache__/find_goal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/add_goals.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/_ops/formulate/modules/add_goals.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/recipe_with_goals/recipe_with_goals.S.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/recipe_with_goals/recipe_with_goals.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/_assertions/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/_assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/_assertions/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/_assertions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin a.r.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin a.r.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin b.r.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin b.r.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin d.r.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/_journal/structures/vitamin d.r.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/forward channel.s.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/forward channel.s.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/structures.s.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/forward_channel/structures.s.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/__pycache__/develop.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/__pycache__/develop.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_empty_grove/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_2.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_2.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_and_meq/status_2.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/add_measured_ingredient/status_m_eq_and_ba/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/assertions_one/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/assertions_one/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/calculate_portions/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/calculate_portions/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/calculate_portions/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/calculate_portions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/cultivate/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/cultivate/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/cultivate/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/cultivate/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/develop.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/develop.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/measures_sums/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_2.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_loop_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/__pycache__/status_loop_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/multiply_measures.s.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/multiply_measures.s.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_2.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_2.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_loop_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/_ops/multiply_amount/status_loop_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/assertions/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/assertions/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/assertions/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/assertions/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/has_uniters/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/is_story_1/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_cautionary.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_cautionary.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_essentials.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/__pycache__/status_essentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/status_cautionary.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/status_cautionary.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/status_essentials.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/nurture/status_essentials.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/status_essentials.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/__pycache__/status_essentials.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/status_essentials.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek/status_essentials.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_2.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/__pycache__/status_essentials_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_2.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_name_or_accepts/status_essentials_2.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/_ops/seek_uniter/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/grove.S.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/grove.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/grove/unites/unites.S.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/grove/unites/unites.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/land.S.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/land.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_2.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_3.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/__pycache__/status_3.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_2.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_2.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_3.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/merge/status_3.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__init__.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__init__.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-311.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/status_1.cpython-310.pyc` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/__pycache__/status_1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/status_1.py` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/land/measures/multiply/status_1.py`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/measures/measures.S.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/measures/measures.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/shows_v2/treasure/nature/nature.S.HTML` & `vegan-2.1.2/venues/stages/vegan/shows_v2/treasure/nature/nature.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/vegan.S.HTML` & `vegan-2.1.2/venues/stages/vegan/vegan.S.HTML`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/venues/stages/vegan/vegan.css` & `vegan-2.1.2/venues/stages/vegan/vegan.css`

 * *Files identical despite different names*

### Comparing `vegan-2.1.1/PKG-INFO` & `vegan-2.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vegan
-Version: 2.1.1
+Version: 2.1.2
 Summary: vegan health
 License: >1 [Vegan + GPL 3.0 + Non-Commercial]
 Keywords: vegan
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -42,38 +42,32 @@
 
 You are now officially certified to include "vegan" in your practice!
 
 Encore! Encore! Encore! Encore!
 
 ******
 
-<section style="border: 2px solid black; border-radius: 6px">
-	<h1>vegan</h1>
+# vegan
 
 
-</section>
+## summary
 
-<div style="height: 1px; background: black;" ></div>	
 
-
-<h2>summary</h2>
-
-
-<div style="height: 1px; background: black;" ></div>	
 		
-<h2>obtain</h2>
-`[USD] pip install vegan`
-
+## obtain
+```
+[USD] pip install vegan
+```
 
 ---	
-<h2>on</h2>
+## on
 
 
 
-<code>
+```
 	#
 	#	vegan_essence.py
 	#
 	#
 
 	import json
 	fp = open ("/online/ridges/vegan/ridges.JSON", "r")
@@ -104,29 +98,30 @@
 		"USDA": {
 			"food": ridges ["USDA"] ["food"]
 		},
 		"NIH": {
 			"supp": ridges ["NIH"] ["supp"]
 		}
 	}
-</code>
+```
 
-<code>
+```
 	vegan adventures on
-</code>
+```
 
-<code>
+```
 	vegan adventures monetary saves import --name 5.JSON
-</code>
+```
 
 ---
 
 ## tutorial
-`[USD] vegan help`
-
+```
+[USD] vegan help
+```
 ---
 
 ## contacts
 Bryan@Status600.com
```

