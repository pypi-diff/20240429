# Comparing `tmp/tap-chargebee-1.3.5.tar.gz` & `tmp/tap-chargebee-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-chargebee-1.3.5.tar", last modified: Tue Oct 31 12:14:59 2023, max compression
+gzip compressed data, was "tap-chargebee-1.4.0.tar", last modified: Mon Apr 29 14:55:48 2024, max compression
```

## Comparing `tap-chargebee-1.3.5.tar` & `tap-chargebee-1.4.0.tar`

### file list

```diff
@@ -1,68 +1,77 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-31 12:14:59.714891 tap-chargebee-1.3.5/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-10-31 12:14:59.710891 tap-chargebee-1.3.5/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2750 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-10-31 12:14:59.714891 tap-chargebee-1.3.5/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      767 2023-10-31 12:06:22.000000 tap-chargebee-1.3.5/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-31 12:14:59.694890 tap-chargebee-1.3.5/tap_chargebee/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2106 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5612 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/client.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-31 12:14:59.682890 tap-chargebee-1.3.5/tap_chargebee/schemas/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-31 12:14:59.706890 tap-chargebee-1.3.5/tap_chargebee/schemas/common/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1121 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/cards.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      663 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/comments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/credit_notes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10157 2023-10-31 11:14:27.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/customers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1512 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/gifts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16164 2023-10-31 12:06:22.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/invoices.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9264 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/orders.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2667 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/payment_sources.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/promotional_credits.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8819 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/quotes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5460 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/transactions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/common/virtual_bank_accounts.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-31 12:14:59.706890 tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4948 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/coupons.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19626 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      992 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/item_families.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/item_prices.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3204 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/items.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18697 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/subscriptions.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-31 12:14:59.706890 tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3545 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/addons.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2108 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/coupons.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19440 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/events.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5561 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/plans.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10862 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/subscriptions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/state.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-31 12:14:59.710891 tap-chargebee-1.3.5/tap_chargebee/streams/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1373 2023-10-26 08:31:56.000000 tap-chargebee-1.3.5/tap_chargebee/streams/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      577 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/addons.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10386 2023-10-26 08:32:08.000000 tap-chargebee-1.3.5/tap_chargebee/streams/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      590 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/comments.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/coupons.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      604 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/credit_notes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      596 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/customers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      805 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/events.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/gifts.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      591 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/invoices.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      610 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/item_families.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/item_prices.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/items.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/orders.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/payment_sources.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      572 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/plans.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      637 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/promotional_credits.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/quotes.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/subscriptions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      611 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/transactions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/util.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      646 2023-10-25 16:19:04.000000 tap-chargebee-1.3.5/tap_chargebee/streams/virtual_bank_accounts.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-10-31 12:14:59.706890 tap-chargebee-1.3.5/tap_chargebee.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2023-10-31 12:14:59.000000 tap-chargebee-1.3.5/tap_chargebee.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2177 2023-10-31 12:14:59.000000 tap-chargebee-1.3.5/tap_chargebee.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-10-31 12:14:59.000000 tap-chargebee-1.3.5/tap_chargebee.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2023-10-31 12:14:59.000000 tap-chargebee-1.3.5/tap_chargebee.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2023-10-31 12:14:59.000000 tap-chargebee-1.3.5/tap_chargebee.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2023-10-31 12:14:59.000000 tap-chargebee-1.3.5/tap_chargebee.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.313901 tap-chargebee-1.4.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       39 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      303 2024-04-29 14:55:48.313901 tap-chargebee-1.4.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2750 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-29 14:55:48.313901 tap-chargebee-1.4.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      767 2024-04-29 14:52:23.000000 tap-chargebee-1.4.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.305900 tap-chargebee-1.4.0/tap_chargebee/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2106 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5612 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.301900 tap-chargebee-1.4.0/tap_chargebee/schemas/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.305900 tap-chargebee-1.4.0/tap_chargebee/schemas/common/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1121 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/cards.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      663 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/comments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9723 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/credit_notes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10157 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/customers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1512 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/gifts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16164 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/invoices.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9264 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/orders.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2667 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/payment_sources.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      876 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/promotional_credits.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8819 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/quotes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5460 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/transactions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1105 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/common/virtual_bank_accounts.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.305900 tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4948 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/coupons.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19626 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      992 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/item_families.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6491 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/item_prices.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3204 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22459 2024-04-29 14:52:23.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/subscriptions.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.309900 tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3545 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/addons.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2108 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/coupons.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19440 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5561 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/plans.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10862 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/subscriptions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1385 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/state.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.309900 tap-chargebee-1.4.0/tap_chargebee/streams/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1373 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      577 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/addons.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10386 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/base.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      590 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/comments.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      807 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/coupons.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      604 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/credit_notes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      596 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/customers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      805 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/events.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      568 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/gifts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      591 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/invoices.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      610 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/item_families.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      609 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/item_prices.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/items.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      581 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/orders.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/payment_sources.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      572 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/plans.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      637 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/promotional_credits.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      575 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/quotes.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/subscriptions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      611 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/transactions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      646 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tap_chargebee/streams/virtual_bank_accounts.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.305900 tap-chargebee-1.4.0/tap_chargebee.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      303 2024-04-29 14:55:48.000000 tap-chargebee-1.4.0/tap_chargebee.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2458 2024-04-29 14:55:48.000000 tap-chargebee-1.4.0/tap_chargebee.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-29 14:55:48.000000 tap-chargebee-1.4.0/tap_chargebee.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       78 2024-04-29 14:55:48.000000 tap-chargebee-1.4.0/tap_chargebee.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       21 2024-04-29 14:55:48.000000 tap-chargebee-1.4.0/tap_chargebee.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       14 2024-04-29 14:55:48.000000 tap-chargebee-1.4.0/tap_chargebee.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 14:55:48.313901 tap-chargebee-1.4.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12587 2024-04-29 14:52:23.000000 tap-chargebee-1.4.0/tests/test_chargebee_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2944 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tests/test_chargebee_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8922 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tests/test_chargebee_bookmark.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6528 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tests/test_chargebee_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3231 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tests/test_chargebee_include_delete.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3904 2024-04-29 14:52:23.000000 tap-chargebee-1.4.0/tests/test_chargebee_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6809 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tests/test_chargebee_start_date.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1412 2024-04-16 06:00:46.000000 tap-chargebee-1.4.0/tests/test_chargebee_sync.py
```

### Comparing `tap-chargebee-1.3.5/LICENSE` & `tap-chargebee-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/README.md` & `tap-chargebee-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/setup.py` & `tap-chargebee-1.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-chargebee',
-      version='1.3.5',
+      version='1.4.0',
       description='Singer.io tap for extracting data from the Chargebee API',
       author='dwallace@envoy.com',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_chargebee'],
       install_requires=[
           'tap-framework==0.1.1'
       ],
