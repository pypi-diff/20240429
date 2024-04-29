# Comparing `tmp/fds.sdk.FactSetESG-1.2.3-py3-none-any.whl.zip` & `tmp/fds.sdk.FactSetESG-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,71 +1,51 @@
-Zip file size: 311238 bytes, number of entries: 69
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 14:48 fds/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-08 14:48 fds/sdk/__init__.py
--rw-r--r--  2.0 unx     1559 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/__init__.py
--rw-r--r--  2.0 unx    40554 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/api_client.py
--rw-r--r--  2.0 unx    19130 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/configuration.py
--rw-r--r--  2.0 unx     5849 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/exceptions.py
--rw-r--r--  2.0 unx    83237 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model_utils.py
--rw-r--r--  2.0 unx    14977 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/rest.py
--rw-r--r--  2.0 unx      223 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/api/__init__.py
--rw-r--r--  2.0 unx   192999 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/api/articles_api.py
--rw-r--r--  2.0 unx   219451 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/api/sasb_api.py
--rw-r--r--  2.0 unx    94994 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/api/sdg_api.py
--rw-r--r--  2.0 unx    47995 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/api/sfdr_api.py
--rw-r--r--  2.0 unx   224913 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/api/spotlights_api.py
--rw-r--r--  2.0 unx      693 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/apis/__init__.py
--rw-r--r--  2.0 unx      348 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/__init__.py
--rw-r--r--  2.0 unx    15863 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/articles_fields.py
--rw-r--r--  2.0 unx    12840 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/calendar.py
--rw-r--r--  2.0 unx    88611 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/categories.py
--rw-r--r--  2.0 unx    12908 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/date_of.py
--rw-r--r--  2.0 unx    13135 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/error_response.py
--rw-r--r--  2.0 unx    12618 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/error_response_sub_errors.py
--rw-r--r--  2.0 unx    15121 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/fields_sasb_spotlights.py
--rw-r--r--  2.0 unx    27542 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/fields_sdg_spotlights.py
--rw-r--r--  2.0 unx    13252 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/frequency.py
--rw-r--r--  2.0 unx    13994 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/ids.py
--rw-r--r--  2.0 unx    21833 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/indicators.py
--rw-r--r--  2.0 unx    13787 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/pai_ids.py
--rw-r--r--  2.0 unx    14674 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/rank_categories.py
--rw-r--r--  2.0 unx    12763 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_article.py
--rw-r--r--  2.0 unx    87145 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_articles_categories.py
--rw-r--r--  2.0 unx    14273 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_articles_request.py
--rw-r--r--  2.0 unx    12083 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_articles_response.py
--rw-r--r--  2.0 unx    13737 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_ranks.py
--rw-r--r--  2.0 unx    14393 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_ranks_request.py
--rw-r--r--  2.0 unx    12064 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_ranks_response.py
--rw-r--r--  2.0 unx    25814 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_score_types.py
--rw-r--r--  2.0 unx    14467 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_scores.py
--rw-r--r--  2.0 unx    25603 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_scores_all.py
--rw-r--r--  2.0 unx    14410 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_scores_all_request.py
--rw-r--r--  2.0 unx    12115 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_scores_all_response.py
--rw-r--r--  2.0 unx    14734 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_scores_request.py
--rw-r--r--  2.0 unx    12076 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_scores_response.py
--rw-r--r--  2.0 unx    88551 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_spotlights_categories.py
--rw-r--r--  2.0 unx    15200 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sasb_spotlights_request.py
--rw-r--r--  2.0 unx    12762 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_article.py
--rw-r--r--  2.0 unx    56820 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_articles_categories.py
--rw-r--r--  2.0 unx    14263 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_articles_request.py
--rw-r--r--  2.0 unx    12081 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_articles_response.py
--rw-r--r--  2.0 unx    58524 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_categories.py
--rw-r--r--  2.0 unx    13313 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_frequency.py
--rw-r--r--  2.0 unx    24615 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_score_types.py
--rw-r--r--  2.0 unx    13473 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_scores.py
--rw-r--r--  2.0 unx    14191 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_scores_request.py
--rw-r--r--  2.0 unx    12064 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_scores_response.py
--rw-r--r--  2.0 unx    57491 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_spotlight_categories.py
--rw-r--r--  2.0 unx    15176 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sdg_spotlights_request.py
--rw-r--r--  2.0 unx    15179 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sfdr_pai.py
--rw-r--r--  2.0 unx    14959 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sfdr_pai_request.py
--rw-r--r--  2.0 unx    12056 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/sfdr_pai_response.py
--rw-r--r--  2.0 unx    12814 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/spotlights.py
--rw-r--r--  2.0 unx    12071 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/spotlights_response.py
--rw-r--r--  2.0 unx    14047 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/model/tvl_ids.py
--rw-r--r--  2.0 unx     3655 b- defN 24-Apr-08 14:48 fds/sdk/FactSetESG/models/__init__.py
--rw-r--r--  2.0 unx    11358 b- defN 24-Apr-08 14:48 fds.sdk.FactSetESG-1.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    42800 b- defN 24-Apr-08 14:48 fds.sdk.FactSetESG-1.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-08 14:48 fds.sdk.FactSetESG-1.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Apr-08 14:48 fds.sdk.FactSetESG-1.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     6755 b- defN 24-Apr-08 14:48 fds.sdk.FactSetESG-1.2.3.dist-info/RECORD
-69 files, 2063091 bytes uncompressed, 300314 bytes compressed:  85.4%
+Zip file size: 211073 bytes, number of entries: 49
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 09:18 fds/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-29 09:18 fds/sdk/__init__.py
+-rw-r--r--  2.0 unx     1559 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/__init__.py
+-rw-r--r--  2.0 unx    40554 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/api_client.py
+-rw-r--r--  2.0 unx    19130 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/configuration.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/exceptions.py
+-rw-r--r--  2.0 unx    83237 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model_utils.py
+-rw-r--r--  2.0 unx    14977 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/rest.py
+-rw-r--r--  2.0 unx      223 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/api/__init__.py
+-rw-r--r--  2.0 unx   112412 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/api/articles_api.py
+-rw-r--r--  2.0 unx   219451 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/api/sasb_api.py
+-rw-r--r--  2.0 unx   128682 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/api/spotlights_api.py
+-rw-r--r--  2.0 unx      591 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/apis/__init__.py
+-rw-r--r--  2.0 unx      348 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/__init__.py
+-rw-r--r--  2.0 unx    15863 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/articles_fields.py
+-rw-r--r--  2.0 unx    12840 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/calendar.py
+-rw-r--r--  2.0 unx    88611 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/categories.py
+-rw-r--r--  2.0 unx    12908 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/date_of.py
+-rw-r--r--  2.0 unx    13135 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/error_response.py
+-rw-r--r--  2.0 unx    12618 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/error_response_sub_errors.py
+-rw-r--r--  2.0 unx    15121 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/fields_sasb_spotlights.py
+-rw-r--r--  2.0 unx    13240 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/frequency.py
+-rw-r--r--  2.0 unx    13994 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/ids.py
+-rw-r--r--  2.0 unx    13787 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/pai_ids.py
+-rw-r--r--  2.0 unx    14674 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/rank_categories.py
+-rw-r--r--  2.0 unx    12763 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_article.py
+-rw-r--r--  2.0 unx    87145 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_articles_categories.py
+-rw-r--r--  2.0 unx    14273 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_articles_request.py
+-rw-r--r--  2.0 unx    12083 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_articles_response.py
+-rw-r--r--  2.0 unx    13737 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_ranks.py
+-rw-r--r--  2.0 unx    14393 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_ranks_request.py
+-rw-r--r--  2.0 unx    12064 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_ranks_response.py
+-rw-r--r--  2.0 unx    25814 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_score_types.py
+-rw-r--r--  2.0 unx    14275 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_scores.py
+-rw-r--r--  2.0 unx    25219 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_scores_all.py
+-rw-r--r--  2.0 unx    14410 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_scores_all_request.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_scores_all_response.py
+-rw-r--r--  2.0 unx    14734 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_scores_request.py
+-rw-r--r--  2.0 unx    12076 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_scores_response.py
+-rw-r--r--  2.0 unx    88551 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_spotlights_categories.py
+-rw-r--r--  2.0 unx    15200 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/sasb_spotlights_request.py
+-rw-r--r--  2.0 unx    12814 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/spotlights.py
+-rw-r--r--  2.0 unx    12071 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/model/spotlights_response.py
+-rw-r--r--  2.0 unx     2403 b- defN 24-Apr-29 09:18 fds/sdk/FactSetESG/models/__init__.py
+-rw-r--r--  2.0 unx    11358 b- defN 24-Apr-29 09:18 fds.sdk.FactSetESG-1.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    38133 b- defN 24-Apr-29 09:18 fds.sdk.FactSetESG-1.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 09:18 fds.sdk.FactSetESG-1.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-29 09:18 fds.sdk.FactSetESG-1.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4735 b- defN 24-Apr-29 09:18 fds.sdk.FactSetESG-1.3.0.dist-info/RECORD
+49 files, 1324266 bytes uncompressed, 203389 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -27,20 +27,14 @@
 
 Filename: fds/sdk/FactSetESG/api/articles_api.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/api/sasb_api.py
 Comment: 
 
-Filename: fds/sdk/FactSetESG/api/sdg_api.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/api/sfdr_api.py
-Comment: 
-
 Filename: fds/sdk/FactSetESG/api/spotlights_api.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/apis/__init__.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/model/__init__.py
@@ -63,26 +57,20 @@
 
 Filename: fds/sdk/FactSetESG/model/error_response_sub_errors.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/model/fields_sasb_spotlights.py
 Comment: 
 
-Filename: fds/sdk/FactSetESG/model/fields_sdg_spotlights.py
-Comment: 
-
 Filename: fds/sdk/FactSetESG/model/frequency.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/model/ids.py
 Comment: 
 
-Filename: fds/sdk/FactSetESG/model/indicators.py
-Comment: 
-
 Filename: fds/sdk/FactSetESG/model/pai_ids.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/model/rank_categories.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/model/sasb_article.py
@@ -129,80 +117,32 @@
 
 Filename: fds/sdk/FactSetESG/model/sasb_spotlights_categories.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/model/sasb_spotlights_request.py
 Comment: 
 
-Filename: fds/sdk/FactSetESG/model/sdg_article.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_articles_categories.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_articles_request.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_articles_response.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_categories.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_frequency.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_score_types.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_scores.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_scores_request.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_scores_response.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_spotlight_categories.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sdg_spotlights_request.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sfdr_pai.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sfdr_pai_request.py
-Comment: 
-
-Filename: fds/sdk/FactSetESG/model/sfdr_pai_response.py
-Comment: 
-
 Filename: fds/sdk/FactSetESG/model/spotlights.py
 Comment: 
 
 Filename: fds/sdk/FactSetESG/model/spotlights_response.py
 Comment: 
 
-Filename: fds/sdk/FactSetESG/model/tvl_ids.py
-Comment: 
-
 Filename: fds/sdk/FactSetESG/models/__init__.py
 Comment: 
 
-Filename: fds.sdk.FactSetESG-1.2.3.dist-info/LICENSE
+Filename: fds.sdk.FactSetESG-1.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: fds.sdk.FactSetESG-1.2.3.dist-info/METADATA
+Filename: fds.sdk.FactSetESG-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: fds.sdk.FactSetESG-1.2.3.dist-info/WHEEL
+Filename: fds.sdk.FactSetESG-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: fds.sdk.FactSetESG-1.2.3.dist-info/top_level.txt
+Filename: fds.sdk.FactSetESG-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fds.sdk.FactSetESG-1.2.3.dist-info/RECORD
+Filename: fds.sdk.FactSetESG-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fds/sdk/FactSetESG/__init__.py

```diff
@@ -1,21 +1,21 @@
 # flake8: noqa
 
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.2.3"
+__version__ = "1.3.0"
 
 # import ApiClient
 from fds.sdk.FactSetESG.api_client import ApiClient
 
 # import Configuration
 from fds.sdk.FactSetESG.configuration import Configuration
```

## fds/sdk/FactSetESG/api_client.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
@@ -102,15 +102,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'fds-sdk/python/FactSetESG/1.2.3'
+        self.user_agent = 'fds-sdk/python/FactSetESG/1.3.0'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

## fds/sdk/FactSetESG/configuration.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
@@ -425,16 +425,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.6.0\n"\
-               "SDK Package Version: 1.2.3".\
+               "Version of the API: 1.7.0\n"\
+               "SDK Package Version: 1.3.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

## fds/sdk/FactSetESG/exceptions.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
```

## fds/sdk/FactSetESG/model_utils.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
```

