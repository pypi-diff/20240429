# Comparing `tmp/mpi-cbs.mediforms-0.2.2a27.tar.gz` & `tmp/mpi-cbs.mediforms-0.3.0rc28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpi-cbs.mediforms-0.2.2a27.tar", last modified: Mon Feb 19 15:38:10 2024, max compression
+gzip compressed data, was "mpi-cbs.mediforms-0.3.0rc28.tar", last modified: Mon Apr 29 09:45:21 2024, max compression
```

## Comparing `mpi-cbs.mediforms-0.2.2a27.tar` & `mpi-cbs.mediforms-0.3.0rc28.tar`

### file list

```diff
@@ -1,71 +1,83 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.581571 mpi-cbs.mediforms-0.2.2a27/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       65 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/MANIFEST.in
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      936 2024-02-19 15:38:10.581571 mpi-cbs.mediforms-0.2.2a27/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       12 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.573571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.577571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      167 2024-02-19 15:37:42.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1768 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      189 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/apps.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     7872 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/forms.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.573571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.573571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/de/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.577571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/de/LC_MESSAGES/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     7739 2023-11-28 13:56:48.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 lotus     (1000) lotus     (1000)   105412 2023-11-28 13:56:43.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.573571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/en/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.577571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/en/LC_MESSAGES/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)   122037 2023-11-28 13:56:48.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 lotus     (1000) lotus     (1000)   158154 2023-11-28 13:56:43.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.577571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/migrations/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    48474 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/migrations/0001_initial.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1229 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/migrations/0002_alter_formdatamrt_email_alter_formdatamrt7tptx_email_and_more.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      892 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/migrations/0003_remove_formdatamrtconnectom_token_created_by_and_more.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/migrations/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    10439 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/models.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.573571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.577571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      711 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/base.html
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.581571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     7405 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/data_protection_declaration_mrt.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2444 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/data_storage_and_usage_consent_mrtbegleitung.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     6705 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrt.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     3306 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrtbegleitung.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     4060 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_tms.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    21313 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrt.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     7095 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrtbegleitung.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    13558 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/information_text_tms.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1796 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/iup.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      317 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/index.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      230 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/login.html
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.581571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      738 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/base.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      215 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/data_protection_declaration_mrt.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      228 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/data_protection_declaration_mrtbegleitung.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     3669 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/data_storage_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      257 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/exploration_consent.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5681 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      939 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form_complete.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5354 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form_mrt.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     4901 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form_mrtbegleitung.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5059 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form_tms.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      254 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/information_text.html
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.581571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pdfs/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     3786 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pdfs/mrt.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     3628 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pdfs/mrtbegleitung.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      397 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pdfs/pdf.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     4009 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pdfs/tms.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      636 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/token_list.html
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.581571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/widgets/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      367 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/widgets/radio_select.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1998 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     7005 2024-02-19 15:36:59.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/views.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      123 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/widgets.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-02-19 15:38:10.577571 mpi-cbs.mediforms-0.2.2a27/mpi_cbs.mediforms.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      936 2024-02-19 15:38:10.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs.mediforms.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2848 2024-02-19 15:38:10.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs.mediforms.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2024-02-19 15:38:10.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs.mediforms.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       87 2024-02-19 15:38:10.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs.mediforms.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        8 2024-02-19 15:38:10.000000 mpi-cbs.mediforms-0.2.2a27/mpi_cbs.mediforms.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2024-02-19 15:38:10.581571 mpi-cbs.mediforms-0.2.2a27/setup.cfg
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1513 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.2.2a27/setup.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.036885 mpi-cbs.mediforms-0.3.0rc28/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       65 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/MANIFEST.in
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      937 2024-04-29 09:45:21.032885 mpi-cbs.mediforms-0.3.0rc28/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       12 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.020885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.024885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      164 2024-04-12 09:54:10.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1929 2024-03-26 08:30:54.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/admin.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      189 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/apps.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     7872 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/forms.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.020885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.020885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/de/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.024885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     7739 2023-11-28 13:56:48.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)   105412 2023-11-28 13:56:43.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.020885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/en/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.024885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)   122037 2023-11-28 13:56:48.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)   158154 2023-11-28 13:56:43.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.028885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/management/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2024-03-25 14:09:17.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/management/__init__.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.028885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/management/commands/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2024-03-25 14:09:41.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/management/commands/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     4391 2024-04-29 08:11:24.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/management/commands/process_pdf_rendering_jobs.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.028885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    48474 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/0001_initial.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1229 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/0002_alter_formdatamrt_email_alter_formdatamrt7tptx_email_and_more.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      892 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/0003_remove_formdatamrtconnectom_token_created_by_and_more.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1104 2024-04-29 08:16:36.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/0004_pdfrenderingjob.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    11044 2024-04-29 08:15:54.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/models.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.024885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.028885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      711 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/base.html
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.028885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/emails/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      790 2024-04-11 10:41:32.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/emails/base.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      646 2024-04-11 10:56:01.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/emails/mrt.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      693 2024-04-11 11:07:17.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/emails/mrtbegleitung.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      625 2024-04-11 10:45:53.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/emails/tms.txt
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.032885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     7405 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/data_protection_declaration_mrt.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2444 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/data_storage_and_usage_consent_mrtbegleitung.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     6705 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrt.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     3306 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrtbegleitung.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     4060 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_tms.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    21313 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrt.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     7095 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrtbegleitung.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    13558 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/information_text_tms.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1796 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/iup.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      317 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/index.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      230 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/login.html
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.032885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      738 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/base.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      215 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/data_protection_declaration_mrt.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      228 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/data_protection_declaration_mrtbegleitung.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     3669 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/data_storage_consent.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      257 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/exploration_consent.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     5681 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      939 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form_complete.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     5354 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form_mrt.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     4901 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form_mrtbegleitung.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     5059 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form_tms.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      254 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/information_text.html
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.032885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pdfs/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     3734 2024-03-26 08:48:09.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pdfs/mrt.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     3576 2024-04-05 08:49:02.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pdfs/mrtbegleitung.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      397 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pdfs/pdf.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     3957 2024-04-05 08:48:14.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pdfs/tms.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      887 2024-04-11 11:02:29.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/success.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      636 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/token_list.html
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.032885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/widgets/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      367 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/widgets/radio_select.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2147 2024-04-05 09:59:21.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     4243 2024-04-12 09:37:57.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/views.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      123 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/widgets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2024-04-29 09:45:21.024885 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs.mediforms.egg-info/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      937 2024-04-29 09:45:20.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs.mediforms.egg-info/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     3334 2024-04-29 09:45:20.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs.mediforms.egg-info/SOURCES.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2024-04-29 09:45:20.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs.mediforms.egg-info/dependency_links.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       87 2024-04-29 09:45:20.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs.mediforms.egg-info/requires.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        8 2024-04-29 09:45:20.000000 mpi-cbs.mediforms-0.3.0rc28/mpi_cbs.mediforms.egg-info/top_level.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2024-04-29 09:45:21.036885 mpi-cbs.mediforms-0.3.0rc28/setup.cfg
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1513 2023-11-28 13:56:38.000000 mpi-cbs.mediforms-0.3.0rc28/setup.py
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/PKG-INFO` & `mpi-cbs.mediforms-0.3.0rc28/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpi-cbs.mediforms
-Version: 0.2.2a27
+Version: 0.3.0rc28
 Home-page: https://bitbucket.org/huscy/mediforms
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/admin.py` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     form = MethodForm
     list_display = 'key', 'name', '_color'
 
     def _color(self, method):
         return format_html('<span style="color: {};">{}</span>', method.color, method.color)
 
 
+class PDFRenderingJobAdmin(admin.ModelAdmin):
+    list_display = 'id', 'method', 'form_data'
+
+
 class PDFAdmin(admin.ModelAdmin):
     list_display = 'pseudonym', 'last_name', 'first_name'
 
     def pseudonym(self, pdf):
         return pdf.form_data.pseudonym
 
     def last_name(self, pdf):
@@ -51,9 +55,10 @@
 
 admin.site.register(models.FormDataMRT, FormDataAdmin)
 admin.site.register(models.FormDataMRTBegleitung, FormDataAdmin)
 admin.site.register(models.FormDataTMS, FormDataAdmin)
 admin.site.register(models.Method, MethodAdmin)
 admin.site.register(models.PDFMRT, PDFAdmin)
 admin.site.register(models.PDFMRTBegleitung, PDFAdmin)
+admin.site.register(models.PDFRenderingJob, PDFRenderingJobAdmin)
 admin.site.register(models.PDFTMS, PDFAdmin)
 admin.site.register(models.Token, TokenAdmin)
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/forms.py` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/forms.py`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.mo` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.po` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.mo` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.po` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/migrations/0001_initial.py` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/migrations/0002_alter_formdatamrt_email_alter_formdatamrt7tptx_email_and_more.py` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/0002_alter_formdatamrt_email_alter_formdatamrt7tptx_email_and_more.py`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/migrations/0003_remove_formdatamrtconnectom_token_created_by_and_more.py` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/migrations/0003_remove_formdatamrtconnectom_token_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/models.py` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 import string
 import unicodedata
 from uuid import uuid4
 
 from django.conf import settings
