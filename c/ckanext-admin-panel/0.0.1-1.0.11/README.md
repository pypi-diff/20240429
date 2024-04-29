# Comparing `tmp/ckanext-admin-panel-0.0.1.tar.gz` & `tmp/ckanext_admin_panel-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-admin-panel-0.0.1.tar", last modified: Sun Jul 23 09:41:57 2023, max compression
+gzip compressed data, was "ckanext_admin_panel-1.0.11.tar", last modified: Mon Apr 29 10:45:02 2024, max compression
```

## Comparing `ckanext-admin-panel-0.0.1.tar` & `ckanext_admin_panel-1.0.11.tar`

### file list

```diff
@@ -1,61 +1,108 @@
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/
--rw-r--r--   0 berry     (1000) berry     (1000)    34500 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/LICENSE
--rw-r--r--   0 berry     (1000) berry     (1000)      207 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/MANIFEST.in
--rw-r--r--   0 berry     (1000) berry     (1000)     4059 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/PKG-INFO
--rw-r--r--   0 berry     (1000) berry     (1000)     3371 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/README.md
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/
--rw-r--r--   0 berry     (1000) berry     (1000)      221 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/__init__.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/__init__.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/assets/
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/assets/css/
--rw-r--r--   0 berry     (1000) berry     (1000)     8136 2023-06-29 13:29:17.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/assets/css/admin_panel.css
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/assets/js/
--rw-r--r--   0 berry     (1000) berry     (1000)      235 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/assets/js/ap-main.js
--rw-r--r--   0 berry     (1000) berry     (1000)     1006 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/assets/js/ap-nested-dropdown.js
--rw-r--r--   0 berry     (1000) berry     (1000)     1876 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/assets/js/ap-theme-switcher.js
--rw-r--r--   0 berry     (1000) berry     (1000)      358 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/assets/webassets.yml
--rw-r--r--   0 berry     (1000) berry     (1000)     1868 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/helpers.py
--rw-r--r--   0 berry     (1000) berry     (1000)      380 2023-06-19 08:36:10.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/interfaces.py
--rw-r--r--   0 berry     (1000) berry     (1000)      649 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/plugin.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/
--rw-r--r--   0 berry     (1000) berry     (1000)     1717 2023-06-29 13:25:11.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/base.html
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/
--rw-r--r--   0 berry     (1000) berry     (1000)     4261 2023-07-19 13:21:14.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/basic.html
--rw-r--r--   0 berry     (1000) berry     (1000)     2105 2023-06-29 13:27:08.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/config_list.html
--rw-r--r--   0 berry     (1000) berry     (1000)      556 2023-07-19 13:21:15.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/confirm_reset.html
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/snippets/
--rw-r--r--   0 berry     (1000) berry     (1000)      831 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/snippets/confirm_delete.html
--rw-r--r--   0 berry     (1000) berry     (1000)      189 2023-06-29 13:24:02.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/snippets/home_breadcrumb.html
--rw-r--r--   0 berry     (1000) berry     (1000)     1151 2023-06-29 13:25:57.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/trash.html
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/user/
--rw-r--r--   0 berry     (1000) berry     (1000)     2076 2023-07-19 13:15:48.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/config/user/user_list.html
--rw-r--r--   0 berry     (1000) berry     (1000)     2450 2023-07-19 13:21:12.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/panel_links.html
--rw-r--r--   0 berry     (1000) berry     (1000)      281 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/panel_search.html
--rw-r--r--   0 berry     (1000) berry     (1000)      934 2023-07-19 13:21:14.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/admin_panel/toolbar.html
--rw-r--r--   0 berry     (1000) berry     (1000)      178 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/header.html
--rw-r--r--   0 berry     (1000) berry     (1000)      333 2023-06-29 12:51:41.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/page.html
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/snippets/
--rw-r--r--   0 berry     (1000) berry     (1000)      171 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/templates/snippets/apply_color_schema.html
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/tests/
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/tests/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     1390 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/tests/test_plugin.py
--rw-r--r--   0 berry     (1000) berry     (1000)      270 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/types.py
--rw-r--r--   0 berry     (1000) berry     (1000)      608 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/utils.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext/admin_panel/views/
--rw-r--r--   0 berry     (1000) berry     (1000)      235 2023-06-29 13:30:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/views/__init__.py
--rw-r--r--   0 berry     (1000) berry     (1000)     8300 2023-06-29 13:28:45.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/views/basic.py
--rw-r--r--   0 berry     (1000) berry     (1000)      472 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/views/config.py
--rw-r--r--   0 berry     (1000) berry     (1000)     2564 2023-06-29 14:14:38.000000 ckanext-admin-panel-0.0.1/ckanext/admin_panel/views/user.py
-drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/ckanext_admin_panel.egg-info/
--rw-r--r--   0 berry     (1000) berry     (1000)     4059 2023-07-23 09:41:57.000000 ckanext-admin-panel-0.0.1/ckanext_admin_panel.egg-info/PKG-INFO
--rw-r--r--   0 berry     (1000) berry     (1000)     1860 2023-07-23 09:41:57.000000 ckanext-admin-panel-0.0.1/ckanext_admin_panel.egg-info/SOURCES.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        1 2023-07-23 09:41:57.000000 ckanext-admin-panel-0.0.1/ckanext_admin_panel.egg-info/dependency_links.txt
--rw-r--r--   0 berry     (1000) berry     (1000)      130 2023-07-23 09:41:57.000000 ckanext-admin-panel-0.0.1/ckanext_admin_panel.egg-info/entry_points.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        8 2023-07-23 09:41:57.000000 ckanext-admin-panel-0.0.1/ckanext_admin_panel.egg-info/namespace_packages.txt
--rw-r--r--   0 berry     (1000) berry     (1000)        8 2023-07-23 09:41:57.000000 ckanext-admin-panel-0.0.1/ckanext_admin_panel.egg-info/top_level.txt
--rw-r--r--   0 berry     (1000) berry     (1000)     2971 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/pyproject.toml
--rw-r--r--   0 berry     (1000) berry     (1000)        0 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/requirements.txt
--rw-r--r--   0 berry     (1000) berry     (1000)     1710 2023-07-23 09:41:57.297437 ckanext-admin-panel-0.0.1/setup.cfg
--rw-r--r--   0 berry     (1000) berry     (1000)      528 2023-06-19 08:34:19.000000 ckanext-admin-panel-0.0.1/setup.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/
+-rw-r--r--   0 berry     (1000) berry     (1000)    34500 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/LICENSE
+-rw-r--r--   0 berry     (1000) berry     (1000)      207 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/MANIFEST.in
+-rw-r--r--   0 berry     (1000) berry     (1000)     8109 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     6970 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/README.md
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/
+-rw-r--r--   0 berry     (1000) berry     (1000)      221 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/__init__.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_cron/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1324 2024-04-29 09:11:07.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/cli.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1252 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/col_renderers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_cron/collection/
+-rw-r--r--   0 berry     (1000) berry     (1000)       70 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/collection/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4444 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/collection/cron.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      251 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      248 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/const.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1384 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/helpers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      417 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/interfaces.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2654 2024-04-29 09:18:55.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/action.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      784 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/auth.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3094 2024-04-29 08:59:14.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/schema.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2219 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/logic/validators.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3406 2024-04-29 07:22:40.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/model.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2637 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      418 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/types.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3701 2024-04-29 09:54:16.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/utils.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     7768 2024-04-29 08:21:06.000000 ckanext_admin_panel-1.0.11/ckanext/ap_cron/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_doi/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-22 08:08:05.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4375 2024-04-23 09:06:42.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/collection.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      216 2024-04-23 12:04:03.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)       39 2024-04-22 08:20:24.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/const.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4042 2024-04-24 10:10:27.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4160 2024-04-23 10:19:36.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/utils.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3662 2024-04-24 10:08:37.000000 ckanext_admin_panel-1.0.11/ckanext/ap_doi/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_example/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_example/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2257 2024-04-24 10:11:27.000000 ckanext_admin_panel-1.0.11/ckanext/ap_example/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1553 2024-04-24 10:08:30.000000 ckanext_admin_panel-1.0.11/ckanext/ap_example/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_log/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      529 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/col_renderers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4146 2024-04-23 14:19:12.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/collection.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      823 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/log_handlers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_log/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2207 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/model.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1693 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1195 2024-04-29 07:56:45.000000 ckanext_admin_panel-1.0.11/ckanext/ap_log/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2482 2024-04-29 10:43:14.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/col_renderers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/
+-rw-r--r--   0 berry     (1000) berry     (1000)      134 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     3332 2024-04-22 18:25:05.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/base.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     6406 2024-04-29 10:41:23.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/content.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4713 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/collection/user.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      350 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5267 2024-04-24 10:08:44.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/helpers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      716 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/interfaces.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4799 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/action.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      285 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/auth.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      689 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/logic/schema.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2196 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/plugin.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/tests/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/tests/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      212 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/tests/test_plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      706 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/types.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1108 2024-04-24 09:55:12.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/utils.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/
+-rw-r--r--   0 berry     (1000) berry     (1000)      291 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5750 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/basic.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      467 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4530 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/content.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4750 2024-04-25 10:25:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/generics.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     5767 2024-04-23 08:23:29.000000 ckanext_admin_panel-1.0.11/ckanext/ap_main/views/user.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_support/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      497 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/col_renderers.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4648 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/collection.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      353 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/config.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      309 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/helpers.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/
+-rw-r--r--   0 berry     (1000) berry     (1000)        0 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/__init__.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2268 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/action.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      545 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/auth.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1527 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/schema.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      773 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/logic/validators.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     2692 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/model.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     1995 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/plugin.py
+-rw-r--r--   0 berry     (1000) berry     (1000)      330 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/types.py
+-rw-r--r--   0 berry     (1000) berry     (1000)     4646 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/ckanext/ap_support/views.py
+drwxr-xr-x   0 berry     (1000) berry     (1000)        0 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/
+-rw-r--r--   0 berry     (1000) berry     (1000)     8109 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/PKG-INFO
+-rw-r--r--   0 berry     (1000) berry     (1000)     2670 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/SOURCES.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        1 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/dependency_links.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)      560 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/entry_points.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/namespace_packages.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)      265 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/requires.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)        8 2024-04-29 10:45:02.000000 ckanext_admin_panel-1.0.11/ckanext_admin_panel.egg-info/top_level.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     2974 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/pyproject.toml
+-rw-r--r--   0 berry     (1000) berry     (1000)       16 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/requirements.txt
+-rw-r--r--   0 berry     (1000) berry     (1000)     2240 2024-04-29 10:45:02.923523 ckanext_admin_panel-1.0.11/setup.cfg
+-rw-r--r--   0 berry     (1000) berry     (1000)      528 2024-04-18 11:33:20.000000 ckanext_admin_panel-1.0.11/setup.py
```

### Comparing `ckanext-admin-panel-0.0.1/LICENSE` & `ckanext_admin_panel-1.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-admin-panel-0.0.1/pyproject.toml` & `ckanext_admin_panel-1.0.11/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 [tool.ruff]
 target-version = "py38"
 
 [tool.isort]
 known_ckan = "ckan"
 known_ckanext = "ckanext"
-known_self = "ckanext.nwg"
+known_self = "ckanext.ap_main"
 sections = "FUTURE,STDLIB,FIRSTPARTY,THIRDPARTY,CKAN,CKANEXT,SELF,LOCALFOLDER"
 
 [tool.pytest.ini_options]
 addopts = "--ckan-ini test.ini"
 filterwarnings = [
                "ignore::sqlalchemy.exc.SADeprecationWarning",
                "ignore::sqlalchemy.exc.SAWarning",
                "ignore::DeprecationWarning",
 ]
 
 [tool.pyright]
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 include = ["ckanext"]
 exclude = [
     "**/test*",
     "**/migration",
 ]
 strict = []
 
@@ -87,8 +87,7 @@
 reportUnboundVariable = true
 reportInvalidStubStatement = true
 reportIncompleteStub = true
 reportUnsupportedDunderAll = true
 reportUnusedCoroutine = true
 reportUnnecessaryTypeIgnoreComment = true
 reportMatchNotExhaustive = true
-
```

### Comparing `ckanext-admin-panel-0.0.1/setup.py` & `ckanext_admin_panel-1.0.11/setup.py`

 * *Files identical despite different names*