## fds/sdk/FactSetESG/rest.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
```

## fds/sdk/FactSetESG/api/articles_api.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -24,16 +24,14 @@
     none_type,
     validate_and_convert_types
 )
 from fds.sdk.FactSetESG.exceptions import ApiException
 from fds.sdk.FactSetESG.model.error_response import ErrorResponse
 from fds.sdk.FactSetESG.model.sasb_articles_request import SasbArticlesRequest
 from fds.sdk.FactSetESG.model.sasb_articles_response import SasbArticlesResponse
-from fds.sdk.FactSetESG.model.sdg_articles_request import SdgArticlesRequest
-from fds.sdk.FactSetESG.model.sdg_articles_response import SdgArticlesResponse
 
 
 
 
 
 class ArticlesApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -192,163 +190,14 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
-        self.get_sdg_articles_endpoint = _Endpoint(
-            settings={
-                'response_type': (
-                  { 200: (SdgArticlesResponse,), 400: (ErrorResponse,), 401: (ErrorResponse,), 403: (ErrorResponse,), 408: (ErrorResponse,), 415: (ErrorResponse,), 500: (ErrorResponse,),  },
-                  None
-                ),
-                'auth': [
-                    'FactSetApiKey',
-                    'FactSetOAuth2'
-                ],
-                'endpoint_path': '/factset-esg/v1/sdg-articles',
-                'operation_id': 'get_sdg_articles',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'ids',
-                    'start_date',
-                    'end_date',
-                    'date_of',
-                    'fields',
-                    'categories',
-                ],
-                'required': [
-                    'ids',
-                    'start_date',
-                    'end_date',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                    'date_of',
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                    ('date_of',): {
-
-                        "PUBLICATION": "PUBLICATION",
-                        "INGESTION": "INGESTION"
-                    },
-                },
-                'openapi_types': {
-                    'ids':
-                        ([str],),
-                    'start_date':
-                        (str,),
-                    'end_date':
-                        (str,),
-                    'date_of':
-                        (str,),
-                    'fields':
-                        ([str],),
-                    'categories':
-                        ([str],),
-                },
-                'attribute_map': {
-                    'ids': 'ids',
-                    'start_date': 'startDate',
-                    'end_date': 'endDate',
-                    'date_of': 'dateOf',
-                    'fields': 'fields',
-                    'categories': 'categories',
-                },
-                'location_map': {
-                    'ids': 'query',
-                    'start_date': 'query',
-                    'end_date': 'query',
-                    'date_of': 'query',
-                    'fields': 'query',
-                    'categories': 'query',
-                },
-                'collection_format_map': {
-                    'ids': 'csv',
-                    'fields': 'csv',
-                    'categories': 'csv',
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-
-        self.get_sdg_articles_for_list_endpoint = _Endpoint(
-            settings={
-                'response_type': (
-                  { 200: (SdgArticlesResponse,), 400: (ErrorResponse,), 401: (ErrorResponse,), 403: (ErrorResponse,), 408: (ErrorResponse,), 415: (ErrorResponse,), 500: (ErrorResponse,),  },
-                  None
-                ),
-                'auth': [
-                    'FactSetApiKey',
-                    'FactSetOAuth2'
-                ],
-                'endpoint_path': '/factset-esg/v1/sdg-articles',
-                'operation_id': 'get_sdg_articles_for_list',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'sdg_articles_request',
-                ],
-                'required': [
-                    'sdg_articles_request',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'sdg_articles_request':
-                        (SdgArticlesRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'sdg_articles_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-
 
     @staticmethod
     def apply_kwargs_defaults(kwargs, return_http_data_only, async_req):
         kwargs["async_req"] = async_req
         kwargs["_return_http_data_only"] = return_http_data_only
         kwargs["_preload_content"] = kwargs.get("_preload_content", True)
         kwargs["_request_timeout"] = kwargs.get("_request_timeout", None)
@@ -781,433 +630,7 @@
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
         kwargs['sasb_articles_request'] = \
             sasb_articles_request
         return self.get_sasb_articles_for_list_endpoint.call_with_http_info(**kwargs)
 
 
-    def get_sdg_articles(
-        self,
-        ids,
-        start_date,
-        end_date,
-        **kwargs
-    ) -> SdgArticlesResponse:
-        """Request articles tagged with SDG lens categories from 2016-01-01 to previous day.  # noqa: E501
-
-        Articles endpoint allows to retrieve underlying news articles used by the AI engine to calculate the ESG Scores of companies and therefore provides ESG relevant news and also transparency into the ESG Scores.   # noqa: E501
-        This method makes a synchronous HTTP request. Returns the http data only
-
-        Args:
-            ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
-            start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
-            end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
-
-        Keyword Args:
-            date_of (str): Date of Publication or Ingestion   * **Publication:**  use for startDate and endDate the articles publication date   * **Ingestion:**  use for startDate and endDate the articles TVL first processing date    . [optional] if omitted the server will use the default value of "PUBLICATION"
-            fields ([str]): Request available Articles data fields to be included in the response.  Default is all fields. _fsymId_ and _articleId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |articleId|Unique ID of the article assigned by Truvalue|               <h3>Articles Fields</h3>     |field|description|   |---|---|   |datePub|Publication date of the article in YYYY-MM-DD format|   |title|Title of the article|   |source|Source of the article|   |categories|categories assigned by Truvalue|   |bullets|AI-generated bullet point summary for each article. Note, including bullets increases response size drastically|   |author|Author of the article|   |url|URL of the article|   |language|Language code of the article|   |dateIngestion|Date of TVL article ingestion and processing|   |orgName| Organization name assigned by Truvalue|   |orgId| Unique identifier assigned by Truvalue that is applied on an organization level  . [optional]
-            categories ([str]): The SDG Categories specified for the Truvalue Scores being requested. To specify select categories returned in the response, provide a comma-separated list of the scores using the description below.  |**SDG Category Input**|**Description**| |---|---| |**IMPACT**|**Impact** - Provides Articles tagged to all SDG categories| |**GOAL1NOPOVERTY**|**No Poverty** - Goal 1 focuses on poverty in all its manifestations and also aims to ensure social protection for the poor and vulnerable, increase access to basic services and support people harmed by climate related extreme events and other economic, social and environmental shocks and disasters. <p>**Company-Level Issue Examples** *- Financial services access and affordability, Underserved groups,Unethical pricing.*| |**GOAL2ZEROHUNGER**|**Zero Hunger** - Goal 2 aims to end hunger and all forms of malnutrition and commits to universal access to safe, nutritious and sufficient food at all times of the year, particularly for the poor and people in vulnerable situations (e.g., infants). This will require sustainable food production systems and resilient agricultural practices, equal access to land, technology, and markets and international cooperation on investments in infrastructure and technology to boost agricultural productivity. <p>**Company-Level Issue Examples** *- Sustainable agricultural practices, Agricultural ingredients sourcing and certifications, Food safety concerns, Animal welfare.*| |**GOAL3GOODHEALTHANDWELLBEING**|**Good Health and Wellbeing** - Goal 3 seeks to ensure health and wellbeing for all, at every stage of life and addresses all major health priorities, including reproductive, maternal, and child health; communicable, noncommunicable and environmental diseases; universal health coverage; and access for all to safe, effective, quality, and affordable medicines and vaccines.<p> **Company-Level Issue Examples** *- Harmful Chemicals in Products, Product Recalls, Healthcare Access and Affordability.*| |**GOAL4QUALITYEDUCATION**|**Quality Education** - Goal 4 addresses access and affordability of education and skills development starting from childhood development and continuing through adulthood, including for girls, persons with disabilities, indigenous peoples and children in vulnerable situations, Improvements to the access to education it hopes to ensure that all youth and a substantial proportion of adults achieve literacy and numeracy. It also seeks to build and upgrade education facilities and to increase the supply of qualified teachers.<p>**Company-Level Issue Examples** *- Mentorship and training, Education company quality, Education company ethics.*| |**GOAL5GENDEREQUALITY**|**Gender Equality** - Goal 5 emphasizes eliminating discrimination and violence against women and girls. The Goal emphasizes ensuring women's full and effective participation and equal opportunities for leadership at all levels of decision-making in political, economic and public life. Access to sexual and reproductive health and reproductive rights and access to economic resources (e.g., land ownership, financial services) are also emphasized.<p>**Company-Level Issue Examples** *- Board Diversity, Gender Discrimination, Sexual Harassment.*| |**GOAL6CLEANWATERANDSANITATION**|**Clean Water and Sanitation** - Goal 6 not only addresses issues relating to drinking water, sanitation and hygiene, but also the quality and sustainability of water resources worldwide. It strives to achieve universal and equitable access to safe and affordable drinking water for all. It also focuses on adequate and equitable sanitation and hygiene and reducing pollution, minimizing release of hazardous chemicals and materials, and protection of water-related ecosystems. It also highlights increasing water-use efficiency across all sectors, recycling, and ensuring sustainable withdrawals and supply of freshwater.<p>**Company-Level Issue Examples** *- Water Pollution, Water Recycling and Stewardship, Water Infrastructure.*| |**GOAL7AFFORDABLEANDCLEANENERGY**|**Goal 7 Affordable and Clean Energy** - Goal 7 seeks to ensure access to affordable, reliable, and modern energy services for all. It aims to increase renewable energy in the global energy mix and improve energy efficiency significantly. It also calls for more access to clean energy research, technology, and infrastructure for renewable energy, energy efficiency, and advanced and cleaner fossil-fuel technology, and promoting investment in energy infrastructure and clean energy technology.<p>**Company-Level Issue Examples** *- Green Buildings, Renewable Energy, Unethical Utility Pricing.*| |**GOAL8DECENTWORKANDECONOMICGROWTH**|**Decent Work and Economic Growth** - Goal 8 focuses on economic productivity and supports policies for entrepreneurship, creativity and innovation that assist micro, small, and medium-sized enterprises. The Goal also seeks to reduce unemployment, the proportion of youth not working or in school, child labor, and forced labor. Also covered are the protection of labor rights, migrant workers, safe and secure working environments, sustainable tourism, and increasing the capacity of domestic financial institutions in regards to access to banking, insurance, and financial services.<p>**Company-Level Issue Examples** *-  Job Creation, Labor Exploitation, Employee Health and Safety, Workplace Turnover, Supplier Transparency.*| |**GOAL9INDUSTRYINNOVATIONANDINFRASTRUCTURE**|**Industry Innovation and Infrastructure** - Goal 9 focuses on three important aspects of sustainable development, infrastructure, industrialization and innovation, including considerations for resiliency, equity, quality, reliability, access and affordability, and regional and transborder infrastructure. The Goal focuses on infrastructure upgrades and retrofitting of industries with increased resource-use efficiency and clean and environmentally sound technologies and industrial processes.<p>**Company-Level Issue Examples** *- Digital Divide, ESG integration in financial services, Engineering Structural Integrity.*| |**GOAL10REDUCEDINEQUALITIES**|**Reduced Inequalities** - Goal 10 calls for reducing inequalities in income as well as those based on age, sex, disability, race, ethnicity, origin, religion, or economic or other status within a country. The Goal addresses inequalities among countries, including those related to representation, migration, and development assistance. It aims to empower and promote social, economic, and political inclusion of all. The Goal stresses regulation and monitoring of global financial markets and institutions.<p>**Company-Level Issue Examples** *- Responsible Lending, Worker Discrimination, CEO Pay Gap, Worker Pay Gap, Workplace Diversity and Inclusion.*| |**GOAL11SUSTAINABLECITIESANDCOMMUNITIES**|**Sustainable Cities and Communities** - Goal 11 seeks to ensure access for all to adequate, safe, and affordable housing and basic services, and green and public spaces, and to upgrade slums. It focuses on improving transportation, air quality and municipal and other waste management, and creating inclusive and sustainable urbanization through participatory urban planning. The Goal also supports safeguarding the world's cultural and natural heritage, while aiming to increase the number of cities and human settlements adopting and implementing integrated policies and plans towards inclusion, resource efficiency, mitigation and adaptation to climate change, and resilience to disasters.<p>**Company-Level Issue Examples** *- Air Pollution, Environmental Justice, Human Rights Violations, Affordable Housing.*| |**GOAL12RESPONSIBLECONSUMPTIONANDPRODUCTION**|**Responsible Consumption and Production** - Goal 12 aims to achieve the sustainable management and efficient use of natural resources through both the public and private sector. It specifically addresses global food waste in consumption, production, and distribution, sustainable tourism, waste and chemicals management. Goal 12 encourages sustainability reporting in the private sector, while in the public sector it encourages restructuring taxation and subsidies for fossil fuels and promoting sustainable public procurement practices.<p>**Company-Level Issue Examples** *- Sustainability Reporting, Circular Economy, Hazardous Waste Management, Waste Reduction.*| |**GOAL13CLIMATEACTION**|**Climate Action** - While Goal 13 is focused on actions by countries towards climate mitigation and adaptation, the private sector can also play a role in these areas. The goal seeks to strengthen resilience and adaptive capacity to climate-related hazards and natural disasters in all countries. It calls for integrating climate change measures, including those related to climate resilience and low GHG development, into national policies, strategies, and planning. It aims to improve education and awareness of climate change mitigation, adaptation, impact reduction, and early warning.<p>**Company-Level Issue Examples** *- GHG Emissions, Sustainable Transportation, Physical Climate Impacts.*| |**GOAL14LIFEBELOWWATER**|**Life Below Water** - Goal 14 focuses on preventing marine pollution of all kinds, particularly from land-based activities, and to minimize and address the impacts of ocean acidification. The Goal also aims to achieve sustainable yields in fisheries, through regulation of harvesting, controlling subsidies, and ending overfishing. It seeks to sustainably manage and protect marine and coastal ecosystems to avoid significant adverse impacts, including by strengthening their resilience, and take action for their restoration in order to achieve healthy and productive oceans.<p>**Company-Level Issue Examples** *- Impacts on water-related endangered species and habitats, Oil Spills, Seafood Sourcing.*| |**GOAL15LIFEONLAND**|**Life On Land** - Goal 15 seeks to ensure the conservation, restoration, and sustainable use of terrestrial and inland freshwater ecosystems and their services, in order to preserve biodiversity. It focuses specifically on sustainably managing forests, halting deforestation, restoring degraded lands and successfully combating desertification, reducing degraded natural habitats and ending biodiversity loss, with an emphasis on threatened species and invasive alien species.<p>**Company-Level Issue Examples** *- Impacts on land-related endangered species and habitats, Sustainable forestry practices and certifications, Project lifecycle environmental impacts.*| |**GOAL16PEACEJUSTICEANDSTRONGINSTITUTIONS**|**Peace, Justice, and Strong Institutions** - Goal 16 aims to significantly reduce all forms of violence, and also focuses specifically on reducing violence against children in the forms of abuse, exploitation, trafficking, and torture. It also aims to significantly reduce illicit financial and arms flows and to substantially reduce corruption and bribery in all their forms. The Goal also emphasizes effective and transparent institutions at all levels, inclusive and participatory decision-making, ensuring public access to information, and protection of fundamental freedoms.<p>**Company-Level Issue Examples** *- Tax Avoidance, Anti-Competitive Behavior, Cyber Security, Corruption, ESG Resolutions.*| . [optional] if omitted the server will use the default value of ["IMPACT"]
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            SdgArticlesResponse
-                Response Object
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
-        kwargs['ids'] = \
-            ids
-        kwargs['start_date'] = \
-            start_date
-        kwargs['end_date'] = \
-            end_date
-        return self.get_sdg_articles_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_articles_with_http_info(
-        self,
-        ids,
-        start_date,
-        end_date,
-        **kwargs
-    ) -> typing.Tuple[SdgArticlesResponse, int, typing.MutableMapping]:
-        """Request articles tagged with SDG lens categories from 2016-01-01 to previous day.  # noqa: E501
-
-        Articles endpoint allows to retrieve underlying news articles used by the AI engine to calculate the ESG Scores of companies and therefore provides ESG relevant news and also transparency into the ESG Scores.   # noqa: E501
-        This method makes a synchronous HTTP request. Returns http data, http status and headers
-
-        Args:
-            ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
-            start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
-            end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
-
-        Keyword Args:
-            date_of (str): Date of Publication or Ingestion   * **Publication:**  use for startDate and endDate the articles publication date   * **Ingestion:**  use for startDate and endDate the articles TVL first processing date    . [optional] if omitted the server will use the default value of "PUBLICATION"
-            fields ([str]): Request available Articles data fields to be included in the response.  Default is all fields. _fsymId_ and _articleId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |articleId|Unique ID of the article assigned by Truvalue|               <h3>Articles Fields</h3>     |field|description|   |---|---|   |datePub|Publication date of the article in YYYY-MM-DD format|   |title|Title of the article|   |source|Source of the article|   |categories|categories assigned by Truvalue|   |bullets|AI-generated bullet point summary for each article. Note, including bullets increases response size drastically|   |author|Author of the article|   |url|URL of the article|   |language|Language code of the article|   |dateIngestion|Date of TVL article ingestion and processing|   |orgName| Organization name assigned by Truvalue|   |orgId| Unique identifier assigned by Truvalue that is applied on an organization level  . [optional]
-            categories ([str]): The SDG Categories specified for the Truvalue Scores being requested. To specify select categories returned in the response, provide a comma-separated list of the scores using the description below.  |**SDG Category Input**|**Description**| |---|---| |**IMPACT**|**Impact** - Provides Articles tagged to all SDG categories| |**GOAL1NOPOVERTY**|**No Poverty** - Goal 1 focuses on poverty in all its manifestations and also aims to ensure social protection for the poor and vulnerable, increase access to basic services and support people harmed by climate related extreme events and other economic, social and environmental shocks and disasters. <p>**Company-Level Issue Examples** *- Financial services access and affordability, Underserved groups,Unethical pricing.*| |**GOAL2ZEROHUNGER**|**Zero Hunger** - Goal 2 aims to end hunger and all forms of malnutrition and commits to universal access to safe, nutritious and sufficient food at all times of the year, particularly for the poor and people in vulnerable situations (e.g., infants). This will require sustainable food production systems and resilient agricultural practices, equal access to land, technology, and markets and international cooperation on investments in infrastructure and technology to boost agricultural productivity. <p>**Company-Level Issue Examples** *- Sustainable agricultural practices, Agricultural ingredients sourcing and certifications, Food safety concerns, Animal welfare.*| |**GOAL3GOODHEALTHANDWELLBEING**|**Good Health and Wellbeing** - Goal 3 seeks to ensure health and wellbeing for all, at every stage of life and addresses all major health priorities, including reproductive, maternal, and child health; communicable, noncommunicable and environmental diseases; universal health coverage; and access for all to safe, effective, quality, and affordable medicines and vaccines.<p> **Company-Level Issue Examples** *- Harmful Chemicals in Products, Product Recalls, Healthcare Access and Affordability.*| |**GOAL4QUALITYEDUCATION**|**Quality Education** - Goal 4 addresses access and affordability of education and skills development starting from childhood development and continuing through adulthood, including for girls, persons with disabilities, indigenous peoples and children in vulnerable situations, Improvements to the access to education it hopes to ensure that all youth and a substantial proportion of adults achieve literacy and numeracy. It also seeks to build and upgrade education facilities and to increase the supply of qualified teachers.<p>**Company-Level Issue Examples** *- Mentorship and training, Education company quality, Education company ethics.*| |**GOAL5GENDEREQUALITY**|**Gender Equality** - Goal 5 emphasizes eliminating discrimination and violence against women and girls. The Goal emphasizes ensuring women's full and effective participation and equal opportunities for leadership at all levels of decision-making in political, economic and public life. Access to sexual and reproductive health and reproductive rights and access to economic resources (e.g., land ownership, financial services) are also emphasized.<p>**Company-Level Issue Examples** *- Board Diversity, Gender Discrimination, Sexual Harassment.*| |**GOAL6CLEANWATERANDSANITATION**|**Clean Water and Sanitation** - Goal 6 not only addresses issues relating to drinking water, sanitation and hygiene, but also the quality and sustainability of water resources worldwide. It strives to achieve universal and equitable access to safe and affordable drinking water for all. It also focuses on adequate and equitable sanitation and hygiene and reducing pollution, minimizing release of hazardous chemicals and materials, and protection of water-related ecosystems. It also highlights increasing water-use efficiency across all sectors, recycling, and ensuring sustainable withdrawals and supply of freshwater.<p>**Company-Level Issue Examples** *- Water Pollution, Water Recycling and Stewardship, Water Infrastructure.*| |**GOAL7AFFORDABLEANDCLEANENERGY**|**Goal 7 Affordable and Clean Energy** - Goal 7 seeks to ensure access to affordable, reliable, and modern energy services for all. It aims to increase renewable energy in the global energy mix and improve energy efficiency significantly. It also calls for more access to clean energy research, technology, and infrastructure for renewable energy, energy efficiency, and advanced and cleaner fossil-fuel technology, and promoting investment in energy infrastructure and clean energy technology.<p>**Company-Level Issue Examples** *- Green Buildings, Renewable Energy, Unethical Utility Pricing.*| |**GOAL8DECENTWORKANDECONOMICGROWTH**|**Decent Work and Economic Growth** - Goal 8 focuses on economic productivity and supports policies for entrepreneurship, creativity and innovation that assist micro, small, and medium-sized enterprises. The Goal also seeks to reduce unemployment, the proportion of youth not working or in school, child labor, and forced labor. Also covered are the protection of labor rights, migrant workers, safe and secure working environments, sustainable tourism, and increasing the capacity of domestic financial institutions in regards to access to banking, insurance, and financial services.<p>**Company-Level Issue Examples** *-  Job Creation, Labor Exploitation, Employee Health and Safety, Workplace Turnover, Supplier Transparency.*| |**GOAL9INDUSTRYINNOVATIONANDINFRASTRUCTURE**|**Industry Innovation and Infrastructure** - Goal 9 focuses on three important aspects of sustainable development, infrastructure, industrialization and innovation, including considerations for resiliency, equity, quality, reliability, access and affordability, and regional and transborder infrastructure. The Goal focuses on infrastructure upgrades and retrofitting of industries with increased resource-use efficiency and clean and environmentally sound technologies and industrial processes.<p>**Company-Level Issue Examples** *- Digital Divide, ESG integration in financial services, Engineering Structural Integrity.*| |**GOAL10REDUCEDINEQUALITIES**|**Reduced Inequalities** - Goal 10 calls for reducing inequalities in income as well as those based on age, sex, disability, race, ethnicity, origin, religion, or economic or other status within a country. The Goal addresses inequalities among countries, including those related to representation, migration, and development assistance. It aims to empower and promote social, economic, and political inclusion of all. The Goal stresses regulation and monitoring of global financial markets and institutions.<p>**Company-Level Issue Examples** *- Responsible Lending, Worker Discrimination, CEO Pay Gap, Worker Pay Gap, Workplace Diversity and Inclusion.*| |**GOAL11SUSTAINABLECITIESANDCOMMUNITIES**|**Sustainable Cities and Communities** - Goal 11 seeks to ensure access for all to adequate, safe, and affordable housing and basic services, and green and public spaces, and to upgrade slums. It focuses on improving transportation, air quality and municipal and other waste management, and creating inclusive and sustainable urbanization through participatory urban planning. The Goal also supports safeguarding the world's cultural and natural heritage, while aiming to increase the number of cities and human settlements adopting and implementing integrated policies and plans towards inclusion, resource efficiency, mitigation and adaptation to climate change, and resilience to disasters.<p>**Company-Level Issue Examples** *- Air Pollution, Environmental Justice, Human Rights Violations, Affordable Housing.*| |**GOAL12RESPONSIBLECONSUMPTIONANDPRODUCTION**|**Responsible Consumption and Production** - Goal 12 aims to achieve the sustainable management and efficient use of natural resources through both the public and private sector. It specifically addresses global food waste in consumption, production, and distribution, sustainable tourism, waste and chemicals management. Goal 12 encourages sustainability reporting in the private sector, while in the public sector it encourages restructuring taxation and subsidies for fossil fuels and promoting sustainable public procurement practices.<p>**Company-Level Issue Examples** *- Sustainability Reporting, Circular Economy, Hazardous Waste Management, Waste Reduction.*| |**GOAL13CLIMATEACTION**|**Climate Action** - While Goal 13 is focused on actions by countries towards climate mitigation and adaptation, the private sector can also play a role in these areas. The goal seeks to strengthen resilience and adaptive capacity to climate-related hazards and natural disasters in all countries. It calls for integrating climate change measures, including those related to climate resilience and low GHG development, into national policies, strategies, and planning. It aims to improve education and awareness of climate change mitigation, adaptation, impact reduction, and early warning.<p>**Company-Level Issue Examples** *- GHG Emissions, Sustainable Transportation, Physical Climate Impacts.*| |**GOAL14LIFEBELOWWATER**|**Life Below Water** - Goal 14 focuses on preventing marine pollution of all kinds, particularly from land-based activities, and to minimize and address the impacts of ocean acidification. The Goal also aims to achieve sustainable yields in fisheries, through regulation of harvesting, controlling subsidies, and ending overfishing. It seeks to sustainably manage and protect marine and coastal ecosystems to avoid significant adverse impacts, including by strengthening their resilience, and take action for their restoration in order to achieve healthy and productive oceans.<p>**Company-Level Issue Examples** *- Impacts on water-related endangered species and habitats, Oil Spills, Seafood Sourcing.*| |**GOAL15LIFEONLAND**|**Life On Land** - Goal 15 seeks to ensure the conservation, restoration, and sustainable use of terrestrial and inland freshwater ecosystems and their services, in order to preserve biodiversity. It focuses specifically on sustainably managing forests, halting deforestation, restoring degraded lands and successfully combating desertification, reducing degraded natural habitats and ending biodiversity loss, with an emphasis on threatened species and invasive alien species.<p>**Company-Level Issue Examples** *- Impacts on land-related endangered species and habitats, Sustainable forestry practices and certifications, Project lifecycle environmental impacts.*| |**GOAL16PEACEJUSTICEANDSTRONGINSTITUTIONS**|**Peace, Justice, and Strong Institutions** - Goal 16 aims to significantly reduce all forms of violence, and also focuses specifically on reducing violence against children in the forms of abuse, exploitation, trafficking, and torture. It also aims to significantly reduce illicit financial and arms flows and to substantially reduce corruption and bribery in all their forms. The Goal also emphasizes effective and transparent institutions at all levels, inclusive and participatory decision-making, ensuring public access to information, and protection of fundamental freedoms.<p>**Company-Level Issue Examples** *- Tax Avoidance, Anti-Competitive Behavior, Cyber Security, Corruption, ESG Resolutions.*| . [optional] if omitted the server will use the default value of ["IMPACT"]
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            SdgArticlesResponse
-                Response Object
-            int
-                Http Status Code
-            dict
-                Dictionary of the response headers
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
-        kwargs['ids'] = \
-            ids
-        kwargs['start_date'] = \
-            start_date
-        kwargs['end_date'] = \
-            end_date
-        return self.get_sdg_articles_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_articles_async(
-        self,
-        ids,
-        start_date,
-        end_date,
-        **kwargs
-    ) -> "ApplyResult[SdgArticlesResponse]":
-        """Request articles tagged with SDG lens categories from 2016-01-01 to previous day.  # noqa: E501
-
-        Articles endpoint allows to retrieve underlying news articles used by the AI engine to calculate the ESG Scores of companies and therefore provides ESG relevant news and also transparency into the ESG Scores.   # noqa: E501
-        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
-
-        Args:
-            ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
-            start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
-            end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
-
-        Keyword Args:
-            date_of (str): Date of Publication or Ingestion   * **Publication:**  use for startDate and endDate the articles publication date   * **Ingestion:**  use for startDate and endDate the articles TVL first processing date    . [optional] if omitted the server will use the default value of "PUBLICATION"
-            fields ([str]): Request available Articles data fields to be included in the response.  Default is all fields. _fsymId_ and _articleId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |articleId|Unique ID of the article assigned by Truvalue|               <h3>Articles Fields</h3>     |field|description|   |---|---|   |datePub|Publication date of the article in YYYY-MM-DD format|   |title|Title of the article|   |source|Source of the article|   |categories|categories assigned by Truvalue|   |bullets|AI-generated bullet point summary for each article. Note, including bullets increases response size drastically|   |author|Author of the article|   |url|URL of the article|   |language|Language code of the article|   |dateIngestion|Date of TVL article ingestion and processing|   |orgName| Organization name assigned by Truvalue|   |orgId| Unique identifier assigned by Truvalue that is applied on an organization level  . [optional]
-            categories ([str]): The SDG Categories specified for the Truvalue Scores being requested. To specify select categories returned in the response, provide a comma-separated list of the scores using the description below.  |**SDG Category Input**|**Description**| |---|---| |**IMPACT**|**Impact** - Provides Articles tagged to all SDG categories| |**GOAL1NOPOVERTY**|**No Poverty** - Goal 1 focuses on poverty in all its manifestations and also aims to ensure social protection for the poor and vulnerable, increase access to basic services and support people harmed by climate related extreme events and other economic, social and environmental shocks and disasters. <p>**Company-Level Issue Examples** *- Financial services access and affordability, Underserved groups,Unethical pricing.*| |**GOAL2ZEROHUNGER**|**Zero Hunger** - Goal 2 aims to end hunger and all forms of malnutrition and commits to universal access to safe, nutritious and sufficient food at all times of the year, particularly for the poor and people in vulnerable situations (e.g., infants). This will require sustainable food production systems and resilient agricultural practices, equal access to land, technology, and markets and international cooperation on investments in infrastructure and technology to boost agricultural productivity. <p>**Company-Level Issue Examples** *- Sustainable agricultural practices, Agricultural ingredients sourcing and certifications, Food safety concerns, Animal welfare.*| |**GOAL3GOODHEALTHANDWELLBEING**|**Good Health and Wellbeing** - Goal 3 seeks to ensure health and wellbeing for all, at every stage of life and addresses all major health priorities, including reproductive, maternal, and child health; communicable, noncommunicable and environmental diseases; universal health coverage; and access for all to safe, effective, quality, and affordable medicines and vaccines.<p> **Company-Level Issue Examples** *- Harmful Chemicals in Products, Product Recalls, Healthcare Access and Affordability.*| |**GOAL4QUALITYEDUCATION**|**Quality Education** - Goal 4 addresses access and affordability of education and skills development starting from childhood development and continuing through adulthood, including for girls, persons with disabilities, indigenous peoples and children in vulnerable situations, Improvements to the access to education it hopes to ensure that all youth and a substantial proportion of adults achieve literacy and numeracy. It also seeks to build and upgrade education facilities and to increase the supply of qualified teachers.<p>**Company-Level Issue Examples** *- Mentorship and training, Education company quality, Education company ethics.*| |**GOAL5GENDEREQUALITY**|**Gender Equality** - Goal 5 emphasizes eliminating discrimination and violence against women and girls. The Goal emphasizes ensuring women's full and effective participation and equal opportunities for leadership at all levels of decision-making in political, economic and public life. Access to sexual and reproductive health and reproductive rights and access to economic resources (e.g., land ownership, financial services) are also emphasized.<p>**Company-Level Issue Examples** *- Board Diversity, Gender Discrimination, Sexual Harassment.*| |**GOAL6CLEANWATERANDSANITATION**|**Clean Water and Sanitation** - Goal 6 not only addresses issues relating to drinking water, sanitation and hygiene, but also the quality and sustainability of water resources worldwide. It strives to achieve universal and equitable access to safe and affordable drinking water for all. It also focuses on adequate and equitable sanitation and hygiene and reducing pollution, minimizing release of hazardous chemicals and materials, and protection of water-related ecosystems. It also highlights increasing water-use efficiency across all sectors, recycling, and ensuring sustainable withdrawals and supply of freshwater.<p>**Company-Level Issue Examples** *- Water Pollution, Water Recycling and Stewardship, Water Infrastructure.*| |**GOAL7AFFORDABLEANDCLEANENERGY**|**Goal 7 Affordable and Clean Energy** - Goal 7 seeks to ensure access to affordable, reliable, and modern energy services for all. It aims to increase renewable energy in the global energy mix and improve energy efficiency significantly. It also calls for more access to clean energy research, technology, and infrastructure for renewable energy, energy efficiency, and advanced and cleaner fossil-fuel technology, and promoting investment in energy infrastructure and clean energy technology.<p>**Company-Level Issue Examples** *- Green Buildings, Renewable Energy, Unethical Utility Pricing.*| |**GOAL8DECENTWORKANDECONOMICGROWTH**|**Decent Work and Economic Growth** - Goal 8 focuses on economic productivity and supports policies for entrepreneurship, creativity and innovation that assist micro, small, and medium-sized enterprises. The Goal also seeks to reduce unemployment, the proportion of youth not working or in school, child labor, and forced labor. Also covered are the protection of labor rights, migrant workers, safe and secure working environments, sustainable tourism, and increasing the capacity of domestic financial institutions in regards to access to banking, insurance, and financial services.<p>**Company-Level Issue Examples** *-  Job Creation, Labor Exploitation, Employee Health and Safety, Workplace Turnover, Supplier Transparency.*| |**GOAL9INDUSTRYINNOVATIONANDINFRASTRUCTURE**|**Industry Innovation and Infrastructure** - Goal 9 focuses on three important aspects of sustainable development, infrastructure, industrialization and innovation, including considerations for resiliency, equity, quality, reliability, access and affordability, and regional and transborder infrastructure. The Goal focuses on infrastructure upgrades and retrofitting of industries with increased resource-use efficiency and clean and environmentally sound technologies and industrial processes.<p>**Company-Level Issue Examples** *- Digital Divide, ESG integration in financial services, Engineering Structural Integrity.*| |**GOAL10REDUCEDINEQUALITIES**|**Reduced Inequalities** - Goal 10 calls for reducing inequalities in income as well as those based on age, sex, disability, race, ethnicity, origin, religion, or economic or other status within a country. The Goal addresses inequalities among countries, including those related to representation, migration, and development assistance. It aims to empower and promote social, economic, and political inclusion of all. The Goal stresses regulation and monitoring of global financial markets and institutions.<p>**Company-Level Issue Examples** *- Responsible Lending, Worker Discrimination, CEO Pay Gap, Worker Pay Gap, Workplace Diversity and Inclusion.*| |**GOAL11SUSTAINABLECITIESANDCOMMUNITIES**|**Sustainable Cities and Communities** - Goal 11 seeks to ensure access for all to adequate, safe, and affordable housing and basic services, and green and public spaces, and to upgrade slums. It focuses on improving transportation, air quality and municipal and other waste management, and creating inclusive and sustainable urbanization through participatory urban planning. The Goal also supports safeguarding the world's cultural and natural heritage, while aiming to increase the number of cities and human settlements adopting and implementing integrated policies and plans towards inclusion, resource efficiency, mitigation and adaptation to climate change, and resilience to disasters.<p>**Company-Level Issue Examples** *- Air Pollution, Environmental Justice, Human Rights Violations, Affordable Housing.*| |**GOAL12RESPONSIBLECONSUMPTIONANDPRODUCTION**|**Responsible Consumption and Production** - Goal 12 aims to achieve the sustainable management and efficient use of natural resources through both the public and private sector. It specifically addresses global food waste in consumption, production, and distribution, sustainable tourism, waste and chemicals management. Goal 12 encourages sustainability reporting in the private sector, while in the public sector it encourages restructuring taxation and subsidies for fossil fuels and promoting sustainable public procurement practices.<p>**Company-Level Issue Examples** *- Sustainability Reporting, Circular Economy, Hazardous Waste Management, Waste Reduction.*| |**GOAL13CLIMATEACTION**|**Climate Action** - While Goal 13 is focused on actions by countries towards climate mitigation and adaptation, the private sector can also play a role in these areas. The goal seeks to strengthen resilience and adaptive capacity to climate-related hazards and natural disasters in all countries. It calls for integrating climate change measures, including those related to climate resilience and low GHG development, into national policies, strategies, and planning. It aims to improve education and awareness of climate change mitigation, adaptation, impact reduction, and early warning.<p>**Company-Level Issue Examples** *- GHG Emissions, Sustainable Transportation, Physical Climate Impacts.*| |**GOAL14LIFEBELOWWATER**|**Life Below Water** - Goal 14 focuses on preventing marine pollution of all kinds, particularly from land-based activities, and to minimize and address the impacts of ocean acidification. The Goal also aims to achieve sustainable yields in fisheries, through regulation of harvesting, controlling subsidies, and ending overfishing. It seeks to sustainably manage and protect marine and coastal ecosystems to avoid significant adverse impacts, including by strengthening their resilience, and take action for their restoration in order to achieve healthy and productive oceans.<p>**Company-Level Issue Examples** *- Impacts on water-related endangered species and habitats, Oil Spills, Seafood Sourcing.*| |**GOAL15LIFEONLAND**|**Life On Land** - Goal 15 seeks to ensure the conservation, restoration, and sustainable use of terrestrial and inland freshwater ecosystems and their services, in order to preserve biodiversity. It focuses specifically on sustainably managing forests, halting deforestation, restoring degraded lands and successfully combating desertification, reducing degraded natural habitats and ending biodiversity loss, with an emphasis on threatened species and invasive alien species.<p>**Company-Level Issue Examples** *- Impacts on land-related endangered species and habitats, Sustainable forestry practices and certifications, Project lifecycle environmental impacts.*| |**GOAL16PEACEJUSTICEANDSTRONGINSTITUTIONS**|**Peace, Justice, and Strong Institutions** - Goal 16 aims to significantly reduce all forms of violence, and also focuses specifically on reducing violence against children in the forms of abuse, exploitation, trafficking, and torture. It also aims to significantly reduce illicit financial and arms flows and to substantially reduce corruption and bribery in all their forms. The Goal also emphasizes effective and transparent institutions at all levels, inclusive and participatory decision-making, ensuring public access to information, and protection of fundamental freedoms.<p>**Company-Level Issue Examples** *- Tax Avoidance, Anti-Competitive Behavior, Cyber Security, Corruption, ESG Resolutions.*| . [optional] if omitted the server will use the default value of ["IMPACT"]
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            ApplyResult[SdgArticlesResponse]
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
-        kwargs['ids'] = \
-            ids
-        kwargs['start_date'] = \
-            start_date
-        kwargs['end_date'] = \
-            end_date
-        return self.get_sdg_articles_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_articles_with_http_info_async(
-        self,
-        ids,
-        start_date,
-        end_date,
-        **kwargs
-    ) -> "ApplyResult[typing.Tuple[SdgArticlesResponse, int, typing.MutableMapping]]":
-        """Request articles tagged with SDG lens categories from 2016-01-01 to previous day.  # noqa: E501
-
-        Articles endpoint allows to retrieve underlying news articles used by the AI engine to calculate the ESG Scores of companies and therefore provides ESG relevant news and also transparency into the ESG Scores.   # noqa: E501
-        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
-
-        Args:
-            ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
-            start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
-            end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
-
-        Keyword Args:
-            date_of (str): Date of Publication or Ingestion   * **Publication:**  use for startDate and endDate the articles publication date   * **Ingestion:**  use for startDate and endDate the articles TVL first processing date    . [optional] if omitted the server will use the default value of "PUBLICATION"
-            fields ([str]): Request available Articles data fields to be included in the response.  Default is all fields. _fsymId_ and _articleId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |articleId|Unique ID of the article assigned by Truvalue|               <h3>Articles Fields</h3>     |field|description|   |---|---|   |datePub|Publication date of the article in YYYY-MM-DD format|   |title|Title of the article|   |source|Source of the article|   |categories|categories assigned by Truvalue|   |bullets|AI-generated bullet point summary for each article. Note, including bullets increases response size drastically|   |author|Author of the article|   |url|URL of the article|   |language|Language code of the article|   |dateIngestion|Date of TVL article ingestion and processing|   |orgName| Organization name assigned by Truvalue|   |orgId| Unique identifier assigned by Truvalue that is applied on an organization level  . [optional]
-            categories ([str]): The SDG Categories specified for the Truvalue Scores being requested. To specify select categories returned in the response, provide a comma-separated list of the scores using the description below.  |**SDG Category Input**|**Description**| |---|---| |**IMPACT**|**Impact** - Provides Articles tagged to all SDG categories| |**GOAL1NOPOVERTY**|**No Poverty** - Goal 1 focuses on poverty in all its manifestations and also aims to ensure social protection for the poor and vulnerable, increase access to basic services and support people harmed by climate related extreme events and other economic, social and environmental shocks and disasters. <p>**Company-Level Issue Examples** *- Financial services access and affordability, Underserved groups,Unethical pricing.*| |**GOAL2ZEROHUNGER**|**Zero Hunger** - Goal 2 aims to end hunger and all forms of malnutrition and commits to universal access to safe, nutritious and sufficient food at all times of the year, particularly for the poor and people in vulnerable situations (e.g., infants). This will require sustainable food production systems and resilient agricultural practices, equal access to land, technology, and markets and international cooperation on investments in infrastructure and technology to boost agricultural productivity. <p>**Company-Level Issue Examples** *- Sustainable agricultural practices, Agricultural ingredients sourcing and certifications, Food safety concerns, Animal welfare.*| |**GOAL3GOODHEALTHANDWELLBEING**|**Good Health and Wellbeing** - Goal 3 seeks to ensure health and wellbeing for all, at every stage of life and addresses all major health priorities, including reproductive, maternal, and child health; communicable, noncommunicable and environmental diseases; universal health coverage; and access for all to safe, effective, quality, and affordable medicines and vaccines.<p> **Company-Level Issue Examples** *- Harmful Chemicals in Products, Product Recalls, Healthcare Access and Affordability.*| |**GOAL4QUALITYEDUCATION**|**Quality Education** - Goal 4 addresses access and affordability of education and skills development starting from childhood development and continuing through adulthood, including for girls, persons with disabilities, indigenous peoples and children in vulnerable situations, Improvements to the access to education it hopes to ensure that all youth and a substantial proportion of adults achieve literacy and numeracy. It also seeks to build and upgrade education facilities and to increase the supply of qualified teachers.<p>**Company-Level Issue Examples** *- Mentorship and training, Education company quality, Education company ethics.*| |**GOAL5GENDEREQUALITY**|**Gender Equality** - Goal 5 emphasizes eliminating discrimination and violence against women and girls. The Goal emphasizes ensuring women's full and effective participation and equal opportunities for leadership at all levels of decision-making in political, economic and public life. Access to sexual and reproductive health and reproductive rights and access to economic resources (e.g., land ownership, financial services) are also emphasized.<p>**Company-Level Issue Examples** *- Board Diversity, Gender Discrimination, Sexual Harassment.*| |**GOAL6CLEANWATERANDSANITATION**|**Clean Water and Sanitation** - Goal 6 not only addresses issues relating to drinking water, sanitation and hygiene, but also the quality and sustainability of water resources worldwide. It strives to achieve universal and equitable access to safe and affordable drinking water for all. It also focuses on adequate and equitable sanitation and hygiene and reducing pollution, minimizing release of hazardous chemicals and materials, and protection of water-related ecosystems. It also highlights increasing water-use efficiency across all sectors, recycling, and ensuring sustainable withdrawals and supply of freshwater.<p>**Company-Level Issue Examples** *- Water Pollution, Water Recycling and Stewardship, Water Infrastructure.*| |**GOAL7AFFORDABLEANDCLEANENERGY**|**Goal 7 Affordable and Clean Energy** - Goal 7 seeks to ensure access to affordable, reliable, and modern energy services for all. It aims to increase renewable energy in the global energy mix and improve energy efficiency significantly. It also calls for more access to clean energy research, technology, and infrastructure for renewable energy, energy efficiency, and advanced and cleaner fossil-fuel technology, and promoting investment in energy infrastructure and clean energy technology.<p>**Company-Level Issue Examples** *- Green Buildings, Renewable Energy, Unethical Utility Pricing.*| |**GOAL8DECENTWORKANDECONOMICGROWTH**|**Decent Work and Economic Growth** - Goal 8 focuses on economic productivity and supports policies for entrepreneurship, creativity and innovation that assist micro, small, and medium-sized enterprises. The Goal also seeks to reduce unemployment, the proportion of youth not working or in school, child labor, and forced labor. Also covered are the protection of labor rights, migrant workers, safe and secure working environments, sustainable tourism, and increasing the capacity of domestic financial institutions in regards to access to banking, insurance, and financial services.<p>**Company-Level Issue Examples** *-  Job Creation, Labor Exploitation, Employee Health and Safety, Workplace Turnover, Supplier Transparency.*| |**GOAL9INDUSTRYINNOVATIONANDINFRASTRUCTURE**|**Industry Innovation and Infrastructure** - Goal 9 focuses on three important aspects of sustainable development, infrastructure, industrialization and innovation, including considerations for resiliency, equity, quality, reliability, access and affordability, and regional and transborder infrastructure. The Goal focuses on infrastructure upgrades and retrofitting of industries with increased resource-use efficiency and clean and environmentally sound technologies and industrial processes.<p>**Company-Level Issue Examples** *- Digital Divide, ESG integration in financial services, Engineering Structural Integrity.*| |**GOAL10REDUCEDINEQUALITIES**|**Reduced Inequalities** - Goal 10 calls for reducing inequalities in income as well as those based on age, sex, disability, race, ethnicity, origin, religion, or economic or other status within a country. The Goal addresses inequalities among countries, including those related to representation, migration, and development assistance. It aims to empower and promote social, economic, and political inclusion of all. The Goal stresses regulation and monitoring of global financial markets and institutions.<p>**Company-Level Issue Examples** *- Responsible Lending, Worker Discrimination, CEO Pay Gap, Worker Pay Gap, Workplace Diversity and Inclusion.*| |**GOAL11SUSTAINABLECITIESANDCOMMUNITIES**|**Sustainable Cities and Communities** - Goal 11 seeks to ensure access for all to adequate, safe, and affordable housing and basic services, and green and public spaces, and to upgrade slums. It focuses on improving transportation, air quality and municipal and other waste management, and creating inclusive and sustainable urbanization through participatory urban planning. The Goal also supports safeguarding the world's cultural and natural heritage, while aiming to increase the number of cities and human settlements adopting and implementing integrated policies and plans towards inclusion, resource efficiency, mitigation and adaptation to climate change, and resilience to disasters.<p>**Company-Level Issue Examples** *- Air Pollution, Environmental Justice, Human Rights Violations, Affordable Housing.*| |**GOAL12RESPONSIBLECONSUMPTIONANDPRODUCTION**|**Responsible Consumption and Production** - Goal 12 aims to achieve the sustainable management and efficient use of natural resources through both the public and private sector. It specifically addresses global food waste in consumption, production, and distribution, sustainable tourism, waste and chemicals management. Goal 12 encourages sustainability reporting in the private sector, while in the public sector it encourages restructuring taxation and subsidies for fossil fuels and promoting sustainable public procurement practices.<p>**Company-Level Issue Examples** *- Sustainability Reporting, Circular Economy, Hazardous Waste Management, Waste Reduction.*| |**GOAL13CLIMATEACTION**|**Climate Action** - While Goal 13 is focused on actions by countries towards climate mitigation and adaptation, the private sector can also play a role in these areas. The goal seeks to strengthen resilience and adaptive capacity to climate-related hazards and natural disasters in all countries. It calls for integrating climate change measures, including those related to climate resilience and low GHG development, into national policies, strategies, and planning. It aims to improve education and awareness of climate change mitigation, adaptation, impact reduction, and early warning.<p>**Company-Level Issue Examples** *- GHG Emissions, Sustainable Transportation, Physical Climate Impacts.*| |**GOAL14LIFEBELOWWATER**|**Life Below Water** - Goal 14 focuses on preventing marine pollution of all kinds, particularly from land-based activities, and to minimize and address the impacts of ocean acidification. The Goal also aims to achieve sustainable yields in fisheries, through regulation of harvesting, controlling subsidies, and ending overfishing. It seeks to sustainably manage and protect marine and coastal ecosystems to avoid significant adverse impacts, including by strengthening their resilience, and take action for their restoration in order to achieve healthy and productive oceans.<p>**Company-Level Issue Examples** *- Impacts on water-related endangered species and habitats, Oil Spills, Seafood Sourcing.*| |**GOAL15LIFEONLAND**|**Life On Land** - Goal 15 seeks to ensure the conservation, restoration, and sustainable use of terrestrial and inland freshwater ecosystems and their services, in order to preserve biodiversity. It focuses specifically on sustainably managing forests, halting deforestation, restoring degraded lands and successfully combating desertification, reducing degraded natural habitats and ending biodiversity loss, with an emphasis on threatened species and invasive alien species.<p>**Company-Level Issue Examples** *- Impacts on land-related endangered species and habitats, Sustainable forestry practices and certifications, Project lifecycle environmental impacts.*| |**GOAL16PEACEJUSTICEANDSTRONGINSTITUTIONS**|**Peace, Justice, and Strong Institutions** - Goal 16 aims to significantly reduce all forms of violence, and also focuses specifically on reducing violence against children in the forms of abuse, exploitation, trafficking, and torture. It also aims to significantly reduce illicit financial and arms flows and to substantially reduce corruption and bribery in all their forms. The Goal also emphasizes effective and transparent institutions at all levels, inclusive and participatory decision-making, ensuring public access to information, and protection of fundamental freedoms.<p>**Company-Level Issue Examples** *- Tax Avoidance, Anti-Competitive Behavior, Cyber Security, Corruption, ESG Resolutions.*| . [optional] if omitted the server will use the default value of ["IMPACT"]
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            ApplyResult[(SdgArticlesResponse, int, typing.Dict)]
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
-        kwargs['ids'] = \
-            ids
-        kwargs['start_date'] = \
-            start_date
-        kwargs['end_date'] = \
-            end_date
-        return self.get_sdg_articles_endpoint.call_with_http_info(**kwargs)
-
-
-    def get_sdg_articles_for_list(
-        self,
-        sdg_articles_request,
-        **kwargs
-    ) -> SdgArticlesResponse:
-        """Request articles tagged with SDG lens categories from 2016-01-01 to previous day  # noqa: E501
-
-        Articles endpoint allows to retrieve underlying news articles used by the AI engine to calculate the ESG Scores of companies and therefore provides ESG relevant news and also transparency into the ESG Scores.   # noqa: E501
-        This method makes a synchronous HTTP request. Returns the http data only
-
-        Args:
-            sdg_articles_request (SdgArticlesRequest): The SDG Article metadata like Dates, Headlines, Articles, Volume
-
-        Keyword Args:
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            SdgArticlesResponse
-                Response Object
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
-        kwargs['sdg_articles_request'] = \
-            sdg_articles_request
-        return self.get_sdg_articles_for_list_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_articles_for_list_with_http_info(
-        self,
-        sdg_articles_request,
-        **kwargs
-    ) -> typing.Tuple[SdgArticlesResponse, int, typing.MutableMapping]:
-        """Request articles tagged with SDG lens categories from 2016-01-01 to previous day  # noqa: E501
-
-        Articles endpoint allows to retrieve underlying news articles used by the AI engine to calculate the ESG Scores of companies and therefore provides ESG relevant news and also transparency into the ESG Scores.   # noqa: E501
-        This method makes a synchronous HTTP request. Returns http data, http status and headers
-
-        Args:
-            sdg_articles_request (SdgArticlesRequest): The SDG Article metadata like Dates, Headlines, Articles, Volume
-
-        Keyword Args:
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            SdgArticlesResponse
-                Response Object
-            int
-                Http Status Code
-            dict
-                Dictionary of the response headers
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
-        kwargs['sdg_articles_request'] = \
-            sdg_articles_request
-        return self.get_sdg_articles_for_list_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_articles_for_list_async(
-        self,
-        sdg_articles_request,
-        **kwargs
-    ) -> "ApplyResult[SdgArticlesResponse]":
-        """Request articles tagged with SDG lens categories from 2016-01-01 to previous day  # noqa: E501
-
-        Articles endpoint allows to retrieve underlying news articles used by the AI engine to calculate the ESG Scores of companies and therefore provides ESG relevant news and also transparency into the ESG Scores.   # noqa: E501
-        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
-
-        Args:
-            sdg_articles_request (SdgArticlesRequest): The SDG Article metadata like Dates, Headlines, Articles, Volume
-
-        Keyword Args:
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            ApplyResult[SdgArticlesResponse]
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
-        kwargs['sdg_articles_request'] = \
-            sdg_articles_request
-        return self.get_sdg_articles_for_list_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_articles_for_list_with_http_info_async(
-        self,
-        sdg_articles_request,
-        **kwargs
-    ) -> "ApplyResult[typing.Tuple[SdgArticlesResponse, int, typing.MutableMapping]]":
-        """Request articles tagged with SDG lens categories from 2016-01-01 to previous day  # noqa: E501
-
-        Articles endpoint allows to retrieve underlying news articles used by the AI engine to calculate the ESG Scores of companies and therefore provides ESG relevant news and also transparency into the ESG Scores.   # noqa: E501
-        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
-
-        Args:
-            sdg_articles_request (SdgArticlesRequest): The SDG Article metadata like Dates, Headlines, Articles, Volume
-
-        Keyword Args:
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            ApplyResult[(SdgArticlesResponse, int, typing.Dict)]
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
-        kwargs['sdg_articles_request'] = \
-            sdg_articles_request
-        return self.get_sdg_articles_for_list_endpoint.call_with_http_info(**kwargs)
-
-
```

