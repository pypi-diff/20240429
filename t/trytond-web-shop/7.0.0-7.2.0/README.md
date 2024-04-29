# Comparing `tmp/trytond_web_shop-7.0.0.tar.gz` & `tmp/trytond_web_shop-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trytond_web_shop-7.0.0.tar", last modified: Mon Oct 30 17:45:06 2023, max compression
+gzip compressed data, was "trytond_web_shop-7.2.0.tar", last modified: Mon Apr 29 15:54:05 2024, max compression
```

## Comparing `trytond_web_shop-7.0.0.tar` & `trytond_web_shop-7.2.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:06.206468 trytond_web_shop-7.0.0/
--rw-r--r--   0 ced       (1000) ced       (1000)      197 2023-10-22 17:23:29.000000 trytond_web_shop-7.0.0/.readthedocs.yaml
--rw-r--r--   0 ced       (1000) ced       (1000)      761 2023-10-30 17:16:14.000000 trytond_web_shop-7.0.0/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      680 2023-10-30 17:16:14.000000 trytond_web_shop-7.0.0/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     2756 2023-10-30 17:45:06.206468 trytond_web_shop-7.0.0/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/README.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      817 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/__init__.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:06.203134 trytond_web_shop-7.0.0/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     2809 2023-10-22 17:23:29.000000 trytond_web_shop-7.0.0/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)       36 2023-10-22 17:23:29.000000 trytond_web_shop-7.0.0/doc/requirements-doc.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:06.199801 trytond_web_shop-7.0.0/locale/
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/bg.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5569 2023-10-30 16:47:45.000000 trytond_web_shop-7.0.0/locale/ca.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/cs.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5712 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/de.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5583 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/es.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/es_419.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/et.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/fa.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/fi.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5795 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/fr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4812 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/hu.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4565 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/id.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4556 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/it.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/lo.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/lt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5690 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/nl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/pl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/pt.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/ro.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/ru.po
--rw-r--r--   0 ced       (1000) ced       (1000)     5677 2023-10-30 16:47:45.000000 trytond_web_shop-7.0.0/locale/sl.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/tr.po
--rw-r--r--   0 ced       (1000) ced       (1000)     6492 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/uk.po
--rw-r--r--   0 ced       (1000) ced       (1000)     4467 2023-10-28 12:11:27.000000 trytond_web_shop-7.0.0/locale/zh_CN.po
--rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/message.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     1536 2023-10-06 22:51:03.000000 trytond_web_shop-7.0.0/product.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2222 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/product.xml
--rw-r--r--   0 ced       (1000) ced       (1000)     2208 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/sale.py
--rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/sale.xml
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2023-10-30 17:45:06.206468 trytond_web_shop-7.0.0/setup.cfg
--rwxr-xr-x   0 ced       (1000) ced       (1000)     4465 2023-10-27 17:38:49.000000 trytond_web_shop-7.0.0/setup.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:06.203134 trytond_web_shop-7.0.0/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)      440 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/tests/test_module.py
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2023-10-27 17:38:49.000000 trytond_web_shop-7.0.0/tox.ini
--rw-r--r--   0 ced       (1000) ced       (1000)      237 2023-10-30 17:16:10.000000 trytond_web_shop-7.0.0/tryton.cfg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:06.203134 trytond_web_shop-7.0.0/trytond_web_shop.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     2756 2023-10-30 17:45:05.000000 trytond_web_shop-7.0.0/trytond_web_shop.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1975 2023-10-30 17:45:06.000000 trytond_web_shop-7.0.0/trytond_web_shop.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2023-10-30 17:45:05.000000 trytond_web_shop-7.0.0/trytond_web_shop.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       54 2023-10-30 17:45:05.000000 trytond_web_shop-7.0.0/trytond_web_shop.egg-info/entry_points.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_web_shop-7.0.0/trytond_web_shop.egg-info/not-zip-safe
--rw-r--r--   0 ced       (1000) ced       (1000)      273 2023-10-30 17:45:05.000000 trytond_web_shop-7.0.0/trytond_web_shop.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        8 2023-10-30 17:45:05.000000 trytond_web_shop-7.0.0/trytond_web_shop.egg-info/top_level.txt
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2023-10-30 17:45:06.203134 trytond_web_shop-7.0.0/view/
--rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/product_attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/product_category_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/product_image_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/product_image_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/product_product_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/product_template_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/sale_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/shop_attribute_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      886 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/shop_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/shop_list.xml
--rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/view/user_form.xml
--rw-r--r--   0 ced       (1000) ced       (1000)    10812 2023-10-07 15:40:36.000000 trytond_web_shop-7.0.0/web.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3395 2023-04-15 07:12:15.000000 trytond_web_shop-7.0.0/web.xml
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/
+-rw-r--r--   0 ced       (1000) ced       (1000)      929 2024-04-29 15:29:56.000000 trytond_web_shop-7.2.0/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      680 2024-04-29 15:29:56.000000 trytond_web_shop-7.2.0/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)      103 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/README.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      961 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/__init__.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.014681 trytond_web_shop-7.2.0/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     3071 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      116 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)       36 2024-04-07 09:37:38.000000 trytond_web_shop-7.2.0/doc/requirements-doc.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.014681 trytond_web_shop-7.2.0/locale/
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/bg.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5569 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/ca.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/cs.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5712 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/de.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5583 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/es.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/es_419.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/et.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/fa.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/fi.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5795 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/fr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4812 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/hu.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4565 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/id.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4556 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/it.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/lo.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/lt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5690 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/nl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/pl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/pt.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/ro.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/ru.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     5677 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/sl.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/tr.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     6492 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/uk.po
+-rw-r--r--   0 ced       (1000) ced       (1000)     4467 2024-04-27 16:43:28.000000 trytond_web_shop-7.2.0/locale/zh_CN.po
+-rw-r--r--   0 ced       (1000) ced       (1000)      754 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/message.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2419 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/product.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2222 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/product.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)     2208 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/sale.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      448 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/sale.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/setup.cfg
+-rwxr-xr-x   0 ced       (1000) ced       (1000)     4517 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/setup.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.014681 trytond_web_shop-7.2.0/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)      144 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      459 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/tests/test_module.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2024-04-07 09:37:38.000000 trytond_web_shop-7.2.0/tox.ini
+-rw-r--r--   0 ced       (1000) ced       (1000)      269 2024-04-29 15:29:52.000000 trytond_web_shop-7.2.0/tryton.cfg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     2863 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     2019 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       54 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/entry_points.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2022-12-19 09:40:00.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/not-zip-safe
+-rw-r--r--   0 ced       (1000) ced       (1000)      333 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        8 2024-04-29 15:54:04.000000 trytond_web_shop-7.2.0/trytond_web_shop.egg-info/top_level.txt
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2024-04-29 15:54:05.018014 trytond_web_shop-7.2.0/view/
+-rw-r--r--   0 ced       (1000) ced       (1000)      288 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      359 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_category_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      351 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_image_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      293 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_image_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      315 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_product_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      489 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/product_template_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      405 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/sale_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      294 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/shop_attribute_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      984 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/view/shop_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      354 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/shop_list.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      425 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/view/shop_price_list_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)      433 2023-04-15 07:12:15.000000 trytond_web_shop-7.2.0/view/user_form.xml
+-rw-r--r--   0 ced       (1000) ced       (1000)    12739 2024-04-29 13:17:17.000000 trytond_web_shop-7.2.0/web.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3595 2024-04-27 16:30:39.000000 trytond_web_shop-7.2.0/web.xml
```

### Comparing `trytond_web_shop-7.0.0/CHANGELOG` & `trytond_web_shop-7.2.0/CHANGELOG`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,14 @@
 
+Version 7.2.0 - 2024-04-29
+--------------------------
+* Bug fixes (see mercurial logs for details)
+* Add countries for web shop
+* Support sale price list per web shop
+
 Version 7.0.0 - 2023-10-30
 --------------------------
 * Bug fixes (see mercurial logs for details)
 * Add support for Python 3.12
 
 Version 6.8.0 - 2023-05-01
 --------------------------
```

