# Comparing `tmp/hg_oap-0.1.0.tar.gz` & `tmp/hg_oap-0.1.1.tar.gz`

## Comparing `hg_oap-0.1.0.tar` & `hg_oap-0.1.1.tar`

### file list

```diff
@@ -1,60 +1,68 @@
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 hg_oap-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hg_oap-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hg_oap-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hg_oap-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 hg_oap-0.1.0/.github/workflows/deploy-on-tag.yml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hg_oap-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/assets/__init__.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/assets/asset.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/assets/commodities.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/assets/currency.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/dates/__init__.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/dates/calendar.py
--rw-r--r--   0        0        0    23596 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/dates/dgen.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/dates/tenor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/instruments/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/instruments/cash.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/instruments/commodity.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/instruments/forward.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/instruments/future.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/instruments/instrument.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/instruments/physical.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/orders/__init__.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/orders/order.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/orders/order_type.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/portfolio/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/portfolio/portfolio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/position/__init__.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/position/position.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/pricing/__init__.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/pricing/price.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/quanity/__init__.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/quanity/quantity.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/units/__init__.py
--rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/units/dimension.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/units/quantity.py
--rw-r--r--   0        0        0    12895 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/units/unit.py
--rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/units/unit_system.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/utils/__init__.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/utils/exprclass.py
--rw-r--r--   0        0        0    25267 2020-02-02 00:00:00.000000 hg_oap-0.1.0/src/hg_oap/utils/magic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/quantity/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/__init__.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/test_calendar.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/test_dataclassex.py
--rw-r--r--   0        0        0     9290 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/test_dgen.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/test_dimension.py
--rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/test_magic.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/test_quantity.py
--rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/test_quantity_ts.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 hg_oap-0.1.0/tests/unit/hg_oap/utils/test_units.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hg_oap-0.1.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hg_oap-0.1.0/LICENSE
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hg_oap-0.1.0/README.md
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 hg_oap-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hg_oap-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.coveragerc
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 hg_oap-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/workflows/deploy-on-tag.yml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/assets/__init__.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/assets/asset.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/assets/commodities.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/assets/currency.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/dates/__init__.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/dates/calendar.py
+-rw-r--r--   0        0        0    23590 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/dates/dgen.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/dates/tenor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/cash.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/commodity.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/forward.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/future.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/fx.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/instrument.py
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/instruments/physical.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/orders/__init__.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/orders/order.py
+-rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/orders/order_service.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/orders/order_type.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/portfolio/__init__.py
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/portfolio/portfolio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/position/__init__.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/position/position.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/pricing/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/pricing/price.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/quanity/__init__.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/U.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/__init__.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/dimension.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/quantity.py
+-rw-r--r--   0        0        0    13230 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/unit.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/units/unit_system.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/utils/__init__.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/utils/exprclass.py
+-rw-r--r--   0        0        0    25216 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/utils/op.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 hg_oap-0.1.1/src/hg_oap/utils/op_delarations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/example/__init__.py
+-rw-r--r--   0        0        0    10861 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/example/test_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/orders/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/orders/test_order_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/quantity/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/__init__.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_calendar.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dataclassex.py
+-rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dgen.py
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dimension.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_magic.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_quantity.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_quantity_ts.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 hg_oap-0.1.1/tests/unit/hg_oap/utils/test_units.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 hg_oap-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 hg_oap-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 hg_oap-0.1.1/README.md
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 hg_oap-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 hg_oap-0.1.1/PKG-INFO
```

### Comparing `hg_oap-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `hg_oap-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `hg_oap-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/.github/workflows/deploy-on-tag.yml` & `hg_oap-0.1.1/.github/workflows/deploy-on-tag.yml`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/src/hg_oap/assets/commodities.py` & `hg_oap-0.1.1/src/hg_oap/assets/commodities.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,27 +15,29 @@
 class BaseMetal(Commodity):
     """
     Metals such as Copper.
     """
 
 
 class BaseMetals(Enum):
-    MAL = BaseMetal("MAL", "Aluminium")
-    MCU = BaseMetal("MCU", "Copper")
-    MNI = BaseMetal("MNI", "Nickel")
-    MPB = BaseMetal("MPB", "Lead")
-    MSN = BaseMetal("MSN", "Tin")
-    MZN = BaseMetal("MZN", "Zinc")
+    ...
+    # MAL = BaseMetal("MAL", "Aluminium")
+    # MCU = BaseMetal("MCU", "Copper")
+    # MNI = BaseMetal("MNI", "Nickel")
+    # MPB = BaseMetal("MPB", "Lead")
+    # MSN = BaseMetal("MSN", "Tin")
+    # MZN = BaseMetal("MZN", "Zinc")
 
 
 @dataclass(frozen=True)
 class PreciousMetal(Commodity):
     """
     Gold, Silver, Platinum, Palladium.
     """
 
 
 class PreciousMetals(Enum):
-    XAU = PreciousMetal("XAU", "Gold")
-    XAG = PreciousMetal("XAG", "Silver")
-    XPD = PreciousMetal("XPD", "Palladium")
-    XPT = PreciousMetal("XPT", "Platinum")
+    ...
+    # XAU = PreciousMetal("XAU", "Gold")
+    # XAG = PreciousMetal("XAG", "Silver")
+    # XPD = PreciousMetal("XPD", "Palladium")
+    # XPT = PreciousMetal("XPT", "Platinum")
```

### Comparing `hg_oap-0.1.0/src/hg_oap/assets/currency.py` & `hg_oap-0.1.1/src/hg_oap/assets/currency.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,31 @@
 from dataclasses import dataclass
+from decimal import Decimal
 from enum import Enum
+from typing import Optional
 