## fds/sdk/FactSetESG/api/sasb_api.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/api/spotlights_api.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -23,15 +23,14 @@
     file_type,
     none_type,
     validate_and_convert_types
 )
 from fds.sdk.FactSetESG.exceptions import ApiException
 from fds.sdk.FactSetESG.model.error_response import ErrorResponse
 from fds.sdk.FactSetESG.model.sasb_spotlights_request import SasbSpotlightsRequest
-from fds.sdk.FactSetESG.model.sdg_spotlights_request import SdgSpotlightsRequest
 from fds.sdk.FactSetESG.model.spotlights_response import SpotlightsResponse
 
 
 
 
 
 class SpotlightsApi(object):
@@ -190,162 +189,14 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
-        self.get_sdg_spotlights_endpoint = _Endpoint(
-            settings={
-                'response_type': (
-                  { 200: (SpotlightsResponse,), 400: (ErrorResponse,), 401: (ErrorResponse,), 403: (ErrorResponse,), 408: (ErrorResponse,), 415: (ErrorResponse,), 500: (ErrorResponse,),  },
-                  None
-                ),
-                'auth': [
-                    'FactSetApiKey',
-                    'FactSetOAuth2'
-                ],
-                'endpoint_path': '/factset-esg/v1/sdg-spotlights',
-                'operation_id': 'get_sdg_spotlights',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'ids',
-                    'start_date',
-                    'end_date',
-                    'categories',
-                    'fields',
-                    'primary_only',
-                    'is_removed',
-                ],
-                'required': [
-                    'ids',
-                    'start_date',
-                    'end_date',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'ids':
-                        ([str],),
-                    'start_date':
-                        (str,),
-                    'end_date':
-                        (str,),
-                    'categories':
-                        ([str],),
-                    'fields':
-                        ([str],),
-                    'primary_only':
-                        (bool,),
-                    'is_removed':
-                        (bool,),
-                },
-                'attribute_map': {
-                    'ids': 'ids',
-                    'start_date': 'startDate',
-                    'end_date': 'endDate',
-                    'categories': 'categories',
-                    'fields': 'fields',
-                    'primary_only': 'primaryOnly',
-                    'is_removed': 'isRemoved',
-                },
-                'location_map': {
-                    'ids': 'query',
-                    'start_date': 'query',
-                    'end_date': 'query',
-                    'categories': 'query',
-                    'fields': 'query',
-                    'primary_only': 'query',
-                    'is_removed': 'query',
-                },
-                'collection_format_map': {
-                    'ids': 'csv',
-                    'categories': 'csv',
-                    'fields': 'csv',
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-
-        self.get_sdg_spotlights_for_list_endpoint = _Endpoint(
-            settings={
-                'response_type': (
-                  { 200: (SpotlightsResponse,), 400: (ErrorResponse,), 401: (ErrorResponse,), 403: (ErrorResponse,), 408: (ErrorResponse,), 415: (ErrorResponse,), 500: (ErrorResponse,),  },
-                  None
-                ),
-                'auth': [
-                    'FactSetApiKey',
-                    'FactSetOAuth2'
-                ],
-                'endpoint_path': '/factset-esg/v1/sdg-spotlights',
-                'operation_id': 'get_sdg_spotlights_for_list',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'sdg_spotlights_request',
-                ],
-                'required': [
-                    'sdg_spotlights_request',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'sdg_spotlights_request':
-                        (SdgSpotlightsRequest,),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'sdg_spotlights_request': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-
 
     @staticmethod
     def apply_kwargs_defaults(kwargs, return_http_data_only, async_req):
         kwargs["async_req"] = async_req
         kwargs["_return_http_data_only"] = return_http_data_only
         kwargs["_preload_content"] = kwargs.get("_preload_content", True)
         kwargs["_request_timeout"] = kwargs.get("_request_timeout", None)
@@ -372,15 +223,15 @@
             ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
             start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
             end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
 
         Keyword Args:
             fields ([str]): Request available SASB Spotlights data fields to be included in the response.  Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |orgId|Unique identifier assigned by Truvalue that is applied on an organization level |             |date|Date for the period requested in YYYY-MM-DD format.|   |spotlightId|Unique identifier identifying a Spotlight ESG event that is detected at the company level, within a single category.|   |groupId|Unique identifier  identifying a Spotlight group using the Spotlight ID of the Primary Spotlight.|   |requestId|Identifier that was used for the request.|     <h3>SASB Spotlights Fields</h3>     |field|description|   |---|---|   |orgName|The current name of the organization (not point-in-time)|   |primarySpotlight|Y/N value indicating the primary Spotlight in a Spotlight Group.|   |spotlightCategory|SASB category tagged to each Spotlight.|   |materialCategory|Indicates if the category is material for the organization based on SASBs Materiality Map|   |status|Indicates status of a spotlight, which can be one of Completed or Ongoing.|   |removed|Displays the date a Spotlight was removed from the dataset, if it has been removed.|   |startDate|Date when a Spotlight has met the volume threshold for Spotlight consideration. Score and volume change metadata are associated with this date.|   |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start date|   |firstArticleDate|Date of earliest article in the Spotlight as of the Start Date.|   |finalArticleDate|Date of final article in the Spotlight. This value can change over the course of the Spotlight until the Spotlight is marked as completed.|   |organizationVolumeThreshold|The article volume needed to create a Spotlight, as set by the company's overall volume level classification on the Start Date.|   |totalSpotlightVolume|Total number of articles in the Spotlight. This number will change until the Spotlight is marked as completed.|   |startDateVolume|Number of articles in the Spotlight on the Start Date when it met the volume threshold. Does not include the number of articles that were added to the Spotlight after the Spotlight Start Date.|   |primaryArticleSource|Source of the primary article.|   |primaryArticleUrl|URL of the primary article.|   |primaryArticleHeadline|Headline of primary Spotlight article.|   |primaryArticleBulletpoints|Bullet points summarizing the primary article.|   |meanArtScoreFinalDate|Average score of articles in Spotlight on Final Article Date. This score will continue to change until the Spotlight is marked as completed.|   |meanArtScoreStartDate|Average score of articles in Spotlight on Start Date. This score will not change throughout the history of the spotlight.|   |meanPulseScore|Average of pulse scores for each day from First Article Date to Final Article Date, including scores for both Start Date and Final Article Date.|   |pulseBeforeFirstArticle|Pulse score for category at end-of-day on day before the First Article Date|   |pulseOnFinalArticleDate|Pulse score for category at the end-of-day on the Final Article Date.|   |pulseOnStartDate|Pulse score for the category at the end-of-day on the Start Date.|   |zScoreOnFinalDate|Z-score for Spotlight as of Final Article Date. This score will continue to change until the Spotlight is marked as completed.|   |zScoreOnStartDate|Z-score for Spotlight as of Start Date. This score will not change throughout the history of the spotlight.|   |standoutLvlOnFinalDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.  This score will continue to change until the Spotlight is marked as completed.|   |standoutLvlOnStartDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.| . [optional]
             categories ([str]): The SASB Categories requested for the respective scoreType(s). The default value is **ALLCATEGORIES**, which represents all 26 categories in a single overall score. To request a specifc category or list of categories, simply input the category names below.   ### SASB Categories |**SASB Category Inputs**|**Description**| |---|---| |**ALLCATEGORIES**|**All Categories** - this category represents a company's overall SASB Score for the specific 'scoreType'. This value is equal to the cumulative average of all 26 SASB categories for the specific 'scoreType'.*Note that category is not available for the Dynamic Materiality 'scoreType'.| |**ACCESSANDAFFORDABILITY**|**Access and Affordability** - The category addresses a company's ability to ensure broad access to its products and services, specifically in the context of underserved markets and/or population groups. It includes the management of issues related to universal needs, such as the accessibility and affordability of health care, financial services, utilities , education, and telecommunications.| |**AIRQUALITY**|**Air Quality** - the category addresses management of air quality impacts resulting from stationary (e.g., factories, power plants) and mobile sources (e.g., trucks, delivery vehicles, planes) as well as industrial emissions. Relevant airborne pollutants include, but are not limited to, oxides of nitrogen (NOx), oxides of sulfur (SOx), volatile organic compounds (VOCs), heavy metals, particulate matter, and chlorofluorocarbons. The category does not include GHG emissions, which are addressed in a separate category.| |**BUSINESSETHICS**|**Business Ethics** - the category addresses the company's approach to managing risks and opportunities surrounding ethical conduct of business, including fraud, corruption, bribery and facilitation payments, fiduciary responsibilities, and other behavior that may have an ethical component. This includes sensitivity to business norms and standards as they shift over time, jurisdiction, and culture. It addresses the company's ability to provide services that satisfy the highest professional and ethical standards of the industry, which means to avoid conflicts of interest, misrepresentation, bias, and negligence through training employees adequately and implementing policies and procedures to ensure employees provide services free from bias and error.| |**BUSMODELRESILIENCE**|**Business Model Resilience** - the category addresses an industry's capacity to manage risks and opportunities associated with incorporating social, environmental, and political transitions into long-term business model planning. This includes responsiveness to the transition to a low-carbon and climate-constrained economy, as well as growth and creation of new markets among unserved and underserved socioeconomic populations. The category highlights industries in which evolving environmental and social realities may challenge companies to fundamentally adapt or may put their business models at risk.| |**COMPETITIVEBEHAVIOR**|**Competitive Behavior** - the category covers social issues associated with existence of monopolies, which may include, but are not limited to, excessive prices, poor quality of service, and inefficiencies. It addresses a company's management of legal and social expectation around monopolistic and anti-competitive practices, including issues related to bargaining power, collusion, price fixing or manipulation, and protection of patents and intellectual property (IP).| |**CRITINCIDENTRISKMGT**|**Critical Incident Risk Management** - the category addresses the company's use of management systems and scenario planning to identify, understand, and prevent or minimize the occurrence of low-probability, high-impact accidents and emergencies with significant potential environmental and social externalities. It relates to the culture of safety at a company, its relevant safety management systems and technological controls, the potential human, environmental, and social implications of such events occurring, and the long-term effects to an organization, its workers, and society should these events occur.| |**CUSTOMERPRIVACY**|**Customer Privacy** - the category addresses management of risks related to the use of personally identifiable information (PII) and other customer or user data for secondary purposes including but not limited to marketing through affiliates and non-affiliates. The scope of the category includes social issues that may arise from a company's approach to collecting data, obtaining consent (e.g., opt-in policies), managing user and customer expectations regarding how their data is used, and managing evolving regulation. It excludes social issues arising from cybersecurity risks, which are covered in a separate category.| |**CUSTWELFARE**|**Customer Welfare** - the category addresses customer welfare concerns over issues including, but not limited to, health and nutrition of foods and beverages, antibiotic use in animal production, and management of controlled substances. The category addresses the company's ability to provide consumers with manufactured products and services that are aligned with societal expectations. It does not include issues directly related to quality and safety malfunctions of manufactured products and services, but instead addresses qualities inherent to the design and delivery of products and services where customer welfare may be in question. The scope of the category also captures companies' ability to prevent counterfeit products.| |**DATASECURITY**|**Data Security** - the category addresses management of risks related to collection, retention, and use of sensitive, confidential, and/or proprietary customer or user data. It includes social issues that may arise from incidents such as data breaches in which personally identifiable information (PII) and other user or customer data may be exposed. It addresses a company's strategy, policies, and practices related to IT infrastructure, staff training, record keeping, cooperation with law enforcement, and other mechanisms used to ensure security of customer or user data.| |**ECOLOGICALIMPACTS**|**Ecological Impacts** - the category addresses management of the company's impacts on ecosystems and biodiversity through activities including, but not limited to, land use for exploration, natural resource extraction, and cultivation, as well as project development, construction, and siting. The impacts include, but are not limited to, biodiversity loss, habitat destruction, and deforestation at all stages – planning, land acquisition, permitting, development, operations, and site remediation. The category does not cover impacts of climate change on ecosystems and biodiversity.| |**EMPENGDIVANDINC**|**Employee Engagement Diversity and Inclusion** - the category addresses a company's ability to ensure that its culture and hiring and promotion practices embrace the building of a diverse and inclusive workforce that reflects the makeup of local talent pools and its customer base. It addresses the issues of discriminatory practices on the bases of race, gender, ethnicity, religion, sexual orientation, and other factors.| |**EMPHEALTHANDSAFETY**|**Employee Health and Safety** - the category addresses a company's ability to create and maintain a safe and healthy workplace environment that is free of injuries, fatalities, and illness (both chronic and acute). It is traditionally accomplished through implementing safety management plans, developing training requirements for employees and contractors, and conducting regular audits of their own practices as well as those of their subcontractors. The category further captures how companies ensure physical and mental health of workforce through technology, training, corporate culture, regulatory compliance, monitoring and testing, and personal protective equipment.| |**ENERGYMGT**|**Energy Management** - the category addresses environmental impacts associated with energy consumption. It addresses the company's management of energy in manufacturing and/or for provision of products and services derived from utility providers (grid energy) not owned or controlled by the company. More specifically, it includes management of energy efficiency and intensity, energy mix, as well as grid reliance. Upstream (e.g., suppliers) and downstream (e.g., product use) energy use is not included in the scope.| |**GHGEMISSIONS**|**Greenhouse Gas Emissions** - the category addresses direct (Scope 1) greenhouse gas (GHG) emissions that a company generates through its operations. This includes GHG emissions from stationary (e.g., factories, power plants) and mobile sources (e.g., trucks, delivery vehicles, planes), whether a result of combustion of fuel or non-combusted direct releases during activities such as natural resource extraction, power generation, land use, or biogenic processes. The category further includes management of regulatory risks, environmental compliance, and reputational risks and opportunities, as they related to direct GHG emissions. The seven GHGs covered under the Kyoto Protocol are included within the category— carbon dioxide (CO2 ), methane (CH4), nitrous oxide (N2O), hydrofluorocarbons (HFCs), perfluorocarbons (PFCs), sulfur hexafluoride (SF6), and nitrogen trifluoride (NF3).| |**HUMANRIGHTSANDCOMRELS**|**Human Rights and Community Relations** - the category addresses management of the relationship between businesses and the communities in which they operate, including, but not limited to, management of direct and indirect impacts on core human rights and the treatment of indigenous peoples. More specifically, such management may cover socio-economic community impacts, community engagement, environmental justice, cultivation of local workforces, impact on local businesses, license to operate, and environmental/social impact assessments. The category does not include environmental impacts such as air pollution or waste which, although they may impact the health and safety of members of local communities, are addressed in separate categories.| |**LABORPRACTICES**|**Labor Practices** - the category addresses the company's ability to uphold commonly accepted labor standards in the workplace, including compliance with labor laws and internationally accepted norms and standards. This includes, but is not limited to, ensuring basic human rights related to child labor, forced or bonded labor, exploitative labor, fair wages and overtime pay, and other basic workers' rights. It also includes minimum wage policies and provision of benefits, which may influence how a workforce is attracted, retained, and motivated. The category further addresses a company's relationship with organized labor and freedom of association.| |**MGTOFLEGALANDREGENV**|**Management of the Legal and Regulatory Environment** - the category addresses a company's approach to engaging with regulators in cases where conflicting corporate and public interests may have the potential for long-term adverse direct or indirect environmental and social impacts. The category addresses a company's level of reliance upon regulatory policy or monetary incentives (such as subsidies and taxes), actions to influence industry policy (such as through lobbying), overall reliance on a favorable regulatory environment for business competitiveness, and ability to comply with relevant regulations. It may relate to the alignment of management and investor views of regulatory engagement and compliance at large.| |**MATSOURCINGANDEFF**|**Materials Sourcing and Efficiency** - the category addresses issues related to the resilience of materials supply chains to impacts of climate change and other external environmental and social factors. It captures the impacts of such external factors on operational activity of suppliers, which can further affect availability and pricing of key resources. It addresses a company's ability to manage these risks through product design, manufacturing, and end-of-life management, such as by using of recycled and renewable materials, reducing the use of key materials (dematerialization), maximizing resource efficiency in manufacturing, and making R&D investments in substitute materials. Additionally, companies can manage these issues by screening, selection, monitoring, and engagement with suppliers to ensure their resilience to external risks. It does not address issues associated with environmental and social externalities created by operational activity of individual suppliers, which is covered in a separate category.| |**MATERIALITY**|**Materiality** - this category represents a composite score of all 'material' SASB categories for the given entity. For more information on SASB's Materiality Map, visit [materiality.sasb.org](https://materiality.sasb.org/)| |**PHYIMPACTSOFCLIMATECHG**|**Physical Impacts of Climate Change** - the category addresses the company's ability to manage risks and opportunities associated with direct exposure of its owned or controlled assets and operations to actual or potential physical impacts of climate change. It captures environmental and social issues that may arise from operational disruptions due to physical impacts of climate change. It further captures socioeconomic issues resulting from companies failing to incorporate climate change consideration in products and services sold, such as insurance policies and mortgages. The category relates to the company's ability to adapt to increased frequency and severity of extreme weather, shifting climate, sea level risk, and other expected physical impacts of climate change. Management may involve enhancing resiliency of physical assets and/or surrounding infrastructure as well as incorporation of climate change-related considerations into key business activities (e.g., mortgage and insurance underwriting, planning and development of real estate projects).| |**PDANDLIFECYCLEMGT**|**Product Design and Lifecycle Management** - the category addresses incorporation of environmental, social, and governance (ESG) considerations in characteristics of products and services provided or sold by the company. It includes, but is not limited to, managing the lifecycle impacts of products and services, such as those related to packaging, distribution, use-phase resource intensity, and other environmental and social externalities that may occur during their use-phase or at the end of life. The category captures a company's ability to address customer and societal demand for more sustainable products and services as well as to meet evolving environmental and social regulation. It does not address direct environmental or social impacts of the company's operations nor does it address health and safety risks to consumers from product use, which are covered in other categories.| |**PRODQUALITYANDSFTY**|**Product Quality and Safety** - the category addresses issues involving unintended characteristics of products sold or services provided that may create health or safety risks to end-users. It addresses a company's ability to offer manufactured products and/or services that meet customer expectations with respect to their health and safety characteristics. It includes, but is not limited to, issues involving liability, management of recalls and market withdrawals, product testing, and chemicals/content/ ingredient management in products.| |**SELLPRACANDPRODLABEL**|**Selling Practices and Product Labeling** - the category addresses social issues that may arise from a failure to manage the transparency, accuracy, and comprehensibility of marketing statements, advertising, and labeling of products and services. It includes, but is not limited to, advertising standards and regulations, ethical and responsible marketing practices, misleading or deceptive labeling, as well as discriminatory or predatory selling and lending practices. This may include deceptive or aggressive selling practices in which incentive structures for employees could encourage the sale of products or services that are not in the best interest of customers or clients.| |**SUPPLYCHAINMGT**|**Supply Chain Management** - the category addresses management of environmental, social, and governance (ESG) risks within a company's supply chain. It addresses issues associated with environmental and social externalities created by suppliers through their operational activities. Such issues include, but are not limited to, environmental responsibility, human rights, labor practices, and ethics and corruption. Management may involve screening, selection, monitoring, and engagement with suppliers on their environmental and social impacts. The category does not address the impacts of external factors – such as climate change and other environmental and social factors – on suppliers' operations and/or on the availability and pricing of key resources, which is covered in a separate category.| |**SYSTEMICRISKMGT**|**Systemic Risk Management** - the category addresses the company's contributions to, or management of systemic risks resulting from large-scale weakening or collapse of systems upon which the economy and society depend. This includes financial systems, natural resource systems, and technological systems. It addresses the mechanisms a company has in place to reduce its contributions to systemic risks and to improve safeguards that may mitigate the impacts of systemic failure. For financial institutions, the category also captures the company's ability to absorb shocks arising from financial and economic stress and meet stricter regulatory requirements related to the complexity and interconnectedness of companies in the industry.| |**WASTEANDHZRDMATSMGT**|**Waste and Hazardous Materials Management** - the category addresses environmental issues associated with hazardous and non-hazardous waste generated by companies. It addresses a company's management of solid wastes in manufacturing, agriculture, and other industrial processes. It covers treatment, handling, storage, disposal, and regulatory compliance. The category does not cover emissions to air or wastewater, nor does it cover waste from end-of-life of products, which are addressed in separate categories.| |**WATERANDWASTEWATERMGT**|**Water and Wastewater Management** - the category addresses a company's water use, water consumption, wastewater generation, and other impacts of operations on water resources, which may be influenced by regional differences in the availability and quality of and competition for water resources. More specifically, it addresses management strategies including, but not limited to, water efficiency, intensity, and recycling. Lastly, the category also addresses management of wastewater treatment and discharge, including groundwater and aquifer pollution.| . [optional] if omitted the server will use the default value of ["ALLCATEGORIES"]
-            primary_only (bool): This parameter would return only primary spotlights when set to `true` . [optional] if omitted the server will use the default value of True
+            primary_only (bool): This parameter would return only primary spotlights when set to `true`    . [optional] if omitted the server will use the default value of True
             is_removed (bool): This parameter would return the spotlights removed in the response(i.e. Spotlight is marked as Rejected but has a firstApprovedOnDate))when set to `true` Only Spotlights that are marked as approved will be returned when set to `false` . [optional] if omitted the server will use the default value of False
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -431,15 +282,15 @@
             ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
             start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
             end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
 
         Keyword Args:
             fields ([str]): Request available SASB Spotlights data fields to be included in the response.  Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |orgId|Unique identifier assigned by Truvalue that is applied on an organization level |             |date|Date for the period requested in YYYY-MM-DD format.|   |spotlightId|Unique identifier identifying a Spotlight ESG event that is detected at the company level, within a single category.|   |groupId|Unique identifier  identifying a Spotlight group using the Spotlight ID of the Primary Spotlight.|   |requestId|Identifier that was used for the request.|     <h3>SASB Spotlights Fields</h3>     |field|description|   |---|---|   |orgName|The current name of the organization (not point-in-time)|   |primarySpotlight|Y/N value indicating the primary Spotlight in a Spotlight Group.|   |spotlightCategory|SASB category tagged to each Spotlight.|   |materialCategory|Indicates if the category is material for the organization based on SASBs Materiality Map|   |status|Indicates status of a spotlight, which can be one of Completed or Ongoing.|   |removed|Displays the date a Spotlight was removed from the dataset, if it has been removed.|   |startDate|Date when a Spotlight has met the volume threshold for Spotlight consideration. Score and volume change metadata are associated with this date.|   |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start date|   |firstArticleDate|Date of earliest article in the Spotlight as of the Start Date.|   |finalArticleDate|Date of final article in the Spotlight. This value can change over the course of the Spotlight until the Spotlight is marked as completed.|   |organizationVolumeThreshold|The article volume needed to create a Spotlight, as set by the company's overall volume level classification on the Start Date.|   |totalSpotlightVolume|Total number of articles in the Spotlight. This number will change until the Spotlight is marked as completed.|   |startDateVolume|Number of articles in the Spotlight on the Start Date when it met the volume threshold. Does not include the number of articles that were added to the Spotlight after the Spotlight Start Date.|   |primaryArticleSource|Source of the primary article.|   |primaryArticleUrl|URL of the primary article.|   |primaryArticleHeadline|Headline of primary Spotlight article.|   |primaryArticleBulletpoints|Bullet points summarizing the primary article.|   |meanArtScoreFinalDate|Average score of articles in Spotlight on Final Article Date. This score will continue to change until the Spotlight is marked as completed.|   |meanArtScoreStartDate|Average score of articles in Spotlight on Start Date. This score will not change throughout the history of the spotlight.|   |meanPulseScore|Average of pulse scores for each day from First Article Date to Final Article Date, including scores for both Start Date and Final Article Date.|   |pulseBeforeFirstArticle|Pulse score for category at end-of-day on day before the First Article Date|   |pulseOnFinalArticleDate|Pulse score for category at the end-of-day on the Final Article Date.|   |pulseOnStartDate|Pulse score for the category at the end-of-day on the Start Date.|   |zScoreOnFinalDate|Z-score for Spotlight as of Final Article Date. This score will continue to change until the Spotlight is marked as completed.|   |zScoreOnStartDate|Z-score for Spotlight as of Start Date. This score will not change throughout the history of the spotlight.|   |standoutLvlOnFinalDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.  This score will continue to change until the Spotlight is marked as completed.|   |standoutLvlOnStartDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.| . [optional]
             categories ([str]): The SASB Categories requested for the respective scoreType(s). The default value is **ALLCATEGORIES**, which represents all 26 categories in a single overall score. To request a specifc category or list of categories, simply input the category names below.   ### SASB Categories |**SASB Category Inputs**|**Description**| |---|---| |**ALLCATEGORIES**|**All Categories** - this category represents a company's overall SASB Score for the specific 'scoreType'. This value is equal to the cumulative average of all 26 SASB categories for the specific 'scoreType'.*Note that category is not available for the Dynamic Materiality 'scoreType'.| |**ACCESSANDAFFORDABILITY**|**Access and Affordability** - The category addresses a company's ability to ensure broad access to its products and services, specifically in the context of underserved markets and/or population groups. It includes the management of issues related to universal needs, such as the accessibility and affordability of health care, financial services, utilities , education, and telecommunications.| |**AIRQUALITY**|**Air Quality** - the category addresses management of air quality impacts resulting from stationary (e.g., factories, power plants) and mobile sources (e.g., trucks, delivery vehicles, planes) as well as industrial emissions. Relevant airborne pollutants include, but are not limited to, oxides of nitrogen (NOx), oxides of sulfur (SOx), volatile organic compounds (VOCs), heavy metals, particulate matter, and chlorofluorocarbons. The category does not include GHG emissions, which are addressed in a separate category.| |**BUSINESSETHICS**|**Business Ethics** - the category addresses the company's approach to managing risks and opportunities surrounding ethical conduct of business, including fraud, corruption, bribery and facilitation payments, fiduciary responsibilities, and other behavior that may have an ethical component. This includes sensitivity to business norms and standards as they shift over time, jurisdiction, and culture. It addresses the company's ability to provide services that satisfy the highest professional and ethical standards of the industry, which means to avoid conflicts of interest, misrepresentation, bias, and negligence through training employees adequately and implementing policies and procedures to ensure employees provide services free from bias and error.| |**BUSMODELRESILIENCE**|**Business Model Resilience** - the category addresses an industry's capacity to manage risks and opportunities associated with incorporating social, environmental, and political transitions into long-term business model planning. This includes responsiveness to the transition to a low-carbon and climate-constrained economy, as well as growth and creation of new markets among unserved and underserved socioeconomic populations. The category highlights industries in which evolving environmental and social realities may challenge companies to fundamentally adapt or may put their business models at risk.| |**COMPETITIVEBEHAVIOR**|**Competitive Behavior** - the category covers social issues associated with existence of monopolies, which may include, but are not limited to, excessive prices, poor quality of service, and inefficiencies. It addresses a company's management of legal and social expectation around monopolistic and anti-competitive practices, including issues related to bargaining power, collusion, price fixing or manipulation, and protection of patents and intellectual property (IP).| |**CRITINCIDENTRISKMGT**|**Critical Incident Risk Management** - the category addresses the company's use of management systems and scenario planning to identify, understand, and prevent or minimize the occurrence of low-probability, high-impact accidents and emergencies with significant potential environmental and social externalities. It relates to the culture of safety at a company, its relevant safety management systems and technological controls, the potential human, environmental, and social implications of such events occurring, and the long-term effects to an organization, its workers, and society should these events occur.| |**CUSTOMERPRIVACY**|**Customer Privacy** - the category addresses management of risks related to the use of personally identifiable information (PII) and other customer or user data for secondary purposes including but not limited to marketing through affiliates and non-affiliates. The scope of the category includes social issues that may arise from a company's approach to collecting data, obtaining consent (e.g., opt-in policies), managing user and customer expectations regarding how their data is used, and managing evolving regulation. It excludes social issues arising from cybersecurity risks, which are covered in a separate category.| |**CUSTWELFARE**|**Customer Welfare** - the category addresses customer welfare concerns over issues including, but not limited to, health and nutrition of foods and beverages, antibiotic use in animal production, and management of controlled substances. The category addresses the company's ability to provide consumers with manufactured products and services that are aligned with societal expectations. It does not include issues directly related to quality and safety malfunctions of manufactured products and services, but instead addresses qualities inherent to the design and delivery of products and services where customer welfare may be in question. The scope of the category also captures companies' ability to prevent counterfeit products.| |**DATASECURITY**|**Data Security** - the category addresses management of risks related to collection, retention, and use of sensitive, confidential, and/or proprietary customer or user data. It includes social issues that may arise from incidents such as data breaches in which personally identifiable information (PII) and other user or customer data may be exposed. It addresses a company's strategy, policies, and practices related to IT infrastructure, staff training, record keeping, cooperation with law enforcement, and other mechanisms used to ensure security of customer or user data.| |**ECOLOGICALIMPACTS**|**Ecological Impacts** - the category addresses management of the company's impacts on ecosystems and biodiversity through activities including, but not limited to, land use for exploration, natural resource extraction, and cultivation, as well as project development, construction, and siting. The impacts include, but are not limited to, biodiversity loss, habitat destruction, and deforestation at all stages – planning, land acquisition, permitting, development, operations, and site remediation. The category does not cover impacts of climate change on ecosystems and biodiversity.| |**EMPENGDIVANDINC**|**Employee Engagement Diversity and Inclusion** - the category addresses a company's ability to ensure that its culture and hiring and promotion practices embrace the building of a diverse and inclusive workforce that reflects the makeup of local talent pools and its customer base. It addresses the issues of discriminatory practices on the bases of race, gender, ethnicity, religion, sexual orientation, and other factors.| |**EMPHEALTHANDSAFETY**|**Employee Health and Safety** - the category addresses a company's ability to create and maintain a safe and healthy workplace environment that is free of injuries, fatalities, and illness (both chronic and acute). It is traditionally accomplished through implementing safety management plans, developing training requirements for employees and contractors, and conducting regular audits of their own practices as well as those of their subcontractors. The category further captures how companies ensure physical and mental health of workforce through technology, training, corporate culture, regulatory compliance, monitoring and testing, and personal protective equipment.| |**ENERGYMGT**|**Energy Management** - the category addresses environmental impacts associated with energy consumption. It addresses the company's management of energy in manufacturing and/or for provision of products and services derived from utility providers (grid energy) not owned or controlled by the company. More specifically, it includes management of energy efficiency and intensity, energy mix, as well as grid reliance. Upstream (e.g., suppliers) and downstream (e.g., product use) energy use is not included in the scope.| |**GHGEMISSIONS**|**Greenhouse Gas Emissions** - the category addresses direct (Scope 1) greenhouse gas (GHG) emissions that a company generates through its operations. This includes GHG emissions from stationary (e.g., factories, power plants) and mobile sources (e.g., trucks, delivery vehicles, planes), whether a result of combustion of fuel or non-combusted direct releases during activities such as natural resource extraction, power generation, land use, or biogenic processes. The category further includes management of regulatory risks, environmental compliance, and reputational risks and opportunities, as they related to direct GHG emissions. The seven GHGs covered under the Kyoto Protocol are included within the category— carbon dioxide (CO2 ), methane (CH4), nitrous oxide (N2O), hydrofluorocarbons (HFCs), perfluorocarbons (PFCs), sulfur hexafluoride (SF6), and nitrogen trifluoride (NF3).| |**HUMANRIGHTSANDCOMRELS**|**Human Rights and Community Relations** - the category addresses management of the relationship between businesses and the communities in which they operate, including, but not limited to, management of direct and indirect impacts on core human rights and the treatment of indigenous peoples. More specifically, such management may cover socio-economic community impacts, community engagement, environmental justice, cultivation of local workforces, impact on local businesses, license to operate, and environmental/social impact assessments. The category does not include environmental impacts such as air pollution or waste which, although they may impact the health and safety of members of local communities, are addressed in separate categories.| |**LABORPRACTICES**|**Labor Practices** - the category addresses the company's ability to uphold commonly accepted labor standards in the workplace, including compliance with labor laws and internationally accepted norms and standards. This includes, but is not limited to, ensuring basic human rights related to child labor, forced or bonded labor, exploitative labor, fair wages and overtime pay, and other basic workers' rights. It also includes minimum wage policies and provision of benefits, which may influence how a workforce is attracted, retained, and motivated. The category further addresses a company's relationship with organized labor and freedom of association.| |**MGTOFLEGALANDREGENV**|**Management of the Legal and Regulatory Environment** - the category addresses a company's approach to engaging with regulators in cases where conflicting corporate and public interests may have the potential for long-term adverse direct or indirect environmental and social impacts. The category addresses a company's level of reliance upon regulatory policy or monetary incentives (such as subsidies and taxes), actions to influence industry policy (such as through lobbying), overall reliance on a favorable regulatory environment for business competitiveness, and ability to comply with relevant regulations. It may relate to the alignment of management and investor views of regulatory engagement and compliance at large.| |**MATSOURCINGANDEFF**|**Materials Sourcing and Efficiency** - the category addresses issues related to the resilience of materials supply chains to impacts of climate change and other external environmental and social factors. It captures the impacts of such external factors on operational activity of suppliers, which can further affect availability and pricing of key resources. It addresses a company's ability to manage these risks through product design, manufacturing, and end-of-life management, such as by using of recycled and renewable materials, reducing the use of key materials (dematerialization), maximizing resource efficiency in manufacturing, and making R&D investments in substitute materials. Additionally, companies can manage these issues by screening, selection, monitoring, and engagement with suppliers to ensure their resilience to external risks. It does not address issues associated with environmental and social externalities created by operational activity of individual suppliers, which is covered in a separate category.| |**MATERIALITY**|**Materiality** - this category represents a composite score of all 'material' SASB categories for the given entity. For more information on SASB's Materiality Map, visit [materiality.sasb.org](https://materiality.sasb.org/)| |**PHYIMPACTSOFCLIMATECHG**|**Physical Impacts of Climate Change** - the category addresses the company's ability to manage risks and opportunities associated with direct exposure of its owned or controlled assets and operations to actual or potential physical impacts of climate change. It captures environmental and social issues that may arise from operational disruptions due to physical impacts of climate change. It further captures socioeconomic issues resulting from companies failing to incorporate climate change consideration in products and services sold, such as insurance policies and mortgages. The category relates to the company's ability to adapt to increased frequency and severity of extreme weather, shifting climate, sea level risk, and other expected physical impacts of climate change. Management may involve enhancing resiliency of physical assets and/or surrounding infrastructure as well as incorporation of climate change-related considerations into key business activities (e.g., mortgage and insurance underwriting, planning and development of real estate projects).| |**PDANDLIFECYCLEMGT**|**Product Design and Lifecycle Management** - the category addresses incorporation of environmental, social, and governance (ESG) considerations in characteristics of products and services provided or sold by the company. It includes, but is not limited to, managing the lifecycle impacts of products and services, such as those related to packaging, distribution, use-phase resource intensity, and other environmental and social externalities that may occur during their use-phase or at the end of life. The category captures a company's ability to address customer and societal demand for more sustainable products and services as well as to meet evolving environmental and social regulation. It does not address direct environmental or social impacts of the company's operations nor does it address health and safety risks to consumers from product use, which are covered in other categories.| |**PRODQUALITYANDSFTY**|**Product Quality and Safety** - the category addresses issues involving unintended characteristics of products sold or services provided that may create health or safety risks to end-users. It addresses a company's ability to offer manufactured products and/or services that meet customer expectations with respect to their health and safety characteristics. It includes, but is not limited to, issues involving liability, management of recalls and market withdrawals, product testing, and chemicals/content/ ingredient management in products.| |**SELLPRACANDPRODLABEL**|**Selling Practices and Product Labeling** - the category addresses social issues that may arise from a failure to manage the transparency, accuracy, and comprehensibility of marketing statements, advertising, and labeling of products and services. It includes, but is not limited to, advertising standards and regulations, ethical and responsible marketing practices, misleading or deceptive labeling, as well as discriminatory or predatory selling and lending practices. This may include deceptive or aggressive selling practices in which incentive structures for employees could encourage the sale of products or services that are not in the best interest of customers or clients.| |**SUPPLYCHAINMGT**|**Supply Chain Management** - the category addresses management of environmental, social, and governance (ESG) risks within a company's supply chain. It addresses issues associated with environmental and social externalities created by suppliers through their operational activities. Such issues include, but are not limited to, environmental responsibility, human rights, labor practices, and ethics and corruption. Management may involve screening, selection, monitoring, and engagement with suppliers on their environmental and social impacts. The category does not address the impacts of external factors – such as climate change and other environmental and social factors – on suppliers' operations and/or on the availability and pricing of key resources, which is covered in a separate category.| |**SYSTEMICRISKMGT**|**Systemic Risk Management** - the category addresses the company's contributions to, or management of systemic risks resulting from large-scale weakening or collapse of systems upon which the economy and society depend. This includes financial systems, natural resource systems, and technological systems. It addresses the mechanisms a company has in place to reduce its contributions to systemic risks and to improve safeguards that may mitigate the impacts of systemic failure. For financial institutions, the category also captures the company's ability to absorb shocks arising from financial and economic stress and meet stricter regulatory requirements related to the complexity and interconnectedness of companies in the industry.| |**WASTEANDHZRDMATSMGT**|**Waste and Hazardous Materials Management** - the category addresses environmental issues associated with hazardous and non-hazardous waste generated by companies. It addresses a company's management of solid wastes in manufacturing, agriculture, and other industrial processes. It covers treatment, handling, storage, disposal, and regulatory compliance. The category does not cover emissions to air or wastewater, nor does it cover waste from end-of-life of products, which are addressed in separate categories.| |**WATERANDWASTEWATERMGT**|**Water and Wastewater Management** - the category addresses a company's water use, water consumption, wastewater generation, and other impacts of operations on water resources, which may be influenced by regional differences in the availability and quality of and competition for water resources. More specifically, it addresses management strategies including, but not limited to, water efficiency, intensity, and recycling. Lastly, the category also addresses management of wastewater treatment and discharge, including groundwater and aquifer pollution.| . [optional] if omitted the server will use the default value of ["ALLCATEGORIES"]
-            primary_only (bool): This parameter would return only primary spotlights when set to `true` . [optional] if omitted the server will use the default value of True
+            primary_only (bool): This parameter would return only primary spotlights when set to `true`    . [optional] if omitted the server will use the default value of True
             is_removed (bool): This parameter would return the spotlights removed in the response(i.e. Spotlight is marked as Rejected but has a firstApprovedOnDate))when set to `true` Only Spotlights that are marked as approved will be returned when set to `false` . [optional] if omitted the server will use the default value of False
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -494,15 +345,15 @@
             ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
             start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
             end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
 
         Keyword Args:
             fields ([str]): Request available SASB Spotlights data fields to be included in the response.  Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |orgId|Unique identifier assigned by Truvalue that is applied on an organization level |             |date|Date for the period requested in YYYY-MM-DD format.|   |spotlightId|Unique identifier identifying a Spotlight ESG event that is detected at the company level, within a single category.|   |groupId|Unique identifier  identifying a Spotlight group using the Spotlight ID of the Primary Spotlight.|   |requestId|Identifier that was used for the request.|     <h3>SASB Spotlights Fields</h3>     |field|description|   |---|---|   |orgName|The current name of the organization (not point-in-time)|   |primarySpotlight|Y/N value indicating the primary Spotlight in a Spotlight Group.|   |spotlightCategory|SASB category tagged to each Spotlight.|   |materialCategory|Indicates if the category is material for the organization based on SASBs Materiality Map|   |status|Indicates status of a spotlight, which can be one of Completed or Ongoing.|   |removed|Displays the date a Spotlight was removed from the dataset, if it has been removed.|   |startDate|Date when a Spotlight has met the volume threshold for Spotlight consideration. Score and volume change metadata are associated with this date.|   |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start date|   |firstArticleDate|Date of earliest article in the Spotlight as of the Start Date.|   |finalArticleDate|Date of final article in the Spotlight. This value can change over the course of the Spotlight until the Spotlight is marked as completed.|   |organizationVolumeThreshold|The article volume needed to create a Spotlight, as set by the company's overall volume level classification on the Start Date.|   |totalSpotlightVolume|Total number of articles in the Spotlight. This number will change until the Spotlight is marked as completed.|   |startDateVolume|Number of articles in the Spotlight on the Start Date when it met the volume threshold. Does not include the number of articles that were added to the Spotlight after the Spotlight Start Date.|   |primaryArticleSource|Source of the primary article.|   |primaryArticleUrl|URL of the primary article.|   |primaryArticleHeadline|Headline of primary Spotlight article.|   |primaryArticleBulletpoints|Bullet points summarizing the primary article.|   |meanArtScoreFinalDate|Average score of articles in Spotlight on Final Article Date. This score will continue to change until the Spotlight is marked as completed.|   |meanArtScoreStartDate|Average score of articles in Spotlight on Start Date. This score will not change throughout the history of the spotlight.|   |meanPulseScore|Average of pulse scores for each day from First Article Date to Final Article Date, including scores for both Start Date and Final Article Date.|   |pulseBeforeFirstArticle|Pulse score for category at end-of-day on day before the First Article Date|   |pulseOnFinalArticleDate|Pulse score for category at the end-of-day on the Final Article Date.|   |pulseOnStartDate|Pulse score for the category at the end-of-day on the Start Date.|   |zScoreOnFinalDate|Z-score for Spotlight as of Final Article Date. This score will continue to change until the Spotlight is marked as completed.|   |zScoreOnStartDate|Z-score for Spotlight as of Start Date. This score will not change throughout the history of the spotlight.|   |standoutLvlOnFinalDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.  This score will continue to change until the Spotlight is marked as completed.|   |standoutLvlOnStartDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.| . [optional]
             categories ([str]): The SASB Categories requested for the respective scoreType(s). The default value is **ALLCATEGORIES**, which represents all 26 categories in a single overall score. To request a specifc category or list of categories, simply input the category names below.   ### SASB Categories |**SASB Category Inputs**|**Description**| |---|---| |**ALLCATEGORIES**|**All Categories** - this category represents a company's overall SASB Score for the specific 'scoreType'. This value is equal to the cumulative average of all 26 SASB categories for the specific 'scoreType'.*Note that category is not available for the Dynamic Materiality 'scoreType'.| |**ACCESSANDAFFORDABILITY**|**Access and Affordability** - The category addresses a company's ability to ensure broad access to its products and services, specifically in the context of underserved markets and/or population groups. It includes the management of issues related to universal needs, such as the accessibility and affordability of health care, financial services, utilities , education, and telecommunications.| |**AIRQUALITY**|**Air Quality** - the category addresses management of air quality impacts resulting from stationary (e.g., factories, power plants) and mobile sources (e.g., trucks, delivery vehicles, planes) as well as industrial emissions. Relevant airborne pollutants include, but are not limited to, oxides of nitrogen (NOx), oxides of sulfur (SOx), volatile organic compounds (VOCs), heavy metals, particulate matter, and chlorofluorocarbons. The category does not include GHG emissions, which are addressed in a separate category.| |**BUSINESSETHICS**|**Business Ethics** - the category addresses the company's approach to managing risks and opportunities surrounding ethical conduct of business, including fraud, corruption, bribery and facilitation payments, fiduciary responsibilities, and other behavior that may have an ethical component. This includes sensitivity to business norms and standards as they shift over time, jurisdiction, and culture. It addresses the company's ability to provide services that satisfy the highest professional and ethical standards of the industry, which means to avoid conflicts of interest, misrepresentation, bias, and negligence through training employees adequately and implementing policies and procedures to ensure employees provide services free from bias and error.| |**BUSMODELRESILIENCE**|**Business Model Resilience** - the category addresses an industry's capacity to manage risks and opportunities associated with incorporating social, environmental, and political transitions into long-term business model planning. This includes responsiveness to the transition to a low-carbon and climate-constrained economy, as well as growth and creation of new markets among unserved and underserved socioeconomic populations. The category highlights industries in which evolving environmental and social realities may challenge companies to fundamentally adapt or may put their business models at risk.| |**COMPETITIVEBEHAVIOR**|**Competitive Behavior** - the category covers social issues associated with existence of monopolies, which may include, but are not limited to, excessive prices, poor quality of service, and inefficiencies. It addresses a company's management of legal and social expectation around monopolistic and anti-competitive practices, including issues related to bargaining power, collusion, price fixing or manipulation, and protection of patents and intellectual property (IP).| |**CRITINCIDENTRISKMGT**|**Critical Incident Risk Management** - the category addresses the company's use of management systems and scenario planning to identify, understand, and prevent or minimize the occurrence of low-probability, high-impact accidents and emergencies with significant potential environmental and social externalities. It relates to the culture of safety at a company, its relevant safety management systems and technological controls, the potential human, environmental, and social implications of such events occurring, and the long-term effects to an organization, its workers, and society should these events occur.| |**CUSTOMERPRIVACY**|**Customer Privacy** - the category addresses management of risks related to the use of personally identifiable information (PII) and other customer or user data for secondary purposes including but not limited to marketing through affiliates and non-affiliates. The scope of the category includes social issues that may arise from a company's approach to collecting data, obtaining consent (e.g., opt-in policies), managing user and customer expectations regarding how their data is used, and managing evolving regulation. It excludes social issues arising from cybersecurity risks, which are covered in a separate category.| |**CUSTWELFARE**|**Customer Welfare** - the category addresses customer welfare concerns over issues including, but not limited to, health and nutrition of foods and beverages, antibiotic use in animal production, and management of controlled substances. The category addresses the company's ability to provide consumers with manufactured products and services that are aligned with societal expectations. It does not include issues directly related to quality and safety malfunctions of manufactured products and services, but instead addresses qualities inherent to the design and delivery of products and services where customer welfare may be in question. The scope of the category also captures companies' ability to prevent counterfeit products.| |**DATASECURITY**|**Data Security** - the category addresses management of risks related to collection, retention, and use of sensitive, confidential, and/or proprietary customer or user data. It includes social issues that may arise from incidents such as data breaches in which personally identifiable information (PII) and other user or customer data may be exposed. It addresses a company's strategy, policies, and practices related to IT infrastructure, staff training, record keeping, cooperation with law enforcement, and other mechanisms used to ensure security of customer or user data.| |**ECOLOGICALIMPACTS**|**Ecological Impacts** - the category addresses management of the company's impacts on ecosystems and biodiversity through activities including, but not limited to, land use for exploration, natural resource extraction, and cultivation, as well as project development, construction, and siting. The impacts include, but are not limited to, biodiversity loss, habitat destruction, and deforestation at all stages – planning, land acquisition, permitting, development, operations, and site remediation. The category does not cover impacts of climate change on ecosystems and biodiversity.| |**EMPENGDIVANDINC**|**Employee Engagement Diversity and Inclusion** - the category addresses a company's ability to ensure that its culture and hiring and promotion practices embrace the building of a diverse and inclusive workforce that reflects the makeup of local talent pools and its customer base. It addresses the issues of discriminatory practices on the bases of race, gender, ethnicity, religion, sexual orientation, and other factors.| |**EMPHEALTHANDSAFETY**|**Employee Health and Safety** - the category addresses a company's ability to create and maintain a safe and healthy workplace environment that is free of injuries, fatalities, and illness (both chronic and acute). It is traditionally accomplished through implementing safety management plans, developing training requirements for employees and contractors, and conducting regular audits of their own practices as well as those of their subcontractors. The category further captures how companies ensure physical and mental health of workforce through technology, training, corporate culture, regulatory compliance, monitoring and testing, and personal protective equipment.| |**ENERGYMGT**|**Energy Management** - the category addresses environmental impacts associated with energy consumption. It addresses the company's management of energy in manufacturing and/or for provision of products and services derived from utility providers (grid energy) not owned or controlled by the company. More specifically, it includes management of energy efficiency and intensity, energy mix, as well as grid reliance. Upstream (e.g., suppliers) and downstream (e.g., product use) energy use is not included in the scope.| |**GHGEMISSIONS**|**Greenhouse Gas Emissions** - the category addresses direct (Scope 1) greenhouse gas (GHG) emissions that a company generates through its operations. This includes GHG emissions from stationary (e.g., factories, power plants) and mobile sources (e.g., trucks, delivery vehicles, planes), whether a result of combustion of fuel or non-combusted direct releases during activities such as natural resource extraction, power generation, land use, or biogenic processes. The category further includes management of regulatory risks, environmental compliance, and reputational risks and opportunities, as they related to direct GHG emissions. The seven GHGs covered under the Kyoto Protocol are included within the category— carbon dioxide (CO2 ), methane (CH4), nitrous oxide (N2O), hydrofluorocarbons (HFCs), perfluorocarbons (PFCs), sulfur hexafluoride (SF6), and nitrogen trifluoride (NF3).| |**HUMANRIGHTSANDCOMRELS**|**Human Rights and Community Relations** - the category addresses management of the relationship between businesses and the communities in which they operate, including, but not limited to, management of direct and indirect impacts on core human rights and the treatment of indigenous peoples. More specifically, such management may cover socio-economic community impacts, community engagement, environmental justice, cultivation of local workforces, impact on local businesses, license to operate, and environmental/social impact assessments. The category does not include environmental impacts such as air pollution or waste which, although they may impact the health and safety of members of local communities, are addressed in separate categories.| |**LABORPRACTICES**|**Labor Practices** - the category addresses the company's ability to uphold commonly accepted labor standards in the workplace, including compliance with labor laws and internationally accepted norms and standards. This includes, but is not limited to, ensuring basic human rights related to child labor, forced or bonded labor, exploitative labor, fair wages and overtime pay, and other basic workers' rights. It also includes minimum wage policies and provision of benefits, which may influence how a workforce is attracted, retained, and motivated. The category further addresses a company's relationship with organized labor and freedom of association.| |**MGTOFLEGALANDREGENV**|**Management of the Legal and Regulatory Environment** - the category addresses a company's approach to engaging with regulators in cases where conflicting corporate and public interests may have the potential for long-term adverse direct or indirect environmental and social impacts. The category addresses a company's level of reliance upon regulatory policy or monetary incentives (such as subsidies and taxes), actions to influence industry policy (such as through lobbying), overall reliance on a favorable regulatory environment for business competitiveness, and ability to comply with relevant regulations. It may relate to the alignment of management and investor views of regulatory engagement and compliance at large.| |**MATSOURCINGANDEFF**|**Materials Sourcing and Efficiency** - the category addresses issues related to the resilience of materials supply chains to impacts of climate change and other external environmental and social factors. It captures the impacts of such external factors on operational activity of suppliers, which can further affect availability and pricing of key resources. It addresses a company's ability to manage these risks through product design, manufacturing, and end-of-life management, such as by using of recycled and renewable materials, reducing the use of key materials (dematerialization), maximizing resource efficiency in manufacturing, and making R&D investments in substitute materials. Additionally, companies can manage these issues by screening, selection, monitoring, and engagement with suppliers to ensure their resilience to external risks. It does not address issues associated with environmental and social externalities created by operational activity of individual suppliers, which is covered in a separate category.| |**MATERIALITY**|**Materiality** - this category represents a composite score of all 'material' SASB categories for the given entity. For more information on SASB's Materiality Map, visit [materiality.sasb.org](https://materiality.sasb.org/)| |**PHYIMPACTSOFCLIMATECHG**|**Physical Impacts of Climate Change** - the category addresses the company's ability to manage risks and opportunities associated with direct exposure of its owned or controlled assets and operations to actual or potential physical impacts of climate change. It captures environmental and social issues that may arise from operational disruptions due to physical impacts of climate change. It further captures socioeconomic issues resulting from companies failing to incorporate climate change consideration in products and services sold, such as insurance policies and mortgages. The category relates to the company's ability to adapt to increased frequency and severity of extreme weather, shifting climate, sea level risk, and other expected physical impacts of climate change. Management may involve enhancing resiliency of physical assets and/or surrounding infrastructure as well as incorporation of climate change-related considerations into key business activities (e.g., mortgage and insurance underwriting, planning and development of real estate projects).| |**PDANDLIFECYCLEMGT**|**Product Design and Lifecycle Management** - the category addresses incorporation of environmental, social, and governance (ESG) considerations in characteristics of products and services provided or sold by the company. It includes, but is not limited to, managing the lifecycle impacts of products and services, such as those related to packaging, distribution, use-phase resource intensity, and other environmental and social externalities that may occur during their use-phase or at the end of life. The category captures a company's ability to address customer and societal demand for more sustainable products and services as well as to meet evolving environmental and social regulation. It does not address direct environmental or social impacts of the company's operations nor does it address health and safety risks to consumers from product use, which are covered in other categories.| |**PRODQUALITYANDSFTY**|**Product Quality and Safety** - the category addresses issues involving unintended characteristics of products sold or services provided that may create health or safety risks to end-users. It addresses a company's ability to offer manufactured products and/or services that meet customer expectations with respect to their health and safety characteristics. It includes, but is not limited to, issues involving liability, management of recalls and market withdrawals, product testing, and chemicals/content/ ingredient management in products.| |**SELLPRACANDPRODLABEL**|**Selling Practices and Product Labeling** - the category addresses social issues that may arise from a failure to manage the transparency, accuracy, and comprehensibility of marketing statements, advertising, and labeling of products and services. It includes, but is not limited to, advertising standards and regulations, ethical and responsible marketing practices, misleading or deceptive labeling, as well as discriminatory or predatory selling and lending practices. This may include deceptive or aggressive selling practices in which incentive structures for employees could encourage the sale of products or services that are not in the best interest of customers or clients.| |**SUPPLYCHAINMGT**|**Supply Chain Management** - the category addresses management of environmental, social, and governance (ESG) risks within a company's supply chain. It addresses issues associated with environmental and social externalities created by suppliers through their operational activities. Such issues include, but are not limited to, environmental responsibility, human rights, labor practices, and ethics and corruption. Management may involve screening, selection, monitoring, and engagement with suppliers on their environmental and social impacts. The category does not address the impacts of external factors – such as climate change and other environmental and social factors – on suppliers' operations and/or on the availability and pricing of key resources, which is covered in a separate category.| |**SYSTEMICRISKMGT**|**Systemic Risk Management** - the category addresses the company's contributions to, or management of systemic risks resulting from large-scale weakening or collapse of systems upon which the economy and society depend. This includes financial systems, natural resource systems, and technological systems. It addresses the mechanisms a company has in place to reduce its contributions to systemic risks and to improve safeguards that may mitigate the impacts of systemic failure. For financial institutions, the category also captures the company's ability to absorb shocks arising from financial and economic stress and meet stricter regulatory requirements related to the complexity and interconnectedness of companies in the industry.| |**WASTEANDHZRDMATSMGT**|**Waste and Hazardous Materials Management** - the category addresses environmental issues associated with hazardous and non-hazardous waste generated by companies. It addresses a company's management of solid wastes in manufacturing, agriculture, and other industrial processes. It covers treatment, handling, storage, disposal, and regulatory compliance. The category does not cover emissions to air or wastewater, nor does it cover waste from end-of-life of products, which are addressed in separate categories.| |**WATERANDWASTEWATERMGT**|**Water and Wastewater Management** - the category addresses a company's water use, water consumption, wastewater generation, and other impacts of operations on water resources, which may be influenced by regional differences in the availability and quality of and competition for water resources. More specifically, it addresses management strategies including, but not limited to, water efficiency, intensity, and recycling. Lastly, the category also addresses management of wastewater treatment and discharge, including groundwater and aquifer pollution.| . [optional] if omitted the server will use the default value of ["ALLCATEGORIES"]
-            primary_only (bool): This parameter would return only primary spotlights when set to `true` . [optional] if omitted the server will use the default value of True
+            primary_only (bool): This parameter would return only primary spotlights when set to `true`    . [optional] if omitted the server will use the default value of True
             is_removed (bool): This parameter would return the spotlights removed in the response(i.e. Spotlight is marked as Rejected but has a firstApprovedOnDate))when set to `true` Only Spotlights that are marked as approved will be returned when set to `false` . [optional] if omitted the server will use the default value of False
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -552,15 +403,15 @@
             ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
             start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
             end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
 
         Keyword Args:
             fields ([str]): Request available SASB Spotlights data fields to be included in the response.  Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |orgId|Unique identifier assigned by Truvalue that is applied on an organization level |             |date|Date for the period requested in YYYY-MM-DD format.|   |spotlightId|Unique identifier identifying a Spotlight ESG event that is detected at the company level, within a single category.|   |groupId|Unique identifier  identifying a Spotlight group using the Spotlight ID of the Primary Spotlight.|   |requestId|Identifier that was used for the request.|     <h3>SASB Spotlights Fields</h3>     |field|description|   |---|---|   |orgName|The current name of the organization (not point-in-time)|   |primarySpotlight|Y/N value indicating the primary Spotlight in a Spotlight Group.|   |spotlightCategory|SASB category tagged to each Spotlight.|   |materialCategory|Indicates if the category is material for the organization based on SASBs Materiality Map|   |status|Indicates status of a spotlight, which can be one of Completed or Ongoing.|   |removed|Displays the date a Spotlight was removed from the dataset, if it has been removed.|   |startDate|Date when a Spotlight has met the volume threshold for Spotlight consideration. Score and volume change metadata are associated with this date.|   |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start date|   |firstArticleDate|Date of earliest article in the Spotlight as of the Start Date.|   |finalArticleDate|Date of final article in the Spotlight. This value can change over the course of the Spotlight until the Spotlight is marked as completed.|   |organizationVolumeThreshold|The article volume needed to create a Spotlight, as set by the company's overall volume level classification on the Start Date.|   |totalSpotlightVolume|Total number of articles in the Spotlight. This number will change until the Spotlight is marked as completed.|   |startDateVolume|Number of articles in the Spotlight on the Start Date when it met the volume threshold. Does not include the number of articles that were added to the Spotlight after the Spotlight Start Date.|   |primaryArticleSource|Source of the primary article.|   |primaryArticleUrl|URL of the primary article.|   |primaryArticleHeadline|Headline of primary Spotlight article.|   |primaryArticleBulletpoints|Bullet points summarizing the primary article.|   |meanArtScoreFinalDate|Average score of articles in Spotlight on Final Article Date. This score will continue to change until the Spotlight is marked as completed.|   |meanArtScoreStartDate|Average score of articles in Spotlight on Start Date. This score will not change throughout the history of the spotlight.|   |meanPulseScore|Average of pulse scores for each day from First Article Date to Final Article Date, including scores for both Start Date and Final Article Date.|   |pulseBeforeFirstArticle|Pulse score for category at end-of-day on day before the First Article Date|   |pulseOnFinalArticleDate|Pulse score for category at the end-of-day on the Final Article Date.|   |pulseOnStartDate|Pulse score for the category at the end-of-day on the Start Date.|   |zScoreOnFinalDate|Z-score for Spotlight as of Final Article Date. This score will continue to change until the Spotlight is marked as completed.|   |zScoreOnStartDate|Z-score for Spotlight as of Start Date. This score will not change throughout the history of the spotlight.|   |standoutLvlOnFinalDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.  This score will continue to change until the Spotlight is marked as completed.|   |standoutLvlOnStartDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.| . [optional]
             categories ([str]): The SASB Categories requested for the respective scoreType(s). The default value is **ALLCATEGORIES**, which represents all 26 categories in a single overall score. To request a specifc category or list of categories, simply input the category names below.   ### SASB Categories |**SASB Category Inputs**|**Description**| |---|---| |**ALLCATEGORIES**|**All Categories** - this category represents a company's overall SASB Score for the specific 'scoreType'. This value is equal to the cumulative average of all 26 SASB categories for the specific 'scoreType'.*Note that category is not available for the Dynamic Materiality 'scoreType'.| |**ACCESSANDAFFORDABILITY**|**Access and Affordability** - The category addresses a company's ability to ensure broad access to its products and services, specifically in the context of underserved markets and/or population groups. It includes the management of issues related to universal needs, such as the accessibility and affordability of health care, financial services, utilities , education, and telecommunications.| |**AIRQUALITY**|**Air Quality** - the category addresses management of air quality impacts resulting from stationary (e.g., factories, power plants) and mobile sources (e.g., trucks, delivery vehicles, planes) as well as industrial emissions. Relevant airborne pollutants include, but are not limited to, oxides of nitrogen (NOx), oxides of sulfur (SOx), volatile organic compounds (VOCs), heavy metals, particulate matter, and chlorofluorocarbons. The category does not include GHG emissions, which are addressed in a separate category.| |**BUSINESSETHICS**|**Business Ethics** - the category addresses the company's approach to managing risks and opportunities surrounding ethical conduct of business, including fraud, corruption, bribery and facilitation payments, fiduciary responsibilities, and other behavior that may have an ethical component. This includes sensitivity to business norms and standards as they shift over time, jurisdiction, and culture. It addresses the company's ability to provide services that satisfy the highest professional and ethical standards of the industry, which means to avoid conflicts of interest, misrepresentation, bias, and negligence through training employees adequately and implementing policies and procedures to ensure employees provide services free from bias and error.| |**BUSMODELRESILIENCE**|**Business Model Resilience** - the category addresses an industry's capacity to manage risks and opportunities associated with incorporating social, environmental, and political transitions into long-term business model planning. This includes responsiveness to the transition to a low-carbon and climate-constrained economy, as well as growth and creation of new markets among unserved and underserved socioeconomic populations. The category highlights industries in which evolving environmental and social realities may challenge companies to fundamentally adapt or may put their business models at risk.| |**COMPETITIVEBEHAVIOR**|**Competitive Behavior** - the category covers social issues associated with existence of monopolies, which may include, but are not limited to, excessive prices, poor quality of service, and inefficiencies. It addresses a company's management of legal and social expectation around monopolistic and anti-competitive practices, including issues related to bargaining power, collusion, price fixing or manipulation, and protection of patents and intellectual property (IP).| |**CRITINCIDENTRISKMGT**|**Critical Incident Risk Management** - the category addresses the company's use of management systems and scenario planning to identify, understand, and prevent or minimize the occurrence of low-probability, high-impact accidents and emergencies with significant potential environmental and social externalities. It relates to the culture of safety at a company, its relevant safety management systems and technological controls, the potential human, environmental, and social implications of such events occurring, and the long-term effects to an organization, its workers, and society should these events occur.| |**CUSTOMERPRIVACY**|**Customer Privacy** - the category addresses management of risks related to the use of personally identifiable information (PII) and other customer or user data for secondary purposes including but not limited to marketing through affiliates and non-affiliates. The scope of the category includes social issues that may arise from a company's approach to collecting data, obtaining consent (e.g., opt-in policies), managing user and customer expectations regarding how their data is used, and managing evolving regulation. It excludes social issues arising from cybersecurity risks, which are covered in a separate category.| |**CUSTWELFARE**|**Customer Welfare** - the category addresses customer welfare concerns over issues including, but not limited to, health and nutrition of foods and beverages, antibiotic use in animal production, and management of controlled substances. The category addresses the company's ability to provide consumers with manufactured products and services that are aligned with societal expectations. It does not include issues directly related to quality and safety malfunctions of manufactured products and services, but instead addresses qualities inherent to the design and delivery of products and services where customer welfare may be in question. The scope of the category also captures companies' ability to prevent counterfeit products.| |**DATASECURITY**|**Data Security** - the category addresses management of risks related to collection, retention, and use of sensitive, confidential, and/or proprietary customer or user data. It includes social issues that may arise from incidents such as data breaches in which personally identifiable information (PII) and other user or customer data may be exposed. It addresses a company's strategy, policies, and practices related to IT infrastructure, staff training, record keeping, cooperation with law enforcement, and other mechanisms used to ensure security of customer or user data.| |**ECOLOGICALIMPACTS**|**Ecological Impacts** - the category addresses management of the company's impacts on ecosystems and biodiversity through activities including, but not limited to, land use for exploration, natural resource extraction, and cultivation, as well as project development, construction, and siting. The impacts include, but are not limited to, biodiversity loss, habitat destruction, and deforestation at all stages – planning, land acquisition, permitting, development, operations, and site remediation. The category does not cover impacts of climate change on ecosystems and biodiversity.| |**EMPENGDIVANDINC**|**Employee Engagement Diversity and Inclusion** - the category addresses a company's ability to ensure that its culture and hiring and promotion practices embrace the building of a diverse and inclusive workforce that reflects the makeup of local talent pools and its customer base. It addresses the issues of discriminatory practices on the bases of race, gender, ethnicity, religion, sexual orientation, and other factors.| |**EMPHEALTHANDSAFETY**|**Employee Health and Safety** - the category addresses a company's ability to create and maintain a safe and healthy workplace environment that is free of injuries, fatalities, and illness (both chronic and acute). It is traditionally accomplished through implementing safety management plans, developing training requirements for employees and contractors, and conducting regular audits of their own practices as well as those of their subcontractors. The category further captures how companies ensure physical and mental health of workforce through technology, training, corporate culture, regulatory compliance, monitoring and testing, and personal protective equipment.| |**ENERGYMGT**|**Energy Management** - the category addresses environmental impacts associated with energy consumption. It addresses the company's management of energy in manufacturing and/or for provision of products and services derived from utility providers (grid energy) not owned or controlled by the company. More specifically, it includes management of energy efficiency and intensity, energy mix, as well as grid reliance. Upstream (e.g., suppliers) and downstream (e.g., product use) energy use is not included in the scope.| |**GHGEMISSIONS**|**Greenhouse Gas Emissions** - the category addresses direct (Scope 1) greenhouse gas (GHG) emissions that a company generates through its operations. This includes GHG emissions from stationary (e.g., factories, power plants) and mobile sources (e.g., trucks, delivery vehicles, planes), whether a result of combustion of fuel or non-combusted direct releases during activities such as natural resource extraction, power generation, land use, or biogenic processes. The category further includes management of regulatory risks, environmental compliance, and reputational risks and opportunities, as they related to direct GHG emissions. The seven GHGs covered under the Kyoto Protocol are included within the category— carbon dioxide (CO2 ), methane (CH4), nitrous oxide (N2O), hydrofluorocarbons (HFCs), perfluorocarbons (PFCs), sulfur hexafluoride (SF6), and nitrogen trifluoride (NF3).| |**HUMANRIGHTSANDCOMRELS**|**Human Rights and Community Relations** - the category addresses management of the relationship between businesses and the communities in which they operate, including, but not limited to, management of direct and indirect impacts on core human rights and the treatment of indigenous peoples. More specifically, such management may cover socio-economic community impacts, community engagement, environmental justice, cultivation of local workforces, impact on local businesses, license to operate, and environmental/social impact assessments. The category does not include environmental impacts such as air pollution or waste which, although they may impact the health and safety of members of local communities, are addressed in separate categories.| |**LABORPRACTICES**|**Labor Practices** - the category addresses the company's ability to uphold commonly accepted labor standards in the workplace, including compliance with labor laws and internationally accepted norms and standards. This includes, but is not limited to, ensuring basic human rights related to child labor, forced or bonded labor, exploitative labor, fair wages and overtime pay, and other basic workers' rights. It also includes minimum wage policies and provision of benefits, which may influence how a workforce is attracted, retained, and motivated. The category further addresses a company's relationship with organized labor and freedom of association.| |**MGTOFLEGALANDREGENV**|**Management of the Legal and Regulatory Environment** - the category addresses a company's approach to engaging with regulators in cases where conflicting corporate and public interests may have the potential for long-term adverse direct or indirect environmental and social impacts. The category addresses a company's level of reliance upon regulatory policy or monetary incentives (such as subsidies and taxes), actions to influence industry policy (such as through lobbying), overall reliance on a favorable regulatory environment for business competitiveness, and ability to comply with relevant regulations. It may relate to the alignment of management and investor views of regulatory engagement and compliance at large.| |**MATSOURCINGANDEFF**|**Materials Sourcing and Efficiency** - the category addresses issues related to the resilience of materials supply chains to impacts of climate change and other external environmental and social factors. It captures the impacts of such external factors on operational activity of suppliers, which can further affect availability and pricing of key resources. It addresses a company's ability to manage these risks through product design, manufacturing, and end-of-life management, such as by using of recycled and renewable materials, reducing the use of key materials (dematerialization), maximizing resource efficiency in manufacturing, and making R&D investments in substitute materials. Additionally, companies can manage these issues by screening, selection, monitoring, and engagement with suppliers to ensure their resilience to external risks. It does not address issues associated with environmental and social externalities created by operational activity of individual suppliers, which is covered in a separate category.| |**MATERIALITY**|**Materiality** - this category represents a composite score of all 'material' SASB categories for the given entity. For more information on SASB's Materiality Map, visit [materiality.sasb.org](https://materiality.sasb.org/)| |**PHYIMPACTSOFCLIMATECHG**|**Physical Impacts of Climate Change** - the category addresses the company's ability to manage risks and opportunities associated with direct exposure of its owned or controlled assets and operations to actual or potential physical impacts of climate change. It captures environmental and social issues that may arise from operational disruptions due to physical impacts of climate change. It further captures socioeconomic issues resulting from companies failing to incorporate climate change consideration in products and services sold, such as insurance policies and mortgages. The category relates to the company's ability to adapt to increased frequency and severity of extreme weather, shifting climate, sea level risk, and other expected physical impacts of climate change. Management may involve enhancing resiliency of physical assets and/or surrounding infrastructure as well as incorporation of climate change-related considerations into key business activities (e.g., mortgage and insurance underwriting, planning and development of real estate projects).| |**PDANDLIFECYCLEMGT**|**Product Design and Lifecycle Management** - the category addresses incorporation of environmental, social, and governance (ESG) considerations in characteristics of products and services provided or sold by the company. It includes, but is not limited to, managing the lifecycle impacts of products and services, such as those related to packaging, distribution, use-phase resource intensity, and other environmental and social externalities that may occur during their use-phase or at the end of life. The category captures a company's ability to address customer and societal demand for more sustainable products and services as well as to meet evolving environmental and social regulation. It does not address direct environmental or social impacts of the company's operations nor does it address health and safety risks to consumers from product use, which are covered in other categories.| |**PRODQUALITYANDSFTY**|**Product Quality and Safety** - the category addresses issues involving unintended characteristics of products sold or services provided that may create health or safety risks to end-users. It addresses a company's ability to offer manufactured products and/or services that meet customer expectations with respect to their health and safety characteristics. It includes, but is not limited to, issues involving liability, management of recalls and market withdrawals, product testing, and chemicals/content/ ingredient management in products.| |**SELLPRACANDPRODLABEL**|**Selling Practices and Product Labeling** - the category addresses social issues that may arise from a failure to manage the transparency, accuracy, and comprehensibility of marketing statements, advertising, and labeling of products and services. It includes, but is not limited to, advertising standards and regulations, ethical and responsible marketing practices, misleading or deceptive labeling, as well as discriminatory or predatory selling and lending practices. This may include deceptive or aggressive selling practices in which incentive structures for employees could encourage the sale of products or services that are not in the best interest of customers or clients.| |**SUPPLYCHAINMGT**|**Supply Chain Management** - the category addresses management of environmental, social, and governance (ESG) risks within a company's supply chain. It addresses issues associated with environmental and social externalities created by suppliers through their operational activities. Such issues include, but are not limited to, environmental responsibility, human rights, labor practices, and ethics and corruption. Management may involve screening, selection, monitoring, and engagement with suppliers on their environmental and social impacts. The category does not address the impacts of external factors – such as climate change and other environmental and social factors – on suppliers' operations and/or on the availability and pricing of key resources, which is covered in a separate category.| |**SYSTEMICRISKMGT**|**Systemic Risk Management** - the category addresses the company's contributions to, or management of systemic risks resulting from large-scale weakening or collapse of systems upon which the economy and society depend. This includes financial systems, natural resource systems, and technological systems. It addresses the mechanisms a company has in place to reduce its contributions to systemic risks and to improve safeguards that may mitigate the impacts of systemic failure. For financial institutions, the category also captures the company's ability to absorb shocks arising from financial and economic stress and meet stricter regulatory requirements related to the complexity and interconnectedness of companies in the industry.| |**WASTEANDHZRDMATSMGT**|**Waste and Hazardous Materials Management** - the category addresses environmental issues associated with hazardous and non-hazardous waste generated by companies. It addresses a company's management of solid wastes in manufacturing, agriculture, and other industrial processes. It covers treatment, handling, storage, disposal, and regulatory compliance. The category does not cover emissions to air or wastewater, nor does it cover waste from end-of-life of products, which are addressed in separate categories.| |**WATERANDWASTEWATERMGT**|**Water and Wastewater Management** - the category addresses a company's water use, water consumption, wastewater generation, and other impacts of operations on water resources, which may be influenced by regional differences in the availability and quality of and competition for water resources. More specifically, it addresses management strategies including, but not limited to, water efficiency, intensity, and recycling. Lastly, the category also addresses management of wastewater treatment and discharge, including groundwater and aquifer pollution.| . [optional] if omitted the server will use the default value of ["ALLCATEGORIES"]
-            primary_only (bool): This parameter would return only primary spotlights when set to `true` . [optional] if omitted the server will use the default value of True
+            primary_only (bool): This parameter would return only primary spotlights when set to `true`    . [optional] if omitted the server will use the default value of True
             is_removed (bool): This parameter would return the spotlights removed in the response(i.e. Spotlight is marked as Rejected but has a firstApprovedOnDate))when set to `true` Only Spotlights that are marked as approved will be returned when set to `false` . [optional] if omitted the server will use the default value of False
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True. NOTE: if this API returns a file, it is the responsibility
                 of the caller to close the file stream.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -782,437 +633,7 @@
         """
         self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
         kwargs['sasb_spotlights_request'] = \
             sasb_spotlights_request
         return self.get_sasb_spotlights_for_list_endpoint.call_with_http_info(**kwargs)
 
 
-    def get_sdg_spotlights(
-        self,
-        ids,
-        start_date,
-        end_date,
-        **kwargs
-    ) -> SpotlightsResponse:
-        """Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management  # noqa: E501
-
-        FactSet ESG by Truvalue Labs’ Spotlight Data solutions are a daily collection of the most important positive and negative ESG events detected by our algorithms, with a variety of quantitative metadata to enable timely and systematic trading strategies and portfolio management. Qualitive informational data points such as the headline and key bullet points for articles is also included.    # noqa: E501
-        This method makes a synchronous HTTP request. Returns the http data only
-
-        Args:
-            ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
-            start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
-            end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
-
-        Keyword Args:
-            categories ([str]): The SDG Categories specified for the Truvalue Scores being requested. To specify select categories returned in the response, provide a comma-separated list of the scores using the description below.  |**SDG Category Input**|**Description**| |---|---| |**IMPACT**|**Impact** - The aggregate SDG score for each company is simply named \"Impact.\" The SDG Impact Score is produced using a weighted average of individual category scores, where the weight utilized is the category score volume.| |**GOAL1NOPOVERTY**|**No Poverty** - Goal 1 focuses on poverty in all its manifestations and also aims to ensure social protection for the poor and vulnerable, increase access to basic services and support people harmed by climate related extreme events and other economic, social and environmental shocks and disasters. <p>**Company-Level Issue Examples** *- Financial services access and affordability, Underserved groups,Unethical pricing.*| |**GOAL2ZEROHUNGER**|**Zero Hunger** - Goal 2 aims to end hunger and all forms of malnutrition and commits to universal access to safe, nutritious and sufficient food at all times of the year, particularly for the poor and people in vulnerable situations (e.g., infants). This will require sustainable food production systems and resilient agricultural practices, equal access to land, technology, and markets and international cooperation on investments in infrastructure and technology to boost agricultural productivity. <p>**Company-Level Issue Examples** *- Sustainable agricultural practices, Agricultural ingredients sourcing and certifications, Food safety concerns, Animal welfare.*| |**GOAL3GOODHEALTHANDWELLBEING**|**Good Health and Wellbeing** - Goal 3 seeks to ensure health and wellbeing for all, at every stage of life and addresses all major health priorities, including reproductive, maternal, and child health; communicable, noncommunicable and environmental diseases; universal health coverage; and access for all to safe, effective, quality, and affordable medicines and vaccines.<p> **Company-Level Issue Examples** *- Harmful Chemicals in Products, Product Recalls, Healthcare Access and Affordability.*| |**GOAL4QUALITYEDUCATION**|**Quality Education** - Goal 4 addresses access and affordability of education and skills development starting from childhood development and continuing through adulthood, including for girls, persons with disabilities, indigenous peoples and children in vulnerable situations, Improvements to the access to education it hopes to ensure that all youth and a substantial proportion of adults achieve literacy and numeracy. It also seeks to build and upgrade education facilities and to increase the supply of qualified teachers.<p>**Company-Level Issue Examples** *- Mentorship and training, Education company quality, Education company ethics.*| |**GOAL5GENDEREQUALITY**|**Gender Equality** - Goal 5 emphasizes eliminating discrimination and violence against women and girls. The Goal emphasizes ensuring women's full and effective participation and equal opportunities for leadership at all levels of decision-making in political, economic and public life. Access to sexual and reproductive health and reproductive rights and access to economic resources (e.g., land ownership, financial services) are also emphasized.<p>**Company-Level Issue Examples** *- Board Diversity, Gender Discrimination, Sexual Harassment.*| |**GOAL6CLEANWATERANDSANITATION**|**Clean Water and Sanitation** - Goal 6 not only addresses issues relating to drinking water, sanitation and hygiene, but also the quality and sustainability of water resources worldwide. It strives to achieve universal and equitable access to safe and affordable drinking water for all. It also focuses on adequate and equitable sanitation and hygiene and reducing pollution, minimizing release of hazardous chemicals and materials, and protection of water-related ecosystems. It also highlights increasing water-use efficiency across all sectors, recycling, and ensuring sustainable withdrawals and supply of freshwater.<p>**Company-Level Issue Examples** *- Water Pollution, Water Recycling and Stewardship, Water Infrastructure.*| |**GOAL7AFFORDABLEANDCLEANENERGY**|**Goal 7 Affordable and Clean Energy** - Goal 7 seeks to ensure access to affordable, reliable, and modern energy services for all. It aims to increase renewable energy in the global energy mix and improve energy efficiency significantly. It also calls for more access to clean energy research, technology, and infrastructure for renewable energy, energy efficiency, and advanced and cleaner fossil-fuel technology, and promoting investment in energy infrastructure and clean energy technology.<p>**Company-Level Issue Examples** *- Green Buildings, Renewable Energy, Unethical Utility Pricing.*| |**GOAL8DECENTWORKANDECONOMICGROWTH**|**Decent Work and Economic Growth** - Goal 8 focuses on economic productivity and supports policies for entrepreneurship, creativity and innovation that assist micro, small, and medium-sized enterprises. The Goal also seeks to reduce unemployment, the proportion of youth not working or in school, child labor, and forced labor. Also covered are the protection of labor rights, migrant workers, safe and secure working environments, sustainable tourism, and increasing the capacity of domestic financial institutions in regards to access to banking, insurance, and financial services.<p>**Company-Level Issue Examples** *-  Job Creation, Labor Exploitation, Employee Health and Safety, Workplace Turnover, Supplier Transparency.*| |**GOAL9INDUSTRYINNOVATIONANDINFRASTRUCTURE**|**Industry Innovation and Infrastructure** - Goal 9 focuses on three important aspects of sustainable development, infrastructure, industrialization and innovation, including considerations for resiliency, equity, quality, reliability, access and affordability, and regional and transborder infrastructure. The Goal focuses on infrastructure upgrades and retrofitting of industries with increased resource-use efficiency and clean and environmentally sound technologies and industrial processes.<p>**Company-Level Issue Examples** *- Digital Divide, ESG integration in financial services, Engineering Structural Integrity.*| |**GOAL10REDUCEDINEQUALITIES**|**Reduced Inequalities** - Goal 10 calls for reducing inequalities in income as well as those based on age, sex, disability, race, ethnicity, origin, religion, or economic or other status within a country. The Goal addresses inequalities among countries, including those related to representation, migration, and development assistance. It aims to empower and promote social, economic, and political inclusion of all. The Goal stresses regulation and monitoring of global financial markets and institutions.<p>**Company-Level Issue Examples** *- Responsible Lending, Worker Discrimination, CEO Pay Gap, Worker Pay Gap, Workplace Diversity and Inclusion.*| |**GOAL11SUSTAINABLECITIESANDCOMMUNITIES**|**Sustainable Cities and Communities** - Goal 11 seeks to ensure access for all to adequate, safe, and affordable housing and basic services, and green and public spaces, and to upgrade slums. It focuses on improving transportation, air quality and municipal and other waste management, and creating inclusive and sustainable urbanization through participatory urban planning. The Goal also supports safeguarding the world's cultural and natural heritage, while aiming to increase the number of cities and human settlements adopting and implementing integrated policies and plans towards inclusion, resource efficiency, mitigation and adaptation to climate change, and resilience to disasters.<p>**Company-Level Issue Examples** *- Air Pollution, Environmental Justice, Human Rights Violations, Affordable Housing.*| |**GOAL12RESPONSIBLECONSUMPTIONANDPRODUCTION**|**Responsible Consumption and Production** - Goal 12 aims to achieve the sustainable management and efficient use of natural resources through both the public and private sector. It specifically addresses global food waste in consumption, production, and distribution, sustainable tourism, waste and chemicals management. Goal 12 encourages sustainability reporting in the private sector, while in the public sector it encourages restructuring taxation and subsidies for fossil fuels and promoting sustainable public procurement practices.<p>**Company-Level Issue Examples** *- Sustainability Reporting, Circular Economy, Hazardous Waste Management, Waste Reduction.*| |**GOAL13CLIMATEACTION**|**Climate Action** - While Goal 13 is focused on actions by countries towards climate mitigation and adaptation, the private sector can also play a role in these areas. The goal seeks to strengthen resilience and adaptive capacity to climate-related hazards and natural disasters in all countries. It calls for integrating climate change measures, including those related to climate resilience and low GHG development, into national policies, strategies, and planning. It aims to improve education and awareness of climate change mitigation, adaptation, impact reduction, and early warning.<p>**Company-Level Issue Examples** *- GHG Emissions, Sustainable Transportation, Physical Climate Impacts.*| |**GOAL14LIFEBELOWWATER**|**Life Below Water** - Goal 14 focuses on preventing marine pollution of all kinds, particularly from land-based activities, and to minimize and address the impacts of ocean acidification. The Goal also aims to achieve sustainable yields in fisheries, through regulation of harvesting, controlling subsidies, and ending overfishing. It seeks to sustainably manage and protect marine and coastal ecosystems to avoid significant adverse impacts, including by strengthening their resilience, and take action for their restoration in order to achieve healthy and productive oceans.<p>**Company-Level Issue Examples** *- Impacts on water-related endangered species and habitats, Oil Spills, Seafood Sourcing.*| |**GOAL15LIFEONLAND**|**Life On Land** - Goal 15 seeks to ensure the conservation, restoration, and sustainable use of terrestrial and inland freshwater ecosystems and their services, in order to preserve biodiversity. It focuses specifically on sustainably managing forests, halting deforestation, restoring degraded lands and successfully combating desertification, reducing degraded natural habitats and ending biodiversity loss, with an emphasis on threatened species and invasive alien species.<p>**Company-Level Issue Examples** *- Impacts on land-related endangered species and habitats, Sustainable forestry practices and certifications, Project lifecycle environmental impacts.*| |**GOAL16PEACEJUSTICEANDSTRONGINSTITUTIONS**|**Peace, Justice, and Strong Institutions** - Goal 16 aims to significantly reduce all forms of violence, and also focuses specifically on reducing violence against children in the forms of abuse, exploitation, trafficking, and torture. It also aims to significantly reduce illicit financial and arms flows and to substantially reduce corruption and bribery in all their forms. The Goal also emphasizes effective and transparent institutions at all levels, inclusive and participatory decision-making, ensuring public access to information, and protection of fundamental freedoms.<p>**Company-Level Issue Examples** *- Tax Avoidance, Anti-Competitive Behavior, Cyber Security, Corruption, ESG Resolutions.*| . [optional] if omitted the server will use the default value of ["IMPACT"]
-            fields ([str]): Request available SDG Spotlights data fields to be included in the response.  Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |orgId|Unique identifier assigned by Truvalue that is applied on an organization level |   |date|Date for the period requested in YYYY-MM-DD format.|   |spotlightId|Unique identifier identifying a Spotlight ESG event that is detected at the company level, within a single category.|   |groupId|Unique identifier  identifying a Spotlight group using the Spotlight ID of the Primary Spotlight.|   |requestId|Identifier that was used for the request.|    <h3>SDG Spotlights Fields</h3>     |field|description|   |----|----|   |orgName|The current name of the organization according to Truvalue (not point-in-time)|   |primarySpotlight|Value indicating the primary Spotlight in a Spotlight Group. It could be either \"Yes\" or \"No\".|   |spotlightCategory|SDG category tagged to each Spotlight.|    |status|Indicates status of a spotlight, which can be one of Completed or Ongoing. |   |removed|Displays the date a Spotlight was removed from the dataset, if it has been removed.|    |startDate|Date when a Spotlight has met the volume threshold for Spotlight consideration. Score and volume change metadata are associated with this date.|   |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start_date. |             |firstArticleDate|Date of earliest article in the Spotlight as of the Start Date. |   |finalArticleDate|Date of final article in the Spotlight. This value can change over the course of the Spotlight until the Spotlight is marked as completed.|       |organizationVolumeThreshold| The article volume needed to create a Spotlight, as set by the company's overall volume level classification on the Start Date. |    |totalSpotlightVolume|Total number of articles in the Spotlight. This number will change until the Spotlight is marked as completed.|             |startDateVolume|Number of articles in the Spotlight on the Start Date when it met the volume threshold. Does not include the number of articles that were added to the Spotlight after the Spotlight Start Date.|   |primaryArticleSource|Source of the primary article.|    |primaryArticleUrl|URL of the primary article.|              |primaryArticleHeadline|Headline of primary Spotlight article.|             |primaryArticleBulletpoints|Bullet points summarizing the primary article. |   |meanArtScoreFinalDate|Average score of articles in Spotlight on Final Article Date. This score will continue to change until the Spotlight is marked as completed.|      |meanArtScoreStartDate|Average score of articles in Spotlight on Start Date. This score will not change throughout the history of the spotlight.|             |meanPulseScore|Average of pulse scores for each day from First Article Date to Final Article Date, including scores for both Start Date and Final Article Date.|   |pulseBeforeFirstArticle|Pulse score for category at end-of-day on day before the First Article Date. |              |pulseOnFinalArticleDate|Pulse score for category at the end-of-day on the Final Article Date.|             |pulseOnStartDate|Pulse score for the category at the end-of-day on the Start Date. |   |zScoreOnFinalDate|Z-score for Spotlight as of Final Article Date. This score will continue to change until the Spotlight is marked as completed.|          |zScoreOnStartDate|Z-score for Spotlight as of Start Date. This score will not change throughout the history of the spotlight.|   |standoutLvlOnFinalDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.  This score will continue to change until the Spotlight is marked as completed.|    |standoutLvlOnStartDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.|            . [optional]
-            primary_only (bool): This parameter would return only primary spotlights when set to `true` . [optional] if omitted the server will use the default value of True
-            is_removed (bool): This parameter would return the spotlights removed in the response(i.e. Spotlight is marked as Rejected but has a firstApprovedOnDate))when set to `true` Only Spotlights that are marked as approved will be returned when set to `false` . [optional] if omitted the server will use the default value of False
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            SpotlightsResponse
-                Response Object
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
-        kwargs['ids'] = \
-            ids
-        kwargs['start_date'] = \
-            start_date
-        kwargs['end_date'] = \
-            end_date
-        return self.get_sdg_spotlights_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_spotlights_with_http_info(
-        self,
-        ids,
-        start_date,
-        end_date,
-        **kwargs
-    ) -> typing.Tuple[SpotlightsResponse, int, typing.MutableMapping]:
-        """Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management  # noqa: E501
-
-        FactSet ESG by Truvalue Labs’ Spotlight Data solutions are a daily collection of the most important positive and negative ESG events detected by our algorithms, with a variety of quantitative metadata to enable timely and systematic trading strategies and portfolio management. Qualitive informational data points such as the headline and key bullet points for articles is also included.    # noqa: E501
-        This method makes a synchronous HTTP request. Returns http data, http status and headers
-
-        Args:
-            ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
-            start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
-            end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
-
-        Keyword Args:
-            categories ([str]): The SDG Categories specified for the Truvalue Scores being requested. To specify select categories returned in the response, provide a comma-separated list of the scores using the description below.  |**SDG Category Input**|**Description**| |---|---| |**IMPACT**|**Impact** - The aggregate SDG score for each company is simply named \"Impact.\" The SDG Impact Score is produced using a weighted average of individual category scores, where the weight utilized is the category score volume.| |**GOAL1NOPOVERTY**|**No Poverty** - Goal 1 focuses on poverty in all its manifestations and also aims to ensure social protection for the poor and vulnerable, increase access to basic services and support people harmed by climate related extreme events and other economic, social and environmental shocks and disasters. <p>**Company-Level Issue Examples** *- Financial services access and affordability, Underserved groups,Unethical pricing.*| |**GOAL2ZEROHUNGER**|**Zero Hunger** - Goal 2 aims to end hunger and all forms of malnutrition and commits to universal access to safe, nutritious and sufficient food at all times of the year, particularly for the poor and people in vulnerable situations (e.g., infants). This will require sustainable food production systems and resilient agricultural practices, equal access to land, technology, and markets and international cooperation on investments in infrastructure and technology to boost agricultural productivity. <p>**Company-Level Issue Examples** *- Sustainable agricultural practices, Agricultural ingredients sourcing and certifications, Food safety concerns, Animal welfare.*| |**GOAL3GOODHEALTHANDWELLBEING**|**Good Health and Wellbeing** - Goal 3 seeks to ensure health and wellbeing for all, at every stage of life and addresses all major health priorities, including reproductive, maternal, and child health; communicable, noncommunicable and environmental diseases; universal health coverage; and access for all to safe, effective, quality, and affordable medicines and vaccines.<p> **Company-Level Issue Examples** *- Harmful Chemicals in Products, Product Recalls, Healthcare Access and Affordability.*| |**GOAL4QUALITYEDUCATION**|**Quality Education** - Goal 4 addresses access and affordability of education and skills development starting from childhood development and continuing through adulthood, including for girls, persons with disabilities, indigenous peoples and children in vulnerable situations, Improvements to the access to education it hopes to ensure that all youth and a substantial proportion of adults achieve literacy and numeracy. It also seeks to build and upgrade education facilities and to increase the supply of qualified teachers.<p>**Company-Level Issue Examples** *- Mentorship and training, Education company quality, Education company ethics.*| |**GOAL5GENDEREQUALITY**|**Gender Equality** - Goal 5 emphasizes eliminating discrimination and violence against women and girls. The Goal emphasizes ensuring women's full and effective participation and equal opportunities for leadership at all levels of decision-making in political, economic and public life. Access to sexual and reproductive health and reproductive rights and access to economic resources (e.g., land ownership, financial services) are also emphasized.<p>**Company-Level Issue Examples** *- Board Diversity, Gender Discrimination, Sexual Harassment.*| |**GOAL6CLEANWATERANDSANITATION**|**Clean Water and Sanitation** - Goal 6 not only addresses issues relating to drinking water, sanitation and hygiene, but also the quality and sustainability of water resources worldwide. It strives to achieve universal and equitable access to safe and affordable drinking water for all. It also focuses on adequate and equitable sanitation and hygiene and reducing pollution, minimizing release of hazardous chemicals and materials, and protection of water-related ecosystems. It also highlights increasing water-use efficiency across all sectors, recycling, and ensuring sustainable withdrawals and supply of freshwater.<p>**Company-Level Issue Examples** *- Water Pollution, Water Recycling and Stewardship, Water Infrastructure.*| |**GOAL7AFFORDABLEANDCLEANENERGY**|**Goal 7 Affordable and Clean Energy** - Goal 7 seeks to ensure access to affordable, reliable, and modern energy services for all. It aims to increase renewable energy in the global energy mix and improve energy efficiency significantly. It also calls for more access to clean energy research, technology, and infrastructure for renewable energy, energy efficiency, and advanced and cleaner fossil-fuel technology, and promoting investment in energy infrastructure and clean energy technology.<p>**Company-Level Issue Examples** *- Green Buildings, Renewable Energy, Unethical Utility Pricing.*| |**GOAL8DECENTWORKANDECONOMICGROWTH**|**Decent Work and Economic Growth** - Goal 8 focuses on economic productivity and supports policies for entrepreneurship, creativity and innovation that assist micro, small, and medium-sized enterprises. The Goal also seeks to reduce unemployment, the proportion of youth not working or in school, child labor, and forced labor. Also covered are the protection of labor rights, migrant workers, safe and secure working environments, sustainable tourism, and increasing the capacity of domestic financial institutions in regards to access to banking, insurance, and financial services.<p>**Company-Level Issue Examples** *-  Job Creation, Labor Exploitation, Employee Health and Safety, Workplace Turnover, Supplier Transparency.*| |**GOAL9INDUSTRYINNOVATIONANDINFRASTRUCTURE**|**Industry Innovation and Infrastructure** - Goal 9 focuses on three important aspects of sustainable development, infrastructure, industrialization and innovation, including considerations for resiliency, equity, quality, reliability, access and affordability, and regional and transborder infrastructure. The Goal focuses on infrastructure upgrades and retrofitting of industries with increased resource-use efficiency and clean and environmentally sound technologies and industrial processes.<p>**Company-Level Issue Examples** *- Digital Divide, ESG integration in financial services, Engineering Structural Integrity.*| |**GOAL10REDUCEDINEQUALITIES**|**Reduced Inequalities** - Goal 10 calls for reducing inequalities in income as well as those based on age, sex, disability, race, ethnicity, origin, religion, or economic or other status within a country. The Goal addresses inequalities among countries, including those related to representation, migration, and development assistance. It aims to empower and promote social, economic, and political inclusion of all. The Goal stresses regulation and monitoring of global financial markets and institutions.<p>**Company-Level Issue Examples** *- Responsible Lending, Worker Discrimination, CEO Pay Gap, Worker Pay Gap, Workplace Diversity and Inclusion.*| |**GOAL11SUSTAINABLECITIESANDCOMMUNITIES**|**Sustainable Cities and Communities** - Goal 11 seeks to ensure access for all to adequate, safe, and affordable housing and basic services, and green and public spaces, and to upgrade slums. It focuses on improving transportation, air quality and municipal and other waste management, and creating inclusive and sustainable urbanization through participatory urban planning. The Goal also supports safeguarding the world's cultural and natural heritage, while aiming to increase the number of cities and human settlements adopting and implementing integrated policies and plans towards inclusion, resource efficiency, mitigation and adaptation to climate change, and resilience to disasters.<p>**Company-Level Issue Examples** *- Air Pollution, Environmental Justice, Human Rights Violations, Affordable Housing.*| |**GOAL12RESPONSIBLECONSUMPTIONANDPRODUCTION**|**Responsible Consumption and Production** - Goal 12 aims to achieve the sustainable management and efficient use of natural resources through both the public and private sector. It specifically addresses global food waste in consumption, production, and distribution, sustainable tourism, waste and chemicals management. Goal 12 encourages sustainability reporting in the private sector, while in the public sector it encourages restructuring taxation and subsidies for fossil fuels and promoting sustainable public procurement practices.<p>**Company-Level Issue Examples** *- Sustainability Reporting, Circular Economy, Hazardous Waste Management, Waste Reduction.*| |**GOAL13CLIMATEACTION**|**Climate Action** - While Goal 13 is focused on actions by countries towards climate mitigation and adaptation, the private sector can also play a role in these areas. The goal seeks to strengthen resilience and adaptive capacity to climate-related hazards and natural disasters in all countries. It calls for integrating climate change measures, including those related to climate resilience and low GHG development, into national policies, strategies, and planning. It aims to improve education and awareness of climate change mitigation, adaptation, impact reduction, and early warning.<p>**Company-Level Issue Examples** *- GHG Emissions, Sustainable Transportation, Physical Climate Impacts.*| |**GOAL14LIFEBELOWWATER**|**Life Below Water** - Goal 14 focuses on preventing marine pollution of all kinds, particularly from land-based activities, and to minimize and address the impacts of ocean acidification. The Goal also aims to achieve sustainable yields in fisheries, through regulation of harvesting, controlling subsidies, and ending overfishing. It seeks to sustainably manage and protect marine and coastal ecosystems to avoid significant adverse impacts, including by strengthening their resilience, and take action for their restoration in order to achieve healthy and productive oceans.<p>**Company-Level Issue Examples** *- Impacts on water-related endangered species and habitats, Oil Spills, Seafood Sourcing.*| |**GOAL15LIFEONLAND**|**Life On Land** - Goal 15 seeks to ensure the conservation, restoration, and sustainable use of terrestrial and inland freshwater ecosystems and their services, in order to preserve biodiversity. It focuses specifically on sustainably managing forests, halting deforestation, restoring degraded lands and successfully combating desertification, reducing degraded natural habitats and ending biodiversity loss, with an emphasis on threatened species and invasive alien species.<p>**Company-Level Issue Examples** *- Impacts on land-related endangered species and habitats, Sustainable forestry practices and certifications, Project lifecycle environmental impacts.*| |**GOAL16PEACEJUSTICEANDSTRONGINSTITUTIONS**|**Peace, Justice, and Strong Institutions** - Goal 16 aims to significantly reduce all forms of violence, and also focuses specifically on reducing violence against children in the forms of abuse, exploitation, trafficking, and torture. It also aims to significantly reduce illicit financial and arms flows and to substantially reduce corruption and bribery in all their forms. The Goal also emphasizes effective and transparent institutions at all levels, inclusive and participatory decision-making, ensuring public access to information, and protection of fundamental freedoms.<p>**Company-Level Issue Examples** *- Tax Avoidance, Anti-Competitive Behavior, Cyber Security, Corruption, ESG Resolutions.*| . [optional] if omitted the server will use the default value of ["IMPACT"]
-            fields ([str]): Request available SDG Spotlights data fields to be included in the response.  Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |orgId|Unique identifier assigned by Truvalue that is applied on an organization level |   |date|Date for the period requested in YYYY-MM-DD format.|   |spotlightId|Unique identifier identifying a Spotlight ESG event that is detected at the company level, within a single category.|   |groupId|Unique identifier  identifying a Spotlight group using the Spotlight ID of the Primary Spotlight.|   |requestId|Identifier that was used for the request.|    <h3>SDG Spotlights Fields</h3>     |field|description|   |----|----|   |orgName|The current name of the organization according to Truvalue (not point-in-time)|   |primarySpotlight|Value indicating the primary Spotlight in a Spotlight Group. It could be either \"Yes\" or \"No\".|   |spotlightCategory|SDG category tagged to each Spotlight.|    |status|Indicates status of a spotlight, which can be one of Completed or Ongoing. |   |removed|Displays the date a Spotlight was removed from the dataset, if it has been removed.|    |startDate|Date when a Spotlight has met the volume threshold for Spotlight consideration. Score and volume change metadata are associated with this date.|   |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start_date. |             |firstArticleDate|Date of earliest article in the Spotlight as of the Start Date. |   |finalArticleDate|Date of final article in the Spotlight. This value can change over the course of the Spotlight until the Spotlight is marked as completed.|       |organizationVolumeThreshold| The article volume needed to create a Spotlight, as set by the company's overall volume level classification on the Start Date. |    |totalSpotlightVolume|Total number of articles in the Spotlight. This number will change until the Spotlight is marked as completed.|             |startDateVolume|Number of articles in the Spotlight on the Start Date when it met the volume threshold. Does not include the number of articles that were added to the Spotlight after the Spotlight Start Date.|   |primaryArticleSource|Source of the primary article.|    |primaryArticleUrl|URL of the primary article.|              |primaryArticleHeadline|Headline of primary Spotlight article.|             |primaryArticleBulletpoints|Bullet points summarizing the primary article. |   |meanArtScoreFinalDate|Average score of articles in Spotlight on Final Article Date. This score will continue to change until the Spotlight is marked as completed.|      |meanArtScoreStartDate|Average score of articles in Spotlight on Start Date. This score will not change throughout the history of the spotlight.|             |meanPulseScore|Average of pulse scores for each day from First Article Date to Final Article Date, including scores for both Start Date and Final Article Date.|   |pulseBeforeFirstArticle|Pulse score for category at end-of-day on day before the First Article Date. |              |pulseOnFinalArticleDate|Pulse score for category at the end-of-day on the Final Article Date.|             |pulseOnStartDate|Pulse score for the category at the end-of-day on the Start Date. |   |zScoreOnFinalDate|Z-score for Spotlight as of Final Article Date. This score will continue to change until the Spotlight is marked as completed.|          |zScoreOnStartDate|Z-score for Spotlight as of Start Date. This score will not change throughout the history of the spotlight.|   |standoutLvlOnFinalDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.  This score will continue to change until the Spotlight is marked as completed.|    |standoutLvlOnStartDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.|            . [optional]
-            primary_only (bool): This parameter would return only primary spotlights when set to `true` . [optional] if omitted the server will use the default value of True
-            is_removed (bool): This parameter would return the spotlights removed in the response(i.e. Spotlight is marked as Rejected but has a firstApprovedOnDate))when set to `true` Only Spotlights that are marked as approved will be returned when set to `false` . [optional] if omitted the server will use the default value of False
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            SpotlightsResponse
-                Response Object
-            int
-                Http Status Code
-            dict
-                Dictionary of the response headers
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
-        kwargs['ids'] = \
-            ids
-        kwargs['start_date'] = \
-            start_date
-        kwargs['end_date'] = \
-            end_date
-        return self.get_sdg_spotlights_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_spotlights_async(
-        self,
-        ids,
-        start_date,
-        end_date,
-        **kwargs
-    ) -> "ApplyResult[SpotlightsResponse]":
-        """Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management  # noqa: E501
-
-        FactSet ESG by Truvalue Labs’ Spotlight Data solutions are a daily collection of the most important positive and negative ESG events detected by our algorithms, with a variety of quantitative metadata to enable timely and systematic trading strategies and portfolio management. Qualitive informational data points such as the headline and key bullet points for articles is also included.    # noqa: E501
-        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
-
-        Args:
-            ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
-            start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
-            end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
-
-        Keyword Args:
-            categories ([str]): The SDG Categories specified for the Truvalue Scores being requested. To specify select categories returned in the response, provide a comma-separated list of the scores using the description below.  |**SDG Category Input**|**Description**| |---|---| |**IMPACT**|**Impact** - The aggregate SDG score for each company is simply named \"Impact.\" The SDG Impact Score is produced using a weighted average of individual category scores, where the weight utilized is the category score volume.| |**GOAL1NOPOVERTY**|**No Poverty** - Goal 1 focuses on poverty in all its manifestations and also aims to ensure social protection for the poor and vulnerable, increase access to basic services and support people harmed by climate related extreme events and other economic, social and environmental shocks and disasters. <p>**Company-Level Issue Examples** *- Financial services access and affordability, Underserved groups,Unethical pricing.*| |**GOAL2ZEROHUNGER**|**Zero Hunger** - Goal 2 aims to end hunger and all forms of malnutrition and commits to universal access to safe, nutritious and sufficient food at all times of the year, particularly for the poor and people in vulnerable situations (e.g., infants). This will require sustainable food production systems and resilient agricultural practices, equal access to land, technology, and markets and international cooperation on investments in infrastructure and technology to boost agricultural productivity. <p>**Company-Level Issue Examples** *- Sustainable agricultural practices, Agricultural ingredients sourcing and certifications, Food safety concerns, Animal welfare.*| |**GOAL3GOODHEALTHANDWELLBEING**|**Good Health and Wellbeing** - Goal 3 seeks to ensure health and wellbeing for all, at every stage of life and addresses all major health priorities, including reproductive, maternal, and child health; communicable, noncommunicable and environmental diseases; universal health coverage; and access for all to safe, effective, quality, and affordable medicines and vaccines.<p> **Company-Level Issue Examples** *- Harmful Chemicals in Products, Product Recalls, Healthcare Access and Affordability.*| |**GOAL4QUALITYEDUCATION**|**Quality Education** - Goal 4 addresses access and affordability of education and skills development starting from childhood development and continuing through adulthood, including for girls, persons with disabilities, indigenous peoples and children in vulnerable situations, Improvements to the access to education it hopes to ensure that all youth and a substantial proportion of adults achieve literacy and numeracy. It also seeks to build and upgrade education facilities and to increase the supply of qualified teachers.<p>**Company-Level Issue Examples** *- Mentorship and training, Education company quality, Education company ethics.*| |**GOAL5GENDEREQUALITY**|**Gender Equality** - Goal 5 emphasizes eliminating discrimination and violence against women and girls. The Goal emphasizes ensuring women's full and effective participation and equal opportunities for leadership at all levels of decision-making in political, economic and public life. Access to sexual and reproductive health and reproductive rights and access to economic resources (e.g., land ownership, financial services) are also emphasized.<p>**Company-Level Issue Examples** *- Board Diversity, Gender Discrimination, Sexual Harassment.*| |**GOAL6CLEANWATERANDSANITATION**|**Clean Water and Sanitation** - Goal 6 not only addresses issues relating to drinking water, sanitation and hygiene, but also the quality and sustainability of water resources worldwide. It strives to achieve universal and equitable access to safe and affordable drinking water for all. It also focuses on adequate and equitable sanitation and hygiene and reducing pollution, minimizing release of hazardous chemicals and materials, and protection of water-related ecosystems. It also highlights increasing water-use efficiency across all sectors, recycling, and ensuring sustainable withdrawals and supply of freshwater.<p>**Company-Level Issue Examples** *- Water Pollution, Water Recycling and Stewardship, Water Infrastructure.*| |**GOAL7AFFORDABLEANDCLEANENERGY**|**Goal 7 Affordable and Clean Energy** - Goal 7 seeks to ensure access to affordable, reliable, and modern energy services for all. It aims to increase renewable energy in the global energy mix and improve energy efficiency significantly. It also calls for more access to clean energy research, technology, and infrastructure for renewable energy, energy efficiency, and advanced and cleaner fossil-fuel technology, and promoting investment in energy infrastructure and clean energy technology.<p>**Company-Level Issue Examples** *- Green Buildings, Renewable Energy, Unethical Utility Pricing.*| |**GOAL8DECENTWORKANDECONOMICGROWTH**|**Decent Work and Economic Growth** - Goal 8 focuses on economic productivity and supports policies for entrepreneurship, creativity and innovation that assist micro, small, and medium-sized enterprises. The Goal also seeks to reduce unemployment, the proportion of youth not working or in school, child labor, and forced labor. Also covered are the protection of labor rights, migrant workers, safe and secure working environments, sustainable tourism, and increasing the capacity of domestic financial institutions in regards to access to banking, insurance, and financial services.<p>**Company-Level Issue Examples** *-  Job Creation, Labor Exploitation, Employee Health and Safety, Workplace Turnover, Supplier Transparency.*| |**GOAL9INDUSTRYINNOVATIONANDINFRASTRUCTURE**|**Industry Innovation and Infrastructure** - Goal 9 focuses on three important aspects of sustainable development, infrastructure, industrialization and innovation, including considerations for resiliency, equity, quality, reliability, access and affordability, and regional and transborder infrastructure. The Goal focuses on infrastructure upgrades and retrofitting of industries with increased resource-use efficiency and clean and environmentally sound technologies and industrial processes.<p>**Company-Level Issue Examples** *- Digital Divide, ESG integration in financial services, Engineering Structural Integrity.*| |**GOAL10REDUCEDINEQUALITIES**|**Reduced Inequalities** - Goal 10 calls for reducing inequalities in income as well as those based on age, sex, disability, race, ethnicity, origin, religion, or economic or other status within a country. The Goal addresses inequalities among countries, including those related to representation, migration, and development assistance. It aims to empower and promote social, economic, and political inclusion of all. The Goal stresses regulation and monitoring of global financial markets and institutions.<p>**Company-Level Issue Examples** *- Responsible Lending, Worker Discrimination, CEO Pay Gap, Worker Pay Gap, Workplace Diversity and Inclusion.*| |**GOAL11SUSTAINABLECITIESANDCOMMUNITIES**|**Sustainable Cities and Communities** - Goal 11 seeks to ensure access for all to adequate, safe, and affordable housing and basic services, and green and public spaces, and to upgrade slums. It focuses on improving transportation, air quality and municipal and other waste management, and creating inclusive and sustainable urbanization through participatory urban planning. The Goal also supports safeguarding the world's cultural and natural heritage, while aiming to increase the number of cities and human settlements adopting and implementing integrated policies and plans towards inclusion, resource efficiency, mitigation and adaptation to climate change, and resilience to disasters.<p>**Company-Level Issue Examples** *- Air Pollution, Environmental Justice, Human Rights Violations, Affordable Housing.*| |**GOAL12RESPONSIBLECONSUMPTIONANDPRODUCTION**|**Responsible Consumption and Production** - Goal 12 aims to achieve the sustainable management and efficient use of natural resources through both the public and private sector. It specifically addresses global food waste in consumption, production, and distribution, sustainable tourism, waste and chemicals management. Goal 12 encourages sustainability reporting in the private sector, while in the public sector it encourages restructuring taxation and subsidies for fossil fuels and promoting sustainable public procurement practices.<p>**Company-Level Issue Examples** *- Sustainability Reporting, Circular Economy, Hazardous Waste Management, Waste Reduction.*| |**GOAL13CLIMATEACTION**|**Climate Action** - While Goal 13 is focused on actions by countries towards climate mitigation and adaptation, the private sector can also play a role in these areas. The goal seeks to strengthen resilience and adaptive capacity to climate-related hazards and natural disasters in all countries. It calls for integrating climate change measures, including those related to climate resilience and low GHG development, into national policies, strategies, and planning. It aims to improve education and awareness of climate change mitigation, adaptation, impact reduction, and early warning.<p>**Company-Level Issue Examples** *- GHG Emissions, Sustainable Transportation, Physical Climate Impacts.*| |**GOAL14LIFEBELOWWATER**|**Life Below Water** - Goal 14 focuses on preventing marine pollution of all kinds, particularly from land-based activities, and to minimize and address the impacts of ocean acidification. The Goal also aims to achieve sustainable yields in fisheries, through regulation of harvesting, controlling subsidies, and ending overfishing. It seeks to sustainably manage and protect marine and coastal ecosystems to avoid significant adverse impacts, including by strengthening their resilience, and take action for their restoration in order to achieve healthy and productive oceans.<p>**Company-Level Issue Examples** *- Impacts on water-related endangered species and habitats, Oil Spills, Seafood Sourcing.*| |**GOAL15LIFEONLAND**|**Life On Land** - Goal 15 seeks to ensure the conservation, restoration, and sustainable use of terrestrial and inland freshwater ecosystems and their services, in order to preserve biodiversity. It focuses specifically on sustainably managing forests, halting deforestation, restoring degraded lands and successfully combating desertification, reducing degraded natural habitats and ending biodiversity loss, with an emphasis on threatened species and invasive alien species.<p>**Company-Level Issue Examples** *- Impacts on land-related endangered species and habitats, Sustainable forestry practices and certifications, Project lifecycle environmental impacts.*| |**GOAL16PEACEJUSTICEANDSTRONGINSTITUTIONS**|**Peace, Justice, and Strong Institutions** - Goal 16 aims to significantly reduce all forms of violence, and also focuses specifically on reducing violence against children in the forms of abuse, exploitation, trafficking, and torture. It also aims to significantly reduce illicit financial and arms flows and to substantially reduce corruption and bribery in all their forms. The Goal also emphasizes effective and transparent institutions at all levels, inclusive and participatory decision-making, ensuring public access to information, and protection of fundamental freedoms.<p>**Company-Level Issue Examples** *- Tax Avoidance, Anti-Competitive Behavior, Cyber Security, Corruption, ESG Resolutions.*| . [optional] if omitted the server will use the default value of ["IMPACT"]
-            fields ([str]): Request available SDG Spotlights data fields to be included in the response.  Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |orgId|Unique identifier assigned by Truvalue that is applied on an organization level |   |date|Date for the period requested in YYYY-MM-DD format.|   |spotlightId|Unique identifier identifying a Spotlight ESG event that is detected at the company level, within a single category.|   |groupId|Unique identifier  identifying a Spotlight group using the Spotlight ID of the Primary Spotlight.|   |requestId|Identifier that was used for the request.|    <h3>SDG Spotlights Fields</h3>     |field|description|   |----|----|   |orgName|The current name of the organization according to Truvalue (not point-in-time)|   |primarySpotlight|Value indicating the primary Spotlight in a Spotlight Group. It could be either \"Yes\" or \"No\".|   |spotlightCategory|SDG category tagged to each Spotlight.|    |status|Indicates status of a spotlight, which can be one of Completed or Ongoing. |   |removed|Displays the date a Spotlight was removed from the dataset, if it has been removed.|    |startDate|Date when a Spotlight has met the volume threshold for Spotlight consideration. Score and volume change metadata are associated with this date.|   |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start_date. |             |firstArticleDate|Date of earliest article in the Spotlight as of the Start Date. |   |finalArticleDate|Date of final article in the Spotlight. This value can change over the course of the Spotlight until the Spotlight is marked as completed.|       |organizationVolumeThreshold| The article volume needed to create a Spotlight, as set by the company's overall volume level classification on the Start Date. |    |totalSpotlightVolume|Total number of articles in the Spotlight. This number will change until the Spotlight is marked as completed.|             |startDateVolume|Number of articles in the Spotlight on the Start Date when it met the volume threshold. Does not include the number of articles that were added to the Spotlight after the Spotlight Start Date.|   |primaryArticleSource|Source of the primary article.|    |primaryArticleUrl|URL of the primary article.|              |primaryArticleHeadline|Headline of primary Spotlight article.|             |primaryArticleBulletpoints|Bullet points summarizing the primary article. |   |meanArtScoreFinalDate|Average score of articles in Spotlight on Final Article Date. This score will continue to change until the Spotlight is marked as completed.|      |meanArtScoreStartDate|Average score of articles in Spotlight on Start Date. This score will not change throughout the history of the spotlight.|             |meanPulseScore|Average of pulse scores for each day from First Article Date to Final Article Date, including scores for both Start Date and Final Article Date.|   |pulseBeforeFirstArticle|Pulse score for category at end-of-day on day before the First Article Date. |              |pulseOnFinalArticleDate|Pulse score for category at the end-of-day on the Final Article Date.|             |pulseOnStartDate|Pulse score for the category at the end-of-day on the Start Date. |   |zScoreOnFinalDate|Z-score for Spotlight as of Final Article Date. This score will continue to change until the Spotlight is marked as completed.|          |zScoreOnStartDate|Z-score for Spotlight as of Start Date. This score will not change throughout the history of the spotlight.|   |standoutLvlOnFinalDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.  This score will continue to change until the Spotlight is marked as completed.|    |standoutLvlOnStartDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.|            . [optional]
-            primary_only (bool): This parameter would return only primary spotlights when set to `true` . [optional] if omitted the server will use the default value of True
-            is_removed (bool): This parameter would return the spotlights removed in the response(i.e. Spotlight is marked as Rejected but has a firstApprovedOnDate))when set to `true` Only Spotlights that are marked as approved will be returned when set to `false` . [optional] if omitted the server will use the default value of False
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            ApplyResult[SpotlightsResponse]
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
-        kwargs['ids'] = \
-            ids
-        kwargs['start_date'] = \
-            start_date
-        kwargs['end_date'] = \
-            end_date
-        return self.get_sdg_spotlights_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_spotlights_with_http_info_async(
-        self,
-        ids,
-        start_date,
-        end_date,
-        **kwargs
-    ) -> "ApplyResult[typing.Tuple[SpotlightsResponse, int, typing.MutableMapping]]":
-        """Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management  # noqa: E501
-
-        FactSet ESG by Truvalue Labs’ Spotlight Data solutions are a daily collection of the most important positive and negative ESG events detected by our algorithms, with a variety of quantitative metadata to enable timely and systematic trading strategies and portfolio management. Qualitive informational data points such as the headline and key bullet points for articles is also included.    # noqa: E501
-        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
-
-        Args:
-            ids ([str]): Security or Entity identifiers. FactSet Identifiers, tickers, CUSIP and SEDOL are accepted input. <p>***ids limit** =  1500 per request*</p> *<p>Make note, GET Method URL request lines are also limited to a total  length of 8192 bytes (8KB). In cases where the service allows for thousands of ids, which may lead to exceeding this request line limit of 8KB, its advised for any requests with large request lines to be requested through the respective \"POST\" method.</p>* 
-            start_date (str): The start date requested for a given date range in YYYY-MM-DD format. The input start date must be before the input end date. Future dates (T+1) are not accepted in this endpoint. 
-            end_date (str): The end date requested for a given date range in YYYY-MM-DD format. The input end date must be after the input start date. Future dates (T+1) are not accepted in this endpoint. 
-
-        Keyword Args:
-            categories ([str]): The SDG Categories specified for the Truvalue Scores being requested. To specify select categories returned in the response, provide a comma-separated list of the scores using the description below.  |**SDG Category Input**|**Description**| |---|---| |**IMPACT**|**Impact** - The aggregate SDG score for each company is simply named \"Impact.\" The SDG Impact Score is produced using a weighted average of individual category scores, where the weight utilized is the category score volume.| |**GOAL1NOPOVERTY**|**No Poverty** - Goal 1 focuses on poverty in all its manifestations and also aims to ensure social protection for the poor and vulnerable, increase access to basic services and support people harmed by climate related extreme events and other economic, social and environmental shocks and disasters. <p>**Company-Level Issue Examples** *- Financial services access and affordability, Underserved groups,Unethical pricing.*| |**GOAL2ZEROHUNGER**|**Zero Hunger** - Goal 2 aims to end hunger and all forms of malnutrition and commits to universal access to safe, nutritious and sufficient food at all times of the year, particularly for the poor and people in vulnerable situations (e.g., infants). This will require sustainable food production systems and resilient agricultural practices, equal access to land, technology, and markets and international cooperation on investments in infrastructure and technology to boost agricultural productivity. <p>**Company-Level Issue Examples** *- Sustainable agricultural practices, Agricultural ingredients sourcing and certifications, Food safety concerns, Animal welfare.*| |**GOAL3GOODHEALTHANDWELLBEING**|**Good Health and Wellbeing** - Goal 3 seeks to ensure health and wellbeing for all, at every stage of life and addresses all major health priorities, including reproductive, maternal, and child health; communicable, noncommunicable and environmental diseases; universal health coverage; and access for all to safe, effective, quality, and affordable medicines and vaccines.<p> **Company-Level Issue Examples** *- Harmful Chemicals in Products, Product Recalls, Healthcare Access and Affordability.*| |**GOAL4QUALITYEDUCATION**|**Quality Education** - Goal 4 addresses access and affordability of education and skills development starting from childhood development and continuing through adulthood, including for girls, persons with disabilities, indigenous peoples and children in vulnerable situations, Improvements to the access to education it hopes to ensure that all youth and a substantial proportion of adults achieve literacy and numeracy. It also seeks to build and upgrade education facilities and to increase the supply of qualified teachers.<p>**Company-Level Issue Examples** *- Mentorship and training, Education company quality, Education company ethics.*| |**GOAL5GENDEREQUALITY**|**Gender Equality** - Goal 5 emphasizes eliminating discrimination and violence against women and girls. The Goal emphasizes ensuring women's full and effective participation and equal opportunities for leadership at all levels of decision-making in political, economic and public life. Access to sexual and reproductive health and reproductive rights and access to economic resources (e.g., land ownership, financial services) are also emphasized.<p>**Company-Level Issue Examples** *- Board Diversity, Gender Discrimination, Sexual Harassment.*| |**GOAL6CLEANWATERANDSANITATION**|**Clean Water and Sanitation** - Goal 6 not only addresses issues relating to drinking water, sanitation and hygiene, but also the quality and sustainability of water resources worldwide. It strives to achieve universal and equitable access to safe and affordable drinking water for all. It also focuses on adequate and equitable sanitation and hygiene and reducing pollution, minimizing release of hazardous chemicals and materials, and protection of water-related ecosystems. It also highlights increasing water-use efficiency across all sectors, recycling, and ensuring sustainable withdrawals and supply of freshwater.<p>**Company-Level Issue Examples** *- Water Pollution, Water Recycling and Stewardship, Water Infrastructure.*| |**GOAL7AFFORDABLEANDCLEANENERGY**|**Goal 7 Affordable and Clean Energy** - Goal 7 seeks to ensure access to affordable, reliable, and modern energy services for all. It aims to increase renewable energy in the global energy mix and improve energy efficiency significantly. It also calls for more access to clean energy research, technology, and infrastructure for renewable energy, energy efficiency, and advanced and cleaner fossil-fuel technology, and promoting investment in energy infrastructure and clean energy technology.<p>**Company-Level Issue Examples** *- Green Buildings, Renewable Energy, Unethical Utility Pricing.*| |**GOAL8DECENTWORKANDECONOMICGROWTH**|**Decent Work and Economic Growth** - Goal 8 focuses on economic productivity and supports policies for entrepreneurship, creativity and innovation that assist micro, small, and medium-sized enterprises. The Goal also seeks to reduce unemployment, the proportion of youth not working or in school, child labor, and forced labor. Also covered are the protection of labor rights, migrant workers, safe and secure working environments, sustainable tourism, and increasing the capacity of domestic financial institutions in regards to access to banking, insurance, and financial services.<p>**Company-Level Issue Examples** *-  Job Creation, Labor Exploitation, Employee Health and Safety, Workplace Turnover, Supplier Transparency.*| |**GOAL9INDUSTRYINNOVATIONANDINFRASTRUCTURE**|**Industry Innovation and Infrastructure** - Goal 9 focuses on three important aspects of sustainable development, infrastructure, industrialization and innovation, including considerations for resiliency, equity, quality, reliability, access and affordability, and regional and transborder infrastructure. The Goal focuses on infrastructure upgrades and retrofitting of industries with increased resource-use efficiency and clean and environmentally sound technologies and industrial processes.<p>**Company-Level Issue Examples** *- Digital Divide, ESG integration in financial services, Engineering Structural Integrity.*| |**GOAL10REDUCEDINEQUALITIES**|**Reduced Inequalities** - Goal 10 calls for reducing inequalities in income as well as those based on age, sex, disability, race, ethnicity, origin, religion, or economic or other status within a country. The Goal addresses inequalities among countries, including those related to representation, migration, and development assistance. It aims to empower and promote social, economic, and political inclusion of all. The Goal stresses regulation and monitoring of global financial markets and institutions.<p>**Company-Level Issue Examples** *- Responsible Lending, Worker Discrimination, CEO Pay Gap, Worker Pay Gap, Workplace Diversity and Inclusion.*| |**GOAL11SUSTAINABLECITIESANDCOMMUNITIES**|**Sustainable Cities and Communities** - Goal 11 seeks to ensure access for all to adequate, safe, and affordable housing and basic services, and green and public spaces, and to upgrade slums. It focuses on improving transportation, air quality and municipal and other waste management, and creating inclusive and sustainable urbanization through participatory urban planning. The Goal also supports safeguarding the world's cultural and natural heritage, while aiming to increase the number of cities and human settlements adopting and implementing integrated policies and plans towards inclusion, resource efficiency, mitigation and adaptation to climate change, and resilience to disasters.<p>**Company-Level Issue Examples** *- Air Pollution, Environmental Justice, Human Rights Violations, Affordable Housing.*| |**GOAL12RESPONSIBLECONSUMPTIONANDPRODUCTION**|**Responsible Consumption and Production** - Goal 12 aims to achieve the sustainable management and efficient use of natural resources through both the public and private sector. It specifically addresses global food waste in consumption, production, and distribution, sustainable tourism, waste and chemicals management. Goal 12 encourages sustainability reporting in the private sector, while in the public sector it encourages restructuring taxation and subsidies for fossil fuels and promoting sustainable public procurement practices.<p>**Company-Level Issue Examples** *- Sustainability Reporting, Circular Economy, Hazardous Waste Management, Waste Reduction.*| |**GOAL13CLIMATEACTION**|**Climate Action** - While Goal 13 is focused on actions by countries towards climate mitigation and adaptation, the private sector can also play a role in these areas. The goal seeks to strengthen resilience and adaptive capacity to climate-related hazards and natural disasters in all countries. It calls for integrating climate change measures, including those related to climate resilience and low GHG development, into national policies, strategies, and planning. It aims to improve education and awareness of climate change mitigation, adaptation, impact reduction, and early warning.<p>**Company-Level Issue Examples** *- GHG Emissions, Sustainable Transportation, Physical Climate Impacts.*| |**GOAL14LIFEBELOWWATER**|**Life Below Water** - Goal 14 focuses on preventing marine pollution of all kinds, particularly from land-based activities, and to minimize and address the impacts of ocean acidification. The Goal also aims to achieve sustainable yields in fisheries, through regulation of harvesting, controlling subsidies, and ending overfishing. It seeks to sustainably manage and protect marine and coastal ecosystems to avoid significant adverse impacts, including by strengthening their resilience, and take action for their restoration in order to achieve healthy and productive oceans.<p>**Company-Level Issue Examples** *- Impacts on water-related endangered species and habitats, Oil Spills, Seafood Sourcing.*| |**GOAL15LIFEONLAND**|**Life On Land** - Goal 15 seeks to ensure the conservation, restoration, and sustainable use of terrestrial and inland freshwater ecosystems and their services, in order to preserve biodiversity. It focuses specifically on sustainably managing forests, halting deforestation, restoring degraded lands and successfully combating desertification, reducing degraded natural habitats and ending biodiversity loss, with an emphasis on threatened species and invasive alien species.<p>**Company-Level Issue Examples** *- Impacts on land-related endangered species and habitats, Sustainable forestry practices and certifications, Project lifecycle environmental impacts.*| |**GOAL16PEACEJUSTICEANDSTRONGINSTITUTIONS**|**Peace, Justice, and Strong Institutions** - Goal 16 aims to significantly reduce all forms of violence, and also focuses specifically on reducing violence against children in the forms of abuse, exploitation, trafficking, and torture. It also aims to significantly reduce illicit financial and arms flows and to substantially reduce corruption and bribery in all their forms. The Goal also emphasizes effective and transparent institutions at all levels, inclusive and participatory decision-making, ensuring public access to information, and protection of fundamental freedoms.<p>**Company-Level Issue Examples** *- Tax Avoidance, Anti-Competitive Behavior, Cyber Security, Corruption, ESG Resolutions.*| . [optional] if omitted the server will use the default value of ["IMPACT"]
-            fields ([str]): Request available SDG Spotlights data fields to be included in the response.  Default is all fields. _fsymId_,_orgId_, _date_, _spotlightId_, _groupId_ and _requestId_ are always included.    <h3>Common Fields</h3>    |field|description|   |---|---|   |fsymId|Factset Regional Security Identifier|   |orgId|Unique identifier assigned by Truvalue that is applied on an organization level |   |date|Date for the period requested in YYYY-MM-DD format.|   |spotlightId|Unique identifier identifying a Spotlight ESG event that is detected at the company level, within a single category.|   |groupId|Unique identifier  identifying a Spotlight group using the Spotlight ID of the Primary Spotlight.|   |requestId|Identifier that was used for the request.|    <h3>SDG Spotlights Fields</h3>     |field|description|   |----|----|   |orgName|The current name of the organization according to Truvalue (not point-in-time)|   |primarySpotlight|Value indicating the primary Spotlight in a Spotlight Group. It could be either \"Yes\" or \"No\".|   |spotlightCategory|SDG category tagged to each Spotlight.|    |status|Indicates status of a spotlight, which can be one of Completed or Ongoing. |   |removed|Displays the date a Spotlight was removed from the dataset, if it has been removed.|    |startDate|Date when a Spotlight has met the volume threshold for Spotlight consideration. Score and volume change metadata are associated with this date.|   |liveDate|Date when a Spotlight meets confidence threshold and is considered a Spotlight. This date should never precede start_date. |             |firstArticleDate|Date of earliest article in the Spotlight as of the Start Date. |   |finalArticleDate|Date of final article in the Spotlight. This value can change over the course of the Spotlight until the Spotlight is marked as completed.|       |organizationVolumeThreshold| The article volume needed to create a Spotlight, as set by the company's overall volume level classification on the Start Date. |    |totalSpotlightVolume|Total number of articles in the Spotlight. This number will change until the Spotlight is marked as completed.|             |startDateVolume|Number of articles in the Spotlight on the Start Date when it met the volume threshold. Does not include the number of articles that were added to the Spotlight after the Spotlight Start Date.|   |primaryArticleSource|Source of the primary article.|    |primaryArticleUrl|URL of the primary article.|              |primaryArticleHeadline|Headline of primary Spotlight article.|             |primaryArticleBulletpoints|Bullet points summarizing the primary article. |   |meanArtScoreFinalDate|Average score of articles in Spotlight on Final Article Date. This score will continue to change until the Spotlight is marked as completed.|      |meanArtScoreStartDate|Average score of articles in Spotlight on Start Date. This score will not change throughout the history of the spotlight.|             |meanPulseScore|Average of pulse scores for each day from First Article Date to Final Article Date, including scores for both Start Date and Final Article Date.|   |pulseBeforeFirstArticle|Pulse score for category at end-of-day on day before the First Article Date. |              |pulseOnFinalArticleDate|Pulse score for category at the end-of-day on the Final Article Date.|             |pulseOnStartDate|Pulse score for the category at the end-of-day on the Start Date. |   |zScoreOnFinalDate|Z-score for Spotlight as of Final Article Date. This score will continue to change until the Spotlight is marked as completed.|          |zScoreOnStartDate|Z-score for Spotlight as of Start Date. This score will not change throughout the history of the spotlight.|   |standoutLvlOnFinalDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.  This score will continue to change until the Spotlight is marked as completed.|    |standoutLvlOnStartDate|Describes if the spotlight is a High, Medium, or Low standout spotlight.|            . [optional]
-            primary_only (bool): This parameter would return only primary spotlights when set to `true` . [optional] if omitted the server will use the default value of True
-            is_removed (bool): This parameter would return the spotlights removed in the response(i.e. Spotlight is marked as Rejected but has a firstApprovedOnDate))when set to `true` Only Spotlights that are marked as approved will be returned when set to `false` . [optional] if omitted the server will use the default value of False
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            ApplyResult[(SpotlightsResponse, int, typing.Dict)]
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
-        kwargs['ids'] = \
-            ids
-        kwargs['start_date'] = \
-            start_date
-        kwargs['end_date'] = \
-            end_date
-        return self.get_sdg_spotlights_endpoint.call_with_http_info(**kwargs)
-
-
-    def get_sdg_spotlights_for_list(
-        self,
-        sdg_spotlights_request,
-        **kwargs
-    ) -> SpotlightsResponse:
-        """Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management  # noqa: E501
-
-        FactSet ESG by Truvalue Labs’ Spotlight Data solutions are a daily collection of the most important positive and negative ESG events detected by our algorithms, with a variety of quantitative metadata to enable timely and systematic trading strategies and portfolio management. Qualitive informational data points such as the headline and key bullet points for articles is also included. reporting is sparse.   # noqa: E501
-        This method makes a synchronous HTTP request. Returns the http data only
-
-        Args:
-            sdg_spotlights_request (SdgSpotlightsRequest): The SDG Article metadata like Dates, Headlines, Articles, Volume
-
-        Keyword Args:
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            SpotlightsResponse
-                Response Object
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=False)
-        kwargs['sdg_spotlights_request'] = \
-            sdg_spotlights_request
-        return self.get_sdg_spotlights_for_list_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_spotlights_for_list_with_http_info(
-        self,
-        sdg_spotlights_request,
-        **kwargs
-    ) -> typing.Tuple[SpotlightsResponse, int, typing.MutableMapping]:
-        """Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management  # noqa: E501
-
-        FactSet ESG by Truvalue Labs’ Spotlight Data solutions are a daily collection of the most important positive and negative ESG events detected by our algorithms, with a variety of quantitative metadata to enable timely and systematic trading strategies and portfolio management. Qualitive informational data points such as the headline and key bullet points for articles is also included. reporting is sparse.   # noqa: E501
-        This method makes a synchronous HTTP request. Returns http data, http status and headers
-
-        Args:
-            sdg_spotlights_request (SdgSpotlightsRequest): The SDG Article metadata like Dates, Headlines, Articles, Volume
-
-        Keyword Args:
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            SpotlightsResponse
-                Response Object
-            int
-                Http Status Code
-            dict
-                Dictionary of the response headers
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=False)
-        kwargs['sdg_spotlights_request'] = \
-            sdg_spotlights_request
-        return self.get_sdg_spotlights_for_list_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_spotlights_for_list_async(
-        self,
-        sdg_spotlights_request,
-        **kwargs
-    ) -> "ApplyResult[SpotlightsResponse]":
-        """Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management  # noqa: E501
-
-        FactSet ESG by Truvalue Labs’ Spotlight Data solutions are a daily collection of the most important positive and negative ESG events detected by our algorithms, with a variety of quantitative metadata to enable timely and systematic trading strategies and portfolio management. Qualitive informational data points such as the headline and key bullet points for articles is also included. reporting is sparse.   # noqa: E501
-        This method makes a asynchronous HTTP request. Returns the http data, wrapped in ApplyResult
-
-        Args:
-            sdg_spotlights_request (SdgSpotlightsRequest): The SDG Article metadata like Dates, Headlines, Articles, Volume
-
-        Keyword Args:
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            ApplyResult[SpotlightsResponse]
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=True, async_req=True)
-        kwargs['sdg_spotlights_request'] = \
-            sdg_spotlights_request
-        return self.get_sdg_spotlights_for_list_endpoint.call_with_http_info(**kwargs)
-
-    def get_sdg_spotlights_for_list_with_http_info_async(
-        self,
-        sdg_spotlights_request,
-        **kwargs
-    ) -> "ApplyResult[typing.Tuple[SpotlightsResponse, int, typing.MutableMapping]]":
-        """Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management  # noqa: E501
-
-        FactSet ESG by Truvalue Labs’ Spotlight Data solutions are a daily collection of the most important positive and negative ESG events detected by our algorithms, with a variety of quantitative metadata to enable timely and systematic trading strategies and portfolio management. Qualitive informational data points such as the headline and key bullet points for articles is also included. reporting is sparse.   # noqa: E501
-        This method makes a asynchronous HTTP request. Returns http data, http status and headers, wrapped in ApplyResult
-
-        Args:
-            sdg_spotlights_request (SdgSpotlightsRequest): The SDG Article metadata like Dates, Headlines, Articles, Volume
-
-        Keyword Args:
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True. NOTE: if this API returns a file, it is the responsibility
-                of the caller to close the file stream.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _spec_property_naming (bool): True if the variable names in the input data
-                are serialized names, as specified in the OpenAPI document.
-                False if the variable names in the input data
-                are pythonic names, e.g. snake case (default)
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-        Returns:
-            ApplyResult[(SpotlightsResponse, int, typing.Dict)]
-        """
-        self.apply_kwargs_defaults(kwargs=kwargs, return_http_data_only=False, async_req=True)
-        kwargs['sdg_spotlights_request'] = \
-            sdg_spotlights_request
-        return self.get_sdg_spotlights_for_list_endpoint.call_with_http_info(**kwargs)
-
-
```

## fds/sdk/FactSetESG/apis/__init__.py

```diff
@@ -12,10 +12,8 @@
 #
 #   import sys
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from fds.sdk.FactSetESG.api.articles_api import ArticlesApi
 from fds.sdk.FactSetESG.api.sasb_api import SASBApi
