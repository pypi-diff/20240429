# Comparing `tmp/libreflow_launcher-1.0.2.tar.gz` & `tmp/libreflow_launcher-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_launcher-1.0.2.tar", last modified: Thu Apr 25 15:14:36 2024, max compression
+gzip compressed data, was "libreflow_launcher-1.0.3.tar", last modified: Mon Apr 29 14:28:32 2024, max compression
```

## Comparing `libreflow_launcher-1.0.2.tar` & `libreflow_launcher-1.0.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.592540 libreflow_launcher-1.0.2/
--rw-rw-rw-   0 root         (0) root         (0)      907 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1696 2024-04-25 15:14:36.592540 libreflow_launcher-1.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-04-25 15:14:36.592540 libreflow_launcher-1.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1691 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.576540 libreflow_launcher-1.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.581540 libreflow_launcher-1.0.2/src/libreflow_launcher/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-25 15:14:36.592540 libreflow_launcher-1.0.2/src/libreflow_launcher/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    18068 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.582540 libreflow_launcher-1.0.2/src/libreflow_launcher/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.582540 libreflow_launcher-1.0.2/src/libreflow_launcher/data/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/data/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/gui.py
--rw-rw-rw-   0 root         (0) root         (0)     6069 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7983 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.583540 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.585540 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   503824 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   445528 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   579296 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
--rw-rw-rw-   0 root         (0) root         (0)   528976 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/OpenSans.ttf
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.586540 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.590540 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5628 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)     5667 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     9732 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/close.png
--rw-rw-rw-   0 root         (0) root         (0)     9850 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/gitlab.svg
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/kitsu.svg
--rw-rw-rw-   0 root         (0) root         (0)     8760 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/log-out.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
--rw-rw-rw-   0 root         (0) root         (0)     7267 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/open.png
--rw-rw-rw-   0 root         (0) root         (0)    10491 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/pypi.svg
--rw-rw-rw-   0 root         (0) root         (0)    17905 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/server.png
--rw-rw-rw-   0 root         (0) root         (0)    13119 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/settings.png
--rw-rw-rw-   0 root         (0) root         (0)    19182 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/settings_outline.png
--rw-rw-rw-   0 root         (0) root         (0)     5851 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/start.png
--rw-rw-rw-   0 root         (0) root         (0)     7946 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/trash.png
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/trash_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     7996 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/trash_normal.png
--rw-rw-rw-   0 root         (0) root         (0)    11968 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/user.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.591540 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.591540 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/styles/default/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/styles/default/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/ui/styles/default/default_style.css
--rw-rw-rw-   0 root         (0) root         (0)    55947 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/src/libreflow_launcher/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 15:14:36.591540 libreflow_launcher-1.0.2/src/libreflow_launcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1696 2024-04-25 15:14:36.000000 libreflow_launcher-1.0.2/src/libreflow_launcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2191 2024-04-25 15:14:36.000000 libreflow_launcher-1.0.2/src/libreflow_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 15:14:36.000000 libreflow_launcher-1.0.2/src/libreflow_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-25 15:14:36.000000 libreflow_launcher-1.0.2/src/libreflow_launcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-25 15:14:36.000000 libreflow_launcher-1.0.2/src/libreflow_launcher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-25 15:14:27.000000 libreflow_launcher-1.0.2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.897462 libreflow_launcher-1.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-04-29 14:28:32.897462 libreflow_launcher-1.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-04-29 14:28:32.897462 libreflow_launcher-1.0.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.881462 libreflow_launcher-1.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.885462 libreflow_launcher-1.0.3/src/libreflow_launcher/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-29 14:28:32.898462 libreflow_launcher-1.0.3/src/libreflow_launcher/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    18068 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.887462 libreflow_launcher-1.0.3/src/libreflow_launcher/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.887462 libreflow_launcher-1.0.3/src/libreflow_launcher/data/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/data/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     6069 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7983 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.887462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.890462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   503824 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   445528 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   579296 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   528976 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/OpenSans.ttf
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.890462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.895462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/arrow-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     9732 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/close.png
+-rw-rw-rw-   0 root         (0) root         (0)     9850 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/gitlab.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/kitsu.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/open.png
+-rw-rw-rw-   0 root         (0) root         (0)    10491 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/pypi.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17905 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/server.png
+-rw-rw-rw-   0 root         (0) root         (0)    13119 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/settings.png
+-rw-rw-rw-   0 root         (0) root         (0)    19182 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/settings_outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/start.png
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash.png
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     7996 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)    11968 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/user.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.896462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.896462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/default/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/default/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/default/default_style.css
+-rw-rw-rw-   0 root         (0) root         (0)    56132 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.896462 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1859 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2191 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/versioneer.py
```

### Comparing `libreflow_launcher-1.0.2/CHANGELOG.md` & `libreflow_launcher-1.0.3/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
-### Added
-
-### Changed
+## [1.0.3] - 2024-04-29
 
 ### Fixed
 