-from hg_oap.instruments.instrument import Instrument
 from hg_oap.assets.asset import FinancialAsset
+from hg_oap.units import PrimaryUnit
 
 
 @dataclass(frozen=True)
 class Currency(FinancialAsset):
     """
     The medium of exchange for goods and services, you may have used this. For example USD, EUR, GBP, etc.
     These represent the most commonly used currencies in the USA, Europe or the United Kingdom.
     """
-    is_minor_currency: bool = False  # For example US cents rather than dollars
+    minor_currency_ratio: Optional[int] = None  # For example US cents rather than dollars
+
+    def __post_init__(self):
+        from hg_oap.units import U
+        setattr(U, f"currency.{self.symbol}", currency_dim := getattr(U.money, self.symbol))  # Add the currency to the unit system as a qualified dimansion
+        setattr(U, self.symbol, unit := PrimaryUnit(dimension=currency_dim))
+        if self.minor_currency_ratio is not None:
+            minor_symbol = f"{self.symbol[:-1]}X"
+            setattr(U, minor_symbol, Decimal(1)/Decimal(self.minor_currency_ratio) * unit)
 
 
 @dataclass(frozen=True)
 class MinorCurrency(Currency):
     """
     A minor currency is the fractional unit, for example US cents, typically this is a 1:100 ratio, the ratio
     is stored as ratio.
@@ -25,12 +35,10 @@
 
     def to_major_currency(self, value: float) -> float:
         return value * self.ratio
 
 
 class Currencies(Enum):
     """The collection of known currencies"""
-    EUR = Currency("EUR")
-    GBP = (gbp_ := Currency("GBP"))
-    GBX = MinorCurrency("GBX", major_currency=gbp_)
-    USD = (usd_ := Currency("USD"))
-    USX = MinorCurrency("USX", major_currency=usd_)
+    EUR = Currency("EUR", minor_currency_ratio=100)
+    GBP = Currency("GBP", minor_currency_ratio=100)
+    USD = Currency("USD", minor_currency_ratio=100)
```

### Comparing `hg_oap-0.1.0/src/hg_oap/dates/calendar.py` & `hg_oap-0.1.1/src/hg_oap/dates/calendar.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/src/hg_oap/dates/dgen.py` & `hg_oap-0.1.1/src/hg_oap/dates/dgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date, timedelta
 from itertools import islice
 from typing import cast
 
 from hg_oap.dates.calendar import Calendar
-from hg_oap.utils.magic import Item, const, Op
+from hg_oap.utils.op import Item, Op, lazy
 from hg_oap.dates.tenor import Tenor
 
 __all__ = ('is_dgen', 'make_date', 'make_dgen', 'years', 'months', 'weeks', 'weekdays', 'weekends', 'days',
            'business_days', 'roll_fwd', 'roll_bwd')
 
 
 def is_dgen(obj):
@@ -138,15 +138,15 @@
             else:
                 raise ValueError(f"{type(self)} date generator does not support negative indices")
         if isinstance(item, slice):
             if is_negative_slice(item):
                 raise ValueError(f"{type(self)} date generator does not support negative indices")
             return SliceDGen(self, item)
         if isinstance(item, Op):
-            return const(self)[item]
+            return lazy(self)[item]
 
     def over(self, calendar: Calendar):
         return WithCalendarDGen(self, calendar)
 
 
 class ConstDGen(DGen):
     def __init__(self, date):
@@ -602,15 +602,15 @@
 
     def __getitem__(self, item):
         if isinstance(item, int):
             return SubSequenceDGen(self.main_sequence, self.sub_sequence, slice(item, item + 1))
         if isinstance(item, slice):
             return SubSequenceDGen(self.main_sequence, self.sub_sequence, item)
         if isinstance(item, Op):
-            return const(self)[item]
+            return lazy(self)[item]
 
 class DaysOfMonthDGen(DGen):
     def __init__(self, months, days):
         self.months = months
         self.days = days
 
     def __invoke__(self, start: date = date.min, end: date = date.max, after: date = date.min, before: date = date.max,
```

### Comparing `hg_oap-0.1.0/src/hg_oap/dates/tenor.py` & `hg_oap-0.1.1/src/hg_oap/dates/tenor.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/src/hg_oap/instruments/commodity.py` & `hg_oap-0.1.1/src/hg_oap/instruments/commodity.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/src/hg_oap/portfolio/portfolio.py` & `hg_oap-0.1.1/src/hg_oap/portfolio/portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     books: TSS[BOOK_ID]
     portfolios: TSS[PORTFOLIO_ID]
 
 
 @subscription_service
 def get_portfolio(portfolio_id: TS[PORTFOLIO_ID]) -> TSB[Portfolio]:
-    """Returns the porfolio TSB of a given portfolio_id"""
+    """Returns the portfolio TSB of a given portfolio_id"""
 
 
 @subscription_service
 def rolled_positions(portfolio_id: TS[PORTFOLIO_ID]) -> TSD[INSTRUMENT_ID, TSB[PositionQuantity]]:
     """
     Return the positions associated to this portfolio. This will recursively traverse the portfolio collecting up the
     books and then reducing the positions of all the books.
```

### Comparing `hg_oap-0.1.0/src/hg_oap/pricing/price.py` & `hg_oap-0.1.1/src/hg_oap/pricing/price.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,55 @@
+from dataclasses import dataclass
 from typing import Generic
 
-from hgraph import TimeSeriesSchema, TS, Array, SIZE, TSB
+from hgraph import TimeSeriesSchema, TS, Array, SIZE, TSB, CompoundScalar
 
 from hg_oap.assets.currency import Currency
 from hg_oap.units.unit import UNIT
 
 