-from fds.sdk.FactSetESG.api.sdg_api import SDGApi
-from fds.sdk.FactSetESG.api.sfdr_api import SFDRApi
 from fds.sdk.FactSetESG.api.spotlights_api import SpotlightsApi
```

## fds/sdk/FactSetESG/model/articles_fields.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/calendar.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/categories.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/date_of.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/error_response.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/error_response_sub_errors.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/fields_sasb_spotlights.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/frequency.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -105,18 +105,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """Frequency - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Controls the display frequency of the data returned.   * **D** = Daily   * **W** = Weekly, based on the last day of the week of the start date.   * **M** = Monthly, based on the last trading day of the month.   * **CY** = Calendar Annual, based on the last trading day of the calendar year.    . if omitted defaults to "D", must be one of ["D", "W", "M", "CY", "", ]  # noqa: E501
+            args[0] (str): Controls the display frequency of the data returned.   * **D** = Daily   * **W** = Weekly, based on the last day of the week of the start date.   * **M** = Monthly, based on the last trading day of the month.   * **CY** = Calendar Annual, based on the last trading day of the calendar year. . if omitted defaults to "D", must be one of ["D", "W", "M", "CY", "", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Controls the display frequency of the data returned.   * **D** = Daily   * **W** = Weekly, based on the last day of the week of the start date.   * **M** = Monthly, based on the last trading day of the month.   * **CY** = Calendar Annual, based on the last trading day of the calendar year.    . if omitted defaults to "D", must be one of ["D", "W", "M", "CY", "", ]  # noqa: E501
+            value (str): Controls the display frequency of the data returned.   * **D** = Daily   * **W** = Weekly, based on the last day of the week of the start date.   * **M** = Monthly, based on the last trading day of the month.   * **CY** = Calendar Annual, based on the last trading day of the calendar year. . if omitted defaults to "D", must be one of ["D", "W", "M", "CY", "", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -191,18 +191,18 @@
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
         """Frequency - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Controls the display frequency of the data returned.   * **D** = Daily   * **W** = Weekly, based on the last day of the week of the start date.   * **M** = Monthly, based on the last trading day of the month.   * **CY** = Calendar Annual, based on the last trading day of the calendar year.    . if omitted defaults to "D", must be one of ["D", "W", "M", "CY", "", ]  # noqa: E501
+            args[0] (str): Controls the display frequency of the data returned.   * **D** = Daily   * **W** = Weekly, based on the last day of the week of the start date.   * **M** = Monthly, based on the last trading day of the month.   * **CY** = Calendar Annual, based on the last trading day of the calendar year. . if omitted defaults to "D", must be one of ["D", "W", "M", "CY", "", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Controls the display frequency of the data returned.   * **D** = Daily   * **W** = Weekly, based on the last day of the week of the start date.   * **M** = Monthly, based on the last trading day of the month.   * **CY** = Calendar Annual, based on the last trading day of the calendar year.    . if omitted defaults to "D", must be one of ["D", "W", "M", "CY", "", ]  # noqa: E501
+            value (str): Controls the display frequency of the data returned.   * **D** = Daily   * **W** = Weekly, based on the last day of the week of the start date.   * **M** = Monthly, based on the last trading day of the month.   * **CY** = Calendar Annual, based on the last trading day of the calendar year. . if omitted defaults to "D", must be one of ["D", "W", "M", "CY", "", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

## fds/sdk/FactSetESG/model/ids.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/pai_ids.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/rank_categories.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_article.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_articles_categories.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_articles_request.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_articles_response.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_ranks.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_ranks_request.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_ranks_response.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_score_types.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_scores.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -82,15 +82,15 @@
                 and the value is attribute type.
         """
         return {
             'date': (date, none_type,),  # noqa: E501
             'fsym_id': (str, none_type,),  # noqa: E501
             'request_id': (str,),  # noqa: E501
             'sasb_category': (str, none_type,),  # noqa: E501
-            'sasb_score': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'sasb_score': (float, none_type,),  # noqa: E501
             'score_type': (str, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -145,15 +145,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             date (date, none_type): Date for the period requested expressed in YYYY-MM-DD format.. [optional]  # noqa: E501
             fsym_id (str, none_type): FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).. [optional]  # noqa: E501
             request_id (str): Identifier that was used for the request.. [optional]  # noqa: E501
             sasb_category (str, none_type): The specific SASB 'category' the score is referring to.. [optional]  # noqa: E501
-            sasb_score ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): The SASB Score value for the given 'scoreType' and 'category'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
+            sasb_score (float, none_type): The SASB Score value for the given 'scoreType' and 'category'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
             score_type (str, none_type): The name of the specific SASB Score type being shown in the response. This will be represented by the scoreTypes input: PULSE, INSIGHT, MOMENTUM, ART_VOL_TTM, CAT_VOL_TTM, or DYNAMIC_MAT.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -232,15 +232,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             date (date, none_type): Date for the period requested expressed in YYYY-MM-DD format.. [optional]  # noqa: E501
             fsym_id (str, none_type): FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).. [optional]  # noqa: E501
             request_id (str): Identifier that was used for the request.. [optional]  # noqa: E501
             sasb_category (str, none_type): The specific SASB 'category' the score is referring to.. [optional]  # noqa: E501
-            sasb_score ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): The SASB Score value for the given 'scoreType' and 'category'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
+            sasb_score (float, none_type): The SASB Score value for the given 'scoreType' and 'category'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
             score_type (str, none_type): The name of the specific SASB Score type being shown in the response. This will be represented by the scoreTypes input: PULSE, INSIGHT, MOMENTUM, ART_VOL_TTM, CAT_VOL_TTM, or DYNAMIC_MAT.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

## fds/sdk/FactSetESG/model/sasb_scores_all.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
@@ -84,15 +84,15 @@
         return {
             'date': (date, none_type,),  # noqa: E501
             'fsym_id': (str, none_type,),  # noqa: E501
             'request_id': (str,),  # noqa: E501
             'score_type': (str, none_type,),  # noqa: E501
             'access_and_affordability': (float, none_type,),  # noqa: E501
             'air_quality': (float, none_type,),  # noqa: E501
-            'all_categories': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'all_categories': (float, none_type,),  # noqa: E501
             'business_ethics': (float, none_type,),  # noqa: E501
             'business_model_resilience': (float, none_type,),  # noqa: E501
             'competitive_behavior': (float, none_type,),  # noqa: E501
             'critical_incident_risk_management': (float, none_type,),  # noqa: E501
             'customer_privacy': (float, none_type,),  # noqa: E501
             'customer_welfare': (float, none_type,),  # noqa: E501
             'data_security': (float, none_type,),  # noqa: E501
@@ -101,15 +101,15 @@
             'employee_health_and_safety': (float, none_type,),  # noqa: E501
             'energy_management': (float, none_type,),  # noqa: E501
             'g_hg_emissions': (float, none_type,),  # noqa: E501
             'human_rightsand_community_relations': (float, none_type,),  # noqa: E501
             'labor_practices': (float, none_type,),  # noqa: E501
             'management_of_the_legal_and_regulatory_environment': (float, none_type,),  # noqa: E501
             'materials_sourcing_and_efficiency': (float, none_type,),  # noqa: E501
-            'materiality': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type,),  # noqa: E501
+            'materiality': (float, none_type,),  # noqa: E501
             'physical_impacts_of_climate_change': (float, none_type,),  # noqa: E501
             'product_quality_and_safety': (float, none_type,),  # noqa: E501
             'product_design_and_lifecycle_management': (float, none_type,),  # noqa: E501
             'selling_practices_and_product_labeling': (float, none_type,),  # noqa: E501
             'supply_chain_management': (float, none_type,),  # noqa: E501
             'systemic_risk_management': (float, none_type,),  # noqa: E501
             'waste_and_hazardous_materials_management': (float, none_type,),  # noqa: E501
@@ -199,15 +199,15 @@
                                 _visited_composed_classes = (Animal,)
             date (date, none_type): Date for the period requested expressed in YYYY-MM-DD format.. [optional]  # noqa: E501
             fsym_id (str, none_type): FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).. [optional]  # noqa: E501
             request_id (str): Identifier that was used for the request.. [optional]  # noqa: E501
             score_type (str, none_type): The name of the specific SASB Score type being shown in the response. This will be represented by the scoreTypes input: PULSE, INSIGHT, MOMENTUM, ART_VOL_TTM, CAT_VOL_TTM, or DYNAMIC_MAT.. [optional]  # noqa: E501
             access_and_affordability (float, none_type): The Access and Affordability SASB Category.. [optional]  # noqa: E501
             air_quality (float, none_type): The Air Quality SASB Category.. [optional]  # noqa: E501
-            all_categories ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): The All Categories Category. This represents the overall SASB Score for the given 'scoreType'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
+            all_categories (float, none_type): The All Categories Category. This represents the overall SASB Score for the given 'scoreType'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
             business_ethics (float, none_type): The Business Ethics Category.. [optional]  # noqa: E501
             business_model_resilience (float, none_type): The Business Model Resilience Category.. [optional]  # noqa: E501
             competitive_behavior (float, none_type): The Competitive Behavior Category.. [optional]  # noqa: E501
             critical_incident_risk_management (float, none_type): The Critical Incident Risk Management Category.. [optional]  # noqa: E501
             customer_privacy (float, none_type): The Customer Privacy Category.. [optional]  # noqa: E501
             customer_welfare (float, none_type): The Customer Welfare Category.. [optional]  # noqa: E501
             data_security (float, none_type): The Data Security Category.. [optional]  # noqa: E501
@@ -216,15 +216,15 @@
             employee_health_and_safety (float, none_type): The Employee Health And Safety Category.. [optional]  # noqa: E501
             energy_management (float, none_type): The Energy Management Category.. [optional]  # noqa: E501
             g_hg_emissions (float, none_type): The Greenhouse Gases Emissions Category.. [optional]  # noqa: E501
             human_rightsand_community_relations (float, none_type): The Human Rights and Community Relations Category.. [optional]  # noqa: E501
             labor_practices (float, none_type): The Labor Practices Category.. [optional]  # noqa: E501
             management_of_the_legal_and_regulatory_environment (float, none_type): The Management of the Legal and Regulatory Environment Category.. [optional]  # noqa: E501
             materials_sourcing_and_efficiency (float, none_type): The Materials Sourcing and Efficiency Category.. [optional]  # noqa: E501
-            materiality ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): The Materiality Category. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
+            materiality (float, none_type): The Materiality Category. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
             physical_impacts_of_climate_change (float, none_type): The Physical Impacts of Climate Change Category.. [optional]  # noqa: E501
             product_quality_and_safety (float, none_type): The Product Quality and Safety Category.. [optional]  # noqa: E501
             product_design_and_lifecycle_management (float, none_type): The Product Design And Lifecycle Management Category.. [optional]  # noqa: E501
             selling_practices_and_product_labeling (float, none_type): The Selling Practices And Product Labeling Category.. [optional]  # noqa: E501
             supply_chain_management (float, none_type): The Supply Chain Management Category.. [optional]  # noqa: E501
             systemic_risk_management (float, none_type): The Systemic Risk Management Category.. [optional]  # noqa: E501
             waste_and_hazardous_materials_management (float, none_type): The Waste and Hazardous Materials Management Category.. [optional]  # noqa: E501
@@ -312,15 +312,15 @@
                                 _visited_composed_classes = (Animal,)
             date (date, none_type): Date for the period requested expressed in YYYY-MM-DD format.. [optional]  # noqa: E501
             fsym_id (str, none_type): FactSet Entity Identifier. Six alpha-numeric characters, excluding vowels, with a -E suffix (XXXXXX-E).. [optional]  # noqa: E501
             request_id (str): Identifier that was used for the request.. [optional]  # noqa: E501
             score_type (str, none_type): The name of the specific SASB Score type being shown in the response. This will be represented by the scoreTypes input: PULSE, INSIGHT, MOMENTUM, ART_VOL_TTM, CAT_VOL_TTM, or DYNAMIC_MAT.. [optional]  # noqa: E501
             access_and_affordability (float, none_type): The Access and Affordability SASB Category.. [optional]  # noqa: E501
             air_quality (float, none_type): The Air Quality SASB Category.. [optional]  # noqa: E501
-            all_categories ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): The All Categories Category. This represents the overall SASB Score for the given 'scoreType'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
+            all_categories (float, none_type): The All Categories Category. This represents the overall SASB Score for the given 'scoreType'. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
             business_ethics (float, none_type): The Business Ethics Category.. [optional]  # noqa: E501
             business_model_resilience (float, none_type): The Business Model Resilience Category.. [optional]  # noqa: E501
             competitive_behavior (float, none_type): The Competitive Behavior Category.. [optional]  # noqa: E501
             critical_incident_risk_management (float, none_type): The Critical Incident Risk Management Category.. [optional]  # noqa: E501
             customer_privacy (float, none_type): The Customer Privacy Category.. [optional]  # noqa: E501
             customer_welfare (float, none_type): The Customer Welfare Category.. [optional]  # noqa: E501
             data_security (float, none_type): The Data Security Category.. [optional]  # noqa: E501
@@ -329,15 +329,15 @@
             employee_health_and_safety (float, none_type): The Employee Health And Safety Category.. [optional]  # noqa: E501
             energy_management (float, none_type): The Energy Management Category.. [optional]  # noqa: E501
             g_hg_emissions (float, none_type): The Greenhouse Gases Emissions Category.. [optional]  # noqa: E501
             human_rightsand_community_relations (float, none_type): The Human Rights and Community Relations Category.. [optional]  # noqa: E501
             labor_practices (float, none_type): The Labor Practices Category.. [optional]  # noqa: E501
             management_of_the_legal_and_regulatory_environment (float, none_type): The Management of the Legal and Regulatory Environment Category.. [optional]  # noqa: E501
             materials_sourcing_and_efficiency (float, none_type): The Materials Sourcing and Efficiency Category.. [optional]  # noqa: E501
-            materiality ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type): The Materiality Category. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
+            materiality (float, none_type): The Materiality Category. When scoreType = ESG_RANK, the data type will be string, otherwise data type will be a number with double format.. [optional]  # noqa: E501
             physical_impacts_of_climate_change (float, none_type): The Physical Impacts of Climate Change Category.. [optional]  # noqa: E501
             product_quality_and_safety (float, none_type): The Product Quality and Safety Category.. [optional]  # noqa: E501
             product_design_and_lifecycle_management (float, none_type): The Product Design And Lifecycle Management Category.. [optional]  # noqa: E501
             selling_practices_and_product_labeling (float, none_type): The Selling Practices And Product Labeling Category.. [optional]  # noqa: E501
             supply_chain_management (float, none_type): The Supply Chain Management Category.. [optional]  # noqa: E501
             systemic_risk_management (float, none_type): The Systemic Risk Management Category.. [optional]  # noqa: E501
             waste_and_hazardous_materials_management (float, none_type): The Waste and Hazardous Materials Management Category.. [optional]  # noqa: E501
```