+from django.contrib.contenttypes.fields import GenericForeignKey
+from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 
 def sanitize_string(_string):
     # replace umlauts
     _string = re.sub('[ä]', 'ae', _string)
@@ -237,14 +239,26 @@
 class FormDataTMS(FormData, PersonalData, QuestionsTMS, QuestionsWomen):
     class Meta:
         ordering = 'last_name', 'first_name', 'date_of_birth'
         verbose_name = _('Form data TMS')
         verbose_name_plural = _('Form data TMS')
 
 
+class PDFRenderingJob(models.Model):
+    method = models.ForeignKey(Method, on_delete=models.PROTECT)
+    content_type = models.ForeignKey(ContentType, on_delete=models.PROTECT)
+    object_id = models.PositiveIntegerField()
+    form_data = GenericForeignKey('content_type', 'object_id')
+    language = models.CharField(_('Language'), max_length=8, default='de')
+
+    class Meta:
+        verbose_name = _('PDF rendering job')
+        verbose_name_plural = _('PDF rendering jobs')
+
+
 class PDF(models.Model):
     def get_upload_path(self, filename):
         pseudonym = sanitize_string(self.form_data.pseudonym)
         return f'consents/{pseudonym}/{filename}'
 
     file_handle = models.FileField(_('File handle'), upload_to=get_upload_path, max_length=128)
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/base.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/base.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/data_protection_declaration_mrt.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/data_protection_declaration_mrt.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/data_storage_and_usage_consent_mrtbegleitung.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/data_storage_and_usage_consent_mrtbegleitung.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrt.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrt.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrtbegleitung.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrtbegleitung.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_tms.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_tms.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrt.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrt.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrtbegleitung.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrtbegleitung.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/information_text_tms.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/information_text_tms.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/includes/iup.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/includes/iup.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/base.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/base.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/data_storage_consent.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/data_storage_consent.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form_complete.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form_complete.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form_mrt.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form_mrt.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form_mrtbegleitung.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form_mrtbegleitung.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pages/form_tms.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pages/form_tms.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pdfs/mrt.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pdfs/tms.html`

 * *Files 16% similar despite different names*

```diff
@@ -2,110 +2,109 @@
 
 {% load i18n %}
 
 
 {% block body %}
 <div class="ui centered grid">
   <div class="sixteen wide column">