### Comparing `trytond_web_shop-7.0.0/COPYRIGHT` & `trytond_web_shop-7.2.0/COPYRIGHT`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Copyright (C) 2020-2023 Cédric Krier
-Copyright (C) 2020-2023 B2CK
+Copyright (C) 2020-2024 Cédric Krier
+Copyright (C) 2020-2024 B2CK
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

### Comparing `trytond_web_shop-7.0.0/LICENSE` & `trytond_web_shop-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/PKG-INFO` & `trytond_web_shop-7.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: trytond_web_shop
-Version: 7.0.0
+Version: 7.2.0
 Summary: Tryton module that provides a common base for webshops
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -45,24 +45,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_web_user<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_web_user<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_product_attribute<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_image<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_product_attribute<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_image<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_price_list<7.3,>=7.2; extra == "test"
 
 Web Shop Module
 ###############
 
 The web_shop module provides facilities to store configuration of online web
 shop.
```

### Comparing `trytond_web_shop-7.0.0/__init__.py` & `trytond_web_shop-7.2.0/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from . import product, sale, web
 
 
 def register():
     Pool.register(
         web.Shop,
         web.Shop_Warehouse,
+        web.Shop_Country,
         web.Shop_Product,
         web.Shop_ProductCategory,
         web.User,
         product.Template,
         product.Product,
         product.Category,
         sale.Sale,
@@ -24,7 +25,10 @@
         web.ShopAttribute,
         web.Shop_Attribute,
         product.Attribute,
         module='web_shop', type_='model', depends=['product_attribute'])
     Pool.register(
         product.Image,
         module='web_shop', type_='model', depends=['product_image'])
