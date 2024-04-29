# Comparing `tmp/libreflow_launcher-1.0.3.tar.gz` & `tmp/libreflow_launcher-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreflow_launcher-1.0.3.tar", last modified: Mon Apr 29 14:28:32 2024, max compression
+gzip compressed data, was "libreflow_launcher-1.0.4.tar", last modified: Mon Apr 29 15:33:49 2024, max compression
```

## Comparing `libreflow_launcher-1.0.3.tar` & `libreflow_launcher-1.0.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.897462 libreflow_launcher-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1859 2024-04-29 14:28:32.897462 libreflow_launcher-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-04-29 14:28:32.897462 libreflow_launcher-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1691 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.881462 libreflow_launcher-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.885462 libreflow_launcher-1.0.3/src/libreflow_launcher/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-29 14:28:32.898462 libreflow_launcher-1.0.3/src/libreflow_launcher/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    18068 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.887462 libreflow_launcher-1.0.3/src/libreflow_launcher/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.887462 libreflow_launcher-1.0.3/src/libreflow_launcher/data/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/data/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/gui.py
--rw-rw-rw-   0 root         (0) root         (0)     6069 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/model.py
--rw-rw-rw-   0 root         (0) root         (0)     7983 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.887462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.890462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   503824 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   445528 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
--rw-rw-rw-   0 root         (0) root         (0)   579296 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
--rw-rw-rw-   0 root         (0) root         (0)   528976 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/OpenSans.ttf
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.890462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.895462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5628 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/arrow-down.png
--rw-rw-rw-   0 root         (0) root         (0)     5667 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/arrow-right.png
--rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
--rw-rw-rw-   0 root         (0) root         (0)     9732 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/close.png
--rw-rw-rw-   0 root         (0) root         (0)     9850 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
--rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/gitlab.svg
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/kitsu.svg
--rw-rw-rw-   0 root         (0) root         (0)     8760 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
--rw-rw-rw-   0 root         (0) root         (0)     7267 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/open.png
--rw-rw-rw-   0 root         (0) root         (0)    10491 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/pypi.svg
--rw-rw-rw-   0 root         (0) root         (0)    17905 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/server.png
--rw-rw-rw-   0 root         (0) root         (0)    13119 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/settings.png
--rw-rw-rw-   0 root         (0) root         (0)    19182 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/settings_outline.png
--rw-rw-rw-   0 root         (0) root         (0)     5851 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/start.png
--rw-rw-rw-   0 root         (0) root         (0)     7946 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash.png
--rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash_hover.png
--rw-rw-rw-   0 root         (0) root         (0)     7996 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash_normal.png
--rw-rw-rw-   0 root         (0) root         (0)    11968 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/user.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.896462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.896462 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/default/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/default/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/default/default_style.css
--rw-rw-rw-   0 root         (0) root         (0)    56132 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/src/libreflow_launcher/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 14:28:32.896462 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1859 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2191 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-29 14:28:32.000000 libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-29 14:28:22.000000 libreflow_launcher-1.0.3/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.832674 libreflow_launcher-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-04-29 15:33:49.832674 libreflow_launcher-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-04-29 15:33:49.833674 libreflow_launcher-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.814674 libreflow_launcher-1.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.821674 libreflow_launcher-1.0.4/src/libreflow_launcher/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-29 15:33:49.833674 libreflow_launcher-1.0.4/src/libreflow_launcher/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    18205 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.822674 libreflow_launcher-1.0.4/src/libreflow_launcher/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.823674 libreflow_launcher-1.0.4/src/libreflow_launcher/data/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/data/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     6069 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     7983 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.823674 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.826674 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   503824 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   445528 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   579296 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf
+-rw-rw-rw-   0 root         (0) root         (0)   528976 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/OpenSans.ttf
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.826674 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.831673 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/arrow-down.png
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/arrow-right.png
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png
+-rw-rw-rw-   0 root         (0) root         (0)     9732 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/close.png
+-rw-rw-rw-   0 root         (0) root         (0)     9850 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/gitlab.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/kitsu.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/log-out.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/log-out_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/log-out_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/open.png
+-rw-rw-rw-   0 root         (0) root         (0)    10491 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/pypi.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17905 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/server.png
+-rw-rw-rw-   0 root         (0) root         (0)    13119 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/settings.png
+-rw-rw-rw-   0 root         (0) root         (0)    19182 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/settings_outline.png
+-rw-rw-rw-   0 root         (0) root         (0)     5851 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/start.png
+-rw-rw-rw-   0 root         (0) root         (0)     7946 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/trash.png
+-rw-rw-rw-   0 root         (0) root         (0)     8358 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/trash_hover.png
+-rw-rw-rw-   0 root         (0) root         (0)     7996 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/trash_normal.png
+-rw-rw-rw-   0 root         (0) root         (0)    11968 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/user.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.831673 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/styles/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/styles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.832674 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/styles/default/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/styles/default/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5049 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/ui/styles/default/default_style.css
+-rw-rw-rw-   0 root         (0) root         (0)    56132 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/src/libreflow_launcher/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:33:49.832674 libreflow_launcher-1.0.4/src/libreflow_launcher.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1998 2024-04-29 15:33:49.000000 libreflow_launcher-1.0.4/src/libreflow_launcher.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2191 2024-04-29 15:33:49.000000 libreflow_launcher-1.0.4/src/libreflow_launcher.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 15:33:49.000000 libreflow_launcher-1.0.4/src/libreflow_launcher.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-29 15:33:49.000000 libreflow_launcher-1.0.4/src/libreflow_launcher.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-29 15:33:49.000000 libreflow_launcher-1.0.4/src/libreflow_launcher.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    86677 2024-04-29 15:33:39.000000 libreflow_launcher-1.0.4/versioneer.py
```

### Comparing `libreflow_launcher-1.0.3/CHANGELOG.md` & `libreflow_launcher-1.0.4/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.4] - 2024-04-29
+
+### Added
+
+* An environment variable `LF_LAUNCHER_POETRY_PATH` can be used to define a specific path for poetry.
+
 ## [1.0.3] - 2024-04-29
 
 ### Fixed
 
 * Host address for a server can now be a domain name instead of a direct IP address.
   * The default port is `5500` if you don't specify it in the wizard.
