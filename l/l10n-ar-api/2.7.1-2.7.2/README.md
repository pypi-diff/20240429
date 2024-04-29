# Comparing `tmp/l10n_ar_api-2.7.1.tar.gz` & `tmp/l10n_ar_api-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l10n_ar_api-2.7.1.tar", last modified: Mon Jan 22 15:02:07 2024, max compression
+gzip compressed data, was "l10n_ar_api-2.7.2.tar", last modified: Mon Apr 29 11:43:24 2024, max compression
```

## Comparing `l10n_ar_api-2.7.1.tar` & `l10n_ar_api-2.7.2.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.866333 l10n_ar_api-2.7.1/
--rw-r--r--   0 lbaldi     (501) staff       (20)      729 2024-01-22 15:02:07.865971 l10n_ar_api-2.7.1/PKG-INFO
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1391 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.1/README.md
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.835651 l10n_ar_api-2.7.1/l10n_ar_api/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      206 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/__init__.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.838348 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      188 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1324 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/config.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.838913 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/ws_sr_padron/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       27 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/ws_sr_padron/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1764 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/ws_sr_padron/ws_sr_padron.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.840388 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsaa/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       66 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsaa/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     1830 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsaa/certificate.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     4964 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsaa/tokens.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      944 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsaa/wsaa.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.841806 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsbfe/
--rw-r--r--   0 lbaldi     (501) staff       (20)       62 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsbfe/__init__.py
--rw-r--r--   0 lbaldi     (501) staff       (20)      218 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsbfe/error.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     3749 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsbfe/invoice.py
--rw-r--r--   0 lbaldi     (501) staff       (20)    12022 2023-10-18 16:07:13.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsbfe/wsbfe.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.843711 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsct/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)       60 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsct/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      296 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsct/error.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     5025 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsct/invoice.py
--rw-r--r--   0 lbaldi     (501) staff       (20)    17475 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsct/wsct.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.846694 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)       88 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      248 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/error.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     4499 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/invoice.py
--rw-r--r--   0 lbaldi     (501) staff       (20)      879 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/qr_generator.py
--rw-r--r--   0 lbaldi     (501) staff       (20)    14310 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/wsfe.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.848745 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfex/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       62 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfex/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      222 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfex/error.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     4326 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfex/invoice.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)    12271 2023-10-18 16:07:13.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfex/wsfex.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.850037 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wstesimbrefiscal/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)       50 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wstesimbrefiscal/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      282 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wstesimbrefiscal/error.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     5574 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wstesimbrefiscal/wstesimbrefiscal.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.851575 l10n_ar_api-2.7.1/l10n_ar_api/anmat_webservices/
--rw-r--r--   0 lbaldi     (501) staff       (20)       41 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/anmat_webservices/__init__.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     4923 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/anmat_webservices/anmat.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      199 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/anmat_webservices/config.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.853059 l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      939 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      252 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/config.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.854459 l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/cot/
--rw-r--r--   0 lbaldi     (501) staff       (20)       26 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/cot/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1251 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/cot/config.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)    20330 2024-01-22 14:51:58.000000 l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/cot/cot.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1979 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/iibb.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.856288 l10n_ar_api-2.7.1/l10n_ar_api/documents/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      101 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/documents/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      597 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/documents/invoice.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      611 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/documents/tax.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.858038 l10n_ar_api-2.7.1/l10n_ar_api/documents/tests/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       85 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/documents/tests/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     1568 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/documents/tests/test_gross_income.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     2377 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/documents/tests/test_profit.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      246 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/documents/tests/test_tribute.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     3553 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/documents/tribute.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.859744 l10n_ar_api-2.7.1/l10n_ar_api/padron/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       46 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/padron/__init__.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)    10346 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/padron/banks.py
--rw-r--r--   0 lbaldi     (501) staff       (20)       60 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/padron/config.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      712 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/padron/contributor.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.861431 l10n_ar_api-2.7.1/l10n_ar_api/padron/test/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       57 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/padron/test/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      836 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/padron/test/test_banks.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      899 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/padron/test/test_contributors.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.862575 l10n_ar_api-2.7.1/l10n_ar_api/presentations/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       59 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/presentations/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     2253 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/presentations/presentation.py
--rwxr-xr-x   0 lbaldi     (501) staff       (20)   141463 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/presentations/presentation_line.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.865288 l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/
--rwxr-xr-x   0 lbaldi     (501) staff       (20)      209 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/__init__.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     8316 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/test_purchases_sales_presentation.py
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     9156 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/test_purchases_sales_presentation_line.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     7411 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book.py
--rw-r--r--   0 lbaldi     (501) staff       (20)     8082 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book_line.py
-drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-01-22 15:02:07.837598 l10n_ar_api-2.7.1/l10n_ar_api.egg-info/
--rwxrwxrwx   0 lbaldi     (501) staff       (20)      729 2024-01-22 15:02:07.000000 l10n_ar_api-2.7.1/l10n_ar_api.egg-info/PKG-INFO
--rwxrwxrwx   0 lbaldi     (501) staff       (20)     2904 2024-01-22 15:02:07.000000 l10n_ar_api-2.7.1/l10n_ar_api.egg-info/SOURCES.txt
--rwxrwxrwx   0 lbaldi     (501) staff       (20)        1 2024-01-22 15:02:07.000000 l10n_ar_api-2.7.1/l10n_ar_api.egg-info/dependency_links.txt
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       77 2024-01-22 15:02:07.000000 l10n_ar_api-2.7.1/l10n_ar_api.egg-info/requires.txt
--rwxrwxrwx   0 lbaldi     (501) staff       (20)       12 2024-01-22 15:02:07.000000 l10n_ar_api-2.7.1/l10n_ar_api.egg-info/top_level.txt
--rw-r--r--   0 lbaldi     (501) staff       (20)       38 2024-01-22 15:02:07.866474 l10n_ar_api-2.7.1/setup.cfg
--rwxr-xr-x   0 lbaldi     (501) staff       (20)     1278 2024-01-22 14:51:58.000000 l10n_ar_api-2.7.1/setup.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.210536 l10n_ar_api-2.7.2/
+-rw-r--r--   0 lbaldi     (501) staff       (20)      729 2024-04-29 11:43:24.210101 l10n_ar_api-2.7.2/PKG-INFO
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1391 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.2/README.md
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.164902 l10n_ar_api-2.7.2/l10n_ar_api/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      206 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/__init__.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.168096 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      188 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1324 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/config.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.169331 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/ws_sr_padron/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       27 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/ws_sr_padron/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1764 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/ws_sr_padron/ws_sr_padron.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.171496 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsaa/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       66 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsaa/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     1830 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsaa/certificate.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     4964 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsaa/tokens.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      944 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsaa/wsaa.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.173798 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsbfe/
+-rw-r--r--   0 lbaldi     (501) staff       (20)       62 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsbfe/__init__.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)      218 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsbfe/error.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     3749 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsbfe/invoice.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)    12022 2023-10-18 16:07:13.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsbfe/wsbfe.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.176261 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsct/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)       60 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsct/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      296 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsct/error.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     5025 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsct/invoice.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)    17475 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsct/wsct.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.180036 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)       88 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      248 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/error.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     4499 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/invoice.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)      879 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/qr_generator.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)    14310 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/wsfe.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.182564 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfex/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       62 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfex/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      222 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfex/error.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     4326 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfex/invoice.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)    12271 2023-10-18 16:07:13.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfex/wsfex.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.184900 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wstesimbrefiscal/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)       50 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wstesimbrefiscal/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      282 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wstesimbrefiscal/error.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     5574 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wstesimbrefiscal/wstesimbrefiscal.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.187245 l10n_ar_api-2.7.2/l10n_ar_api/anmat_webservices/
+-rw-r--r--   0 lbaldi     (501) staff       (20)       41 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/anmat_webservices/__init__.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     4923 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/anmat_webservices/anmat.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      199 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/anmat_webservices/config.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.189526 l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      939 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      252 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/config.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.191762 l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/cot/
+-rw-r--r--   0 lbaldi     (501) staff       (20)       26 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/cot/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1251 2023-12-07 15:36:31.000000 l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/cot/config.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)    20330 2024-01-22 14:51:58.000000 l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/cot/cot.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1979 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/iibb.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     1789 2024-04-29 11:41:55.000000 l10n_ar_api-2.7.2/l10n_ar_api/document_types.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.195100 l10n_ar_api-2.7.2/l10n_ar_api/documents/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      101 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/documents/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      597 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/documents/invoice.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      611 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/documents/tax.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.197901 l10n_ar_api-2.7.2/l10n_ar_api/documents/tests/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       85 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/documents/tests/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     1568 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/documents/tests/test_gross_income.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     2377 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/documents/tests/test_profit.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      246 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/documents/tests/test_tribute.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     3553 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/documents/tribute.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.200455 l10n_ar_api-2.7.2/l10n_ar_api/padron/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       46 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/padron/__init__.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)    10346 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/padron/banks.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)       60 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/padron/config.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      712 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/padron/contributor.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.202566 l10n_ar_api-2.7.2/l10n_ar_api/padron/test/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       57 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/padron/test/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      836 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/padron/test/test_banks.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      899 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/padron/test/test_contributors.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.204403 l10n_ar_api-2.7.2/l10n_ar_api/presentations/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       59 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/presentations/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     2253 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/presentations/presentation.py
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)   141463 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/presentations/presentation_line.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.209102 l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)      209 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/__init__.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     8316 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/test_purchases_sales_presentation.py
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     9156 2019-02-26 14:56:03.000000 l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/test_purchases_sales_presentation_line.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     7411 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book.py
+-rw-r--r--   0 lbaldi     (501) staff       (20)     8082 2023-10-12 18:42:59.000000 l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book_line.py
+drwxr-xr-x   0 lbaldi     (501) staff       (20)        0 2024-04-29 11:43:24.166699 l10n_ar_api-2.7.2/l10n_ar_api.egg-info/
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)      729 2024-04-29 11:43:24.000000 l10n_ar_api-2.7.2/l10n_ar_api.egg-info/PKG-INFO
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)     2934 2024-04-29 11:43:24.000000 l10n_ar_api-2.7.2/l10n_ar_api.egg-info/SOURCES.txt
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)        1 2024-04-29 11:43:24.000000 l10n_ar_api-2.7.2/l10n_ar_api.egg-info/dependency_links.txt
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       77 2024-04-29 11:43:24.000000 l10n_ar_api-2.7.2/l10n_ar_api.egg-info/requires.txt
+-rwxrwxrwx   0 lbaldi     (501) staff       (20)       12 2024-04-29 11:43:24.000000 l10n_ar_api-2.7.2/l10n_ar_api.egg-info/top_level.txt
+-rw-r--r--   0 lbaldi     (501) staff       (20)       38 2024-04-29 11:43:24.210722 l10n_ar_api-2.7.2/setup.cfg
+-rwxr-xr-x   0 lbaldi     (501) staff       (20)     1278 2024-04-29 11:41:59.000000 l10n_ar_api-2.7.2/setup.py
```

### Comparing `l10n_ar_api-2.7.1/PKG-INFO` & `l10n_ar_api-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: l10n_ar_api
-Version: 2.7.1
+Version: 2.7.2
 Summary: Libreria para localizacion Argentina
 Home-page: https://github.com/odoo-arg/l10n_ar_api
 Author: BLUEORANGE GROUP SRL
 Author-email: daniel@blueorange.com.ar
 License: UNKNOWN
 Description: Libreria para localizacion Argentina
 Keywords: Libreria para localizacion Argentina
