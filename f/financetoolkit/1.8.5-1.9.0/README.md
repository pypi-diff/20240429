# Comparing `tmp/financetoolkit-1.8.5.tar.gz` & `tmp/financetoolkit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financetoolkit-1.8.5.tar", max compression
+gzip compressed data, was "financetoolkit-1.9.0.tar", max compression
```

## Comparing `financetoolkit-1.8.5.tar` & `financetoolkit-1.9.0.tar`

### file list

```diff
@@ -1,67 +1,73 @@
--rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.8.5/LICENSE.txt
--rw-r--r--   0        0        0   235829 2024-04-02 14:55:09.340278 financetoolkit-1.8.5/README.md
--rw-r--r--   0        0        0      200 2024-04-02 13:53:46.521829 financetoolkit-1.8.5/financetoolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-01-02 16:19:56.729619 financetoolkit-1.8.5/financetoolkit/discovery/__init__.py
--rw-r--r--   0        0        0    52191 2024-01-05 15:16:03.401705 financetoolkit-1.8.5/financetoolkit/discovery/discovery_controller.py
--rw-r--r--   0        0        0    21555 2024-01-02 16:19:56.730152 financetoolkit-1.8.5/financetoolkit/discovery/discovery_model.py
--rw-r--r--   0        0        0        0 2023-12-11 15:16:16.590582 financetoolkit-1.8.5/financetoolkit/economics/__init__.py
--rw-r--r--   0        0        0     2718 2023-12-18 12:15:31.628859 financetoolkit-1.8.5/financetoolkit/economics/ecb_model.py
--rw-r--r--   0        0        0   129829 2024-04-02 14:55:09.341394 financetoolkit-1.8.5/financetoolkit/economics/economics_controller.py
--rw-r--r--   0        0        0     5924 2023-12-18 12:15:31.629485 financetoolkit-1.8.5/financetoolkit/economics/fed_model.py
--rw-r--r--   0        0        0     7889 2024-04-02 14:55:09.341765 financetoolkit-1.8.5/financetoolkit/economics/fred_model.py
--rw-r--r--   0        0        0    41430 2023-12-21 12:41:19.719057 financetoolkit-1.8.5/financetoolkit/economics/oecd_model.py
--rw-r--r--   0        0        0    47381 2024-01-26 13:56:45.140582 financetoolkit-1.8.5/financetoolkit/fundamentals_model.py
--rw-r--r--   0        0        0    18368 2024-04-02 15:17:03.310710 financetoolkit-1.8.5/financetoolkit/helpers.py
--rw-r--r--   0        0        0    43761 2024-04-02 15:19:39.434469 financetoolkit-1.8.5/financetoolkit/historical_model.py
--rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.8.5/financetoolkit/models/__init__.py
--rw-r--r--   0        0        0     7478 2024-02-11 09:36:03.861799 financetoolkit-1.8.5/financetoolkit/models/altman_model.py
--rw-r--r--   0        0        0     5320 2023-12-05 14:17:55.353456 financetoolkit-1.8.5/financetoolkit/models/dupont_model.py
--rw-r--r--   0        0        0     2859 2023-12-05 14:17:55.353743 financetoolkit-1.8.5/financetoolkit/models/enterprise_model.py
--rw-r--r--   0        0        0     1682 2024-01-09 09:12:45.437621 financetoolkit-1.8.5/financetoolkit/models/growth_model.py
--rw-r--r--   0        0        0     1576 2024-02-04 11:49:16.648377 financetoolkit-1.8.5/financetoolkit/models/helpers.py
--rw-r--r--   0        0        0     5562 2024-02-04 11:49:16.648585 financetoolkit-1.8.5/financetoolkit/models/intrinsic_model.py
--rw-r--r--   0        0        0    54517 2024-02-11 09:36:03.862148 financetoolkit-1.8.5/financetoolkit/models/models_controller.py
--rw-r--r--   0        0        0    21129 2023-12-05 14:17:55.355064 financetoolkit-1.8.5/financetoolkit/models/piotroski_model.py
--rw-r--r--   0        0        0     7264 2024-04-02 15:30:42.742540 financetoolkit-1.8.5/financetoolkit/models/wacc_model.py
--rw-r--r--   0        0        0     1795 2023-12-05 12:12:44.159114 financetoolkit-1.8.5/financetoolkit/normalization/balance.csv
--rw-r--r--   0        0        0     1364 2023-12-05 12:12:44.159234 financetoolkit-1.8.5/financetoolkit/normalization/cash.csv
--rw-r--r--   0        0        0     1119 2023-12-05 12:12:44.159347 financetoolkit-1.8.5/financetoolkit/normalization/income.csv
--rw-r--r--   0        0        0      205 2023-12-05 12:12:44.159428 financetoolkit-1.8.5/financetoolkit/normalization/statistics.csv
--rw-r--r--   0        0        0     6859 2023-12-05 14:17:55.355618 financetoolkit-1.8.5/financetoolkit/normalization_model.py
--rw-r--r--   0        0        0        0 2024-01-17 13:13:01.201305 financetoolkit-1.8.5/financetoolkit/options/__init__.py
--rw-r--r--   0        0        0     9128 2024-02-04 11:49:16.649095 financetoolkit-1.8.5/financetoolkit/options/binomial_trees_model.py
--rw-r--r--   0        0        0     3481 2024-01-17 13:13:01.201463 financetoolkit-1.8.5/financetoolkit/options/black_scholes_model.py
--rw-r--r--   0        0        0    27717 2024-01-17 13:13:01.201597 financetoolkit-1.8.5/financetoolkit/options/greeks_model.py
--rw-r--r--   0        0        0     9093 2024-02-04 11:49:16.649301 financetoolkit-1.8.5/financetoolkit/options/helpers.py
--rw-r--r--   0        0        0   211062 2024-04-02 14:55:03.298677 financetoolkit-1.8.5/financetoolkit/options/options_controller.py
--rw-r--r--   0        0        0     4540 2024-02-11 09:36:03.863368 financetoolkit-1.8.5/financetoolkit/options/options_model.py
--rw-r--r--   0        0        0        0 2023-12-05 12:12:44.159580 financetoolkit-1.8.5/financetoolkit/performance/__init__.py
--rw-r--r--   0        0        0     7028 2024-01-26 13:56:45.141380 financetoolkit-1.8.5/financetoolkit/performance/helpers.py
--rw-r--r--   0        0        0    70539 2024-01-26 13:56:45.141733 financetoolkit-1.8.5/financetoolkit/performance/performance_controller.py
--rw-r--r--   0        0        0    25650 2024-01-26 13:56:45.141950 financetoolkit-1.8.5/financetoolkit/performance/performance_model.py
--rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.8.5/financetoolkit/ratios/__init__.py
--rw-r--r--   0        0        0     9837 2024-01-05 15:16:03.403144 financetoolkit-1.8.5/financetoolkit/ratios/efficiency_model.py
--rw-r--r--   0        0        0     5029 2023-12-05 14:17:55.357009 financetoolkit-1.8.5/financetoolkit/ratios/liquidity_model.py
--rw-r--r--   0        0        0    12829 2024-01-05 15:16:03.403517 financetoolkit-1.8.5/financetoolkit/ratios/profitability_model.py
--rw-r--r--   0        0        0   261569 2024-02-04 11:49:16.650933 financetoolkit-1.8.5/financetoolkit/ratios/ratios_controller.py
--rw-r--r--   0        0        0     7011 2023-12-05 14:17:55.357905 financetoolkit-1.8.5/financetoolkit/ratios/solvency_model.py
--rw-r--r--   0        0        0    15318 2024-01-05 15:16:03.404873 financetoolkit-1.8.5/financetoolkit/ratios/valuation_model.py
--rw-r--r--   0        0        0        0 2023-12-05 12:12:44.161409 financetoolkit-1.8.5/financetoolkit/risk/__init__.py
--rw-r--r--   0        0        0     7713 2024-01-05 15:16:03.405414 financetoolkit-1.8.5/financetoolkit/risk/cvar_model.py
--rw-r--r--   0        0        0     1723 2024-01-05 15:16:03.405651 financetoolkit-1.8.5/financetoolkit/risk/evar_model.py
--rw-r--r--   0        0        0     9537 2024-01-05 15:16:03.405900 financetoolkit-1.8.5/financetoolkit/risk/garch_model.py
--rw-r--r--   0        0        0     2531 2024-01-26 13:56:45.142894 financetoolkit-1.8.5/financetoolkit/risk/helpers.py
--rw-r--r--   0        0        0    38389 2024-01-26 13:56:45.143141 financetoolkit-1.8.5/financetoolkit/risk/risk_controller.py
--rw-r--r--   0        0        0     5609 2024-01-05 15:16:03.406914 financetoolkit-1.8.5/financetoolkit/risk/risk_model.py
--rw-r--r--   0        0        0     5471 2024-01-19 13:10:21.010912 financetoolkit-1.8.5/financetoolkit/risk/var_model.py
--rw-r--r--   0        0        0        0 2024-01-17 13:13:01.202491 financetoolkit-1.8.5/financetoolkit/technicals/__init__.py
--rw-r--r--   0        0        0     3620 2024-01-17 13:13:01.202619 financetoolkit-1.8.5/financetoolkit/technicals/breadth_model.py
--rw-r--r--   0        0        0     1993 2024-01-26 13:56:45.143315 financetoolkit-1.8.5/financetoolkit/technicals/helpers.py
--rw-r--r--   0        0        0    16454 2024-01-17 13:13:01.202824 financetoolkit-1.8.5/financetoolkit/technicals/momentum_model.py
--rw-r--r--   0        0        0     2761 2024-01-17 13:13:01.202897 financetoolkit-1.8.5/financetoolkit/technicals/overlap_model.py
--rw-r--r--   0        0        0    14582 2024-04-02 15:45:53.162486 financetoolkit-1.8.5/financetoolkit/technicals/statistic_model.py
--rw-r--r--   0        0        0   134139 2024-01-26 13:56:45.143730 financetoolkit-1.8.5/financetoolkit/technicals/technicals_controller.py
--rw-r--r--   0        0        0     3598 2024-01-17 13:13:01.203383 financetoolkit-1.8.5/financetoolkit/technicals/volatility_model.py
--rw-r--r--   0        0        0   161448 2024-04-02 15:19:40.167959 financetoolkit-1.8.5/financetoolkit/toolkit_controller.py
--rw-r--r--   0        0        0     2492 2024-04-02 15:46:11.943579 financetoolkit-1.8.5/pyproject.toml
--rw-r--r--   0        0        0   236978 1970-01-01 00:00:00.000000 financetoolkit-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 17:19:30.665832 financetoolkit-1.9.0/LICENSE.txt
+-rw-r--r--   0        0        0   247121 2024-04-29 18:24:37.870076 financetoolkit-1.9.0/README.md
+-rw-r--r--   0        0        0      260 2024-04-29 18:23:59.825558 financetoolkit-1.9.0/financetoolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-02 16:19:56.729619 financetoolkit-1.9.0/financetoolkit/discovery/__init__.py
+-rw-r--r--   0        0        0    52191 2024-01-05 15:16:03.401705 financetoolkit-1.9.0/financetoolkit/discovery/discovery_controller.py
+-rw-r--r--   0        0        0    21555 2024-01-02 16:19:56.730152 financetoolkit-1.9.0/financetoolkit/discovery/discovery_model.py
+-rw-r--r--   0        0        0        0 2023-12-11 15:16:16.590582 financetoolkit-1.9.0/financetoolkit/economics/__init__.py
+-rw-r--r--   0        0        0   108131 2024-04-29 18:23:59.826104 financetoolkit-1.9.0/financetoolkit/economics/economics_controller.py
+-rw-r--r--   0        0        0    41430 2023-12-21 12:41:19.719057 financetoolkit-1.9.0/financetoolkit/economics/oecd_model.py
+-rw-r--r--   0        0        0        0 2024-04-29 18:23:59.826176 financetoolkit-1.9.0/financetoolkit/fixedincome/__init__.py
+-rw-r--r--   0        0        0    13245 2024-04-29 18:23:59.844627 financetoolkit-1.9.0/financetoolkit/fixedincome/bond_model.py
+-rw-r--r--   0        0        0     4000 2024-04-29 18:23:59.961651 financetoolkit-1.9.0/financetoolkit/fixedincome/derivative_model.py
+-rw-r--r--   0        0        0     2224 2024-04-29 18:23:59.961882 financetoolkit-1.9.0/financetoolkit/fixedincome/ecb_model.py
+-rw-r--r--   0        0        0     1042 2024-04-29 18:23:59.962023 financetoolkit-1.9.0/financetoolkit/fixedincome/euribor_model.py
+-rw-r--r--   0        0        0     5924 2024-04-29 18:23:59.827045 financetoolkit-1.9.0/financetoolkit/fixedincome/fed_model.py
+-rw-r--r--   0        0        0    66392 2024-04-29 18:24:37.794605 financetoolkit-1.9.0/financetoolkit/fixedincome/fixedincome_controller.py
+-rw-r--r--   0        0        0     7889 2024-04-29 18:23:59.827689 financetoolkit-1.9.0/financetoolkit/fixedincome/fred_model.py
+-rw-r--r--   0        0        0      851 2024-04-29 18:23:59.962735 financetoolkit-1.9.0/financetoolkit/fixedincome/helpers.py
+-rw-r--r--   0        0        0    47381 2024-01-26 13:56:45.140582 financetoolkit-1.9.0/financetoolkit/fundamentals_model.py
+-rw-r--r--   0        0        0    18368 2024-04-02 15:17:03.310710 financetoolkit-1.9.0/financetoolkit/helpers.py
+-rw-r--r--   0        0        0    43761 2024-04-29 18:22:33.320011 financetoolkit-1.9.0/financetoolkit/historical_model.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:54:28.954198 financetoolkit-1.9.0/financetoolkit/models/__init__.py
+-rw-r--r--   0        0        0     7478 2024-02-11 09:36:03.861799 financetoolkit-1.9.0/financetoolkit/models/altman_model.py
+-rw-r--r--   0        0        0     5320 2023-12-05 14:17:55.353456 financetoolkit-1.9.0/financetoolkit/models/dupont_model.py
+-rw-r--r--   0        0        0     2859 2023-12-05 14:17:55.353743 financetoolkit-1.9.0/financetoolkit/models/enterprise_model.py
+-rw-r--r--   0        0        0     1682 2024-01-09 09:12:45.437621 financetoolkit-1.9.0/financetoolkit/models/growth_model.py
+-rw-r--r--   0        0        0     1576 2024-02-04 11:49:16.648377 financetoolkit-1.9.0/financetoolkit/models/helpers.py
+-rw-r--r--   0        0        0     5562 2024-02-04 11:49:16.648585 financetoolkit-1.9.0/financetoolkit/models/intrinsic_model.py
+-rw-r--r--   0        0        0    54517 2024-02-11 09:36:03.862148 financetoolkit-1.9.0/financetoolkit/models/models_controller.py
+-rw-r--r--   0        0        0    21129 2023-12-05 14:17:55.355064 financetoolkit-1.9.0/financetoolkit/models/piotroski_model.py
+-rw-r--r--   0        0        0     7264 2024-04-29 18:22:33.320375 financetoolkit-1.9.0/financetoolkit/models/wacc_model.py
+-rw-r--r--   0        0        0     1795 2023-12-05 12:12:44.159114 financetoolkit-1.9.0/financetoolkit/normalization/balance.csv
+-rw-r--r--   0        0        0     1364 2023-12-05 12:12:44.159234 financetoolkit-1.9.0/financetoolkit/normalization/cash.csv
+-rw-r--r--   0        0        0     1119 2023-12-05 12:12:44.159347 financetoolkit-1.9.0/financetoolkit/normalization/income.csv
+-rw-r--r--   0        0        0      205 2023-12-05 12:12:44.159428 financetoolkit-1.9.0/financetoolkit/normalization/statistics.csv
+-rw-r--r--   0        0        0     6859 2023-12-05 14:17:55.355618 financetoolkit-1.9.0/financetoolkit/normalization_model.py
+-rw-r--r--   0        0        0        0 2024-01-17 13:13:01.201305 financetoolkit-1.9.0/financetoolkit/options/__init__.py
+-rw-r--r--   0        0        0     9128 2024-02-04 11:49:16.649095 financetoolkit-1.9.0/financetoolkit/options/binomial_trees_model.py
+-rw-r--r--   0        0        0     3481 2024-01-17 13:13:01.201463 financetoolkit-1.9.0/financetoolkit/options/black_scholes_model.py
+-rw-r--r--   0        0        0    27717 2024-01-17 13:13:01.201597 financetoolkit-1.9.0/financetoolkit/options/greeks_model.py
+-rw-r--r--   0        0        0     9093 2024-02-04 11:49:16.649301 financetoolkit-1.9.0/financetoolkit/options/helpers.py
+-rw-r--r--   0        0        0   211062 2024-04-29 18:22:33.321511 financetoolkit-1.9.0/financetoolkit/options/options_controller.py
+-rw-r--r--   0        0        0     4540 2024-02-11 09:36:03.863368 financetoolkit-1.9.0/financetoolkit/options/options_model.py
+-rw-r--r--   0        0        0        0 2023-12-05 12:12:44.159580 financetoolkit-1.9.0/financetoolkit/performance/__init__.py
+-rw-r--r--   0        0        0     7028 2024-01-26 13:56:45.141380 financetoolkit-1.9.0/financetoolkit/performance/helpers.py
+-rw-r--r--   0        0        0    70539 2024-04-27 10:10:54.618662 financetoolkit-1.9.0/financetoolkit/performance/performance_controller.py
+-rw-r--r--   0        0        0    25650 2024-01-26 13:56:45.141950 financetoolkit-1.9.0/financetoolkit/performance/performance_model.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:28:40.501711 financetoolkit-1.9.0/financetoolkit/ratios/__init__.py
+-rw-r--r--   0        0        0     9837 2024-01-05 15:16:03.403144 financetoolkit-1.9.0/financetoolkit/ratios/efficiency_model.py
+-rw-r--r--   0        0        0     5029 2023-12-05 14:17:55.357009 financetoolkit-1.9.0/financetoolkit/ratios/liquidity_model.py
+-rw-r--r--   0        0        0    12829 2024-01-05 15:16:03.403517 financetoolkit-1.9.0/financetoolkit/ratios/profitability_model.py
+-rw-r--r--   0        0        0   261569 2024-02-04 11:49:16.650933 financetoolkit-1.9.0/financetoolkit/ratios/ratios_controller.py
+-rw-r--r--   0        0        0     7011 2023-12-05 14:17:55.357905 financetoolkit-1.9.0/financetoolkit/ratios/solvency_model.py
+-rw-r--r--   0        0        0    15318 2024-01-05 15:16:03.404873 financetoolkit-1.9.0/financetoolkit/ratios/valuation_model.py
+-rw-r--r--   0        0        0        0 2023-12-05 12:12:44.161409 financetoolkit-1.9.0/financetoolkit/risk/__init__.py
+-rw-r--r--   0        0        0     7713 2024-01-05 15:16:03.405414 financetoolkit-1.9.0/financetoolkit/risk/cvar_model.py
+-rw-r--r--   0        0        0     1723 2024-01-05 15:16:03.405651 financetoolkit-1.9.0/financetoolkit/risk/evar_model.py
+-rw-r--r--   0        0        0     9537 2024-01-05 15:16:03.405900 financetoolkit-1.9.0/financetoolkit/risk/garch_model.py
+-rw-r--r--   0        0        0     2531 2024-01-26 13:56:45.142894 financetoolkit-1.9.0/financetoolkit/risk/helpers.py
+-rw-r--r--   0        0        0    38389 2024-01-26 13:56:45.143141 financetoolkit-1.9.0/financetoolkit/risk/risk_controller.py
+-rw-r--r--   0        0        0     5609 2024-01-05 15:16:03.406914 financetoolkit-1.9.0/financetoolkit/risk/risk_model.py
+-rw-r--r--   0        0        0     5471 2024-01-19 13:10:21.010912 financetoolkit-1.9.0/financetoolkit/risk/var_model.py
+-rw-r--r--   0        0        0        0 2024-01-17 13:13:01.202491 financetoolkit-1.9.0/financetoolkit/technicals/__init__.py
+-rw-r--r--   0        0        0     3620 2024-01-17 13:13:01.202619 financetoolkit-1.9.0/financetoolkit/technicals/breadth_model.py
+-rw-r--r--   0        0        0     1993 2024-01-26 13:56:45.143315 financetoolkit-1.9.0/financetoolkit/technicals/helpers.py
+-rw-r--r--   0        0        0    16454 2024-01-17 13:13:01.202824 financetoolkit-1.9.0/financetoolkit/technicals/momentum_model.py
+-rw-r--r--   0        0        0     2761 2024-01-17 13:13:01.202897 financetoolkit-1.9.0/financetoolkit/technicals/overlap_model.py
+-rw-r--r--   0        0        0    14582 2024-04-29 18:22:33.321927 financetoolkit-1.9.0/financetoolkit/technicals/statistic_model.py
+-rw-r--r--   0        0        0   134139 2024-01-26 13:56:45.143730 financetoolkit-1.9.0/financetoolkit/technicals/technicals_controller.py
+-rw-r--r--   0        0        0     3598 2024-01-17 13:13:01.203383 financetoolkit-1.9.0/financetoolkit/technicals/volatility_model.py
+-rw-r--r--   0        0        0   164184 2024-04-29 18:23:59.845946 financetoolkit-1.9.0/financetoolkit/toolkit_controller.py
+-rw-r--r--   0        0        0     2497 2024-04-29 18:24:49.034852 financetoolkit-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0   248270 1970-01-01 00:00:00.000000 financetoolkit-1.9.0/PKG-INFO
```

### Comparing `financetoolkit-1.8.5/LICENSE.txt` & `financetoolkit-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/README.md` & `financetoolkit-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,17 @@
 
 # a Risk example
 value_at_risk = companies.risk.get_value_at_risk(period="weekly")
 
 # a Technical example
 ichimoku_cloud = companies.technicals.get_ichimoku_cloud()
 