```

### Comparing `tap-chargebee-1.3.5/tap_chargebee/__init__.py` & `tap-chargebee-1.4.0/tap_chargebee/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/client.py` & `tap-chargebee-1.4.0/tap_chargebee/client.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/cards.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/cards.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/comments.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/comments.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/credit_notes.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/credit_notes.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/customers.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/customers.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/gifts.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/gifts.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/invoices.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/invoices.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/orders.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/orders.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/payment_sources.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/payment_sources.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/promotional_credits.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/promotional_credits.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/quotes.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/quotes.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/transactions.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/transactions.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/common/virtual_bank_accounts.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/common/virtual_bank_accounts.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/coupons.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/coupons.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/events.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/events.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/item_families.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/item_families.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/item_prices.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/item_prices.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/item_model/items.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/item_model/items.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/addons.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/addons.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/coupons.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/coupons.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/events.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/events.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/plans.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/plans.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/schemas/plan_model/subscriptions.json` & `tap-chargebee-1.4.0/tap_chargebee/schemas/plan_model/subscriptions.json`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/state.py` & `tap-chargebee-1.4.0/tap_chargebee/state.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/__init__.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/addons.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/addons.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/base.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/base.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/comments.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/comments.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/coupons.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/coupons.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/credit_notes.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/credit_notes.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/customers.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/customers.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/events.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/events.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/gifts.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/gifts.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/invoices.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/invoices.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/item_families.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/item_families.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/item_prices.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/item_prices.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/items.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/items.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/orders.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/orders.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/payment_sources.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/payment_sources.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/plans.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/plans.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/promotional_credits.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/promotional_credits.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/quotes.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/quotes.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/subscriptions.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/subscriptions.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/transactions.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/transactions.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee/streams/virtual_bank_accounts.py` & `tap-chargebee-1.4.0/tap_chargebee/streams/virtual_bank_accounts.py`

 * *Files identical despite different names*

### Comparing `tap-chargebee-1.3.5/tap_chargebee.egg-info/SOURCES.txt` & `tap-chargebee-1.4.0/tap_chargebee.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -51,8 +51,16 @@
 tap_chargebee/streams/payment_sources.py
 tap_chargebee/streams/plans.py
 tap_chargebee/streams/promotional_credits.py
 tap_chargebee/streams/quotes.py
 tap_chargebee/streams/subscriptions.py
 tap_chargebee/streams/transactions.py
 tap_chargebee/streams/util.py
-tap_chargebee/streams/virtual_bank_accounts.py
+tap_chargebee/streams/virtual_bank_accounts.py
+tests/test_chargebee_all_fields.py
+tests/test_chargebee_automatic_fields.py
+tests/test_chargebee_bookmark.py
+tests/test_chargebee_discovery.py
+tests/test_chargebee_include_delete.py
+tests/test_chargebee_pagination.py
+tests/test_chargebee_start_date.py
+tests/test_chargebee_sync.py
```