```

### Comparing `libreflow_launcher-1.0.3/PKG-INFO` & `libreflow_launcher-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.3
+Version: 1.0.4
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.4] - 2024-04-29
+
+### Added
+
+* An environment variable `LF_LAUNCHER_POETRY_PATH` can be used to define a specific path for poetry.
+
 ## [1.0.3] - 2024-04-29
 
 ### Fixed
 
 * Host address for a server can now be a domain name instead of a direct IP address.
   * The default port is `5500` if you don't specify it in the wizard.
```

### Comparing `libreflow_launcher-1.0.3/README.md` & `libreflow_launcher-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/setup.py` & `libreflow_launcher-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/controller.py` & `libreflow_launcher-1.0.4/src/libreflow_launcher/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,17 @@
                         ))
                 except IOError as e:
                     continue
         
         return sorted(versions, key=lambda d: d['version'])
 
     def fetch_poetry_path(self):
-        if platform.system() == "Windows":
+        if os.getenv('LF_LAUNCHER_POETRY_PATH', None) is not None:
+            self.poetry_path = os.getenv('LF_LAUNCHER_POETRY_PATH')
+        elif platform.system() == "Windows":
             self.poetry_path = f"{pathlib.Path.home()}/AppData/Roaming/Python/Scripts/poetry"
         elif platform.system() == "Linux":
             self.poetry_path = f"{pathlib.Path.home()}/.local/bin/poetry"
 
     def user_settings_folder(self):
         return os.path.join(pathlib.Path.home(), '.libreflow_launcher')
```

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/gui.py` & `libreflow_launcher-1.0.4/src/libreflow_launcher/gui.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/model.py` & `libreflow_launcher-1.0.4/src/libreflow_launcher/model.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/resources.py` & `libreflow_launcher-1.0.4/src/libreflow_launcher/resources.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/Asap-Italic-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/Asap-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/fonts/OpenSans.ttf` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/fonts/OpenSans.ttf`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/arrow-down.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/arrow-down.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/arrow-right.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/arrow-right.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/circular-shape-silhouette.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/close.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/close.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/feespeciales_icon.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/gitlab.svg` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/gitlab.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/kitsu.svg` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/kitsu.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/log-out.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out_hover.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/log-out_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/log-out_normal.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/log-out_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/open.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/open.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/pypi.svg` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/pypi.svg`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/server.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/server.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/settings.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/settings.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/settings_outline.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/settings_outline.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/start.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/start.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/trash.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash_hover.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/trash_hover.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/trash_normal.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/trash_normal.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/icons/gui/user.png` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/icons/gui/user.png`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/ui/styles/default/default_style.css` & `libreflow_launcher-1.0.4/src/libreflow_launcher/ui/styles/default/default_style.css`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher/view.py` & `libreflow_launcher-1.0.4/src/libreflow_launcher/view.py`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/PKG-INFO` & `libreflow_launcher-1.0.4/src/libreflow_launcher.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreflow_launcher
-Version: 1.0.3
+Version: 1.0.4
 Summary: Launcher for instances of Libreflow asset-manager
 Home-page: https://gitlab.com/lfs.coop/libreflow/libreflow_launcher
 Author: Valentin Braem
 Author-email: valentin.braem@les-fees-speciales.coop
 License: LGPLv3+
 Keywords: kabaret kitsu gazu animation pipeline libreflow launcher lfs overseer asset-manager
 Classifier: Programming Language :: Python :: 3
@@ -36,14 +36,20 @@
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
 -->
 
 ## [Unreleased]
 
+## [1.0.4] - 2024-04-29
+
+### Added
+
+* An environment variable `LF_LAUNCHER_POETRY_PATH` can be used to define a specific path for poetry.
+
 ## [1.0.3] - 2024-04-29
 
 ### Fixed
 
 * Host address for a server can now be a domain name instead of a direct IP address.
   * The default port is `5500` if you don't specify it in the wizard.
```

### Comparing `libreflow_launcher-1.0.3/src/libreflow_launcher.egg-info/SOURCES.txt` & `libreflow_launcher-1.0.4/src/libreflow_launcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libreflow_launcher-1.0.3/versioneer.py` & `libreflow_launcher-1.0.4/versioneer.py`

 * *Files identical despite different names*