+# a Fixed Income example
+corporate_bond_yields = companies.fixed_income.get_ice_bofa_effective_yield()
+
 # an Economics example
 unemployment_rates = companies.economics.get_unemployment_rate()
 ````
 
 Generally, the functions return a DataFrame with a multi-index in which all tickers, in this case Apple and Microsoft, are presented. To keep things manageable for this README, I select just Apple but in essence the list of tickers can be endless as I've seen DataFrames with thousands of tickers. The filtering is done through `.loc['AAPL']` and `.xs('AAPL', level=1, axis=1)` based on whether it's fundamental data or historical data respectively.
 
 ### Obtaining Historical Data
@@ -242,14 +245,30 @@
 | 2023-11-02 |     174.005 |           171.725 |          176.235 |            178.8 |
 | 2023-11-03 |     174.005 |           171.725 |          175.558 |            178.8 |
 
 And below the Ichimoku Cloud parameters are plotted for Apple and Microsoft side-by-side.
 
 ![Technicals](https://github.com/JerBouma/FinanceToolkit/assets/46355364/1ced5b34-2410-4206-8ddf-bb053bcb21b2)
 
+### Obtaining Fixed Income Metrics
+
+Get access to the ICE BofA Corporate Bond benchmark indices and a variety of other bond and derivative related valuations within the `fixedincome` module. For example, see the Effective Yield for the ICE BofA Corporate Bond Index below for each Credit Rating:
+
+| Date       |    AAA |     AA |      A |    BBB |     BB |      B |    CCC |
+|:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
+| 2024-04-19 | 0.0518 | 0.0532 | 0.0561 | 0.0594 | 0.0678 | 0.0804 | 0.1385 |
+| 2024-04-22 | 0.0517 | 0.0532 | 0.056  | 0.0593 | 0.0671 | 0.0793 | 0.1377 |
+| 2024-04-23 | 0.0514 | 0.0528 | 0.0556 | 0.0589 | 0.066  | 0.0777 | 0.1364 |
+| 2024-04-24 | 0.0518 | 0.0531 | 0.0559 | 0.0592 | 0.0664 | 0.0778 | 0.1361 |
+| 2024-04-25 | 0.0524 | 0.0537 | 0.0564 | 0.0598 | 0.0673 | 0.079  | 0.1368 |
+
+And below Effective Yields, Option-Adjusted Spreads (OAS), Yield to Worst and Total Returns are plotted over time for the different maturity periods.
+
+![Fixed Income](https://github.com/JerBouma/FinanceToolkit/assets/46355364/816cf251-4152-4341-a08e-a36268f5f721)
+
 ### Understanding Key Economic Indicators
 
 Get insights for 60+ countries into key economic indicators such as the Consumer Price Index (CPI), Gross Domestic Product (GDP), Unemployment Rates and 3-month and 10-year Government Interest Rates. This is done through the `economics` module and can be used as a standalone module as well by using `from financetoolkit import Economics`. For example see a selection of the countries below:
 
 |      |   Colombia |   United States |   Sweden |   Japan |   Germany |
 |:-----|-----------:|----------------:|---------:|--------:|----------:|
 | 2017 |     0.093  |          0.0435 |   0.0686 |  0.0281 |    0.0357 |
@@ -257,15 +276,15 @@
 | 2019 |     0.1037 |          0.0367 |   0.0691 |  0.0235 |    0.0298 |
 | 2020 |     0.1586 |          0.0809 |   0.0848 |  0.0278 |    0.0362 |
 | 2021 |     0.1381 |          0.0537 |   0.0889 |  0.0282 |    0.0358 |
 | 2022 |     0.1122 |          0.0365 |   0.0748 |  0.026  |    0.0307 |
 
 And below these Unemployment Rates are plotted over time:
 
-![Economics](https://github.com/JerBouma/FinanceToolkit/assets/46355364/bb44bd4e-07a1-4ecf-a4eb-7fc09a960930)
+![Economics](https://github.com/JerBouma/FinanceToolkit/assets/46355364/0bba2ce2-9846-42de-a89d-737cdcd07b31)
 
 # Core Functionality and Metrics
 
 The Finance Toolkit has the ability to collect 30+ years of financial statements and calculate 150+ financial metrics. The following list shows all of the available functionality and metrics.
 
 Each ratio and indicator has a corresponding function that can be called directly for example `ratios.get_return_on_equity` or `technicals.get_relative_strength_index`. However, there are also functions that collect multiple ratios or indicators at once such as `ratios.collect_profitability_ratios`. These functions are useful when you want to collect a large amount of ratios or indicators at once.
 
@@ -2528,14 +2547,231 @@
 
 > **Bollinger Bands**
 
 Bollinger Bands are a volatility indicator that consists of three lines: an upper band, a middle band (simple moving average), and a lower band. The upper and lower bands are calculated as the moving average plus and minus a specified number of standard deviations, respectively. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/technicals#get_bollinger_bands).
 
 </details>
 
+## Fixed Income
+
+The Fixed Income module contains a wide variety of fixed income related calculations such as the Effective Yield, the Macaulay Duration, the Modified Duration Convexity, the Yield to Maturity and models such as Black and Bachelier to valuate derivative instruments such as Swaptions. This module can be called directly via the Toolkit but also separately if desired through `from financetoolkit import FixedIncome`. **Find the Notebook [here](https://www.jeroenbouma.com/projects/financetoolkit/fixedincome-module) and the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome) which includes an explanation about each indicator, the parameters and an example.**
+
+<details>
+    <summary><b>Bond Valuations</b></summary>
+The Bond Valuations section contains a variety of metrics to evaluate the performance of bonds. These metrics include Present Value calculations, the Effective Yield, the Macaulay and Modified Duration and convexity.
+
+All bond valuations can be called by using `get_` to get a single valuation. E.g. `get_present_value` or `get_duration`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_present_value()
+```
+
+> **Bond Statistics**
+
+The bond statistics contains a variety of different metrics to evaluate a bond. These include:
+
+- **Par Value:** The face value of the bond.
+- **Coupon Rate:** The annual coupon rate (in decimal).
+- **Years to Maturity:** The number of years until the bond matures.
+- **Yield to Maturity:** The yield to maturity of the bond (in decimal).
+- **Frequency:** The number of coupon payments per year.
+- **Present Value:** The present value of the bond.
+- **Current Yield:** The annual coupon payment divided by the bond price.
+- **Effective Yield:** The return on a bond that has its interest payments (or coupons) reinvested at the same rate by the bondholder.
+- **Macaulay's Duration:** The weighted average time to receive the bond's cash flows.
+- **Modified Duration:** The Macaulay's duration divided by 1 plus the yield to maturity.
+- **Effective Duration:** The percentage change in the bond price for a 1% change in the yield to maturity.
+- **Dollar Duration:** The modified duration multiplied by the bond price.
+- **DV01:** The dollar value of a 0.01% change in yield to maturity.
+- **Convexity:** The second derivative of the bond price with respect to the yield to maturity.
+
+It gives a complete overview of the bond's performance. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_statistics) and an example below which shows the bond statistics for six different bonds using this functionality.
+
+|                     |   Bond 1 |   Bond 2 |   Bond 3 |    Bond 4 |   Bond 5 |   Bond 6 |
+|:--------------------|---------:|---------:|---------:|----------:|---------:|---------:|
+| Par Value           | 100      | 250      |  50      | 1000      |  85      | 320      |
+| Coupon Rate         |   0.05   |   0.02   |   0.075  |    0      |   0.15   |   0.015  |
+| Years to Maturity   |   5      |  10      |   2      |   10      |   3      |   1      |
+| Yield to Maturity   |   0.08   |   0.021  |   0.03   |    0      |   0.16   |   0.04   |
+| Frequency           |   1      |   1      |   4      |    1      |   2      |  12      |
+| Present Value       |  88.0219 | 247.766  |  54.3518 | 1000      |  83.0353 | 312.171  |
+| Current Yield       |   0.0568 |   0.0202 |   0.069  |    0      |   0.1535 |   0.0154 |
+| Effective Yield     |   0.05   |   0.02   |   0.0771 |    0      |   0.1556 |   0.0151 |
+| Macaulay's Duration |   4.5116 |   9.1576 |   1.8849 |   10      |   2.5667 |   0.9932 |
+| Modified Duration   |   4.1774 |   8.9693 |   1.8709 |   10      |   2.3766 |   0.9899 |
+| Effective Duration  |   4.0677 |   8.5181 |   1.8477 |    9.4713 |   2.2952 |   0.9844 |
+| Dollar Duration     |   3.677  |  22.2228 |   1.0168 |  100      |   1.9734 |   3.0902 |
+| DV01                |   0.0004 |   0.0022 |   0      |    0.01   |   0.0001 |   0      |
+| Convexity           |  22.4017 |  93.7509 |   4.0849 |  110      |   7.0923 |   1.0662 |
+
+> **Present Value**
+
+The bond price is the present value of the bond's future cash flows. It is calculated by discounting the bond's coupon payments and principal repayment to the present value using the bond's yield to maturity. The present value is depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_price).
+
+> **Duration**
+
+The bond duration is a measure of the bond's sensitivity to changes in interest rates. It is the weighted average of the bond's cash flows, where the weights are the present value of each cash flow divided by the bond's price. It is possible to calculate the following durations:
+
+- **Macaulay's Duration:** The weighted average time to receive the bond's cash flows.
+- **Modified Duration:** The Macaulay's duration divided by 1 plus the yield to maturity.
+- **Effective Duration:** The percentage change in the bond price for a 1% change in the yield to maturity.
+- **Dollar Duration:** The modified duration multiplied by the bond price.
+
+The duration values are depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_duration).
+
+> **Yield to Maturity**
+
+The Yield to Maturity (YTM) is the total return anticipated on a bond if it is held until it matures. It is the internal rate of return of an investment in a bond if the investor holds the bond until maturity and receives all payments as scheduled. The yield to maturity is depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_yield_to_maturity).
+
+</details>
+
+<details>
+    <summary><b>Derivative Valuations</b></summary>
+The Derivative Valuations section contains a variety of models that can be used to value derivative instruments such as Swaptions. These models include the Black Model and the Bachelier Model.
+
+All derivative valuations can be called by using `get_` to get a single valuation. E.g. `get_derivative_price`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_derivative_price(model_type="black")
+```
+
+> **Black Model**
+
+The Black Model is a mathematical model used to calculate the price of European-style options. It is based on the Black-Scholes model but is used for interest rate options. The Black Model is used to value interest rate options, such as caps, floors, and swaptions. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_derivative_price).
+
+> **Bachelier Model**
+
+The Bachelier Model is a mathematical model used to calculate the price of European-style options. It is based on the normal distribution and is used for interest rate options as opposed to the Black model which uses a log-normal distribution. The Bachelier Model is used to value interest rate options, such as caps, floors, and swaptions. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_derivative_price).
+
+</details>
+
+<details>
+    <summary><b>Central Banks</b></summary>
+
+The central bank metrics revolve around the interest rates of the European Central Bank (ECB) and the Federal Reserve (FED). This includes the main refinancing operations, marginal lending facility, deposit facility, effective federal funds rate, overnight bank funding rate, tri-party general collateral rate, broad general collateral rate and secured overnight financing rate.
+
+All central bank metrics can be called by using `get_` to get a single metric. E.g. `get_european_central_bank_rates` or `get_federal_reserve_rates`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_european_central_bank_rates()
+```
+
+> **Main Refinancing Operations**
+
+The main refinancing operations (MRO) rate is the interest rate banks pay when they borrow money from the ECB for one week. When they do this, they have to provide collateral to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+
+> **Marginal Lending Facility**
+
+The marginal lending facility rate is the interest rate banks pay when they borrow from the ECB overnight. When they do this, they have to provide collateral, for example securities, to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+> **Deposit Facility**
+
+The deposit facility rate is one of the three interest rates the ECB sets every six weeks as part of its monetary policy. The rate defines the interest banks receive for depositing money with the central bank overnight. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+> **Euribor Rates**
+
+The Euro Interbank Offered Rate (Euribor) is a daily reference rate based on the averaged interest rates at which Eurozone banks offer to lend unsecured funds to other banks in the euro wholesale money market. It is widely used as the base rate for a variety of financial products, including mortgages, savings accounts, and derivatives. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_euribor_rates).
+
+> **Effective Federal Funds Rate**
+
+The effective federal funds rate (EFFR) is calculated as a volume-weighted median of overnight federal funds transactions reported in the FR 2420 Report of Selected Money Market Rates. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Overnight Bank Funding Rate**
+
+The overnight bank funding rate (OBFR) is calculated as a volume-weighted median of overnight federal funds transactions, Eurodollar transactions, and the domestic deposits reported as “Selected Deposits” in the FR 2420 Report. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Tri-Party General Collateral Rate**
+
+The TGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Broad General Collateral Rate**
+
+The BGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Secured Overnight Financing Rate (SOFR)**
+
+The SOFR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data and data on bilateral Treasury repo transactions cleared through FICC’s DVP service, which are obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+</details>
+
+<details>
+    <summary><b>Government Bonds</b></summary>
+
+It is possible to view both short-term (3-month) and long-term (10-year) interest rates for each of the available countries. These rates relate to the interest rates at which countries issue government bonds and are used as a benchmark for other interest rates in the economy. For example, the German government bond yield is an overall indicator of the European economy.
+
+These interest rates can be obtained with `get_government_bond_yield`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_government_bond_yield()
+```
+
+> **Long Term Interest Rates (10 year)**
+
+Long-term interest rates refer to government bonds maturing in ten years. Rates are mainly determined by the price charged by the lender, the risk from the borrower and the fall in the capital value. Long-term interest rates are generally averages of daily rates, measured as a percentage. These interest rates are implied by the prices at which the government bonds are traded on financial markets, not the interest rates at which the loans were issued.
+
+In all cases, they refer to bonds whose capital repayment is guaranteed by governments. Long-term interest rates are one of the determinants of business investment. Low long term interest rates encourage investment in new equipment and high interest rates discourage it. Investment is, in turn, a major source of economic growth. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_government_bond_yield).
+
+> **Short Term Interest Rates (3 month)**
+
+Short-term interest rates are the rates at which short-term borrowings are effected between financial institutions or the rate at which short-term government paper is issued or traded in the market. Short-term interest rates are generally averages of daily rates, measured as a percentage.
+
+Short-term interest rates are based on three-month money market rates where available. Typical standardised names are “money market rate” and “treasury bill rate”. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_government_bond_yield).
+
+</details>
+
+<details>
+    <summary><b>Corporate Bonds</b></summary>
+
+The Corporate Bonds section features the widely used ICE BofA benchmarks which include option-adjusted spreads, effective yields and the total returns. It is possible to view both the indices of the ratings (AAA, AA, A, BBB, BB, B and CCC) and the maturities (1-3 years, 3-5 years, 5-7 years, 7-10 years, 10-15 years, 15-30 years and 30+ years).
+
+All corporate bond metrics can be called by using `get_` to get a single metric. E.g. `get_ice_bofa_option_adjusted_spread` or `get_ice_bofa_yield_to_worst`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_ice_bofa_option_adjusted_spread()
+```
+
+> **Option-Adjusted Spread (OAS)**
+
+The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the uncertainty of the cash flows. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_option_adjusted_spread).
+
+> **Effective Yield**
+
+The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price. The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_effective_yield).
+
+> **Total Return**
+
+The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period. Total return includes interest, capital gains, dividends and distributions realized over a given period of time. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_total_return).
+
+> **Yield to Worst**
+
+Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_yield_to_worst).
+
+</details>
+
 ## Key Economic Indicators
 
 The Economics Module contains a variety of Key Economic Indicators that help in understanding the health and performance of more than 60 different countries. This module can be called directly via the Toolkit but also separately if desired through `from financetoolkit import Economics`. **Find the Notebook [here](https://www.jeroenbouma.com/projects/financetoolkit/economics-module) and the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics) which includes an explanation about each indicator, the parameters and an example.**
 
 <details>
     <summary><b>Economy 💵</b></summary>
 
@@ -2655,99 +2891,14 @@
 > **Exchange Rates**
 
 Exchange rates are defined as the price of one country’s’ currency in relation to another country’s currency. This indicator is measured in terms of national currency per US dollar. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_exchange_rates).
 
 </details>
 
 <details>
-    <summary><b>Central Banks 🏦</b></summary>
-
-The central bank metrics revolve around the interest rates of the European Central Bank (ECB) and the Federal Reserve (FED). This includes the main refinancing operations, marginal lending facility, deposit facility, effective federal funds rate, overnight bank funding rate, tri-party general collateral rate, broad general collateral rate and secured overnight financing rate.
-
-All central bank metrics can be called by using `get_` to get a single metric. E.g. `get_european_central_bank_rates` or `get_federal_reserve_rates`. As an example:
-
-```python
-from financetoolkit import Toolkit
-
-toolkit = Toolkit(["AAPL", "TSLA"], api_key="FINANCIAL_MODELING_PREP_KEY")
-
-# Get Central Bank Results
-toolkit.economics.get_european_central_bank_rates()
-```
-
-> **Main Refinancing Operations**
-
-The main refinancing operations (MRO) rate is the interest rate banks pay when they borrow money from the ECB for one week. When they do this, they have to provide collateral to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_european_central_bank_rates).
-
-
-> **Marginal Lending Facility**
-
-The marginal lending facility rate is the interest rate banks pay when they borrow from the ECB overnight. When they do this, they have to provide collateral, for example securities, to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_european_central_bank_rates).
-
-> **Deposit Facility**
-
-The deposit facility rate is one of the three interest rates the ECB sets every six weeks as part of its monetary policy. The rate defines the interest banks receive for depositing money with the central bank overnight. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_european_central_bank_rates).
-
-> **Effective Federal Funds Rate**
-
-The effective federal funds rate (EFFR) is calculated as a volume-weighted median of overnight federal funds transactions reported in the FR 2420 Report of Selected Money Market Rates. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-> **Overnight Bank Funding Rate**
-
-The overnight bank funding rate (OBFR) is calculated as a volume-weighted median of overnight federal funds transactions, Eurodollar transactions, and the domestic deposits reported as “Selected Deposits” in the FR 2420 Report. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-> **Tri-Party General Collateral Rate**
-
-The TGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-> **Broad General Collateral Rate**
-
-The BGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-> **Secured Overnight Financing Rate**
-
-The SOFR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data and data on bilateral Treasury repo transactions cleared through FICC’s DVP service, which are obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-</details>
-
-<details>
-    <summary><b>Fixed Income 📃 </b></summary>
-
-The fixed income metrics revolve around option-adjusted spreads, effective yields and total returns of corporate bonds based on the ICE BofA US Corporate Indices. It is possible to view both the indices of the ratings (AAA, AA, A, BBB, BB, B and CCC) and the maturities (1-3 years, 3-5 years, 5-7 years, 7-10 years, 10-15 years, 15-30 years and 30+ years).
-
-All fixed income metrics can be called by using `get_` to get a single metric. E.g. `get_option_adjusted_spread` or `get_yield_to_worst`. As an example:
-
-```python
-from financetoolkit import Toolkit
-
-toolkit = Toolkit(["AAPL", "TSLA"], api_key="FINANCIAL_MODELING_PREP_KEY")
-
-# Get Fixed Income Results
-toolkit.economics.get_option_adjusted_spread()
-```
-
-> Option-Adjusted Spread (OAS)
-
-The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the uncertainty of the cash flows. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_option_adjusted_spread).
-
-> Effective Yield
-
-The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price. The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_effective_yield).
-
-> Total Return
-
-The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period. Total return includes interest, capital gains, dividends and distributions realized over a given period of time. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_total_return).
-
-> Yield to Worst
-
-Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_yield_to_worst).
-
-</details>
-
-<details>
     <summary><b>Environment 💚</b></summary>
 
 The environment metrics revolve around renewable energy, environmental tax, greenhouse gas emissions, crude oil production and crude oil prices of countries. This includes the renewable energy as a percentage of total energy, environmental tax as a percentage of GDP, greenhouse gas emissions, crude oil production and crude oil prices.
 
 All environment metrics can be called by using `get_` to get a single metric. E.g. `get_renewable_energy` or `get_crude_oil_prices`. As an example:
 
 ```python
```

### Comparing `financetoolkit-1.8.5/financetoolkit/discovery/discovery_controller.py` & `financetoolkit-1.9.0/financetoolkit/discovery/discovery_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/discovery/discovery_model.py` & `financetoolkit-1.9.0/financetoolkit/discovery/discovery_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/economics/ecb_model.py` & `financetoolkit-1.9.0/financetoolkit/fixedincome/ecb_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,29 @@
 """ECB Model"""
 __docformat__ = "google"
 
 import pandas as pd
 
-BASE_URL = "https://data-api.ecb.europa.eu/service/data/FM/"
-EXTENSIONS = "?format=csvdata"
-
-
-def collect_ecb_data(ecb_data_string: str) -> pd.DataFrame:
-    """
-    Collect the data from the ECB API and return it as a DataFrame.
-
-    Args:
-        ecb_data_string (str): The string that is appended to the base URL to
-            get the data from the ECB API.
-
-    Returns:
-       pd.DataFrame: A DataFrame containing the data from the ECB API.
-    """
-    ecb_data = pd.read_csv(f"{BASE_URL}{ecb_data_string}{EXTENSIONS}")
-
-    ecb_data = ecb_data.set_index("TIME_PERIOD")
-
-    ecb_data.index = pd.PeriodIndex(data=ecb_data.index, freq="D")
-
-    ecb_data.index.name = None
-
-    ecb_data = ecb_data["OBS_VALUE"]
-
-    return ecb_data
+from financetoolkit.fixedincome.helpers import collect_ecb_data
 
 
 def get_main_refinancing_operations() -> pd.DataFrame:
     """
     Get the Main Refinancing Operations from the European Central Bank over
     time. The Main Refinancing Operations are the rate at which banks can
     borrow money from the central bank for the duration of one week.
 
     Returns:
        pd.DataFrame: A DataFrame containing the Main Refinancing Operations over time.
     """
     ecb_data_string = "D.U2.EUR.4F.KR.MRR_RT.LEV"
 
-    main_refinancing_operations = collect_ecb_data(ecb_data_string)
+    main_refinancing_operations = collect_ecb_data(
+        ecb_data_string=ecb_data_string, dataset="FM", frequency="D"
+    )
 
     # Convert to percentage
     main_refinancing_operations = main_refinancing_operations / 100
 
     return main_refinancing_operations
 
 
@@ -60,15 +37,17 @@
         per_capita (bool): Whether to return the per capita data or the total data.
 
     Returns:
        pd.DataFrame: A DataFrame containing the Marginal Lending Facility over time.
     """
     ecb_data_string = "D.U2.EUR.4F.KR.MLFR.LEV"
 
-    marginal_lending_facility = collect_ecb_data(ecb_data_string)
+    marginal_lending_facility = collect_ecb_data(
+        ecb_data_string=ecb_data_string, dataset="FM", frequency="D"
+    )
 
     # Convert to percentage
     marginal_lending_facility = marginal_lending_facility / 100
 
     return marginal_lending_facility
 
 
@@ -79,13 +58,15 @@
     use to make overnight deposits with the Eurosystem.
 
     Returns:
        pd.DataFrame: A DataFrame containing the Deposit Facility over time.
     """
     ecb_data_string = "D.U2.EUR.4F.KR.DFR.LEV"
 
-    deposit_facility = collect_ecb_data(ecb_data_string)
+    deposit_facility = collect_ecb_data(
+        ecb_data_string=ecb_data_string, dataset="FM", frequency="D"
+    )
 
     # Convert to percentage
     deposit_facility = deposit_facility / 100
 
     return deposit_facility
```

### Comparing `financetoolkit-1.8.5/financetoolkit/economics/economics_controller.py` & `financetoolkit-1.9.0/financetoolkit/economics/economics_controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 import re
 from datetime import datetime, timedelta
 
 import pandas as pd
 
-from financetoolkit.economics import ecb_model, fed_model, fred_model, oecd_model
+from financetoolkit.economics import oecd_model
 from financetoolkit.helpers import calculate_growth, handle_errors
 
 # pylint: disable=too-many-instance-attributes,too-few-public-methods,too-many-lines,
 # pylint: disable=too-many-locals,line-too-long,too-many-public-methods
 # ruff: noqa: E501
 
 
@@ -1257,468 +1257,14 @@
                 axis="rows",
             )
 
         exchange_rates = exchange_rates.loc[self._start_date : self._end_date]
 
         return exchange_rates.round(rounding if rounding else self._rounding)
 