-    <h1>{% blocktranslate %}Magnetresonanz-Tomographie (MRT){% endblocktranslate %}</h1>
+    <h1>
+      {% blocktranslate %}Informationen zum Untersuchungsablauf und Einwilligungserklärungen zu Studien mit Einsatz von magnetischen und elektrischen Stimulationsmethoden:{% endblocktranslate %}<br>
+      {% blocktranslate %}Transkranielle Magnetstimulation (TMS){% endblocktranslate %}<br>
+      {% blocktranslate %}Transkranielle Gleichstromstimulation (tDCS){% endblocktranslate %}<br>
+      {% blocktranslate %}Transkutane spinale Gleichstromstimulation (tsDCS){% endblocktranslate %}
+    </h1>
   </div>
 
-  {% include "mediforms/includes/information_text_mrt.html" %}
+  {% include "mediforms/includes/information_text_tms.html" %}
 </div>
 
 
 <div class="ui centered grid" style="page-break-before: always;">
-  <div class="sixteen wide column">
+  <div class="fourteen wide column">
     <p style="text-align: center; border: 2px solid black; padding: 5px;">
       <b>{% blocktranslate %}Fragebogen zur Person und zu Kontraindikationen im Rahmen der Studie{% endblocktranslate %}</b><br>
-      <span class="h3">{% blocktranslate %}Magnetresonanz-Tomographie (MRT){% endblocktranslate %}</span>
+      <span>{% blocktranslate %}TMS/tDCS/tsDCS-Untersuchung{% endblocktranslate %}</span>
     </p>
 
     <table>
       <tr>
         <th>{{ form.last_name.label_tag }}</th>
-        <td>{{ form.instance.last_name }}</td>
+        <td>{{ form_data.last_name }}</td>
         <th>{{ form.first_name.label_tag }}</th>
-        <td>{{ form.instance.first_name }}</td>
+        <td>{{ form_data.first_name }}</td>
         <th>{{ form.height.label_tag }}</th>
-        <td>{{ form.instance.height|default_if_none:"" }} cm</td>
+        <td>{{ form_data.height|default_if_none:"" }}</td>
       </tr>
       <tr>
         <th>{{ form.date_of_birth.label_tag }}</th>
-        <td>{{ form.instance.date_of_birth }}</td>
+        <td>{{ form_data.date_of_birth }}</td>
         <th>{{ form.birthplace.label_tag }}</th>
-        <td>{{ form.instance.birthplace|default_if_none:"" }}</td>
+        <td>{{ form_data.birthplace|default_if_none:"" }}</td>
         <th>{{ form.weight.label_tag }}</th>
-        <td>{{ form.instance.weight|default_if_none:"" }} kg</td>
+        <td>{{ form_data.weight|default_if_none:"" }}</td>
       </tr>
       <tr>
         <th>{{ form.gender.label_tag }}</th>
-        <td>{{ form.instance.get_gender_display|default_if_none:"" }}</td>
+        <td>{{ form_data.get_gender_display|default_if_none:"" }}</td>
         <td colspan="4"></td>
       </tr>
       <tr>
         <th>{{ form.street.label_tag }}</th>
-        <td>{{ form.instance.street|default_if_none:"" }}</td>
+        <td>{{ form_data.street|default_if_none:"" }}</td>
         <th>{{ form.zip_code.label_tag }}</th>
-        <td>{{ form.instance.zip_code|default_if_none:"" }}</td>
+        <td>{{ form_data.zip_code|default_if_none:"" }}</td>
         <th>{{ form.city.label_tag }}</th>
-        <td>{{ form.instance.city|default_if_none:"" }}</td>
+        <td>{{ form_data.city|default_if_none:"" }}</td>
       </tr>
       <tr>
         <th>{{ form.phone_number.label_tag }}</th>
-        <td>{{ form.instance.phone_number|default_if_none:"" }}</td>
+        <td>{{ form_data.phone_number|default_if_none:"" }}</td>
         <th>{{ form.mobile_number.label_tag }}</th>
-        <td>{{ form.instance.mobile_number|default_if_none:"" }}</td>
+        <td>{{ form_data.mobile_number|default_if_none:"" }}</td>
         <td colspan="2"></td>
       </tr>
       <tr>
         <th>{{ form.email.label_tag }}</th>
-        <td>{{ form.instance.email }}</td>
+        <td>{{ form_data.email }}</td>
         <td colspan="4"></td>
       </tr>
     </table>
 
-    <table style="width: 80%">
+    <table style="width: 75%">
       {% for field in questions_form %}
       <tr>
         <td>{{ forloop.counter }}. {{ field.label_tag }}</td>
         <td>
           {% if field.field.widget.input_type == "radio" %}
           {% trans field.value %}
           {% else %}
           {{ field.value }}
           {% endif %}
         </td>
       </tr>
       {% endfor %}
 
       <tr>