## fds/sdk/FactSetESG/model/sasb_scores_all_request.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_scores_all_response.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_scores_request.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_scores_response.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_spotlights_categories.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/sasb_spotlights_request.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/spotlights.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/model/spotlights_response.py

```diff
@@ -1,13 +1,13 @@
 """
     FactSet ESG API
 
     FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>   # noqa: E501
 
-    The version of the OpenAPI document: 1.6.0
+    The version of the OpenAPI document: 1.7.0
     Contact: api@factset.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

## fds/sdk/FactSetESG/models/__init__.py

```diff
@@ -12,18 +12,16 @@
 from fds.sdk.FactSetESG.model.articles_fields import ArticlesFields
 from fds.sdk.FactSetESG.model.calendar import Calendar
 from fds.sdk.FactSetESG.model.categories import Categories
 from fds.sdk.FactSetESG.model.date_of import DateOf
 from fds.sdk.FactSetESG.model.error_response import ErrorResponse
 from fds.sdk.FactSetESG.model.error_response_sub_errors import ErrorResponseSubErrors
 from fds.sdk.FactSetESG.model.fields_sasb_spotlights import FieldsSasbSpotlights
-from fds.sdk.FactSetESG.model.fields_sdg_spotlights import FieldsSdgSpotlights
 from fds.sdk.FactSetESG.model.frequency import Frequency
 from fds.sdk.FactSetESG.model.ids import Ids