-    def get_european_central_bank_rates(self, rate: str | None = None):
-        """
-        The Governing Council of the ECB sets the key interest rates for the
-        euro area. The available rates are:
-
-        - Main refinancing operations (refinancing)
-        - Marginal lending facility (lending)
-        - Deposit facility (deposit)
-
-        The main refinancing operations (MRO) rate is the interest rate banks
-        pay when they borrow money from the ECB for one week. When they do this,
-        they have to provide collateral to guarantee that the money will be paid back.
-
-        The marginal lending facility rate is the interest rate banks pay when they
-        borrow from the ECB overnight. When they do this, they have to provide collateral,
-        for example securities, to guarantee that the money will be paid back.
-
-        The deposit facility rate is one of the three interest rates the ECB sets every
-        six weeks as part of its monetary policy. The rate defines the interest banks
-        receive for depositing money with the central bank overnight.
-
-        See source: https://data.ecb.europa.eu/main-figures/
-
-        Args:
-            rate (str, optional): The rate to return. Defaults to None, which returns all rates.
-                Choose between 'refinancing', 'lending' or 'deposit'.
-
-        Returns:
-            pd.DataFrame: A DataFrame containing the ECB rates.
-
-        As an example:
-
-        ```python
-        from financetoolkit import Economics
-
-        economics = Economics(start_date='2023-12-01')
-
-        economics.get_european_central_bank_rates()
-        ```
-
-        Which returns:
-
-        |            |   Refinancing |   Lending |   Deposit |
-        |:-----------|--------------:|----------:|----------:|
-        | 2023-12-01 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-02 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-03 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-04 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-05 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-06 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-07 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-08 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-09 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-10 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-11 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-12 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-13 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-14 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-15 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-16 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-17 |         0.045 |    0.0475 |      0.04 |
-        | 2023-12-18 |         0.045 |    0.0475 |      0.04 |
-        """
-        ecb_rates = pd.DataFrame()
-
-        if rate and rate not in ["refinancing", "lending", "deposit"]:
-            raise ValueError(
-                "Rate must be one of 'refinancing', 'lending' or 'deposit' or left empty for all."
-            )
-
-        if not rate or rate == "refinancing":
-            ecb_rates["Refinancing"] = ecb_model.get_main_refinancing_operations()
-        if not rate or rate == "lending":
-            ecb_rates["Lending"] = ecb_model.get_marginal_lending_facility()
-        if not rate or rate == "deposit":
-            ecb_rates["Deposit"] = ecb_model.get_deposit_facility()
-
-        ecb_rates = ecb_rates.loc[self._start_date : self._end_date]
-
-        return ecb_rates
-
-    def get_federal_reserve_rates(self, rate: str = "EFFR"):
-        """
-        Get the Federal Reserve rates as published by the Federal Reserve Bank of New York.
-        The federal funds market consists of domestic unsecured borrowings in U.S. dollars
-        by depository institutions from other depository institutions and certain other
-        entities, primarily government-sponsored enterprises.
-
-        The following rates are available:
-
-        - Effective Federal Funds Rate (EFFR)
-        - Overnight Bank Funding Rate (OBFR)
-        - Tri-Party General Collateral Rate (TGCR)
-        - Broad General Collateral Rate (BGCR)
-        - Secured Overnight Financing Rate (SOFR)
-
-        The effective federal funds rate (EFFR) is calculated as a volume-weighted median
-        of overnight federal funds transactions reported in the FR 2420 Report of Selected
-        Money Market Rates.
-
-        The overnight bank funding rate (OBFR) is calculated as a volume-weighted median
-        of overnight federal funds transactions, Eurodollar transactions, and the
-        domestic deposits reported as “Selected Deposits” in the FR 2420 Report.
-
-        The TGCR is calculated as a volume-weighted median of transaction-level
-        tri-party repo data collected from the Bank of New York Mellon.
-
-        The BGCR is calculated as a volume-weighted median of transaction-level
-        tri-party repo data collected from the Bank of New York Mellon as well
-        as GCF Repo transaction data obtained from the U.S. Department of the
-        Treasury’s Office of Financial Research (OFR).
-
-        The SOFR is calculated as a volume-weighted median of transaction-level
-        tri-party repo data collected from the Bank of New York Mellon as well as
-        GCF Repo transaction data and data on bilateral Treasury repo transactions
-        cleared through FICC's DVP service, which are obtained from the U.S.
-        Department of the Treasury’s Office of Financial Research (OFR).
-
-        The New York Fed publishes the rates for the prior business day on the New
-        York Fed’s website between 8:00 and 9:00 a.m.
-
-        See source: https://www.newyorkfed.org/markets/reference-rates/
-
-        Args:
-            rate (str): The rate to return. Defaults to 'EFFR' (Effective Federal Funds Rate).
-
-        Returns:
-            pd.DataFrame: A DataFrame containing the Federal Reserve rates including the rate,
-                percentiles, volume and upper and lower bounds.
-
-        As an example:
-
-        ```python
-        from financetoolkit import Economics
-
-        economics = Economics(start_date='2023-12-01')
-
-        effr = economics.get_federal_reserve_rates()
-
-        effr.loc[:, ['Rate', '1st Percentile', '25th Percentile', '75th Percentile', '99th Percentile']]
-        ```
-
-        Which returns:
-
-        | Effective Date   |   Rate |   1st Percentile |   25th Percentile |   75th Percentile |   99th Percentile |
-        |:-----------------|-------:|-----------------:|------------------:|------------------:|------------------:|
-        | 2023-12-01       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0544 |
-        | 2023-12-04       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-05       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-06       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-07       | 0.0533 |            0.053 |            0.0531 |            0.0534 |            0.0545 |
-        | 2023-12-08       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-11       | 0.0533 |            0.053 |            0.0532 |            0.0533 |            0.0545 |
-        | 2023-12-12       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0544 |
-        | 2023-12-13       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0545 |
-        | 2023-12-14       | 0.0533 |            0.053 |            0.0531 |            0.0533 |            0.0535 |
-        """
-        rate = rate.upper()
-
-        if rate == "EFFR":
-            fed_data = fed_model.get_effective_federal_funds_rate()
-        elif rate == "OBFR":
-            fed_data = fed_model.get_overnight_banking_funding_rate()
-        elif rate == "TGCR":
-            fed_data = fed_model.get_tri_party_general_collateral_rate()
-        elif rate == "BGCR":
-            fed_data = fed_model.get_broad_general_collateral_rate()
-        elif rate == "SOFR":
-            fed_data = fed_model.get_secured_overnight_financing_rate()
-        else:
-            raise ValueError(
-                "Rate must be one of 'EFFR', 'OBFR', 'TGCR', 'BGCR' or 'SOFR'."
-            )
-
-        fed_data = fed_data.loc[self._start_date : self._end_date]
-
-        return fed_data
-
-    @handle_errors
-    def get_option_adjusted_spread(
-        self,
-        maturity: bool = True,
-        rounding: int | None = None,
-    ):
-        """
-        The ICE BofA Option-Adjusted Spreads (OASs) are the calculated spreads between a computed OAS index
-        of all bonds in a given maturity and rating category and a spot Treasury curve. An OAS index is constructed
-        using each constituent bond's OAS, weighted by market capitalization.
-
-        The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in
-        basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the
-        market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the
-        uncertainty of the cash flows.
-
-        See definitions:
-
-        - Ratings: https://fred.stlouisfed.org/series/BAMLC0A4CBBB
-        - Maturity: https://fred.stlouisfed.org/series/BAMLC1A0C13Y
-
-        Args:
-            maturity (bool, optional): Whether to return the maturity option adjusted spread or the rating option adjusted spread.
-            rounding (int | None, optional): The number of decimals to round the results to. Defaults to None.
-
-        Returns:
-            pd.DataFrame: A DataFrame containing the Option Adjusted Spread
-
-        As an example:
-
-        ```python
-        from financetoolkit import Economics
-
-        economics = Economics(
-            start_date='2024-01-01',
-            end_date='2024-01-15',
-        )
-
-        economics.get_option_adjusted_spread()
-        ```
-
-        Which returns:
-
-        | Date       |   1-3 Years |   3-5 Years |   5-7 Years |   7-10 Years |   10-15 Years |   15+ Years |
-        |:-----------|------------:|------------:|------------:|-------------:|--------------:|------------:|
-        | 2024-01-01 |          77 |          94 |       108.5 |          127 |         131.5 |         118 |
-        | 2024-01-02 |          78 |          95 |       109   |          128 |         133   |         119 |
-        | 2024-01-03 |          80 |          98 |       113   |          133 |         136   |         122 |
-        | 2024-01-04 |          80 |          98 |       112   |          133 |         135   |         122 |
-        | 2024-01-05 |          80 |          98 |       112   |          132 |         134   |         121 |
-        | 2024-01-08 |          79 |          98 |       112   |          132 |         134   |         120 |
-        | 2024-01-09 |          78 |          96 |       110   |          130 |         131   |         117 |
-        | 2024-01-10 |          77 |          94 |       108   |          128 |         128   |         113 |
-        | 2024-01-11 |          75 |          94 |       107   |          128 |         127   |         113 |
-        | 2024-01-12 |          74 |          94 |       107   |          128 |         126   |         112 |
-        | 2024-01-15 |          74 |          94 |       107   |          128 |         125   |         111 |
-        """
-        option_adjusted_spread = (
-            fred_model.get_maturity_option_adjusted_spread()
-            if maturity
-            else fred_model.get_rating_option_adjusted_spread()
-        )
-
-        option_adjusted_spread = option_adjusted_spread.loc[
-            self._start_date : self._end_date
-        ]
-
-        option_adjusted_spread = option_adjusted_spread.round(
-            rounding if rounding else self._rounding
-        )
-
-        return option_adjusted_spread
-
-    @handle_errors
-    def get_effective_yield(
-        self,
-        maturity: bool = True,
-        rounding: int | None = None,
-    ):
-        """
-        This data represents the effective yield of the ICE BofA Indices, When the last calendar day of the month
-        takes place on the weekend, weekend observations will occur as a result of month ending accrued interest adjustments.
-
-        The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price.
-        The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided
-        by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into
-        account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures.
-
-        See definitions:
-
-        - Ratings: https://fred.stlouisfed.org/series/BAMLC0A4CBBBEY
-        - Maturity: https://fred.stlouisfed.org/series/BAMLC1A0C13YEY
-
-        Args:
-            maturity (bool, optional): Whether to return the maturity effective yield or the rating effective yield.
-            rounding (int | None, optional): The number of decimals to round the results to. Defaults to None.
-
-        Returns:
-            pd.DataFrame: A DataFrame containing the Gross Domestic Product
-
-        As an example:
-
-        ```python
-        from financetoolkit import Economics
-
-        economics = Economics(
-            start_date='2024-01-01',
-            end_date='2024-01-15',
-        )
-
-        economics.get_effective_yield(maturity=False)
-        ```
-
-        Which returns:
-
-        | Date       |    AAA |     AA |      A |    BBB |     BB |      B |    CCC |
-        |:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
-        | 2024-01-01 | 0.0456 | 0.047  | 0.0505 | 0.054  | 0.0613 | 0.0752 | 0.1319 |
-        | 2024-01-02 | 0.0459 | 0.0473 | 0.0509 | 0.0543 | 0.0622 | 0.0763 | 0.1333 |
-        | 2024-01-03 | 0.0459 | 0.0474 | 0.051  | 0.0544 | 0.0634 | 0.0779 | 0.1358 |
-        | 2024-01-04 | 0.0466 | 0.0481 | 0.0518 | 0.0551 | 0.0639 | 0.0784 | 0.1367 |
-        | 2024-01-05 | 0.047  | 0.0485 | 0.0521 | 0.0554 | 0.0641 | 0.0787 | 0.137  |
-        | 2024-01-08 | 0.0465 | 0.0481 | 0.0517 | 0.055  | 0.0633 | 0.0776 | 0.1365 |
-        | 2024-01-09 | 0.0464 | 0.048  | 0.0516 | 0.0548 | 0.0629 | 0.0771 | 0.1359 |
-        | 2024-01-10 | 0.0464 | 0.048  | 0.0515 | 0.0547 | 0.0622 | 0.0762 | 0.1351 |
-        | 2024-01-11 | 0.0456 | 0.0472 | 0.0507 | 0.054  | 0.0619 | 0.076  | 0.1344 |
-        | 2024-01-12 | 0.0451 | 0.0467 | 0.0502 | 0.0534 | 0.0613 | 0.0753 | 0.1338 |
-        | 2024-01-15 | 0.0451 | 0.0467 | 0.0501 | 0.0533 | 0.0611 | 0.0751 | 0.1328 |
-        """
-        effective_yield = (
-            fred_model.get_maturity_effective_yield()
-            if maturity
-            else fred_model.get_rating_effective_yield()
-        )
-
-        effective_yield = effective_yield.loc[self._start_date : self._end_date]
-
-        effective_yield = effective_yield.round(
-            rounding if rounding else self._rounding
-        )
-
-        return effective_yield
-
-    @handle_errors
-    def get_total_return(
-        self,
-        maturity: bool = True,
-        rounding: int | None = None,
-    ):
-        """
-        This data represents the total return of the ICE BofA Indices, When the last calendar day of the month
-        takes place on the weekend, weekend observations will occur as a result of month ending accrued interest adjustments.
-
-        The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period.
-        Total return includes interest, capital gains, dividends and distributions realized over a given period of time.
-
-        See definitions:
-
-        - Ratings: https://fred.stlouisfed.org/series/BAMLC0A4CBBBEY
-        - Maturity: https://fred.stlouisfed.org/series/BAMLC1A0C13YEY
-
-        Args:
-            maturity (bool, optional): Whether to return the maturity total return or the rating total return.
-            rounding (int | None, optional): The number of decimals to round the results to. Defaults to None.
-
-        Returns:
-            pd.DataFrame: A DataFrame containing the Gross Domestic Product
-
-        As an example:
-
-        ```python
-        from financetoolkit import Economics
-
-        economics = Economics(
-            start_date='2024-01-01',
-            end_date='2024-01-15',
-        )
-
-        economics.get_total_return(maturity=True)
-        ```
-
-        Which returns:
-
-        | Date       |   1-3 Years |   3-5 Years |   5-7 Years |   7-10 Years |   10-15 Years |   15+ Years |
-        |:-----------|------------:|------------:|------------:|-------------:|--------------:|------------:|
-        | 2024-01-01 |     1913.78 |     2487.68 |      809.13 |      585.705 |       4206.25 |     4358.69 |
-        | 2024-01-02 |     1912.73 |     2484.25 |      807.62 |      584.32  |       4193.7  |     4343.71 |
-        | 2024-01-03 |     1912.18 |     2483.95 |      807.54 |      583.84  |       4194.39 |     4339.07 |
-        | 2024-01-04 |     1910.86 |     2477.9  |      804.35 |      580.42  |       4163.24 |     4289.24 |
-        | 2024-01-05 |     1910.86 |     2475.75 |      802.82 |      578.73  |       4148.31 |     4262.52 |
-        | 2024-01-08 |     1912.48 |     2480.39 |      804.97 |      580.71  |       4167.04 |     4302.16 |
-        | 2024-01-09 |     1913.5  |     2482.27 |      805.72 |      581.26  |       4173.04 |     4303.34 |
-        | 2024-01-10 |     1914.12 |     2483.6  |      806.21 |      581.29  |       4175.16 |     4304.82 |
-        | 2024-01-11 |     1918.28 |     2492.25 |      809.94 |      583.92  |       4200.49 |     4330.72 |
-        | 2024-01-12 |     1922.1  |     2498.89 |      812.41 |      585.2   |       4213.47 |     4338.43 |
-        | 2024-01-15 |     1922.67 |     2499.76 |      812.67 |      585.41  |       4215.34 |     4340.24 |
-        """
-        total_return = (
-            fred_model.get_maturity_total_return()
-            if maturity
-            else fred_model.get_rating_total_return()
-        )
-
-        total_return = total_return.loc[self._start_date : self._end_date]
-
-        total_return = total_return.round(rounding if rounding else self._rounding)
-
-        return total_return
-
-    @handle_errors
-    def get_yield_to_worst(
-        self,
-        maturity: bool = True,
-        rounding: int | None = None,
-    ):
-        """
-        This data represents the semi-annual yield to worst of the ICE BofA Indices, When the last calendar day of the month
-        takes place on the weekend, weekend observations will occur as a result of month ending accrued interest adjustments.
-
-        Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US
-        convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is
-        to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly.
-
-        See definitions:
-
-        - Ratings: https://fred.stlouisfed.org/series/BAMLC0A4CBBBEY
-        - Maturity: https://fred.stlouisfed.org/series/BAMLC1A0C13YEY
-
-        Args:
-            maturity (bool, optional): Whether to return the maturity yield to worst or the rating yield to worst.
-            rounding (int | None, optional): The number of decimals to round the results to. Defaults to None.
-
-        Returns:
-            pd.DataFrame: A DataFrame containing the Gross Domestic Product
-
-        As an example:
-
-        ```python
-        from financetoolkit import Economics
-
-        economics = Economics(
-            start_date='2024-01-01',
-            end_date='2024-01-15',
-        )
-
-        economics.get_yield_to_worst(maturity=False)
-        ```
-
-        Which returns:
-
-        | Date       |    AAA |     AA |      A |    BBB |     BB |      B |    CCC |
-        |:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
-        | 2024-01-01 | 0.0456 | 0.0472 | 0.0503 | 0.0542 | 0.0645 | 0.0786 | 0.1316 |
-        | 2024-01-02 | 0.046  | 0.0475 | 0.0506 | 0.0546 | 0.0652 | 0.0796 | 0.1329 |
-        | 2024-01-03 | 0.0461 | 0.0475 | 0.0507 | 0.0547 | 0.0662 | 0.081  | 0.1353 |
-        | 2024-01-04 | 0.0468 | 0.0483 | 0.0515 | 0.0554 | 0.0665 | 0.0814 | 0.136  |
-        | 2024-01-05 | 0.0471 | 0.0486 | 0.0518 | 0.0557 | 0.0667 | 0.0816 | 0.1362 |
-        | 2024-01-08 | 0.0466 | 0.0482 | 0.0514 | 0.0553 | 0.066  | 0.0806 | 0.1359 |
-        | 2024-01-09 | 0.0465 | 0.0481 | 0.0513 | 0.0551 | 0.0656 | 0.0803 | 0.1353 |
-        | 2024-01-10 | 0.0465 | 0.0481 | 0.0512 | 0.0551 | 0.065  | 0.0795 | 0.1345 |
-        | 2024-01-11 | 0.0458 | 0.0473 | 0.0504 | 0.0543 | 0.0648 | 0.0793 | 0.134  |
-        | 2024-01-12 | 0.0453 | 0.0468 | 0.0499 | 0.0537 | 0.0642 | 0.0786 | 0.1335 |
-        | 2024-01-15 | 0.0452 | 0.0468 | 0.0498 | 0.0537 | 0.064  | 0.0784 | 0.1325 |
-        """
-        yield_to_worst = (
-            fred_model.get_maturity_yield_to_worst()
-            if maturity
-            else fred_model.get_rating_yield_to_worst()
-        )
-
-        yield_to_worst = yield_to_worst.loc[self._start_date : self._end_date]
-
-        yield_to_worst = yield_to_worst.round(rounding if rounding else self._rounding)
-
-        return yield_to_worst
-
     def get_renewable_energy(
         self,
         growth: bool = False,
         lag: int = 1,
         rounding: int | None = None,
     ):
         """
```

### Comparing `financetoolkit-1.8.5/financetoolkit/economics/fed_model.py` & `financetoolkit-1.9.0/financetoolkit/fixedincome/fed_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/economics/fred_model.py` & `financetoolkit-1.9.0/financetoolkit/fixedincome/fred_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/economics/oecd_model.py` & `financetoolkit-1.9.0/financetoolkit/economics/oecd_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/fundamentals_model.py` & `financetoolkit-1.9.0/financetoolkit/fundamentals_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/helpers.py` & `financetoolkit-1.9.0/financetoolkit/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/historical_model.py` & `financetoolkit-1.9.0/financetoolkit/historical_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/altman_model.py` & `financetoolkit-1.9.0/financetoolkit/models/altman_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/dupont_model.py` & `financetoolkit-1.9.0/financetoolkit/models/dupont_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/enterprise_model.py` & `financetoolkit-1.9.0/financetoolkit/models/enterprise_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/growth_model.py` & `financetoolkit-1.9.0/financetoolkit/models/growth_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/helpers.py` & `financetoolkit-1.9.0/financetoolkit/models/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/intrinsic_model.py` & `financetoolkit-1.9.0/financetoolkit/models/intrinsic_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/models_controller.py` & `financetoolkit-1.9.0/financetoolkit/models/models_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/piotroski_model.py` & `financetoolkit-1.9.0/financetoolkit/models/piotroski_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/models/wacc_model.py` & `financetoolkit-1.9.0/financetoolkit/models/wacc_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/normalization/balance.csv` & `financetoolkit-1.9.0/financetoolkit/normalization/balance.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/normalization/cash.csv` & `financetoolkit-1.9.0/financetoolkit/normalization/cash.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/normalization/income.csv` & `financetoolkit-1.9.0/financetoolkit/normalization/income.csv`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/normalization_model.py` & `financetoolkit-1.9.0/financetoolkit/normalization_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/options/binomial_trees_model.py` & `financetoolkit-1.9.0/financetoolkit/options/binomial_trees_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/options/black_scholes_model.py` & `financetoolkit-1.9.0/financetoolkit/options/black_scholes_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/options/greeks_model.py` & `financetoolkit-1.9.0/financetoolkit/options/greeks_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/options/helpers.py` & `financetoolkit-1.9.0/financetoolkit/options/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/options/options_controller.py` & `financetoolkit-1.9.0/financetoolkit/options/options_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/options/options_model.py` & `financetoolkit-1.9.0/financetoolkit/options/options_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/performance/helpers.py` & `financetoolkit-1.9.0/financetoolkit/performance/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/performance/performance_controller.py` & `financetoolkit-1.9.0/financetoolkit/performance/performance_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/performance/performance_model.py` & `financetoolkit-1.9.0/financetoolkit/performance/performance_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/ratios/efficiency_model.py` & `financetoolkit-1.9.0/financetoolkit/ratios/efficiency_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/ratios/liquidity_model.py` & `financetoolkit-1.9.0/financetoolkit/ratios/liquidity_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/ratios/profitability_model.py` & `financetoolkit-1.9.0/financetoolkit/ratios/profitability_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/ratios/ratios_controller.py` & `financetoolkit-1.9.0/financetoolkit/ratios/ratios_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/ratios/solvency_model.py` & `financetoolkit-1.9.0/financetoolkit/ratios/solvency_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/ratios/valuation_model.py` & `financetoolkit-1.9.0/financetoolkit/ratios/valuation_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/risk/cvar_model.py` & `financetoolkit-1.9.0/financetoolkit/risk/cvar_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/risk/evar_model.py` & `financetoolkit-1.9.0/financetoolkit/risk/evar_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/risk/garch_model.py` & `financetoolkit-1.9.0/financetoolkit/risk/garch_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/risk/helpers.py` & `financetoolkit-1.9.0/financetoolkit/risk/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/risk/risk_controller.py` & `financetoolkit-1.9.0/financetoolkit/risk/risk_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/risk/risk_model.py` & `financetoolkit-1.9.0/financetoolkit/risk/risk_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/risk/var_model.py` & `financetoolkit-1.9.0/financetoolkit/risk/var_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/technicals/breadth_model.py` & `financetoolkit-1.9.0/financetoolkit/technicals/breadth_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/technicals/helpers.py` & `financetoolkit-1.9.0/financetoolkit/technicals/helpers.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/technicals/momentum_model.py` & `financetoolkit-1.9.0/financetoolkit/technicals/momentum_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/technicals/overlap_model.py` & `financetoolkit-1.9.0/financetoolkit/technicals/overlap_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/technicals/statistic_model.py` & `financetoolkit-1.9.0/financetoolkit/technicals/statistic_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/technicals/technicals_controller.py` & `financetoolkit-1.9.0/financetoolkit/technicals/technicals_controller.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/technicals/volatility_model.py` & `financetoolkit-1.9.0/financetoolkit/technicals/volatility_model.py`

 * *Files identical despite different names*

### Comparing `financetoolkit-1.8.5/financetoolkit/toolkit_controller.py` & `financetoolkit-1.9.0/financetoolkit/toolkit_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from datetime import datetime, timedelta
 
 import pandas as pd
 import requests
 
 from financetoolkit import helpers
 from financetoolkit.economics.economics_controller import Economics
+from financetoolkit.fixedincome.fixedincome_controller import FixedIncome
 from financetoolkit.fundamentals_model import (
     get_analyst_estimates as _get_analyst_estimates,
     get_dividend_calendar as _get_dividend_calendar,
     get_earnings_calendar as _get_earnings_calendar,
     get_esg_scores as _get_esg_scores,
     get_financial_statements as _get_financial_statements,
     get_profile as _get_profile,
@@ -697,15 +698,15 @@
         """
         This gives access to the Options module. The Options Module is meant to provide Options valuations
         based on real market data. This includes the Black-Scholes model and in the future the Binomial model
         and the Monte Carlo model. It also includes all available first-order, second-order and third-order
         Greeks such as Delta, Gamma, Theta, Vega, Rho, Charm, Vanna, Vomma, Veta, Speed and Zomma.
 
         It gives insights in the sensitivity of an option to changes in the underlying asset price, volatility,