-## [1.0.0] - 2024-04-25
+* Host address for a server can now be a domain name instead of a direct IP address.
+  * The default port is `5500` if you don't specify it in the wizard.
+
+## [1.0.0-1.0.2] - 2024-04-25
 
 Initial public commit and pypi setup. This is an early version of Libreflow Launcher.
 It includes management of Overseer servers, access to projects (instances of Libreflow) that have been assigned to the user, and can be installed locally on the machine by Poetry.
 
 The user interface is likely to change in the future.
```

### Comparing `libreflow_launcher-1.0.2/PKG-INFO` & `libreflow_launcher-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.2
+Version: 1.0.3
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,19 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
-### Added
-
-### Changed
+## [1.0.3] - 2024-04-29
 
 ### Fixed
 
-## [1.0.0] - 2024-04-25
+* Host address for a server can now be a domain name instead of a direct IP address.
+  * The default port is `5500` if you don't specify it in the wizard.
+
+## [1.0.0-1.0.2] - 2024-04-25
 
 Initial public commit and pypi setup. This is an early version of Libreflow Launcher.
 It includes management of Overseer servers, access to projects (instances of Libreflow) that have been assigned to the user, and can be installed locally on the machine by Poetry.
 
 The user interface is likely to change in the future.
```

### Comparing `libreflow_launcher-1.0.2/README.md` & `libreflow_launcher-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/setup.py` & `libreflow_launcher-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/controller.py` & `libreflow_launcher-1.0.3/src/libreflow_launcher/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def strip_accents(s):
     return ''.join(c for c in unicodedata.normalize('NFD', s)
                    if unicodedata.category(c) != 'Mn')
 
 
 class Controller():
 
-    BASE_URL = 'http://0.0.0.0:0000'
+    BASE_URL = 'http://0.0.0.0:5500'
     
     server_name = None
     server_uid = None
     
     current_user = None
     
     CONFIG = {'headers': None}
```

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/gui.py` & `libreflow_launcher-1.0.3/src/libreflow_launcher/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/model.py` & `libreflow_launcher-1.0.3/src/libreflow_launcher/model.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/resources.py` & `libreflow_launcher-1.0.3/src/libreflow_launcher/resources.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/fonts/OpenSans.ttf` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/OpenSans.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/arrow-down.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/arrow-down.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/arrow-right.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/close.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/close.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/gitlab.svg` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/gitlab.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/kitsu.svg` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/kitsu.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/log-out.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/log-out_hover.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/log-out_normal.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/open.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/open.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/pypi.svg` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/pypi.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/server.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/server.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/settings.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/settings.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/settings_outline.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/settings_outline.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/start.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/start.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/trash.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/trash_hover.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/trash_normal.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/icons/gui/user.png` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/user.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/ui/styles/default/default_style.css` & `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/default/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher/view.py` & `libreflow_launcher-1.0.3/src/libreflow_launcher/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,16 @@
         if self.text() == '':
             if "mandatory" in self.options:
                 self.setProperty('warning', True)
                 self.setToolTip('You cannot leave this parameter empty.')
                 return False
         
         if "host" in self.options:
-            if not re.match(r'^[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\:[0-9]{1,5}$', self.text()):
+            host_regex = r'^(?:\b(?!\bhttp[s]{0,1})([a-zA-Z\.\/]+)|(\d+\.\d+.\d+.\d+))(?::(\d{1,5}))?'
+            if re.match(host_regex, self.text()) is None:
                 self.setProperty('warning', True)
                 self.setToolTip('Host format is not valid.')
                 return False
 
         return True
 
     def reveal_explorer(self):
@@ -604,18 +605,24 @@
 
     def _on_add_button_clicked(self):
         for i in range(self.server_lo.count()):
             widget = self.server_lo.itemAt(i).widget()
             if widget.property('warning'):
                 return
 
+        api_host = self.host_input.text()
+        api_port = '5500'
+        
+        if ':' in self.host_input.text():
+            api_host, api_port = self.host_input.text().split(':')
+
         data = dict(
             display_name=self.name_input.text(),
-            api_host=self.host_input.text().split(':')[0],
-            api_port=self.host_input.text().split(':')[1]
+            api_host=api_host,
+            api_port=api_port
         )
         uid = self._ctrl.update_server(data)
         self._mw.page_refresh('projects', True)
 
 
 class SettingsPage(QtWidgets.QFrame):
```

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher.egg-info/PKG-INFO` & `libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.2
+Version: 1.0.3
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,19 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
-### Added
-
-### Changed
+## [1.0.3] - 2024-04-29
 
 ### Fixed
 
-## [1.0.0] - 2024-04-25
+* Host address for a server can now be a domain name instead of a direct IP address.
+  * The default port is `5500` if you don't specify it in the wizard.
+
+## [1.0.0-1.0.2] - 2024-04-25
 
 Initial public commit and pypi setup. This is an early version of Libreflow Launcher.
 It includes management of Overseer servers, access to projects (instances of Libreflow) that have been assigned to the user, and can be installed locally on the machine by Poetry.
 
 The user interface is likely to change in the future.
```

### Comparing `libreflow_launcher-1.0.2/src/libreflow_launcher.egg-info/SOURCES.txt` & `libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.2/versioneer.py` & `libreflow_launcher-1.0.3/versioneer.py`

 * *Files identical despite different names*