-        <td colspan="2"><i style="font-size: 15px">{% blocktranslate %}NUR FÜR VERSUCHSTEILNEHMERINNEN:{% endblocktranslate %}</i></td>
+        <td colspan="2"><i style="font-size: 15px;">{% blocktranslate %}NUR FÜR VERSUCHSTEILNEHMERINNEN:{% endblocktranslate %}</i></td>
       </tr>
 
       {% for field in questions_form_women %}
       <tr>
         <td>{{ field.label_tag }}</td>
         <td>{% if field.value %}{% trans field.value %}{% endif %}</td>
       </tr>
       {% endfor %}
     </table>
-
-    <p style="margin-top: 30px">{% blocktranslate %}Wenn Sie etwas nicht verstanden haben oder zusätzliche Informationen benötigen, geben wir Ihnen gerne nähere Auskünfte im Gespräch. Bitte fragen Sie uns nach allem, was Ihnen wichtig erscheint.{% endblocktranslate %}</p>
   </div>
 </div>
 
 
-<div class="ui centered grid" style="page-break-before: always;">
-{% include "mediforms/includes/iup.html" %}
+<div class="fifteen wide column">
+  <p>{% blocktranslate %}Wenn Sie etwas nicht verstanden haben oder zusätzliche Informationen benötigen, geben wir Ihnen gerne nähere Auskünfte im Gespräch. Bitte fragen Sie uns nach allem, was Ihnen wichtig erscheint.{% endblocktranslate %}</p>
 </div>
 
 
 <div class="ui centered grid" style="page-break-before: always;">
-{% include "mediforms/includes/data_protection_declaration_mrt.html" %}
+  {% include "mediforms/includes/exploration_consent_tms.html" %}
 </div>
 
-
-{% include "mediforms/includes/exploration_consent_mrt.html" %}
-
-
 {% endblock body %}
```

#### html2text {}

```diff
@@ -1,42 +1,47 @@
 {% extends "mediforms/pdfs/pdf.html" %} {% load i18n %} {% block body %}
-************ {{%% bblloocckkttrraannssllaattee %%}}MMaaggnneettrreessoonnaannzz--TToommooggrraapphhiiee ((MMRRTT)){{%% eennddbblloocckkttrraannssllaattee
-%%}} ************
-{% include "mediforms/includes/information_text_mrt.html" %}
+************ {{%% bblloocckkttrraannssllaattee %%}}IInnffoorrmmaattiioonneenn zzuumm UUnntteerrssuucchhuunnggssaabbllaauuff uunndd
+EEiinnwwiilllliigguunnggsseerrkkll?Ã?¤rruunnggeenn zzuu SSttuuddiieenn mmiitt EEiinnssaattzz vvoonn mmaaggnneettiisscchheenn uunndd
+eelleekkttrriisscchheenn SSttiimmuullaattiioonnssmmeetthhooddeenn::{{%% eennddbblloocckkttrraannssllaattee %%}}
+{{%% bblloocckkttrraannssllaattee %%}}TTrraannsskkrraanniieellllee MMaaggnneettssttiimmuullaattiioonn ((TTMMSS)){{%% eennddbblloocckkttrraannssllaattee
+%%}}
+{{%% bblloocckkttrraannssllaattee %%}}TTrraannsskkrraanniieellllee GGlleeiicchhssttrroommssttiimmuullaattiioonn ((ttDDCCSS)){{%%
+eennddbblloocckkttrraannssllaattee %%}}
+{{%% bblloocckkttrraannssllaattee %%}}TTrraannsskkuuttaannee ssppiinnaallee GGlleeiicchhssttrroommssttiimmuullaattiioonn ((ttssDDCCSS)){{%%
+eennddbblloocckkttrraannssllaattee %%}} ************
+{% include "mediforms/includes/information_text_tms.html" %}
 {{%% bblloocckkttrraannssllaattee %%}}FFrraaggeebbooggeenn zzuurr PPeerrssoonn uunndd zzuu KKoonnttrraaiinnddiikkaattiioonneenn iimm RRaahhmmeenn
 ddeerr SSttuuddiiee{{%% eennddbblloocckkttrraannssllaattee %%}}
-{% blocktranslate %}Magnetresonanz-Tomographie (MRT){% endblocktranslate %}
-                                                                                                                                                         {{                     {
-{{{{ ffoorrmm..llaasstt__nnaammee..llaabbeell__ttaagg  {{ form.instance.last_name }}                     {{{{ ffoorrmm..ffiirrsstt__nnaammee..llaabbeell__ttaagg {{ form.instance.first_name }}               {{                     {
-}}}}                                                                             }}}}                                                                        ffoorrmm..hheeiigghhtt..llaabbeell__ttaagg form.instance.height|default_if_none:
-                                                                                                                                                         }}}}                    "" }} cm
-{{                                                                                                                                                        {{                     {
-{{                            {{ form.instance.date_of_birth }}                 {{{{ ffoorrmm..bbiirrtthhppllaaccee..llaabbeell__ttaagg {{ form.instance.birthplace|default_if_none: {{                     {
-ffoorrmm..ddaattee__ooff__bbiirrtthh..llaabbeell__ttaagg                                                   }}}}                           "" }}                                        ffoorrmm..wweeiigghhtt..llaabbeell__ttaagg form.instance.weight|default_if_none:
-}}}}                                                                                                                                                       }}}}                    "" }} kg
+{% blocktranslate %}TMS/tDCS/tsDCS-Untersuchung{% endblocktranslate %}
+                                                                                                                                                 {{                     {
+{{{{ ffoorrmm..llaasstt__nnaammee..llaabbeell__ttaagg  {{ form_data.last_name }}                     {{{{ ffoorrmm..ffiirrsstt__nnaammee..llaabbeell__ttaagg {{ form_data.first_name }}               {{                     {
+}}}}                                                                         }}}}                                                                    ffoorrmm..hheeiigghhtt..llaabbeell__ttaagg form_data.height|default_if_none:
+                                                                                                                                                 }}}}                    "" }}
+{{                                                                                                                                                {{                     {
+{{                            {{ form_data.date_of_birth }}                 {{{{ ffoorrmm..bbiirrtthhppllaaccee..llaabbeell__ttaagg {{ form_data.birthplace|default_if_none: {{                     {
+ffoorrmm..ddaattee__ooff__bbiirrtthh..llaabbeell__ttaagg                                               }}}}                           "" }}                                    ffoorrmm..wweeiigghhtt..llaabbeell__ttaagg form_data.weight|default_if_none:
+}}}}                                                                                                                                               }}}}                    "" }}
                              {
 {{{{ ffoorrmm..ggeennddeerr..llaabbeell__ttaagg }}}}  {
-                             form.instance.get_gender_display|default_if_none:
+                             form_data.get_gender_display|default_if_none:
                              "" }}