-        time to maturity, dividend yilds and interest rates and several derivatives of these sensitivities.
+        years to maturity, dividend yilds and interest rates and several derivatives of these sensitivities.
 
         See the following link for more information: https://www.jeroenbouma.com/projects/financetoolkit/docs/options
 
         As an example:
 
         ```python
         from financetoolkit import Toolkit
@@ -1003,14 +1004,67 @@
             historical_data=historical_data,
             intraday_period=self._intraday_period,
             quarterly=self._quarterly,
             rounding=self._rounding,
         )
 
     @property
+    def fixedincome(self) -> FixedIncome:
+        """
+        This gives access to the Fixed Income module. This module contains a wide variety of fixed income
+        related calculations such as the Effective Yield, the Macaulay Duration, the Modified Duration,
+        the Convexity, the Yield to Maturity and models such as Black and Bachelier to valuate derivative
+        instruments such as Swaptions.
+
+        Next to that, it is also possible to acquire Central Bank Rates and ICE BofA Indices such as the
+        ICE BofA US High Yield Index, the ICE BofA US Corporate Index and the ICE BofA US Treasury Index.
+
+        Note that this class can also be directly accessed by importing the FixedIncome class directly via
+        from financetoolkit import FixedIncome. This is useful if you only want to use the FixedIncome class
+        and not the other classes within the Toolkit module.
+
+        See the following link for more information: https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome
+
+        As an example:
+
+        ```python
+        from financetoolkit import FixedIncome
+
+        fixedincome = FixedIncome(
+            start_date='2024-01-01',
+            end_date='2024-01-15',
+        )
+
+        fixedincome.get_effective_yield(maturity=False)
+        ```
+
+        Which returns:
+
+        | Date       |    AAA |     AA |      A |    BBB |     BB |      B |    CCC |
+        |:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
+        | 2024-01-01 | 0.0456 | 0.047  | 0.0505 | 0.054  | 0.0613 | 0.0752 | 0.1319 |
+        | 2024-01-02 | 0.0459 | 0.0473 | 0.0509 | 0.0543 | 0.0622 | 0.0763 | 0.1333 |
+        | 2024-01-03 | 0.0459 | 0.0474 | 0.051  | 0.0544 | 0.0634 | 0.0779 | 0.1358 |
+        | 2024-01-04 | 0.0466 | 0.0481 | 0.0518 | 0.0551 | 0.0639 | 0.0784 | 0.1367 |
+        | 2024-01-05 | 0.047  | 0.0485 | 0.0521 | 0.0554 | 0.0641 | 0.0787 | 0.137  |
+        | 2024-01-08 | 0.0465 | 0.0481 | 0.0517 | 0.055  | 0.0633 | 0.0776 | 0.1365 |
+        | 2024-01-09 | 0.0464 | 0.048  | 0.0516 | 0.0548 | 0.0629 | 0.0771 | 0.1359 |
+        | 2024-01-10 | 0.0464 | 0.048  | 0.0515 | 0.0547 | 0.0622 | 0.0762 | 0.1351 |
+        | 2024-01-11 | 0.0456 | 0.0472 | 0.0507 | 0.054  | 0.0619 | 0.076  | 0.1344 |
+        | 2024-01-12 | 0.0451 | 0.0467 | 0.0502 | 0.0534 | 0.0613 | 0.0753 | 0.1338 |
+        | 2024-01-15 | 0.0451 | 0.0467 | 0.0501 | 0.0533 | 0.0611 | 0.0751 | 0.1328 |
+        """
+        return FixedIncome(
+            start_date=self._start_date,
+            end_date=self._end_date,
+            quarterly=self._quarterly,
+            rounding=self._rounding,
+        )
+
+    @property
     def economics(self) -> Economics:
         """
         This gives access to the Economics module. This module contains a wide variety of economic data
         obtained from OECD. These include things such as the Consumer Price Index (CPI), the Producer
         Price Index (PPI), the Unemployment Rate, the GDP Growth Rate, the Long and Short Term Interest
         Rate and the Consumer Confidence Index.
```

