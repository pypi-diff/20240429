# Comparing `tmp/pyslth-0.1.8.tar.gz` & `tmp/pyslth-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.1.8.tar", last modified: Sun Apr 28 01:11:18 2024, max compression
+gzip compressed data, was "pyslth-0.1.9.tar", last modified: Sun Apr 28 13:37:57 2024, max compression
```

## Comparing `pyslth-0.1.8.tar` & `pyslth-0.1.9.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.060392 pyslth-0.1.8/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.1.8/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 01:11:18.060179 pyslth-0.1.8/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.030859 pyslth-0.1.8/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1723 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-28 01:11:17.000000 pyslth-0.1.8/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.1.8/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-28 01:11:18.060455 pyslth-0.1.8/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-28 01:10:54.000000 pyslth-0.1.8/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.036938 pyslth-0.1.8/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-23 12:02:55.000000 pyslth-0.1.8/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.1.8/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.037568 pyslth-0.1.8/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.8/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.8/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    20281 2024-04-28 00:16:11.000000 pyslth-0.1.8/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.1.8/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.8/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.037922 pyslth-0.1.8/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.038644 pyslth-0.1.8/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.8/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.8/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.040874 pyslth-0.1.8/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.8/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.8/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.8/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.1.8/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.8/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.8/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.8/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.041377 pyslth-0.1.8/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.1.8/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.1.8/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.8/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.041686 pyslth-0.1.8/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.042949 pyslth-0.1.8/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.049536 pyslth-0.1.8/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.1.8/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.1.8/slth/static/css/solid.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.051591 pyslth-0.1.8/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.8/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.8/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.8/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.1.8/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.059409 pyslth-0.1.8/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-28 01:11:08.000000 pyslth-0.1.8/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)    79781 2024-04-28 01:11:08.000000 pyslth-0.1.8/slth/static/js/lib.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-28 01:11:08.000000 pyslth-0.1.8/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/slth.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.8/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 01:11:18.059888 pyslth-0.1.8/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     2244 2024-04-28 00:37:31.000000 pyslth-0.1.8/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.1.8/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.8/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-27 15:06:10.000000 pyslth-0.1.8/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.1.8/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.1.8/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.713009 pyslth-0.1.9/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.1.9/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 13:37:57.712514 pyslth-0.1.9/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.675909 pyslth-0.1.9/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-28 13:37:57.000000 pyslth-0.1.9/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1752 2024-04-28 13:37:57.000000 pyslth-0.1.9/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-28 13:37:57.000000 pyslth-0.1.9/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-04-28 13:37:57.000000 pyslth-0.1.9/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-28 13:37:57.000000 pyslth-0.1.9/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.1.9/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-28 13:37:57.713092 pyslth-0.1.9/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-28 13:34:19.000000 pyslth-0.1.9/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.683857 pyslth-0.1.9/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3774 2024-04-28 09:42:58.000000 pyslth-0.1.9/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6947 2024-04-26 09:39:45.000000 pyslth-0.1.9/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.684952 pyslth-0.1.9/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.1.9/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     4817 2024-04-23 11:29:24.000000 pyslth-0.1.9/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    20281 2024-04-28 00:16:11.000000 pyslth-0.1.9/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.1.9/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     2379 2024-04-26 12:42:49.000000 pyslth-0.1.9/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    25162 2024-04-25 15:16:26.000000 pyslth-0.1.9/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.685371 pyslth-0.1.9/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.9/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.686259 pyslth-0.1.9/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.9/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.1.9/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.1.9/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.690122 pyslth-0.1.9/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.1.9/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.1.9/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      602 2024-04-18 19:49:54.000000 pyslth-0.1.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      452 2024-04-23 08:05:28.000000 pyslth-0.1.9/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-04-23 12:54:25.000000 pyslth-0.1.9/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.1.9/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.1.9/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6442 2024-04-28 00:48:21.000000 pyslth-0.1.9/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.1.9/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.1.9/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19210 2024-04-25 14:39:52.000000 pyslth-0.1.9/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.1.9/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.691114 pyslth-0.1.9/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.1.9/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11326 2024-04-28 13:32:26.000000 pyslth-0.1.9/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    14390 2024-04-22 11:20:25.000000 pyslth-0.1.9/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.691644 pyslth-0.1.9/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.693470 pyslth-0.1.9/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.696585 pyslth-0.1.9/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)   107280 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   116316 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   112880 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)      861 2024-04-27 15:14:58.000000 pyslth-0.1.9/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.1.9/slth/static/css/solid.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.699264 pyslth-0.1.9/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.1.9/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.1.9/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.1.9/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.1.9/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.710985 pyslth-0.1.9/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)  1112414 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      755 2024-04-28 13:34:07.000000 pyslth-0.1.9/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    79917 2024-04-28 13:34:07.000000 pyslth-0.1.9/slth/static/js/lib.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141741 2024-04-28 13:34:07.000000 pyslth-0.1.9/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      129 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/js/slth.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.1.9/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-28 13:37:57.711989 pyslth-0.1.9/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     2244 2024-04-28 00:37:31.000000 pyslth-0.1.9/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)      660 2024-04-27 15:01:32.000000 pyslth-0.1.9/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.1.9/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-27 15:06:10.000000 pyslth-0.1.9/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-04-27 19:14:01.000000 pyslth-0.1.9/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2425 2024-04-28 00:39:41.000000 pyslth-0.1.9/slth/views.py
```

### Comparing `pyslth-0.1.8/PKG-INFO` & `pyslth-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.8
+Version: 0.1.9
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.8/pyslth.egg-info/PKG-INFO` & `pyslth-0.1.9/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.1.8
+Version: 0.1.9
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.1.8/pyslth.egg-info/SOURCES.txt` & `pyslth-0.1.9/pyslth.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 slth/management/commands/integration_test.py
 slth/management/commands/sync.py
 slth/migrations/0001_initial.py
 slth/migrations/0002_email_role_pushsubscription_error.py
 slth/migrations/0003_rename_photo_profile_alter_profile_options.py
 slth/migrations/0004_alter_profile_photo.py
 slth/migrations/0005_alter_profile_photo.py
+slth/migrations/0006_user.py
 slth/migrations/__init__.py
 slth/selenium/__init__.py
 slth/selenium/browser.py
 slth/static/index.html
 slth/static/css/fontawesome.min.css
 slth/static/css/slth.css
 slth/static/css/solid.min.css
```

### Comparing `pyslth-0.1.8/setup.py` & `pyslth-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.1.8/slth/__init__.py` & `pyslth-0.1.9/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/components.py` & `pyslth-0.1.9/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/db/models.py` & `pyslth-0.1.9/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/endpoints.py` & `pyslth-0.1.9/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/factory.py` & `pyslth-0.1.9/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/forms.py` & `pyslth-0.1.9/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/management/commands/integration_test.py` & `pyslth-0.1.9/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/management/commands/sync.py` & `pyslth-0.1.9/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/migrations/0001_initial.py` & `pyslth-0.1.9/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.1.9/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.1.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/models.py` & `pyslth-0.1.9/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/permissions.py` & `pyslth-0.1.9/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/queryset.py` & `pyslth-0.1.9/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/roles.py` & `pyslth-0.1.9/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/selenium/__init__.py` & `pyslth-0.1.9/slth/selenium/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from django.contrib.staticfiles.handlers import StaticFilesHandler
 from django.contrib.staticfiles.testing import LiveServerTestCase
 from django.core.cache import cache
 from django.core.management import call_command
 from django.core.servers.basehttp import WSGIServer
 from django.db import connection
 from django.http import HttpResponse
-
+from django.core.management import call_command
 from django.contrib.auth.models import User
 
 from .browser import Browser
 
 WSGIServer.handle_error = lambda *args, **kwargs: None
 
 
@@ -56,24 +56,25 @@
         self._url = "/app/login/"
         self._execute = 1
         self._step = 0
         self._adverb = 0
 
     @classmethod
     def setUpClass(cls):
+        call_command("sync")
         cls.host = os.environ.get('BACKEND_HOST', '127.0.0.1')
         cls.port = int(os.environ.get('BACKEND_PORT', '8000'))
         super().setUpClass()
         print(cls.live_server_url)
         cache.clear()
-        url = "http://{}:{}".format(
-            os.environ.get('FRONTEND_HOST', '127.0.0.1'),
-            os.environ.get('FRONTEND_PORT', '5173')
-        )
-        cls.browser = Browser(url, slowly=False, headless=SeleniumTestCase.HEADLESS)
+        # url = "http://{}:{}".format(
+        #     os.environ.get('FRONTEND_HOST', '127.0.0.1'),
+        #     os.environ.get('FRONTEND_PORT', '5173')
+        # )
+        cls.browser = Browser(cls.live_server_url, slowly=False, headless=SeleniumTestCase.HEADLESS)
         for app_label in settings.INSTALLED_APPS:
             app_module = __import__(app_label)
             app_dir = os.path.dirname(app_module.__file__)
             fixture_path = os.path.join(app_dir, "fixtures", "test.json")
             if os.path.exists(fixture_path):
                 call_command("loaddata", fixture_path)
         settings.DEBUG = True
```

### Comparing `pyslth-0.1.8/slth/selenium/browser.py` & `pyslth-0.1.9/slth/selenium/browser.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,43 +12,48 @@
     WebDriverException,
 )
 from selenium.webdriver.common.by import By
 from selenium.webdriver.firefox.options import Options
 from selenium.webdriver.support.ui import Select
 
 
-from selenium.webdriver import Remote
+from selenium.webdriver import Remote, Firefox
 from selenium.webdriver.remote.file_detector import LocalFileDetector
 from selenium.webdriver.remote.webelement import WebElement
 
+REMOTE = 'SELENIUM_HOST' in os.environ
 
 def to_label_case(text):
     return unicodedata.normalize('NFD', text.replace('-', '').replace('_', '').lower())
 
 def _upload(self, filename):
     return filename
 
 WebElement._upload = _upload
 
-class Browser(Remote):
+class Browser(Remote if REMOTE else Firefox):
     def __init__(self, server_url, options=None, verbose=True, slowly=False, maximize=True, headless=True):
         if not options:
             options = Options()
         if maximize:
             options.add_argument("--start-maximized")
         else:
             options.add_argument("--window-size=720x800")
         if headless and "-v" not in sys.argv:
             options.add_argument("--headless")
-        url = 'http://{}:{}'.format(
-            os.environ.get('SELENIUM_HOST', '127.0.0.1'),
-            os.environ.get('SELENIUM_POST', '4444')
-        )
-        super().__init__(command_executor=url, options=options)
-        self.file_detector = LocalFileDetector()
+        
+        if REMOTE:
+            url = 'http://{}:{}'.format(
+                os.environ.get('SELENIUM_HOST', '127.0.0.1'),
+                os.environ.get('SELENIUM_POST', '4444')
+            )
+            super().__init__(command_executor=url, options=options)
+            self.file_detector = LocalFileDetector()
+        else:
+             super().__init__(options=options)
 
         self.cursor = None
         self.verbose = verbose
         self.slowly = slowly
         self.server_url = server_url
         self.headless = headless
 
@@ -127,15 +132,15 @@
                 raise WebDriverException(f"Element {value} not found in the dialog.")
             if self.cursor.tag_name != "html":
                 self.debug(f"Element {value} not found in {self.cursor.tag_name}. Searching in the parent element...")
                 self.cursor = self.cursor.find_element("xpath", "..")
             else:
                 raise WebDriverException(f"Element {value} NOT FOUND in {self.cursor.tag_name}.")
 
-    def wait(self, seconds=1):
+    def wait(self, seconds=2):
         time.sleep(seconds)
 
     def watch(self, e):
         self.save_screenshot("/tmp/test.png")
         if self.headless:
             raise e
         else:
@@ -171,53 +176,57 @@
         self.print('{} "{}" for "{}"'.format("Entering", value, name))
         if value:
             value = str(value)
             if len(value) == 10 and value[2] == "/" and value[5] == "/":
                 value = datetime.datetime.strptime(value, "%d/%m/%Y").strftime("%Y-%m-%d")
         try:
             widget = self.find_element("css selector", f'[data-label="{to_label_case(name)}"]')
-            if widget.tag_name == "input" and widget.get_property("type") == "file":
-                value = os.path.join(settings.BASE_DIR, value)
-            widget.clear()
-            widget.send_keys(value)
+            if widget.tag_name == "input" and widget.get_property("type") == "color":
+                self.execute_script(
+                    f'document.querySelector(\'input[data-label="{to_label_case(name)}"]\').value = "{value}";'
+                )
+            else:
+                if widget.tag_name == "input" and widget.get_property("type") == "file":
+                    value = os.path.join(settings.BASE_DIR, value)
+                widget.clear()
+                widget.send_keys(value)
         except WebDriverException as e:
             if count:
                 self.wait()
                 self.enter(name, value, submit, count - 1)
             else:
                 self.watch(e)
         if self.slowly:
             self.wait(2)
 
     def choose(self, name, value, count=4):
         self.print('{} "{}" for "{}"'.format("Choosing", value, name))
         try:
-            widgets = self.find_elements(By.CSS_SELECTOR, f'select[data-label="{to_label_case(name)}"]')
+            widgets = self.find_elements(By.CSS_SELECTOR, f'[data-label="{to_label_case(name)}"]')
             if widgets:
                 if widgets[0].tag_name.lower() == "select":
                     select = Select(widgets[0])
                     select.select_by_visible_text(value)
                 elif widgets[0].tag_name.lower() == "input":
                     widgets[0].send_keys(value)
                     for i in range(0, 6):
                         # print('Trying ({}) click at "{}"...'.format(i, value))
                         self.wait(0.5)
                         try:
                             super().find_element(By.CSS_SELECTOR, f'.autocomplete-item[data-label*="{to_label_case(value)}"]').click()
+                            self.wait(0.5)
                             break
                         except WebDriverException:
                             pass
+                elif widgets[0].get_dom_attribute("type") == "radio":
+                    widgets[0].click()
+                elif widgets[0].get_dom_attribute("type") == "checkbox":
+                    widgets[0].click()
             else:
-                self.look_at(name)
-                inputs = self.find_elements(By.CSS_SELECTOR, f'input[data-label="{to_label_case(value)}"]')
-                if inputs:
-                    if inputs[0].get_dom_attribute("type") == "radio":
-                        inputs[0].click()
-                    elif inputs[0].get_dom_attribute("type") == "checkbox":
-                        inputs[0].click()
+                raise WebDriverException()
         except WebDriverException as e:
             if count:
                 self.wait()
                 self.choose(name, value, count - 1)
             else:
                 self.watch(e)
         if self.slowly:
```

### Comparing `pyslth-0.1.8/slth/serializer.py` & `pyslth-0.1.9/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/css/fontawesome.min.css` & `pyslth-0.1.9/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/css/fonts/Eina02-Bold.f8011405.ttf` & `pyslth-0.1.9/slth/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/css/fonts/Eina02-Regular.2e682693.ttf` & `pyslth-0.1.9/slth/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `pyslth-0.1.9/slth/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.1.9/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/css/slth.css` & `pyslth-0.1.9/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/css/solid.min.css` & `pyslth-0.1.9/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/images/logo.png` & `pyslth-0.1.9/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/images/logo.svg` & `pyslth-0.1.9/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/images/user.png` & `pyslth-0.1.9/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/js/echarts.min.js` & `pyslth-0.1.9/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/js/index.min.js` & `pyslth-0.1.9/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/js/lib.min.js` & `pyslth-0.1.9/slth/static/js/lib.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     j as t,
     c as H,
     r as S
 } from "./react.min.js";
 
-function k(e) {
+function b(e) {
     return e != null && (e = e.toString().replace("-", "").normalize("NFD").replace("_", "").toLowerCase()), e
 }
 
 function Me(e) {
     function n(r) {
         navigator.clipboard.writeText(r), Q('Icon "' + r + '" copied to clipboard!')
     }
@@ -42,15 +42,15 @@
             style: e.style,
             className: "fa-solid fa-circle-notch fa-spin fa-1x spin"
         })
     }
     return n()
 }
 
-function w(e) {
+function j(e) {
     var n = "fa-solid fa-" + e.icon;
     return e.className && (n += " " + e.className), (e.onClick || e.clickable) && (n += " clickable"), t.jsx("i", {
         style: e.style,
         className: n,
         onClick: e.onClick
     })
 }
@@ -68,50 +68,50 @@
         };
         return e.primary && (a.backgroundColor = "#1351b4", a.color = "white"), e.default && (a.color = "#1351b4", a.border = "solid 1px #1351b4"), t.jsx("a", {
             id: e.id,
             style: a,
             onClick: r => {
                 r.preventDefault(), e.onClick()
             },
-            children: t.jsx(w, {
+            children: t.jsx(j, {
                 icon: e.icon
             })
         })
     }
     return n()
 }
 const Te = ["1", "2", "3", "4", "5", "6", "7", "8", "9", "fill-drip", "arrows-to-circle", "circle-chevron-right", "at", "trash-can", "text-height", "user-xmark", "stethoscope", "message", "info", "down-left-and-up-right-to-center", "explosion", "file-text", "wave-square", "ring", "building-un", "dice-three", "calendar-days", "anchor-circle-check", "building-circle-arrow-right", "volleyball", "arrows-up-to-line", "sort-down", "minus-circle", "door-open", "sign-out-alt", "atom", "soap", "icons", "microphone-lines-slash", "bridge-circle-check", "pump-medical", "fingerprint", "hand-point-right", "search-location", "step-forward", "smile-beam", "flag-checkered", "football", "school-circle-exclamation", "crop", "angles-down", "users-rectangle", "people-roof", "people-line", "beer", "diagram-predecessor", "long-arrow-up", "fire-flame-simple", "person", "laptop", "file-csv", "menorah", "truck-plane", "record-vinyl", "grin-stars", "bong", "spaghetti-monster-flying", "arrow-down-up-across-line", "utensil-spoon", "jar-wheat", "mail-bulk", "file-circle-exclamation", "hospital-symbol", "pager", "contact-book", "strikethrough", "k", "landmark-flag", "pencil", "backward", "caret-right", "comments", "paste", "code-pull-request", "clipboard-list", "truck-ramp-box", "user-check", "vial-virus", "sheet-plastic", "blog", "user-ninja", "person-arrow-up-from-line", "torah", "quidditch", "toggle-off", "box-archive", "person-drowning", "sort-numeric-down-alt", "grin-tongue-squint", "spray-can", "truck-monster", "w", "globe-africa", "rainbow", "circle-notch", "tablet-screen-button", "paw", "cloud", "trowel-bricks", "flushed", "hospital-user", "tent-arrow-left-right", "legal", "binoculars", "microphone-slash", "box-tissue", "motorcycle", "concierge-bell", "pencil-ruler", "people-arrows", "mars-and-venus-burst", "square-caret-right", "scissors", "sun-plant-wilt", "toilets-portable", "hockey-puck", "table", "magnifying-glass-arrow-right", "tachograph-digital", "users-slash", "clover", "reply", "star-and-crescent", "house-fire", "square-minus", "helicopter", "compass", "square-caret-down", "file-circle-question", "laptop-code", "swatchbook", "prescription-bottle", "navicon", "people-group", "hourglass-end", "heart-crack", "square-up-right", "kiss-beam", "film", "ruler-horizontal", "people-robbery", "lightbulb", "caret-left", "exclamation-circle", "school-circle-xmark", "sign-out", "circle-chevron-down", "unlock-keyhole", "cloud-showers-heavy", "headphones-simple", "sitemap", "donate", "memory", "road-spikes", "fire-burner", "flag", "hanukiah", "feather", "volume-low", "comment-slash", "cloud-sun-rain", "compress", "wheat-awn", "ankh", "hands-holding-child", "asterisk", "square-check", "peseta-sign", "heading", "ghost", "list", "square-phone-flip", "cart-plus", "gamepad", "dot-circle", "face-dizzy", "egg", "house-medical-circle-xmark", "campground", "folder-plus", "soccer-ball", "paintbrush", "lock", "gas-pump", "hot-tub", "map-marked", "house-flood-water", "tree", "bridge-lock", "sack-dollar", "pen-to-square", "car-side", "share-nodes", "heart-circle-minus", "hourglass-half", "microscope", "sink", "shopping-bag", "sort-alpha-down-alt", "mitten", "person-rays", "users", "eye-slash", "flask-vial", "hand", "om", "worm", "house-circle-xmark", "plug", "chevron-up", "hand-spock", "stopwatch", "kiss", "bridge-circle-xmark", "grin-tongue", "chess-bishop", "grin-wink", "hard-of-hearing", "road-circle-check", "dice-five", "square-rss", "land-mine-on", "i-cursor", "stamp", "stairs", "i", "hryvnia", "pills", "grin-alt", "tooth", "v", "bangladeshi-taka-sign", "bicycle", "staff-snake", "head-side-cough-slash", "truck-medical", "wheat-awn-circle-exclamation", "snowman", "mortar-pestle", "road-barrier", "school", "igloo", "joint", "angle-right", "horse", "q", "g", "notes-medical", "thermometer-half", "dong-sign", "capsules", "poo-storm", "frown-open", "hand-point-up", "money-bill", "bookmark", "align-justify", "umbrella-beach", "helmet-un", "bullseye", "bacon", "hand-point-down", "arrow-up-from-bracket", "folder", "file-waveform", "radiation", "chart-simple", "mars-stroke", "vial", "tachometer-alt-average", "wand-magic-sparkles", "e", "pen-clip", "bridge-circle-exclamation", "user", "school-circle-check", "dumpster", "van-shuttle", "building-user", "square-caret-left", "highlighter", "key", "bullhorn", "globe", "synagogue", "person-half-dress", "road-bridge", "location-arrow", "c", "tablet-button", "building-lock", "pizza-slice", "money-bill-wave", "chart-area", "house-flag", "person-circle-minus", "cancel", "camera-rotate", "spray-can-sparkles", "star", "repeat", "cross", "box", "venus-mars", "mouse-pointer", "maximize", "charging-station", "triangle-circle-square", "shuffle", "running", "mobile-retro", "grip-lines-vertical", "spider", "hands-bound", "file-invoice-dollar", "plane-circle-exclamation", "x-ray", "spell-check", "slash", "mouse", "sign-in", "store-alt-slash", "server", "virus-covid-slash", "shop-lock", "hourglass-start", "blender-phone", "building-wheat", "person-breastfeeding", "sign-in-alt", "venus", "passport", "heartbeat", "people-carry", "temperature-high", "microchip", "crown", "weight-hanging", "xmarks-lines", "file-prescription", "weight", "user-group", "sort-alpha-up", "chess-knight", "laugh-squint", "wheelchair", "circle-arrow-up", "toggle-on", "walking", "l", "fire", "procedures", "space-shuttle", "laugh", "folder-open", "heart-circle-plus", "code-fork", "city", "microphone-lines", "pepper-hot", "unlock", "colon-sign", "headset", "store-slash", "road-circle-xmark", "user-minus", "mars-stroke-v", "glass-cheers", "clipboard", "house-circle-exclamation", "file-upload", "wifi", "bathtub", "underline", "user-pen", "signature", "stroopwafel", "bold", "anchor-lock", "building-ngo", "manat-sign", "not-equal", "border-top-left", "map-marked-alt", "jedi", "square-poll-vertical", "mug-hot", "car-battery", "gift", "dice-two", "chess-queen", "glasses", "chess-board", "building-circle-check", "person-chalkboard", "mars-stroke-right", "hand-rock", "square-caret-up", "cloud-showers-water", "chart-bar", "hands-wash", "less-than-equal", "train", "low-vision", "crow", "sailboat", "window-restore", "square-plus", "torii-gate", "frog", "bucket", "image", "microphone", "cow", "caret-up", "screwdriver", "folder-closed", "house-tsunami", "square-nfi", "arrow-up-from-ground-water", "martini-glass", "undo-alt", "table-columns", "lemon", "head-side-mask", "handshake", "gem", "dolly", "smoking", "minimize", "monument", "snowplow", "angles-right", "cannabis", "play-circle", "tablets", "ethernet", "euro", "chair", "circle-check", "stop-circle", "drafting-compass", "plate-wheat", "icicles", "person-shelter", "neuter", "id-badge", "marker", "laugh-beam", "helicopter-symbol", "universal-access", "circle-chevron-up", "lari-sign", "volcano", "person-walking-dashed-line-arrow-right", "sterling-sign", "viruses", "square-person-confined", "user-tie", "long-arrow-down", "tent-arrow-down-to-line", "certificate", "reply-all", "suitcase", "skating", "funnel-dollar", "camera-retro", "circle-arrow-down", "file-import", "square-arrow-up-right", "box-open", "scroll", "spa", "location-pin-lock", "pause", "hill-avalanche", "thermometer-empty", "bomb", "registered", "vcard", "scale-unbalanced-flip", "subscript", "directions", "burst", "laptop-house", "tired", "money-bills", "smog", "crutch", "cloud-upload", "palette", "arrows-turn-right", "vest", "ferry", "arrows-down-to-people", "sprout", "left-right", "boxes-packing", "circle-arrow-left", "group-arrows-rotate", "bowl-food", "candy-cane", "sort-amount-down", "thunderstorm", "text-slash", "smile-wink", "file-word", "file-powerpoint", "arrows-left-right", "house-lock", "cloud-download", "children", "chalkboard", "user-large-slash", "envelope-open", "handshake-simple-slash", "mattress-pillow", "guarani-sign", "sync", "fire-extinguisher", "cruzeiro-sign", "greater-than-equal", "shield-halved", "book-atlas", "virus", "envelope-circle-check", "layer-group", "arrows-to-dot", "archway", "heart-circle-check", "house-damage", "file-zipper", "square", "martini-glass-empty", "couch", "cedi-sign", "italic", "church", "comments-dollar", "democrat", "z", "skiing", "road-lock", "a", "temperature-down", "feather-pointed", "p", "snowflake", "newspaper", "rectangle-ad", "circle-arrow-right", "filter-circle-xmark", "locust", "unsorted", "list-ol", "person-dress-burst", "money-check-dollar", "vector-square", "bread-slice", "language", "kiss-wink-heart", "filter", "question", "file-signature", "up-down-left-right", "house-chimney-user", "hand-holding-heart", "puzzle-piece", "money-check", "star-half-stroke", "code", "whiskey-glass", "building-circle-exclamation", "magnifying-glass-chart", "external-link", "cubes-stacked", "won", "virus-covid", "austral-sign", "f", "leaf", "road", "taxi", "person-circle-plus", "pie-chart", "bolt-lightning", "sack-xmark", "file-excel", "file-contract", "fish-fins", "building-flag", "grin-beam", "object-ungroup", "poop", "map-marker", "kaaba", "toilet-paper", "helmet-safety", "eject", "circle-right", "plane-circle-check", "meh-rolling-eyes", "object-group", "line-chart", "mask-ventilator", "arrow-right", "signs-post", "cash-register", "person-circle-question", "h", "tarp", "tools", "arrows-to-eye", "plug-circle-bolt", "heart", "mars-and-venus", "house-user", "dumpster-fire", "house-crack", "martini-glass-citrus", "surprise", "bottle-water", "pause-circle", "toilet-paper-slash", "apple-whole", "kitchen-set", "r", "thermometer-quarter", "cube", "bitcoin-sign", "shield-dog", "solar-panel", "lock-open", "elevator", "money-bill-transfer", "money-bill-trend-up", "house-flood-water-circle-arrow-right", "square-poll-horizontal", "circle", "fast-backward", "recycle", "user-astronaut", "plane-slash", "trademark", "basketball", "satellite-dish", "circle-up", "mobile-screen-button", "volume-up", "users-rays", "wallet", "clipboard-check", "file-audio", "hamburger", "wrench", "bugs", "rupee", "file-image", "question-circle", "plane-departure", "handshake-slash", "book-bookmark", "code-branch", "hat-cowboy", "bridge", "phone-flip", "truck-front", "cat", "anchor-circle-exclamation", "truck-field", "route", "clipboard-question", "panorama", "comment-medical", "teeth-open", "file-circle-minus", "tags", "wine-glass", "fast", "meh-blank", "square-parking", "house-signal", "tasks-alt", "faucet-drip", "dolly-flatbed", "smoking-ban", "terminal", "mobile-button", "house-medical-flag", "shopping-basket", "tape", "bus-simple", "eye", "sad-cry", "audio-description", "person-military-to-person", "file-shield", "user-slash", "pen", "tower-observation", "file-code", "signal", "bus", "heart-circle-xmark", "house-chimney", "window-maximize", "frown", "prescription", "store-alt", "save", "vihara", "scale-unbalanced", "sort-up", "commenting", "plant-wilt", "diamond", "grin-squint", "hand-holding-usd", "bacterium", "hand-pointer", "drum-steelpan", "hand-scissors", "praying-hands", "redo", "biohazard", "location", "mars-double", "child-dress", "users-between-lines", "lungs-virus", "grin-tears", "phone", "calendar-xmark", "child-reaching", "head-side-virus", "user-gear", "sort-numeric-up", "door-closed", "shield-virus", "dice-six", "mosquito-net", "bridge-water", "person-booth", "text-width", "hat-wizard", "fancy", "person-digging", "trash", "tachometer-average", "book-medical", "poo", "quote-right", "tshirt", "cubes", "divide", "tenge", "headphones", "hands-holding", "hands-clapping", "republican", "arrow-left", "person-circle-xmark", "ruler", "align-left", "dice-d6", "restroom", "j", "users-viewfinder", "file-video", "up-right-from-square", "th", "file-pdf", "book-bible", "o", "suitcase-medical", "user-secret", "otter", "person-dress", "comment-dollar", "business-time", "th-large", "tanakh", "volume-control-phone", "hat-cowboy-side", "clipboard-user", "child", "lira-sign", "satellite", "plane-lock", "tag", "comment", "cake", "envelope", "angles-up", "paperclip", "arrow-right-to-city", "ribbon", "lungs", "sort-numeric-up-alt", "litecoin-sign", "border-none", "circle-nodes", "parachute-box", "indent", "truck-field-un", "hourglass", "mountain", "user-md", "info-circle", "cloud-meatball", "camera", "square-virus", "meteor", "car-on", "sleigh", "sort-numeric-down", "hand-holding-water", "water", "calendar-check", "braille", "prescription-bottle-medical", "landmark", "truck", "crosshairs", "person-cane", "tent", "vest-patches", "check-double", "sort-alpha-down", "money-bill-wheat", "cookie", "undo", "hdd", "grin-squint-tears", "dumbbell", "rectangle-list", "tarp-droplet", "house-medical-circle-check", "skiing-nordic", "calendar-plus", "plane-arrival", "circle-left", "train-subway", "chart-gantt", "inr", "crop-simple", "money-bill-alt", "long-arrow-alt-left", "dna", "virus-slash", "subtract", "chess", "long-arrow-left", "plug-circle-check", "street-view", "franc-sign", "volume-off", "hands-asl-interpreting", "gear", "tint-slash", "mosque", "mosquito", "star-of-david", "person-military-rifle", "shopping-cart", "vials", "plug-circle-plus", "place-of-worship", "grip-vertical", "level-up", "u", "square-root-variable", "clock", "step-backward", "pallet", "faucet", "baseball-bat-ball", "s", "timeline", "keyboard", "caret-down", "house-chimney-medical", "thermometer-three-quarters", "mobile-screen", "plane-up", "piggy-bank", "battery-half", "mountain-city", "coins", "khanda", "sliders", "folder-tree", "network-wired", "map-pin", "hamsa", "cent-sign", "flask", "person-pregnant", "wand-sparkles", "ellipsis-vertical", "ticket", "power-off", "right-long", "flag-usa", "laptop-file", "tty", "diagram-next", "person-rifle", "house-medical-circle-exclamation", "closed-captioning", "person-hiking", "venus-double", "images", "calculator", "people-pulling", "n", "tram", "cloud-rain", "building-circle-xmark", "ship", "arrows-down-to-line", "download", "grin", "delete-left", "eyedropper", "file-circle-check", "forward", "mobile", "meh", "align-center", "book-skull", "id-card", "outdent", "heart-circle-exclamation", "house", "calendar-week", "laptop-medical", "b", "file-medical", "dice-one", "kiwi-bird", "exchange", "rotate-right", "utensils", "sort-amount-up", "mill-sign", "bowl-rice", "skull", "tower-broadcast", "truck-pickup", "up-long", "stop", "code-merge", "upload", "hurricane", "mound", "toilet-portable", "compact-disc", "file-download", "caravan", "shield-cat", "zap", "glass-water", "oil-well", "vault", "mars", "toilet", "plane-circle-xmark", "yen", "ruble", "sun", "guitar", "laugh-wink", "horse-head", "bore-hole", "industry", "circle-down", "arrows-turn-to-dots", "florin-sign", "sort-amount-down-alt", "less-than", "angle-down", "car-tunnel", "head-side-cough", "grip-lines", "thumbs-down", "user-lock", "long-arrow-right", "anchor-circle-xmark", "ellipsis", "chess-pawn", "kit-medical", "person-through-window", "toolbox", "hands-holding-circle", "bug", "credit-card", "car", "hand-holding-hand", "book-reader", "mountain-sun", "arrows-left-right-to-line", "dice-d20", "truck-droplet", "file-circle-xmark", "temperature-up", "medal", "bed", "square-h", "podcast", "thermometer-full", "bell", "superscript", "plug-circle-xmark", "star-of-life", "phone-slash", "paint-roller", "handshake-angle", "map-marker-alt", "file", "greater-than", "swimmer", "arrow-down", "tint", "eraser", "globe-americas", "person-burst", "dove", "battery-empty", "socks", "inbox", "section", "tachometer-alt", "envelope-open-text", "hospital", "wine-bottle", "chess-rook", "stream", "dharmachakra", "hotdog", "person-walking-with-cane", "drum", "ice-cream", "heart-circle-bolt", "fax", "paragraph", "vote-yea", "star-half", "boxes", "link", "ear-listen", "tree-city", "play", "font", "rupiah-sign", "search", "table-tennis", "person-dots-from-line", "trash-restore-alt", "naira-sign", "cart-arrow-down", "walkie-talkie", "file-pen", "receipt", "square-pen", "suitcase-rolling", "person-circle-exclamation", "chevron-down", "battery", "skull-crossbones", "code-compare", "list-ul", "school-lock", "tower-cell", "long-arrow-alt-down", "ranking-star", "chess-king", "person-harassing", "brazilian-real-sign", "landmark-dome", "arrow-up", "tv", "shrimp", "tasks", "jug-detergent", "user-circle", "user-shield", "wind", "car-crash", "y", "snowboarding", "fast", "fish", "user-graduate", "circle-half-stroke", "clapperboard", "radiation-alt", "baseball", "jet-fighter-up", "project-diagram", "copy", "volume-xmark", "hand-sparkles", "grip", "share-square", "child-rifle", "gun", "square-phone", "plus", "expand", "computer", "xmark", "arrows", "chalkboard-user", "peso-sign", "building-shield", "baby", "users-line", "quote-left", "tractor", "trash-restore", "arrow-down-up-lock", "lines-leaning", "ruler-combined", "copyright", "equals", "blender", "teeth", "sheqel", "map", "rocket", "photo-video", "folder-minus", "store", "arrow-trend-up", "plug-circle-minus", "sign", "bezier-curve", "bell-slash", "tablet", "school-flag", "fill", "angle-up", "drumstick-bite", "holly-berry", "chevron-left", "bacteria", "hand-lizard", "notdef", "disease", "briefcase-medical", "genderless", "chevron-right", "retweet", "car-rear", "pump-soap", "video-slash", "battery-quarter", "radio", "carriage-baby", "traffic-light", "thermometer", "vr-cardboard", "hand-middle-finger", "percentage", "truck-moving", "glass-water-droplet", "display", "smile", "thumbtack", "trophy", "pray", "hammer", "hand-peace", "sync-alt", "spinner", "robot", "peace", "gears", "warehouse", "arrow-up-right-dots", "splotch", "grin-hearts", "dice-four", "sim-card", "transgender", "mercury", "level-down", "falling-burst", "award", "ticket-simple", "building", "angles-left", "qrcode", "history", "grin-beam-sweat", "file-export", "shield", "sort-amount-up-alt", "house-medical", "golf-ball", "circle-chevron-left", "house-chimney-window", "pen-nib", "tent-arrow-turn-left", "tents", "wand-magic", "dog", "carrot", "moon", "wine-glass-empty", "cheese", "yin-yang", "music", "code-commit", "temperature-low", "person-biking", "broom", "shield-heart", "gopuram", "globe-oceania", "xmark-square", "hashtag", "up-right-and-down-left-from-center", "oil-can", "t", "hippo", "chart-column", "infinity", "vial-circle-check", "person-arrow-down-to-line", "voicemail", "fan", "person-walking-luggage", "up-down", "cloud-moon-rain", "calendar", "trailer", "haykal", "sd-card", "dragon", "shoe-prints", "plus-circle", "grin-tongue-wink", "hand-holding", "plug-circle-exclamation", "unlink", "clone", "person-walking-arrow-loop-left", "sort-alpha-up-alt", "fire-flame-curved", "tornado", "file-circle-plus", "quran", "anchor", "border-all", "face-angry", "cookie-bite", "arrow-trend-down", "rss", "draw-polygon", "scale-balanced", "tachometer", "shower", "desktop", "m", "th-list", "sms", "book", "user-plus", "check", "battery-three-quarters", "house-circle-check", "angle-left", "diagram-successor", "truck-arrow-right", "arrows-split-up-and-left", "hand-fist", "cloud-moon", "briefcase", "falling", "portrait", "user-tag", "rug", "globe-europe", "luggage-cart", "window-close", "baht-sign", "book-open", "journal-whills", "handcuffs", "warning", "database", "share", "bottle-droplet", "face", "hill-rockslide", "right-left", "paper-plane", "road-circle-exclamation", "dungeon", "align-right", "money-bill-wave-alt", "life-ring", "signing", "calendar-day", "water-ladder", "arrows-v", "grimace", "wheelchair-move", "turn-down", "person-walking-arrow-right", "square-envelope", "dice", "bowling-ball", "brain", "bandage", "calendar-minus", "xmark-circle", "gifts", "hotel", "globe-asia", "id-card-clip", "search-plus", "thumbs-up", "user-clock", "hand-dots", "file-invoice", "window-minimize", "mug-saucer", "brush", "mask", "search-minus", "ruler-vertical", "user-large", "train-tram", "user-nurse", "syringe", "cloud-sun", "stopwatch-20", "square-full", "magnet", "jar", "sticky-note", "bug-slash", "arrow-up-from-water-pump", "bone", "user-injured", "sad-tear", "plane", "tent-arrows-down", "exclamation", "arrows-spin", "print", "turkish-lira", "usd", "x", "search-dollar", "users-gear", "person-military-pointing", "university", "umbrella", "trowel", "d", "stapler", "theater-masks", "kip-sign", "hand-point-left", "handshake-simple", "jet-fighter", "square-share-nodes", "barcode", "plus-minus", "video", "mortar-board", "hand-holding-medical", "person-circle-check", "turn-up"];
 
-function qe(e) {
+function Ie(e) {
     function n() {
         const a = {
             position: "fixed",
             color: "white",
             backgroundColor: e.isError ? "#e52207" : "black",
             width: 300,
             top: 10,
             left: (window.innerWidth - 320) / 2,
             padding: 10
         };
         return t.jsxs("div", {
             style: a,
-            children: [t.jsx(w, {
+            children: [t.jsx(j, {
                 icon: e.isError ? "xmark-circle" : "circle-check",
                 style: {
                     marginRight: 5
                 }
             }), e.text]
         })
     }
     return n()
 }
 
 function Q(e, n = !1) {
     const a = document.createElement("div");
-    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(qe, {
+    a.classList.add("message"), H.createRoot(document.body.appendChild(a)).render(t.jsx(Ie, {
         text: e,
         isError: n
     })), setTimeout(function() {
         a.remove()
     }, 3e3)
 }
 
@@ -140,42 +140,42 @@
                 children: e.children
             })]
         })
     }
     return n()
 }
 
-function Ie(e) {
+function qe(e) {
     return ge(e.data)
 }
 
-function A(e) {
+function B(e) {
     return e.replace("/app/", "/api/")
 }
 
 function F(e) {
     return e.replace("/api/", "/app/")
 }
 
-function q(e, n, a, r) {
-    const c = localStorage.getItem("token");
+function I(e, n, a, r) {
+    const d = localStorage.getItem("token");
     var i = {
         Accept: "application/json"
     };
-    c && (i.Authorization = "Token " + c);
-    const l = A(n);
-    var d = {
+    d && (i.Authorization = "Token " + d);
+    const l = B(n);
+    var c = {
         method: e,
         headers: new Headers(i),
         ajax: 1
     };
-    r && (d.body = r);
+    r && (c.body = r);
     var o = null,
         h = null;
-    fetch(l, d).then(function(s) {
+    fetch(l, c).then(function(s) {
         if (o = s, h = o.headers.get("Content-Type"), h == "application/json") return s.text();
         if (h.indexOf("text") < 0 || h.indexOf("csv") >= 0) return s.arrayBuffer();
         s.text()
     }).then(s => {
         if (h == "application/json") {
             var m = JSON.parse(s || "{}");
             typeof m == "object" && m.type == "redirect" ? document.location.href = F(m.url) : a && a(m, o)
@@ -192,41 +192,41 @@
 function ge(e) {
     e.store && Object.keys(e.store).map(function(n) {
         e.store[n] ? localStorage.setItem(n, e.store[n]) : localStorage.removeItem(n, e.store[n])
     }), e.redirect ? (e.message && localStorage.setItem("message", e.message), document.location.href = F(e.redirect)) : e.message && Q(e.message)
 }
 
 function xe() {
-    document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Be, {}))
+    document.querySelector(".layer") == null && H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Le, {}))
 }
 
 function ye(e, n) {
     fe(), xe(), window.reloader = n;
     for (var a = document.getElementsByTagName("dialog"), r = 0; r < a.length; r++) a[r].style.display = "none";
-    H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ae, {
-        url: A(e)
+    H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Be, {
+        url: B(e)
     }))
 }
 
 function De(e) {
-    fe(), xe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Le, {
-        url: A(e)
+    fe(), xe(), H.createRoot(document.body.appendChild(document.createElement("div"))).render(t.jsx(Ae, {
+        url: B(e)
     }))
 }
 
 function U(e) {
     e != null && showMessage(e);
     for (var n = document.getElementsByTagName("dialog"), a = 0; a < n.length; a++)
         if (a == n.length - 1) {
             var r = n[a];
             r.close(), r.classList.remove("opened"), r.remove(), a == 0 ? (document.querySelector(".layer").style.display = "none", window.reloader && window.reloader()) : n[a - 1].style.display = "block"
         }
 }
 
-function Be(e) {
+function Le(e) {
     const n = {
         backgroundColor: "black",
         bottom: 0,
         left: 0,
         position: "fixed",
         right: 0,
         top: 0,
@@ -238,86 +238,86 @@
         onClick: function() {
             U()
         },
         style: n
     })
 }
 
-function Ae(e) {
-    const [n, a] = S.useState(null), [r, c] = S.useState(0);
+function Be(e) {
+    const [n, a] = S.useState(null), [r, d] = S.useState(0);
     S.useEffect(() => {
-        i(A(e.url)), document.querySelector(".layer").style.display = "block"
+        i(B(e.url)), document.querySelector(".layer").style.display = "block"
     }, []);
 
     function i(o) {
-        q("GET", A(o), function(h) {
-            a(h), c(r + 1)
+        I("GET", B(o), function(h) {
+            a(h), d(r + 1)
         })
     }
 
     function l() {
         const o = {
             textAlign: "right",
             cursor: "pointer"
         };
         if (n) return t.jsxs("div", {
             children: [t.jsx("div", {
                 style: o,
-                children: t.jsx(w, {
+                children: t.jsx(j, {
                     icon: "x",
                     onClick: () => U()
                 })
             }), t.jsx(y, {
                 data: n
             })]
         })
     }
-    const d = {
+    const c = {
         minWidth: "50%",
         display: n ? "block" : "none",
         maxWidth: "90%",
         top: window.scrollY + 40
     };
     return t.jsx("dialog", {
-        style: d,
+        style: c,
         children: l()
     }, r)
 }
 
-function Le(e) {
+function Ae(e) {
     var n = Math.random();
     S.useEffect(() => {
         document.querySelector(".layer").style.display = "block";
         var r = document.getElementById(n);
         r.style.top = document.documentElement.scrollTop + 100
     }, []);
 
     function a() {
         const r = {
                 minWidth: "50%",
                 display: "block",
                 maxWidth: "90%",
                 top: window.scrollY + 40
             },
-            c = {
+            d = {
                 float: "right",
                 cursor: "pointer",
                 marginTop: -20
             };
         return t.jsxs("dialog", {
             style: r,
             id: n,
             children: [t.jsx("div", {
-                style: c,
-                children: t.jsx(w, {
+                style: d,
+                children: t.jsx(j, {
                     icon: "x",
                     onClick: () => U()
                 })
             }), t.jsx("iframe", {
-                src: A(e.url),
+                src: B(e.url),
                 width: "100%",
                 height: 500,
                 style: {
                     border: 0
                 }
             })]
         })
@@ -332,29 +332,29 @@
 }
 
 function D({
     id: e,
     onClick: n,
     icon: a,
     label: r,
-    display: c,
+    display: d,
     primary: i,
     compact: l,
-    spin: d
+    spin: c
 }) {
     function o() {
-        return a ? l || !r ? t.jsx(w, {
+        return a ? l || !r ? t.jsx(j, {
             icon: a
         }) : t.jsxs(t.Fragment, {
             children: [t.jsx(Ee, {
                 style: {
                     marginRight: 10,
                     display: "none"
                 }
-            }), t.jsx(w, {
+            }), t.jsx(j, {
                 icon: a,
                 style: {
                     marginRight: 10
                 }
             }), r || ""]
         }) : r
     }
@@ -363,91 +363,91 @@
         const s = {
             padding: 12,
             textDecoration: "none",
             whiteSpace: "nowrap",
             borderRadius: 5,
             margin: 5,
             cursor: "pointer",
-            display: c || "block",
+            display: d || "block",
             width: "fit-content",
             textWrap: "nowrap"
         };
         return i ? (s.backgroundColor = "#1351b4", s.color = "white") : (s.border = "solid 1px #1351b4", s.color = "#1351b4"), t.jsx("a", {
             id: e,
             style: s,
-            "data-label": k(r || a),
+            "data-label": b(r || a),
             onClick: m => {
-                m.preventDefault(), a && d && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
+                m.preventDefault(), a && c && (m.target.dataset.spinning = a, m.target.querySelector("i.fa-spin").style.display = "inline-block", m.target.querySelector("i.fa-" + a).style.display = "none"), n(m)
             },
             children: o()
         })
     }
     return h()
 }
 
 function O(e) {
     const n = e.id || Math.random(),
         [a, r] = S.useState(e.data.name);
 
-    function c(d) {
-        d.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(d)) : e.data.modal == !1 ? window.load(F(e.data.url)) : ye(e.data.url)
+    function d(c) {
+        c.preventDefault(), e.onClick ? (a && r("Aguarde...."), e.onClick(c)) : e.data.modal == !1 ? window.load(F(e.data.url)) : ye(e.data.url)
     }
 
     function i() {
-        return e.data.icon ? e.compact || !e.data.name ? t.jsx(w, {
+        return e.data.icon ? e.compact || !e.data.name ? t.jsx(j, {
             icon: e.data.icon
         }) : t.jsxs(t.Fragment, {
-            children: [t.jsx(w, {
+            children: [t.jsx(j, {
                 icon: e.data.icon,
                 style: {
                     paddingRight: 10
                 }
             }), e.data.name || ""]
         }) : e.data.name
     }
 
     function l() {
-        var d = {
+        var c = {
             padding: 12,
             textDecoration: "none",
             borderRadius: 5,
             margin: 5
         };
-        return e.primary && (d.backgroundColor = "#1351b4", d.color = "white"), e.default && (d.border = "solid 1px #1351b4", d.color = "#1351b4"), e.style && Object.keys(e.style).map(function(o) {
-            d[o] = e.style[o]
+        return e.primary && (c.backgroundColor = "#1351b4", c.color = "white"), e.default && (c.border = "solid 1px #1351b4", c.color = "#1351b4"), e.style && Object.keys(e.style).map(function(o) {
+            c[o] = e.style[o]
         }), t.jsx("a", {
             id: n,
             href: F(e.data.url) || "#",
-            onClick: c,
-            style: d,
-            "data-label": k(e.data.name),
+            onClick: d,
+            style: c,
+            "data-label": b(e.data.name),
             children: i()
         })
     }
     return l()
 }
 
 function $(e) {
     function n(i) {
         var l = i.target.parentNode.querySelector(".dropdown");
         return l == null && (l = i.target.parentNode.parentNode.querySelector(".dropdown")), l == null && (l = i.target.parentNode.parentNode.parentNode.querySelector(".dropdown")), l
     }
 
     function a(i) {
         const l = i.target.getBoundingClientRect(),
-            d = n(i);
-        document.querySelectorAll(".dropdown").forEach(o => o.style.display = "none"), d.style.left = l.left - 150 + l.width + "px", d.style.display = "block"
+            c = n(i);
+        document.querySelectorAll(".dropdown").forEach(o => o.style.display = "none"), c.style.left = l.left - 150 + l.width + "px", c.style.display = "block"
     }
 
     function r(i) {
         const l = n(i);
         l.style.display = "none"
     }
 
-    function c() {
+    function d() {
         const i = {
                 padding: 0,
                 position: "absolute",
                 width: 150,
                 left: 0,
                 textAlign: "center",
                 backgroundColor: "white",
@@ -460,33 +460,33 @@
             };
         return t.jsxs(t.Fragment, {
             children: [t.jsx("div", {
                 onClick: a,
                 style: {
                     cursor: "pointer"
                 },
-                "data-label": k(e.dataLabel),
+                "data-label": b(e.dataLabel),
                 children: e.children
             }), e.actions && e.actions.length > 0 && t.jsx("ul", {
                 style: i,
                 onMouseLeave: r,
                 className: "dropdown",
-                children: e.actions.map(d => t.jsx("li", {
+                children: e.actions.map(c => t.jsx("li", {
                     style: l,
                     children: t.jsx(O, {
-                        data: d,
+                        data: c,
                         style: {
                             padding: 0
                         }
                     })
                 }, Math.random()))
             })]
         })
     }
-    return c()
+    return d()
 }
 const Oe = ["text", "password", "email", "number", "date", "datetime-local", "file", "image", "range", "search", "tel", "time", "url", "week", "hidden", "color"],
     V = {
         padding: 15,
         border: "solid 1px #CCC",
         borderRadius: 5
     };
@@ -497,15 +497,15 @@
         for (var n = 0; n < a.length; n++)
             if (e.toLowerCase().indexOf(a[n]) > 0) return !0
     }
 }
 
 function pe(e, n) {
     var a = new FormData(e);
-    q("POST", n, ze, a)
+    I("POST", n, ze, a)
 }
 
 function Re(e) {
     if (e) {
         var n = document.querySelector(".form-fieldset." + e);
         n && (n.style.display = "none");
         var a = document.querySelector(".form-group." + e);
@@ -529,17 +529,17 @@
     else if (r.tagName == "SELECT") {
         if (r.style.display != "none") r.dispatchEvent(new CustomEvent("customchange", {
             detail: {
                 value: n
             }
         }));
         else
-            for (var c = 0; c < r.options.length; c++)
-                if (r.options[c].value == n) {
-                    r.selectedIndex = c;
+            for (var d = 0; d < r.options.length; d++)
+                if (r.options[d].value == n) {
+                    r.selectedIndex = d;
                     break
                 }
     }
 }
 
 function ze(e) {
     if (e) {
@@ -559,15 +559,15 @@
             justifyContent: "space-between",
             marginTop: 10,
             marginBottom: 10
         };
         return t.jsxs("div", {
             style: a,
             children: [t.jsxs("div", {
-                children: [t.jsx(w, {
+                children: [t.jsx(j, {
                     icon: "circle-check",
                     style: {
                         color: "#155bcb",
                         marginRight: 20
                     }
                 }), e.data.text]
             }), e.children && t.jsx("div", {
@@ -587,15 +587,15 @@
             marginTop: 2,
             marginBottom: 2,
             padding: 8
         };
         return t.jsxs("div", {
             style: a,
             id: e.id,
-            children: [t.jsx(w, {
+            children: [t.jsx(j, {
                 icon: "xmark-circle",
                 style: {
                     marginRight: 5
                 }
             }), t.jsx("span", {})]
         })
     }
@@ -619,21 +619,21 @@
     return n()
 }
 
 function Y(e) {
     const n = e.data.name + Math.random();
 
     function a() {
-        const d = {
+        const c = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
         return e.data.action && (e.data.action.modal = !0), t.jsxs("div", {
-            style: d,
+            style: c,
             children: [t.jsx("label", {
                 className: e.data.required ? "bold" : "",
                 children: e.data.label
             }), e.data.action && t.jsx(O, {
                 data: e.data.action,
                 style: {
                     padding: 0
@@ -664,124 +664,124 @@
         }) : e.data.type == "textarea" ? t.jsx(Ge, {
             data: e.data
         }) : t.jsx("span", {
             children: e.data.name
         })
     }
 
-    function c() {
+    function d() {
         return t.jsx("div", {
             children: t.jsx(Pe, {
                 id: e.data.name + "_error"
             })
         })
     }
 
     function i() {
         return e.data.help_text && t.jsx(We, {
             text: e.data.help_text
         })
     }
 
     function l() {
-        const d = {
+        const c = {
             display: e.data.type == "hidden" ? "none" : "flex",
             flexDirection: "column",
             padding: 5
         };
         return t.jsxs("div", {
             id: n,
             className: "form-group " + e.data.name,
-            style: d,
-            children: [a(), r(), i(), c()]
+            style: c,
+            children: [a(), r(), i(), d()]
         })
     }
     return l()
 }
 
 function ce(e) {
     var n = "";
     const a = e.data.name + Math.random();
     e.data.mask == "decimal" && (n = "decimal", e.data.value && (e.data.value = Math.round(parseFloat(e.data.value)).toFixed(2).replace(".", ","))), S.useEffect(() => {
         function l(h, s, m) {
             var x = m.target,
                 v = x.value.replace(/\D/g, ""),
-                j = x.value.length > s ? 1 : 0;
-            VMasker(x).unMask(), VMasker(x).maskPattern(h[j]), x.value = VMasker.toPattern(v, h[j])
+                k = x.value.length > s ? 1 : 0;
+            VMasker(x).unMask(), VMasker(x).maskPattern(h[k]), x.value = VMasker.toPattern(v, h[k])
         }
         if (e.data.mask) {
-            var d = document.getElementById(a);
-            if (e.data.mask == "decimal") VMasker(d).maskMoney({
+            var c = document.getElementById(a);
+            if (e.data.mask == "decimal") VMasker(c).maskMoney({
                 precision: 2,
                 separator: ",",
                 delimiter: "."
             });
             else if (e.data.mask.indexOf("|") > 0) {
                 var o = e.data.mask.split("|");
-                VMasker(d).maskPattern(o[0]), d.addEventListener("input", l.bind(void 0, o, 14), !1)
-            } else VMasker(d).maskPattern(e.data.mask)
+                VMasker(c).maskPattern(o[0]), c.addEventListener("input", l.bind(void 0, o, 14), !1)
+            } else VMasker(c).maskPattern(e.data.mask)
         }
     }, []);
 
     function r(l) {
         pe(l.target.closest("form"), e.data.onchange)
     }
 
-    function c(l) {
+    function d(l) {
         if (e.data.type == "file" && l.target.files) {
             let o = l.target.files[0];
-            var d = new FileReader;
-            d.onload = function(h) {
+            var c = new FileReader;
+            c.onload = function(h) {
                 if (te(o.name)) {
                     const v = "display" + a;
                     var s = document.createElement("img");
-                    s.id = l.target.id + "img", s.style.width = "200px", s.style.display = "block", s.style.margin = "auto", s.style.marginTop = "20px", s.onload = function(j) {
-                        const I = e.data.width > e.data.height ? e.data.width / s.width : e.data.height / s.height;
+                    s.id = l.target.id + "img", s.style.width = "200px", s.style.display = "block", s.style.margin = "auto", s.style.marginTop = "20px", s.onload = function(k) {
+                        const q = e.data.width > e.data.height ? e.data.width / s.width : e.data.height / s.height;
                         var C = document.createElement("canvas");
-                        const M = C.getContext("2d");
+                        const E = C.getContext("2d");
                         C.height = C.width * (s.height / s.width);
-                        const E = document.createElement("canvas"),
-                            P = E.getContext("2d");
-                        E.width = s.width * I, E.height = s.height * I, P.drawImage(s, 0, 0, E.width, E.height), M.drawImage(E, 0, 0, E.width * I, E.height * I, 0, 0, C.width, C.height), E.toBlob(function(g) {
+                        const T = document.createElement("canvas"),
+                            P = T.getContext("2d");
+                        T.width = s.width * q, T.height = s.height * q, P.drawImage(s, 0, 0, T.width, T.height), E.drawImage(T, 0, 0, T.width * q, T.height * q, 0, 0, C.width, C.height), T.toBlob(function(g) {
                             const f = new DataTransfer;
                             f.items.add(new File([g], o.name)), l.target.files = f.files
                         });
                         var u = document.getElementById(v);
                         u == null ? (u = document.createElement("div"), u.id = v) : u.removeChild(u.childNodes[0]), u.appendChild(s), l.target.parentNode.appendChild(u)
                     }, s.src = h.target.result
                 }
                 const m = document.getElementById("fileinfo" + a);
                 var x = o.size / 1024;
                 x < 1024 ? x = parseInt(x) + " Kb" : x = (x / 1024).toFixed(2) + " Mb", m.innerHTML = o.name + " / " + x, e.data.max_size && o.size / 1024 / 1024 > e.data.max_size && alert("O limite de tamanho é " + e.data.max_size + "Mb. O arquivo informado possui " + x + ". Por favor, adicione um arquivo menor.")
-            }, d.readAsDataURL(o)
+            }, c.readAsDataURL(o)
         }
     }
 
     function i() {
         var l = e.data.type;
         if (l == "datetime" && (l = "datetime-regional"), l == "decimal" && (l = "text"), l == "file") {
             const h = {
                 alignContent: "center",
                 height: 75,
                 padding: 30,
                 maxWidth: "100%"
             };
-            var d = null;
-            return e.data.extensions && e.data.extensions.length > 0 && (d = e.data.extensions.map(s => "." + s).join(", ")), t.jsxs(t.Fragment, {
+            var c = null;
+            return e.data.extensions && e.data.extensions.length > 0 && (c = e.data.extensions.map(s => "." + s).join(", ")), t.jsxs(t.Fragment, {
                 children: [t.jsxs("div", {
                     style: {
                         display: "flex",
                         justifyContent: "space-between",
                         backgroundColor: "rgba(15, 145, 210, 0.05)",
                         border: "1px dashed rgba(15, 145, 210, 0.4)",
                         borderRadius: 10
                     },
                     children: [t.jsx("div", {
                         style: h,
-                        children: t.jsx(w, {
+                        children: t.jsx(j, {
                             icon: "cloud-upload",
                             style: {
                                 fontSize: "2.5rem",
                                 color: "#1351b4"
                             }
                         })
                     }), t.jsxs("div", {
@@ -812,38 +812,39 @@
                         })
                     })]
                 }), t.jsx("input", {
                     className: "form-control " + n,
                     type: l,
                     name: e.data.name,
                     id: a,
-                    "data-label": k(e.data.label),
+                    "data-label": b(e.data.label),
                     readOnly: e.data.read_only,
                     onBlur: e.data.onchange ? r : null,
-                    onChange: c,
+                    onChange: d,
                     style: {
-                        display: "none"
+                        zIndex: "-1",
+                        marginTop: -20
                     },
-                    accept: d
+                    accept: c
                 })]
             })
         } else {
             var o = V;
             return l == "color" && (o = {
                 ...V
             }, o.width = "100%", o.backgroundColor = "white", o.height = 47.5), t.jsx("input", {
                 className: "form-control " + n,
                 type: l,
                 name: e.data.name,
                 id: a,
                 defaultValue: e.data.value,
-                "data-label": k(e.data.label),
+                "data-label": b(e.data.label),
                 readOnly: e.data.read_only,
                 onBlur: e.data.onchange ? r : null,
-                onChange: c,
+                onChange: d,
                 style: o
             })
         }
     }
     return i()
 }
 
@@ -856,74 +857,74 @@
         })
     }) : e.data.value != null && n.push({
         id: e.data.value.id,
         value: e.data.value.label
     }), e.data.id == null && (e.data.id = Math.random()), e.data.id2 == null && (e.data.id2 = e.data.id + "__autocomplete");
     const a = e.data.id,
         r = e.data.id2,
-        c = Array.isArray(e.data.value),
+        d = Array.isArray(e.data.value),
         [i, l] = S.useState(!1),
-        [d, o] = S.useState(null);
+        [c, o] = S.useState(null);
     var h = !1;
     S.useEffect(() => {
-        M(n), document.getElementById(a).addEventListener("customchange", function(u) {
-            M(u.detail.value), reactTriggerChange(document.getElementById(e.data.name))
+        E(n), document.getElementById(a).addEventListener("customchange", function(u) {
+            E(u.detail.value), reactTriggerChange(document.getElementById(e.data.name))
         })
     }, []);
 
     function s() {
         const u = document.getElementById(a);
-        if (c) {
+        if (d) {
             const g = {
                     padding: 5,
                     display: "inline"
                 },
                 f = {
                     cursor: "pointer",
                     marginRight: 5
                 },
                 p = {
                     fontSize: "0.8rem"
                 };
             return t.jsxs("div", {
-                children: [u == null && n.map((b, L) => t.jsxs("div", {
+                children: [u == null && n.map((w, A) => t.jsxs("div", {
                     style: g,
                     children: [t.jsx("span", {
-                        onClick: () => E(L),
+                        onClick: () => T(A),
                         style: f,
-                        children: t.jsx(w, {
+                        children: t.jsx(j, {
                             icon: "trash-can",
                             style: p
                         })
-                    }), b.value]
-                }, Math.random())), u != null && Array.from(u.options).map((b, L) => t.jsxs("div", {
+                    }), w.value]
+                }, Math.random())), u != null && Array.from(u.options).map((w, A) => t.jsxs("div", {
                     style: g,
                     children: [t.jsx("span", {
-                        onClick: () => E(L),
+                        onClick: () => T(A),
                         style: f,
-                        children: t.jsx(w, {
+                        children: t.jsx(j, {
                             icon: "trash-can",
                             style: p
                         })
-                    }), b.innerHTML]
+                    }), w.innerHTML]
                 }, Math.random()))]
             })
         }
     }
 
     function m(u) {
         o([])
     }
 
     function x() {
         return t.jsx("select", {
             onChange: m,
             id: a,
             name: e.data.name,
-            multiple: c,
+            multiple: d,
             readOnly: !0,
             style: {
                 display: "contents"
             }
         })
     }
 
@@ -940,93 +941,96 @@
                 borderRadius: 5,
                 maxHeight: 150,
                 overflowY: "auto"
             };
         g.position = "absolute", g.backgroundColor = "white";
         const f = document.getElementById(r);
         if (f) {
-            let T = null,
+            let M = null,
                 _ = f,
                 W = null;
             for (; !W && (_ = _.parentElement) instanceof HTMLElement;) _.matches("dialog") && (W = _);
-            T = W;
+            M = W;
             const N = f.getBoundingClientRect();
             var p = N.top + N.height,
-                b = N.left;
-            if (T) {
-                const J = T.getBoundingClientRect();
-                p = p - J.top, b = b - J.left
-            } else p += window.scrollY, b += window.scrollX;
-            g.width = N.width, g.top = p, g.left = b
+                w = N.left;
+            if (M) {
+                const J = M.getBoundingClientRect();
+                p = p - J.top, w = w - J.left
+            } else p += window.scrollY, w += window.scrollX;
+            g.width = N.width, g.top = p, g.left = w
         }
-        const L = {
+        const A = {
                 cursor: "pointer",
                 padding: 10
             },
-            Z = !c && n.length > 0 && n[0].value || "";
+            Z = !d && n.length > 0 && n[0].value || "";
         return t.jsxs(t.Fragment, {
             children: [t.jsx("input", {
                 id: r,
                 name: e.data.name + "__autocomplete",
                 type: "text",
                 className: "form-control",
-                onFocus: T => {
-                    T.target.select(), C(T)
+                onFocus: M => {
+                    M.target.select(), C(M)
                 },
                 onChange: C,
-                onMouseLeave: j,
-                onBlur: j,
+                onMouseLeave: k,
+                onBlur: k,
                 defaultValue: Z,
-                style: u
-            }), d && i && t.jsxs("ul", {
+                style: u,
+                "data-label": b(e.data.label)
+            }), c && i && t.jsxs("ul", {
                 style: g,
-                onMouseLeave: I,
-                onMouseEnter: function(T) {
+                onMouseLeave: q,
+                onMouseEnter: function(M) {
                     h = !0
                 },
-                children: [d.length == 0 && t.jsx("li", {
-                    style: L,
+                children: [c.length == 0 && t.jsx("li", {
+                    style: A,
                     children: "Nenhuma opção encontrada."
-                }), d.map(T => t.jsx("li", {
+                }), c.map(M => t.jsx("li", {
                     onClick: () => {
-                        l(!1), e.onSelect ? e.onSelect(T) : M(T)
+                        l(!1), e.onSelect ? e.onSelect(M) : E(M)
                     },
-                    style: L,
-                    children: T.value
+                    style: A,
+                    className: "autocomplete-item",
+                    "data-label": b(M.value),
+                    children: M.value
                 }, Math.random()))]
             })]
         })
     }
 
-    function j(u) {
+    function k(u) {
         h = !1, setTimeout(function() {
-            I(u)
+            q(u)
         }, 250)
     }
 
-    function I(u) {
+    function q(u) {
         const g = document.getElementById(a),
             f = document.getElementById(r);
-        c || g.options.length > 0 && f.value != g.options[0].innerHTML && (g.innerHTML = "", f.value = "", l(!1)), u.target.tagName == "UL" ? l(!1) : h || l(!1)
+        d || g.options.length > 0 && f.value != g.options[0].innerHTML && (g.innerHTML = "", f.value = "", l(!1)), u.target.tagName == "UL" ? l(!1) : h || l(!1)
     }
 
     function C(u) {
         const g = e.data.choices.indexOf("?") < 0 ? "?" : "&";
-        l(!0), q("GET", e.data.choices + g + "term=" + u.target.value, function(p) {
+        l(!0), I("GET", e.data.choices + g + "term=" + u.target.value, function(p) {
             o(p)
         })
     }
 
-    function M(u) {
+    function E(u) {
         const g = document.getElementById(a),
             f = document.getElementById(r);
-        g.innerHTML == null && (g.innerHTML = ""), Array.isArray(u) ? g.innerHTML = u.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : c ? (g.innerHTML += `<option selected value="${u.id}">${u.value}</option>`, f.value = "") : (g.innerHTML = `<option selected value="${u.id}">${u.value}</option>`, f.value = u.value), e.data.onchange && pe(f.closest("form"), e.data.onchange)
+        g.innerHTML == null && (g.innerHTML = ""), Array.isArray(u) ? g.innerHTML = u.map(p => `<option selected value="${p.id}">${p.value}</option>`).join("") : d ? (g.innerHTML += `<option selected value="${u.id}">${u.value}</option>`, f.value = "") : (g.innerHTML = `<option selected value="${u.id}">${u.value}</option>`, f.value = u.value), e.data.onchange && pe(f.closest("form"), e.data.onchange)
     }
 
-    function E(u) {
+    function T(u) {
         const g = document.getElementById(a);
         var f = Array.from(g.options);
         g.innerHTML = f.slice(0, u).concat(f.slice(u + 1)).map(p => `<option selected value="${p.value}">${p.innerHTML}</option>`).join(""), o([])
     }
 
     function P() {
         return t.jsxs(t.Fragment, {
@@ -1040,15 +1044,15 @@
     function n() {
         var a = {
             ...V
         };
         return a.height = 100, t.jsx("textarea", {
             id: e.data.name,
             name: e.data.name,
-            "data-label": k(e.data.label),
+            "data-label": b(e.data.label),
             style: a,
             defaultValue: e.data.value || ""
         })
     }
     return n()
 }
 
@@ -1065,104 +1069,104 @@
     })
 }
 
 function ne(e) {
     var n = Math.random(),
         a = e.data;
 
-    function r(d) {
-        return a.value != null ? a.value == d.id ? !0 : a.value.id == d.id : !1
+    function r(c) {
+        return a.value != null ? a.value == c.id ? !0 : a.value.id == c.id : !1
     }
 
-    function c(d) {
-        var o = document.getElementById(d);
+    function d(c) {
+        var o = document.getElementById(c);
         a.checked && (o.checked = !1)
     }
 
-    function i(d) {
-        var o = document.getElementById(d);
+    function i(c) {
+        var o = document.getElementById(c);
         a.checked = o.checked
     }
 
     function l() {
         return t.jsx("div", {
             className: "radio-group",
-            children: a.choices.map((d, o) => t.jsxs("div", {
+            children: a.choices.map((c, o) => t.jsxs("div", {
                 style: {
                     paddingTop: 10
                 },
                 children: [t.jsx("input", {
                     id: a.name + n + o,
                     type: "radio",
                     name: a.name,
-                    defaultValue: d.id,
-                    defaultChecked: r(d),
-                    "data-label": k(d.value),
+                    defaultValue: c.id,
+                    defaultChecked: r(c),
+                    "data-label": b(c.value),
                     onClick: function() {
-                        c(a.name + n + o)
+                        d(a.name + n + o)
                     },
                     onMouseEnter: function() {
                         i(a.name + n + o)
                     }
                 }), t.jsx("label", {
                     htmlFor: a.name + n + o,
-                    children: d.value
+                    children: c.value
                 })]
             }, n + o))
         })
     }
     return l()
 }
 
 function ue(e) {
     var n = Math.random(),
         a = e.data;
 
     function r(i) {
         var l = !1;
         if (a.value)
-            for (var d = 0; d < a.value.length; d++) {
-                var o = a.value[d];
+            for (var c = 0; c < a.value.length; c++) {
+                var o = a.value[c];
                 (o == i.id || o.id == i.id) && (l = !0)
             }
         return l
     }
 
-    function c() {
+    function d() {
         return t.jsx("div", {
             className: "checkbox-group",
             children: a.choices.map((i, l) => t.jsxs("div", {
                 style: {
                     paddingTop: 10
                 },
                 children: [t.jsx("input", {
                     id: a.name + n + l,
                     type: "checkbox",
                     name: a.name,
                     defaultValue: i.id,
                     defaultChecked: r(i),
-                    "data-label": k(i.value)
+                    "data-label": b(i.value)
                 }), t.jsx("label", {
                     htmlFor: a.name + n + l,
                     children: i.value
                 })]
             }, n + l))
         })
     }
-    return c()
+    return d()
 }
 
 function Ve(e) {
     var n = e.data;
     return t.jsx(t.Fragment, {
         children: t.jsx("select", {
             className: "form-control",
             id: n.name,
             name: n.name,
-            "data-label": k(n.label),
+            "data-label": b(n.label),
             defaultValue: n.value,
             style: V,
             children: n.choices.map(a => t.jsx("option", {
                 value: a.id,
                 children: a.value
             }, Math.random()))
         })
@@ -1170,15 +1174,15 @@
 }
 
 function Je(e) {
     const n = Math.random(),
         a = e.data.value[0],
         r = a.fields ? a.fields[0] : a.fieldsets[0].fields[0][0];
 
-    function c() {
+    function d() {
         return !e.data.required && t.jsx("div", {
             id: "info-" + n,
             children: t.jsxs(ie, {
                 data: {
                     text: "Esta informação é opcional. Controle seu preenchimento com o botão ao lado."
                 },
                 children: [t.jsx(D, {
@@ -1218,28 +1222,28 @@
                 return t.jsx(le, {
                     data: h
                 }, Math.random())
             })
         })
     }
 
-    function d() {
+    function c() {
         const o = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: o,
-                "data-label": k(e.data.label),
+                "data-label": b(e.data.label),
                 children: e.data.label
-            }), c(), l()]
+            }), d(), l()]
         })
     }
-    return d()
+    return c()
 }
 
 function $e(e) {
     var n = 0;
     const a = Math.random();
     e.data.template == null && (e.data.template = e.data.value.pop());
 
@@ -1270,50 +1274,50 @@
                     onClick: () => l(x),
                     display: "inline"
                 })]
             })]
         }, Math.random())
     }
 
-    function c() {
-        const s = d(),
+    function d() {
+        const s = c(),
             m = s.length > 0 ? "none" : "inline";
         document.getElementById("add-" + a).style.display = m;
         for (var x = 0; x < n; x++) {
             var v = document.getElementById("extra-add-" + x + "-");
             v.style.display = "none"
         }
         if (s.length > 0) {
             var v = document.getElementById("extra-add-" + s[s.length - 1] + "-");
             v.style.display = "inline"
         }
     }
 
     function i() {
-        c();
+        d();
         var s = JSON.parse(JSON.stringify(e.data.template));
         s.fields ? (s.fields.map(function(m) {
             m.name = m.name.replace("__n__", "__" + n + "__")
         }), s.fields[0].value = 0) : s.fieldsets.map(function(m) {
             m.fields.map(function(x) {
                 x.map(function(v) {
                     v.name = v.name.replace("__n__", "__" + n + "__")
                 }), x[0].value = 0
             })
-        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(s, "inline")), setTimeout(c, 100)
+        }), H.createRoot(document.getElementById(a).appendChild(document.createElement("div"))).render(r(s, "inline")), setTimeout(d, 100)
     }
 
     function l(s) {
         const m = e.data.template,
             v = (m.fields ? m.fields[0] : m.fieldsets[0].fields[0][0]).name.replace("__n__", "__" + s + "__"),
-            j = document.querySelector("input[name=" + v + "]");
-        parseInt(j.value) == 0 ? j.value = "" : j.value = -parseInt(j.value), document.getElementById("form-" + s + "-" + a).style.display = "none", c()
+            k = document.querySelector("input[name=" + v + "]");
+        parseInt(k.value) == 0 ? k.value = "" : k.value = -parseInt(k.value), document.getElementById("form-" + s + "-" + a).style.display = "none", d()
     }
 
-    function d() {
+    function c() {
         for (var s = [], m = 0; m < n; m++) document.getElementById("form-" + m + "-" + a).style.display == "block" && s.push(m);
         return s
     }
 
     function o() {
         return t.jsx("div", {
             id: "info-" + a,
@@ -1336,15 +1340,15 @@
         const s = {
             margin: 0
         };
         return t.jsxs("div", {
             className: "form-fieldset",
             children: [t.jsx("h2", {
                 style: s,
-                "data-label": k(e.data.label),
+                "data-label": b(e.data.label),
                 children: e.data.label
             }), t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 id: a,
                 className: "fieldset-inline-forms",
                 children: [o(), e.data.value.map(function(m, x) {
@@ -1371,25 +1375,25 @@
         return e.data.fields ? t.jsx("div", {
             className: "form-fields",
             children: e.data.fields.map(r => n(r))
         }) : e.data.fieldsets.map(r => t.jsx("div", {
             className: "form-fieldset",
             children: r.type == "inline" ? n(r) : t.jsxs(t.Fragment, {
                 children: [t.jsx("h2", {
-                    "data-label": k(r.title),
+                    "data-label": b(r.title),
                     style: {
                         margin: 0
                     },
                     children: r.title
                 }), t.jsx("div", {
                     className: "fieldset-fields",
-                    children: r.fields.map(c => t.jsx("div", {
-                        children: c.map(i => t.jsx("div", {
+                    children: r.fields.map(d => t.jsx("div", {
+                        children: d.map(i => t.jsx("div", {
                             style: {
-                                width: 100 / c.length + "%",
+                                width: 100 / d.length + "%",
                                 display: i.type == "hidden" ? "none" : "inline-block"
                             },
                             children: n(i)
                         }, Math.random()))
                     }, Math.random()))
                 })]
             })
@@ -1416,15 +1420,15 @@
         return e.data.info && t.jsx(He, {
             data: {
                 text: e.data.info
             }
         })
     }
 
-    function c() {
+    function d() {
         if (e.data.display) return t.jsxs(t.Fragment, {
             children: [e.data.display.map(s => t.jsx(y, {
                 data: s
             }, Math.random())), t.jsx("div", {
                 style: {
                     marginTop: 30
                 }
@@ -1456,55 +1460,55 @@
                 display: "inline",
                 icon: "chevron-right",
                 spin: !0
             })]
         })
     }
 
-    function d() {
+    function c() {
         return t.jsxs("form", {
             id: n,
             action: e.data.url,
             style: {
                 margin: "auto",
                 width: e.data.width,
                 backgroundColor: "white"
             },
             children: [t.jsx("div", {
                 children: !1
             }), t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [a(), r(), c(), i(), l()]
+                children: [a(), r(), d(), i(), l()]
             })]
         })
     }
 
     function o() {
         U()
     }
 
     function h(s) {
         s.preventDefault();
         var m = document.getElementById(n),
             x = new FormData(m);
-        q("POST", e.data.url, function(j) {
-            if (s.target.dataset.spinning && (s.target.querySelector("i.fa-spin").style.display = "none", s.target.querySelector("i.fa-" + s.target.dataset.spinning).style.display = "inline-block"), j.type == "response") return U(), Ne(), ge(j);
-            var I = j.text;
-            console.log(j), Object.keys(j.errors).map(function(C) {
-                if (C == "__all__") I = j.errors[C];
+        I("POST", e.data.url, function(k) {
+            if (s.target.dataset.spinning && (s.target.querySelector("i.fa-spin").style.display = "none", s.target.querySelector("i.fa-" + s.target.dataset.spinning).style.display = "inline-block"), k.type == "response") return U(), Ne(), ge(k);
+            var q = k.text;
+            console.log(k), Object.keys(k.errors).map(function(C) {
+                if (C == "__all__") q = k.errors[C];
                 else {
-                    const M = m.querySelector("#" + C + "_error");
-                    M.querySelector("span").innerHTML = j.errors[C], M.style.display = "block"
+                    const E = m.querySelector("#" + C + "_error");
+                    E.querySelector("span").innerHTML = k.errors[C], E.style.display = "block"
                 }
-            }), Q(I, !0)
+            }), Q(q, !0)
         }, x)
     }
-    return d()
+    return c()
 }
 
 function G(e) {
     if (e === null || e === "") return "-";
     if (e === !0) return "Sim";
     if (e === !1) return "Não";
     if (typeof e == "number") {
@@ -1528,17 +1532,17 @@
     }
     return typeof e == "object" && e.type ? t.jsx(y, {
         data: e
     }) : typeof e == "object" && Array.isArray(e) ? e.length == 0 ? "-" : t.jsx("ul", {
         style: {
             padding: 0
         },
-        children: e.map(function(c) {
+        children: e.map(function(d) {
             return t.jsx("li", {
-                children: c
+                children: d
             }, Math.random())
         })
     }) : typeof e == "object" && JSON.stringify(Object.keys(e)) == JSON.stringify(["id", "text"]) ? e.text : JSON.stringify(e)
 }
 
 function X(e) {
     function n() {
@@ -1557,53 +1561,53 @@
 }
 
 function z({
     id: e,
     href: n,
     modal: a,
     imodal: r,
-    children: c,
+    children: d,
     onClick: i,
     dataLabel: l,
-    style: d
+    style: c
 }) {
     const o = n && n.indexOf("/media/") < 0 ? F(n) : n;
 
     function h(m) {
         m.preventDefault(), a ? ye(o) : r ? De(o) : window.load(o)
     }
 
     function s() {
         return t.jsx("a", {
             id: e,
             onClick: i || h,
             href: o || "#",
-            "data-label": k(l),
-            style: d,
-            children: c
+            "data-label": b(l),
+            style: c,
+            children: d
         })
     }
     return s()
 }
 
 function Xe(e) {
     e.data.id == null && (e.data.id = Math.random());
     const [n, a] = S.useState(e.data);
 
     function r() {
         return n.attrname ? t.jsx("h2", {
-            "data-label": k(n.title),
+            "data-label": b(n.title),
             children: n.title
         }) : t.jsx("h1", {
-            "data-label": k(n.title),
+            "data-label": b(n.title),
             children: n.title
         })
     }
 
-    function c() {
+    function d() {
         const u = {
             display: "flex",
             justifyContent: "space-between",
             alignItems: "baseline"
         };
         return t.jsxs("div", {
             style: u,
@@ -1641,49 +1645,50 @@
                         paddingRight: 15,
                         fontWeight: f ? "bold" : "normal",
                         borderBottom: f ? "solid 3px #2670e8" : "solid 3px #DDD",
                         textDecoration: "none",
                         color: "#0c326f"
                     },
                     onClick: function(p) {
-                        p.preventDefault(), d(u.name)
+                        p.preventDefault(), c(u.name)
                     },
+                    dataLabel: b(u.label),
                     children: t.jsxs("div", {
                         style: {
                             display: "inline-block"
                         },
                         children: [u.label, " (", u.count, ")"]
                     })
                 }, Math.random())
             })
         })
     }
 
-    function d(u) {
+    function c(u) {
         const g = document.getElementById("subset-" + e.data.id);
-        g.value = u || "", M()
+        g.value = u || "", E()
     }
 
     function o(u, g, f) {
         const p = document.getElementById("form-" + e.data.id);
-        p.querySelector("input[name=" + n.calendar.field + "__day]").value = u || "", p.querySelector("input[name=" + n.calendar.field + "__month]").value = g || "", p.querySelector("input[name=" + n.calendar.field + "__year]").value = f || "", M()
+        p.querySelector("input[name=" + n.calendar.field + "__day]").value = u || "", p.querySelector("input[name=" + n.calendar.field + "__month]").value = g || "", p.querySelector("input[name=" + n.calendar.field + "__year]").value = f || "", E()
     }
 
     function h() {
         if (n.calendar) {
-            const b = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
-                L = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
+            const w = ["SEG", "TER", "QUA", "QUI", "SEX", "SAB", "DOM"],
+                A = ["JANEIRO", "FEVEVEIRO", "MARÇO", "ABRIL", "MAIO", "JUNHO", "JULHO", "AGOSTO", "SETEMRO", "OUTUBRO", "NOVEMBRO", "DEZEMBRO"],
                 Z = {
                     width: "100%",
                     borderSpacing: 0,
                     borderCollapse: "collapse",
                     marginTop: 15,
                     marginBottom: 15
                 },
-                T = {
+                M = {
                     marginLeft: "17",
                     textAlign: "right",
                     paddingRight: 2,
                     paddingTop: 2,
                     float: "right",
                     fontSize: "0.8rem"
                 },
@@ -1742,19 +1747,19 @@
                         })
                     }), t.jsxs("div", {
                         children: [t.jsxs("h3", {
                             align: "center",
                             style: {
                                 margin: 0
                             },
-                            children: [L[n.calendar.month - 1], " ", n.calendar.year]
+                            children: [A[n.calendar.month - 1], " ", n.calendar.year]
                         }), n.calendar.day && t.jsxs("div", {
                             align: "center",
-                            className: T,
-                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(w, {
+                            className: M,
+                            children: [new Date(n.calendar.year, n.calendar.month - 1, n.calendar.day).toLocaleDateString("pt-BR"), t.jsx(j, {
                                 default: !0,
                                 icon: "x",
                                 onClick: () => o(null, n.calendar.month, n.calendar.year),
                                 style: {
                                     marginLeft: 10,
                                     cursor: "pointer"
                                 }
@@ -1767,43 +1772,43 @@
                             onClick: () => o(null, n.calendar.next.month, n.calendar.next.year)
                         })
                     })]
                 }), t.jsxs("table", {
                     style: Z,
                     children: [t.jsx("thead", {
                         children: t.jsx("tr", {
-                            children: b.map(ee => t.jsx("th", {
+                            children: w.map(ee => t.jsx("th", {
                                 children: ee
                             }, Math.random()))
                         })
                     }), t.jsx("tbody", {
                         children: u.map(ee => t.jsx("tr", {
-                            children: ee.map(B => t.jsxs("td", {
+                            children: ee.map(L => t.jsxs("td", {
                                 style: _,
                                 children: [t.jsx("div", {
-                                    style: T,
-                                    children: B.today ? t.jsx("span", {
+                                    style: M,
+                                    children: L.today ? t.jsx("span", {
                                         style: {
                                             textDecoration: "underline"
                                         },
-                                        children: B.date
-                                    }) : B.date + B.today
-                                }), B.total && t.jsx("div", {
+                                        children: L.date
+                                    }) : L.date + L.today
+                                }), L.total && t.jsx("div", {
                                     style: N,
-                                    onClick: () => o(B.date, n.calendar.month, n.calendar.year),
+                                    onClick: () => o(L.date, n.calendar.month, n.calendar.year),
                                     children: t.jsx("div", {
                                         style: W,
                                         children: t.jsx("span", {
                                             style: {
-                                                textDecoration: B.selected ? "underline" : "normal"
+                                                textDecoration: L.selected ? "underline" : "normal"
                                             },
-                                            children: B.total
+                                            children: L.total
                                         })
                                     })
-                                }), !B.total && t.jsx("div", {
+                                }), !L.total && t.jsx("div", {
                                     style: N,
                                     children: " "
                                 })]
                             }, Math.random()))
                         }, Math.random()))
                     })]
                 })]
@@ -1910,22 +1915,22 @@
                 text: "Nenhum registro encontrado."
             }
         })
     }
 
     function v(u) {
         const f = document.getElementById("form-" + e.data.id).querySelector("input[name=page]");
-        f.value = u, M()
+        f.value = u, E()
     }
 
-    function j() {
+    function k() {
         const u = document.getElementById("form-" + e.data.id);
         if (u) {
-            const b = u.querySelector("input[name=page]");
-            b && (b.value = n.pagination.page.current)
+            const w = u.querySelector("input[name=page]");
+            w && (w.value = n.pagination.page.current)
         }
         const g = {
                 display: "flex",
                 justifyContent: "space-between",
                 lineHeight: "4rem",
                 alignItems: "baseline"
             },
@@ -1947,17 +1952,17 @@
                 children: [t.jsxs("div", {
                     style: f,
                     children: ["Exibir", t.jsx("select", {
                         style: p,
                         name: "page_size",
                         onChange: () => v(1),
                         value: n.pagination.page.size,
-                        children: n.pagination.page.sizes.map(function(b) {
+                        children: n.pagination.page.sizes.map(function(w) {
                             return t.jsx("option", {
-                                children: b
+                                children: w
                             }, Math.random())
                         })
                     })]
                 }), t.jsx("div", {
                     style: f,
                     children: "|"
                 }), t.jsxs("div", {
@@ -1976,16 +1981,16 @@
                         style: {
                             width: 30,
                             marginLeft: 10,
                             marginRight: 10,
                             height: "2rem",
                             textAlign: "center"
                         },
-                        onKeyDown: function(b) {
-                            b.key == "Enter" && (b.preventDefault(), v(b.target.value < 0 ? 1 : Math.min(b.target.value, n.pagination.page.total)))
+                        onKeyDown: function(w) {
+                            w.key == "Enter" && (w.preventDefault(), v(w.target.value < 0 ? 1 : Math.min(w.target.value, n.pagination.page.total)))
                         }
                     }), t.jsx("div", {
                         style: f,
                         children: "|"
                     }), n.pagination.page.previous && t.jsx(D, {
                         icon: "chevron-left",
                         default: !0,
@@ -1998,15 +2003,15 @@
                         onClick: () => v(n.pagination.page.next)
                     })]
                 })
             })]
         })
     }
 
-    function I() {
+    function q() {
         return t.jsx("div", {
             align: "right",
             style: {
                 marginTop: 20,
                 marginBottom: 20
             },
             children: n.actions.map(function(u) {
@@ -2034,51 +2039,51 @@
                 children: [t.jsxs(X, {
                     width: 250,
                     children: [g && t.jsx("div", {
                         style: u,
                         children: t.jsx(Y, {
                             data: p
                         })
-                    }), f && n.filters.map(function(b) {
-                        return b.type != "hidden" && t.jsx("div", {
+                    }), f && n.filters.map(function(w) {
+                        return w.type != "hidden" && t.jsx("div", {
                             style: u,
                             children: t.jsx(Y, {
-                                data: b
+                                data: w
                             })
                         }, Math.random())
                     }), t.jsx("div", {
                         style: u,
                         children: t.jsx(D, {
-                            onClick: M,
+                            onClick: E,
                             label: "Filtrar",
                             default: !0
                         })
                     })]
-                }), f && n.filters.map(function(b) {
-                    return b.type == "hidden" && t.jsx("div", {
+                }), f && n.filters.map(function(w) {
+                    return w.type == "hidden" && t.jsx("div", {
                         style: u,
                         children: t.jsx(Y, {
-                            data: b
+                            data: w
                         })
                     }, Math.random())
                 })]
             })
         }
     }
 
-    function M() {
+    function E() {
         i(!0);
         var u;
         const g = new URLSearchParams(new FormData(document.getElementById("form-" + e.data.id))).toString();
-        e.data.url.indexOf("?") > 0 ? u = e.data.url + "&" + g : u = e.data.url + "?" + g, q("GET", u, function(f) {
+        e.data.url.indexOf("?") > 0 ? u = e.data.url + "&" + g : u = e.data.url + "?" + g, I("GET", u, function(f) {
             a(f), i(!1)
         })
     }
 
-    function E() {
+    function T() {
         return n.bi ? t.jsxs(t.Fragment, {
             children: [C(), n.bi.map(function(u) {
                 return t.jsx(X, {
                     width: 300,
                     alignItems: "start",
                     children: u.map(function(g) {
                         return t.jsx("div", {
@@ -2086,20 +2091,20 @@
                                 data: g
                             })
                         }, Math.random())
                     })
                 }, Math.random())
             })]
         }) : t.jsxs(t.Fragment, {
-            children: [I(), l(), C(), h(), x(), j()]
+            children: [q(), l(), C(), h(), x(), k()]
         })
     }
 
     function P() {
-        window[e.data.id] = () => M();
+        window[e.data.id] = () => E();
         const u = {
             backgroundColor: "white",
             padding: 20
         };
         return t.jsx("div", {
             className: "reloadable",
             id: e.data.id,
@@ -2108,15 +2113,15 @@
                 id: "form-" + e.data.id,
                 children: [t.jsx("div", {
                     children: !1
                 }), t.jsx("input", {
                     type: "hidden",
                     name: "subset",
                     id: "subset-" + e.data.id
-                }), c(), E()]
+                }), d(), T()]
             })
         })
     }
     return P()
 }
 
 function ae(e) {
@@ -2147,22 +2152,22 @@
     return n()
 }
 
 function Qe(e) {
     const n = Math.random(),
         [a, r] = S.useState(e.data);
 
-    function c(l) {
-        q("GET", l, function(d) {
-            r(d)
+    function d(l) {
+        I("GET", l, function(c) {
+            r(c)
         })
     }
 
     function i() {
-        return window[n] = () => c(e.data.url), t.jsx("div", {
+        return window[n] = () => d(e.data.url), t.jsx("div", {
             className: e.data.url && "reloadable",
             id: n,
             children: t.jsx(be, {
                 data: a,
                 width: 100
             })
         })
@@ -2170,15 +2175,15 @@
     return i()
 }
 
 function Ke(e) {
     const n = Math.random(),
         [a, r] = S.useState(e.data);
 
-    function c() {
+    function d() {
         return t.jsx(we, {
             data: a
         })
     }
 
     function i() {
         return Array.isArray(a.data) ? a.data.length == 0 ? t.jsx("div", {
@@ -2198,53 +2203,53 @@
             }, Math.random())
         }) : t.jsx(y, {
             data: a.data
         })
     }
 
     function l(o) {
-        q("GET", o, function(h) {
+        I("GET", o, function(h) {
             r(h)
         })
     }
 
-    function d() {
+    function c() {
         return e.data.url ? (window[n] = () => l(e.data.url), t.jsxs("div", {
             className: e.data.url && "reloadable",
             id: n,
-            children: [c(), i()]
+            children: [d(), i()]
         })) : t.jsxs("div", {
-            children: [c(), i()]
+            children: [d(), i()]
         })
     }
-    return d()
+    return c()
 }
 
 function Ze(e) {
     const n = Math.random(),
         [a, r] = S.useState(e.data.actions);
 
-    function c() {
-        const d = e.data.url.indexOf("?") < 0 ? "?" : "&";
-        return e.data.url + d + "only=actions"
+    function d() {
+        const c = e.data.url.indexOf("?") < 0 ? "?" : "&";
+        return e.data.url + c + "only=actions"
     }
 
     function i() {
-        q("GET", c(), function(d) {
-            r(d)
+        I("GET", d(), function(c) {
+            r(c)
         })
     }
 
     function l() {
         return window[n] = () => i(), t.jsx("div", {
             className: "reloadable",
             id: n,
-            children: a.map(function(d) {
+            children: a.map(function(c) {
                 return t.jsx(O, {
-                    data: d,
+                    data: c,
                     default: !0
                 }, Math.random())
             })
         })
     }
     return l()
 }
@@ -2259,15 +2264,15 @@
             r = {
                 margin: 0
             };
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h1", {
                 style: r,
-                "data-label": k(e.data.title),
+                "data-label": b(e.data.title),
                 children: e.data.title
             }), t.jsx(Ze, {
                 data: e.data
             })]
         })
     }
     return n()
@@ -2284,20 +2289,20 @@
                 marginBottom: 0,
                 marginTop: 15
             };
         return t.jsxs("div", {
             style: a,
             children: [e.data.title && t.jsx("h2", {
                 style: r,
-                "data-label": k(e.data.title),
+                "data-label": b(e.data.title),
                 children: e.data.title
             }), e.data.actions.length > 0 && t.jsx("div", {
-                children: e.data.actions.map(function(c) {
+                children: e.data.actions.map(function(d) {
                     return t.jsx(O, {
-                        data: c,
+                        data: d,
                         default: !0
                     }, Math.random())
                 })
             })]
         })
     }
     return n()
@@ -2307,17 +2312,17 @@
     function n() {
         return t.jsx(et, {
             data: e.data
         })
     }
 
     function a() {
-        return e.data.data.map(function(c, i) {
+        return e.data.data.map(function(d, i) {
             return t.jsx(y, {
-                data: c
+                data: d
             }, Math.random())
         })
     }
 
     function r() {
         return t.jsxs(t.Fragment, {
             children: [n(), a()]
@@ -2330,20 +2335,20 @@
     function n() {
         return t.jsx(we, {
             data: e.data
         })
     }
 
     function a() {
-        const c = {
+        const d = {
             backgroundColor: "white"
         };
         return e.data.data.map(function(i, l) {
             return t.jsx("div", {
-                style: c,
+                style: d,
                 children: t.jsx(y, {
                     data: i
                 }, Math.random())
             })
         })
     }
 
@@ -2363,43 +2368,44 @@
             style: {
                 display: "inline-block",
                 textAlign: "center",
                 width: "100%",
                 margin: "auto",
                 marginBottom: 20
             },
-            children: e.data.map(function(c, i) {
+            children: e.data.map(function(d, i) {
                 return t.jsx(z, {
-                    href: c.url,
+                    href: d.url,
                     style: {
                         padding: 5,
                         fontWeight: n == i ? "bold" : "normal",
                         borderBottom: n == i ? "solid 3px #2670e8" : "solid 3px inherite",
                         textDecoration: "none",
                         color: "#0c326f",
                         margin: 15
                     },
                     onClick: function(l) {
-                        l.preventDefault(), a(i), e.loadContent(c.url)
+                        l.preventDefault(), a(i), e.loadContent(d.url)
                     },
-                    children: c.title
+                    dataLabel: b(d.title),
+                    children: d.title
                 }, Math.random())
             })
         })
     }
     return r()
 }
 
 function rt(e) {
     var n = Math.random();
     const [a, r] = S.useState(e.data.data[0]);
 
-    function c() {
+    function d() {
         return e.data.title != "Top" && t.jsx("h2", {
-            "data-label": k(e.data.title),
+            "data-label": b(e.data.title),
             children: e.data.title
         })
     }
 
     function i() {
         return t.jsx(at, {
             data: e.data.data,
@@ -2419,51 +2425,51 @@
             style: m,
             children: t.jsx(y, {
                 data: s
             }, Math.random())
         })
     }
 
-    function d() {
+    function c() {
         const s = {
             width: "50%",
             margin: "auto",
             border: "solid 0.5px #DDD",
             marginTop: 30,
             marginBottom: 30
         };
         return t.jsx("div", {
             style: s
         })
     }
 
     function o(s) {
-        q("GET", s, function(m) {
+        I("GET", s, function(m) {
             r(m)
         })
     }
 
     function h() {
         return window[n] = () => o(a.url), e.data.data.length > 0 && t.jsxs("div", {
             className: "reloadable",
             id: n,
-            children: [c(), i(), l(), d()]
+            children: [d(), i(), l(), c()]
         })
     }
     return h()
 }
 
 function K(e) {
     var n = Math.random();
 
     function a() {
         var r = document.getElementById(n);
         if (r) {
-            var c = echarts.init(r);
-            c.setOption(e.option)
+            var d = echarts.init(r);
+            d.setOption(e.option)
         } else setTimeout(a, 1e3)
     }
     return setTimeout(a, 1e3), t.jsx("div", {
         id: n,
         style: {
             width: "100%",
             height: 300
@@ -2479,17 +2485,17 @@
         ["40%", "48%"],
         ["30%", "48%"],
         ["20%", "28%"],
         ["10%", "18%"]
     ];
 
     function a() {
-        return e.headers ? e.headers.slice(1).map(function(c, i) {
+        return e.headers ? e.headers.slice(1).map(function(d, i) {
             return {
-                name: c,
+                name: d,
                 type: "pie",
                 radius: n[i],
                 emphasis: {
                     label: {
                         show: !0,
                         formatter: function(l) {
                             return l.value.toLocaleString("pt-BR")
@@ -2508,32 +2514,32 @@
         }) : {
             name: null,
             type: "pie",
             radius: e.donut ? ["25%", "65%"] : ["0%", "75%"],
             emphasis: {
                 label: {
                     show: !0,
-                    formatter: function(c) {
-                        return c.value.toLocaleString("pt-BR")
+                    formatter: function(d) {
+                        return d.value.toLocaleString("pt-BR")
                     },
                     fontWeight: "bold"
                 }
             },
             roseType: e.area ? "area" : null,
-            data: e.rows.map(function(c, i) {
+            data: e.rows.map(function(d, i) {
                 return {
-                    name: c[0],
-                    value: c[1]
+                    name: d[0],
+                    value: d[1]
                 }
             })
         }
     }
 
     function r() {
-        var c = {
+        var d = {
             tooltip: {
                 trigger: "item",
                 formatter: function(i) {
                     return `${i.name}: <b>${i.data.value.toLocaleString("pt-BR")}</b> (${i.percent.toLocaleString("pt-BR")}%)`
                 }
             },
             legend: {},
@@ -2542,15 +2548,15 @@
                 formatter(i) {
                     return i.name + " (" + i.percent.toLocaleString("pt-BR") + "%)"
                 }
             },
             series: a()
         };
         return t.jsx(K, {
-            option: c
+            option: d
         })
     }
     return r()
 }
 
 function it(e) {
     return t.jsx(oe, {
@@ -2568,15 +2574,15 @@
     })
 }
 
 function R(e) {
     var n = e.invert || !1,
         a = e.type || "bar",
         r = e.stack,
-        c = {
+        d = {
             type: "value"
         },
         i = {
             show: !0,
             feature: {
                 mark: {
                     show: !0
@@ -2584,15 +2590,15 @@
                 saveAsImage: {
                     show: !0
                 }
             }
         },
         l = e.area ? {} : null;
 
-    function d() {
+    function c() {
         return e.headers ? {
             type: "category",
             data: e.headers.slice(1)
         } : {
             type: "category",
             data: e.rows.map(function(s) {
                 return s[0]
@@ -2635,16 +2641,16 @@
             legend: {},
             label: {
                 show: !0,
                 formatter: function(m) {
                     return m.value.toLocaleString("pt-BR")
                 }
             },
-            xAxis: n ? c : d(),
-            yAxis: n ? d() : c,
+            xAxis: n ? d : c(),
+            yAxis: n ? c() : d,
             series: o()
         };
         return t.jsx(K, {
             option: s
         })
     }
     return h()
@@ -2701,22 +2707,22 @@
 
 function mt(e) {
     function n() {
         return e.headers ? [{
             type: "treemap",
             roam: "move",
             nodeClick: !0,
-            data: e.headers.slice(1).map(function(r, c) {
+            data: e.headers.slice(1).map(function(r, d) {
                 return {
                     name: r,
                     type: "pie",
                     children: e.rows.map(function(i) {
                         return {
                             name: i[0],
-                            value: i[c + 1]
+                            value: i[d + 1]
                         }
                     })
                 }
             })
         }] : [{
             type: "treemap",
             roam: "move",
@@ -2734,16 +2740,16 @@
         var r = {
             tooltip: {
                 trigger: "item"
             },
             legend: {},
             label: {
                 show: !0,
-                formatter(c) {
-                    return c.name + " (" + c.value.toLocaleString("pt-BR") + ")"
+                formatter(d) {
+                    return d.name + " (" + d.value.toLocaleString("pt-BR") + ")"
                 }
             },
             series: n()
         };
         return t.jsx(K, {
             option: r
         })
@@ -2879,81 +2885,81 @@
         })
     }
     return a()
 }
 
 function gt(e) {
     function n() {
-        for (var r = [], c = 0; c < e.data.series.length; c++) r.push([e.data.series[c][0], e.data.series[c][1]]);
+        for (var r = [], d = 0; d < e.data.series.length; d++) r.push([e.data.series[d][0], e.data.series[d][1]]);
         return e.data.chart ? t.jsx(he, {
             type: e.data.chart,
             title: e.data.title,
             rows: r
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": k(e.data.title),
+                "data-label": b(e.data.title),
                 children: e.data.title
             }), t.jsx("table", {
                 style: {
                     width: "100%"
                 },
                 children: t.jsx("tbody", {
                     children: r.map(i => t.jsx("tr", {
-                        children: i.map((l, d) => d == 0 ? t.jsx("th", {
+                        children: i.map((l, c) => c == 0 ? t.jsx("th", {
                             style: {
                                 textAlign: "left"
                             },
                             children: l
                         }, Math.random()) : t.jsx("td", {
                             children: G(l)
                         }, Math.random()))
                     }, Math.random()))
                 })
             })]
         })
     }
 
     function a() {
-        for (var r = [], c = [], i = Object.keys(e.data.series), l = [], d = 0; d < i.length; d++) {
-            d == 0 && r.push("");
-            for (var o = [i[d]], h = 0, s = 0; s < e.data.series[i[d]].length; s++) {
-                var m = e.data.series[i[d]];
-                d == 0 && r.push(m[s][0]), o.push(m[s][1]), h += m[s][1], i.length > 1 && (d == 0 ? l.push(m[s][1]) : l[s] += m[s][1], s > 0 && s == e.data.series[i[d]].length - 1 && (d == 0 ? l.push(h) : l[s + 1] += h))
+        for (var r = [], d = [], i = Object.keys(e.data.series), l = [], c = 0; c < i.length; c++) {
+            c == 0 && r.push("");
+            for (var o = [i[c]], h = 0, s = 0; s < e.data.series[i[c]].length; s++) {
+                var m = e.data.series[i[c]];
+                c == 0 && r.push(m[s][0]), o.push(m[s][1]), h += m[s][1], i.length > 1 && (c == 0 ? l.push(m[s][1]) : l[s] += m[s][1], s > 0 && s == e.data.series[i[c]].length - 1 && (c == 0 ? l.push(h) : l[s + 1] += h))
             }
-            o.length > 2 && (d == 0 && r.push("TOTAL"), o.push(h)), c.push(o)
+            o.length > 2 && (c == 0 && r.push("TOTAL"), o.push(h)), d.push(o)
         }
         return e.data.chart ? t.jsx(he, {
             type: e.data.chart,
             title: e.data.title,
             headers: r,
-            rows: c
+            rows: d
         }) : t.jsxs("div", {
             className: "statistics",
             children: [e.data.title && t.jsx("h2", {
-                "data-label": k(e.data.title),
+                "data-label": b(e.data.title),
                 children: e.data.title
             }), t.jsxs("table", {
                 style: {
                     width: "100%"
                 },
                 children: [r && t.jsx("thead", {
                     children: t.jsx("tr", {
                         children: r.map(x => t.jsx("th", {
                             children: x
                         }, Math.random()))
                     })
                 }), t.jsxs("tbody", {
-                    children: [c.map(x => t.jsx("tr", {
-                        children: x.map((v, j) => j == 0 ? t.jsx("th", {
+                    children: [d.map(x => t.jsx("tr", {
+                        children: x.map((v, k) => k == 0 ? t.jsx("th", {
                             children: v
                         }, Math.random()) : t.jsx("td", {
                             align: "center",
                             style: {
-                                backgroundColor: j == x.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
+                                backgroundColor: k == x.length - 1 && r && r[r.length - 1] == "TOTAL" ? "var(--info-color)" : "inherite"
                             },
                             children: G(v)
                         }, Math.random()))
                     }, Math.random())), l.length > 0 && t.jsxs("tr", {
                         children: [t.jsx("th", {
                             children: "TOTAL"
                         }), l.map(x => t.jsxs("td", {
@@ -3019,65 +3025,65 @@
                 })
             })]
         })
     }
 
     function n(i) {
         var l = i.target;
-        const d = l.querySelector(":scope > ul, :scope > li");
-        if (d) {
-            d.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(s) {
+        const c = l.querySelector(":scope > ul, :scope > li");
+        if (c) {
+            c.offsetParent === null ? l.querySelectorAll(":scope > ul, :scope > li, :scope > ul > li").forEach(function(s) {
                 s.style.display = "block"
             }) : l.querySelectorAll(":scope > ul, :scope > li").forEach(function(s) {
                 s.style.display = "none"
             });
             const o = l.querySelector(":scope > i.fa-solid.fa-chevron-right"),
                 h = l.querySelector(":scope > i.fa-solid.fa-chevron-up");
             return o && (o.classList.remove("fa-chevron-right"), o.classList.add("fa-chevron-up")), h && (h.classList.remove("fa-chevron-up"), h.classList.add("fa-chevron-right")), i.preventDefault(), i.stopPropagation(), i.cancelBubble = !0, !1
         } else {
             const o = document.querySelector("aside");
             o.style.display = window.innerWidth < 800 ? "none" : "block"
         }
     }
 
     function a(i, l) {
-        const d = {
+        const c = {
                 display: l == 0 ? "block" : "none",
                 cursor: "pointer",
                 paddingLeft: 5,
                 paddingTop: 10,
                 paddingBottom: 10,
                 lineHeight: "2rem"
             },
             o = {
                 padding: 5,
                 fontSize: "1.2rem"
             };
         return i.url ? t.jsx("li", {
-            style: d,
+            style: c,
             onClick: n,
             children: t.jsxs(z, {
                 href: i.url,
-                dataLabel: k(i.label),
+                dataLabel: b(i.label),
                 style: {
                     textDecoration: "none"
                 },
-                children: [l == 0 && t.jsx(w, {
+                children: [l == 0 && t.jsx(j, {
                     icon: i.icon || "dot-circle",
                     style: o
                 }), i.label]
             })
         }, Math.random()) : i.items.length > 0 && t.jsxs("li", {
             onClick: n,
-            style: d,
-            "data-label": k(i.label),
-            children: [l == 0 && t.jsx(w, {
+            style: c,
+            "data-label": b(i.label),
+            children: [l == 0 && t.jsx(j, {
                 icon: i.icon || "dot-circle",
                 style: o
-            }), i.label, t.jsx(w, {
+            }), i.label, t.jsx(j, {
                 icon: "chevron-right",
                 style: {
                     float: "right",
                     paddingTop: 8
                 }
             }), t.jsx("ul", {
                 style: {
@@ -3099,90 +3105,90 @@
             style: i,
             children: window.application.menu.items.map(function(l) {
                 return a(l, 0)
             })
         })
     }
 
-    function c() {
+    function d() {
         const i = {
             padding: 25,
             height: "100%",
             borderRight: "solid 1px #EEE"
         };
         return t.jsxs("div", {
             style: i,
             children: [e(), r()]
         })
     }
-    return c()
+    return d()
 }
 
 function pt(e) {
     var n;
 
     function a(i) {
         const l = "=".repeat((4 - i.length % 4) % 4),
-            d = (i + l).replace(/\-/g, "+").replace(/_/g, "/"),
-            o = window.atob(d),
+            c = (i + l).replace(/\-/g, "+").replace(/_/g, "/"),
+            o = window.atob(c),
             h = new Uint8Array(o.length);
         for (let s = 0; s < o.length; ++s) h[s] = o.charCodeAt(s);
         return h
     }
 
     function r() {
         "serviceWorker" in navigator && "PushManager" in window ? navigator.serviceWorker.getRegistration().then(function(i) {
             if (i) {
                 const l = a("BLoLJSopQbe04v_zpegJmayhH2Px0EGzrFIlM0OedSOTYsMpO5YGmHOxbpPXdM09ttIuDaDTI86uC85JXZPpEtA");
                 i.pushManager.subscribe({
                     userVisibleOnly: !0,
                     applicationServerKey: l
-                }).then(function(d) {
-                    if (console.log(d), n = JSON.stringify(d), console.log(n), d) {
+                }).then(function(c) {
+                    if (console.log(c), n = JSON.stringify(c), console.log(n), c) {
                         alert("Notificação ativada com sucesso.");
                         var o = new FormData;
-                        o.append("subscription", n), q("POST", "/api/pushsubscribe/", function(h) {
+                        o.append("subscription", n), I("POST", "/api/pushsubscribe/", function(h) {
                             console.log(h)
                         }, o)
                     } else {
                         alert("Problema ao ativar notificações.");
                         return
                     }
-                }).catch(function(d) {
-                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", d)
+                }).catch(function(c) {
+                    alert("Problema ao tentar ativar notificações."), console.log("Failed to subscribe the user: ", c)
                 })
             } else console.log("No registered service worker.")
         }).catch(function(i) {
             alert("Erro"), console.error("Service Worker Error", i)
         }) : alert("Push messaging is not supported")
     }
 
-    function c() {
-        return t.jsx(w, {
+    function d() {
+        return t.jsx(j, {
             onClick: r,
             icon: "bell",
             style: {
                 cursor: "pointer"
             }
         })
     }
-    return c()
+    return d()
 }
 
 function vt(e) {
     const [n, a] = S.useState(e.data);
-    window.loaddata = c => a(c);
+    window.loaddata = d => a(d);
 
     function r() {
-        const c = {
+        const d = {
             minHeight: 400,
             margin: 20
         };
         return t.jsx("div", {
-            style: c,
+            style: d,
             id: "container",
             children: t.jsx(y, {
                 data: n
             }, Math.random())
         })
     }
     return r()
@@ -3221,15 +3227,15 @@
             };
         return e.data.navbar ? t.jsxs("div", {
             style: o,
             children: [t.jsxs("div", {
                 style: {
                     padding: 20
                 },
-                children: [t.jsx(w, {
+                children: [t.jsx(j, {
                     icon: "navicon",
                     style: {
                         fontSize: "1.5rem",
                         marginRight: 10,
                         cursor: "pointer"
                     },
                     onClick: a
@@ -3253,15 +3259,15 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx($, {
                         actions: e.data.navbar.adder,
                         position: {},
                         dataLabel: "plus",
-                        children: t.jsx(w, {
+                        children: t.jsx(j, {
                             icon: "plus"
                         })
                     })
                 }), t.jsx("div", {
                     style: {
                         padding: 10
                     },
@@ -3270,27 +3276,27 @@
                     style: {
                         padding: 10
                     },
                     children: t.jsx($, {
                         actions: e.data.navbar.tools,
                         position: {},
                         dataLabel: "tools",
-                        children: t.jsx(w, {
+                        children: t.jsx(j, {
                             icon: "tools"
                         })
                     })
                 }), e.data.navbar.settings.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx($, {
                         actions: e.data.navbar.settings,
                         position: {},
                         dataLabel: "gear",
-                        children: t.jsx(w, {
+                        children: t.jsx(j, {
                             icon: "gear"
                         })
                     })
                 }), window.innerWidth > 800 && t.jsx(ve, {
                     data: h,
                     style: {
                         padding: 10
@@ -3299,23 +3305,23 @@
                 }), e.data.navbar.usermenu.length > 0 && t.jsx("div", {
                     style: {
                         padding: 10
                     },
                     children: t.jsx($, {
                         actions: e.data.navbar.usermenu,
                         position: {},
-                        dataLabel: k(e.data.navbar.user),
+                        dataLabel: b(e.data.navbar.user),
                         children: e.data.navbar.user
                     })
                 })]
             })]
         }) : null
     }
 
-    function c() {
+    function d() {
         return window.application.menu && t.jsx("aside", {
             style: {
                 flexGrow: 2,
                 maxWidth: "350px",
                 minWidth: "350px",
                 display: window.innerWidth < 800 ? "none" : "block"
             },
@@ -3344,31 +3350,31 @@
                 children: "Todos os direitos reservados"
             }), t.jsx("div", {
                 children: e.data.footer.version
             })]
         }) : null
     }
 
-    function d() {
+    function c() {
         return t.jsxs("div", {
             children: [t.jsx("header", {
                 children: r()
             }), t.jsxs("div", {
                 style: {
                     overflowX: "hide",
                     width: "100%",
                     display: "flex",
                     overflow: "hidden",
                     minHeight: window.innerHeight - 70
                 },
-                children: [c(), i()]
+                children: [d(), i()]
             })]
         })
     }
-    return d()
+    return c()
 }
 
 function wt(e) {
     return t.jsx("img", {
         src: e.data.src,
         style: {
             width: "100%"
@@ -3405,15 +3411,15 @@
         marginHeight: "0",
         marginWidth: "0"
     })
 }
 
 function St(e) {
     function n(i) {
-        return e.data.icon ? i.done ? t.jsx(w, {
+        return e.data.icon ? i.done ? t.jsx(j, {
             style: {
                 marginTop: 12
             },
             icon: e.data.icon
         }) : t.jsx("span", {
             children: " "
         }) : t.jsx("div", {
@@ -3443,29 +3449,29 @@
             listStyleType: "none",
             display: "flex",
             justifyContent: "center",
             minWidth: i.length * 100
         }
     }
 
-    function c() {
+    function d() {
         const i = {
                 width: "100%",
                 margin: "auto",
                 overflowX: "auto",
                 "&::WebkitScrollbar": {
                     width: 0
                 }
             },
             l = {
                 width: 100,
                 marginWidth: 100,
                 textAlign: "center"
             },
-            d = {
+            c = {
                 position: "relative",
                 borderBottom: "2px solid #EEE",
                 top: -28,
                 width: 45,
                 left: 77
             };
         return t.jsx("div", {
@@ -3475,51 +3481,51 @@
                     style: r(e.data.steps),
                     children: e.data.steps.map((o, h) => t.jsxs("li", {
                         style: l,
                         children: [t.jsx("div", {
                             style: a(o),
                             children: n(o)
                         }), h < e.data.steps.length - 1 && t.jsx("div", {
-                            style: d
+                            style: c
                         }), t.jsx("div", {
                             children: o.name
                         })]
                     }, Math.random()))
                 })
             })
         })
     }
-    return c()
+    return d()
 }
 
 function Ct(e) {
     function n() {
         const a = {
                 display: "inline-block",
                 width: "100%",
                 backgroundColor: "#DDD",
                 borderRadius: 5,
                 marginTop: 5
             },
             r = {
                 marginLeft: 10
             },
-            c = {
+            d = {
                 display: "block",
                 paddingTop: 2,
                 paddingBottom: 2,
                 color: "white",
                 borderRadius: 5,
                 width: e.data.value + "%",
                 backgroundColor: je[e.data.style]
             };
         return t.jsx("span", {
             style: a,
             children: t.jsx("span", {
-                style: c,
+                style: d,
                 children: t.jsxs("span", {
                     style: r,
                     children: [e.data.value, "%"]
                 })
             })
         })
     }
@@ -3569,15 +3575,15 @@
                 width: 250,
                 height: 250,
                 backgroundColor: "white",
                 boxShadow: "0px 15px 10px -15px #DDD",
                 margin: 10,
                 textDecoration: "none"
             },
-            c = {
+            d = {
                 marginTop: 30,
                 fontSize: "3rem",
                 color: "#2670e8"
             },
             i = {
                 marginTop: 40,
                 fontWeight: "bold",
@@ -3585,24 +3591,24 @@
                 textTransform: "uppercase",
                 height: 70,
                 color: "#0c326f"
             };
         return e.data.items.length ? t.jsxs("div", {
             style: a,
             children: [t.jsx("h2", {
-                "data-label": k(e.data.title),
+                "data-label": b(e.data.title),
                 children: e.data.title
             }), t.jsx("div", {
                 children: e.data.items.map(l => t.jsxs(z, {
                     href: l.url,
                     style: r,
                     dataLabel: l.label,
                     children: [t.jsx("div", {
-                        children: t.jsx(w, {
-                            style: c,
+                        children: t.jsx(j, {
+                            style: d,
                             icon: l.icon
                         })
                     }), t.jsx("div", {
                         style: i,
                         children: l.label
                     })]
                 }, Math.random()))
@@ -3628,30 +3634,30 @@
                 children: a
             }, Math.random()))
         })
     }
     return n()
 }
 
-function qt(e) {
+function It(e) {
     function n() {
         return e.data.url ? t.jsx(z, {
             href: e.data.url,
             imodal: !!e.data.modal,
-            children: e.data.icon ? t.jsx(w, {
+            children: e.data.icon ? t.jsx(j, {
                 icon: e.data.icon
             }) : e.data.url
         }) : t.jsx("span", {
             children: "-"
         })
     }
     return n()
 }
 
-function It(e) {
+function qt(e) {
     function n() {
         return t.jsx("iframe", {
             src: e.data.url,
             width: "100%",
             height: 500,
             style: {
                 border: 0
@@ -3678,29 +3684,29 @@
         return t.jsx("div", {
             id: n
         })
     }
     return a()
 }
 
-function Bt(e) {
+function Lt(e) {
     function n() {
         return t.jsx(X, {
             width: 400,
             children: e.data.items.map((a, r) => t.jsx("div", {
                 children: t.jsx(y, {
                     data: a
                 })
             }, Math.random()))
         })
     }
     return n()
 }
 
-function At(e) {
+function Bt(e) {
     function n() {
         return t.jsxs("div", {
             children: [t.jsx("h2", {
                 children: e.data.title
             }), t.jsx("div", {
                 style: {
                     fontSize: "12rem",
@@ -3710,30 +3716,30 @@
                 children: e.data.value
             })]
         })
     }
     return n()
 }
 var re, Se = {};
-const Lt = "/api/application/",
+const At = "/api/application/",
     me = localStorage.getItem("application");
 
 function y(e) {
     const n = Se[e.data.type];
     return n ? n(e.data) : t.jsx("div", {
         children: JSON.stringify(e.data)
     })
 }
 y.register = function(e, n) {
     Se[e] = n
 };
 y.render = function(e) {
     re = e, document.location.pathname == "/" ? localStorage.getItem("token") ? window.reload("/app/dashboard/") : window.reload("/app/login/") : document.location.pathname == "/app/login/" && (localStorage.getItem("token") || localStorage.getItem("application")) ? (localStorage.removeItem("token"), localStorage.removeItem("application"), document.location.reload()) : window.reload(document.location.href)
 };
-y.register("counter", e => t.jsx(At, {
+y.register("counter", e => t.jsx(Bt, {
     data: e
 }));
 y.register("form", e => t.jsx(Ye, {
     data: e
 }));
 y.register("queryset", e => t.jsx(Xe, {
     data: e
@@ -3785,51 +3791,51 @@
 }));
 y.register("boxes", e => t.jsx(Et, {
     data: e
 }));
 y.register("shell", e => t.jsx(Tt, {
     data: e
 }));
-y.register("file_link", e => t.jsx(qt, {
+y.register("file_link", e => t.jsx(It, {
     data: e
 }));
-y.register("file_viewer", e => t.jsx(It, {
+y.register("file_viewer", e => t.jsx(qt, {
     data: e
 }));
-y.register("response", e => t.jsx(Ie, {
+y.register("response", e => t.jsx(qe, {
     data: e
 }));
 y.register("application", e => t.jsx(bt, {
     data: e
 }));
 y.register("iconset", e => t.jsx(Me, {
     data: e
 }));
-y.register("grid", e => t.jsx(Bt, {
+y.register("grid", e => t.jsx(Lt, {
     data: e
 }));
 window.addEventListener("popstate", e => {
     window.reload(e.currentTarget.location.href)
 });
 window.reload = function(e) {
     e != document.location.href && window.history.pushState({
         url: e
-    }, "", e), me ? (window.application = JSON.parse(me), q("GET", A(e), function(n) {
+    }, "", e), me ? (window.application = JSON.parse(me), I("GET", B(e), function(n) {
         window.application.content = n, re.render(t.jsx(y, {
             data: window.application
         }, Math.random()))
-    })) : q("GET", Lt, function(a) {
-        window.application = a, localStorage.setItem("application", JSON.stringify(window.application)), q("GET", A(e), function(r) {
+    })) : I("GET", At, function(a) {
+        window.application = a, localStorage.setItem("application", JSON.stringify(window.application)), I("GET", B(e), function(r) {
             window.application.content = r, re.render(t.jsx(y, {
                 data: window.application
             }, Math.random()))
         })
     })
 };
 window.load = function(e) {
     e.indexOf(window.origin) >= 0 || e.startsWith("/") ? (e != document.location.href && e != document.location.pathname && window.history.pushState({
         url: e
-    }, "", e), q("GET", A(e), function(n) {
+    }, "", e), I("GET", B(e), function(n) {
         window.loaddata(n)
     })) : document.location.href = e
 };
 y.render(H.createRoot(document.getElementById("root")));
```

### Comparing `pyslth-0.1.8/slth/static/js/peerjs.min.js` & `pyslth-0.1.9/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/js/qrcode.min.js` & `pyslth-0.1.9/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/js/react-trigger-change.js` & `pyslth-0.1.9/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/js/react.min.js` & `pyslth-0.1.9/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/js/vanilla-masker.js` & `pyslth-0.1.9/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/static/js/vanilla-masker.min.js` & `pyslth-0.1.9/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/statistics.py` & `pyslth-0.1.9/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/templates/index.html` & `pyslth-0.1.9/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/templates/service-worker.js` & `pyslth-0.1.9/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/tests.py` & `pyslth-0.1.9/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/urls.py` & `pyslth-0.1.9/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/utils.py` & `pyslth-0.1.9/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.1.8/slth/views.py` & `pyslth-0.1.9/slth/views.py`

 * *Files identical despite different names*