-class Price(TimeSeriesSchema):
+@dataclass
+class Price(CompoundScalar):
     """
     A bundle schema representing the price as a float and the associated currency asset that the price is representing.
     """
-    price: TS[float]
-    currency: TS[Currency]
+    price: float
+    currency: Currency
+
+    def __add__(self, other):
+        """This class should be same as quantity, but for now..."""
+        if other.currency == self.currency:
+            return Price(price=self.price + other.price, currency=self.currency)
+        else:
+            raise ValueError(f"Cannot add {self} to {other} of {self.currency}")
 
 
+@dataclass
 class L1Price(TimeSeriesSchema):
     """
     The l1 price represents the mid and spread or bid and ask price. Along with the currency the prices represent.
     """
     mid: TS[float]
     spread: TS[float]
     currency: TS[Currency]
 
 
+@dataclass
 class PriceProfile(TimeSeriesSchema, Generic[SIZE]):
     """
     The price offsets represent the relative price from whichever side the profile represents, the values of prices
     must be monotonically increasing and should not include duplicates (though it may temporarily do so).
     The value in the prices are relative to the TOB of the side the price represents.
     The quantities are always positive.
     """
     price_offsets: TS[Array[float, SIZE]]
     quantities: TS[Array[float, SIZE]]
 
 
+@dataclass
 class L2Price(L1Price, Generic[SIZE, UNIT]):
     """
     The set of price offsets and quantities on top of the L1 price.
     """
     bid_profile: TSB[PriceProfile[SIZE]]
     ask_profile: TSB[PriceProfile[SIZE]]
     qty_unit: TS[UNIT]
```

### Comparing `hg_oap-0.1.0/src/hg_oap/units/dimension.py` & `hg_oap-0.1.1/src/hg_oap/units/dimension.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import Tuple
 
 from hg_oap.units.unit_system import UnitSystem
+from hg_oap.utils.exprclass import ExprClass
 
+__all__ = ("Dimension", "Dimensionless", "PrimaryDimension", "DerivedDimension", "QualifiedDimension")
 
-@dataclass(frozen=True, kw_only=True)
-class Dimension:
+
+@dataclass(frozen=True, kw_only=True, init=False)
+class Dimension(ExprClass):
     name: str = None
 
     def __new__(cls, name=None):
         assert cls is not Dimension, 'Base Dimension types is not instantiable.'
 
         if name:
             if d := UnitSystem.instance().__dimensions__.get(name):
@@ -19,14 +22,45 @@
         n = super().__new__(cls)
         if name:
             object.__setattr__(n, 'name', name)
             UnitSystem.instance().__dimensions__[name] = n
 
         return n
 
+    def __pow__(self, power, modulo=None):
+        if power == 1:
+            return self
+        else:
+            return DerivedDimension(components=((self, power),))
+
+    def __mul__(self, other: "Dimension"):
+        if isinstance(other, Dimension):
+            components = defaultdict(int, other._to_components())
+        else:
+            raise ValueError(f"cannot multiply {self} and {other}")
+
+        for d, p in self._to_components():
+            components[d] += p
+
+        return DerivedDimension(components=tuple(components.items()))
+
+    def __truediv__(self, other: "Dimension"):
+        if isinstance(other, Dimension):
+            components = defaultdict(int, other._to_components(-1))
+        else:
+            raise ValueError(f"cannot multiply {self} and {other}")
+
+        for d, p in self._to_components():
+            components[d] += p
+
+        return DerivedDimension(components=tuple(components.items()))
+
+    def __getattr__(self, item):
+        return QualifiedDimension(base=self, qualifier=item)
+
     def __str__(self):
         return self.name
 
     def __hash__(self):
         return id(self)
 
     def _to_components(self, power=1):
@@ -62,48 +96,25 @@
 
 
 @dataclass(frozen=True)
 class PrimaryDimension(Dimension):
     def __hash__(self):
         return id(self)
 
-    def __pow__(self, power, modulo=None):
-        return DerivedDimension(components=((self, power),))
-
-    def __mul__(self, other: Dimension):
-        if isinstance(other, Dimension):
-            components = defaultdict(int, other._to_components())
-        else:
-            raise ValueError(f"cannot multiply {self} and {other}")
-
-        components[self] += 1
-        return DerivedDimension(components=tuple(components.items()))
 
-    def __truediv__(self, other):
-        if isinstance(other, Dimension):
-            components = defaultdict(int, other._to_components(-1))
-        else:
-            raise ValueError(f"cannot divide {self} and {other}")
-
-        components[self] += 1
-        return DerivedDimension(components=tuple(components.items()))
-
-
-@dataclass(frozen=True)
+@dataclass(frozen=True, kw_only=True, init=False)
 class DerivedDimension(Dimension):
+    name: str = lambda self: self._build_name()
     components: Tuple[Tuple[PrimaryDimension, int], ...]
 
     def __new__(cls, components, name=None):
         reduced_components = defaultdict(int)
         for d, p in components:
-            if type(d) is PrimaryDimension:
-                reduced_components[d] += p
-            elif type(d) is DerivedDimension:
-                for d1, p1 in d.components:
-                    reduced_components[d1] += p1 * p
+            for d1, p1 in d._to_components(p):
+                reduced_components[d1] += p1
 
         reduced_components = tuple((d, p) for d, p in reduced_components.items() if p != 0)
 
         if len(reduced_components) == 0:
             return Dimensionless()
 
         if len(reduced_components) == 1 and reduced_components[0][1] == 1:
@@ -113,51 +124,50 @@
 
         if d := UnitSystem.instance().__derived_dimensions__.get(reduced_components):
             return d
 
         n = super().__new__(cls)
         object.__setattr__(n, 'components', reduced_components)
         if name:
-            object.__setattr__(n, 'name', name)
+            type(n).name.__override__(n, name)
         UnitSystem.instance().__derived_dimensions__[reduced_components] = n
         return n
 
-    def __post_init__(self):
-        if not self.name:
-            up = '*'.join(f"{d}**{p}" if p != 1 else str(d) for d, p in self.components if p > 0) or '1'
-            dn = ('*'.join(f"{d}**{abs(p)}" if p != -1 else str(d) for d, p in self.components if p < 0))
-            dn = ('/' + dn) if dn else ''
-            object.__setattr__(self, 'name', up + dn)
+    def _build_name(self):
+        up = '*'.join(f"{d}**{p}" if p != 1 else str(d) for d, p in self.components if p > 0) or '1'
+        dn = ('*'.join(f"{d}**{abs(p)}" if p != -1 else str(d) for d, p in self.components if p < 0))
+        dn = ('/' + dn) if dn else ''
+        return f"{up}{dn}"
 
     def __hash__(self):
         return id(self)
 
-    def __pow__(self, power, modulo=None):
-        return DerivedDimension(components=tuple((d, p * power) for d, p in self.components))
-
-    def __mul__(self, other: Dimension):
-        if isinstance(other, Dimension):
-            components = defaultdict(int, other._to_components())
+    def _to_components(self, power=1):
+        if power == 1:
+            return self.components
         else:
-            raise ValueError(f"cannot multiply {self} and {other}")
+            return tuple((c, p*power) for c, p in self.components)
 
-        for d, p in self.components:
-            components[d] += p
 
-        return DerivedDimension(components=tuple(components.items()))
+@dataclass(frozen=True)
+class QualifiedDimension(Dimension):
+    base: Dimension
+    qualifier: object
+
+    def __new__(cls, base: Dimension, qualifier: object):
+        assert qualifier is not None
+        qualified_name = f"{base.name}.{qualifier}"
 
-    def __truediv__(self, other):
-        if isinstance(other, Dimension):
-            components = defaultdict(int, other._to_components(-1))
-        else:
-            raise ValueError(f"cannot multiply {self} and {other}")
+        if d := UnitSystem.instance().__dimensions__.get(qualified_name):
+            return d
 
-        for d, p in self.components:
-            components[d] += p
+        n = super().__new__(cls, name=qualified_name)
+        object.__setattr__(n, 'name', qualified_name)
+        object.__setattr__(n, 'base', base)
+        object.__setattr__(n, 'qualifier', qualifier)
 
-        return DerivedDimension(components=tuple(components.items()))
+        UnitSystem.instance().__dimensions__[qualified_name] = n
 
-    def _to_components(self, power=1):
-        if power == 1:
-            return self.components
-        else:
-            return tuple((c, p*power) for c, p in self.components)
+        return n
+
+    def __hash__(self):
+        return id(self)
```

### Comparing `hg_oap-0.1.0/src/hg_oap/units/quantity.py` & `hg_oap-0.1.1/src/hg_oap/units/quantity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from dataclasses import dataclass
 from numbers import Number
 from typing import Generic
 
 from hg_oap.units.unit import Unit, NUMBER
 from hgraph import CompoundScalar
 
+__all__ = ("Quantity",)
+
 
 @dataclass(frozen=True)
 class Quantity(CompoundScalar, Generic[NUMBER]):
     qty: NUMBER
     unit: Unit
 
     def __str__(self):
@@ -52,16 +54,18 @@
             return Quantity[type(self.qty)](self.qty / other.qty, self.unit / other.unit)
         elif isinstance(other, type(self.qty)):
             return Quantity[type(self.qty)](self.qty / other, self.unit)
 
         return NotImplemented
 
     def __rtruediv__(self, other):
-        if isinstance(other, type(self.qty)) and self.qty != 0:
+        if isinstance(other, type(self.qty)):
             return Quantity[type(self.qty)](other / self.qty, self.unit ** -1)
+        else:
+            return Quantity[type(self.qty)](type(self.qty)(other) / self.qty, self.unit ** -1)
 
         return NotImplemented
 
     def __pow__(self, other):
         if isinstance(other, Number):
             return Quantity[type(self.qty)](self.qty ** other, self.unit ** other)
```

### Comparing `hg_oap-0.1.0/src/hg_oap/units/unit.py` & `hg_oap-0.1.1/src/hg_oap/units/unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 from decimal import Decimal
 from functools import reduce
 from typing import Tuple, ForwardRef, TypeVar, ClassVar
 
 from hg_oap.units.dimension import Dimension
 from hg_oap.utils.exprclass import ExprClass
 from hg_oap.units.unit_system import UnitSystem
+from hgraph import CompoundScalar
 
 NUMBER = TypeVar('NUMBER', int, float, Decimal)
 
+__all__ = ("Unit", "PrimaryUnit", "DerivedUnit", "OffsetDerivedUnit", "DiffDerivedUnit", "ComplexUnit", "UNIT")
 
-@dataclass(frozen=True, kw_only=True, init=False)
-class Unit(ExprClass):
+@dataclass(frozen=True, kw_only=True, init=False, repr=False)
+class Unit(CompoundScalar, ExprClass):
     name: str = None
     dimension: Dimension
     prefixes: Tuple[str, ...] | None = field(default=None, hash=False)
 
     def __str__(self):
         return self.name
 
+    def __repr__(self):
+        return self.name
+
     def __hash__(self):
         return id(self)  # units are singletons within a UnitSystem by construction so this is safe
 
     def __rmul__(self, value):
         if isinstance(value, (int, float, Decimal)):
             from hg_oap.units.quantity import Quantity
             return Quantity(value, self)
@@ -79,15 +84,15 @@
 
     _is_multiplicative: ClassVar[bool] = True
 
 
 UNIT = TypeVar("UNIT", bound=Unit)
 
 