### Comparing `financetoolkit-1.8.5/pyproject.toml` & `financetoolkit-1.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "financetoolkit"
-version = "1.8.5"
+version = "1.9.0"
 description = "Transparent and Efficient Financial Analysis"
 license = "MIT"
 authors = ["Jeroen Bouma"]
 packages = [
     { include = "financetoolkit" },
 ]
 include = ['normalization/*.csv']
@@ -47,15 +47,15 @@
 requests = "^2.31"
 scikit-learn = "^1.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.1"
 pylint = "^2.17.5"
 codespell = "^2.2.5"
-black = "^23.7.0"
+black = ">=23.7,<25.0"
 pytest-mock = "^3.11.1"
 pytest-recording = "^0.13.0"
 pytest-cov = "^4.1.0"
 ruff = "^0.0.287"
 pytest-timeout = "^2.1.0"
 pytest-recorder = "^0.2.3"
 ipykernel = "^6.25.2"
```

### Comparing `financetoolkit-1.8.5/PKG-INFO` & `financetoolkit-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: financetoolkit
-Version: 1.8.5
+Version: 1.9.0
 Summary: Transparent and Efficient Financial Analysis
 Home-page: https://www.jeroenbouma.com/projects/financetoolkit
 License: MIT
 Keywords: Finance,Toolkit,Financial,Analysis,Fundamental,Technical,Quantitative,Database,Equities,Currencies,Economics,ETFs,Funds,Indices,Moneymarkets,Commodities,Options
 Author: Jeroen Bouma
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 5 - Production/Stable
@@ -131,14 +131,17 @@
 
 # a Risk example
 value_at_risk = companies.risk.get_value_at_risk(period="weekly")
 
 # a Technical example
 ichimoku_cloud = companies.technicals.get_ichimoku_cloud()
 
