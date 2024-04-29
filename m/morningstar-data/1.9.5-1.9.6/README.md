# Comparing `tmp/morningstar_data-1.9.5.tar.gz` & `tmp/morningstar_data-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-1.9.5.tar", max compression
+gzip compressed data, was "morningstar_data-1.9.6.tar", max compression
```

## Comparing `morningstar_data-1.9.5.tar` & `morningstar_data-1.9.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0      558 2024-04-24 21:02:12.678098 morningstar_data-1.9.5/LICENSE
--rw-r--r--   0        0        0    11417 2024-04-24 21:02:12.678098 morningstar_data-1.9.5/README.md
--rw-r--r--   0        0        0      168 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/__init__.py
--rw-r--r--   0        0        0      598 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/_base.py
--rw-r--r--   0        0        0     4233 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/_utils.py
--rw-r--r--   0        0        0       82 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/_version.py
--rw-r--r--   0        0        0       61 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/__init__.py
--rw-r--r--   0        0        0       62 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/__init__.py
--rw-r--r--   0        0        0      557 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/_file.py
--rw-r--r--   0        0        0      763 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/_table.py
--rw-r--r--   0        0        0      996 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/csvfile.py
--rw-r--r--   0        0        0     2202 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/temptable.py
--rw-r--r--   0        0        0      544 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/_error_messages.py
--rw-r--r--   0        0        0      937 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/_exceptions.py
--rw-r--r--   0        0        0     5604 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/datalake/base.py
--rw-r--r--   0        0        0     1171 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/__init__.py
--rw-r--r--   0        0        0     2432 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_api.py
--rw-r--r--   0        0        0      179 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_backend_apis/__init__.py
--rw-r--r--   0        0        0     2075 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_backend_apis/_delivery_backend.py
--rw-r--r--   0        0        0     4790 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_backend_apis/_holdings_backend.py
--rw-r--r--   0        0        0     3372 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_backend_apis/_signed_url_backend.py
--rw-r--r--   0        0        0     3795 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_base_api.py
--rw-r--r--   0        0        0     5076 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_config.py
--rw-r--r--   0        0        0     1999 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_config_key.py
--rw-r--r--   0        0        0     7854 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_core_api.py
--rw-r--r--   0        0        0      197 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_data_objects/__init__.py
--rw-r--r--   0        0        0     2296 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_data_objects/_custom_data_points_types.py
--rw-r--r--   0        0        0    26798 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_data_objects/_data_points_object.py
--rw-r--r--   0        0        0     7574 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_data_objects/_investments_object.py
--rw-r--r--   0        0        0     2887 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_data_point.py
--rw-r--r--   0        0        0     1453 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_data_type.py
--rw-r--r--   0        0        0     1614 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_decorator.py
--rw-r--r--   0        0        0    14042 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_error_messages.py
--rw-r--r--   0        0        0     3711 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_exceptions.py
--rw-r--r--   0        0        0        0 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_investment/__init__.py
--rw-r--r--   0        0        0     4620 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_investment/_asset_flow_data.py
--rw-r--r--   0        0        0     1560 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_investment/_common.py
--rw-r--r--   0        0        0     9136 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_investment/_data.py
--rw-r--r--   0        0        0     8526 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_investment/_normal_data.py
--rw-r--r--   0        0        0     5127 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_investment/_peer_group_data.py
--rw-r--r--   0        0        0      162 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_portfolio/__init__.py
--rw-r--r--   0        0        0     1273 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_portfolio/_common.py
--rw-r--r--   0        0        0     8263 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
--rw-r--r--   0        0        0     8023 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_portfolio/_portfolio_settings.py
--rw-r--r--   0        0        0      719 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_portfolio/_portfolio_type.py
--rw-r--r--   0        0        0    11071 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_portfolio_data_set.py
--rw-r--r--   0        0        0     3356 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/_utils.py
--rw-r--r--   0        0        0    13081 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/asset_flow.py
--rw-r--r--   0        0        0    16435 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/custom_database.py
--rw-r--r--   0        0        0     1513 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/data_type.py
--rw-r--r--   0        0        0    45132 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/holdings.py
--rw-r--r--   0        0        0    18226 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/investment.py
--rw-r--r--   0        0        0    32429 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/lookup.py
--rw-r--r--   0        0        0     6154 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/peer_group.py
--rw-r--r--   0        0        0    19460 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/performance_report.py
--rw-r--r--   0        0        0    37410 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/portfolio.py
--rw-r--r--   0        0        0    11511 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/returns.py
--rw-r--r--   0        0        0      455 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/user_items/__init__.py
--rw-r--r--   0        0        0      582 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/user_items/_utils.py
--rw-r--r--   0        0        0     7910 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/user_items/data_set.py
--rw-r--r--   0        0        0    13091 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/user_items/investment_lists.py
--rw-r--r--   0        0        0    11276 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/user_items/portfolio.py
--rw-r--r--   0        0        0    10433 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/direct/user_items/search_criteria.py
--rw-r--r--   0        0        0     4768 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/lookup.py
--rw-r--r--   0        0        0       90 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/mdapi/__init__.py
--rw-r--r--   0        0        0     2359 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/mdapi/_exceptions.py
--rw-r--r--   0        0        0     6256 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/mdapi/_mdapi.py
--rw-r--r--   0        0        0     1496 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/mdapi/_types.py
--rw-r--r--   0        0        0      128 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/utils/__init__.py
--rw-r--r--   0        0        0    10975 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/utils/_delivery_config.py
--rw-r--r--   0        0        0     5814 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/utils/_helpers.py
--rw-r--r--   0        0        0    18353 2024-04-24 21:02:12.686098 morningstar_data-1.9.5/morningstar_data/utils/delivery.py
--rw-r--r--   0        0        0     2316 2024-04-24 21:04:14.932469 morningstar_data-1.9.5/pyproject.toml
--rw-r--r--   0        0        0    12424 1970-01-01 00:00:00.000000 morningstar_data-1.9.5/PKG-INFO
+-rw-r--r--   0        0        0      558 2024-04-29 16:50:07.280376 morningstar_data-1.9.6/LICENSE
+-rw-r--r--   0        0        0    11417 2024-04-29 16:50:07.280376 morningstar_data-1.9.6/README.md
+-rw-r--r--   0        0        0      168 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      598 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/_base.py
+-rw-r--r--   0        0        0     4233 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       82 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/_version.py
+-rw-r--r--   0        0        0       61 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       62 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      557 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      763 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0      996 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2202 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      544 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      937 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5604 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0     1171 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2432 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      179 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     2075 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     4798 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3376 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3799 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     5076 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     1999 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7854 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      197 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2296 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26798 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7574 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2887 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1453 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1614 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    14042 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3711 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4620 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1560 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     9136 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8526 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5131 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      162 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1277 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     8263 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     8023 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      719 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    11071 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3356 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    13085 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16439 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1513 2024-04-29 16:50:07.288376 morningstar_data-1.9.6/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    45132 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    18226 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    32433 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6154 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19460 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    37410 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    11511 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      455 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      582 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     7914 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    13095 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11276 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10437 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4772 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/lookup.py
+-rw-r--r--   0        0        0       90 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/mdapi/__init__.py
+-rw-r--r--   0        0        0     2359 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/mdapi/_exceptions.py
+-rw-r--r--   0        0        0     6256 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/mdapi/_mdapi.py
+-rw-r--r--   0        0        0     1496 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/mdapi/_types.py
+-rw-r--r--   0        0        0      128 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0    10975 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     5881 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    18353 2024-04-29 16:50:07.292376 morningstar_data-1.9.6/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2316 2024-04-29 16:52:17.187673 morningstar_data-1.9.6/pyproject.toml
+-rw-r--r--   0        0        0    12424 1970-01-01 00:00:00.000000 morningstar_data-1.9.6/PKG-INFO
```

### Comparing `morningstar_data-1.9.5/LICENSE` & `morningstar_data-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/README.md` & `morningstar_data-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/_base.py` & `morningstar_data-1.9.6/morningstar_data/_base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/_utils.py` & `morningstar_data-1.9.6/morningstar_data/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/_file.py` & `morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/_file.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/_table.py` & `morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/_table.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/csvfile.py` & `morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/csvfile.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/datalake/_data_objects/temptable.py` & `morningstar_data-1.9.6/morningstar_data/datalake/_data_objects/temptable.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/datalake/_error_messages.py` & `morningstar_data-1.9.6/morningstar_data/datalake/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/datalake/_exceptions.py` & `morningstar_data-1.9.6/morningstar_data/datalake/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/datalake/base.py` & `morningstar_data-1.9.6/morningstar_data/datalake/base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/__init__.py` & `morningstar_data-1.9.6/morningstar_data/direct/__init__.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_api.py` & `morningstar_data-1.9.6/morningstar_data/direct/_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_backend_apis/_delivery_backend.py` & `morningstar_data-1.9.6/morningstar_data/direct/_backend_apis/_delivery_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_backend_apis/_holdings_backend.py` & `morningstar_data-1.9.6/morningstar_data/direct/_backend_apis/_holdings_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     def __init__(self) -> None:
         super().__init__()
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_HOLDING) from None
 
 
 class FoFAPIBackend(APIBackend):
     """
@@ -127,11 +127,11 @@
             self._handle_custom_http_errors(res)
             self._handle_default_http_errors(res)
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_HOLDING) from None
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_backend_apis/_signed_url_backend.py` & `morningstar_data-1.9.6/morningstar_data/direct/_backend_apis/_signed_url_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             self._handle_default_http_errors(res)
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
         try:
-            response_message = res.json()["message"]
+            response_message = res.json().get("message")
         except requests.JSONDecodeError:
             response_message = res.text
 
         if res.status_code == 400:
             _logger.debug(f"Bad Request Error: {res.status_code} {response_message}")
             raise InvalidQueryException(response_message) from None
         if res.status_code == 401:
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_base_api.py` & `morningstar_data-1.9.6/morningstar_data/direct/_base_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             self._handle_default_http_errors(res)
 
     def _handle_default_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with standard messages
         """
         try:
-            response_message = res.json()["message"]
+            response_message = res.json().get("message")
         except KeyError:
             response_message = res.json()
             _logger.debug("DO Request Error")
         if res.status_code == 401:
             _logger.debug(f"Access Denied Error: {res.status_code} {response_message}")
             raise AccessDeniedError from None
         elif res.status_code == 403:
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_config.py` & `morningstar_data-1.9.6/morningstar_data/direct/_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_config_key.py` & `morningstar_data-1.9.6/morningstar_data/direct/_config_key.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_core_api.py` & `morningstar_data-1.9.6/morningstar_data/direct/_core_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_data_objects/_custom_data_points_types.py` & `morningstar_data-1.9.6/morningstar_data/direct/_data_objects/_custom_data_points_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_data_objects/_data_points_object.py` & `morningstar_data-1.9.6/morningstar_data/direct/_data_objects/_data_points_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_data_objects/_investments_object.py` & `morningstar_data-1.9.6/morningstar_data/direct/_data_objects/_investments_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_data_point.py` & `morningstar_data-1.9.6/morningstar_data/direct/_data_point.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_data_type.py` & `morningstar_data-1.9.6/morningstar_data/direct/_data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_decorator.py` & `morningstar_data-1.9.6/morningstar_data/direct/_decorator.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_error_messages.py` & `morningstar_data-1.9.6/morningstar_data/direct/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_exceptions.py` & `morningstar_data-1.9.6/morningstar_data/direct/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_investment/_asset_flow_data.py` & `morningstar_data-1.9.6/morningstar_data/direct/_investment/_asset_flow_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_investment/_common.py` & `morningstar_data-1.9.6/morningstar_data/direct/_investment/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_investment/_data.py` & `morningstar_data-1.9.6/morningstar_data/direct/_investment/_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_investment/_normal_data.py` & `morningstar_data-1.9.6/morningstar_data/direct/_investment/_normal_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_investment/_peer_group_data.py` & `morningstar_data-1.9.6/morningstar_data/direct/_investment/_peer_group_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     def __init__(self) -> None:
         super().__init__()
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError from None
 
         if res.status_code == 500:
             _logger.debug(f"Something went wrong: {res.status_code} {response_message}")
             raise InternalServerError(response_message) from None
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_portfolio/_common.py` & `morningstar_data-1.9.6/morningstar_data/direct/_portfolio/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,11 +31,11 @@
     def __init__(self) -> None:
         super().__init__()
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise PortfolioNotFoundError(RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_List) from None
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py` & `morningstar_data-1.9.6/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_portfolio/_portfolio_settings.py` & `morningstar_data-1.9.6/morningstar_data/direct/_portfolio/_portfolio_settings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_portfolio/_portfolio_type.py` & `morningstar_data-1.9.6/morningstar_data/direct/_portfolio/_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_portfolio_data_set.py` & `morningstar_data-1.9.6/morningstar_data/direct/_portfolio_data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/_utils.py` & `morningstar_data-1.9.6/morningstar_data/direct/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/asset_flow.py` & `morningstar_data-1.9.6/morningstar_data/direct/asset_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def __init__(self) -> None:
         super().__init__()
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 403 and "Exceed query limitation." in response_message:
             _logger.debug(f"Query Limit Exception: {res.status_code} {response_message}")
             query_limit = self._get_security_data_query_limit()
             raise QueryLimitException(query_limit) from None
         elif res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ASSET_FLOW) from None
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/custom_database.py` & `morningstar_data-1.9.6/morningstar_data/direct/custom_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __init__(self) -> None:
         super().__init__()
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_CUSTOM_DATABASE) from None
 
 
 ResultType = Dict[str, Union[bool, str]]
 ListDatapointType = List[Dict[str, Any]]
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/data_type.py` & `morningstar_data-1.9.6/morningstar_data/direct/data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/holdings.py` & `morningstar_data-1.9.6/morningstar_data/direct/holdings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/investment.py` & `morningstar_data-1.9.6/morningstar_data/direct/investment.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/lookup.py` & `morningstar_data-1.9.6/morningstar_data/direct/lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             return _error_messages.RESOURCE_NOT_FOUND_ERROR_DATA_POINT_LOOKUP
         return _error_messages.RESOURCE_NOT_FOUND_ERROR
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(self._get_resource_not_found_message()) from None
 
 
 _data_set_lookup_api_request = LookupDataAPIBackend(_LookupModule.DATA_SET)
 _investment_lookup_api_request = LookupDataAPIBackend(_LookupModule.INVESTMENT)
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/peer_group.py` & `morningstar_data-1.9.6/morningstar_data/direct/peer_group.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/performance_report.py` & `morningstar_data-1.9.6/morningstar_data/direct/performance_report.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/portfolio.py` & `morningstar_data-1.9.6/morningstar_data/direct/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/returns.py` & `morningstar_data-1.9.6/morningstar_data/direct/returns.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/user_items/_utils.py` & `morningstar_data-1.9.6/morningstar_data/direct/user_items/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/user_items/data_set.py` & `morningstar_data-1.9.6/morningstar_data/direct/user_items/data_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     def __init__(self) -> None:
         super().__init__()
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_DATA_SET) from None
         else:
             pass
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/user_items/investment_lists.py` & `morningstar_data-1.9.6/morningstar_data/direct/user_items/investment_lists.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     def __init__(self) -> None:
         super().__init__()
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_INVESTMENT_List) from None
 
 
 _investment_list_api_request = InvestmentListAPIBackend()