+    Pool.register(
+        web.Shop_PriceList,
+        module='web_shop', type_='model', depends=['sale_price_list'])
```

### Comparing `trytond_web_shop-7.0.0/doc/conf.py` & `trytond_web_shop-7.2.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 base_url = os.environ.get('DOC_BASE_URL')
 if base_url:
     modules_url = base_url + '/modules-{module}/'
     trytond_url = base_url + '/server/'
 else:
     modules_url = (
-        'https://docs.tryton.org/projects/modules-{module}/en/{series}/')
-    trytond_url = 'https://docs.tryton.org/projects/server/en/{series}/'
+        'https://docs.tryton.org/${series}/modules-{module}/')
+    trytond_url = 'https://docs.tryton.org/${series}/server/'
 
 
 def get_info():
     import configparser
     import subprocess
     import sys
 
@@ -67,22 +67,33 @@
     }
 html_title = info['description']
 master_doc = 'index'
 project = info['name']
 release = version = info['series']
 default_role = 'ref'
 highlight_language = 'none'
+exclude_patterns = ['**/*.inc.rst']
 extensions = [
     'sphinx_copybutton',
     'sphinx.ext.intersphinx',
     ]
 intersphinx_mapping = {
     'trytond': (trytond_url.format(series=version), None),
     }
 intersphinx_mapping.update({
         m: (modules_url.format(
                 module=m.replace('_', '-'), series=version), None)
         for m in info['modules']
         })
 linkcheck_ignore = [r'/.*', r'https://demo.tryton.org/*']
 
+try:
+    with open(os.path.join(
+                os.path.dirname(__file__),
+                'linkcheck_ignore.json'), 'r') as f:
+        import json
+        linkcheck_ignore.extend(json.load(f))
+        del json
+except FileNotFoundError:
+    pass
+
 del get_info, info, base_url, modules_url, trytond_url