-from fds.sdk.FactSetESG.model.indicators import Indicators
 from fds.sdk.FactSetESG.model.pai_ids import PaiIds
 from fds.sdk.FactSetESG.model.rank_categories import RankCategories
 from fds.sdk.FactSetESG.model.sasb_article import SasbArticle
 from fds.sdk.FactSetESG.model.sasb_articles_categories import SasbArticlesCategories
 from fds.sdk.FactSetESG.model.sasb_articles_request import SasbArticlesRequest
 from fds.sdk.FactSetESG.model.sasb_articles_response import SasbArticlesResponse
 from fds.sdk.FactSetESG.model.sasb_ranks import SasbRanks
@@ -34,25 +32,9 @@
 from fds.sdk.FactSetESG.model.sasb_scores_all import SasbScoresAll
 from fds.sdk.FactSetESG.model.sasb_scores_all_request import SasbScoresAllRequest
 from fds.sdk.FactSetESG.model.sasb_scores_all_response import SasbScoresAllResponse
 from fds.sdk.FactSetESG.model.sasb_scores_request import SasbScoresRequest
 from fds.sdk.FactSetESG.model.sasb_scores_response import SasbScoresResponse
 from fds.sdk.FactSetESG.model.sasb_spotlights_categories import SasbSpotlightsCategories
 from fds.sdk.FactSetESG.model.sasb_spotlights_request import SasbSpotlightsRequest