```

### Comparing `l10n_ar_api-2.7.1/README.md` & `l10n_ar_api-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/config.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/config.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/ws_sr_padron/ws_sr_padron.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/ws_sr_padron/ws_sr_padron.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsaa/certificate.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsaa/certificate.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsaa/tokens.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsaa/tokens.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsaa/wsaa.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsaa/wsaa.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsbfe/invoice.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsbfe/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsbfe/wsbfe.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsbfe/wsbfe.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsct/invoice.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsct/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsct/wsct.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsct/wsct.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/invoice.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/qr_generator.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/qr_generator.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfe/wsfe.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfe/wsfe.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfex/invoice.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfex/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wsfex/wsfex.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wsfex/wsfex.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/afip_webservices/wstesimbrefiscal/wstesimbrefiscal.py` & `l10n_ar_api-2.7.2/l10n_ar_api/afip_webservices/wstesimbrefiscal/wstesimbrefiscal.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/anmat_webservices/anmat.py` & `l10n_ar_api-2.7.2/l10n_ar_api/anmat_webservices/anmat.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/__init__.py` & `l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/__init__.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/cot/config.py` & `l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/cot/config.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/cot/cot.py` & `l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/cot/cot.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/arba_webservices/iibb.py` & `l10n_ar_api-2.7.2/l10n_ar_api/arba_webservices/iibb.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/documents/invoice.py` & `l10n_ar_api-2.7.2/l10n_ar_api/documents/invoice.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/documents/tax.py` & `l10n_ar_api-2.7.2/l10n_ar_api/documents/tax.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/documents/tests/test_gross_income.py` & `l10n_ar_api-2.7.2/l10n_ar_api/documents/tests/test_gross_income.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/documents/tests/test_profit.py` & `l10n_ar_api-2.7.2/l10n_ar_api/documents/tests/test_profit.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/documents/tribute.py` & `l10n_ar_api-2.7.2/l10n_ar_api/documents/tribute.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/padron/banks.py` & `l10n_ar_api-2.7.2/l10n_ar_api/padron/banks.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/padron/contributor.py` & `l10n_ar_api-2.7.2/l10n_ar_api/padron/contributor.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/padron/test/test_banks.py` & `l10n_ar_api-2.7.2/l10n_ar_api/padron/test/test_banks.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/padron/test/test_contributors.py` & `l10n_ar_api-2.7.2/l10n_ar_api/padron/test/test_contributors.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/presentations/presentation.py` & `l10n_ar_api-2.7.2/l10n_ar_api/presentations/presentation.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/presentations/presentation_line.py` & `l10n_ar_api-2.7.2/l10n_ar_api/presentations/presentation_line.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/test_purchases_sales_presentation.py` & `l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/test_purchases_sales_presentation.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/test_purchases_sales_presentation_line.py` & `l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/test_purchases_sales_presentation_line.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book.py` & `l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book_line.py` & `l10n_ar_api-2.7.2/l10n_ar_api/presentations/test/test_purchases_sales_vat_digital_book_line.py`

 * *Files identical despite different names*

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api.egg-info/PKG-INFO` & `l10n_ar_api-2.7.2/l10n_ar_api.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: l10n-ar-api
-Version: 2.7.1
+Version: 2.7.2
 Summary: Libreria para localizacion Argentina
 Home-page: https://github.com/odoo-arg/l10n_ar_api
 Author: BLUEORANGE GROUP SRL
 Author-email: daniel@blueorange.com.ar
 License: UNKNOWN
 Description: Libreria para localizacion Argentina
 Keywords: Libreria para localizacion Argentina
```