```

### Comparing `trytond_web_shop-7.0.0/locale/bg.po` & `trytond_web_shop-7.2.0/locale/bg.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/ca.po` & `trytond_web_shop-7.2.0/locale/ca.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/cs.po` & `trytond_web_shop-7.2.0/locale/cs.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/de.po` & `trytond_web_shop-7.2.0/locale/de.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/es.po` & `trytond_web_shop-7.2.0/locale/es.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/es_419.po` & `trytond_web_shop-7.2.0/locale/es_419.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/et.po` & `trytond_web_shop-7.2.0/locale/et.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/fa.po` & `trytond_web_shop-7.2.0/locale/fa.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/fi.po` & `trytond_web_shop-7.2.0/locale/fi.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/fr.po` & `trytond_web_shop-7.2.0/locale/fr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/hu.po` & `trytond_web_shop-7.2.0/locale/hu.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/id.po` & `trytond_web_shop-7.2.0/locale/id.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/it.po` & `trytond_web_shop-7.2.0/locale/it.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/lo.po` & `trytond_web_shop-7.2.0/locale/lo.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/lt.po` & `trytond_web_shop-7.2.0/locale/lt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/nl.po` & `trytond_web_shop-7.2.0/locale/nl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/pl.po` & `trytond_web_shop-7.2.0/locale/pl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/pt.po` & `trytond_web_shop-7.2.0/locale/pt.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/ro.po` & `trytond_web_shop-7.2.0/locale/ro.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/ru.po` & `trytond_web_shop-7.2.0/locale/ru.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/sl.po` & `trytond_web_shop-7.2.0/locale/sl.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/tr.po` & `trytond_web_shop-7.2.0/locale/tr.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/uk.po` & `trytond_web_shop-7.2.0/locale/uk.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/locale/zh_CN.po` & `trytond_web_shop-7.2.0/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/message.xml` & `trytond_web_shop-7.2.0/message.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/product.py` & `trytond_web_shop-7.2.0/product.py`

 * *Files 27% similar despite different names*

```diff
@@ -23,28 +23,52 @@
     web_shops = fields.Many2Many(
         'web.shop-product.product', 'product', 'shop', "Web Shops",
         states={
             'invisible': ~Eval('salable'),
             },
         help="The list of web shops on which the product is published.")
 
+    @classmethod
+    def copy(cls, products, default=None):
+        default = default.copy() if default is not None else {}
+        default.setdefault('web_shops')
+        return super().copy(products, default=default)
+
 
 class Category(metaclass=PoolMeta):
     __name__ = 'product.category'
 
     web_shops = fields.Many2Many(
         'web.shop-product.category', 'category', 'shop', "Web Shops",
         help="The list of web shops on which the category is published.")
 
+    @classmethod
+    def copy(cls, categories, default=None):
+        default = default.copy() if default is not None else {}
+        default.setdefault('web_shops')
+        return super().copy(categories, default=default)
+
 
 class Attribute(metaclass=PoolMeta):
     __name__ = 'product.attribute'
 
     web_shops = fields.Many2Many(
         'web.shop-product.attribute', 'attribute', 'shop', "Web Shops",
         help="The list of web shops on which the attribute is published.")
 
+    @classmethod
+    def copy(cls, attributes, default=None):
+        default = default.copy() if default is not None else {}
+        default.setdefault('web_shops')
+        return super().copy(attributes, default=default)
+
 
 class Image(metaclass=PoolMeta):
     __name__ = 'product.image'
 
     web_shop = fields.Boolean("Web Shop")