-                                                                               {{{{ ffoorrmm..zziipp__ccooddee..llaabbeell__ttaagg   {{ form.instance.zip_code|default_if_none:"" {{                     {
-{{{{ ffoorrmm..ssttrreeeett..llaabbeell__ttaagg }}}}  {{ form.instance.street|default_if_none:"" }}     }}}}                           }}                                           {{ ffoorrmm..cciittyy..llaabbeell__ttaagg { form.instance.city|default_if_none:
-                                                                                                                                                         }}}}                    "" }}
-{{                                                                              {{                            {
-{{                            {{ form.instance.phone_number|default_if_none:""  {{                            {
-ffoorrmm..pphhoonnee__nnuummbbeerr..llaabbeell__ttaagg  }}                                                ffoorrmm..mmoobbiillee__nnuummbbeerr..llaabbeell__ttaagg form.instance.mobile_number|default_if_none:
-}}}}                                                                             }}}}                           "" }}
-{{{{ ffoorrmm..eemmaaiill..llaabbeell__ttaagg }}}}   {{ form.instance.email }}
+                                                                           {{{{ ffoorrmm..zziipp__ccooddee..llaabbeell__ttaagg   {{ form_data.zip_code|default_if_none:"" {{                     {
+{{{{ ffoorrmm..ssttrreeeett..llaabbeell__ttaagg }}}}  {{ form_data.street|default_if_none:"" }}     }}}}                           }}                                       {{ ffoorrmm..cciittyy..llaabbeell__ttaagg { form_data.city|default_if_none:
+                                                                                                                                                 }}}}                    "" }}
+{{                                                                          {{                            {
+{{                            {{ form_data.phone_number|default_if_none:""  {{                            {
+ffoorrmm..pphhoonnee__nnuummbbeerr..llaabbeell__ttaagg  }}                                            ffoorrmm..mmoobbiillee__nnuummbbeerr..llaabbeell__ttaagg form_data.mobile_number|default_if_none:
+}}}}                                                                         }}}}                           "" }}
+{{{{ ffoorrmm..eemmaaiill..llaabbeell__ttaagg }}}}   {{ form_data.email }}
 {{ forloop.counter }}. { {% if field.field.widget.input_type ==
 { field.label_tag }}     "radio" %} {% trans field.value %} {%
                          else %} {{ field.value }} {% endif %}
 {% blocktranslate %}NUR FÃR VERSUCHSTEILNEHMERINNEN:{%
 endblocktranslate %}
 {{ field.label_tag }}    {% if field.value %}{% trans field.value
                          %}{% endif %}
 {% blocktranslate %}Wenn Sie etwas nicht verstanden haben oder zusÃ¤tzliche
 Informationen benÃ¶tigen, geben wir Ihnen gerne nÃ¤here AuskÃ¼nfte im
 GesprÃ¤ch. Bitte fragen Sie uns nach allem, was Ihnen wichtig erscheint.{%
 endblocktranslate %}
-{% include "mediforms/includes/iup.html" %}
-{% include "mediforms/includes/data_protection_declaration_mrt.html" %}
-{% include "mediforms/includes/exploration_consent_mrt.html" %} {% endblock
-body %}
+{% include "mediforms/includes/exploration_consent_tms.html" %}
+{% endblock body %}
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/pdfs/mrtbegleitung.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/pdfs/mrt.html`

 * *Files 13% similar despite different names*

```diff
@@ -2,109 +2,110 @@
 
 {% load i18n %}
 
 
 {% block body %}
 <div class="ui centered grid">
   <div class="sixteen wide column">
-    <h1>{% blocktranslate %}Magnetresonanz-Untersuchung für Begleitpersonen{% endblocktranslate %}</h1>
+    <h1>{% blocktranslate %}Magnetresonanz-Tomographie (MRT){% endblocktranslate %}</h1>
   </div>
 
-  {% include "mediforms/includes/information_text_mrtbegleitung.html" %}
+  {% include "mediforms/includes/information_text_mrt.html" %}
 </div>
 
 
 <div class="ui centered grid" style="page-break-before: always;">
   <div class="sixteen wide column">
     <p style="text-align: center; border: 2px solid black; padding: 5px;">
       <b>{% blocktranslate %}Fragebogen zur Person und zu Kontraindikationen im Rahmen der Studie{% endblocktranslate %}</b><br>