-from fds.sdk.FactSetESG.model.sdg_article import SdgArticle
-from fds.sdk.FactSetESG.model.sdg_articles_categories import SdgArticlesCategories
-from fds.sdk.FactSetESG.model.sdg_articles_request import SdgArticlesRequest
-from fds.sdk.FactSetESG.model.sdg_articles_response import SdgArticlesResponse
-from fds.sdk.FactSetESG.model.sdg_categories import SdgCategories
-from fds.sdk.FactSetESG.model.sdg_frequency import SdgFrequency
-from fds.sdk.FactSetESG.model.sdg_score_types import SdgScoreTypes
-from fds.sdk.FactSetESG.model.sdg_scores import SdgScores
-from fds.sdk.FactSetESG.model.sdg_scores_request import SdgScoresRequest
-from fds.sdk.FactSetESG.model.sdg_scores_response import SdgScoresResponse
-from fds.sdk.FactSetESG.model.sdg_spotlight_categories import SdgSpotlightCategories
-from fds.sdk.FactSetESG.model.sdg_spotlights_request import SdgSpotlightsRequest
-from fds.sdk.FactSetESG.model.sfdr_pai import SfdrPai
-from fds.sdk.FactSetESG.model.sfdr_pai_request import SfdrPaiRequest
-from fds.sdk.FactSetESG.model.sfdr_pai_response import SfdrPaiResponse
 from fds.sdk.FactSetESG.model.spotlights import Spotlights
 from fds.sdk.FactSetESG.model.spotlights_response import SpotlightsResponse