+
+    @classmethod
+    def copy(cls, images, default=None):
+        default = default.copy() if default is not None else {}
+        default.setdefault('web_shop')
+        return super().copy(images, default=default)
```

### Comparing `trytond_web_shop-7.0.0/product.xml` & `trytond_web_shop-7.2.0/product.xml`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/sale.py` & `trytond_web_shop-7.2.0/sale.py`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/setup.py` & `trytond_web_shop-7.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     if not re.match(r'(ir|res)(\W|$)', dep):
         requires.append(get_require_version('trytond_%s' % dep))
 requires.append(get_require_version('trytond'))
 
 tests_require = [
     get_require_version('trytond_product_attribute'),
     get_require_version('trytond_product_image'),
+    get_require_version('trytond_sale_price_list'),
     ]
 
 setup(name=name,
     version=version,
     description='Tryton module that provides a common base for webshops',
     long_description=read('README.rst'),
     author='Tryton',
```

### Comparing `trytond_web_shop-7.0.0/tox.ini` & `trytond_web_shop-7.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `trytond_web_shop-7.0.0/trytond_web_shop.egg-info/PKG-INFO` & `trytond_web_shop-7.2.0/trytond_web_shop.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: trytond-web-shop
-Version: 7.0.0
+Name: trytond_web_shop
+Version: 7.2.0
 Summary: Tryton module that provides a common base for webshops
 Home-page: http://www.tryton.org/
-Download-URL: http://downloads.tryton.org/7.0/
+Download-URL: http://downloads.tryton.org/7.2/
 Author: Tryton
 Author-email: foundation@tryton.org
 License: GPL-3
 Project-URL: Bug Tracker, https://bugs.tryton.org/
 Project-URL: Documentation, https://docs.tryton.org/
 Project-URL: Forum, https://www.tryton.org/forum
 Project-URL: Source Code, https://code.tryton.org/tryton
@@ -45,24 +45,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: trytond_account<7.1,>=7.0
-Requires-Dist: trytond_company<7.1,>=7.0
-Requires-Dist: trytond_currency<7.1,>=7.0
-Requires-Dist: trytond_product<7.1,>=7.0
-Requires-Dist: trytond_sale<7.1,>=7.0
-Requires-Dist: trytond_stock<7.1,>=7.0
-Requires-Dist: trytond_web_user<7.1,>=7.0
-Requires-Dist: trytond<7.1,>=7.0
+Requires-Dist: trytond_account<7.3,>=7.2
+Requires-Dist: trytond_company<7.3,>=7.2
+Requires-Dist: trytond_country<7.3,>=7.2
+Requires-Dist: trytond_currency<7.3,>=7.2
+Requires-Dist: trytond_product<7.3,>=7.2
+Requires-Dist: trytond_sale<7.3,>=7.2
+Requires-Dist: trytond_stock<7.3,>=7.2
+Requires-Dist: trytond_web_user<7.3,>=7.2
+Requires-Dist: trytond<7.3,>=7.2
 Provides-Extra: test
-Requires-Dist: trytond_product_attribute<7.1,>=7.0; extra == "test"
-Requires-Dist: trytond_product_image<7.1,>=7.0; extra == "test"
+Requires-Dist: trytond_product_attribute<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_product_image<7.3,>=7.2; extra == "test"
+Requires-Dist: trytond_sale_price_list<7.3,>=7.2; extra == "test"
 
 Web Shop Module
 ###############
 
 The web_shop module provides facilities to store configuration of online web
 shop.
```

### Comparing `trytond_web_shop-7.0.0/trytond_web_shop.egg-info/SOURCES.txt` & `trytond_web_shop-7.2.0/trytond_web_shop.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.readthedocs.yaml
 CHANGELOG
 COPYRIGHT
 LICENSE
 MANIFEST.in
 README.rst
 __init__.py
 message.xml
@@ -56,14 +55,15 @@
 ./view/product_image_list.xml
 ./view/product_product_form.xml
 ./view/product_template_form.xml
 ./view/sale_form.xml
 ./view/shop_attribute_form.xml
 ./view/shop_form.xml
 ./view/shop_list.xml
+./view/shop_price_list_form.xml
 ./view/user_form.xml
 doc/conf.py
 doc/index.rst
 doc/requirements-doc.txt
 locale/bg.po
 locale/ca.po
 locale/cs.po
@@ -103,8 +103,9 @@
 view/product_image_list.xml
 view/product_product_form.xml
 view/product_template_form.xml
 view/sale_form.xml
 view/shop_attribute_form.xml
 view/shop_form.xml
 view/shop_list.xml
+view/shop_price_list_form.xml
 view/user_form.xml
```

### Comparing `trytond_web_shop-7.0.0/view/shop_form.xml` & `trytond_web_shop-7.2.0/view/shop_form.xml`

 * *Files 14% similar despite different names*

#### Comparing `trytond_web_shop-7.0.0/view/shop_form.xml` & `trytond_web_shop-7.2.0/view/shop_form.xml`

```diff
@@ -16,13 +16,16 @@
   <field name="type"/>
   <label name="guest_party"/>
   <field name="guest_party"/>
   <notebook colspan="4">
     <page name="warehouses">
       <field name="warehouses" colspan="4"/>
     </page>
+    <page name="countries">
+      <field name="countries" colspan="4"/>
+    </page>
     <page string="Products" id="products">
       <field name="products" colspan="4"/>
       <field name="categories" colspan="4"/>
     </page>
   </notebook>
 </form>
```

### Comparing `trytond_web_shop-7.0.0/web.py` & `trytond_web_shop-7.2.0/web.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,14 +66,16 @@
             ])
     guest_party = fields.Many2One(
         'party.party', "Guest Party",
         context={
             'company': Eval('company', -1),
             },
         depends={'company'})