-      <span>{% blocktranslate %}Magnetresonanz-Untersuchung für Begleitpersonen{% endblocktranslate %}</span>
+      <span class="h3">{% blocktranslate %}Magnetresonanz-Tomographie (MRT){% endblocktranslate %}</span>
     </p>
 
     <table>
       <tr>
         <th>{{ form.last_name.label_tag }}</th>
-        <td>{{ form.instance.last_name }}</td>
+        <td>{{ form_data.last_name }}</td>
         <th>{{ form.first_name.label_tag }}</th>
-        <td>{{ form.instance.first_name }}</td>
+        <td>{{ form_data.first_name }}</td>
         <th>{{ form.height.label_tag }}</th>
-        <td>{{ form.instance.height|default_if_none:"" }}</td>
+        <td>{{ form_data.height|default_if_none:"" }} cm</td>
       </tr>
       <tr>
         <th>{{ form.date_of_birth.label_tag }}</th>
-        <td>{{ form.instance.date_of_birth }}</td>
+        <td>{{ form_data.date_of_birth }}</td>
         <th>{{ form.birthplace.label_tag }}</th>
-        <td>{{ form.instance.birthplace|default_if_none:"" }}</td>
+        <td>{{ form_data.birthplace|default_if_none:"" }}</td>
         <th>{{ form.weight.label_tag }}</th>
-        <td>{{ form.instance.weight|default_if_none:"" }}</td>
+        <td>{{ form_data.weight|default_if_none:"" }} kg</td>
       </tr>
       <tr>
         <th>{{ form.gender.label_tag }}</th>
-        <td>{{ form.instance.get_gender_display|default_if_none:"" }}</td>
+        <td>{{ form_data.get_gender_display|default_if_none:"" }}</td>
         <td colspan="4"></td>
       </tr>
       <tr>
         <th>{{ form.street.label_tag }}</th>
-        <td>{{ form.instance.street|default_if_none:"" }}</td>
+        <td>{{ form_data.street|default_if_none:"" }}</td>
         <th>{{ form.zip_code.label_tag }}</th>
-        <td>{{ form.instance.zip_code|default_if_none:"" }}</td>
+        <td>{{ form_data.zip_code|default_if_none:"" }}</td>
         <th>{{ form.city.label_tag }}</th>
-        <td>{{ form.instance.city|default_if_none:"" }}</td>
+        <td>{{ form_data.city|default_if_none:"" }}</td>
       </tr>
       <tr>
         <th>{{ form.phone_number.label_tag }}</th>
-        <td>{{ form.instance.phone_number|default_if_none:"" }}</td>
+        <td>{{ form_data.phone_number|default_if_none:"" }}</td>
         <th>{{ form.mobile_number.label_tag }}</th>
-        <td>{{ form.instance.mobile_number|default_if_none:"" }}</td>
+        <td>{{ form_data.mobile_number|default_if_none:"" }}</td>
         <td colspan="2"></td>
       </tr>
       <tr>
         <th>{{ form.email.label_tag }}</th>
-        <td>{{ form.instance.email }}</td>
+        <td>{{ form_data.email }}</td>
         <td colspan="4"></td>
       </tr>
     </table>
 
-    <table style="width: 75%">
+    <table style="width: 80%">
       {% for field in questions_form %}
       <tr>
         <td>{{ forloop.counter }}. {{ field.label_tag }}</td>
         <td>
           {% if field.field.widget.input_type == "radio" %}
           {% trans field.value %}
           {% else %}
           {{ field.value }}
           {% endif %}
         </td>
       </tr>
       {% endfor %}
 
       <tr>
-        <td colspan="2"><i style="font-size: 15px;">{% blocktranslate %}NUR FÜR VERSUCHSTEILNEHMERINNEN:{% endblocktranslate %}</i></td>
+        <td colspan="2"><i style="font-size: 15px">{% blocktranslate %}NUR FÜR VERSUCHSTEILNEHMERINNEN:{% endblocktranslate %}</i></td>
       </tr>
 
       {% for field in questions_form_women %}
       <tr>
         <td>{{ field.label_tag }}</td>
         <td>{% if field.value %}{% trans field.value %}{% endif %}</td>
       </tr>
       {% endfor %}
     </table>
+
+    <p style="margin-top: 30px">{% blocktranslate %}Wenn Sie etwas nicht verstanden haben oder zusätzliche Informationen benötigen, geben wir Ihnen gerne nähere Auskünfte im Gespräch. Bitte fragen Sie uns nach allem, was Ihnen wichtig erscheint.{% endblocktranslate %}</p>
   </div>
 </div>
 
 
 <div class="ui centered grid" style="page-break-before: always;">
 {% include "mediforms/includes/iup.html" %}
 </div>
 
 
 <div class="ui centered grid" style="page-break-before: always;">
-{% include "mediforms/includes/exploration_consent_mrtbegleitung.html" %}
+{% include "mediforms/includes/data_protection_declaration_mrt.html" %}
 </div>
 
 
-<div class="ui centered grid" style="page-break-before: always;">
-{% include "mediforms/includes/data_storage_and_usage_consent_mrtbegleitung.html" %}
-</div>
+{% include "mediforms/includes/exploration_consent_mrt.html" %}
+
 
 {% endblock body %}
```

#### html2text {}

```diff
@@ -1,40 +1,42 @@
 {% extends "mediforms/pdfs/pdf.html" %} {% load i18n %} {% block body %}