```

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/user_items/portfolio.py` & `morningstar_data-1.9.6/morningstar_data/direct/user_items/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/direct/user_items/search_criteria.py` & `morningstar_data-1.9.6/morningstar_data/direct/user_items/search_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def __init__(self) -> None:
         super().__init__()
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_SEARCH_CRITERIA) from None
         else:
             pass
```

### Comparing `morningstar_data-1.9.5/morningstar_data/lookup.py` & `morningstar_data-1.9.6/morningstar_data/lookup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             return RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD
         return RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD_UNIVERSE
 
     def _handle_custom_http_errors(self, res: Any) -> Any:
         """
         Handle HTTP errors with custom error messages
         """
-        response_message = res.json()["message"]
+        response_message = res.json().get("message")
         if res.status_code == 404:
             _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
             raise ResourceNotFoundError(self._get_resource_not_found_message()) from None
 
 
 _keyword_api_request = LookupAPIBackend(_LookupParameter.KEYWORD)
 _keyword_universe_api_request = LookupAPIBackend(_LookupParameter.KEYWORD_UNIVERSE)
```

### Comparing `morningstar_data-1.9.5/morningstar_data/mdapi/_exceptions.py` & `morningstar_data-1.9.6/morningstar_data/mdapi/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/mdapi/_mdapi.py` & `morningstar_data-1.9.6/morningstar_data/mdapi/_mdapi.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/mdapi/_types.py` & `morningstar_data-1.9.6/morningstar_data/mdapi/_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/utils/_delivery_config.py` & `morningstar_data-1.9.6/morningstar_data/utils/_delivery_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/morningstar_data/utils/_helpers.py` & `morningstar_data-1.9.6/morningstar_data/utils/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,16 @@
         _logger.error("Could not encrypt password using /encrypt-message")
         raise
 
 
 def _create_output_file_name(file_path: str) -> str:
     """Creates the output file name for the file which will be uploaded to MDS s3 bucket"""
     file_name = pathlib.Path(file_path).name