+    countries = fields.Many2Many(
+        'web.shop-country.country', 'shop', 'country', "Countries")
 
     products = fields.Many2Many(
         'web.shop-product.product', 'shop', 'product', "Products",
         domain=[
             ('salable', '=', True),
             ],
         context={
@@ -142,14 +144,24 @@
             shop, = cls.search([('name', '=', name)])
             cls._name_cache.set(name, shop.id)
         else:
             shop = cls(shop_id)
         return shop
 
     @classmethod
+    def copy(cls, shops, default=None):
+        default = default.copy() if default is not None else {}
+        default.setdefault('warehouses')
+        default.setdefault('products')
+        default.setdefault('products_removed')
+        default.setdefault('categories')
+        default.setdefault('categories_removed')
+        return super().copy(shops, default=default)
+
+    @classmethod
     def write(cls, *args):
         cls._name_cache.clear()
         super().write(*args)
 
     @classmethod
     def delete(cls, shops):
         cls._name_cache.clear()
@@ -211,16 +223,16 @@
             taxes2products[tuple(sorted(taxes))].append(product)
 
         prices, taxes = {}, {}
         for tax_ids, products in taxes2products.items():
             with Transaction().set_context(**self.get_context()):
                 products = Product.browse(products)
                 taxes_ = Tax.browse(tax_ids)
-            with Transaction().set_context(taxes=tax_ids):
-                prices.update(Product.get_sale_price(products))
+                with Transaction().set_context(taxes=tax_ids):
+                    prices.update(Product.get_sale_price(products))
             for product in products:
                 price = prices[product.id]
                 if price is not None:
                     taxes[product.id] = sum(
                         t['amount'] for t in Tax.compute(
                             taxes_, price, 1, today))
                 else:
@@ -248,27 +260,70 @@
         sale.shipment_method = 'order'
         sale.web_shop = self
         sale.on_change_party()
         sale.on_change_web_shop()
         return sale
 
 
+class Shop_PriceList(metaclass=PoolMeta):
+    __name__ = 'web.shop'
+
+    sale_price_list = fields.Many2One(
+        'product.price_list', "Sale Price List",
+        domain=[
+            ('company', '=', Eval('company', -1)),
+            ],
+        help="The price list to compute sale price of products.")
+    non_sale_price_list = fields.Many2One(
+        'product.price_list', "Non-Sale Price List",
+        domain=[
+            ('company', '=', Eval('company', -1)),
+            ],
+        help="The price list to compute the price of products "
+        "when it is not on sale.")
+
+    def get_context(self):
+        context = super().get_context()
+        if self.sale_price_list:
+            context['price_list'] = self.sale_price_list.id
+        if (self.non_sale_price_list
+                and Transaction().context.get('_non_sale_price', False)):
+            context['price_list'] = self.non_sale_price_list.id
+        return context
+
+    def get_sale(self, party=None):
+        sale = super().get_sale(party=party)
+        if self.sale_price_list:
+            sale.price_list = self.sale_price_list
+        return sale
+
+
 class Shop_Warehouse(ModelSQL):
     "Web Shop - Warehouse"
     __name__ = 'web.shop-stock.location'
 
     shop = fields.Many2One(
         'web.shop', "Shop", ondelete='CASCADE', required=True)
     warehouse = fields.Many2One(
         'stock.location', "Warehouse", ondelete='CASCADE', required=True,
         domain=[
             ('type', '=', 'warehouse'),
             ])
 
 
+class Shop_Country(ModelSQL):
+    "Web Shop - Country"
+    __name__ = 'web.shop-country.country'
+
+    shop = fields.Many2One(
+        'web.shop', "Shop", ondelete='CASCADE', required=True)
+    country = fields.Many2One(
+        'country.country', "Country", ondelete='CASCADE', required=True)
+
+
 class Shop_Product(Inactivate):
     "Web Shop - Product"
     __name__ = 'web.shop-product.product'
 
     shop = fields.Many2One(
         'web.shop', "Shop", ondelete='CASCADE', required=True)
     product = fields.Many2One(
```

### Comparing `trytond_web_shop-7.0.0/web.xml` & `trytond_web_shop-7.2.0/web.xml`

 * *Files 5% similar despite different names*

#### Comparing `trytond_web_shop-7.0.0/web.xml` & `trytond_web_shop-7.2.0/web.xml`

```diff
@@ -26,44 +26,51 @@
       <field name="sequence" eval="20"/>
       <field name="view" ref="shop_view_form"/>
       <field name="act_window" ref="act_shop"/>
     </record>
     <menuitem parent="sale.menu_configuration" action="act_shop" sequence="20" id="menu_shop"/>
     <record model="ir.rule.group" id="rule_group_shop_companies">
       <field name="name">User in companies</field>
-      <field name="model" search="[('model', '=', 'web.shop')]"/>
+      <field name="model">web.shop</field>
       <field name="global_p" eval="True"/>
     </record>
     <record model="ir.rule" id="rule_shop_companies">
       <field name="domain" eval="[('company', 'in', Eval('companies', []))]" pyson="1"/>
       <field name="rule_group" ref="rule_group_shop_companies"/>
     </record>
     <record model="ir.model.access" id="access_shop">
-      <field name="model" search="[('model', '=', 'web.shop')]"/>
+      <field name="model">web.shop</field>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="False"/>
       <field name="perm_create" eval="False"/>
       <field name="perm_delete" eval="False"/>
     </record>
     <record model="ir.model.access" id="access_shop_sale_admin">
-      <field name="model" search="[('model', '=', 'web.shop')]"/>
+      <field name="model">web.shop</field>
       <field name="group" ref="sale.group_sale_admin"/>
       <field name="perm_read" eval="True"/>
       <field name="perm_write" eval="True"/>
       <field name="perm_create" eval="True"/>
       <field name="perm_delete" eval="True"/>
     </record>
   </data>
   <data depends="product_attribute">
     <record model="ir.ui.view" id="shop_view_attribute_form">
       <field name="model">web.shop</field>
       <field name="inherit" ref="shop_view_form"/>
       <field name="name">shop_attribute_form</field>
     </record>
   </data>
+  <data depends="sale_price_list">
+    <record model="ir.ui.view" id="shop_view_price_list_form">
+      <field name="model">web.shop</field>
+      <field name="inherit" ref="shop_view_form"/>
+      <field name="name">shop_price_list_form</field>
+    </record>
+  </data>
   <data>
     <record model="ir.ui.view" id="user_view_form">
       <field name="model">web.user</field>
       <field name="inherit" ref="web_user.user_view_form"/>
       <field name="name">user_form</field>
     </record>
   </data>
```

