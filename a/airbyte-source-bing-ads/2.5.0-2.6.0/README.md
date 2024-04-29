# Comparing `tmp/airbyte_source_bing_ads-2.5.0.tar.gz` & `tmp/airbyte_source_bing_ads-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_bing_ads-2.5.0.tar", max compression
+gzip compressed data, was "airbyte_source_bing_ads-2.6.0.tar", max compression
```

## Comparing `airbyte_source_bing_ads-2.5.0.tar` & `airbyte_source_bing_ads-2.6.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     4532 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/README.md
--rw-r--r--   0        0        0      865 2024-03-29 14:48:28.539552 airbyte_source_bing_ads-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/__init__.py
--rw-r--r--   0        0        0    14454 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/base_streams.py
--rw-r--r--   0        0        0     7851 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/bulk_streams.py
--rw-r--r--   0        0        0    11425 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/client.py
--rw-r--r--   0        0        0    32975 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/report_streams.py
--rw-r--r--   0        0        0      234 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/run.py
--rw-r--r--   0        0        0     5723 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/account_impression_performance_report.json
--rw-r--r--   0        0        0     4545 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/account_impression_performance_report_hourly.json
--rw-r--r--   0        0        0     2532 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/account_performance_report.json
--rw-r--r--   0        0        0     2586 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/account_performance_report_hourly.json
--rw-r--r--   0        0        0     3550 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/accounts.json
--rw-r--r--   0        0        0     6540 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_impression_performance_report.json
--rw-r--r--   0        0        0     5159 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_impression_performance_report_hourly.json
--rw-r--r--   0        0        0      648 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_labels.json
--rw-r--r--   0        0        0     3547 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_performance_report.json
--rw-r--r--   0        0        0     3306 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_performance_report_hourly.json
--rw-r--r--   0        0        0     3618 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_groups.json
--rw-r--r--   0        0        0     3300 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_performance_report.json
--rw-r--r--   0        0        0     3198 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_performance_report_hourly.json
--rw-r--r--   0        0        0     8896 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ads.json
--rw-r--r--   0        0        0     2274 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/age_gender_audience_report.json
--rw-r--r--   0        0        0     2328 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/age_gender_audience_report_hourly.json
--rw-r--r--   0        0        0      532 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/app_install_ad_labels.json
--rw-r--r--   0        0        0     1490 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/app_install_ads.json
--rw-r--r--   0        0        0     3244 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/audience_performance_report.json
--rw-r--r--   0        0        0     3298 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/audience_performance_report_hourly.json
--rw-r--r--   0        0        0      825 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/budget.json
--rw-r--r--   0        0        0      675 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/budget_summary_report.json
--rw-r--r--   0        0        0     6912 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_impression_performance_report.json
--rw-r--r--   0        0        0     5456 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_impression_performance_report_hourly.json
--rw-r--r--   0        0        0      590 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_labels.json
--rw-r--r--   0        0        0     4008 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_performance_report.json
--rw-r--r--   0        0        0     3767 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_performance_report_hourly.json
--rw-r--r--   0        0        0     3521 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaigns.json
--rw-r--r--   0        0        0     4445 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/geographic_performance_report.json
--rw-r--r--   0        0        0     4499 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/geographic_performance_report_hourly.json
--rw-r--r--   0        0        0     1779 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/goals_and_funnels_report.json
--rw-r--r--   0        0        0     1833 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/goals_and_funnels_report_hourly.json
--rw-r--r--   0        0        0      532 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keyword_labels.json
--rw-r--r--   0        0        0     3733 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keyword_performance_report.json
--rw-r--r--   0        0        0     3996 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keyword_performance_report_daily.json
--rw-r--r--   0        0        0     3787 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keyword_performance_report_hourly.json
--rw-r--r--   0        0        0     2210 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keywords.json
--rw-r--r--   0        0        0      643 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/labels.json
--rw-r--r--   0        0        0     5371 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/product_dimension_performance_report.json
--rw-r--r--   0        0        0     5425 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/product_dimension_performance_report_hourly.json
--rw-r--r--   0        0        0     3656 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/product_search_query_performance_report.json
--rw-r--r--   0        0        0     3710 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/product_search_query_performance_report_hourly.json
--rw-r--r--   0        0        0     3752 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/search_query_performance_report.json
--rw-r--r--   0        0        0     3806 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/search_query_performance_report_hourly.json
--rw-r--r--   0        0        0     4511 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/user_location_performance_report.json
--rw-r--r--   0        0        0     4565 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/user_location_performance_report_hourly.json
--rw-r--r--   0        0        0     7578 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/source.py
--rw-r--r--   0        0        0     9533 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/spec.json
--rw-r--r--   0        0        0     1207 2024-03-29 10:28:47.000000 airbyte_source_bing_ads-2.5.0/source_bing_ads/utils.py
--rw-r--r--   0        0        0     5385 1970-01-01 00:00:00.000000 airbyte_source_bing_ads-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     4532 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/README.md
+-rw-r--r--   0        0        0      865 2024-04-29 15:48:11.141847 airbyte_source_bing_ads-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/__init__.py
+-rw-r--r--   0        0        0    14454 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/base_streams.py
+-rw-r--r--   0        0        0     7851 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/bulk_streams.py
+-rw-r--r--   0        0        0    11425 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/client.py
+-rw-r--r--   0        0        0    32975 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/report_streams.py
+-rw-r--r--   0        0        0      234 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/run.py
+-rw-r--r--   0        0        0     5723 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_impression_performance_report.json
+-rw-r--r--   0        0        0     4545 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_impression_performance_report_hourly.json
+-rw-r--r--   0        0        0     2532 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_performance_report.json
+-rw-r--r--   0        0        0     2586 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_performance_report_hourly.json
+-rw-r--r--   0        0        0     3550 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/accounts.json
+-rw-r--r--   0        0        0     6540 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_impression_performance_report.json
+-rw-r--r--   0        0        0     5159 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_impression_performance_report_hourly.json
+-rw-r--r--   0        0        0      648 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_labels.json
+-rw-r--r--   0        0        0     3547 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_performance_report.json
+-rw-r--r--   0        0        0     3306 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_performance_report_hourly.json
+-rw-r--r--   0        0        0     3618 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_groups.json
+-rw-r--r--   0        0        0     3300 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_performance_report.json
+-rw-r--r--   0        0        0     3198 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_performance_report_hourly.json
+-rw-r--r--   0        0        0     8896 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ads.json
+-rw-r--r--   0        0        0     2274 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/age_gender_audience_report.json
+-rw-r--r--   0        0        0     2328 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/age_gender_audience_report_hourly.json
+-rw-r--r--   0        0        0      532 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/app_install_ad_labels.json
+-rw-r--r--   0        0        0     1490 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/app_install_ads.json
+-rw-r--r--   0        0        0     3244 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/audience_performance_report.json
+-rw-r--r--   0        0        0     3298 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/audience_performance_report_hourly.json
+-rw-r--r--   0        0        0      825 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/budget.json
+-rw-r--r--   0        0        0      675 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/budget_summary_report.json
+-rw-r--r--   0        0        0     6912 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_impression_performance_report.json
+-rw-r--r--   0        0        0     5456 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_impression_performance_report_hourly.json
+-rw-r--r--   0        0        0      590 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_labels.json
+-rw-r--r--   0        0        0     4008 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_performance_report.json
+-rw-r--r--   0        0        0     3767 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_performance_report_hourly.json
+-rw-r--r--   0        0        0     3521 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaigns.json
+-rw-r--r--   0        0        0     4445 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/geographic_performance_report.json
+-rw-r--r--   0        0        0     4499 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/geographic_performance_report_hourly.json
+-rw-r--r--   0        0        0     1779 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/goals_and_funnels_report.json
+-rw-r--r--   0        0        0     1833 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/goals_and_funnels_report_hourly.json
+-rw-r--r--   0        0        0      532 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_labels.json
+-rw-r--r--   0        0        0     4755 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report.json
+-rw-r--r--   0        0        0     5018 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report_daily.json
+-rw-r--r--   0        0        0     4809 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report_hourly.json
+-rw-r--r--   0        0        0     2210 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keywords.json
+-rw-r--r--   0        0        0      643 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/labels.json
+-rw-r--r--   0        0        0     5371 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_dimension_performance_report.json
+-rw-r--r--   0        0        0     5425 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_dimension_performance_report_hourly.json
+-rw-r--r--   0        0        0     3656 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_search_query_performance_report.json
+-rw-r--r--   0        0        0     3710 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_search_query_performance_report_hourly.json
+-rw-r--r--   0        0        0     3752 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/search_query_performance_report.json
+-rw-r--r--   0        0        0     3806 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/search_query_performance_report_hourly.json
+-rw-r--r--   0        0        0     4511 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/user_location_performance_report.json
+-rw-r--r--   0        0        0     4565 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/user_location_performance_report_hourly.json
+-rw-r--r--   0        0        0     7578 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/source.py
+-rw-r--r--   0        0        0     9533 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/spec.json
+-rw-r--r--   0        0        0     1207 2024-04-29 14:12:42.000000 airbyte_source_bing_ads-2.6.0/source_bing_ads/utils.py
+-rw-r--r--   0        0        0     5385 1970-01-01 00:00:00.000000 airbyte_source_bing_ads-2.6.0/PKG-INFO
```

### Comparing `airbyte_source_bing_ads-2.5.0/README.md` & `airbyte_source_bing_ads-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/pyproject.toml` & `airbyte_source_bing_ads-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.5.0"
+version = "2.6.0"
 name = "airbyte-source-bing-ads"
 description = "Source implementation for Bing Ads."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/__init__.py` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/base_streams.py` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/base_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/bulk_streams.py` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/bulk_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/client.py` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/client.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/report_streams.py` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/report_streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/account_impression_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_impression_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/account_impression_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_impression_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/account_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/account_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/account_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/accounts.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_impression_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_impression_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_impression_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_impression_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_labels.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_group_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_group_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_groups.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ad_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ad_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/ads.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/age_gender_audience_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/age_gender_audience_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/age_gender_audience_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/age_gender_audience_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/app_install_ad_labels.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/app_install_ad_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/app_install_ads.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/app_install_ads.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/audience_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/audience_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/audience_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/audience_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/budget.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/budget.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/budget_summary_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/budget_summary_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_impression_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_impression_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_impression_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_impression_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_labels.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaign_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaign_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/campaigns.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/geographic_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/geographic_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/geographic_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/geographic_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/goals_and_funnels_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/goals_and_funnels_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/goals_and_funnels_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/goals_and_funnels_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keyword_labels.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keyword_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/search_query_performance_report_hourly.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5685529279279279%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{'TimePeriod': {'format': 'date-time', 'airbyte_type': "*

 * *                 "'timestamp_with_timezone'}, 'Conversions': {'type': {insert: [(1, 'integer')], "*

 * *                 "delete: [1]}}, 'AccountNumber': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'AdType': OrderedDict([('type', ['null', 'string'])]), 'DestinationUrl': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'CampaignStatus': "*

 * *      […]*

```diff
@@ -1,24 +1,41 @@
 {
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": true,
+    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
+        "AbsoluteTopImpressionRatePercent": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "AccountId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdDistribution": {
+        "AccountNumber": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "AccountStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "AdGroupCriterionId": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupId": {
             "type": [
@@ -28,38 +45,56 @@
         },
         "AdGroupName": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "AdGroupStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "AdId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AdRelevance": {
+        "AdStatus": {
             "type": [
                 "null",
-                "number"
+                "string"
+            ]
+        },
+        "AdType": {
+            "type": [
+                "null",
+                "string"
             ]
         },
         "AllConversionRate": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllConversions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
+        "AllConversionsQualified": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "AllCostPerConversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllReturnOnAdSpend": {
@@ -118,14 +153,26 @@
         },
         "CampaignName": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "CampaignStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "CampaignType": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "Clicks": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionRate": {
@@ -133,15 +180,15 @@
                 "null",
                 "number"
             ]
         },
         "Conversions": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "ConversionsQualified": {
             "type": [
                 "null",
                 "number"
             ]
@@ -160,74 +207,62 @@
         },
         "Ctr": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CurrencyCode": {
+        "CustomerId": {
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "CurrentMaxCpc": {
-            "type": [
-                "null",
-                "number"
+                "integer"
             ]
         },
-        "CustomParameters": {
+        "CustomerName": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "DeliveredMatchType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceOS": {
+        "DestinationUrl": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceType": {
+        "DeviceOS": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ExpectedCtr": {
+        "DeviceType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FinalAppUrl": {
+        "Goal": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FinalUrlSuffix": {
+        "GoalType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FirstPageBid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Impressions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "Keyword": {
@@ -244,56 +279,26 @@
         },
         "KeywordStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "LandingPageExperience": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Language": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Mainline1Bid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "MainlineBid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Network": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "QualityImpact": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "QualityScore": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "ReturnOnAdSpend": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "Revenue": {
@@ -310,41 +315,42 @@
         },
         "RevenuePerConversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Spend": {
+        "SearchQuery": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "TimePeriod": {
-            "format": "date",
+        "Spend": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "TopVsOther": {
+        "TimePeriod": {
+            "airbyte_type": "timestamp_with_timezone",
+            "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ViewThroughConversions": {
+        "TopImpressionRatePercent": {
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "ViewThroughConversionsQualified": {
+        "TopVsOther": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keyword_performance_report_daily.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report_daily.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9653679653679653%*

 * *Differences: {"'properties'": "{'CampaignStatus': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'TopImpressionRatePercent': OrderedDict([('type', ['null', 'number'])]), "*

 * *                 "'AdGroupStatus': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'TrackingTemplate': OrderedDict([('type', ['null', 'string'])]), "*

 * *                 "'BidStrategyType': OrderedDict([('type', ['null', 'string'])]), 'AccountStatus': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'Fin […]*

```diff
@@ -1,22 +1,40 @@
 {
     "$schema": "http://json-schema.org/draft-07/schema#",
     "properties": {
+        "AbsoluteTopImpressionRatePercent": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "AccountId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "AccountNumber": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "AccountStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "AdDistribution": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupId": {
@@ -27,26 +45,38 @@
         },
         "AdGroupName": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "AdGroupStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "AdId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AdRelevance": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "AdType": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "AllConversionRate": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllConversions": {
@@ -99,32 +129,50 @@
         },
         "AveragePosition": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "BaseCampaignId": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
         "BidMatchType": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "BidStrategyType": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "CampaignId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "CampaignName": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "CampaignStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "Clicks": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionRate": {
@@ -183,14 +231,20 @@
         },
         "DeliveredMatchType": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "DestinationUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "DeviceOS": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "DeviceType": {
@@ -207,26 +261,50 @@
         },
         "FinalAppUrl": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "FinalMobileUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "FinalUrlSuffix": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "FirstPageBid": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "Goal": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "GoalType": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "HistoricalAdRelevance": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "HistoricalExpectedCtr": {
@@ -261,14 +339,20 @@
         },
         "KeywordId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
+        "KeywordLabels": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "KeywordStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "LandingPageExperience": {
@@ -346,20 +430,32 @@
         "TimePeriod": {
             "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
+        "TopImpressionRatePercent": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "TopVsOther": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "TrackingTemplate": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "ViewThroughConversions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ViewThroughConversionsQualified": {
```

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keyword_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/search_query_performance_report.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5685529279279279%*

 * *Differences: {"'$schema'": "'https://json-schema.org/draft-07/schema#'",*

 * * "'properties'": "{'TimePeriod': {'format': 'date', delete: ['airbyte_type']}, 'Conversions': "*

 * *                 "{'type': {insert: [(1, 'integer')], delete: [1]}}, 'AccountNumber': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'AdType': OrderedDict([('type', "*

 * *                 "['null', 'string'])]), 'DestinationUrl': OrderedDict([('type', ['null', "*

 * *                 "'string'])]), 'CampaignStatus': OrderedDict([('type', ['null' […]*

```diff
@@ -1,24 +1,41 @@
 {
-    "$schema": "http://json-schema.org/draft-07/schema#",
-    "additionalProperties": true,
+    "$schema": "https://json-schema.org/draft-07/schema#",
     "properties": {
+        "AbsoluteTopImpressionRatePercent": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "AccountId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "AccountName": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdDistribution": {
+        "AccountNumber": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "AccountStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "AdGroupCriterionId": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupId": {
             "type": [
@@ -28,38 +45,56 @@
         },
         "AdGroupName": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "AdGroupStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "AdId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AdRelevance": {
+        "AdStatus": {
             "type": [
                 "null",
-                "number"
+                "string"
+            ]
+        },
+        "AdType": {
+            "type": [
+                "null",
+                "string"
             ]
         },
         "AllConversionRate": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllConversions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
+        "AllConversionsQualified": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "AllCostPerConversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllReturnOnAdSpend": {
@@ -118,14 +153,26 @@
         },
         "CampaignName": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "CampaignStatus": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "CampaignType": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "Clicks": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "ConversionRate": {
@@ -133,15 +180,15 @@
                 "null",
                 "number"
             ]
         },
         "Conversions": {
             "type": [
                 "null",
-                "number"
+                "integer"
             ]
         },
         "ConversionsQualified": {
             "type": [
                 "null",
                 "number"
             ]
@@ -160,74 +207,62 @@
         },
         "Ctr": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CurrencyCode": {
+        "CustomerId": {
             "type": [
                 "null",
-                "string"
-            ]
-        },
-        "CurrentMaxCpc": {
-            "type": [
-                "null",
-                "number"
+                "integer"
             ]
         },
-        "CustomParameters": {
+        "CustomerName": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "DeliveredMatchType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceOS": {
+        "DestinationUrl": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "DeviceType": {
+        "DeviceOS": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ExpectedCtr": {
+        "DeviceType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FinalAppUrl": {
+        "Goal": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FinalUrlSuffix": {
+        "GoalType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "FirstPageBid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Impressions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
         "Keyword": {
@@ -244,56 +279,26 @@
         },
         "KeywordStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "LandingPageExperience": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Language": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "Mainline1Bid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "MainlineBid": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "Network": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "QualityImpact": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
-        "QualityScore": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "ReturnOnAdSpend": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "Revenue": {
@@ -310,42 +315,41 @@
         },
         "RevenuePerConversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Spend": {
+        "SearchQuery": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         },
-        "TimePeriod": {
-            "airbyte_type": "timestamp_with_timezone",
-            "format": "date-time",
+        "Spend": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
-        "TopVsOther": {
+        "TimePeriod": {
+            "format": "date",
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ViewThroughConversions": {
+        "TopImpressionRatePercent": {
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
-        "ViewThroughConversionsQualified": {
+        "TopVsOther": {
             "type": [
                 "null",
-                "number"
+                "string"
             ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/keywords.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keywords.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/labels.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/labels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/product_dimension_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_dimension_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/product_dimension_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_dimension_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/product_search_query_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_search_query_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/product_search_query_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/product_search_query_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/search_query_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5794270833333333%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'additionalProperties'": 'True',*

 * * "'properties'": "{'Conversions': {'type': {insert: [(1, 'number')], delete: [1]}}, "*

 * *                 "'CurrencyCode': OrderedDict([('type', ['null', 'string'])]), 'AdDistribution': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'CurrentMaxCpc': "*

 * *                 "OrderedDict([('type', ['null', 'number'])]), 'QualityScore': "*

 * *                 "OrderedDict([('type', ['null', 'number'])]), 'Expect […]*

```diff
@@ -1,9 +1,10 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": true,
     "properties": {
         "AbsoluteTopImpressionRatePercent": {
             "type": [
                 "null",
                 "number"
             ]
         },
@@ -27,15 +28,15 @@
         },
         "AccountStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdGroupCriterionId": {
+        "AdDistribution": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupId": {
             "type": [
@@ -57,18 +58,18 @@
         },
         "AdId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AdStatus": {
+        "AdRelevance": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
         "AdType": {
             "type": [
                 "null",
                 "string"
             ]
@@ -81,20 +82,14 @@
         },
         "AllConversions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AllConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AllCostPerConversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllReturnOnAdSpend": {
@@ -135,39 +130,45 @@
         },
         "AveragePosition": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "BaseCampaignId": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
         "BidMatchType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CampaignId": {
+        "BidStrategyType": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "CampaignName": {
+        "CampaignId": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "CampaignStatus": {
+        "CampaignName": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CampaignType": {
+        "CampaignStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "Clicks": {
             "type": [
@@ -180,15 +181,15 @@
                 "null",
                 "number"
             ]
         },
         "Conversions": {
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
         "ConversionsQualified": {
             "type": [
                 "null",
                 "number"
             ]
@@ -207,21 +208,27 @@
         },
         "Ctr": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CustomerId": {
+        "CurrencyCode": {
             "type": [
                 "null",
-                "integer"
+                "string"
+            ]
+        },
+        "CurrentMaxCpc": {
+            "type": [
+                "null",
+                "number"
             ]
         },
-        "CustomerName": {
+        "CustomParameters": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "DeliveredMatchType": {
             "type": [
@@ -243,14 +250,50 @@
         },
         "DeviceType": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "ExpectedCtr": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalAppUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalMobileUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalUrlSuffix": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FirstPageBid": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "Goal": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "GoalType": {
@@ -273,60 +316,90 @@
         },
         "KeywordId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
+        "KeywordLabels": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "KeywordStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "LandingPageExperience": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "Language": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "Mainline1Bid": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "MainlineBid": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "Network": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ReturnOnAdSpend": {
+        "QualityImpact": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Revenue": {
+        "QualityScore": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerAssist": {
+        "ReturnOnAdSpend": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerConversion": {
+        "Revenue": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "SearchQuery": {
+        "RevenuePerAssist": {
             "type": [
                 "null",
-                "string"
+                "number"
+            ]
+        },
+        "RevenuePerConversion": {
+            "type": [
+                "null",
+                "number"
             ]
         },
         "Spend": {
             "type": [
                 "null",
                 "number"
             ]
@@ -345,11 +418,29 @@
             ]
         },
         "TopVsOther": {
             "type": [
                 "null",
                 "string"
             ]
+        },
+        "TrackingTemplate": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ViewThroughConversions": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "ViewThroughConversionsQualified": {
+            "type": [
+                "null",
+                "number"
+            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/search_query_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/keyword_performance_report_hourly.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5794270833333333%*

 * *Differences: {"'$schema'": "'http://json-schema.org/draft-07/schema#'",*

 * * "'additionalProperties'": 'True',*

 * * "'properties'": "{'Conversions': {'type': {insert: [(1, 'number')], delete: [1]}}, "*

 * *                 "'CurrencyCode': OrderedDict([('type', ['null', 'string'])]), 'AdDistribution': "*

 * *                 "OrderedDict([('type', ['null', 'string'])]), 'CurrentMaxCpc': "*

 * *                 "OrderedDict([('type', ['null', 'number'])]), 'QualityScore': "*

 * *                 "OrderedDict([('type', ['null', 'number'])]), 'Expect […]*

```diff
@@ -1,9 +1,10 @@
 {
-    "$schema": "https://json-schema.org/draft-07/schema#",
+    "$schema": "http://json-schema.org/draft-07/schema#",
+    "additionalProperties": true,
     "properties": {
         "AbsoluteTopImpressionRatePercent": {
             "type": [
                 "null",
                 "number"
             ]
         },
@@ -27,15 +28,15 @@
         },
         "AccountStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "AdGroupCriterionId": {
+        "AdDistribution": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "AdGroupId": {
             "type": [
@@ -57,18 +58,18 @@
         },
         "AdId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AdStatus": {
+        "AdRelevance": {
             "type": [
                 "null",
-                "string"
+                "number"
             ]
         },
         "AdType": {
             "type": [
                 "null",
                 "string"
             ]
@@ -81,20 +82,14 @@
         },
         "AllConversions": {
             "type": [
                 "null",
                 "integer"
             ]
         },
-        "AllConversionsQualified": {
-            "type": [
-                "null",
-                "number"
-            ]
-        },
         "AllCostPerConversion": {
             "type": [
                 "null",
                 "number"
             ]
         },
         "AllReturnOnAdSpend": {
@@ -135,39 +130,45 @@
         },
         "AveragePosition": {
             "type": [
                 "null",
                 "number"
             ]
         },
+        "BaseCampaignId": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
         "BidMatchType": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CampaignId": {
+        "BidStrategyType": {
             "type": [
                 "null",
-                "integer"
+                "string"
             ]
         },
-        "CampaignName": {
+        "CampaignId": {
             "type": [
                 "null",
-                "string"
+                "integer"
             ]
         },
-        "CampaignStatus": {
+        "CampaignName": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "CampaignType": {
+        "CampaignStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "Clicks": {
             "type": [
@@ -180,15 +181,15 @@
                 "null",
                 "number"
             ]
         },
         "Conversions": {
             "type": [
                 "null",
-                "integer"
+                "number"
             ]
         },
         "ConversionsQualified": {
             "type": [
                 "null",
                 "number"
             ]
@@ -207,21 +208,27 @@
         },
         "Ctr": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "CustomerId": {
+        "CurrencyCode": {
             "type": [
                 "null",
-                "integer"
+                "string"
+            ]
+        },
+        "CurrentMaxCpc": {
+            "type": [
+                "null",
+                "number"
             ]
         },
-        "CustomerName": {
+        "CustomParameters": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "DeliveredMatchType": {
             "type": [
@@ -243,14 +250,50 @@
         },
         "DeviceType": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "ExpectedCtr": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalAppUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalMobileUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalUrl": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FinalUrlSuffix": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "FirstPageBid": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "Goal": {
             "type": [
                 "null",
                 "string"
             ]
         },
         "GoalType": {
@@ -273,60 +316,90 @@
         },
         "KeywordId": {
             "type": [
                 "null",
                 "integer"
             ]
         },
+        "KeywordLabels": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "KeywordStatus": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "LandingPageExperience": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "Language": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "Mainline1Bid": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
+        "MainlineBid": {
+            "type": [
+                "null",
+                "number"
+            ]
+        },
         "Network": {
             "type": [
                 "null",
                 "string"
             ]
         },
-        "ReturnOnAdSpend": {
+        "QualityImpact": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "Revenue": {
+        "QualityScore": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerAssist": {
+        "ReturnOnAdSpend": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "RevenuePerConversion": {
+        "Revenue": {
             "type": [
                 "null",
                 "number"
             ]
         },
-        "SearchQuery": {
+        "RevenuePerAssist": {
             "type": [
                 "null",
-                "string"
+                "number"
+            ]
+        },
+        "RevenuePerConversion": {
+            "type": [
+                "null",
+                "number"
             ]
         },
         "Spend": {
             "type": [
                 "null",
                 "number"
             ]
@@ -346,11 +419,29 @@
             ]
         },
         "TopVsOther": {
             "type": [
                 "null",
                 "string"
             ]
+        },
+        "TrackingTemplate": {
+            "type": [
+                "null",
+                "string"
+            ]
+        },
+        "ViewThroughConversions": {
+            "type": [
+                "null",
+                "integer"
+            ]
+        },
+        "ViewThroughConversionsQualified": {
+            "type": [
+                "null",
+                "number"
+            ]
         }
     },
     "type": "object"
 }
```

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/user_location_performance_report.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/user_location_performance_report.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/schemas/user_location_performance_report_hourly.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/schemas/user_location_performance_report_hourly.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/source.py` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/spec.json` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/source_bing_ads/utils.py` & `airbyte_source_bing_ads-2.6.0/source_bing_ads/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_bing_ads-2.5.0/PKG-INFO` & `airbyte_source_bing_ads-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-bing-ads
-Version: 2.5.0
+Version: 2.6.0
 Summary: Source implementation for Bing Ads.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