### Comparing `l10n_ar_api-2.7.1/l10n_ar_api.egg-info/SOURCES.txt` & `l10n_ar_api-2.7.2/l10n_ar_api.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 l10n_ar_api/__init__.py
+l10n_ar_api/document_types.py
 l10n_ar_api.egg-info/PKG-INFO
 l10n_ar_api.egg-info/SOURCES.txt
 l10n_ar_api.egg-info/dependency_links.txt
 l10n_ar_api.egg-info/requires.txt
 l10n_ar_api.egg-info/top_level.txt
 l10n_ar_api/afip_webservices/__init__.py
 l10n_ar_api/afip_webservices/config.py
```

### Comparing `l10n_ar_api-2.7.1/setup.py` & `l10n_ar_api-2.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import sys
 
 install_requires = [
-    'zeep==2.5.0',
+    'zeep==4.1.0',
     'python-dateutil',
     'M2Crypto',
     'pytz',
     'unidecode',
     'requests',
     'lxml',
     'qrcode'
@@ -15,15 +15,15 @@
 if sys.version_info[0] >= 3:
     install_requires.append('bs4')
 else:
     install_requires.append('BeautifulSoup')
 
 setup(
     name='l10n_ar_api',
-    version='2.7.1',
+    version='2.7.2',
     description='Libreria para localizacion Argentina',
     long_description='Libreria para localizacion Argentina',
     url='https://github.com/odoo-arg/l10n_ar_api',
     author='BLUEORANGE GROUP SRL',
     author_email='daniel@blueorange.com.ar',
     license='',
     classifiers=[
```