+# a Fixed Income example
+corporate_bond_yields = companies.fixed_income.get_ice_bofa_effective_yield()
+
 # an Economics example
 unemployment_rates = companies.economics.get_unemployment_rate()
 ````
 
 Generally, the functions return a DataFrame with a multi-index in which all tickers, in this case Apple and Microsoft, are presented. To keep things manageable for this README, I select just Apple but in essence the list of tickers can be endless as I've seen DataFrames with thousands of tickers. The filtering is done through `.loc['AAPL']` and `.xs('AAPL', level=1, axis=1)` based on whether it's fundamental data or historical data respectively.
 
 ### Obtaining Historical Data
@@ -266,14 +269,30 @@
 | 2023-11-02 |     174.005 |           171.725 |          176.235 |            178.8 |
 | 2023-11-03 |     174.005 |           171.725 |          175.558 |            178.8 |
 
 And below the Ichimoku Cloud parameters are plotted for Apple and Microsoft side-by-side.
 
 ![Technicals](https://github.com/JerBouma/FinanceToolkit/assets/46355364/1ced5b34-2410-4206-8ddf-bb053bcb21b2)
 
+### Obtaining Fixed Income Metrics
+
+Get access to the ICE BofA Corporate Bond benchmark indices and a variety of other bond and derivative related valuations within the `fixedincome` module. For example, see the Effective Yield for the ICE BofA Corporate Bond Index below for each Credit Rating:
+
+| Date       |    AAA |     AA |      A |    BBB |     BB |      B |    CCC |
+|:-----------|-------:|-------:|-------:|-------:|-------:|-------:|-------:|
+| 2024-04-19 | 0.0518 | 0.0532 | 0.0561 | 0.0594 | 0.0678 | 0.0804 | 0.1385 |
+| 2024-04-22 | 0.0517 | 0.0532 | 0.056  | 0.0593 | 0.0671 | 0.0793 | 0.1377 |
+| 2024-04-23 | 0.0514 | 0.0528 | 0.0556 | 0.0589 | 0.066  | 0.0777 | 0.1364 |
+| 2024-04-24 | 0.0518 | 0.0531 | 0.0559 | 0.0592 | 0.0664 | 0.0778 | 0.1361 |
+| 2024-04-25 | 0.0524 | 0.0537 | 0.0564 | 0.0598 | 0.0673 | 0.079  | 0.1368 |
+
+And below Effective Yields, Option-Adjusted Spreads (OAS), Yield to Worst and Total Returns are plotted over time for the different maturity periods.
+
+![Fixed Income](https://github.com/JerBouma/FinanceToolkit/assets/46355364/816cf251-4152-4341-a08e-a36268f5f721)
+
 ### Understanding Key Economic Indicators
 
 Get insights for 60+ countries into key economic indicators such as the Consumer Price Index (CPI), Gross Domestic Product (GDP), Unemployment Rates and 3-month and 10-year Government Interest Rates. This is done through the `economics` module and can be used as a standalone module as well by using `from financetoolkit import Economics`. For example see a selection of the countries below:
 
 |      |   Colombia |   United States |   Sweden |   Japan |   Germany |
 |:-----|-----------:|----------------:|---------:|--------:|----------:|
 | 2017 |     0.093  |          0.0435 |   0.0686 |  0.0281 |    0.0357 |
@@ -281,15 +300,15 @@
 | 2019 |     0.1037 |          0.0367 |   0.0691 |  0.0235 |    0.0298 |
 | 2020 |     0.1586 |          0.0809 |   0.0848 |  0.0278 |    0.0362 |
 | 2021 |     0.1381 |          0.0537 |   0.0889 |  0.0282 |    0.0358 |
 | 2022 |     0.1122 |          0.0365 |   0.0748 |  0.026  |    0.0307 |
 
 And below these Unemployment Rates are plotted over time:
 
-![Economics](https://github.com/JerBouma/FinanceToolkit/assets/46355364/bb44bd4e-07a1-4ecf-a4eb-7fc09a960930)
+![Economics](https://github.com/JerBouma/FinanceToolkit/assets/46355364/0bba2ce2-9846-42de-a89d-737cdcd07b31)
 
 # Core Functionality and Metrics
 
 The Finance Toolkit has the ability to collect 30+ years of financial statements and calculate 150+ financial metrics. The following list shows all of the available functionality and metrics.
 
 Each ratio and indicator has a corresponding function that can be called directly for example `ratios.get_return_on_equity` or `technicals.get_relative_strength_index`. However, there are also functions that collect multiple ratios or indicators at once such as `ratios.collect_profitability_ratios`. These functions are useful when you want to collect a large amount of ratios or indicators at once.
 
@@ -2552,14 +2571,231 @@
 
 > **Bollinger Bands**
 
 Bollinger Bands are a volatility indicator that consists of three lines: an upper band, a middle band (simple moving average), and a lower band. The upper and lower bands are calculated as the moving average plus and minus a specified number of standard deviations, respectively. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/technicals#get_bollinger_bands).
 
 </details>
 
+## Fixed Income
+
+The Fixed Income module contains a wide variety of fixed income related calculations such as the Effective Yield, the Macaulay Duration, the Modified Duration Convexity, the Yield to Maturity and models such as Black and Bachelier to valuate derivative instruments such as Swaptions. This module can be called directly via the Toolkit but also separately if desired through `from financetoolkit import FixedIncome`. **Find the Notebook [here](https://www.jeroenbouma.com/projects/financetoolkit/fixedincome-module) and the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome) which includes an explanation about each indicator, the parameters and an example.**
+
+<details>
+    <summary><b>Bond Valuations</b></summary>
+The Bond Valuations section contains a variety of metrics to evaluate the performance of bonds. These metrics include Present Value calculations, the Effective Yield, the Macaulay and Modified Duration and convexity.
+
+All bond valuations can be called by using `get_` to get a single valuation. E.g. `get_present_value` or `get_duration`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_present_value()
+```
+
+> **Bond Statistics**
+
+The bond statistics contains a variety of different metrics to evaluate a bond. These include:
+
+- **Par Value:** The face value of the bond.
+- **Coupon Rate:** The annual coupon rate (in decimal).
+- **Years to Maturity:** The number of years until the bond matures.
+- **Yield to Maturity:** The yield to maturity of the bond (in decimal).
+- **Frequency:** The number of coupon payments per year.
+- **Present Value:** The present value of the bond.
+- **Current Yield:** The annual coupon payment divided by the bond price.
+- **Effective Yield:** The return on a bond that has its interest payments (or coupons) reinvested at the same rate by the bondholder.
+- **Macaulay's Duration:** The weighted average time to receive the bond's cash flows.
+- **Modified Duration:** The Macaulay's duration divided by 1 plus the yield to maturity.
+- **Effective Duration:** The percentage change in the bond price for a 1% change in the yield to maturity.
+- **Dollar Duration:** The modified duration multiplied by the bond price.
+- **DV01:** The dollar value of a 0.01% change in yield to maturity.
+- **Convexity:** The second derivative of the bond price with respect to the yield to maturity.
+
+It gives a complete overview of the bond's performance. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_statistics) and an example below which shows the bond statistics for six different bonds using this functionality.
+
+|                     |   Bond 1 |   Bond 2 |   Bond 3 |    Bond 4 |   Bond 5 |   Bond 6 |
+|:--------------------|---------:|---------:|---------:|----------:|---------:|---------:|
+| Par Value           | 100      | 250      |  50      | 1000      |  85      | 320      |
+| Coupon Rate         |   0.05   |   0.02   |   0.075  |    0      |   0.15   |   0.015  |
+| Years to Maturity   |   5      |  10      |   2      |   10      |   3      |   1      |
+| Yield to Maturity   |   0.08   |   0.021  |   0.03   |    0      |   0.16   |   0.04   |
+| Frequency           |   1      |   1      |   4      |    1      |   2      |  12      |
+| Present Value       |  88.0219 | 247.766  |  54.3518 | 1000      |  83.0353 | 312.171  |
+| Current Yield       |   0.0568 |   0.0202 |   0.069  |    0      |   0.1535 |   0.0154 |
+| Effective Yield     |   0.05   |   0.02   |   0.0771 |    0      |   0.1556 |   0.0151 |
+| Macaulay's Duration |   4.5116 |   9.1576 |   1.8849 |   10      |   2.5667 |   0.9932 |
+| Modified Duration   |   4.1774 |   8.9693 |   1.8709 |   10      |   2.3766 |   0.9899 |
+| Effective Duration  |   4.0677 |   8.5181 |   1.8477 |    9.4713 |   2.2952 |   0.9844 |
+| Dollar Duration     |   3.677  |  22.2228 |   1.0168 |  100      |   1.9734 |   3.0902 |
+| DV01                |   0.0004 |   0.0022 |   0      |    0.01   |   0.0001 |   0      |
+| Convexity           |  22.4017 |  93.7509 |   4.0849 |  110      |   7.0923 |   1.0662 |
+
+> **Present Value**
+
+The bond price is the present value of the bond's future cash flows. It is calculated by discounting the bond's coupon payments and principal repayment to the present value using the bond's yield to maturity. The present value is depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_price).
+
+> **Duration**
+
+The bond duration is a measure of the bond's sensitivity to changes in interest rates. It is the weighted average of the bond's cash flows, where the weights are the present value of each cash flow divided by the bond's price. It is possible to calculate the following durations:
+
+- **Macaulay's Duration:** The weighted average time to receive the bond's cash flows.
+- **Modified Duration:** The Macaulay's duration divided by 1 plus the yield to maturity.
+- **Effective Duration:** The percentage change in the bond price for a 1% change in the yield to maturity.
+- **Dollar Duration:** The modified duration multiplied by the bond price.
+
+The duration values are depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_bond_duration).
+
+> **Yield to Maturity**
+
+The Yield to Maturity (YTM) is the total return anticipated on a bond if it is held until it matures. It is the internal rate of return of an investment in a bond if the investor holds the bond until maturity and receives all payments as scheduled. The yield to maturity is depicted over a variety of coupon rates and years of maturities. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_yield_to_maturity).
+
+</details>
+
+<details>
+    <summary><b>Derivative Valuations</b></summary>
+The Derivative Valuations section contains a variety of models that can be used to value derivative instruments such as Swaptions. These models include the Black Model and the Bachelier Model.
+
+All derivative valuations can be called by using `get_` to get a single valuation. E.g. `get_derivative_price`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_derivative_price(model_type="black")
+```
+
+> **Black Model**
+
+The Black Model is a mathematical model used to calculate the price of European-style options. It is based on the Black-Scholes model but is used for interest rate options. The Black Model is used to value interest rate options, such as caps, floors, and swaptions. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_derivative_price).
+
+> **Bachelier Model**
+
+The Bachelier Model is a mathematical model used to calculate the price of European-style options. It is based on the normal distribution and is used for interest rate options as opposed to the Black model which uses a log-normal distribution. The Bachelier Model is used to value interest rate options, such as caps, floors, and swaptions. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_derivative_price).
+
+</details>
+
+<details>
+    <summary><b>Central Banks</b></summary>
+
+The central bank metrics revolve around the interest rates of the European Central Bank (ECB) and the Federal Reserve (FED). This includes the main refinancing operations, marginal lending facility, deposit facility, effective federal funds rate, overnight bank funding rate, tri-party general collateral rate, broad general collateral rate and secured overnight financing rate.
+
+All central bank metrics can be called by using `get_` to get a single metric. E.g. `get_european_central_bank_rates` or `get_federal_reserve_rates`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_european_central_bank_rates()
+```
+
+> **Main Refinancing Operations**
+
+The main refinancing operations (MRO) rate is the interest rate banks pay when they borrow money from the ECB for one week. When they do this, they have to provide collateral to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+
+> **Marginal Lending Facility**
+
+The marginal lending facility rate is the interest rate banks pay when they borrow from the ECB overnight. When they do this, they have to provide collateral, for example securities, to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+> **Deposit Facility**
+
+The deposit facility rate is one of the three interest rates the ECB sets every six weeks as part of its monetary policy. The rate defines the interest banks receive for depositing money with the central bank overnight. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_european_central_bank_rates).
+
+> **Euribor Rates**
+
+The Euro Interbank Offered Rate (Euribor) is a daily reference rate based on the averaged interest rates at which Eurozone banks offer to lend unsecured funds to other banks in the euro wholesale money market. It is widely used as the base rate for a variety of financial products, including mortgages, savings accounts, and derivatives. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_euribor_rates).
+
+> **Effective Federal Funds Rate**
+
+The effective federal funds rate (EFFR) is calculated as a volume-weighted median of overnight federal funds transactions reported in the FR 2420 Report of Selected Money Market Rates. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Overnight Bank Funding Rate**
+
+The overnight bank funding rate (OBFR) is calculated as a volume-weighted median of overnight federal funds transactions, Eurodollar transactions, and the domestic deposits reported as “Selected Deposits” in the FR 2420 Report. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Tri-Party General Collateral Rate**
+
+The TGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Broad General Collateral Rate**
+
+The BGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+> **Secured Overnight Financing Rate (SOFR)**
+
+The SOFR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data and data on bilateral Treasury repo transactions cleared through FICC’s DVP service, which are obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_federal_reserve_rates).
+
+</details>
+
+<details>
+    <summary><b>Government Bonds</b></summary>
+
+It is possible to view both short-term (3-month) and long-term (10-year) interest rates for each of the available countries. These rates relate to the interest rates at which countries issue government bonds and are used as a benchmark for other interest rates in the economy. For example, the German government bond yield is an overall indicator of the European economy.
+
+These interest rates can be obtained with `get_government_bond_yield`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_government_bond_yield()
+```
+
+> **Long Term Interest Rates (10 year)**
+
+Long-term interest rates refer to government bonds maturing in ten years. Rates are mainly determined by the price charged by the lender, the risk from the borrower and the fall in the capital value. Long-term interest rates are generally averages of daily rates, measured as a percentage. These interest rates are implied by the prices at which the government bonds are traded on financial markets, not the interest rates at which the loans were issued.
+
+In all cases, they refer to bonds whose capital repayment is guaranteed by governments. Long-term interest rates are one of the determinants of business investment. Low long term interest rates encourage investment in new equipment and high interest rates discourage it. Investment is, in turn, a major source of economic growth. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_government_bond_yield).
+
+> **Short Term Interest Rates (3 month)**
+
+Short-term interest rates are the rates at which short-term borrowings are effected between financial institutions or the rate at which short-term government paper is issued or traded in the market. Short-term interest rates are generally averages of daily rates, measured as a percentage.
+
+Short-term interest rates are based on three-month money market rates where available. Typical standardised names are “money market rate” and “treasury bill rate”. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_government_bond_yield).
+
+</details>
+
+<details>
+    <summary><b>Corporate Bonds</b></summary>
+
+The Corporate Bonds section features the widely used ICE BofA benchmarks which include option-adjusted spreads, effective yields and the total returns. It is possible to view both the indices of the ratings (AAA, AA, A, BBB, BB, B and CCC) and the maturities (1-3 years, 3-5 years, 5-7 years, 7-10 years, 10-15 years, 15-30 years and 30+ years).
+
+All corporate bond metrics can be called by using `get_` to get a single metric. E.g. `get_ice_bofa_option_adjusted_spread` or `get_ice_bofa_yield_to_worst`. As an example:
+
+```python
+from financetoolkit import FixedIncome
+
+fixedincome = FixedIncome()
+
+fixedincome.get_ice_bofa_option_adjusted_spread()
+```
+
+> **Option-Adjusted Spread (OAS)**
+
+The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the uncertainty of the cash flows. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_option_adjusted_spread).
+
+> **Effective Yield**
+
+The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price. The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_effective_yield).
+
+> **Total Return**
+
+The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period. Total return includes interest, capital gains, dividends and distributions realized over a given period of time. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_total_return).
+
+> **Yield to Worst**
+
+Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/fixedincome#get_ice_bofa_yield_to_worst).
+
+</details>
+
 ## Key Economic Indicators
 
 The Economics Module contains a variety of Key Economic Indicators that help in understanding the health and performance of more than 60 different countries. This module can be called directly via the Toolkit but also separately if desired through `from financetoolkit import Economics`. **Find the Notebook [here](https://www.jeroenbouma.com/projects/financetoolkit/economics-module) and the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics) which includes an explanation about each indicator, the parameters and an example.**
 
 <details>
     <summary><b>Economy 💵</b></summary>
 
@@ -2679,99 +2915,14 @@
 > **Exchange Rates**
 
 Exchange rates are defined as the price of one country’s’ currency in relation to another country’s currency. This indicator is measured in terms of national currency per US dollar. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_exchange_rates).
 
 </details>
 
 <details>