-************ {{%% bblloocckkttrraannssllaattee %%}}MMaaggnneettrreessoonnaannzz--UUnntteerrssuucchhuunngg ff?Ã?¼rr BBeegglleeiittppeerrssoonneenn{{%%
-eennddbblloocckkttrraannssllaattee %%}} ************
-{% include "mediforms/includes/information_text_mrtbegleitung.html" %}
+************ {{%% bblloocckkttrraannssllaattee %%}}MMaaggnneettrreessoonnaannzz--TToommooggrraapphhiiee ((MMRRTT)){{%% eennddbblloocckkttrraannssllaattee
+%%}} ************
+{% include "mediforms/includes/information_text_mrt.html" %}
 {{%% bblloocckkttrraannssllaattee %%}}FFrraaggeebbooggeenn zzuurr PPeerrssoonn uunndd zzuu KKoonnttrraaiinnddiikkaattiioonneenn iimm RRaahhmmeenn
 ddeerr SSttuuddiiee{{%% eennddbblloocckkttrraannssllaattee %%}}
-{% blocktranslate %}Magnetresonanz-Untersuchung fÃ¼r Begleitpersonen{%
-endblocktranslate %}
-                                                                                                                                                         {{                     {
-{{{{ ffoorrmm..llaasstt__nnaammee..llaabbeell__ttaagg  {{ form.instance.last_name }}                     {{{{ ffoorrmm..ffiirrsstt__nnaammee..llaabbeell__ttaagg {{ form.instance.first_name }}               {{                     {
-}}}}                                                                             }}}}                                                                        ffoorrmm..hheeiigghhtt..llaabbeell__ttaagg form.instance.height|default_if_none:
-                                                                                                                                                         }}}}                    "" }}
-{{                                                                                                                                                        {{                     {
-{{                            {{ form.instance.date_of_birth }}                 {{{{ ffoorrmm..bbiirrtthhppllaaccee..llaabbeell__ttaagg {{ form.instance.birthplace|default_if_none: {{                     {
-ffoorrmm..ddaattee__ooff__bbiirrtthh..llaabbeell__ttaagg                                                   }}}}                           "" }}                                        ffoorrmm..wweeiigghhtt..llaabbeell__ttaagg form.instance.weight|default_if_none:
-}}}}                                                                                                                                                       }}}}                    "" }}
+{% blocktranslate %}Magnetresonanz-Tomographie (MRT){% endblocktranslate %}
+                                                                                                                                                 {{                     {
+{{{{ ffoorrmm..llaasstt__nnaammee..llaabbeell__ttaagg  {{ form_data.last_name }}                     {{{{ ffoorrmm..ffiirrsstt__nnaammee..llaabbeell__ttaagg {{ form_data.first_name }}               {{                     {
+}}}}                                                                         }}}}                                                                    ffoorrmm..hheeiigghhtt..llaabbeell__ttaagg form_data.height|default_if_none:
+                                                                                                                                                 }}}}                    "" }} cm
+{{                                                                                                                                                {{                     {
+{{                            {{ form_data.date_of_birth }}                 {{{{ ffoorrmm..bbiirrtthhppllaaccee..llaabbeell__ttaagg {{ form_data.birthplace|default_if_none: {{                     {
+ffoorrmm..ddaattee__ooff__bbiirrtthh..llaabbeell__ttaagg                                               }}}}                           "" }}                                    ffoorrmm..wweeiigghhtt..llaabbeell__ttaagg form_data.weight|default_if_none:
+}}}}                                                                                                                                               }}}}                    "" }} kg
                              {
 {{{{ ffoorrmm..ggeennddeerr..llaabbeell__ttaagg }}}}  {
-                             form.instance.get_gender_display|default_if_none:
+                             form_data.get_gender_display|default_if_none:
                              "" }}
-                                                                               {{{{ ffoorrmm..zziipp__ccooddee..llaabbeell__ttaagg   {{ form.instance.zip_code|default_if_none:"" {{                     {
-{{{{ ffoorrmm..ssttrreeeett..llaabbeell__ttaagg }}}}  {{ form.instance.street|default_if_none:"" }}     }}}}                           }}                                           {{ ffoorrmm..cciittyy..llaabbeell__ttaagg { form.instance.city|default_if_none:
-                                                                                                                                                         }}}}                    "" }}
-{{                                                                              {{                            {
-{{                            {{ form.instance.phone_number|default_if_none:""  {{                            {
-ffoorrmm..pphhoonnee__nnuummbbeerr..llaabbeell__ttaagg  }}                                                ffoorrmm..mmoobbiillee__nnuummbbeerr..llaabbeell__ttaagg form.instance.mobile_number|default_if_none:
-}}}}                                                                             }}}}                           "" }}
-{{{{ ffoorrmm..eemmaaiill..llaabbeell__ttaagg }}}}   {{ form.instance.email }}
+                                                                           {{{{ ffoorrmm..zziipp__ccooddee..llaabbeell__ttaagg   {{ form_data.zip_code|default_if_none:"" {{                     {
+{{{{ ffoorrmm..ssttrreeeett..llaabbeell__ttaagg }}}}  {{ form_data.street|default_if_none:"" }}     }}}}                           }}                                       {{ ffoorrmm..cciittyy..llaabbeell__ttaagg { form_data.city|default_if_none:
+                                                                                                                                                 }}}}                    "" }}
+{{                                                                          {{                            {
+{{                            {{ form_data.phone_number|default_if_none:""  {{                            {
+ffoorrmm..pphhoonnee__nnuummbbeerr..llaabbeell__ttaagg  }}                                            ffoorrmm..mmoobbiillee__nnuummbbeerr..llaabbeell__ttaagg form_data.mobile_number|default_if_none:
+}}}}                                                                         }}}}                           "" }}
+{{{{ ffoorrmm..eemmaaiill..llaabbeell__ttaagg }}}}   {{ form_data.email }}
 {{ forloop.counter }}. { {% if field.field.widget.input_type ==
 { field.label_tag }}     "radio" %} {% trans field.value %} {%
                          else %} {{ field.value }} {% endif %}
 {% blocktranslate %}NUR FÃR VERSUCHSTEILNEHMERINNEN:{%
 endblocktranslate %}
 {{ field.label_tag }}    {% if field.value %}{% trans field.value
                          %}{% endif %}