-@dataclass(frozen=True, kw_only=True, init=False)
+@dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class PrimaryUnit(Unit):
     ratio: Decimal = Decimal(1)
 
     def __new__(cls, name=None, dimension: Dimension = None, prefixes=None):
         if d := UnitSystem.instance().__primary_units__.get(dimension):
             assert d.dimension is dimension
             return d
@@ -98,14 +103,18 @@
             object.__setattr__(n, 'name', name)
         if prefixes:
             object.__setattr__(n, 'prefixes', prefixes)
 
         UnitSystem.instance().__primary_units__[dimension] = n
         return n
 
+    @property
+    def primary_unit(self):
+        return self
+
     def __pow__(self, power, modulo=None):
         return ComplexUnit(components=((self, power),))
 
     def __mul__(self, other):
         if isinstance(other, (PrimaryUnit, DerivedUnit, ComplexUnit)):
             components = defaultdict(int, other._to_components())
         else:
@@ -128,15 +137,15 @@
             return value / type(value)(to.ratio) - type(value)(to.offset)
         elif isinstance(to, Unit):
             return value / type(value)(to.ratio)
 
         assert False, f'conversion from {self} to {to} is not supported'
 
 
-@dataclass(frozen=True, kw_only=True, init=False)
+@dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class DerivedUnit(Unit):
     primary_unit: Unit
     ratio: Decimal
     dimension: Dimension = lambda s: s.primary_unit.dimension
     name: str = lambda s: f"{s.ratio}*{s.primary_unit.name}"
 
     def __new__(cls, primary_unit: Unit | ForwardRef("Quantity"), ratio: Decimal = Decimal(1), name=None, prefixes=None):
@@ -189,15 +198,15 @@
         primary_value = value * type(value)(self.ratio)
         if to is not self.primary_unit:
             return self.primary_unit._do_convert(primary_value, to)
         else:
             return primary_value
 
 
-@dataclass(frozen=True, kw_only=True, init=False)
+@dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class OffsetDerivedUnit(DerivedUnit):
     offset: Decimal
     diff: Unit = field(default=lambda s: DiffDerivedUnit(offset_unit=s), hash=False)
 
     _is_multiplicative: ClassVar[bool] = False
 
     def __new__(cls, primary_unit: Unit | ForwardRef("Quantity"), ratio: Decimal = Decimal(1), offset: Decimal = Decimal(0), name=None, prefixes=None):
@@ -242,15 +251,15 @@
         primary_value = (value + type(value)(self.offset)) * type(value)(self.ratio)
         if to is not self.primary_unit:
             return self.primary_unit._do_convert(primary_value, to)
         else:
             return primary_value
 
 
-@dataclass(frozen=True, kw_only=True, init=False)
+@dataclass(frozen=True, kw_only=True, init=False, repr=False)
 class DiffDerivedUnit(DerivedUnit):
     offset_unit: Unit = None
     primary_unit: Unit = lambda s: s.offset_unit.primary_unit
     ratio: Decimal = lambda s: s.offset_unit.ratio
     name: str = lambda s: f"{s.offset_unit.name}_diff"
 
     _is_multiplicative: ClassVar[bool] = True
```

### Comparing `hg_oap-0.1.0/src/hg_oap/units/unit_system.py` & `hg_oap-0.1.1/src/hg_oap/units/unit_system.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from functools import reduce
 from itertools import chain, combinations
 from typing import ClassVar, Tuple, Iterable
 
 from hg_oap.utils.exprclass import CallableDescriptor
 
 
+__all__ = ("UnitSystem", "UnitConversionContext")
+
 @dataclass
 class UnitSystem:
     __instance__: ClassVar['UnitSystem'] = None
 
     __dimensions__: dict[str, "Dimension"] = field(default_factory=dict)
     __derived_dimensions__: dict[tuple[tuple["Dimension", int], ...], "Dimension"] = field(default_factory=dict)
 
@@ -49,15 +51,15 @@
             if isinstance(value.unit, (PrimaryUnit, DerivedUnit)):
                 value = DerivedUnit(value)
             elif isinstance(value.unit, ComplexUnit):
                 value = ComplexUnit(value)
 
         if value.name != key:
             if (desc := getattr(type(value), 'name', None)) and isinstance(desc, CallableDescriptor):
-                desc.__override_set__(value, key)
+                desc.__override__(value, key)
             else:
                 object.__setattr__(value, 'name', key)
 
             from hg_oap.units.dimension import PrimaryDimension
             if isinstance(value, PrimaryDimension):
                 self.__dimensions__[key] = value
 
@@ -83,25 +85,29 @@
             if factor := context.conversion_factor(dimension):
                 return factor
 
         return None
 
 
 class UnitConversionContext:
-    def __init__(self, conversion_factors: dict["Dimension", "Quantity[Decimal]"]):
-        self.conversion_factors = conversion_factors
+    def __init__(self, conversion_factors: tuple["Quantity[Decimal]"] = ()):
+        self.unit_conversion_factors = conversion_factors
 
     def __enter__(self):
         UnitSystem.instance().enter_context(self)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         UnitSystem.instance().exit_context(self)
 
     def conversion_factor(self, dimension: "Dimension") -> "Quantity[Decimal]":
-        return self.conversion_factors.get(dimension, None)
+        if (ucf := getattr(self, "_unit_conversion_factors_lookup", None)) is None:
+            ucf = UnitConversionContext.make_conversion_factors(self.unit_conversion_factors)
+            object.__setattr__(self, '_unit_conversion_factors_lookup', ucf)
+
+        return ucf.get(dimension, None)
 
     @staticmethod
     def make_conversion_factors(factors: Iterable["Quantity[Decimal]"]):
         combination_factors = [[reduce(operator.mul, j)
                                 for j in combinations(factors, i)] for i in range(2, len(factors) + 1)]
 
         all_factors = chain(*((f, Decimal(1)/f) for f in chain(factors, chain.from_iterable(combination_factors))))