-    return f"{uuid.uuid4()}-{file_name}"
+    mds_request_id = os.getenv("FEED_RUN_ID", str(uuid.uuid4()))
+    return f"{mds_request_id}-{file_name}"
 
 
 def _retrieve_credentials() -> Dict[str, str]:
     """Retrieves the credentials required to access the MDS s3 bucket"""
     _api_backend = DeliveryAPIBackend()
     url = f"{_get_al_proxy_base_url()}assume-mds-role?user_id={_get_user_id()}"
     try:
```

### Comparing `morningstar_data-1.9.5/morningstar_data/utils/delivery.py` & `morningstar_data-1.9.6/morningstar_data/utils/delivery.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.9.5/pyproject.toml` & `morningstar_data-1.9.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morningstar_data"
-version = "1.9.5"
+version = "1.9.6"
 description = "Morningstar Data"
 authors = ["Morningstar, Inc."]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.morningstar.com/products/md-python-package"
 documentation = "https://docs-analyticslab.morningstar.com/latest/index.html"
```

### Comparing `morningstar_data-1.9.5/PKG-INFO` & `morningstar_data-1.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morningstar-data
-Version: 1.9.5
+Version: 1.9.6
 Summary: Morningstar Data
 Home-page: https://www.morningstar.com/products/md-python-package
 License: Apache-2.0
 Author: Morningstar, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