+{% blocktranslate %}Wenn Sie etwas nicht verstanden haben oder zusÃ¤tzliche
+Informationen benÃ¶tigen, geben wir Ihnen gerne nÃ¤here AuskÃ¼nfte im
+GesprÃ¤ch. Bitte fragen Sie uns nach allem, was Ihnen wichtig erscheint.{%
+endblocktranslate %}
 {% include "mediforms/includes/iup.html" %}
-{% include "mediforms/includes/exploration_consent_mrtbegleitung.html" %}
-{% include "mediforms/includes/
-data_storage_and_usage_consent_mrtbegleitung.html" %}
-{% endblock body %}
+{% include "mediforms/includes/data_protection_declaration_mrt.html" %}
+{% include "mediforms/includes/exploration_consent_mrt.html" %} {% endblock
+body %}
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/templates/mediforms/token_list.html` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/templates/mediforms/token_list.html`

 * *Files identical despite different names*

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs/mediforms/urls.py` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs/mediforms/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 
     path(r'i18n/', include('django.conf.urls.i18n')),
 
     path('mediforms/', include([
         path('', views.Index.as_view(), name='index'),
 
         path('form/<uuid:token>/', views.FormView.as_view(), name='form'),
+        path(
+            'success/',
+            TemplateView.as_view(template_name='mediforms/success.html'),
+            name='success',
+        ),
 
         path(
             'mrt/erklaerung-datenspeicherung-und-nutzung/',
             TemplateView.as_view(template_name='mediforms/pages/data_protection_declaration_mrt.html'),
             name='data-protection-declaration-mrt',
         ),
         path(
@@ -54,9 +59,7 @@
             TemplateView.as_view(template_name='mediforms/pages/information_text.html'),
             name='information-text',
         ),
 
         path('tokens/', views.TokenListView.as_view(), name='token-list'),
     ])),
 ]
-
-
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs.mediforms.egg-info/PKG-INFO` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs.mediforms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpi-cbs.mediforms
-Version: 0.2.2a27
+Version: 0.3.0rc28
 Home-page: https://bitbucket.org/huscy/mediforms
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/mpi_cbs.mediforms.egg-info/SOURCES.txt` & `mpi-cbs.mediforms-0.3.0rc28/mpi_cbs.mediforms.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -14,22 +14,31 @@
 mpi_cbs/mediforms/urls.py
 mpi_cbs/mediforms/views.py
 mpi_cbs/mediforms/widgets.py
 mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.mo
 mpi_cbs/mediforms/locale/de/LC_MESSAGES/django.po
 mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.mo
 mpi_cbs/mediforms/locale/en/LC_MESSAGES/django.po
+mpi_cbs/mediforms/management/__init__.py
+mpi_cbs/mediforms/management/commands/__init__.py
+mpi_cbs/mediforms/management/commands/process_pdf_rendering_jobs.py
 mpi_cbs/mediforms/migrations/0001_initial.py
 mpi_cbs/mediforms/migrations/0002_alter_formdatamrt_email_alter_formdatamrt7tptx_email_and_more.py
 mpi_cbs/mediforms/migrations/0003_remove_formdatamrtconnectom_token_created_by_and_more.py
+mpi_cbs/mediforms/migrations/0004_pdfrenderingjob.py
 mpi_cbs/mediforms/migrations/__init__.py
 mpi_cbs/mediforms/templates/mediforms/base.html
 mpi_cbs/mediforms/templates/mediforms/index.html
 mpi_cbs/mediforms/templates/mediforms/login.html
+mpi_cbs/mediforms/templates/mediforms/success.html
 mpi_cbs/mediforms/templates/mediforms/token_list.html
+mpi_cbs/mediforms/templates/mediforms/emails/base.txt
+mpi_cbs/mediforms/templates/mediforms/emails/mrt.txt
+mpi_cbs/mediforms/templates/mediforms/emails/mrtbegleitung.txt
+mpi_cbs/mediforms/templates/mediforms/emails/tms.txt
 mpi_cbs/mediforms/templates/mediforms/includes/data_protection_declaration_mrt.html
 mpi_cbs/mediforms/templates/mediforms/includes/data_storage_and_usage_consent_mrtbegleitung.html
 mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrt.html
 mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_mrtbegleitung.html
 mpi_cbs/mediforms/templates/mediforms/includes/exploration_consent_tms.html
 mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrt.html
 mpi_cbs/mediforms/templates/mediforms/includes/information_text_mrtbegleitung.html
```

### Comparing `mpi-cbs.mediforms-0.2.2a27/setup.py` & `mpi-cbs.mediforms-0.3.0rc28/setup.py`

 * *Files identical despite different names*