-from fds.sdk.FactSetESG.model.tvl_ids import TvlIds
```

## Comparing `fds.sdk.FactSetESG-1.2.3.dist-info/LICENSE` & `fds.sdk.FactSetESG-1.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fds.sdk.FactSetESG-1.2.3.dist-info/METADATA` & `fds.sdk.FactSetESG-1.3.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fds.sdk.FactSetESG
-Version: 1.2.3
+Version: 1.3.0
 Summary: FactSet ESG client library for Python
 Home-page: https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1
 Author: FactSet Research Systems
 License: Apache License, Version 2.0
 Keywords: FactSet,API,SDK
 Platform: UNKNOWN
 Requires-Python: >=3.7
@@ -14,44 +14,45 @@
 Requires-Dist: python-dateutil
 Requires-Dist: fds.sdk.utils (>=1.0.0)
 
 [![FactSet](https://raw.githubusercontent.com/factset/enterprise-sdk/main/docs/images/factset-logo.svg)](https://www.factset.com)
 
 # FactSet ESG client library for Python
 
+[![API Version](https://img.shields.io/badge/api-v1.7.0-blue)](https://developer.factset.com/api-catalog/factset-esg-api)
 [![PyPi](https://img.shields.io/pypi/v/fds.sdk.FactSetESG)](https://pypi.org/project/fds.sdk.FactSetESG/)
 [![Apache-2 license](https://img.shields.io/badge/license-Apache2-brightgreen.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
 FactSet ESG (powered by FactSet Truvalue Labs) applies machine learning to uncover risks and opportunities from companies' Environmental, Social and Governance (ESG) behavior, which are aggregated and categorized into continuously updated, material ESG scores. The service focuses on company ESG behavior from external sources and includes both positive and negative events that go beyond traditional sources of ESG risk data.<p> FactSet ESG extracts, analyzes, and generates scores from millions of documents each month collected from more than 100,000 data sources in over 30 languages. Sources include news, trade journals, NGOs, watchdog groups, trade blogs, industry reports and social media. Products deliver investable insights by revealing value and risk factors from unstructured data at the speed of current events.</p>
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.6.0
-- Package version: 1.2.3
+- API version: 1.7.0
+- SDK version: 1.3.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://developer.factset.com/contact](https://developer.factset.com/contact)
 
 ## Requirements
 
 * Python >= 3.7
 
 ## Installation
 
 ### Poetry
 
 ```shell
-poetry add fds.sdk.utils fds.sdk.FactSetESG==1.2.3
+poetry add fds.sdk.utils fds.sdk.FactSetESG==1.3.0
 ```
 
 ### pip
 
 ```shell
-pip install fds.sdk.utils fds.sdk.FactSetESG==1.2.3
+pip install fds.sdk.utils fds.sdk.FactSetESG==1.3.0
 ```
 
 ## Usage
 
 1. [Generate authentication credentials](../../../../README.md#authentication).
 2. Setup Python environment.
    1. Install and activate python 3.7+. If you're using [pyenv](https://github.com/pyenv/pyenv):
@@ -235,45 +236,35 @@
 
 All URIs are relative to *https://api.factset.com/content*
 
 Class | Method | HTTP request | Description
 ------------ | ------------- | ------------- | -------------
 *ArticlesApi* | [**get_sasb_articles**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/ArticlesApi.md#get_sasb_articles) | **GET** /factset-esg/v1/sasb-articles | Request articles tagged with SASB lens categories from 2016-01-01 to previous day.
 *ArticlesApi* | [**get_sasb_articles_for_list**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/ArticlesApi.md#get_sasb_articles_for_list) | **POST** /factset-esg/v1/sasb-articles | Request articles tagged with SASB lens categories from 2016-01-01 to previous day
-*ArticlesApi* | [**get_sdg_articles**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/ArticlesApi.md#get_sdg_articles) | **GET** /factset-esg/v1/sdg-articles | Request articles tagged with SDG lens categories from 2016-01-01 to previous day.
-*ArticlesApi* | [**get_sdg_articles_for_list**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/ArticlesApi.md#get_sdg_articles_for_list) | **POST** /factset-esg/v1/sdg-articles | Request articles tagged with SDG lens categories from 2016-01-01 to previous day
 *SASBApi* | [**get_sasb_ranks**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SASBApi.md#get_sasb_ranks) | **GET** /factset-esg/v1/sasb-ranks | Gets ESG Rankings for a requested list of ids and dates.
 *SASBApi* | [**get_sasb_ranks_post**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SASBApi.md#get_sasb_ranks_post) | **POST** /factset-esg/v1/sasb-ranks | Get ESG Ranks for a large list of ids and specified date range.
 *SASBApi* | [**get_sasb_scores**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SASBApi.md#get_sasb_scores) | **GET** /factset-esg/v1/sasb-scores | Gets short-term, long-term, and momentum scores based on the 26 ESG categories defined by the Sustainability Accounting Standards Board (SASB).
 *SASBApi* | [**get_sasb_scores_all**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SASBApi.md#get_sasb_scores_all) | **GET** /factset-esg/v1/sasb-scores-all | Gets a flat key value array of scores for named categories of the input scoreType(s).
 *SASBApi* | [**get_sasb_scores_all_post**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SASBApi.md#get_sasb_scores_all_post) | **POST** /factset-esg/v1/sasb-scores-all | Gets a flat key value array of scores for named categories of the input score type(s).
 *SASBApi* | [**get_sasb_scores_post**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SASBApi.md#get_sasb_scores_post) | **POST** /factset-esg/v1/sasb-scores | For a large list of ids, gets short-term, long-term, and momentum scores based on the 26 ESG categories defined by the Sustainability Accounting Standards Board (SASB).
-*SDGApi* | [**get_sdg_scores**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SDGApi.md#get_sdg_scores) | **GET** /factset-esg/v1/sdg-scores | Gets short-term, long-term, and momentum scores based on the 16 Sustainable Development Goals categories defined by the United Nations.
-*SDGApi* | [**get_sdg_scores_post**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SDGApi.md#get_sdg_scores_post) | **POST** /factset-esg/v1/sdg-scores | Gets short-term, long-term, and momentum scores based on the 16 Sustainable Development Goals categories defined by United Nations.
-*SFDRApi* | [**get_sfdr_pai**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SFDRApi.md#get_sfdr_pai) | **GET** /factset-esg/v1/sfdr-pai | Gets Principle Adverse Impact (PAI) data to support compliant SFDR Sustainable Finance Disclosure Regulation (SFDR) reporting
-*SFDRApi* | [**get_sfdr_pai_for_list**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SFDRApi.md#get_sfdr_pai_for_list) | **POST** /factset-esg/v1/sfdr-pai | Gets Principle Adverse Impact (PAI) data to support compliant SFDR Sustainable Finance Disclosure Regulation (SFDR) reporting
 *SpotlightsApi* | [**get_sasb_spotlights**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SpotlightsApi.md#get_sasb_spotlights) | **GET** /factset-esg/v1/sasb-spotlights | Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management
 *SpotlightsApi* | [**get_sasb_spotlights_for_list**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SpotlightsApi.md#get_sasb_spotlights_for_list) | **POST** /factset-esg/v1/sasb-spotlights | Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management
-*SpotlightsApi* | [**get_sdg_spotlights**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SpotlightsApi.md#get_sdg_spotlights) | **GET** /factset-esg/v1/sdg-spotlights | Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management
-*SpotlightsApi* | [**get_sdg_spotlights_for_list**](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SpotlightsApi.md#get_sdg_spotlights_for_list) | **POST** /factset-esg/v1/sdg-spotlights | Gets Spotlight data for the most important positive and negative ESG events to enable timely and systematic trading strategies and portfolio management
 
 
 ## Documentation For Models
 
  - [ArticlesFields](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/ArticlesFields.md)
  - [Calendar](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/Calendar.md)
  - [Categories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/Categories.md)
  - [DateOf](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/DateOf.md)
  - [ErrorResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/ErrorResponse.md)
  - [ErrorResponseSubErrors](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/ErrorResponseSubErrors.md)
  - [FieldsSasbSpotlights](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/FieldsSasbSpotlights.md)
- - [FieldsSdgSpotlights](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/FieldsSdgSpotlights.md)
  - [Frequency](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/Frequency.md)
  - [Ids](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/Ids.md)
- - [Indicators](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/Indicators.md)
  - [PaiIds](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/PaiIds.md)
  - [RankCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/RankCategories.md)
  - [SasbArticle](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbArticle.md)
  - [SasbArticlesCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbArticlesCategories.md)
  - [SasbArticlesRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbArticlesRequest.md)
  - [SasbArticlesResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbArticlesResponse.md)
  - [SasbRanks](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbRanks.md)
@@ -284,32 +275,16 @@
  - [SasbScoresAll](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbScoresAll.md)
  - [SasbScoresAllRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbScoresAllRequest.md)
  - [SasbScoresAllResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbScoresAllResponse.md)
  - [SasbScoresRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbScoresRequest.md)
  - [SasbScoresResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbScoresResponse.md)
  - [SasbSpotlightsCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbSpotlightsCategories.md)
  - [SasbSpotlightsRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SasbSpotlightsRequest.md)
- - [SdgArticle](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgArticle.md)
- - [SdgArticlesCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgArticlesCategories.md)
- - [SdgArticlesRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgArticlesRequest.md)
- - [SdgArticlesResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgArticlesResponse.md)
- - [SdgCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgCategories.md)
- - [SdgFrequency](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgFrequency.md)
- - [SdgScoreTypes](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgScoreTypes.md)
- - [SdgScores](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgScores.md)
- - [SdgScoresRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgScoresRequest.md)
- - [SdgScoresResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgScoresResponse.md)
- - [SdgSpotlightCategories](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgSpotlightCategories.md)
- - [SdgSpotlightsRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SdgSpotlightsRequest.md)
- - [SfdrPai](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SfdrPai.md)
- - [SfdrPaiRequest](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SfdrPaiRequest.md)
- - [SfdrPaiResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SfdrPaiResponse.md)
  - [Spotlights](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/Spotlights.md)
  - [SpotlightsResponse](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/SpotlightsResponse.md)
- - [TvlIds](https://github.com/FactSet/enterprise-sdk/tree/main/code/python/FactSetESG/v1/docs/TvlIds.md)
 
 
 ## Documentation For Authorization
 
 
 ## FactSetApiKey
```

## Comparing `fds.sdk.FactSetESG-1.2.3.dist-info/RECORD` & `fds.sdk.FactSetESG-1.3.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,49 @@
 fds/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fds/sdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-fds/sdk/FactSetESG/__init__.py,sha256=BDV4PekItTFDm9mhJuYk3RojdLLtpHoYZ9rmSsF8qco,1559
-fds/sdk/FactSetESG/api_client.py,sha256=l7b38e3pukBfuQ9RRYMxZOCFo_UDKe7-tLGejsWYEw4,40554
-fds/sdk/FactSetESG/configuration.py,sha256=n7sTJX_VEmUPvILYWi1kwrpu3iRiPwGFBkb-3ia9d-k,19130
-fds/sdk/FactSetESG/exceptions.py,sha256=ZqUelIFdr_1RLbO6XzNwiWwksVnQruf9wObLb_LMqfE,5849
-fds/sdk/FactSetESG/model_utils.py,sha256=nKcZmpfhqkmJ-GWsdLrnQtREJX-aNZKYlapluCx-gqk,83237
-fds/sdk/FactSetESG/rest.py,sha256=dhQSKGtdyUsJOzaICBTr34rNcon1OQFjKZvwqyYZjng,14977
+fds/sdk/FactSetESG/__init__.py,sha256=sOjlhVQiqpRMAKjU3A0mUOC7geLED3x_vy8sGdUPrgM,1559
+fds/sdk/FactSetESG/api_client.py,sha256=7lLZ8i6IvyLQUdJFNqktPkK0JW3Wf3_qF0mk30snKHg,40554
+fds/sdk/FactSetESG/configuration.py,sha256=V0EqHaBv13JEOhvPxFMrs2UQyRf094Mcm0iO23YVodk,19130
+fds/sdk/FactSetESG/exceptions.py,sha256=_sFtB4ITeNeeAVfzw51DX8Y3qlSqy1h7XG48Tgn1YNI,5849
+fds/sdk/FactSetESG/model_utils.py,sha256=tGhH2HjmLDg4M5a7mZLcVnUxDSsQdqb0KwXPMDL_Zi4,83237
+fds/sdk/FactSetESG/rest.py,sha256=YHjtjF0EMQvytS2kbnMyW9yIlOAtZsr0m3EVprvDfH0,14977
 fds/sdk/FactSetESG/api/__init__.py,sha256=qNxixS-1ooYoEECnFjZlewLDDJ2GRKOX-qdBlHMcm5k,223
-fds/sdk/FactSetESG/api/articles_api.py,sha256=v3ND-ZRmbwu7Cji43DHhz3TwdziTG5I8rcuZBJ5kYF4,192999
-fds/sdk/FactSetESG/api/sasb_api.py,sha256=eK_WAWv_6ZdMn43gaOK4PCRTDkJ9mmXwupZqn8e6nyE,219451
-fds/sdk/FactSetESG/api/sdg_api.py,sha256=wkT089xkjfVb_b7T7V20K4y2epx9AbxtRymDjwjTpLY,94994
-fds/sdk/FactSetESG/api/sfdr_api.py,sha256=yqm6hff-Kke_teK9wSNqOxeLPiUq9LBMqzOVGl6DPyA,47995
-fds/sdk/FactSetESG/api/spotlights_api.py,sha256=YOezvtA04lM7eOeenwKLcOWm5LAauG3Pc-xWKjmUmTE,224913
-fds/sdk/FactSetESG/apis/__init__.py,sha256=VuK-ZzNah2pVqUf2bIG4uJjzhXWpPP52PKaafrlc-WY,693
+fds/sdk/FactSetESG/api/articles_api.py,sha256=a9-0CCm07m7_LupYCsi3NZr-HW7jVSMscSvVAT4Hdpo,112412
+fds/sdk/FactSetESG/api/sasb_api.py,sha256=WEdU-hhSLD2TlOxAuO2igvo-rkedE_FswluVS8l0DaE,219451
+fds/sdk/FactSetESG/api/spotlights_api.py,sha256=svx9S4_zNjHHtw0kJCUKzKj52cN_DV73umDtzqetI5w,128682
+fds/sdk/FactSetESG/apis/__init__.py,sha256=mllnWd2ovZG8PnmkB0rgHULDWJ_ceKrjJFHl3X5zkM0,591
 fds/sdk/FactSetESG/model/__init__.py,sha256=N49d9K35V_Hd5lOHWcMeVRl0Iy_-L-03rZgfKXwlESM,348
-fds/sdk/FactSetESG/model/articles_fields.py,sha256=13fWKUwXs06JQYWERV2gli9IpcOOP3WHfK2zLncZxNQ,15863
-fds/sdk/FactSetESG/model/calendar.py,sha256=m20xgug0UECSbXsAa-vAmxiXEkeQrjlZ_olI1sCZtZk,12840
-fds/sdk/FactSetESG/model/categories.py,sha256=I2sYWm73IYMuo2vYZhB5AfE_Iq847yM0Lyf8VEfxd_0,88611
-fds/sdk/FactSetESG/model/date_of.py,sha256=4uyGszSC0_JtC4794qyIQmS6z1mN-aaWny1u9D8OxLw,12908
-fds/sdk/FactSetESG/model/error_response.py,sha256=7M5xFc6LD6jBnpFmLsV6jIWx5jvSCaGkd3SmbM6UysU,13135
-fds/sdk/FactSetESG/model/error_response_sub_errors.py,sha256=SaSKmBU2wokJ8bk2ra_iWRZAXYayaUh7L1qMNuY2iyc,12618
-fds/sdk/FactSetESG/model/fields_sasb_spotlights.py,sha256=NYVUsPpC6kTMkXhk2qEB4kppY2d67WA5j23UE3k2tyQ,15121
-fds/sdk/FactSetESG/model/fields_sdg_spotlights.py,sha256=uWGIcQRuLugKg4fMH9KMuFqXq3pcC8-0fdk1t-9pDXk,27542
-fds/sdk/FactSetESG/model/frequency.py,sha256=WQ1XqsNTi_F_x5Ta4Lpman4HxQ2byyQklN9Tvtka7nY,13252
-fds/sdk/FactSetESG/model/ids.py,sha256=X0zsJTZkBqGFlaPp2BW5sIHumG8Xkmi6IuGwdgLB3PM,13994
-fds/sdk/FactSetESG/model/indicators.py,sha256=EXOqzsqr4vkGzWSt9mGHGvXecA0TRZWa8eW7Zi4oZOY,21833
-fds/sdk/FactSetESG/model/pai_ids.py,sha256=xIYSU5oSb0xaqapGqPBtHBT7KdGJxQkddtqwcy8L2rI,13787
-fds/sdk/FactSetESG/model/rank_categories.py,sha256=lxmBWSInE5y_WF2OlusWSr7oS8L38-zYc0Wdcnf_hhk,14674
-fds/sdk/FactSetESG/model/sasb_article.py,sha256=3xy9AA6aF33ra1GNh2mbzli5ZznpI9S3-TVSpt_M0R0,12763
-fds/sdk/FactSetESG/model/sasb_articles_categories.py,sha256=8qkIsIMDsPLy5Ih2XsDzgpkvlVF7D9-6Yj94SEJ5ejQ,87145
-fds/sdk/FactSetESG/model/sasb_articles_request.py,sha256=G4ranpRZLPEq6Cz_fwMsVOQ6k8GY3m0xnXRzbQ8PJIA,14273
-fds/sdk/FactSetESG/model/sasb_articles_response.py,sha256=NT4-hykVafQ5QwUF7OTgdliVlVUOyJowWBjNmLqMCu8,12083
-fds/sdk/FactSetESG/model/sasb_ranks.py,sha256=vcVCqGPG3O5ATmfLRl5S7K1ygBOPGIB9U6CGftXhwMs,13737
-fds/sdk/FactSetESG/model/sasb_ranks_request.py,sha256=UxBXKvYAmACPU31owF0Lsl85AA5DKepBNZpAUabbAtY,14393
-fds/sdk/FactSetESG/model/sasb_ranks_response.py,sha256=6YW_YU0iL_zzs_8rGs-FBdCbIIB-eiqbexrnzH9KMVs,12064
-fds/sdk/FactSetESG/model/sasb_score_types.py,sha256=dmQ2FyzYwXqCI_uzix2Vr0D88YnmPU7PMNeTMtuwD1Y,25814
-fds/sdk/FactSetESG/model/sasb_scores.py,sha256=40tQNhFUNFOFFxx-F7YFi3_1CzMPBLm1V79pUoNt2KM,14467
-fds/sdk/FactSetESG/model/sasb_scores_all.py,sha256=YhsSW8rdWmK5aigNMkVoilb3rucEYIbxTG9Ra8pfT0Q,25603
-fds/sdk/FactSetESG/model/sasb_scores_all_request.py,sha256=mhPu0KpfOrx5F0GuS0Gv8VcC4AA7HDvRfcWmrwBx1do,14410
-fds/sdk/FactSetESG/model/sasb_scores_all_response.py,sha256=6_r9-IfknZAW-RyfQRW184pwwvGDwTSFBl74N3c0ob4,12115
-fds/sdk/FactSetESG/model/sasb_scores_request.py,sha256=RdItpjXQWt5ic6vAJXg0m77guJ0Dl-_3PW8Xgqq15ck,14734
-fds/sdk/FactSetESG/model/sasb_scores_response.py,sha256=HUpfxrSez30Wrgx5HgelEo0jhxRfqXMa7n81_CHqtRo,12076
-fds/sdk/FactSetESG/model/sasb_spotlights_categories.py,sha256=bpaQtq6mcw3fT_WKRkeOlXcOjmvjBE56C7cnQBge6Hk,88551
-fds/sdk/FactSetESG/model/sasb_spotlights_request.py,sha256=auC3AxbrC9M-gpdr6viROA8H2-cnHx-FHUnN2Wt6wRI,15200
-fds/sdk/FactSetESG/model/sdg_article.py,sha256=cRhLble6xvKkLPg2AYzBg1f5B_zZvsSLoIvX1qTBTjg,12762
-fds/sdk/FactSetESG/model/sdg_articles_categories.py,sha256=lF4rNAA-UjsJ2YmysnzoHAJXNjQXUUF_12ejNGM5wPc,56820
-fds/sdk/FactSetESG/model/sdg_articles_request.py,sha256=Z4S4UeXFcvv012ZthyMK1oIcX2yFs7BL0YfEW0EK7to,14263
-fds/sdk/FactSetESG/model/sdg_articles_response.py,sha256=zTOAhO2pktBCsiFwglSykGdW6hOJZiGkaOty5XJun7Q,12081
-fds/sdk/FactSetESG/model/sdg_categories.py,sha256=byoaQWsopKxqO_rJ6ZmOnMwHUg3rdfG27hi_Jh1c9pM,58524
-fds/sdk/FactSetESG/model/sdg_frequency.py,sha256=JV0jnJFSWQfrPhaOdDVySLV43dBt8zVLb5CLk1UtUzQ,13313
-fds/sdk/FactSetESG/model/sdg_score_types.py,sha256=4wqpEkpl4nhnGBpjeWmKwcmnMkdcFXerDYi1CfAn4rs,24615
-fds/sdk/FactSetESG/model/sdg_scores.py,sha256=O9UXVWJo-RhrnHoSrkaAOI0dXg865NlR43PlSM-VpJg,13473
-fds/sdk/FactSetESG/model/sdg_scores_request.py,sha256=dTR1Tqw0WHc9rOrcWigLQMGo2a3seIdCA44Dg9IYZXQ,14191
-fds/sdk/FactSetESG/model/sdg_scores_response.py,sha256=H7BkC1y7FiVaANT4B0fFxuj5XS_NKTPOy3cjcDW5648,12064
-fds/sdk/FactSetESG/model/sdg_spotlight_categories.py,sha256=q8sohsjR3gLGcNosHWGJ1ROWIhjWUKeH3nAgbVjpiNU,57491
-fds/sdk/FactSetESG/model/sdg_spotlights_request.py,sha256=UZTllx5-X6opEvcvnKb7O1QmkzSeqpyz2eni72sawRE,15176
-fds/sdk/FactSetESG/model/sfdr_pai.py,sha256=-upzO9Banh9Bnjl6HmJbgWZI8lpPlf7IreKeeNIg3K0,15179
-fds/sdk/FactSetESG/model/sfdr_pai_request.py,sha256=bvUmYiF8oE1eUlqKlf4hTUWz_CCpBNupDewrluW4Uh4,14959
-fds/sdk/FactSetESG/model/sfdr_pai_response.py,sha256=GEAbH6njohsVUwbTJ-GHD8c0tpkc8wk2_DxUi1T3DWk,12056
-fds/sdk/FactSetESG/model/spotlights.py,sha256=pe4eWgvPDpaCDglhJ-c4IyTk4_rbqZixET-M2Ih8djk,12814
-fds/sdk/FactSetESG/model/spotlights_response.py,sha256=IQ0SqLMMP79WDgXLecaRUkHhYsVCYbYTSD7v0xkxUj4,12071
-fds/sdk/FactSetESG/model/tvl_ids.py,sha256=22-rDRVtwKqJzOPzKdyssmiFoROoaN_g4c6PJINnzPk,14047
-fds/sdk/FactSetESG/models/__init__.py,sha256=pJvkRJO4GP6MM9kkwm0_Sguk4fSXY2fz6M5jD0Ds7OQ,3655
-fds.sdk.FactSetESG-1.2.3.dist-info/LICENSE,sha256=o360nv5Th1nES3Sbtp01thapHTMCT0CzuS7uq_ro8fw,11358
-fds.sdk.FactSetESG-1.2.3.dist-info/METADATA,sha256=qT-HrGsz4EwNRlFtj0o6LLZl-NEDJnJCZd_2mAjPz1o,42800
-fds.sdk.FactSetESG-1.2.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-fds.sdk.FactSetESG-1.2.3.dist-info/top_level.txt,sha256=52v1bB-782Xh07STWqzml3q9GVhwaqsY3NCEMiH3Hnc,4
-fds.sdk.FactSetESG-1.2.3.dist-info/RECORD,,
+fds/sdk/FactSetESG/model/articles_fields.py,sha256=UxiCz6yzwqhlXeiuaM3L2pIX1FvAY0shy-ZL4v-U2ZI,15863
+fds/sdk/FactSetESG/model/calendar.py,sha256=NTRop1FNFkoSV5ReCmweluN2Jr-Ku6q0ce6QvKv9n-Q,12840
+fds/sdk/FactSetESG/model/categories.py,sha256=v9PqrklW5PZ0ulW2GSCNLt9BXSNAHcXjmmSjrNNIDB0,88611
+fds/sdk/FactSetESG/model/date_of.py,sha256=5iCJMgDLxhTRhCLzsdz19vLUhR5atHuK72eREDNRE5Y,12908
+fds/sdk/FactSetESG/model/error_response.py,sha256=R5GfkHIeq7MtA4r6S9dnS0qezfWAdOCDnt7QFwTWdx8,13135
+fds/sdk/FactSetESG/model/error_response_sub_errors.py,sha256=-G9G9irbud7VmjB_6ORYHZ_Gmsy8VtkNfL6YJEtkjHA,12618
+fds/sdk/FactSetESG/model/fields_sasb_spotlights.py,sha256=qsYJbSaqzO6IVrgiR881-n4FB_jMXJPguBYlA-WnWdE,15121
+fds/sdk/FactSetESG/model/frequency.py,sha256=OY7gwgXEC2TWejvFSfLqk36E7xGepumhV8c35DCM0hA,13240
+fds/sdk/FactSetESG/model/ids.py,sha256=uAQBIp41y7S7tQ3cDRPeyaJy7Hn6LRUdv2wRiaQssjs,13994
+fds/sdk/FactSetESG/model/pai_ids.py,sha256=srnnSVv2uTN-nYh0H25b5sUij0hgpp9NnYOCJludwc0,13787
+fds/sdk/FactSetESG/model/rank_categories.py,sha256=GuXLy428LNAcbeS-MEUW-3-AQKw-mOwnnHUAb_0ewiw,14674
+fds/sdk/FactSetESG/model/sasb_article.py,sha256=P_F847WQIDI1X7HK7QR8P0XEL07Xg8zRKL9SyXR-5fc,12763
+fds/sdk/FactSetESG/model/sasb_articles_categories.py,sha256=rqxaQueVDkMz_oaMR1rkCEgst7y3t2gOjKO4rXlcgU8,87145
+fds/sdk/FactSetESG/model/sasb_articles_request.py,sha256=4eDB5CjMCVB484e1grbGcOEL8FBgHUGIf8jUGUBBn8g,14273
+fds/sdk/FactSetESG/model/sasb_articles_response.py,sha256=Vh2EZQa9sV6giEBpxb0kx2mbU8GE3awWpKzQICAYE3w,12083
+fds/sdk/FactSetESG/model/sasb_ranks.py,sha256=NZCwueoPfF_XlsLbpq5as6Jm9FXlxEZz-DmMEVhXmF8,13737
+fds/sdk/FactSetESG/model/sasb_ranks_request.py,sha256=n2MQxyO1l4lBJwXSRc0Q5MoMQxbb1QwgZx8m5y1-oDs,14393
+fds/sdk/FactSetESG/model/sasb_ranks_response.py,sha256=QHGC-wv00BKIosV_zx0DRyaHSxLu9P97mn2RmvC_xpw,12064
+fds/sdk/FactSetESG/model/sasb_score_types.py,sha256=Vf8tqzKdH6uIdHvcjvQYrNEvgctm3hkmjzwS-dCyMKI,25814
+fds/sdk/FactSetESG/model/sasb_scores.py,sha256=pVAYzaYxybvOB2-es-c0br7_GMPsCIhVXIqXjKj841g,14275
+fds/sdk/FactSetESG/model/sasb_scores_all.py,sha256=hvyMl_IUHbQuisYz5tXRz_-oYYEEAXq7U-4s1clqSW0,25219
+fds/sdk/FactSetESG/model/sasb_scores_all_request.py,sha256=JX3rGrJLZz6q6_iea4l76XNyEoiwQgqS8pWgXDBhyIw,14410
+fds/sdk/FactSetESG/model/sasb_scores_all_response.py,sha256=svouv_m5kMX5B6GV8d4oANhxyHnaxMieITV1te8q1IU,12115
+fds/sdk/FactSetESG/model/sasb_scores_request.py,sha256=rDB2HjhfjbTir_ESfsATBz0ygBjOHXIjnA9hMVGeYS0,14734
+fds/sdk/FactSetESG/model/sasb_scores_response.py,sha256=IePQy9XFcToB0yIPUgcaMSiBzIzwOnlBkGz7DHc3Op0,12076
+fds/sdk/FactSetESG/model/sasb_spotlights_categories.py,sha256=V9MU1Z0ZoQcUEtVWcwdQD6cfrU3KfPJ7w7DrrYf2fxY,88551
+fds/sdk/FactSetESG/model/sasb_spotlights_request.py,sha256=oSMCkCj4tpKf8uQetrtFdqeFyfSJR_tXBxaOliAvxPw,15200
+fds/sdk/FactSetESG/model/spotlights.py,sha256=QJwe3ycS_teK7_do3peBTNnXSFbVuHaaMkUwreDaI4E,12814
+fds/sdk/FactSetESG/model/spotlights_response.py,sha256=ykgekSai5Rnn98ZQsA7cJpxIDOG6a-ytDswSMzNwDTE,12071
+fds/sdk/FactSetESG/models/__init__.py,sha256=qXv3yxG74qXlyMZWabge4dZ9QAWQJGb-2VZ-u3RtwlA,2403
+fds.sdk.FactSetESG-1.3.0.dist-info/LICENSE,sha256=o360nv5Th1nES3Sbtp01thapHTMCT0CzuS7uq_ro8fw,11358
+fds.sdk.FactSetESG-1.3.0.dist-info/METADATA,sha256=2cPHVUESKqxjsrQttd4oL9dJ4WwJpq1FEkbMrpyuunI,38133
+fds.sdk.FactSetESG-1.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+fds.sdk.FactSetESG-1.3.0.dist-info/top_level.txt,sha256=52v1bB-782Xh07STWqzml3q9GVhwaqsY3NCEMiH3Hnc,4
+fds.sdk.FactSetESG-1.3.0.dist-info/RECORD,,
```