-    <summary><b>Central Banks 🏦</b></summary>
-
-The central bank metrics revolve around the interest rates of the European Central Bank (ECB) and the Federal Reserve (FED). This includes the main refinancing operations, marginal lending facility, deposit facility, effective federal funds rate, overnight bank funding rate, tri-party general collateral rate, broad general collateral rate and secured overnight financing rate.
-
-All central bank metrics can be called by using `get_` to get a single metric. E.g. `get_european_central_bank_rates` or `get_federal_reserve_rates`. As an example:
-
-```python
-from financetoolkit import Toolkit
-
-toolkit = Toolkit(["AAPL", "TSLA"], api_key="FINANCIAL_MODELING_PREP_KEY")
-
-# Get Central Bank Results
-toolkit.economics.get_european_central_bank_rates()
-```
-
-> **Main Refinancing Operations**
-
-The main refinancing operations (MRO) rate is the interest rate banks pay when they borrow money from the ECB for one week. When they do this, they have to provide collateral to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_european_central_bank_rates).
-
-
-> **Marginal Lending Facility**
-
-The marginal lending facility rate is the interest rate banks pay when they borrow from the ECB overnight. When they do this, they have to provide collateral, for example securities, to guarantee that the money will be paid back. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_european_central_bank_rates).
-
-> **Deposit Facility**
-
-The deposit facility rate is one of the three interest rates the ECB sets every six weeks as part of its monetary policy. The rate defines the interest banks receive for depositing money with the central bank overnight. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_european_central_bank_rates).
-
-> **Effective Federal Funds Rate**
-
-The effective federal funds rate (EFFR) is calculated as a volume-weighted median of overnight federal funds transactions reported in the FR 2420 Report of Selected Money Market Rates. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-> **Overnight Bank Funding Rate**
-
-The overnight bank funding rate (OBFR) is calculated as a volume-weighted median of overnight federal funds transactions, Eurodollar transactions, and the domestic deposits reported as “Selected Deposits” in the FR 2420 Report. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-> **Tri-Party General Collateral Rate**
-
-The TGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-> **Broad General Collateral Rate**
-
-The BGCR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-> **Secured Overnight Financing Rate**
-
-The SOFR is calculated as a volume-weighted median of transaction-level tri-party repo data collected from the Bank of New York Mellon as well as GCF Repo transaction data and data on bilateral Treasury repo transactions cleared through FICC’s DVP service, which are obtained from the U.S. Department of the Treasury’s Office of Financial Research (OFR). Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_federal_reserve_rates).
-
-</details>
-
-<details>
-    <summary><b>Fixed Income 📃 </b></summary>
-
-The fixed income metrics revolve around option-adjusted spreads, effective yields and total returns of corporate bonds based on the ICE BofA US Corporate Indices. It is possible to view both the indices of the ratings (AAA, AA, A, BBB, BB, B and CCC) and the maturities (1-3 years, 3-5 years, 5-7 years, 7-10 years, 10-15 years, 15-30 years and 30+ years).
-
-All fixed income metrics can be called by using `get_` to get a single metric. E.g. `get_option_adjusted_spread` or `get_yield_to_worst`. As an example:
-
-```python
-from financetoolkit import Toolkit
-
-toolkit = Toolkit(["AAPL", "TSLA"], api_key="FINANCIAL_MODELING_PREP_KEY")
-
-# Get Fixed Income Results
-toolkit.economics.get_option_adjusted_spread()
-```
-
-> Option-Adjusted Spread (OAS)
-
-The Option-Adjusted Spread (OAS) is the spread relative to a risk-free interest rate, usually measured in basis points (bp), that equates the theoretical present value of a series of uncertain cash flows to the market price of a fixed-income investment. The spread is added to the risk-free rate to compensate for the uncertainty of the cash flows. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_option_adjusted_spread).
-
-> Effective Yield
-
-The Effective Yield is the yield of a bond, calculated by dividing the bond's coupon payments by its market price. The effective yield is not the same as the stated yield, which is the yield on the bond's coupon payments divided by the bond's principal value. The effective yield is a more accurate measure of a bond's return, as it takes into account the fact that the investor will not hold the bond to maturity and will likely sell it before it matures. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_effective_yield).
-
-> Total Return
-
-The total return is the actual rate of return of an investment or a pool of investments over a given evaluation period. Total return includes interest, capital gains, dividends and distributions realized over a given period of time. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_total_return).
-
-> Yield to Worst
-
-Yield to worst is the lowest potential yield that a bond can generate without the issuer defaulting. The standard US convention for this series is to use semi-annual coupon payments, whereas the standard in the foreign markets is to use coupon payments with frequencies of annual, semi-annual, quarterly, and monthly. Find the documentation [here](https://www.jeroenbouma.com/projects/financetoolkit/docs/economics#get_yield_to_worst).
-
-</details>
-
-<details>
     <summary><b>Environment 💚</b></summary>
 
 The environment metrics revolve around renewable energy, environmental tax, greenhouse gas emissions, crude oil production and crude oil prices of countries. This includes the renewable energy as a percentage of total energy, environmental tax as a percentage of GDP, greenhouse gas emissions, crude oil production and crude oil prices.
 
 All environment metrics can be called by using `get_` to get a single metric. E.g. `get_renewable_energy` or `get_crude_oil_prices`. As an example:
 
 ```python
```