```

### Comparing `hg_oap-0.1.0/src/hg_oap/utils/exprclass.py` & `hg_oap-0.1.1/src/hg_oap/utils/exprclass.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from abc import abstractmethod
 from dataclasses import dataclass, Field
 from datetime import date
 from inspect import isfunction, signature
 
 from hg_oap.dates.dgen import make_date, is_dgen
-from hg_oap.utils.magic import Op, Expression, is_op
+from hg_oap.utils.op import Op, Expression, is_op
 
 __all__ = ("dataclassex", 'exprclass', 'ExprClass')
 
 
 class _BaseExDescriptor:
     def __init__(self, expr):
         self.expr = expr
 
     def __get__(self, instance, owner = None):
         if instance is not None:
-            if (v := getattr(instance, self.cache_name, None)) is not None:
+            if (v := instance.__dict__.get(self.cache_name, None)) is not None:
                 return v
 
             v = self.__calc__(instance)
             object.__setattr__(instance, self.cache_name, v)
             return v
         elif owner:
             return self
@@ -30,15 +30,15 @@
     def __set__(self, instance, value):
         if value is not self and instance is not None:
             if not instance.__dataclass_params__.frozen:
                 setattr(instance, self.cache_name, value)
             else:
                 raise AttributeError(f'field {self.name} in {instance} is readonly')
 
-    def __override_set__(self, instance, value):
+    def __override__(self, instance, value):
         if value is not self and instance is not None:
             object.__setattr__(instance, self.cache_name, value)
             object.__setattr__(instance, self.overriden_name, True)
 
     def __overriden__(self, instance):
         return getattr(instance, self.overriden_name, False)
```

### Comparing `hg_oap-0.1.0/src/hg_oap/utils/magic.py` & `hg_oap-0.1.1/src/hg_oap/utils/op.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import itertools
 import operator
 from collections import defaultdict
 from typing import Callable, Union, Sequence, Mapping
 
-__all__ = ('lazy', 'calc', 'const', 'ParameterOp')
+__all__ = ('lazy', 'calc', 'ParameterOp')
 
 
 def is_op(obj):
     return isinstance(obj, Op)
 
 
 def make_op(obj):
@@ -25,18 +25,14 @@
     return ConstOp(obj)
 
 
 def lazy(obj):
     return make_op(obj)
 
 
-def const(obj):
-    return make_op(obj)
-
-
 class Op:
     def __init__(self, _priority):
         self._priority: int = _priority
 
     def __priority__(self):
         return self._priority
```

### Comparing `hg_oap-0.1.0/tests/unit/hg_oap/utils/test_calendar.py` & `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_calendar.py`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/tests/unit/hg_oap/utils/test_dataclassex.py` & `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dataclassex.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from calendar import monthrange
 from dataclasses import dataclass
 from datetime import date, timedelta
 
 from hg_oap.dates.tenor import Tenor
 from hg_oap.dates.dgen import days
 from hg_oap.utils.exprclass import ExprClass, dataclassex, CallableDescriptor, exprclass
-from hg_oap.utils.magic import ParameterOp, lazy
+from hg_oap.utils.op import ParameterOp, lazy
 
 SELF = ParameterOp(_name='SELF', _index=0)
 
 
 def test_expr_descriptor():
     @dataclass
     class expr_1:
```

### Comparing `hg_oap-0.1.0/tests/unit/hg_oap/utils/test_dgen.py` & `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import holidays
 import pytest
 
 from hg_oap.dates.calendar import WeekendCalendar, HolidayCalendar
 from hg_oap.dates.dgen import make_date, make_dgen, days, weeks, weekdays, weekends, months, years, business_days, roll_fwd, \
     roll_bwd
-from hg_oap.utils.magic import Expression
+from hg_oap.utils.op import Expression
 from hg_oap.dates.tenor import Tenor
 
 
 @pytest.mark.parametrize(['s', 'valid'], [
         ('2y3m1w6d', True),
         ('3m', True),
         ('1w', True),
@@ -194,15 +194,15 @@
     assert tuple(d for d in c()) == (date(2020, 4, 17), date(2021, 4, 16), date(2022, 4, 19), date(2023, 4, 21))
 
     c = '2020-01-03' <= roll_bwd(years.apr.fri[2]).over(calendar) < '2023-12-31'
     assert tuple(d for d in c()) == (date(2020, 4, 17), date(2021, 4, 16), date(2022, 4, 14), date(2023, 4, 21))
 
 
 def test_date_expressions():
-    from hg_oap.utils.magic import ParameterOp
+    from hg_oap.utils.op import ParameterOp
     _0 = ParameterOp(_index=0)
     _1 = ParameterOp(_index=1)
 
     c = _0 <= months.fri <= _1
     assert list(Expression(c)('2020-01-01', '2020-02-01')()) == [date(2020, 1, 3), date(2020, 1, 10), date(2020, 1, 17), date(2020, 1, 24), date(2020, 1, 31)]
 
     c = '2020-01-01' <= _0 < '2020-02-01'
```

### Comparing `hg_oap-0.1.0/tests/unit/hg_oap/utils/test_dimension.py` & `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_dimension.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from hg_oap.units.dimension import PrimaryDimension, DerivedDimension, Dimensionless
 from hg_oap.units.unit_system import UnitSystem
 
 
 def test_dimensions():
+    UnitSystem.__instance__ = None # TODO: Either make this stackable or only import U when requried
     with UnitSystem():
         length = PrimaryDimension(name='length')
         volume = length**3
         assert volume.name == 'length**3'
 
         weight = PrimaryDimension(name='weight')
         density = weight/volume
@@ -54,8 +55,18 @@
         assert U.dimensionless * U.dimensionless is U.dimensionless
 
         U.length = PrimaryDimension()
         assert U.length * U.dimensionless is U.length
         assert U.dimensionless * U.length is U.length
         assert U.length / U.dimensionless is U.length
         assert U.dimensionless / U.length**2 is U.length**-2
-        assert U.length / U.length is U.dimensionless
+        assert U.length / U.length is U.dimensionless
+
+
+def test_dimension_qualifiers():
+    with UnitSystem() as U:
+        U.money = PrimaryDimension()
+        U.us_dollars = U.money.us_dollars
+        U.euros = U.money.euros
+        U.bitcoins = U.money.bitcoins
+
+        assert (U.euros / U.us_dollars).name == 'euros/us_dollars'
```

### Comparing `hg_oap-0.1.0/tests/unit/hg_oap/utils/test_magic.py` & `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from dataclasses import dataclass
 
 import pytest
 
-from hg_oap.utils.magic import *
-from hg_oap.utils.magic import FailedOp, Expression
+from hg_oap.utils.op import *
+from hg_oap.utils.op import FailedOp, Expression
 
 
 @dataclass
 class A:
     x: int = 1
 
     def f(self, y):
```

### Comparing `hg_oap-0.1.0/tests/unit/hg_oap/utils/test_quantity_ts.py` & `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_quantity_ts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 from decimal import Decimal
 from typing import TypeVar, Type
 
+from hgraph import graph, TS, compute_node, TSB, TSL, AUTO_RESOLVE
+from hgraph.nodes import cs_from_ts, route_ref, filter_, merge
+from hgraph.test import eval_node
+
+from hg_oap.units import U
 from hg_oap.units.quantity import Quantity
 from hg_oap.units.unit import Unit, NUMBER
-from hgraph import graph, TS, compute_node, STATE, TSB, dispatch, TSL, AUTO_RESOLVE
-from hgraph.nodes import cs_from_ts, route_ref, sample, filter_, merge
-from hgraph.test import eval_node
 
 
 def test_quantity_ts():
-    from .test_quantity import units
-
-    U = units()
 
     @compute_node
     def convert(ts: TS[Quantity[float]], units: TS[Unit]) -> TS[Quantity[float]]:
         return ts.value.as_(units.value)
 
     @graph
     def g(ts: TS[float], u: TS[Unit], u1: TS[Unit]) -> TS[Quantity[float]]:
         v = cs_from_ts(Quantity[float], qty=ts, unit=u)
         return convert(v, u1)
 
     assert eval_node(g, ts=[1., None, 2.], u=[U.kg, None, None], u1=[None, U.kg, U.g]) == [None, 1.*U.kg, 2000.*U.g]
 
 
 def test_quantity_tsb():
-    from .test_quantity import units
-
-    U = units()
 
     UNIT_1 = TypeVar("UNIT_1", bound=Unit)
     UNIT_2 = TypeVar("UNIT_2", bound=Unit)
 
     @graph
     def convert(qty: TS[NUMBER], fr: TS[UNIT_1], to: TS[UNIT_2], tp: Type[NUMBER] = AUTO_RESOLVE) -> TS[NUMBER]:
         """
@@ -68,14 +64,13 @@
         return fr.value.convert(qty.value, to=to.value)
 
     @graph
     def g(ts: TS[Decimal], u: TS[Unit], u1: TS[Unit]) -> TS[Quantity[Decimal]]:
         v = TSB[Quantity[Decimal]].from_ts(qty=ts, unit=u)
         return convert(v, u1).as_scalar_ts()
 
-    with (U):
-        assert eval_node(g, ts=[Decimal(1.), None, Decimal(2.)], u=[U.kg, None, None], u1=[None, U.kg, U.g]) == [None, 1.*U.kg, 2000.*U.g]
-        assert eval_node(g,
-                         ts=[Decimal('274.15'), None, Decimal("273.15"), None],
-                         u=[U.K, None, None, None],
-                         u1=[U.K, U.degC, U.degF, U.K]) == \
-        [Decimal('274.15')*U.K, 1.*U.degC, 32.*U.degF, Decimal("273.15")*U.K]
+    assert eval_node(g, ts=[Decimal(1.), None, Decimal(2.)], u=[U.kg, None, None], u1=[None, U.kg, U.g]) == [None, 1.*U.kg, 2000.*U.g]
+    assert eval_node(g,
+                     ts=[Decimal('274.15'), None, Decimal("273.15"), None],
+                     u=[U.K, None, None, None],
+                     u1=[U.K, U.degC, U.degF, U.K]) == \
+    [Decimal('274.15')*U.K, 1.*U.degC, 32.*U.degF, Decimal("273.15")*U.K]
```

### Comparing `hg_oap-0.1.0/tests/unit/hg_oap/utils/test_units.py` & `hg_oap-0.1.1/tests/unit/hg_oap/utils/test_units.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass
 from decimal import Decimal
 
 import pytest
 
 from hg_oap.units.unit import Unit
-from hg_oap.units.dimension import PrimaryDimension, DerivedDimension
+from hg_oap.units.dimension import PrimaryDimension, DerivedDimension, Dimension
 from hg_oap.utils.exprclass import ExprClass
 from hg_oap.units.quantity import Quantity
 from hg_oap.units.unit import PrimaryUnit, DerivedUnit, OffsetDerivedUnit
 from hg_oap.units.unit_system import UnitSystem, UnitConversionContext
+from hgraph import CompoundScalar
 
 
 def test_units():
     with UnitSystem():
         length = PrimaryDimension(name='length')
         area = DerivedDimension(name='area', components=((length, 2),))
         meter = PrimaryUnit(name='meter', dimension=length)
@@ -131,30 +132,52 @@
 
 def test_time_units():
     with UnitSystem() as U:
         U.time = PrimaryDimension()
         U.seconds = PrimaryUnit(dimension=U.time)
 
 
+def test_qualified_units():
+    with UnitSystem() as U:
+        U.money = PrimaryDimension()
+        U.us_dollars = U.money.us_dollars
+        U.USD = PrimaryUnit(dimension=U.us_dollars)
+        U.USX = Decimal('0.01') * U.USD
+
+        U.euros = U.money.euros
+        U.EUR = PrimaryUnit(dimension=U.euros)
+        U.EUX = Decimal('0.01') * U.EUR
+
+        U.bitcoins = U.money.bitcoins
+        U.BTC = PrimaryUnit(dimension=U.bitcoins)
+
+        assert U.USX.convert(100., to=U.USD) == 1.
+        assert U.EUX.convert(100., to=U.EUR) == 1.
+        assert (U.EUR/U.USD).name == 'EUR/USD'  # EUR/USD
+
+        with UnitConversionContext((Decimal(1.15) * (U.USD/U.EUR),)):
+            assert U.EUR.convert(1., to=U.USD) == 1.15
+
+
 def test_contexts_and_conversion_factors():
     with UnitSystem() as U:
         U.length = PrimaryDimension()
         U.meter = PrimaryUnit(dimension=U.length)
 
         U.timespan = PrimaryDimension()
         U.second = PrimaryUnit(dimension=U.timespan)
         U.minute = DerivedUnit(primary_unit=U.second, ratio=Decimal(60))
         U.hour = DerivedUnit(primary_unit=U.minute, ratio=Decimal(60))
 
         U.velocity = U.length / U.timespan
         U.meter_per_second = U.meter / U.second
 
-        my_speed = 2. * U.meter_per_second
+        my_speed = Decimal(2.) * U.meter_per_second
 
-        with UnitConversionContext({U.length/U.timespan: my_speed}):
+        with UnitConversionContext((my_speed,)):
             assert U.hour.convert(1., to=U.meter) == 7200.
 
 
 def test_contexts_and_conversion_factors_2():
     with UnitSystem() as U:
         U.currency = PrimaryDimension()
         U.currency_unit = PrimaryUnit(dimension=U.currency)
@@ -179,35 +202,32 @@
 
         @dataclass
         class MyAsset:
             name: str
             density: Quantity
 
         @dataclass
-        class MyInstrument(ExprClass):
+        class MyInstrument(CompoundScalar, ExprClass, UnitConversionContext):
             asset: MyAsset
             lot_size: int
             unit: Unit
             price_unit: Unit
             price_tick_size: Decimal
             price_currency: str
 
-            unit_conversion_factors: dict[tuple[Unit, Unit], Quantity] = \
-                lambda s: UnitConversionContext.make_conversion_factors((
-                    Quantity(Decimal(s.lot_size), s.unit / U.lot),
-                    s.asset.density,
-                ))
-
-            def unit_conversion_context(self):
-                return UnitConversionContext(self.unit_conversion_factors)
+            unit_conversion_factors: tuple[Quantity] = \
+                lambda self: (
+                    Quantity(Decimal(self.lot_size), self.unit / U.lot),
+                    self.asset.density,
+                )
 
 
         asset = MyAsset('corn', Quantity(Decimal('0.75'), U.kg / U.liter))
         instrument = MyInstrument(asset, 10000, U.bushel, U.cent, Decimal('0.25'), 'USD')
 
-        with instrument.unit_conversion_context():
+        with instrument:
             assert U.lot.convert(1., to=U.bushel) == 10000.
             assert U.lot.convert(1., to=U.cubic_meter) == 352.391
             assert U.lot.convert(1., to=U.mt) == 264.29325
 
             assert round(U.mt.convert(1., to=U.lot), 5) == 0.00378
             assert round(U.pound.convert(1000., to=U.lot), 5) == 0.00172
```

### Comparing `hg_oap-0.1.0/.gitignore` & `hg_oap-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/LICENSE` & `hg_oap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/README.md` & `hg_oap-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hg_oap-0.1.0/pyproject.toml` & `hg_oap-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hg_oap"
 dynamic = ["version"]
 dependencies = [
-    "hgraph>=0.2.13",
+    "hgraph>=0.2.17",
     "holidays>=0.46",
 ]
 requires-python = ">=3.11"
 authors = [
     { name = "Howard Henson", email = "howard@henson.me.uk" },
 ]
 maintainers = [
```

### Comparing `hg_oap-0.1.0/PKG-INFO` & `hg_oap-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hg_oap
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to faciliate building order and pricing strategies
 Project-URL: Homepage, https://github.com/hhenson/hg_oap
 Project-URL: Repository, https://github.com/hhenson/hg_oap.git
 Author-email: Howard Henson <howard@henson.me.uk>
 License: MIT License
         
         Copyright (c) 2024 Howard Henson
@@ -29,15 +29,15 @@
 License-File: LICENSE
 Keywords: forward propogating graph,fpg,functional reactive programming,graph,oms,order,pricing,reactive,time series
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.11
-Requires-Dist: hgraph>=0.2.13
+Requires-Dist: hgraph>=0.2.17
 Requires-Dist: holidays>=0.46
 Description-Content-Type: text/markdown
 
 # HGraph Orders and Pricing Library
 
 Provides a library, based on the hgraph functional reactive framework to
 support creating order and pricing logic.
```

