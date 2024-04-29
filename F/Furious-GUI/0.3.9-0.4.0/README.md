# Comparing `tmp/Furious-GUI-0.3.9.tar.gz` & `tmp/Furious-GUI-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Furious-GUI-0.3.9.tar", last modified: Sat Mar  9 11:19:51 2024, max compression
+gzip compressed data, was "Furious-GUI-0.4.0.tar", last modified: Mon Apr 29 10:39:16 2024, max compression
```

## Comparing `Furious-GUI-0.3.9.tar` & `Furious-GUI-0.4.0.tar`

### file list

```diff
@@ -1,114 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.773250 Furious-GUI-0.3.9/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.725250 Furious-GUI-0.3.9/Furious/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.725250 Furious-GUI-0.3.9/Furious/Core/
--rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Core/CoreManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Core/Hysteria1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Core/Hysteria2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Core/Tun2socks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Core/XrayCore.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.725250 Furious-GUI-0.3.9/Furious/Data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.729250 Furious-GUI-0.3.9/Furious/Data/font/
--rw-r--r--   0 runner    (1001) docker     (127)   624892 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Data/font/CascadiaMono
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Data/font/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.733250 Furious-GUI-0.3.9/Furious/Data/hysteria/
--rw-r--r--   0 runner    (1001) docker     (127)  1974430 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Data/hysteria/bypass-Iran.acl
--rw-r--r--   0 runner    (1001) docker     (127)  1390176 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Data/hysteria/bypass-mainland-China.acl
--rw-r--r--   0 runner    (1001) docker     (127)  6336270 2024-03-09 11:19:32.000000 Furious-GUI-0.3.9/Furious/Data/hysteria/country.mmdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.757250 Furious-GUI-0.3.9/Furious/Data/xray/
--rw-r--r--   0 runner    (1001) docker     (127) 10853925 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Data/xray/geoip.dat
--rw-r--r--   0 runner    (1001) docker     (127)  5234287 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Data/xray/geosite.dat
--rw-r--r--   0 runner    (1001) docker     (127)  3199463 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Data/xray/iran.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.761250 Furious-GUI-0.3.9/Furious/Externals/
--rw-r--r--   0 runner    (1001) docker     (127)    26561 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Externals/GenTranslation.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Externals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.765250 Furious-GUI-0.3.9/Furious/Interface/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Interface/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Interface/ConfigurationFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Interface/CoreFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Interface/Encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Interface/ItemUpdateProtocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Interface/Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Interface/UserServersTableItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.765250 Furious-GUI-0.3.9/Furious/Library/
--rw-r--r--   0 runner    (1001) docker     (127)    48930 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Library/Configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Library/Encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Library/Tcping.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.765250 Furious-GUI-0.3.9/Furious/PyFramework/
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/PyFramework/Ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/PyFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.765250 Furious-GUI-0.3.9/Furious/QtFramework/
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/Ancestors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/CoreProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/DNSResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/DynamicTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/DynamicTranslate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/NetworkStateManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/QtGui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/QtNetwork.py
--rw-r--r--   0 runner    (1001) docker     (127)    16275 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/QtWidgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/TextEditor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/TextEditorTheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/UpdatesManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/QtFramework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.769250 Furious-GUI-0.3.9/Furious/Storage/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Storage/UserServers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Storage/UserSubs.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.769250 Furious-GUI-0.3.9/Furious/TrayActions/
--rw-r--r--   0 runner    (1001) docker     (127)    10292 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/Connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/EditConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/Exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/Import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/Language.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/Routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/SystemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/TrayActions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.769250 Furious-GUI-0.3.9/Furious/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/AppMainProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)    71000 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/AppResources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/AppSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/AppSettingsFn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/PySide6Legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/StartupOnBoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/SystemProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/SystemRoutingTable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/SystemRuntime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/Utility.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.773250 Furious-GUI-0.3.9/Furious/Widget/
--rw-r--r--   0 runner    (1001) docker     (127)    12009 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Widget/Application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Widget/ConnectProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Widget/IndentSpinBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Widget/SystemTrayIcon.py
--rw-r--r--   0 runner    (1001) docker     (127)    44098 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Widget/UserServersQTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Widget/UserSubsQTableWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Widget/XrayAssetViewerQListWidget.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.773250 Furious-GUI-0.3.9/Furious/Window/
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Window/AppMainWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Window/LogViewerWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Window/QRCodeWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Window/TextEditorWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Window/UserSubsWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Window/XrayAssetViewerWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/Window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/Furious/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 11:19:51.773250 Furious-GUI-0.3.9/Furious_GUI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-09 11:19:51.000000 Furious-GUI-0.3.9/Furious_GUI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-03-09 11:19:51.000000 Furious-GUI-0.3.9/Furious_GUI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 11:19:51.000000 Furious-GUI-0.3.9/Furious_GUI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-09 11:19:51.000000 Furious-GUI-0.3.9/Furious_GUI.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-09 11:19:51.000000 Furious-GUI-0.3.9/Furious_GUI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-09 11:19:51.000000 Furious-GUI-0.3.9/Furious_GUI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-09 11:19:51.773250 Furious-GUI-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 11:19:51.773250 Furious-GUI-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-09 11:19:33.000000 Furious-GUI-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.172474 Furious-GUI-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.124474 Furious-GUI-0.4.0/Furious/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.124474 Furious-GUI-0.4.0/Furious/Core/
+-rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Core/CoreManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Core/Hysteria1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Core/Hysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Core/Tun2socks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Core/XrayCore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.120474 Furious-GUI-0.4.0/Furious/Data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.124474 Furious-GUI-0.4.0/Furious/Data/font/
+-rw-r--r--   0 runner    (1001) docker     (127)   624892 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Data/font/CascadiaMono
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Data/font/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.128474 Furious-GUI-0.4.0/Furious/Data/hysteria/
+-rw-r--r--   0 runner    (1001) docker     (127)  1974430 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Data/hysteria/bypass-Iran.acl
+-rw-r--r--   0 runner    (1001) docker     (127)  1390176 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Data/hysteria/bypass-mainland-China.acl
+-rw-r--r--   0 runner    (1001) docker     (127)  6336270 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Data/hysteria/country.mmdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.156474 Furious-GUI-0.4.0/Furious/Data/xray/
+-rw-r--r--   0 runner    (1001) docker     (127) 10853925 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Data/xray/geoip.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  5234287 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Data/xray/geosite.dat
+-rw-r--r--   0 runner    (1001) docker     (127)  3199463 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Data/xray/iran.dat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.160474 Furious-GUI-0.4.0/Furious/Externals/
+-rw-r--r--   0 runner    (1001) docker     (127)    30336 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Externals/GenTranslation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Externals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.160474 Furious-GUI-0.4.0/Furious/Interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/ConfigurationFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/CoreFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/Encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/GuiEditorItemFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/ItemUpdateProtocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/UserServersTableItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.160474 Furious-GUI-0.4.0/Furious/Library/
+-rw-r--r--   0 runner    (1001) docker     (127)    55774 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Library/Configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Library/EmptyFactoryHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Library/Encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Library/Tcping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.160474 Furious-GUI-0.4.0/Furious/PyFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/PyFramework/Ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/PyFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.164474 Furious-GUI-0.4.0/Furious/QtFramework/
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/Ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5970 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/CoreProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/DNSResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/DynamicTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/DynamicTranslate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11372 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/GuiEditorXXX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/NetworkStateManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/QtGui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/QtNetwork.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16523 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/QtWidgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/TextEditor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/TextEditorTheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/UpdatesManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/QtFramework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.164474 Furious-GUI-0.4.0/Furious/Storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Storage/UserServers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Storage/UserSubs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.164474 Furious-GUI-0.4.0/Furious/TrayActions/
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/Connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/EditConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/Exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/Import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/Language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/Routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/SystemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/TrayActions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.168474 Furious-GUI-0.4.0/Furious/Utility/
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/AppMainProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80238 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/AppResources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/AppSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/AppSettingsFn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/PySide6Legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/StartupOnBoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/SystemProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/SystemRoutingTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/SystemRuntime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/Utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.168474 Furious-GUI-0.4.0/Furious/Widget/
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/Application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/ConnectProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9602 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/GuiHysteria1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/GuiHysteria2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/GuiShadowsocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/GuiTrojan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9638 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/GuiVLESS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/GuiVMess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16043 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/GuiVTLS.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32650 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/GuiVTransport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/IndentSpinBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6972 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/SystemTrayIcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49147 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/UserServersQTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/UserSubsQTableWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/XrayAssetViewerQListWidget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.168474 Furious-GUI-0.4.0/Furious/Window/
+-rw-r--r--   0 runner    (1001) docker     (127)    15031 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Window/AppMainWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Window/LogViewerWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Window/QRCodeWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14078 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Window/TextEditorWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Window/UserSubsWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Window/XrayAssetViewerWindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/Window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/Furious/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:39:16.172474 Furious-GUI-0.4.0/Furious_GUI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-29 10:39:16.000000 Furious-GUI-0.4.0/Furious_GUI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-29 10:39:16.000000 Furious-GUI-0.4.0/Furious_GUI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:39:16.000000 Furious-GUI-0.4.0/Furious_GUI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-29 10:39:16.000000 Furious-GUI-0.4.0/Furious_GUI.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-29 10:39:16.000000 Furious-GUI-0.4.0/Furious_GUI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 10:39:16.000000 Furious-GUI-0.4.0/Furious_GUI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-29 10:39:16.172474 Furious-GUI-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:39:16.172474 Furious-GUI-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-29 10:38:50.000000 Furious-GUI-0.4.0/setup.py
```

### Comparing `Furious-GUI-0.3.9/Furious/Core/CoreManager.py` & `Furious-GUI-0.4.0/Furious/Core/CoreManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Core/Hysteria1.py` & `Furious-GUI-0.4.0/Furious/Core/Hysteria1.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Core/Hysteria2.py` & `Furious-GUI-0.4.0/Furious/Core/Hysteria2.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Core/Tun2socks.py` & `Furious-GUI-0.4.0/Furious/Core/Tun2socks.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Core/XrayCore.py` & `Furious-GUI-0.4.0/Furious/Core/XrayCore.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Core/__init__.py` & `Furious-GUI-0.4.0/Furious/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Data/font/CascadiaMono` & `Furious-GUI-0.4.0/Furious/Data/font/CascadiaMono`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Data/font/LICENSE` & `Furious-GUI-0.4.0/Furious/Data/font/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Data/hysteria/bypass-Iran.acl` & `Furious-GUI-0.4.0/Furious/Data/hysteria/bypass-Iran.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Data/hysteria/bypass-mainland-China.acl` & `Furious-GUI-0.4.0/Furious/Data/hysteria/bypass-mainland-China.acl`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Data/hysteria/country.mmdb` & `Furious-GUI-0.4.0/Furious/Data/hysteria/country.mmdb`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Data/xray/geoip.dat` & `Furious-GUI-0.4.0/Furious/Data/xray/geoip.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Data/xray/geosite.dat` & `Furious-GUI-0.4.0/Furious/Data/xray/geosite.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Data/xray/iran.dat` & `Furious-GUI-0.4.0/Furious/Data/xray/iran.dat`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Externals/GenTranslation.py` & `Furious-GUI-0.4.0/Furious/Externals/GenTranslation.py`

 * *Files 8% similar despite different names*

```diff
@@ -166,14 +166,15 @@
             "Furious.Widget.IndentSpinBox"
         ],
         "ZH": "缩进：",
         "isReviewed": "True"
     },
     "Cancel": {
         "source": [
+            "Furious.QtFramework.GuiEditorXXX",
             "Furious.Widget.IndentSpinBox",
             "Furious.Window.TextEditorWindow",
             "Furious.Window.UserSubsWindow"
         ],
         "ZH": "取消",
         "isReviewed": "True"
     },
@@ -358,43 +359,55 @@
             "Furious.Window.TextEditorWindow"
         ],
         "ZH": "设置缩进出错",
         "isReviewed": "True"
     },
     "Remark": {
         "source": [
+            "Furious.Widget.GuiHysteria1",
+            "Furious.Widget.GuiHysteria2",
             "Furious.Widget.UserServersQTableWidget",
             "Furious.Widget.UserSubsQTableWidget"
         ],
         "ZH": "别名",
         "isReviewed": "True"
     },
     "Protocol": {
         "source": [
+            "Furious.Widget.GuiHysteria1",
             "Furious.Widget.UserServersQTableWidget"
         ],
         "ZH": "协议",
         "isReviewed": "True"
     },
     "Address": {
         "source": [
+            "Furious.Widget.GuiShadowsocks",
+            "Furious.Widget.GuiTrojan",
+            "Furious.Widget.GuiVLESS",
+            "Furious.Widget.GuiVMess",
             "Furious.Widget.UserServersQTableWidget"
         ],
         "ZH": "地址",
         "isReviewed": "True"
     },
     "Port": {
         "source": [
+            "Furious.Widget.GuiShadowsocks",
+            "Furious.Widget.GuiTrojan",
+            "Furious.Widget.GuiVLESS",
+            "Furious.Widget.GuiVMess",
             "Furious.Widget.UserServersQTableWidget"
         ],
         "ZH": "端口",
         "isReviewed": "True"
     },
     "Transport": {
         "source": [
+            "Furious.Widget.GuiVTransport",
             "Furious.Widget.UserServersQTableWidget"
         ],
         "ZH": "传输方式",
         "isReviewed": "True"
     },
     "TLS": {
         "source": [
@@ -416,22 +429,22 @@
             "Furious.Widget.UserServersQTableWidget"
         ],
         "ZH": "延迟",
         "isReviewed": "True"
     },
     "Speed": {
         "source": [
+            "Furious.Widget.GuiHysteria1",
             "Furious.Widget.UserServersQTableWidget"
         ],
         "ZH": "速度",
         "isReviewed": "True"
     },
     "Edit Configuration...": {
         "source": [
-            "Furious.Widget.UserServersQTableWidget",
             "Furious.TrayActions.EditConfiguration"
         ],
         "ZH": "编辑配置...",
         "isReviewed": "True"
     },
     "Move Up": {
         "source": [
@@ -649,14 +662,16 @@
             "Furious.Window.XrayAssetViewerWindow"
         ],
         "ZH": "所有文件 (*)",
         "isReviewed": "True"
     },
     "Server": {
         "source": [
+            "Furious.Widget.GuiHysteria1",
+            "Furious.Widget.GuiHysteria2",
             "Furious.Window.AppMainWindow"
         ],
         "ZH": "服务器",
         "isReviewed": "True"
     },
     "Log": {
         "source": [
@@ -1024,9 +1039,128 @@
     },
     "Test Tcping Latency": {
         "source": [
             "Furious.Widget.UserServersQTableWidget"
         ],
         "ZH": "测试Tcping延迟",
         "isReviewed": "True"
+    },
+    "Basic Configuration": {
+        "source": [
+            "Furious.Widget.GuiHysteria1",
+            "Furious.Widget.GuiHysteria2",
+            "Furious.Widget.GuiShadowsocks",
+            "Furious.Widget.GuiTrojan",
+            "Furious.Widget.GuiVLESS",
+            "Furious.Widget.GuiVMess"
+        ],
+        "ZH": "基本配置",
+        "isReviewed": "True"
+    },
+    "Proxy": {
+        "source": [
+            "Furious.Widget.GuiHysteria1",
+            "Furious.Widget.GuiHysteria2",
+            "Furious.Widget.GuiShadowsocks",
+            "Furious.Widget.GuiTrojan",
+            "Furious.Widget.GuiVLESS",
+            "Furious.Widget.GuiVMess"
+        ],
+        "ZH": "代理",
+        "isReviewed": "True"
+    },
+    "Project Website": {
+        "source": [
+            "Furious.Widget.GuiHysteria1",
+            "Furious.Widget.GuiHysteria2"
+        ],
+        "ZH": "项目网站",
+        "isReviewed": "True"
+    },
+    "Other": {
+        "source": [
+            "Furious.Widget.GuiHysteria1",
+            "Furious.Widget.GuiHysteria2"
+        ],
+        "ZH": "其它",
+        "isReviewed": "True"
+    },
+    "Encryption": {
+        "source": [
+            "Furious.Widget.GuiShadowsocks",
+            "Furious.Widget.GuiVLESS"
+        ],
+        "ZH": "加密",
+        "isReviewed": "True"
+    },
+    "Password": {
+        "source": [
+            "Furious.Widget.GuiShadowsocks",
+            "Furious.Widget.GuiTrojan"
+        ],
+        "ZH": "密码",
+        "isReviewed": "True"
+    },
+    "Flow": {
+        "source": [
+            "Furious.Widget.GuiVLESS"
+        ],
+        "ZH": "流控",
+        "isReviewed": "True"
+    },
+    "Use Monochrome Tray Icon": {
+        "source": [
+            "Furious.TrayActions.Settings"
+        ],
+        "ZH": "使用单色托盘图标",
+        "isReviewed": "True"
+    },
+    "Customize JSON Configuration...": {
+        "source": [
+            "Furious.Widget.UserServersQTableWidget"
+        ],
+        "ZH": "自定义JSON配置...",
+        "isReviewed": "True"
+    },
+    "Add VMess Server...": {
+        "source": [
+            "Furious.Window.AppMainWindow"
+        ],
+        "ZH": "添加VMess服务器...",
+        "isReviewed": "True"
+    },
+    "Add VLESS Server...": {
+        "source": [
+            "Furious.Window.AppMainWindow"
+        ],
+        "ZH": "添加VLESS服务器...",
+        "isReviewed": "True"
+    },
+    "Add Shadowsocks Server...": {
+        "source": [
+            "Furious.Window.AppMainWindow"
+        ],
+        "ZH": "添加Shadowsocks服务器...",
+        "isReviewed": "True"
+    },
+    "Add Trojan Server...": {
+        "source": [
+            "Furious.Window.AppMainWindow"
+        ],
+        "ZH": "添加Trojan服务器...",
+        "isReviewed": "True"
+    },
+    "Add Hysteria1 Server...": {
+        "source": [
+            "Furious.Window.AppMainWindow"
+        ],
+        "ZH": "添加Hysteria1服务器...",
+        "isReviewed": "True"
+    },
+    "Add Hysteria2 Server...": {
+        "source": [
+            "Furious.Window.AppMainWindow"
+        ],
+        "ZH": "添加Hysteria2服务器...",
+        "isReviewed": "True"
     }
 }
```

### Comparing `Furious-GUI-0.3.9/Furious/Externals/__init__.py` & `Furious-GUI-0.4.0/Furious/Externals/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Interface/Application.py` & `Furious-GUI-0.4.0/Furious/Interface/Application.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Interface/ConfigurationFactory.py` & `Furious-GUI-0.4.0/Furious/Interface/ConfigurationFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Interface/CoreFactory.py` & `Furious-GUI-0.4.0/Furious/Interface/CoreFactory.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Interface/Encoder.py` & `Furious-GUI-0.4.0/Furious/Interface/Encoder.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Interface/ItemUpdateProtocol.py` & `Furious-GUI-0.4.0/Furious/Interface/ItemUpdateProtocol.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Interface/Storage.py` & `Furious-GUI-0.4.0/Furious/Interface/Storage.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Interface/UserServersTableItem.py` & `Furious-GUI-0.4.0/Furious/Interface/UserServersTableItem.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Interface/__init__.py` & `Furious-GUI-0.4.0/Furious/Interface/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .Encoder import *
+from .GuiEditorItemFactory import *
 from .UserServersTableItem import *
 from .ItemUpdateProtocol import *
 from .Storage import *
 from .Application import *
 from .ConfigurationFactory import *
 from .CoreFactory import *
```

### Comparing `Furious-GUI-0.3.9/Furious/Library/Configuration.py` & `Furious-GUI-0.4.0/Furious/Library/Configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -377,14 +377,26 @@
 
                 pass
 
         elif network == 'grpc':
             if hasKey('serviceName'):
                 kwargs['path'] = networkObject['serviceName']
 
+        elif network == 'httpupgrade':
+            try:
+                # Get order matters here
+                if hasKey('path'):
+                    kwargs['path'] = quote(networkObject['path'])
+
+                kwargs['host'] = quote(networkObject['host'])
+            except Exception:
+                # Any non-exit exceptions
+
+                pass
+
         return kwargs
 
     @property
     def kwargsFromVLESSProxyStreamSettingsNetworkObject(self) -> dict:
         kwargs = {}
 
         network = self.proxyStreamSettingsNetwork
@@ -456,14 +468,33 @@
 
                 pass
 
         elif network == 'grpc':
             if hasKey('serviceName'):
                 kwargs['serviceName'] = networkObject['serviceName']
 
+            if hasKey('multiMode'):
+                if networkObject['multiMode']:
+                    kwargs['mode'] = 'multi'
+
+            if hasKey('authority'):
+                kwargs['authority'] = networkObject['authority']
+
+        elif network == 'httpupgrade':
+            try:
+                # Get order matters here
+                if hasKey('path'):
+                    kwargs['path'] = quote(networkObject['path'])
+
+                kwargs['host'] = quote(networkObject['host'])
+            except Exception:
+                # Any non-exit exceptions
+
+                pass
+
         return kwargs
 
     @staticmethod
     def kwargs2ProxyStreamSettingsNetworkObject(type_, remote_host, kwargs) -> dict:
         # Note:
         # v2rayN share standard doesn't require unquote. Still
         # unquote value according to (VMess AEAD / VLESS) standard
@@ -586,16 +617,30 @@
 
             if kwargs.get('serviceName'):
                 GRPCObject['serviceName'] = kwargs.get('serviceName')
 
             if kwargs.get('mode', 'gun'):
                 GRPCObject['multiMode'] = kwargs.get('mode', 'gun') == 'multi'
 
+            if kwargs.get('authority'):
+                GRPCObject['authority'] = kwargs.get('authority')
+
             return GRPCObject
 
+        elif type_ == 'httpupgrade':
+            httpUpgradeObject = {}
+
+            if kwargs.get('path', '/'):
+                httpUpgradeObject['path'] = unquote(kwargs.get('path', '/'))
+
+            if kwargs.get('host'):
+                httpUpgradeObject['host'] = unquote(kwargs.get('host'))
+
+            return httpUpgradeObject
+
     @property
     def kwargsFromProxyStreamSettingsTLSObject(self) -> dict:
         kwargs = {}
 
         TLS = self.proxyStreamSettingsTLS
         TLSObject = self.proxyStreamSettingsTLSObject
 
@@ -685,15 +730,16 @@
                 'id': uuid_,
                 'security': encryption,
                 'email': PROXY_OUTBOUND_USER_EMAIL,
             }
 
             # For VMess(v2rayN share standard) only.
             if kwargs.get('aid') is not None:
-                UserObject['alterId'] = kwargs.get('aid')
+                # int: extra guard
+                UserObject['alterId'] = int(kwargs.get('aid'))
 
             return UserObject
 
         if protocol == 'vless':
             UserObject = {
                 'id': uuid_,
                 'encryption': encryption,
@@ -795,26 +841,14 @@
             remark = unquote(result.fragment)
         except Exception:
             # Any non-exit exceptions
 
             return '', {}
 
         def getSSParams():
-            try:
-                # ss://base64...#fragment
-                userinfo, server = (
-                    PyBase64Encoder.decode(result.netloc).decode().split('@')
-                )
-
-                return [*userinfo.split(':', 1), *parseHostPort(server)]
-            except Exception:
-                # Any non-exit exceptions
-
-                pass
-
             # Begin SIP002...
             try:
                 # Try pack with 3 element
                 userinfo, server = result.netloc.split('@')
 
                 # Some old SS share link doesn't add padding
                 # in base64 encoding. Add padding to userinfo
@@ -833,14 +867,26 @@
 
                 return [*userinfo.split(':', 1), *parseHostPort(server)]
             except Exception:
                 # Any non-exit exceptions
 
                 pass
 
+            try:
+                # ss://base64...#fragment
+                userinfo, server = (
+                    PyBase64Encoder.decode(result.netloc).decode().split('@')
+                )
+
+                return [*userinfo.split(':', 1), *parseHostPort(server)]
+            except Exception:
+                # Any non-exit exceptions
+
+                pass
+
             raise ValueError(f'Invalid SS URI format {URI}')
 
         return (
             remark,
             ConfigurationXrayProxyOutboundObjectSS(*getSSParams()),
         )
 
@@ -933,22 +979,22 @@
         if self.proxyProtocol.lower() == 'vmess':
             netloc = PyBase64Encoder.encode(
                 UJSONEncoder.encode(
                     {
                         'v': '2',
                         'ps': override,
                         **{
-                            key: self.proxyServerObject[value]
+                            key: str(self.proxyServerObject[value])
                             for key, value in {
                                 'add': 'address',
                                 'port': 'port',
                             }.items()
                         },
                         **{
-                            key: self.proxyUserObject[value]
+                            key: str(self.proxyUserObject[value])
                             for key, value in {
                                 'id': 'id',
                                 'aid': 'alterId',
                                 'scy': 'security',
                             }.items()
                         },
                         'net': self.proxyStreamSettingsNetwork,
@@ -1137,19 +1183,33 @@
         except Exception:
             # Any non-exit exceptions
 
             return ''
 
     def setHttpProxyEndpoint(self, endpoint: str) -> bool:
         try:
-            listen, port = parseHostPort(endpoint)
-
             if self.get('inbounds') is None:
                 self['inbounds'] = []
 
+            if not isinstance(self['inbounds'], list):
+                self['inbounds'] = []
+
+            if endpoint == '':
+                for inbound in self['inbounds']:
+                    if inbound['protocol'] == 'http':
+                        self['inbounds'].remove(inbound)
+
+                        # Remove first chosen
+                        return True
+
+                # None satisfied. Return success
+                return True
+
+            listen, port = parseHostPort(endpoint)
+
             for inbound in self['inbounds']:
                 if inbound['protocol'] == 'http':
                     # Note: If there are multiple http inbounds
                     # satisfied, the first one will be chosen.
                     inbound['listen'], inbound['port'] = listen, int(port)
 
                     return True
@@ -1180,19 +1240,33 @@
         except Exception:
             # Any non-exit exceptions
 
             return False
 
     def setSocksProxyEndpoint(self, endpoint: str) -> bool:
         try:
-            listen, port = parseHostPort(endpoint)
-
             if self.get('inbounds') is None:
                 self['inbounds'] = []
 
+            if not isinstance(self['inbounds'], list):
+                self['inbounds'] = []
+
+            if endpoint == '':
+                for inbound in self['inbounds']:
+                    if inbound['protocol'] == 'socks':
+                        self['inbounds'].remove(inbound)
+
+                        # Remove first chosen
+                        return True
+
+                # None satisfied. Return success
+                return True
+
+            listen, port = parseHostPort(endpoint)
+
             for inbound in self['inbounds']:
                 if inbound['protocol'] == 'socks':
                     # Note: If there are multiple socks inbounds
                     # satisfied, the first one will be chosen.
                     inbound['listen'], inbound['port'] = listen, int(port)
 
                     return True
@@ -1281,18 +1355,160 @@
 
     def toJSONString(self, **kwargs) -> str:
         indent = kwargs.pop('indent', 4)
 
         return super().toJSONString(indent=indent)
 
     def toURI(self, remark: str = '') -> str:
-        return ''
+        if remark == '':
+            override = self.itemRemark
+        else:
+            override = remark
+
+        try:
+            netloc, mport = self['server'].split(',')
+        except Exception:
+            # Any non-exit exceptions
+
+            netloc, mport = self['server'], ''
+
+        if mport:
+            mportArgs = {'mport': mport}
+        else:
+            mportArgs = {}
+
+        protocol = self.get('protocol', 'udp')
+
+        if self.get('auth_str'):
+            # auth in string
+            authArgs = {'auth': self['auth_str']}
+        else:
+            authArgs = {}
+
+        if self.get('server_name'):
+            peerArgs = {'peer': self['server_name']}
+        else:
+            peerArgs = {}
+
+        if self.get('insecure') is True:
+            insecureArgs = {'insecure': '1'}
+        else:
+            insecureArgs = {}
+
+        upmbps = self['up_mbps']
+        downmbps = self['down_mbps']
+
+        if self.get('alpn'):
+            alpnArgs = {'alpn': self['alpn']}
+        else:
+            alpnArgs = {}
+
+        if self.get('obfs'):
+            obfsParamArgs = {'obfsParam': self['obfs']}
+        else:
+            obfsParamArgs = {}
+
+        query = '&'.join(
+            f'{key}={value}'
+            for key, value in {
+                **mportArgs,
+                'protocol': protocol,
+                **authArgs,
+                **peerArgs,
+                **insecureArgs,
+                'upmbps': upmbps,
+                'downmbps': downmbps,
+                **alpnArgs,
+                **obfsParamArgs,
+            }.items()
+        )
+
+        return urlunparse(['hysteria', netloc, '', '', query, quote(override)])
 
     def fromURI(self, URI: str) -> bool:
-        return False
+        try:
+            result = urlparse(URI)
+            remark = unquote(result.fragment)
+            queryObject = {key: value for key, value in parse_qsl(result.query)}
+
+            if result.scheme != 'hysteria':
+                raise ValueError('Invalid hysteria1 URI scheme')
+
+            server = result.netloc
+
+            mport = queryObject.get('mport', '')
+
+            if mport:
+                server += f',{mport}'
+
+            protocol = queryObject.get('protocol', 'udp')
+
+            if queryObject.get('auth', ''):
+                # auth in string
+                authArgs = {'auth_str': queryObject['auth']}
+            else:
+                authArgs = {}
+
+            if queryObject.get('peer', ''):
+                peerArgs = {'server_name': queryObject['peer']}
+            else:
+                peerArgs = {}
+
+            insecure = queryObject.get('insecure', False)
+
+            if isinstance(insecure, bool):
+                pass
+            elif insecure == '1':
+                insecure = True
+            else:
+                insecure = False
+
+            upmbps = queryObject.get('upmbps', 24)
+            downmbps = queryObject.get('downmbps', 96)
+
+            if queryObject.get('alpn', ''):
+                alpnArgs = {'alpn': queryObject['alpn']}
+            else:
+                alpnArgs = {}
+
+            # obfs mode seems not required, ignored...
+
+            if queryObject.get('obfsParam', ''):
+                obfsParamArgs = {'obfs': queryObject['obfsParam']}
+            else:
+                obfsParamArgs = {}
+
+            dict.__init__(
+                self,
+                **{
+                    'server': server,
+                    'protocol': protocol,
+                    **authArgs,
+                    **obfsParamArgs,
+                    'up_mbps': int(upmbps),
+                    'down_mbps': int(downmbps),
+                    **peerArgs,
+                    **alpnArgs,
+                    'insecure': insecure,
+                    'socks5': {
+                        'listen': '127.0.0.1:10808',
+                    },
+                    'http': {
+                        'listen': '127.0.0.1:10809',
+                    },
+                },
+            )
+
+            self.setExtras('remark', remark)
+
+            return True
+        except Exception:
+            # Any non-exit exceptions
+
+            return False
 
     def httpProxyEndpoint(self) -> str:
         try:
             return self['http']['listen']
         except Exception:
             # Any non-exit exceptions
 
@@ -1304,27 +1520,37 @@
         except Exception:
             # Any non-exit exceptions
 
             return ''
 
     def setHttpProxyEndpoint(self, endpoint: str) -> bool:
         try:
+            if endpoint == '':
+                self.pop('http', None)
+
+                return True
+
             if self.get('http') is None:
                 self['http'] = {}
 
             self['http']['listen'] = endpoint
 
             return True
         except Exception:
             # Any non-exit exceptions
 
             return False
 
     def setSocksProxyEndpoint(self, endpoint: str) -> bool:
         try:
+            if endpoint == '':
+                self.pop('socks5', None)
+
+                return True
+
             if self.get('socks5') is None:
                 self['socks5'] = {}
 
             self['socks5']['listen'] = endpoint
 
             return True
         except Exception:
@@ -1470,20 +1696,20 @@
                 pinSHA256Arg['pinSHA256'] = pinSHA256
 
             dict.__init__(
                 self,
                 **{
                     'server': server,
                     'auth': auth,
+                    **obfsArg,
                     'tls': {
                         'sni': sni,
                         'insecure': insecure,
                         **pinSHA256Arg,
                     },
-                    **obfsArg,
                     'socks5': {
                         'listen': '127.0.0.1:10808',
                     },
                     'http': {
                         'listen': '127.0.0.1:10809',
                     },
                 },
@@ -1511,27 +1737,37 @@
         except Exception:
             # Any non-exit exceptions
 
             return ''
 
     def setHttpProxyEndpoint(self, endpoint: str) -> bool:
         try:
+            if endpoint == '':
+                self.pop('http', None)
+
+                return True
+
             if self.get('http') is None:
                 self['http'] = {}
 
             self['http']['listen'] = endpoint
 
             return True
         except Exception:
             # Any non-exit exceptions
 
             return False
 
     def setSocksProxyEndpoint(self, endpoint: str) -> bool:
         try:
+            if endpoint == '':
+                self.pop('socks5', None)
+
+                return True
+
             if self.get('socks5') is None:
                 self['socks5'] = {}
 
             self['socks5']['listen'] = endpoint
 
             return True
         except Exception:
@@ -1591,14 +1827,16 @@
         if (
             config.startswith('vmess://')
             or config.startswith('vless://')
             or config.startswith('ss://')
             or config.startswith('trojan://')
         ):
             return ConfigurationXray(config, **kwargs)
+        if config.startswith('hysteria://'):
+            return ConfigurationHysteria1(config, **kwargs)
         if config.startswith('hy2://') or config.startswith('hysteria2://'):
             return ConfigurationHysteria2(config, **kwargs)
 
         try:
             # Try to construct from JSON string
             return constructFromDict(UJSONEncoder.decode(config), **kwargs)
         except Exception:
```

### Comparing `Furious-GUI-0.3.9/Furious/Library/Encoder.py` & `Furious-GUI-0.4.0/Furious/Library/Encoder.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Library/Tcping.py` & `Furious-GUI-0.4.0/Furious/Library/Tcping.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Library/__init__.py` & `Furious-GUI-0.4.0/Furious/Library/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .Configuration import *
+from .EmptyFactoryHelper import *
 from .Encoder import *
 from .Tcping import *
```

### Comparing `Furious-GUI-0.3.9/Furious/PyFramework/Ancestors.py` & `Furious-GUI-0.4.0/Furious/PyFramework/Ancestors.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/PyFramework/__init__.py` & `Furious-GUI-0.4.0/Furious/PyFramework/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/Ancestors.py` & `Furious-GUI-0.4.0/Furious/QtFramework/Ancestors.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/CoreProcess.py` & `Furious-GUI-0.4.0/Furious/QtFramework/CoreProcess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/DNSResolver.py` & `Furious-GUI-0.4.0/Furious/QtFramework/DNSResolver.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/DynamicTheme.py` & `Furious-GUI-0.4.0/Furious/QtFramework/DynamicTheme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/DynamicTranslate.py` & `Furious-GUI-0.4.0/Furious/QtFramework/DynamicTranslate.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/NetworkStateManager.py` & `Furious-GUI-0.4.0/Furious/QtFramework/NetworkStateManager.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/QtGui.py` & `Furious-GUI-0.4.0/Furious/QtFramework/QtGui.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,23 @@
         menu=None,
         useActionGroup=True,
         checkable=False,
         checked=False,
         statusTip=None,
         callback=None,
         shortcut=None,
+        isTrayAction=False,
         **kwargs,
     ):
         super().__init__(text=text, **kwargs)
 
         # Do not use QProtection because it's been managed somewhere else!!!
         self.useQProtection = False
         self.iconFileName = ''
+        self.isTrayAction = isTrayAction
 
         self.setShortcutVisibleInContextMenu(True)
 
         if icon is not None:
             self.setIcon(icon)
 
         if menu is not None:
@@ -171,16 +173,16 @@
             return
 
         if theme == 'Dark':
             if PLATFORM == 'Windows':
                 # Windows. Always use black icon
                 super().setIcon(bootstrapIcon(self.iconFileName))
             else:
-                if getUbuntuRelease() == '20.04':
-                    # Ubuntu 20.04 system dark theme does not change menu color.
+                if getUbuntuRelease() == '20.04' and self.isTrayAction:
+                    # Ubuntu 20.04 system dark theme does not change tray menu color.
                     # Make it go black always
                     super().setIcon(bootstrapIcon(self.iconFileName))
                 else:
                     super().setIcon(bootstrapIconWhite(self.iconFileName))
         else:
             super().setIcon(bootstrapIcon(self.iconFileName))
```

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/QtNetwork.py` & `Furious-GUI-0.4.0/Furious/QtFramework/QtNetwork.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/QtWidgets.py` & `Furious-GUI-0.4.0/Furious/QtFramework/QtWidgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 
 import functools
 
 __all__ = [
     'moveToCenter',
+    'AppQCheckBox',
     'AppQDialog',
+    'AppQDialogButtonBox',
     'AppQGroupBox',
     'AppQHeaderView',
     'AppQLabel',
     'AppQListWidget',
     'AppQMainWindow',
     'AppQMenu',
     'AppQMenuBar',
     'AppQMessageBox',
     'AppQPushButton',
-    'AppQStyledItemDelegate',
     'AppQTableWidget',
     'AppQTabWidget',
     'AppQToolBar',
     'QuestionDeleteMBox',
     'NewChangesNextTimeMBox',
 ]
 
@@ -63,14 +64,22 @@
         center = parent.geometry().center()
 
     geometry.moveCenter(center)
 
     widget.move(geometry.topLeft())
 
 
+class AppQCheckBox(QTranslatable, QCheckBox):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def retranslate(self):
+        self.setText(_(self.text()))
+
+
 class AppQDialog(QTranslatable, SupportConnectedCallback, QDialog):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self._firstShowCall = True
 
         if PLATFORM != 'Darwin':
@@ -101,23 +110,32 @@
                 self.setWidthAndHeight()
 
                 self._firstShowCall = False
 
         moveToCenter(self)
 
     def retranslate(self):
-        pass
+        self.setWindowTitle(_(self.windowTitle()))
 
     def disconnectedCallback(self):
         self.setWindowIcon(AppHue.disconnectedWindowIcon())
 
     def connectedCallback(self):
         self.setWindowIcon(AppHue.connectedWindowIcon())
 
 
+class AppQDialogButtonBox(QTranslatable, QDialogButtonBox):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def retranslate(self):
+        for button in self.buttons():
+            button.setText(_(button.text()))
+
+
 class AppQGroupBox(QTranslatable, QGroupBox):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def retranslate(self):
         self.setTitle(_(self.title()))
 
@@ -270,14 +288,16 @@
 
         if PLATFORM == 'Darwin':
             if self._firstShowCall:
                 APP().processEvents()
 
                 self.setWidthAndHeight()
 
+                APP().processEvents()
+
                 self._firstShowCall = False
 
         moveToCenter(self)
 
     def closeEvent(self, event):
         event.ignore()
 
@@ -421,25 +441,14 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def retranslate(self):
         self.setText(_(self.text()))
 
 
-class AppQStyledItemDelegate(QStyledItemDelegate):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def createEditor(self, parent, option, index):
-        editor = QLineEdit(parent)
-        editor.setFont(QFont(APP().customFontName))
-
-        return editor
-
-
 class AppQTableWidget(SupportConnectedCallback, QTableWidget):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.setWordWrap(False)
 
     @property
```

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/TextEditor.py` & `Furious-GUI-0.4.0/Furious/QtFramework/TextEditor.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/TextEditorTheme.py` & `Furious-GUI-0.4.0/Furious/QtFramework/TextEditorTheme.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/UpdatesManager.py` & `Furious-GUI-0.4.0/Furious/QtFramework/UpdatesManager.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,57 +94,64 @@
         f'https://api.github.com/repos/'
         f'{APPLICATION_REPO_OWNER_NAME}/{APPLICATION_REPO_NAME}/releases/latest'
     )
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
-    @staticmethod
-    def handleFinishedByNetworkReply(networkReply):
+    def handleFinishedByNetworkReply(self, networkReply):
         assert isinstance(networkReply, QNetworkReply)
 
         if networkReply.error() != QNetworkReply.NetworkError.NoError:
             logger.error(f'check for updates failed. {networkReply.errorString()}')
 
             mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Critical)
             mbox.setWindowTitle(_(APPLICATION_NAME))
             mbox.setText(_('Check for updates failed'))
 
-            # Show the MessageBox and wait for user to close it
-            mbox.exec()
+            # Show the MessageBox asynchronously
+            mbox.open()
         else:
             logger.info('check for updates success')
 
             # Unchecked?
             info = UJSONEncoder.decode(networkReply.readAll().data())
 
             if versionToNumber(info['tag_name']) > versionToNumber(APPLICATION_VERSION):
+
+                def handleResultCode(code):
+                    if code == PySide6LegacyEnumValueWrapper(
+                        AppQMessageBox.StandardButton.Yes
+                    ):
+                        if QDesktopServices.openUrl(QtCore.QUrl(info['html_url'])):
+                            logger.info('open download page success')
+                        else:
+                            logger.error('open download page failed')
+                    else:
+                        # Do nothing
+                        pass
+
                 mbox = QuestionUpdateMBox(icon=AppQMessageBox.Icon.Information)
                 mbox.version = info['tag_name']
                 mbox.setText(mbox.customText())
                 mbox.setInformativeText(_('Go to download page?'))
+                mbox.finished.connect(functools.partial(handleResultCode))
 
-                # Show the MessageBox and wait for user to close it
-                if mbox.exec() == PySide6LegacyEnumValueWrapper(
-                    AppQMessageBox.StandardButton.Yes
-                ):
-                    if QDesktopServices.openUrl(QtCore.QUrl(info['html_url'])):
-                        logger.info('open download page success')
-                    else:
-                        logger.error('open download page failed')
-                else:
-                    # Do nothing
-                    pass
+                # dummy ref
+                setattr(self, '_questionUpdateMBox', mbox)
+
+                # Show the MessageBox asynchronously
+                mbox.open()
             else:
                 mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Information)
                 mbox.setWindowTitle(_(APPLICATION_NAME))
                 mbox.setText(_(f'{APPLICATION_NAME} is already the latest version'))
 
-                # Show the MessageBox and wait for user to close it
-                mbox.exec()
+                # Show the MessageBox asynchronously
+                mbox.open()
 
     def configureHttpProxy(self, httpProxy: Union[str, None]) -> bool:
         useProxy = super().configureHttpProxy(httpProxy)
 
         if useProxy:
             logger.info(f'check for updates uses proxy server {httpProxy}')
         else:
```

### Comparing `Furious-GUI-0.3.9/Furious/QtFramework/__init__.py` & `Furious-GUI-0.4.0/Furious/QtFramework/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,7 +23,8 @@
 from .QtGui import *
 from .QtWidgets import *
 from .QtNetwork import *
 from .UpdatesManager import *
 from .NetworkStateManager import *
 from .TextEditor import *
 from .TextEditorTheme import *
+from .GuiEditorXXX import *
```

### Comparing `Furious-GUI-0.3.9/Furious/Storage/UserServers.py` & `Furious-GUI-0.4.0/Furious/Storage/UserServers.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Storage/UserSubs.py` & `Furious-GUI-0.4.0/Furious/Storage/UserSubs.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Storage/__init__.py` & `Furious-GUI-0.4.0/Furious/Storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/Connect.py` & `Furious-GUI-0.4.0/Furious/TrayActions/Connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,19 +71,20 @@
 
         return False
     else:
         return True
 
 
 class ConnectAction(AppQAction):
-    def __init__(self):
+    def __init__(self, **kwargs):
         super().__init__(
             _('Connect'),
             icon=bootstrapIcon('unlock-fill.svg'),
             checkable=True,
+            **kwargs,
         )
 
         self.actionQueue = queue.Queue()
         self.coreManager = CoreManager()
         self.progressBar = ConnectProgressBar()
 
         self.actionTimer = QtCore.QTimer()
@@ -189,32 +190,32 @@
 
             mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Critical)
             mbox.setWindowTitle(_('Unable to connect'))
             mbox.setText(
                 _('Server configuration empty. Please configure your server first')
             )
 
-            # Show the MessageBox and wait for user to close it
-            mbox.exec()
+            # Show the MessageBox asynchronously
+            mbox.open()
 
             return
 
         if AS_UserActivatedItemIndex() < 0:
             AppSettings.turnOFF('Connect')
 
             self.setChecked(False)
 
             mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Critical)
             mbox.setWindowTitle(_('Unable to connect'))
             mbox.setText(
                 _('Select and double click to activate configuration and connect')
             )
 
-            # Show the MessageBox and wait for user to close it
-            mbox.exec()
+            # Show the MessageBox asynchronously
+            mbox.open()
 
             return
 
         try:
             config = AS_UserServers()[AS_UserActivatedItemIndex()]
         except Exception:
             # Any non-exit exceptions
@@ -238,16 +239,16 @@
                 _(
                     f'{APPLICATION_NAME} cannot find any valid http proxy '
                     f'endpoint in the configuration'
                 )
             )
             mbox.setInformativeText(_('Please complete your server configuration'))
 
-            # Show the MessageBox and wait for user to close it
-            mbox.exec()
+            # Show the MessageBox asynchronously
+            mbox.open()
 
             return
 
         self.doConnecting()
 
         # Clear previous log
         APP().logViewerWindowCore.clear()
```

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/EditConfiguration.py` & `Furious-GUI-0.4.0/Furious/TrayActions/EditConfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 needTrans = functools.partial(needTransFn, source=__name__)
 
 needTrans('Edit Configuration...')
 
 
 class EditConfigurationAction(AppQAction):
-    def __init__(self):
+    def __init__(self, **kwargs):
         super().__init__(
             _('Edit Configuration...'),
             icon=bootstrapIcon('pencil-square.svg'),
+            **kwargs,
         )
 
     def triggeredCallback(self, checked):
         APP().mainWindow.show()
```

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/Exit.py` & `Furious-GUI-0.4.0/Furious/TrayActions/Exit.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 needTrans = functools.partial(needTransFn, source=__name__)
 
 needTrans('Exit')
 
 
 class ExitAction(AppQAction):
-    def __init__(self):
+    def __init__(self, **kwargs):
         super().__init__(
             _('Exit'),
             icon=bootstrapIcon('box-arrow-in-left.svg'),
+            **kwargs,
         )
 
     def triggeredCallback(self, checked):
         APP().exit()
```

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/Import.py` & `Furious-GUI-0.4.0/Furious/TrayActions/Import.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,29 +51,32 @@
         # Limited
         mbox.setText(_('Invalid data'))
         mbox.setInformativeText('')
     else:
         mbox.setText(_('Invalid data. The content of the clipboard is:'))
         mbox.setInformativeText(clipboard)
 
-    mbox.exec()
+    # Show the MessageBox asynchronously
+    mbox.open()
 
 
 def importItemFromClipboard(clipboard: str):
     factory = constructFromAny(clipboard)
 
     if not factory.isValid():
         showImportErrorMBox(clipboard)
     else:
         APP().mainWindow.appendNewItemByFactory(factory)
 
         mbox = ImportSuccessMBox(icon=AppQMessageBox.Icon.Information)
         mbox.remark = factory.getExtras('remark')
         mbox.setText(mbox.customText())
-        mbox.exec()
+
+        # Show the MessageBox asynchronously
+        mbox.open()
 
 
 needTrans('Import')
 
 
 class ImportErrorMBox(AppQMessageBox):
     def __init__(self, *args, **kwargs):
@@ -189,31 +192,35 @@
                 # Any non-exit exceptions
 
                 mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Critical)
                 mbox.setWindowTitle(_('Error opening file'))
                 mbox.setText(_('Invalid configuration file'))
                 mbox.setInformativeText(str(ex))
 
-                # Show the MessageBox and wait for user to close it
-                mbox.exec()
+                # Show the MessageBox asynchronously
+                mbox.open()
             else:
                 factory = constructFromAny(plainText, remark=os.path.basename(filename))
 
                 if factory.isValid():
                     APP().mainWindow.appendNewItemByFactory(factory)
 
                     mbox = ImportSuccessMBox(icon=AppQMessageBox.Icon.Information)
                     mbox.remark = factory.getExtras('remark')
                     mbox.setText(mbox.customText())
-                    mbox.exec()
+
+                    # Show the MessageBox asynchronously
+                    mbox.open()
                 else:
                     mbox = ImportErrorMBox(icon=AppQMessageBox.Icon.Critical)
                     mbox.setText(_('Invalid data'))
                     mbox.setInformativeText('')
-                    mbox.show()
+
+                    # Show the MessageBox asynchronously
+                    mbox.open()
 
 
 needTrans('Import Share Link From Clipboard')
 
 
 class ImportURIFromClipboardAction(AppQAction):
     def __init__(self, **kwargs):
@@ -244,21 +251,25 @@
                 showImportErrorMBox(clipboard)
             else:
                 if len(imported) == 1:
                     # Fall back to single
                     mbox = ImportSuccessMBox(icon=AppQMessageBox.Icon.Information)
                     mbox.remark = imported[0]
                     mbox.setText(mbox.customText())
-                    mbox.exec()
+
+                    # Show the MessageBox asynchronously
+                    mbox.open()
                 else:
                     mbox = ImportMultiSuccessMBox(icon=AppQMessageBox.Icon.Information)
                     mbox.imported = imported
                     mbox.rowCount = rowCount
                     mbox.setText(mbox.customText())
-                    mbox.exec()
+
+                    # Show the MessageBox asynchronously
+                    mbox.open()
 
 
 needTrans('Import JSON Configuration From Clipboard')
 
 
 class ImportJSONFromClipboardAction(AppQAction):
     def __init__(self, **kwargs):
@@ -270,18 +281,19 @@
         importItemFromClipboard(clipboard)
 
 
 needTrans('Import')
 
 
 class ImportAction(AppQAction):
-    def __init__(self):
+    def __init__(self, **kwargs):
         super().__init__(
             _('Import'),
             icon=bootstrapIcon('lightning-charge.svg'),
             menu=AppQMenu(
                 ImportURIFromClipboardAction(),
                 ImportJSONFromClipboardAction(),
             ),
             useActionGroup=False,
             checkable=True,
+            **kwargs,
         )
```

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/Language.py` & `Furious-GUI-0.4.0/Furious/TrayActions/Language.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,23 +57,24 @@
         pass
 
 
 needTrans('Language')
 
 
 class LanguageAction(AppQAction):
-    def __init__(self):
+    def __init__(self, **kwargs):
         super().__init__(
             _('Language'),
             icon=bootstrapIcon('globe2.svg'),
             menu=AppQMenu(
                 *list(
                     LanguageChildAction(
                         # Language representation
                         text,
                         checkable=True,
                         checked=text == ABBR_TO_LANGUAGE[AppSettings.get('Language')],
                     )
                     for text in list(LANGUAGE_TO_ABBR.keys())
                 ),
             ),
+            **kwargs,
         )
```

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/Routing.py` & `Furious-GUI-0.4.0/Furious/TrayActions/Routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 APP().systemTray.ConnectAction.trigger()
 
 
 needTrans('Routing')
 
 
 class RoutingAction(AppQAction):
-    def __init__(self):
+    def __init__(self, **kwargs):
         if AppSettings.get('Routing') == 'Bypass':
             # Update value for backward compatibility
             AppSettings.set('Routing', 'Bypass Mainland China')
 
         super().__init__(
             _('Routing'),
             icon=bootstrapIcon('shuffle.svg'),
@@ -65,8 +65,9 @@
                         _(routing),
                         checkable=True,
                         checked=AppSettings.get('Routing') == routing,
                     )
                     for routing in BUILTIN_ROUTING
                 ),
             ),
+            **kwargs,
         )
```

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/Settings.py` & `Furious-GUI-0.4.0/Furious/TrayActions/Settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 registerAppSettings('VPNMode', isBinary=True)
 registerAppSettings('DarkMode', isBinary=True)
 registerAppSettings('StartupOnBoot', isBinary=True, default=BinarySettings.ON_)
 registerAppSettings(
     'ShowProgressBarWhenConnecting', isBinary=True, default=BinarySettings.ON_
 )
 registerAppSettings('ShowTabAndSpacesInEditor', isBinary=True)
+registerAppSettings('UseMonochromeTrayIcon', isBinary=True)
 
 needTrans = functools.partial(needTransFn, source=__name__)
 
 needTrans(
     'VPN Mode',
     'VPN Mode Disabled (Administrator)',
     'VPN Mode Disabled (root)',
@@ -58,15 +59,17 @@
             AppSettings.turnON_('VPNMode')
         else:
             AppSettings.turnOFF('VPNMode')
 
         try:
             if APP().isSystemTrayConnected():
                 mbox = NewChangesNextTimeMBox()
-                mbox.exec()
+
+                # Show the MessageBox asynchronously
+                mbox.open()
         except Exception:
             # Any non-exit exceptions
 
             pass
 
 
 class SettingsChildAction(AppQAction):
@@ -113,27 +116,41 @@
                 APP().mainWindow.showTabAndSpaces()
 
                 AppSettings.turnON_('ShowTabAndSpacesInEditor')
             else:
                 APP().mainWindow.hideTabAndSpaces()
 
                 AppSettings.turnOFF('ShowTabAndSpacesInEditor')
+        if self.textCompare('Use Monochrome Tray Icon'):
+            # Settings turn on/off order matters here
+            if checked:
+                AppSettings.turnON_('UseMonochromeTrayIcon')
+
+                APP().systemTray.setMonochromeIcon()
+            else:
+                AppSettings.turnOFF('UseMonochromeTrayIcon')
+
+                if APP().isSystemTrayConnected():
+                    APP().systemTray.setConnectedIcon()
+                else:
+                    APP().systemTray.setDisconnectedIcon()
 
 
 needTrans(
     'Settings',
     'Dark Mode',
     'Startup On Boot',
     'Show Progress Bar When Connecting',
     'Show Tab And Spaces In Editor',
+    'Use Monochrome Tray Icon',
 )
 
 
 class SettingsAction(AppQAction):
-    def __init__(self):
+    def __init__(self, **kwargs):
         if PLATFORM == 'Windows' or PLATFORM == 'Darwin':
             extraActions = [
                 VPNModeAction(
                     checkable=True,
                     checked=AppSettings.isStateON_('VPNMode'),
                 ),
                 AppQSeperator(),
@@ -148,14 +165,19 @@
                 *extraActions,
                 SettingsChildAction(
                     _('Dark Mode'),
                     checkable=True,
                     checked=AppSettings.isStateON_('DarkMode'),
                 ),
                 SettingsChildAction(
+                    _('Use Monochrome Tray Icon'),
+                    checkable=True,
+                    checked=AppSettings.isStateON_('UseMonochromeTrayIcon'),
+                ),
+                SettingsChildAction(
                     _('Startup On Boot'),
                     checkable=True,
                     checked=AppSettings.isStateON_('StartupOnBoot'),
                 ),
                 SettingsChildAction(
                     _('Show Progress Bar When Connecting'),
                     checkable=True,
@@ -164,14 +186,15 @@
                 SettingsChildAction(
                     _('Show Tab And Spaces In Editor'),
                     checkable=True,
                     checked=AppSettings.isStateON_('ShowTabAndSpacesInEditor'),
                 ),
             ),
             useActionGroup=False,
+            **kwargs,
         )
 
     def getVPNModeAction(self) -> Union[AppQAction, None]:
         if PLATFORM == 'Windows' or PLATFORM == 'Darwin':
             # 1st action
             return self._menu.actions()[0]
         else:
```

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/SystemProxy.py` & `Furious-GUI-0.4.0/Furious/TrayActions/SystemProxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     'System Proxy',
     'Automatically Configure System Proxy',
     'Do Not Change System Proxy',
 )
 
 
 class SystemProxyAction(AppQAction):
-    def __init__(self):
+    def __init__(self, **kwargs):
         super().__init__(
             _('System Proxy'),
             icon=bootstrapIcon('hdd-network.svg'),
             menu=AppQMenu(
                 SystemProxyChildAction(
                     _('Automatically Configure System Proxy'),
                     checkable=True,
@@ -61,8 +61,9 @@
                 ),
                 SystemProxyChildAction(
                     _('Do Not Change System Proxy'),
                     checkable=True,
                     checked=AppSettings.get('SystemProxyMode') == 'NoChanges',
                 ),
             ),
+            **kwargs,
         )
```

### Comparing `Furious-GUI-0.3.9/Furious/TrayActions/__init__.py` & `Furious-GUI-0.4.0/Furious/TrayActions/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/AppMainProcess.py` & `Furious-GUI-0.4.0/Furious/Utility/AppMainProcess.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/AppResources.py` & `Furious-GUI-0.4.0/Furious/Utility/AppResources.py`

 * *Files 5% similar despite different names*

```diff
@@ -585,14 +585,92 @@
 242L2 14.732l-.2\
 87-.445L1.268 14\
 l-.026-.529L1 13\
 l.242-.471.026-.\
 529.445-.287.287\
 -.445.529-.026z\x22\
 />\x0a</svg>\
+\x00\x00\x04\xbb\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 width=\x2216\
+\x22 height=\x2216\x22 fi\
+ll=\x22currentColor\
+\x22 class=\x22bi bi-d\
+atabase\x22 viewBox\
+=\x220 0 16 16\x22>\x0a  \
+<path d=\x22M4.318 \
+2.687C5.234 2.27\
+1 6.536 2 8 2s2.\
+766.27 3.682.687\
+C12.644 3.125 13\
+ 3.627 13 4c0 .3\
+74-.356.875-1.31\
+8 1.313C10.766 5\
+.729 9.464 6 8 6\
+s-2.766-.27-3.68\
+2-.687C3.356 4.8\
+75 3 4.373 3 4c0\
+-.374.356-.875 1\
+.318-1.313M13 5.\
+698V7c0 .374-.35\
+6.875-1.318 1.31\
+3C10.766 8.729 9\
+.464 9 8 9s-2.76\
+6-.27-3.682-.687\
+C3.356 7.875 3 7\
+.373 3 7V5.698c.\
+271.202.58.378.9\
+04.525C4.978 6.7\
+11 6.427 7 8 7s3\
+.022-.289 4.096-\
+.777A5 5 0 0 0 1\
+3 5.698M14 4c0-1\
+.007-.875-1.755-\
+1.904-2.223C11.0\
+22 1.289 9.573 1\
+ 8 1s-3.022.289-\
+4.096.777C2.875 \
+2.245 2 2.993 2 \
+4v9c0 1.007.875 \
+1.755 1.904 2.22\
+3C4.978 15.71 6.\
+427 16 8 16s3.02\
+2-.289 4.096-.77\
+7C13.125 14.755 \
+14 14.007 14 13z\
+m-1 4.698V10c0 .\
+374-.356.875-1.3\
+18 1.313C10.766 \
+11.729 9.464 12 \
+8 12s-2.766-.27-\
+3.682-.687C3.356\
+ 10.875 3 10.373\
+ 3 10V8.698c.271\
+.202.58.378.904.\
+525C4.978 9.71 6\
+.427 10 8 10s3.0\
+22-.289 4.096-.7\
+77A5 5 0 0 0 13 \
+8.698m0 3V13c0 .\
+374-.356.875-1.3\
+18 1.313C10.766 \
+14.729 9.464 15 \
+8 15s-2.766-.27-\
+3.682-.687C3.356\
+ 13.875 3 13.373\
+ 3 13v-1.302c.27\
+1.202.58.378.904\
+.525C4.978 12.71\
+ 6.427 13 8 13s3\
+.022-.289 4.096-\
+.777c.324-.147.6\
+33-.323.904-.525\
+\x22/>\x0a</svg>\
 \x00\x00\x03\xfc\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 width=\x2216\
 \x22 height=\x2216\x22 fi\
 ll=\x22currentColor\
@@ -964,14 +1042,56 @@
 1 3.5 3.5zm2.5 1\
 0a1.5 1.5 0 1 0-\
 3 0 1.5 1.5 0 0 \
 0 3 0zm7 0a1.5 1\
 .5 0 1 0-3 0 1.5\
  1.5 0 0 0 3 0z\x22\
 />\x0d\x0a</svg>\
+\x00\x00\x02z\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 width=\x2216\
+\x22 height=\x2216\x22 fi\
+ll=\x22currentColor\
+\x22 class=\x22bi bi-s\
+erver\x22 viewBox=\x22\
+0 0 16 16\x22>\x0a  <p\
+ath d=\x22M1.333 2.\
+667C1.333 1.194 \
+4.318 0 8 0s6.66\
+7 1.194 6.667 2.\
+667V4c0 1.473-2.\
+985 2.667-6.667 \
+2.667S1.333 5.47\
+3 1.333 4z\x22/>\x0a  \
+<path d=\x22M1.333 \
+6.334v3C1.333 10\
+.805 4.318 12 8 \
+12s6.667-1.194 6\
+.667-2.667V6.334\
+a6.5 6.5 0 0 1-1\
+.458.79C11.81 7.\
+684 9.967 8 8 8s\
+-3.809-.317-5.20\
+8-.876a6.5 6.5 0\
+ 0 1-1.458-.79z\x22\
+/>\x0a  <path d=\x22M1\
+4.667 11.668a6.5\
+ 6.5 0 0 1-1.458\
+.789c-1.4.56-3.2\
+42.876-5.21.876-\
+1.966 0-3.809-.3\
+16-5.208-.876a6.\
+5 6.5 0 0 1-1.45\
+8-.79v1.666C1.33\
+3 14.806 4.318 1\
+6 8 16s6.667-1.1\
+94 6.667-2.667z\x22\
+/>\x0a</svg>\
 \x00\x00\x02w\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 width=\x2216\
 \x22 height=\x2216\x22 fi\
 ll=\x22currentColor\
@@ -1006,14 +1126,117 @@
 A1.5 1.5 0 0 0 3\
 .266 14h9.468a1.\
 5 1.5 0 0 0 1.48\
 9-1.314l.64-5.12\
 4A.5.5 0 0 0 14.\
 367 7H1.633z\x22/>\x0a\
 </svg>\
+\x00\x00\x06M\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 width=\x2216\
+\x22 height=\x2216\x22 fi\
+ll=\x22currentColor\
+\x22 class=\x22bi bi-r\
+ocket-takeoff\x22 v\
+iewBox=\x220 0 16 1\
+6\x22>\x0a  <path d=\x22M\
+9.752 6.193c.599\
+.6 1.73.437 2.52\
+8-.362s.96-1.932\
+.362-2.531c-.599\
+-.6-1.73-.438-2.\
+528.361-.798.8-.\
+96 1.933-.362 2.\
+532\x22/>\x0a  <path d\
+=\x22M15.811 3.312c\
+-.363 1.534-1.33\
+4 3.626-3.64 6.2\
+18l-.24 2.408a2.\
+56 2.56 0 0 1-.7\
+32 1.526L8.817 1\
+5.85a.51.51 0 0 \
+1-.867-.434l.27-\
+1.899c.04-.28-.0\
+13-.593-.131-.95\
+6a9 9 0 0 0-.249\
+-.657l-.082-.202\
+c-.815-.197-1.57\
+8-.662-2.191-1.2\
+77-.614-.615-1.0\
+79-1.379-1.275-2\
+.195l-.203-.083a\
+10 10 0 0 0-.655\
+-.248c-.363-.119\
+-.675-.172-.955-\
+.132l-1.896.27A.\
+51.51 0 0 1 .15 \
+7.17l2.382-2.386\
+c.41-.41.947-.67\
+ 1.524-.734h.006\
+l2.4-.238C9.005 \
+1.55 11.087.582 \
+12.623.208c.89-.\
+217 1.59-.232 2.\
+08-.188.244.023.\
+435.06.57.093q.1\
+.026.16.045c.184\
+.06.279.13.351.2\
+95l.029.073a3.5 \
+3.5 0 0 1 .157.7\
+21c.055.485.051 \
+1.178-.159 2.065\
+m-4.828 7.475.04\
+-.04-.107 1.081a\
+1.54 1.54 0 0 1-\
+.44.913l-1.298 1\
+.3.054-.38c.072-\
+.506-.034-.993-.\
+172-1.418a9 9 0 \
+0 0-.164-.45c.73\
+8-.065 1.462-.38\
+ 2.087-1.006M5.2\
+05 5c-.625.626-.\
+94 1.351-1.004 2\
+.09a9 9 0 0 0-.4\
+5-.164c-.424-.13\
+8-.91-.244-1.416\
+-.172l-.38.054 1\
+.3-1.3c.245-.246\
+.566-.401.91-.44\
+l1.08-.107zm9.40\
+6-3.961c-.38-.03\
+4-.967-.027-1.74\
+6.163-1.558.38-3\
+.917 1.496-6.937\
+ 4.521-.62.62-.7\
+99 1.34-.687 2.0\
+51.107.676.483 1\
+.362 1.048 1.928\
+.564.565 1.25.94\
+1 1.924 1.049.71\
+.112 1.429-.067 \
+2.048-.688 3.079\
+-3.083 4.192-5.4\
+44 4.556-6.987.1\
+83-.771.18-1.345\
+.138-1.713a3 3 0\
+ 0 0-.045-.283 3\
+ 3 0 0 0-.3-.041\
+Z\x22/>\x0a  <path d=\x22\
+M7.009 12.139a7.\
+6 7.6 0 0 1-1.80\
+4-1.352A7.6 7.6 \
+0 0 1 3.794 8.86\
+c-1.102.992-1.96\
+5 5.054-1.839 5.\
+18.125.126 3.936\
+-.896 5.054-1.90\
+2Z\x22/>\x0a</svg>\
 \x00\x00\x07\xf4\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 width=\x2216\
 \x22 height=\x2216\x22 fi\
 ll=\x22currentColor\
@@ -1029,15 +1252,15 @@
 op offset=\x220%\x22 s\
 tyle=\x22stop-color\
 :rgb(255,0,0);st\
 op-opacity:1\x22 />\
 \x0d\x0a      <stop of\
 fset=\x22100%\x22 styl\
 e=\x22stop-color:rg\
-b(255,154,153);s\
+b(255,185,185);s\
 top-opacity:1\x22 /\
 >\x0d\x0a    </linearG\
 radient>\x0d\x0a  </de\
 fs>\x0d\x0a  <g fill=\x22\
 url(#grad1)\x22>\x0d\x0a \
    <path\x0d\x0a      \
 d=\x22M9.752 6.193c\
@@ -1238,15 +1461,15 @@
 op offset=\x220%\x22 s\
 tyle=\x22stop-color\
 :rgb(0,138,225);\
 stop-opacity:1\x22 \
 />\x0d\x0a      <stop \
 offset=\x22100%\x22 st\
 yle=\x22stop-color:\
-rgb(135,206,250)\
+rgb(185,225,225)\
 ;stop-opacity:1\x22\
  />\x0d\x0a    </linea\
 rGradient>\x0d\x0a  </\
 defs>\x0d\x0a  <g fill\
 =\x22url(#grad1)\x22>\x0d\
 \x0a    <path\x0d\x0a    \
   d=\x22M9.752 6.19\
@@ -2441,14 +2664,93 @@
 L2 14.732l-.287-\
 .445L1.268 14l-.\
 026-.529L1 13l.2\
 42-.471.026-.529\
 .445-.287.287-.4\
 45.529-.026z\x22/>\x0a\
 </svg>\
+\x00\x00\x04\xc8\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 width=\x2216\
+\x22 height=\x2216\x22 fi\
+ll=\x22currentColor\
+\x22 class=\x22bi bi-d\
+atabase\x22 viewBox\
+=\x220 0 16 16\x22>\x0a  \
+<path fill=\x22whit\
+e\x22 d=\x22M4.318 2.6\
+87C5.234 2.271 6\
+.536 2 8 2s2.766\
+.27 3.682.687C12\
+.644 3.125 13 3.\
+627 13 4c0 .374-\
+.356.875-1.318 1\
+.313C10.766 5.72\
+9 9.464 6 8 6s-2\
+.766-.27-3.682-.\
+687C3.356 4.875 \
+3 4.373 3 4c0-.3\
+74.356-.875 1.31\
+8-1.313M13 5.698\
+V7c0 .374-.356.8\
+75-1.318 1.313C1\
+0.766 8.729 9.46\
+4 9 8 9s-2.766-.\
+27-3.682-.687C3.\
+356 7.875 3 7.37\
+3 3 7V5.698c.271\
+.202.58.378.904.\
+525C4.978 6.711 \
+6.427 7 8 7s3.02\
+2-.289 4.096-.77\
+7A5 5 0 0 0 13 5\
+.698M14 4c0-1.00\
+7-.875-1.755-1.9\
+04-2.223C11.022 \
+1.289 9.573 1 8 \
+1s-3.022.289-4.0\
+96.777C2.875 2.2\
+45 2 2.993 2 4v9\
+c0 1.007.875 1.7\
+55 1.904 2.223C4\
+.978 15.71 6.427\
+ 16 8 16s3.022-.\
+289 4.096-.777C1\
+3.125 14.755 14 \
+14.007 14 13zm-1\
+ 4.698V10c0 .374\
+-.356.875-1.318 \
+1.313C10.766 11.\
+729 9.464 12 8 1\
+2s-2.766-.27-3.6\
+82-.687C3.356 10\
+.875 3 10.373 3 \
+10V8.698c.271.20\
+2.58.378.904.525\
+C4.978 9.71 6.42\
+7 10 8 10s3.022-\
+.289 4.096-.777A\
+5 5 0 0 0 13 8.6\
+98m0 3V13c0 .374\
+-.356.875-1.318 \
+1.313C10.766 14.\
+729 9.464 15 8 1\
+5s-2.766-.27-3.6\
+82-.687C3.356 13\
+.875 3 13.373 3 \
+13v-1.302c.271.2\
+02.58.378.904.52\
+5C4.978 12.71 6.\
+427 13 8 13s3.02\
+2-.289 4.096-.77\
+7c.324-.147.633-\
+.323.904-.525\x22/>\
+\x0a</svg>\
 \x00\x00\x04\x09\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 width=\x2216\
 \x22 height=\x2216\x22 fi\
 ll=\x22currentColor\
@@ -2699,14 +3001,59 @@
 .5 3.5zm2.5 10a1\
 .5 1.5 0 1 0-3 0\
  1.5 1.5 0 0 0 3\
  0zm7 0a1.5 1.5 \
 0 1 0-3 0 1.5 1.\
 5 0 0 0 3 0z\x22/>\x0d\
 \x0a</svg>\
+\x00\x00\x02\xa1\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 width=\x2216\
+\x22 height=\x2216\x22 fi\
+ll=\x22currentColor\
+\x22 class=\x22bi bi-s\
+erver\x22 viewBox=\x22\
+0 0 16 16\x22>\x0a  <p\
+ath fill=\x22white\x22\
+ d=\x22M1.333 2.667\
+C1.333 1.194 4.3\
+18 0 8 0s6.667 1\
+.194 6.667 2.667\
+V4c0 1.473-2.985\
+ 2.667-6.667 2.6\
+67S1.333 5.473 1\
+.333 4z\x22/>\x0a  <pa\
+th fill=\x22white\x22 \
+d=\x22M1.333 6.334v\
+3C1.333 10.805 4\
+.318 12 8 12s6.6\
+67-1.194 6.667-2\
+.667V6.334a6.5 6\
+.5 0 0 1-1.458.7\
+9C11.81 7.684 9.\
+967 8 8 8s-3.809\
+-.317-5.208-.876\
+a6.5 6.5 0 0 1-1\
+.458-.79z\x22/>\x0a  <\
+path fill=\x22white\
+\x22 d=\x22M14.667 11.\
+668a6.5 6.5 0 0 \
+1-1.458.789c-1.4\
+.56-3.242.876-5.\
+21.876-1.966 0-3\
+.809-.316-5.208-\
+.876a6.5 6.5 0 0\
+ 1-1.458-.79v1.6\
+66C1.333 14.806 \
+4.318 16 8 16s6.\
+667-1.194 6.667-\
+2.667z\x22/>\x0a</svg>\
+\
 \x00\x00\x02\x84\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 width=\x2216\
 \x22 height=\x2216\x22 fi\
 ll=\x22currentColor\
@@ -2742,14 +3089,120 @@
 5 1.5 0 0 0 3.26\
 6 14h9.468a1.5 1\
 .5 0 0 0 1.489-1\
 .314l.64-5.124A.\
 5.5 0 0 0 14.367\
  7H1.633z\x22/>\x0a</s\
 vg>\
+\x00\x00\x06t\
+<\
+svg xmlns=\x22http:\
+//www.w3.org/200\
+0/svg\x22 width=\x2216\
+\x22 height=\x2216\x22 fi\
+ll=\x22currentColor\
+\x22 class=\x22bi bi-r\
+ocket-takeoff\x22 v\
+iewBox=\x220 0 16 1\
+6\x22>\x0a  <path fill\
+=\x22white\x22 d=\x22M9.7\
+52 6.193c.599.6 \
+1.73.437 2.528-.\
+362s.96-1.932.36\
+2-2.531c-.599-.6\
+-1.73-.438-2.528\
+.361-.798.8-.96 \
+1.933-.362 2.532\
+\x22/>\x0a  <path fill\
+=\x22white\x22 d=\x22M15.\
+811 3.312c-.363 \
+1.534-1.334 3.62\
+6-3.64 6.218l-.2\
+4 2.408a2.56 2.5\
+6 0 0 1-.732 1.5\
+26L8.817 15.85a.\
+51.51 0 0 1-.867\
+-.434l.27-1.899c\
+.04-.28-.013-.59\
+3-.131-.956a9 9 \
+0 0 0-.249-.657l\
+-.082-.202c-.815\
+-.197-1.578-.662\
+-2.191-1.277-.61\
+4-.615-1.079-1.3\
+79-1.275-2.195l-\
+.203-.083a10 10 \
+0 0 0-.655-.248c\
+-.363-.119-.675-\
+.172-.955-.132l-\
+1.896.27A.51.51 \
+0 0 1 .15 7.17l2\
+.382-2.386c.41-.\
+41.947-.67 1.524\
+-.734h.006l2.4-.\
+238C9.005 1.55 1\
+1.087.582 12.623\
+.208c.89-.217 1.\
+59-.232 2.08-.18\
+8.244.023.435.06\
+.57.093q.1.026.1\
+6.045c.184.06.27\
+9.13.351.295l.02\
+9.073a3.5 3.5 0 \
+0 1 .157.721c.05\
+5.485.051 1.178-\
+.159 2.065m-4.82\
+8 7.475.04-.04-.\
+107 1.081a1.54 1\
+.54 0 0 1-.44.91\
+3l-1.298 1.3.054\
+-.38c.072-.506-.\
+034-.993-.172-1.\
+418a9 9 0 0 0-.1\
+64-.45c.738-.065\
+ 1.462-.38 2.087\
+-1.006M5.205 5c-\
+.625.626-.94 1.3\
+51-1.004 2.09a9 \
+9 0 0 0-.45-.164\
+c-.424-.138-.91-\
+.244-1.416-.172l\
+-.38.054 1.3-1.3\
+c.245-.246.566-.\
+401.91-.44l1.08-\
+.107zm9.406-3.96\
+1c-.38-.034-.967\
+-.027-1.746.163-\
+1.558.38-3.917 1\
+.496-6.937 4.521\
+-.62.62-.799 1.3\
+4-.687 2.051.107\
+.676.483 1.362 1\
+.048 1.928.564.5\
+65 1.25.941 1.92\
+4 1.049.71.112 1\
+.429-.067 2.048-\
+.688 3.079-3.083\
+ 4.192-5.444 4.5\
+56-6.987.183-.77\
+1.18-1.345.138-1\
+.713a3 3 0 0 0-.\
+045-.283 3 3 0 0\
+ 0-.3-.041Z\x22/>\x0a \
+ <path fill=\x22whi\
+te\x22 d=\x22M7.009 12\
+.139a7.6 7.6 0 0\
+ 1-1.804-1.352A7\
+.6 7.6 0 0 1 3.7\
+94 8.86c-1.102.9\
+92-1.965 5.054-1\
+.839 5.18.125.12\
+6 3.936-.896 5.0\
+54-1.902Z\x22/>\x0a</s\
+vg>\
 \x00\x00\x02G\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 width=\x2216\
 \x22 height=\x2216\x22 fi\
 ll=\x22currentColor\
@@ -3266,14 +3719,18 @@
 \x00g\
 \x00e\x00a\x00r\x00-\x00w\x00i\x00d\x00e\x00-\x00c\x00o\x00n\x00n\x00e\x00c\x00t\
 \x00e\x00d\x00.\x00s\x00v\x00g\
 \x00\x09\
 \x066\xac\x07\
 \x00t\
 \x00o\x00o\x00l\x00s\x00.\x00s\x00v\x00g\
+\x00\x0c\
+\x05\xc9\x15\xc7\
+\x00d\
+\x00a\x00t\x00a\x00b\x00a\x00s\x00e\x00.\x00s\x00v\x00g\
 \x00\x0d\
 \x00&\xe7\xa7\
 \x00i\
 \x00n\x00c\x00o\x00g\x00n\x00i\x00t\x00o\x00.\x00s\x00v\x00g\
 \x00\x08\
 \x0f\xccUg\
 \x00w\
@@ -3295,18 +3752,27 @@
 \x00r\
 \x00o\x00c\x00k\x00e\x00t\x00-\x00t\x00a\x00k\x00e\x00o\x00f\x00f\x00.\x00s\x00v\
 \x00g\
 \x00\x0c\
 \x09\xa2O\x87\
 \x00s\
 \x00c\x00i\x00s\x00s\x00o\x00r\x00s\x00.\x00s\x00v\x00g\
+\x00\x0a\
+\x0c\xcac\xe7\
+\x00s\
+\x00e\x00r\x00v\x00e\x00r\x00.\x00s\x00v\x00g\
 \x00\x10\
 \x03SZ\xa7\
 \x00f\
 \x00o\x00l\x00d\x00e\x00r\x002\x00-\x00o\x00p\x00e\x00n\x00.\x00s\x00v\x00g\
+\x00\x1d\
+\x01\x86\x16\xe7\
+\x00m\
+\x00o\x00n\x00o\x00c\x00h\x00r\x00o\x00m\x00e\x00-\x00r\x00o\x00c\x00k\x00e\x00t\
+\x00-\x00t\x00a\x00k\x00e\x00o\x00f\x00f\x00.\x00s\x00v\x00g\
 \x00!\
 \x02\x1bj\xa7\
 \x00r\
 \x00o\x00c\x00k\x00e\x00t\x00-\x00t\x00a\x00k\x00e\x00o\x00f\x00f\x00-\x00c\x00o\
 \x00n\x00n\x00e\x00c\x00t\x00e\x00d\x00-\x00d\x00a\x00r\x00k\x00.\x00s\x00v\x00g\
 \
 \x00\x0b\
@@ -3387,141 +3853,153 @@
 "
 
 qt_resource_struct = b"\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x01\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x02\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x00\x10\x00\x02\x00\x00\x00#\x00\x00\x00\x03\
+\x00\x00\x00\x10\x00\x02\x00\x00\x00&\x00\x00\x00\x03\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x01\xae\x00\x00\x00\x00\x00\x01\x00\x00#-\
+\x00\x00\x01\xcc\x00\x00\x00\x00\x00\x01\x00\x00'\xec\
 \x00\x00\x01\x8akGd\x22\
-\x00\x00\x03\xbc\x00\x02\x00\x00\x00\x1c\x00\x00\x00&\
+\x00\x00\x044\x00\x02\x00\x00\x00\x1f\x00\x00\x00)\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x02\xa8\x00\x00\x00\x00\x00\x01\x00\x00<]\
-\x00\x00\x01\x89(\xfeb\x85\
-\x00\x00\x03V\x00\x00\x00\x00\x00\x01\x00\x00H\xe9\
-\x00\x00\x01\x89(\xfeb\x87\
-\x00\x00\x02\xf0\x00\x00\x00\x00\x00\x01\x00\x00DU\
+\x00\x00\x02\xe0\x00\x00\x00\x00\x00\x01\x00\x00C\x9a\
+\x00\x00\x01\x8f\x22\xaf\x9a?\
+\x00\x00\x03 \x00\x00\x00\x00\x00\x01\x00\x00I\xeb\
+\x00\x00\x01\x8f#\x02\xdc\x8e\
+\x00\x00\x03\xce\x00\x00\x00\x00\x00\x01\x00\x00Vw\
+\x00\x00\x01\x8f#\x0a=U\
+\x00\x00\x03h\x00\x00\x00\x00\x00\x01\x00\x00Q\xe3\
 \x00\x00\x01\x8dn|S\xe5\
-\x00\x00\x02\x06\x00\x00\x00\x00\x00\x01\x00\x00,Y\
+\x00\x00\x02$\x00\x00\x00\x00\x00\x01\x00\x001\x18\
 \x00\x00\x01\x89q\xdb\xa0\xb9\
-\x00\x00\x02\x82\x00\x00\x00\x00\x00\x01\x00\x009\xe2\
+\x00\x00\x02\xba\x00\x00\x00\x00\x00\x01\x00\x00A\x1f\
 \x00\x00\x01\x88j\xc4\x1f\xc9\
 \x00\x00\x00\x98\x00\x00\x00\x00\x00\x01\x00\x00\x0a\xe5\
 \x00\x00\x01\x8dZ\x0d\x14\xb2\
-\x00\x00\x01\xe4\x00\x00\x00\x00\x00\x01\x00\x00*\xc0\
+\x00\x00\x02\x02\x00\x00\x00\x00\x00\x01\x00\x00/\x7f\
 \x00\x00\x01\x8dK\x97\x88\xed\
-\x00\x00\x03\xf4\x00\x00\x00\x00\x00\x01\x00\x00Y7\
+\x00\x00\x04l\x00\x00\x00\x00\x00\x01\x00\x00f\xc5\
 \x00\x00\x01\x8dZ4O\xe8\
-\x00\x00\x04\xca\x00\x00\x00\x00\x00\x01\x00\x00i\xe5\
+\x00\x00\x05B\x00\x00\x00\x00\x00\x01\x00\x00ws\
 \x00\x00\x01\x87x\xc2\xafR\
-\x00\x00\x02:\x00\x00\x00\x00\x00\x01\x00\x0009\
+\x00\x00\x02X\x00\x00\x00\x00\x00\x01\x00\x004\xf8\
 \x00\x00\x01\x87x\xc2\xafS\
-\x00\x00\x02\x1e\x00\x00\x00\x00\x00\x01\x00\x00-\xe0\
+\x00\x00\x02<\x00\x00\x00\x00\x00\x01\x00\x002\x9f\
 \x00\x00\x01\x8akGd\x22\
+\x00\x00\x01\xae\x00\x00\x00\x00\x00\x01\x00\x00#-\
+\x00\x00\x01\x8f$IE\xc7\
 \x00\x00\x01\x96\x00\x00\x00\x00\x00\x01\x00\x00\x1f\x8f\
 \x00\x00\x01\x8dc\xb0\xf9\xfd\
-\x00\x00\x03\xcc\x00\x00\x00\x00\x00\x01\x00\x00V\xee\
+\x00\x00\x04D\x00\x00\x00\x00\x00\x01\x00\x00d|\
 \x00\x00\x01\x89q\xe4\xd2~\
 \x00\x00\x00t\x00\x00\x00\x00\x00\x01\x00\x00\x08\x8e\
 \x00\x00\x01\x8dn\x81\xcf\xd7\
-\x00\x00\x04\x18\x00\x00\x00\x00\x00\x01\x00\x00[\x07\
+\x00\x00\x04\x90\x00\x00\x00\x00\x00\x01\x00\x00h\x95\
 \x00\x00\x01\x8akGd\x22\
 \x00\x00\x00Z\x00\x00\x00\x00\x00\x01\x00\x00\x01z\
 \x00\x00\x01\x85a_\xd8\xe6\
 \x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x10[\
 \x00\x00\x01\x8a\xb6\xf3\x1c:\
-\x00\x00\x05X\x00\x00\x00\x00\x00\x01\x00\x00u\x1e\
+\x00\x00\x05\xd0\x00\x00\x00\x00\x00\x01\x00\x00\x82\xac\
 \x00\x00\x01\x88j\xc3_y\
-\x00\x00\x03\x0c\x00\x00\x00\x00\x00\x01\x00\x00F\x93\
+\x00\x00\x03\x84\x00\x00\x00\x00\x00\x01\x00\x00T!\
 \x00\x00\x01\x89\xdf:\xd3\xbe\
-\x00\x00\x02d\x00\x00\x00\x00\x00\x01\x00\x0083\
+\x00\x00\x02\x82\x00\x00\x00\x00\x00\x01\x00\x00<\xf2\
 \x00\x00\x01\x89q\xdb\xa0\xb9\
-\x00\x00\x04\x80\x00\x00\x00\x00\x00\x01\x00\x00d\xb4\
+\x00\x00\x04\xf8\x00\x00\x00\x00\x00\x01\x00\x00rB\
 \x00\x00\x01\x89q\xdb\xa0\xb9\
 \x00\x00\x01*\x00\x00\x00\x00\x00\x01\x00\x00\x12q\
 \x00\x00\x01\x87\x09\x8a\x8e<\
-\x00\x00\x03\xa6\x00\x00\x00\x00\x00\x01\x00\x00To\
+\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x00a\xfd\
 \x00\x00\x01\x8a\x97O\x0e\xd4\
-\x00\x00\x058\x00\x00\x00\x00\x00\x01\x00\x00t\x09\
+\x00\x00\x05\xb0\x00\x00\x00\x00\x00\x01\x00\x00\x81\x97\
 \x00\x00\x01\x85b\x0b\xe8\xa4\
-\x00\x00\x032\x00\x00\x00\x00\x00\x01\x00\x00G\xc7\
+\x00\x00\x03\xaa\x00\x00\x00\x00\x00\x01\x00\x00UU\
 \x00\x00\x01\x85b\x0b\xdc\xdc\
-\x00\x00\x04\xb0\x00\x00\x00\x00\x00\x01\x00\x00f/\
+\x00\x00\x05(\x00\x00\x00\x00\x00\x01\x00\x00s\xbd\
 \x00\x00\x01\x8dnV\xcf6\
-\x00\x00\x05\x08\x00\x00\x00\x00\x00\x01\x00\x00q\xdd\
+\x00\x00\x05\x80\x00\x00\x00\x00\x00\x01\x00\x00\x7fk\
 \x00\x00\x01\x85ae+\xea\
-\x00\x00\x046\x00\x00\x00\x00\x00\x01\x00\x00\x5c\xb9\
+\x00\x00\x04\xae\x00\x00\x00\x00\x00\x01\x00\x00jG\
 \x00\x00\x01\x8b\x9erg^\
-\x00\x00\x03\x8a\x00\x00\x00\x00\x00\x01\x00\x00P\xe3\
+\x00\x00\x02\xa0\x00\x00\x00\x00\x00\x01\x00\x00>\xa1\
+\x00\x00\x01\x8f#\xf5\xc6\xf5\
+\x00\x00\x04\x02\x00\x00\x00\x00\x00\x01\x00\x00^q\
 \x00\x00\x01\x88\xbf\xc3#\xed\
 \x00\x00\x01b\x00\x00\x00\x00\x00\x01\x00\x00\x1ak\
 \x00\x00\x01\x85ae\x0eD\
 \x00\x00\x00\xb8\x00\x00\x00\x00\x00\x01\x00\x00\x0e\xc3\
 \x00\x00\x01\x88e~\x9cP\
 \x00\x00\x00(\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x89q\xdb\xa0\xb9\
-\x00\x00\x01\xce\x00\x00\x00\x00\x00\x01\x00\x00'-\
+\x00\x00\x01\xec\x00\x00\x00\x00\x00\x01\x00\x00+\xec\
 \x00\x00\x01\x8dn\x7f\x82l\
-\x00\x00\x01\xae\x00\x00\x00\x00\x00\x01\x00\x00\x92\x8e\
+\x00\x00\x01\xcc\x00\x00\x00\x00\x00\x01\x00\x00\xa4\xe8\
 \x00\x00\x01\x8akGd#\
-\x00\x00\x02\xf0\x00\x00\x00\x00\x00\x01\x00\x00\xa4`\
+\x00\x00\x02\xe0\x00\x00\x00\x00\x00\x01\x00\x00\xb9_\
+\x00\x00\x01\x8f\x22\xb2]\xff\
+\x00\x00\x03h\x00\x00\x00\x00\x00\x01\x00\x00\xbf\xd7\
 \x00\x00\x01\x8dn|\xdf\xb8\
-\x00\x00\x02\x06\x00\x00\x00\x00\x00\x01\x00\x00\x9b\xee\
+\x00\x00\x02$\x00\x00\x00\x00\x00\x01\x00\x00\xaeH\
 \x00\x00\x01\x89q\xdb\xa0\xba\
-\x00\x00\x02\x82\x00\x00\x00\x00\x00\x01\x00\x00\xa1\xd8\
+\x00\x00\x02\xba\x00\x00\x00\x00\x00\x01\x00\x00\xb6\xd7\
 \x00\x00\x01\x893\xb5sJ\
-\x00\x00\x00\x98\x00\x00\x00\x00\x00\x01\x00\x00\x81\xf2\
+\x00\x00\x00\x98\x00\x00\x00\x00\x00\x01\x00\x00\x8f\x80\
 \x00\x00\x01\x8dZ\x0d\xc0*\
-\x00\x00\x01\xe4\x00\x00\x00\x00\x00\x01\x00\x00\x9aH\
+\x00\x00\x02\x02\x00\x00\x00\x00\x00\x01\x00\x00\xac\xa2\
 \x00\x00\x01\x8dK\x98d\x1a\
-\x00\x00\x03\xf4\x00\x00\x00\x00\x00\x01\x00\x00\xb1\xad\
+\x00\x00\x04l\x00\x00\x00\x00\x00\x01\x00\x00\xcd$\
 \x00\x00\x01\x8d]\xad\xfa\x8a\
-\x00\x00\x02\x1e\x00\x00\x00\x00\x00\x01\x00\x00\x9d\x82\
+\x00\x00\x02<\x00\x00\x00\x00\x00\x01\x00\x00\xaf\xdc\
 \x00\x00\x01\x8akGd#\
-\x00\x00\x01\x96\x00\x00\x00\x00\x00\x01\x00\x00\x8e\xe3\
+\x00\x00\x01\xae\x00\x00\x00\x00\x00\x01\x00\x00\xa0\x1c\
+\x00\x00\x01\x8f$Zj\xb7\
+\x00\x00\x01\x96\x00\x00\x00\x00\x00\x01\x00\x00\x9cq\
 \x00\x00\x01\x8dc\xb1\x90K\
-\x00\x00\x03\xcc\x00\x00\x00\x00\x00\x01\x00\x00\xafM\
+\x00\x00\x04D\x00\x00\x00\x00\x00\x01\x00\x00\xca\xc4\
 \x00\x00\x01\x893\xb5s^\
-\x00\x00\x00t\x00\x00\x00\x00\x00\x01\x00\x00\x7f\x81\
+\x00\x00\x00t\x00\x00\x00\x00\x00\x01\x00\x00\x8d\x0f\
 \x00\x00\x01\x8dn\x83K\x08\
-\x00\x00\x04\x18\x00\x00\x00\x00\x00\x01\x00\x00\xb3\x97\
+\x00\x00\x04\x90\x00\x00\x00\x00\x00\x01\x00\x00\xcf\x0e\
 \x00\x00\x01\x8akGd\x22\
-\x00\x00\x00Z\x00\x00\x00\x00\x00\x01\x00\x00x`\
+\x00\x00\x00Z\x00\x00\x00\x00\x00\x01\x00\x00\x85\xee\
 \x00\x00\x01\x893\xb5sr\
-\x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x87\x82\
+\x00\x00\x00\xe6\x00\x00\x00\x00\x00\x01\x00\x00\x95\x10\
 \x00\x00\x01\x8a\xb6\xf3\x1c;\
-\x00\x00\x05X\x00\x00\x00\x00\x00\x01\x00\x00\xbe=\
+\x00\x00\x05\xd0\x00\x00\x00\x00\x00\x01\x00\x00\xd9\xb4\
 \x00\x00\x01\x893\xb5sE\
-\x00\x00\x03\x0c\x00\x00\x00\x00\x00\x01\x00\x00\xa6\xab\
+\x00\x00\x03\x84\x00\x00\x00\x00\x00\x01\x00\x00\xc2\x22\
 \x00\x00\x01\x89\xe3\x00+b\
-\x00\x00\x02d\x00\x00\x00\x00\x00\x01\x00\x00\xa0\x1c\
+\x00\x00\x02\x82\x00\x00\x00\x00\x00\x01\x00\x00\xb2v\
 \x00\x00\x01\x89q\xdb\xa0\xba\
-\x00\x00\x04\x80\x00\x00\x00\x00\x00\x01\x00\x00\xb5c\
+\x00\x00\x04\xf8\x00\x00\x00\x00\x00\x01\x00\x00\xd0\xda\
 \x00\x00\x01\x89q\xdb\xa0\xba\
-\x00\x00\x03\xa6\x00\x00\x00\x00\x00\x01\x00\x00\xac\xc1\
+\x00\x00\x04\x1e\x00\x00\x00\x00\x00\x01\x00\x00\xc88\
 \x00\x00\x01\x8a\x97O\xa6\xc0\
-\x00\x00\x058\x00\x00\x00\x00\x00\x01\x00\x00\xbd\x1b\
+\x00\x00\x05\xb0\x00\x00\x00\x00\x00\x01\x00\x00\xd8\x92\
 \x00\x00\x01\x893\xb5sg\
-\x00\x00\x032\x00\x00\x00\x00\x00\x01\x00\x00\xa7\xec\
+\x00\x00\x03\xaa\x00\x00\x00\x00\x00\x01\x00\x00\xc3c\
 \x00\x00\x01\x893\xb5sZ\
-\x00\x00\x04\xb0\x00\x00\x00\x00\x00\x01\x00\x00\xb6\xeb\
+\x00\x00\x05(\x00\x00\x00\x00\x00\x01\x00\x00\xd2b\
 \x00\x00\x01\x8dnW\xb0\xbd\
-\x00\x00\x05\x08\x00\x00\x00\x00\x00\x01\x00\x00\xba\xd5\
+\x00\x00\x05\x80\x00\x00\x00\x00\x00\x01\x00\x00\xd6L\
 \x00\x00\x01\x893\xb5sv\
-\x00\x00\x03\x8a\x00\x00\x00\x00\x00\x01\x00\x00\xa9\x1b\
+\x00\x00\x02\xa0\x00\x00\x00\x00\x00\x01\x00\x00\xb42\
+\x00\x00\x01\x8f#\xf6\xdf|\
+\x00\x00\x04\x02\x00\x00\x00\x00\x00\x01\x00\x00\xc4\x92\
 \x00\x00\x01\x893\xb5sP\
-\x00\x00\x01b\x00\x00\x00\x00\x00\x01\x00\x00\x89\xb2\
+\x00\x00\x01b\x00\x00\x00\x00\x00\x01\x00\x00\x97@\
 \x00\x00\x01\x893\xb5sU\
-\x00\x00\x00\xb8\x00\x00\x00\x00\x00\x01\x00\x00\x85\xdd\
+\x00\x00\x00\xb8\x00\x00\x00\x00\x00\x01\x00\x00\x93k\
 \x00\x00\x01\x893\xb5sl\
-\x00\x00\x00(\x00\x00\x00\x00\x00\x01\x00\x00v\xd9\
+\x00\x00\x00(\x00\x00\x00\x00\x00\x01\x00\x00\x84g\
 \x00\x00\x01\x89q\xdb\xa0\xba\
-\x00\x00\x01\xce\x00\x00\x00\x00\x00\x01\x00\x00\x96\x9b\
+\x00\x00\x01\xec\x00\x00\x00\x00\x00\x01\x00\x00\xa8\xf5\
 \x00\x00\x01\x8dn\x80v\xb5\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
```

### Comparing `Furious-GUI-0.3.9/Furious/Utility/AppSettings.py` & `Furious-GUI-0.4.0/Furious/Utility/AppSettings.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/AppSettingsFn.py` & `Furious-GUI-0.4.0/Furious/Utility/AppSettingsFn.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/Constants.py` & `Furious-GUI-0.4.0/Furious/Utility/Constants.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/PySide6Legacy.py` & `Furious-GUI-0.4.0/Furious/Utility/PySide6Legacy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/StartupOnBoot.py` & `Furious-GUI-0.4.0/Furious/Utility/StartupOnBoot.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/SystemProxy.py` & `Furious-GUI-0.4.0/Furious/Utility/SystemProxy.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/SystemRoutingTable.py` & `Furious-GUI-0.4.0/Furious/Utility/SystemRoutingTable.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Utility/SystemRuntime.py` & `Furious-GUI-0.4.0/Furious/Utility/SystemRuntime.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 def getPythonVersion():
     return '.'.join(str(info) for info in sys.version_info)
 
 
 @functools.lru_cache(None)
 def getUbuntuRelease() -> str:
     try:
+        if PLATFORM != 'Linux':
+            return ''
+
         result = runExternalCommand(
             ['cat', '/etc/lsb-release'],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             check=True,
         )
```

### Comparing `Furious-GUI-0.3.9/Furious/Utility/Utility.py` & `Furious-GUI-0.4.0/Furious/Utility/Utility.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     'Protocol',
     'BinarySettings',
     'protocolRepr',
     'isValidIPAddress',
     'parseHostPort',
     'runExternalCommand',
     'getAbsolutePath',
+    'getXrayProxyOutboundObject',
+    'getXrayProxyOutboundStream',
 ]
 
 
 class Protocol:
     VMess = 'VMess'
     VLESS = 'VLESS'
     Shadowsocks = 'Shadowsocks'
@@ -53,14 +55,17 @@
     ON_ = '1'
 
     RANGE = [OFF, ON_]
 
 
 @functools.lru_cache(None)
 def protocolRepr(protocol: str) -> str:
+    if not isinstance(protocol, str):
+        return ''
+
     if protocol.lower() == 'vmess':
         return Protocol.VMess
 
     if protocol.lower() == 'vless':
         return Protocol.VLESS
 
     if protocol.lower() == 'shadowsocks':
@@ -101,7 +106,30 @@
         return subprocess.run(*args, creationflags=creationflags, **kwargs)
     else:
         return subprocess.run(*args, **kwargs)
 
 
 def getAbsolutePath(path):
     return path if os.path.isabs(path) else str(ROOT_DIR / path)
+
+
+def getXrayProxyOutboundObject(config: dict) -> dict:
+    if not isinstance(config.get('outbounds'), list):
+        config['outbounds'] = []
+
+    for outbound in config['outbounds']:
+        if isinstance(outbound, dict):
+            tag = outbound.get('tag')
+
+            if isinstance(tag, str) and tag == 'proxy':
+                return outbound
+
+    return {}
+
+
+def getXrayProxyOutboundStream(config: dict) -> dict:
+    proxyOutboundObject = getXrayProxyOutboundObject(config)
+
+    if not isinstance(proxyOutboundObject.get('streamSettings'), dict):
+        proxyOutboundObject['streamSettings'] = {}
+
+    return proxyOutboundObject['streamSettings']
```

### Comparing `Furious-GUI-0.3.9/Furious/Utility/__init__.py` & `Furious-GUI-0.4.0/Furious/Utility/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Version.py` & `Furious-GUI-0.4.0/Furious/Version.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.3.9'
+__version__ = '0.4.0'
```

### Comparing `Furious-GUI-0.3.9/Furious/Widget/Application.py` & `Furious-GUI-0.4.0/Furious/Widget/Application.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from PySide6.QtNetwork import *
 from PySide6.QtWidgets import *
 
 import os
 import sys
 import time
 import logging
+import platform
 import threading
 import traceback
 import functools
 import qdarkstyle
 import darkdetect
 
 logger = logging.getLogger(__name__)
@@ -301,14 +302,18 @@
             logger.info(f'application version: {APPLICATION_VERSION}')
             logger.info(
                 f'Qt version: {QtCore.qVersion()}. PySide6 version: {PYSIDE6_VERSION}'
             )
             logger.info(f'platform: {PLATFORM}')
             logger.info(f'platform release: {PLATFORM_RELEASE}')
             logger.info(f'platform machine: {PLATFORM_MACHINE}')
+
+            if PLATFORM == 'Darwin':
+                logger.info(f'mac_ver: {platform.mac_ver()}')
+
             logger.info(f'python version: {getPythonVersion()}')
             logger.info(f'system version: {sys.version}')
             logger.info(f'sys.executable: {sys.executable}')
             logger.info(f'sys.argv: {sys.argv}')
             logger.info(f'appFilePath: {self.applicationFilePath()}')
             logger.info(f'isPythonw: {isPythonw()}')
             logger.info(f'system language is {SYSTEM_LANGUAGE}')
```

### Comparing `Furious-GUI-0.3.9/Furious/Widget/ConnectProgressBar.py` & `Furious-GUI-0.4.0/Furious/Widget/ConnectProgressBar.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Widget/IndentSpinBox.py` & `Furious-GUI-0.4.0/Furious/Widget/IndentSpinBox.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,38 +38,30 @@
 
 class IndentSpinBox(AppQDialog):
     def __init__(self, parent=None):
         super().__init__(parent)
 
         self.setWindowTitle(_('Set Indent'))
 
-        self.indentText = QLabel(_('Indent:'))
+        self.indentText = AppQLabel(_('Indent:'))
 
         self.indentSpin = QSpinBox()
         self.indentSpin.setRange(0, 8)
         self.indentSpin.setValue(2)
 
-        self.dialogBtns = QDialogButtonBox(QtCore.Qt.Orientation.Horizontal)
-
-        self.dialogBtns.addButton(_('OK'), QDialogButtonBox.ButtonRole.AcceptRole)
-        self.dialogBtns.addButton(_('Cancel'), QDialogButtonBox.ButtonRole.RejectRole)
+        self.dialogBtns = AppQDialogButtonBox(QtCore.Qt.Orientation.Horizontal)
+        self.dialogBtns.addButton(_('OK'), AppQDialogButtonBox.ButtonRole.AcceptRole)
+        self.dialogBtns.addButton(
+            _('Cancel'), AppQDialogButtonBox.ButtonRole.RejectRole
+        )
         self.dialogBtns.accepted.connect(self.accept)
         self.dialogBtns.rejected.connect(self.reject)
 
         layout = QFormLayout()
-
         layout.addRow(self.indentText, self.indentSpin)
         layout.addRow(self.dialogBtns)
         layout.setFormAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
 
         self.setLayout(layout)
 
     def value(self):
         return self.indentSpin.value()
-
-    def retranslate(self):
-        self.setWindowTitle(_(self.windowTitle()))
-
-        self.indentText.setText(_(self.indentText.text()))
-
-        for button in self.dialogBtns.buttons():
-            button.setText(_(button.text()))
```

### Comparing `Furious-GUI-0.3.9/Furious/Widget/UserServersQTableWidget.py` & `Furious-GUI-0.4.0/Furious/Widget/UserServersQTableWidget.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 from Furious.PyFramework import *
 from Furious.QtFramework import *
 from Furious.QtFramework import gettext as _
 from Furious.Utility import *
 from Furious.Library import *
 from Furious.Core import *
 from Furious.TrayActions.Import import *
+from Furious.Widget.GuiHysteria1 import *
+from Furious.Widget.GuiHysteria2 import *
+from Furious.Widget.GuiShadowsocks import *
+from Furious.Widget.GuiTrojan import *
+from Furious.Widget.GuiVLESS import *
+from Furious.Widget.GuiVMess import *
 from Furious.Window.QRCodeWindow import *
 from Furious.Window.TextEditorWindow import *
 
 from PySide6 import QtCore
 from PySide6.QtGui import *
 from PySide6.QtWidgets import *
 from PySide6.QtNetwork import *
@@ -202,15 +208,16 @@
 
             def classname(ob) -> str:
                 return ob.__class__.__name__
 
             self.currentItem.setExtras('delayResult', classname(ex))
             self.updateResult()
         else:
-            if result.is_alive:
+            # Result address should not be empty
+            if result.address and result.is_alive:
                 self.currentItem.setExtras('delayResult', f'{round(result.avg_rtt)}ms')
             else:
                 if result.packet_loss == 1:
                     self.currentItem.setExtras('delayResult', 'Timeout')
                 else:
                     self.currentItem.setExtras('delayResult', 'Error')
 
@@ -584,15 +591,15 @@
     'Address',
     'Port',
     'Transport',
     'TLS',
     'Subscription',
     'Latency',
     'Speed',
-    'Edit Configuration...',
+    'Customize JSON Configuration...',
     'Move Up',
     'Move Down',
     'Duplicate',
     'Delete',
     'Select All',
     'Scroll To Activated Server',
     'Test Ping Latency',
@@ -631,18 +638,14 @@
         self.testDownloadSpeedTimer = QtCore.QTimer()
         self.testDownloadSpeedTimer.timeout.connect(self.handleTestDownloadSpeedJob)
         self.testDownloadSpeedTimer.start(250)
 
         # Text Editor Window
         self.textEditorWindow = TextEditorWindow()
 
-        # Delegate
-        self._delegate = AppQStyledItemDelegate(parent=self)
-        self.setItemDelegate(self._delegate)
-
         # Must set before flush all
         self.setColumnCount(len(self.Headers))
 
         # Flush all data to table
         self.flushAll()
 
         # Install custom header
@@ -669,15 +672,15 @@
         # No drag and drop
         self.setDragEnabled(False)
         self.setDragDropMode(QAbstractItemView.DragDropMode.NoDragDrop)
         self.setDropIndicatorShown(False)
         self.setDefaultDropAction(QtCore.Qt.DropAction.IgnoreAction)
 
         self.editConfigActionRef = AppQAction(
-            _('Edit Configuration...'),
+            _('Customize JSON Configuration...'),
             icon=bootstrapIcon('pencil-square.svg'),
             callback=lambda: self.editSelectedItemConfiguration(),
             shortcut=QtCore.QKeyCombination(
                 QtCore.Qt.KeyboardModifier.ControlModifier,
                 QtCore.Qt.Key.Key_E,
             ),
         )
@@ -802,14 +805,16 @@
         self.contextMenu = AppQMenu(*contextMenuActions)
 
         # Add actions to self in order to activate shortcuts
         self.addActions(self.contextMenu.actions())
         self.setContextMenuPolicy(QtCore.Qt.ContextMenuPolicy.CustomContextMenu)
         self.customContextMenuRequested.connect(self.handleCustomContextMenuRequested)
 
+        # Distinguish double-click and activated
+        self.doubleClickedFlag = False
         # Signals
         self.itemChanged.connect(self.handleItemChanged)
         self.itemSelectionChanged.connect(self.handleItemSelectionChanged)
         self.itemActivated.connect(self.handleItemActivated)
         self.itemDoubleClicked.connect(self.handleItemDoubleClicked)
 
         if self.activatedItem() is not None:
@@ -833,14 +838,20 @@
         if len(self.selectedIndex) > 1:
             self.editConfigActionRef.setDisabled(True)
         else:
             self.editConfigActionRef.setDisabled(False)
 
     @QtCore.Slot(QTableWidgetItem)
     def handleItemActivated(self, item: QTableWidgetItem):
+        if self.doubleClickedFlag:
+            # Ignore double-click
+            self.doubleClickedFlag = False
+
+            return
+
         oldIndex = AS_UserActivatedItemIndex()
         newIndex = item.row()
 
         if oldIndex == newIndex:
             # Same item activated. Do nothing
             return
 
@@ -849,40 +860,132 @@
             mbox.setWindowTitle(_('Connecting'))
             mbox.setText(_('Connecting. Please wait'))
 
             if PLATFORM != 'Darwin':
                 # Show the MessageBox asynchronously
                 mbox.open()
             else:
-                # Show the MessageBox and wait for user to close it
-                mbox.exec()
+                # Show the MessageBox asynchronously
+                # TODO: Verify
+                mbox.open()
 
             return
 
         if oldIndex >= 0:
             self.activateItemByIndex(oldIndex, False)
 
         self.activateItemByIndex(newIndex, True)
 
         if APP().isSystemTrayConnected():
             APP().systemTray.ConnectAction.doDisconnect()
             APP().systemTray.ConnectAction.trigger()
 
+    def getGuiEditorByFactory(self, factory, **kwargs):
+        if isinstance(factory, ConfigurationXray):
+            protocol = factory.proxyProtocol
+
+            if protocolRepr(protocol) == Protocol.VMess:
+                guiEditor = GuiVMess(parent=self, **kwargs)
+            elif protocolRepr(protocol) == Protocol.VLESS:
+                guiEditor = GuiVLESS(parent=self, **kwargs)
+            elif protocolRepr(protocol) == Protocol.Shadowsocks:
+                guiEditor = GuiShadowsocks(parent=self, **kwargs)
+            elif protocolRepr(protocol) == Protocol.Trojan:
+                guiEditor = GuiTrojan(parent=self, **kwargs)
+            else:
+                guiEditor = None
+        elif isinstance(factory, ConfigurationHysteria2):
+            guiEditor = GuiHysteria2(parent=self, **kwargs)
+        elif isinstance(factory, ConfigurationHysteria1):
+            guiEditor = GuiHysteria1(parent=self, **kwargs)
+        else:
+            guiEditor = None
+
+        return guiEditor
+
     @QtCore.Slot(QTableWidgetItem)
     def handleItemDoubleClicked(self, item: QTableWidgetItem):
-        pass
+        self.doubleClickedFlag = True
+
+        index = item.row()
+        factory = AS_UserServers()[index]
+
+        guiEditor = self.getGuiEditorByFactory(factory, translatable=False)
+
+        if guiEditor is None:
+            # Unrecognized. Do nothing
+            return
+
+        # Dummy ref
+        setattr(self, '_guiEditorRef0', guiEditor)
+
+        guiEditor.setWindowTitle(f'{index + 1} - ' + factory.getExtras('remark'))
+
+        try:
+            guiEditor.factoryToInput(factory)
+        except Exception as ex:
+            # Any non-exit exceptions
+
+            logger.error(f'error while converting factory to input: {ex}')
+
+        def handleAccepted():
+            modified = guiEditor.inputToFactory(factory)
+
+            self.flushRow(index, factory)
+
+            if index == AS_UserActivatedItemIndex():
+                try:
+                    if modified and APP().isSystemTrayConnected():
+                        mbox = NewChangesNextTimeMBox()
+
+                        # Show the MessageBox asynchronously
+                        mbox.open()
+                except Exception:
+                    # Any non-exit exceptions
+
+                    pass
+
+        guiEditor.connectAccepted(handleAccepted)
+        guiEditor.open()
 
     @QtCore.Slot(QtCore.QPoint)
     def handleCustomContextMenuRequested(self, point):
         self.contextMenu.exec(self.mapToGlobal(point))
 
     def customSortFn(self, clickedIndex, **kwargs):
-        AS_UserServers().sort(
-            key=lambda server: self.Headers[clickedIndex](server), **kwargs
-        )
+        def keyFn(server):
+            data = self.Headers[clickedIndex](server)
+
+            if clickedIndex == self.Headers.index('Latency'):
+                if data.endswith('ms'):
+                    # Strip value
+                    data = data[:-2]
+
+                try:
+                    return float(data)
+                except Exception:
+                    # Any non-exit exceptions
+
+                    return abs(hash(data)) + 2**20
+
+            if clickedIndex == self.Headers.index('Speed'):
+                if data.endswith(' M/s'):
+                    # Strip value
+                    data = data[:-4]
+
+                try:
+                    return float(data)
+                except Exception:
+                    # Any non-exit exceptions
+
+                    return abs(hash(data)) + 2**20
+
+            return data
+
+        AS_UserServers().sort(key=keyFn, **kwargs)
 
         self.flushAll()
 
     def activatedItem(self) -> QTableWidgetItem:
         return self.item(AS_UserActivatedItemIndex(), 0)
 
     def activateItemByIndex(self, index, activate):
@@ -911,28 +1014,70 @@
             # Use existing
             newItem.setFont(oldItem.font())
             newItem.setForeground(oldItem.foreground())
 
             if oldItem.textAlignment() != 0:
                 newItem.setTextAlignment(oldItem.textAlignment())
 
-        if str(header) == 'Remark':
-            # Remark is editable
-            newItem.setFlags(
-                QtCore.Qt.ItemFlag.ItemIsEnabled
-                | QtCore.Qt.ItemFlag.ItemIsSelectable
-                | QtCore.Qt.ItemFlag.ItemIsEditable
-            )
-        else:
-            newItem.setFlags(
-                QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
-            )
+        #
+        # Legacy flags. Not used
+        #
+        # if str(header) == 'Remark':
+        #     # Remark is editable
+        #     newItem.setFlags(
+        #         QtCore.Qt.ItemFlag.ItemIsEnabled
+        #         | QtCore.Qt.ItemFlag.ItemIsSelectable
+        #         | QtCore.Qt.ItemFlag.ItemIsEditable
+        #     )
+        # else:
+        #     newItem.setFlags(
+        #         QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
+        #     )
+
+        # Remark is now editable via GUI window
+        newItem.setFlags(
+            QtCore.Qt.ItemFlag.ItemIsEnabled | QtCore.Qt.ItemFlag.ItemIsSelectable
+        )
 
         self.setItem(row, column, newItem)
 
+    def addServerViaGui(
+        self,
+        protocol: str,
+        windowTitle: str = APPLICATION_NAME,
+        **kwargs,
+    ):
+        factory = getEmptyFactory(protocol)
+
+        guiEditor = self.getGuiEditorByFactory(factory, **kwargs)
+
+        if guiEditor is None:
+            # Unrecognized. Do nothing
+            return
+
+        # Dummy ref
+        setattr(self, '_guiEditorRef1', guiEditor)
+
+        guiEditor.setWindowTitle(windowTitle)
+
+        try:
+            guiEditor.factoryToInput(factory)
+        except Exception as ex:
+            # Any non-exit exceptions
+
+            logger.error(f'error while converting factory to input: {ex}')
+
+        def handleAccepted():
+            guiEditor.inputToFactory(factory)
+
+            self.appendNewItemByFactory(factory)
+
+        guiEditor.connectAccepted(handleAccepted)
+        guiEditor.open()
+
     def flushRow(self, row: int, item: ConfigurationFactory):
         for column in list(range(self.columnCount())):
             self.flushItem(row, column, item)
 
     def flushAll(self):
         if self.rowCount() == 0:
             # Should insert row
@@ -1070,26 +1215,31 @@
     def deleteSelectedItem(self):
         indexes = self.selectedIndex
 
         if len(indexes) == 0:
             # Nothing selected. Do nothing
             return
 
+        def handleResultCode(_indexes, code):
+            if code == PySide6LegacyEnumValueWrapper(AppQMessageBox.StandardButton.Yes):
+                self.deleteItemByIndex(_indexes)
+            else:
+                pass
+
         mbox = QuestionDeleteMBox(icon=AppQMessageBox.Icon.Question)
         mbox.isMulti = bool(len(indexes) > 1)
         mbox.possibleRemark = f'{indexes[0] + 1} - {self.item(indexes[0], 0).text()}'
         mbox.setText(mbox.customText())
+        mbox.finished.connect(functools.partial(handleResultCode, indexes))
 
-        if mbox.exec() == PySide6LegacyEnumValueWrapper(
-            AppQMessageBox.StandardButton.No
-        ):
-            # Do not delete
-            return
+        # dummy ref
+        setattr(self, '_questionDeleteMBox', mbox)
 
-        self.deleteItemByIndex(indexes)
+        # Show the MessageBox asynchronously
+        mbox.open()
 
     def editSelectedItemConfiguration(self):
         indexes = self.selectedIndex
 
         if len(indexes) == 0:
             # Nothing selected. Do nothing
             return
@@ -1323,14 +1473,20 @@
 
     def hideTabAndSpaces(self):
         self.textEditorWindow.hideTabAndSpaces()
 
     def keyPressEvent(self, event):
         if event.key() == QtCore.Qt.Key.Key_Delete:
             self.deleteSelectedItem()
+        elif event.key() == QtCore.Qt.Key.Key_Return:
+            if PLATFORM == 'Darwin':
+                # Activate by Enter key on macOS
+                self.itemActivated.emit(self.currentItem())
+            else:
+                super().keyPressEvent(event)
         else:
             super().keyPressEvent(event)
 
     def disconnectedCallback(self):
         super().disconnectedCallback()
 
         self.activateItemByIndex(AS_UserActivatedItemIndex(), True)
```

### Comparing `Furious-GUI-0.3.9/Furious/Widget/UserSubsQTableWidget.py` & `Furious-GUI-0.4.0/Furious/Widget/UserSubsQTableWidget.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,18 +80,14 @@
     ]
 
     def __init__(self, *args, **kwargs):
         self.deleteUniqueCallback = kwargs.pop('deleteUniqueCallback', None)
 
         super().__init__(*args, **kwargs)
 
-        # Delegate
-        self._delegate = AppQStyledItemDelegate(parent=self)
-        self.setItemDelegate(self._delegate)
-
         # Must set before flush all
         self.setColumnCount(len(self.Headers))
 
         # Flush all data to table
         self.flushAll()
 
         # Install custom header
@@ -147,35 +143,41 @@
     def deleteSelectedItem(self):
         indexes = self.selectedIndex
 
         if len(indexes) == 0:
             # Nothing to do
             return
 
+        def handleResultCode(_indexes, code):
+            if code == PySide6LegacyEnumValueWrapper(AppQMessageBox.StandardButton.Yes):
+                for i in range(len(_indexes)):
+                    deleteIndex = _indexes[i] - i
+                    deleteUnique = list(AS_UserSubscription().keys())[deleteIndex]
+
+                    self.removeRow(deleteIndex)
+
+                    AS_UserSubscription().pop(deleteUnique)
+
+                    if callable(self.deleteUniqueCallback):
+                        self.deleteUniqueCallback(deleteUnique)
+            else:
+                # Do not delete
+                pass
+
         mbox = QuestionDeleteMBox(icon=AppQMessageBox.Icon.Question)
         mbox.isMulti = bool(len(indexes) > 1)
         mbox.possibleRemark = self.item(indexes[0], 0).text()
         mbox.setText(mbox.customText())
+        mbox.finished.connect(functools.partial(handleResultCode, indexes))
 
-        if mbox.exec() == PySide6LegacyEnumValueWrapper(
-            AppQMessageBox.StandardButton.No
-        ):
-            # Do not delete
-            return
-
-        for i in range(len(indexes)):
-            deleteIndex = indexes[i] - i
-            deleteUnique = list(AS_UserSubscription().keys())[deleteIndex]
-
-            self.removeRow(deleteIndex)
-
-            AS_UserSubscription().pop(deleteUnique)
+        # dummy ref
+        setattr(self, '_questionDeleteMBox', mbox)
 
-            if callable(self.deleteUniqueCallback):
-                self.deleteUniqueCallback(deleteUnique)
+        # Show the MessageBox asynchronously
+        mbox.open()
 
     def flushItem(self, row, column, item):
         header = self.Headers[column]
 
         oldItem = self.item(row, column)
         newItem = QTableWidgetItem(header(item))
```

### Comparing `Furious-GUI-0.3.9/Furious/Widget/XrayAssetViewerQListWidget.py` & `Furious-GUI-0.4.0/Furious/Widget/XrayAssetViewerQListWidget.py`

 * *Files 20% similar despite different names*

```diff
@@ -128,75 +128,95 @@
 
             # Ubuntu 20.04. Flush by initial theme(Ubuntu 20.04 theme changes bug)
             self.flushItemByTheme(self.initialTheme)
         else:
             self.flushItemByTheme(darkdetect.theme())
 
     def appendNewItem(self, filename: str):
+        def append(_filename):
+            try:
+                shutil.copy(_filename, XRAY_ASSET_DIR)
+            except shutil.SameFileError:
+                # Same file imported. Do nothing
+                pass
+            except Exception as ex:
+                # Any non-exit exception
+
+                _mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Critical)
+                _mbox.setWindowTitle(_('Import'))
+                _mbox.setText(_('Error import asset file'))
+                _mbox.setInformativeText(str(ex))
+
+                # Show the MessageBox asynchronously
+                _mbox.open()
+            else:
+                self.flushItem()
+
+                _mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Information)
+                _mbox.setWindowTitle(_('Import'))
+                _mbox.setText(_('Import asset file success'))
+
+                # Show the MessageBox asynchronously
+                _mbox.open()
+
         basename = os.path.basename(filename)
 
         if os.path.isfile(XRAY_ASSET_DIR / basename):
+
+            def handleResultCode(_filename, code):
+                if code == PySide6LegacyEnumValueWrapper(
+                    AppQMessageBox.StandardButton.Yes
+                ):
+                    append(_filename)
+                else:
+                    # Do not overwrite
+                    pass
+
             mbox = AssetExistsMBox(icon=AppQMessageBox.Icon.Question)
             mbox.setWindowTitle(_('Import'))
             mbox.setText(_('Asset file already exists. Overwrite?'))
             mbox.setInformativeText(basename)
+            mbox.finished.connect(functools.partial(handleResultCode, filename))
 
-            if mbox.exec() == PySide6LegacyEnumValueWrapper(
-                AppQMessageBox.StandardButton.No
-            ):
-                # Do not overwrite
-                return
-
-        try:
-            shutil.copy(filename, XRAY_ASSET_DIR)
-        except shutil.SameFileError:
-            # Same file imported. Do nothing
-            pass
-        except Exception as ex:
-            # Any non-exit exception
-
-            mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Critical)
-            mbox.setWindowTitle(_('Import'))
-            mbox.setText(_('Error import asset file'))
-            mbox.setInformativeText(str(ex))
+            # dummy ref
+            setattr(self, '_assetExistsMBox', mbox)
 
-            # Show the MessageBox and wait for user to close it
-            mbox.exec()
+            # Show the MessageBox asynchronously
+            mbox.open()
         else:
-            self.flushItem()
-
-            mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Information)
-            mbox.setWindowTitle(_('Import'))
-            mbox.setText(_('Import asset file success'))
-
-            # Show the MessageBox and wait for user to close it
-            mbox.exec()
+            append(filename)
 
     def deleteSelectedItem(self):
         indexes = self.selectedIndex
 
         if len(indexes) == 0:
             # Nothing selected
             return
 
+        def handleResultCode(_indexes, code):
+            if code == PySide6LegacyEnumValueWrapper(AppQMessageBox.StandardButton.Yes):
+                for index in _indexes:
+                    os.remove(XRAY_ASSET_DIR / self.item(index).text())
+
+                self.flushItem()
+            else:
+                # Do not delete
+                pass
+
         mbox = QuestionDeleteMBox(icon=AppQMessageBox.Icon.Question)
         mbox.isMulti = bool(len(indexes) > 1)
         mbox.possibleRemark = f'{self.item(indexes[0]).text()}'
         mbox.setText(mbox.customText())
+        mbox.finished.connect(functools.partial(handleResultCode, indexes))
 
-        if mbox.exec() == PySide6LegacyEnumValueWrapper(
-            AppQMessageBox.StandardButton.No
-        ):
-            # Do not delete
-            return
-
-        for index in indexes:
-            os.remove(XRAY_ASSET_DIR / self.item(index).text())
+        # dummy ref
+        setattr(self, '_questionDeleteMBox', mbox)
 
-        self.flushItem()
+        # Show the MessageBox asynchronously
+        mbox.open()
 
     def keyPressEvent(self, event):
         if event.key() == QtCore.Qt.Key.Key_Delete:
             self.deleteSelectedItem()
         else:
             super().keyPressEvent(event)
```

### Comparing `Furious-GUI-0.3.9/Furious/Widget/__init__.py` & `Furious-GUI-0.4.0/Furious/Widget/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,12 +13,18 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from .Application import *
 from .ConnectProgressBar import *
+from .GuiHysteria1 import *
+from .GuiHysteria2 import *
+from .GuiShadowsocks import *
+from .GuiTrojan import *
+from .GuiVLESS import *
+from .GuiVMess import *
 from .IndentSpinBox import *
 from .SystemTrayIcon import *
 from .UserServersQTableWidget import *
 from .UserSubsQTableWidget import *
 from .XrayAssetViewerQListWidget import *
```

### Comparing `Furious-GUI-0.3.9/Furious/Window/AppMainWindow.py` & `Furious-GUI-0.4.0/Furious/Window/AppMainWindow.py`

 * *Files 14% similar despite different names*

```diff
@@ -126,23 +126,29 @@
             parent.resetNetworkState()
 
         self.stopTest()
 
 
 needTrans(
     'Server',
-    'Log',
-    'Show Furious Log',
-    'Show Core Log',
-    'Show Tun2socks Log',
+    'Add VMess Server...',
+    'Add VLESS Server...',
+    'Add Shadowsocks Server...',
+    'Add Trojan Server...',
+    'Add Hysteria1 Server...',
+    'Add Hysteria2 Server...',
     'Subscription',
     'Update Subscription (Use Current Proxy)',
     'Update Subscription (Force Proxy)',
     'Update Subscription (No Proxy)',
     'Edit Subscription...',
+    'Log',
+    'Show Furious Log',
+    'Show Core Log',
+    'Show Tun2socks Log',
     'Tools',
     'Manage Xray-core Asset File...',
     'Check For Updates',
     'About',
     'Help',
 )
 
@@ -197,14 +203,54 @@
                     QtCore.Qt.KeyboardModifier.ControlModifier
                     | QtCore.Qt.KeyboardModifier.ShiftModifier,
                     QtCore.Qt.Key.Key_T,
                 ),
             ),
         ]
 
+        serverActions = [
+            AppQAction(
+                _('Add VMess Server...'),
+                callback=lambda: self.userServersQTableWidget.addServerViaGui(
+                    Protocol.VMess, _('Add VMess Server...')
+                ),
+            ),
+            AppQAction(
+                _('Add VLESS Server...'),
+                callback=lambda: self.userServersQTableWidget.addServerViaGui(
+                    Protocol.VLESS, _('Add VLESS Server...')
+                ),
+            ),
+            AppQAction(
+                _('Add Shadowsocks Server...'),
+                callback=lambda: self.userServersQTableWidget.addServerViaGui(
+                    Protocol.Shadowsocks, _('Add Shadowsocks Server...')
+                ),
+            ),
+            AppQAction(
+                _('Add Trojan Server...'),
+                callback=lambda: self.userServersQTableWidget.addServerViaGui(
+                    Protocol.Trojan, _('Add Trojan Server...')
+                ),
+            ),
+            AppQSeperator(),
+            AppQAction(
+                _('Add Hysteria1 Server...'),
+                callback=lambda: self.userServersQTableWidget.addServerViaGui(
+                    Protocol.Hysteria1, _('Add Hysteria1 Server...')
+                ),
+            ),
+            AppQAction(
+                _('Add Hysteria2 Server...'),
+                callback=lambda: self.userServersQTableWidget.addServerViaGui(
+                    Protocol.Hysteria2, _('Add Hysteria2 Server...')
+                ),
+            ),
+        ]
+
         subsActions = [
             AppQAction(
                 _('Update Subscription (Use Current Proxy)'),
                 callback=lambda: self.userServersQTableWidget.updateSubs(
                     connectedHttpProxyEndpoint()
                 ),
             ),
@@ -240,14 +286,22 @@
                     icon=bootstrapIcon('pin-angle.svg'),
                     menu=AppQMenu(*logActions),
                     useActionGroup=False,
                     checkable=False,
                 ),
                 AppQSeperator(),
                 AppQAction(
+                    _('Server'),
+                    icon=bootstrapIcon('database.svg'),
+                    menu=AppQMenu(*serverActions),
+                    useActionGroup=False,
+                    checkable=False,
+                ),
+                AppQSeperator(),
+                AppQAction(
                     _('Subscription'),
                     icon=bootstrapIcon('collection.svg'),
                     menu=AppQMenu(*subsActions),
                     useActionGroup=False,
                     checkable=False,
                 ),
                 AppQSeperator(),
@@ -281,14 +335,19 @@
         else:
             # Menu actions
             logMenu = {
                 'name': 'Log',
                 'actions': [*logActions],
             }
 
+            serverMenu = {
+                'name': 'Server',
+                'actions': [*serverActions],
+            }
+
             subsMenu = {
                 'name': 'Subscription',
                 'actions': [*subsActions],
             }
 
             toolsMenu = {
                 'name': 'Tools',
@@ -311,15 +370,15 @@
                         checkable=False,
                         callback=lambda: self.openAboutPage(),
                     ),
                 ],
             }
 
             # Menus
-            for menuDict in (logMenu, subsMenu, toolsMenu, helpMenu):
+            for menuDict in (logMenu, serverMenu, subsMenu, toolsMenu, helpMenu):
                 menuName = menuDict['name']
                 menuObjName = f'_{menuName}Menu'
                 menu = AppQMenu(
                     *menuDict['actions'], title=_(menuName), parent=self.menuBar()
                 )
 
                 # Set reference
```

### Comparing `Furious-GUI-0.3.9/Furious/Window/LogViewerWindow.py` & `Furious-GUI-0.4.0/Furious/Window/LogViewerWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
             # Any non-exit exceptions
 
             mbox = SaveErrorMBox(icon=AppQMessageBox.Icon.Critical)
             mbox.saveError = str(ex)
             mbox.setWindowTitle(_('Error saving log'))
             mbox.setText(mbox.customText())
 
-            # Show the MessageBox and wait for user to close it
-            mbox.exec()
+            # Show the MessageBox asynchronously
+            mbox.open()
 
 
 needTrans(
     'Log Viewer',
     'Save As...',
     'Exit',
     'File',
```

### Comparing `Furious-GUI-0.3.9/Furious/Window/QRCodeWindow.py` & `Furious-GUI-0.4.0/Furious/Window/QRCodeWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Window/TextEditorWindow.py` & `Furious-GUI-0.4.0/Furious/Window/TextEditorWindow.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,17 +112,15 @@
 
 class TextEditorWindow(AppQMainWindow):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.customWindowTitle = ''
         self.setWindowModality(QtCore.Qt.WindowModality.ApplicationModal)
-        self.setFixedSize(470, int(470 * GOLDEN_RATIO))
-
-        self.indentSpinBox = IndentSpinBox(parent=self)
+        self.setFixedSize(450, int(450 * GOLDEN_RATIO))
 
         # Current editing index
         self.currentIndex = -1
 
         self.modified = False
         self.modifiedMark = ' *'
 
@@ -266,32 +264,40 @@
 
     def markAsSaved(self):
         self.modified = False
         self.setWindowTitle(self.customWindowTitle)
 
     def questionSave(self):
         if self.modified:
-            mbox = QuestionSaveMBox(icon=AppQMessageBox.Icon.Question)
-            code = mbox.exec()
 
-            if code == PySide6LegacyEnumValueWrapper(
-                AppQMessageBox.ButtonRole.AcceptRole
-            ):
-                if self.save():
+            def handleResultCode(code):
+                if code == PySide6LegacyEnumValueWrapper(
+                    AppQMessageBox.ButtonRole.AcceptRole
+                ):
+                    if self.save():
+                        self.hide()
+                if code == PySide6LegacyEnumValueWrapper(
+                    AppQMessageBox.ButtonRole.DestructiveRole
+                ):
+                    self.markAsSaved()
                     self.hide()
-            if code == PySide6LegacyEnumValueWrapper(
-                AppQMessageBox.ButtonRole.DestructiveRole
-            ):
-                self.markAsSaved()
-                self.hide()
-            if code == PySide6LegacyEnumValueWrapper(
-                AppQMessageBox.ButtonRole.RejectRole
-            ):
-                # Cancel. Do nothing
-                pass
+                if code == PySide6LegacyEnumValueWrapper(
+                    AppQMessageBox.ButtonRole.RejectRole
+                ):
+                    # Cancel. Do nothing
+                    pass
+
+            mbox = QuestionSaveMBox(icon=AppQMessageBox.Icon.Question)
+            mbox.finished.connect(functools.partial(handleResultCode))
+
+            # dummy ref
+            setattr(self, '_questionSaveMBox', mbox)
+
+            # Show the MessageBox asynchronously
+            mbox.open()
         else:
             self.hide()
 
     def setPlainText(self, text: str, blockSignals: bool):
         if blockSignals:
             with QBlockSignals(self.jsonEditor):
                 self.jsonEditor.setPlainText(text)
@@ -315,16 +321,16 @@
             # Any non-exit exceptions
 
             mbox = JSONDecodeErrorMBox(icon=AppQMessageBox.Icon.Critical)
             mbox.error = str(ex)
             mbox.setWindowTitle(_('Error saving configuration'))
             mbox.setText(mbox.customText())
 
-            # Show the MessageBox and wait for user to close it
-            mbox.exec()
+            # Show the MessageBox asynchronously
+            mbox.open()
 
             return False
         else:
             old = AS_UserServers()[index]
             new = constructFromDict(jsonObject, **old.kwargs)
 
             FastItemDeletionSearch.moveToTrash(old)
@@ -338,15 +344,17 @@
 
                 pass
 
             if index == AS_UserActivatedItemIndex():
                 try:
                     if APP().isSystemTrayConnected():
                         mbox = NewChangesNextTimeMBox()
-                        mbox.exec()
+
+                        # Show the MessageBox asynchronously
+                        mbox.open()
                 except Exception:
                     # Any non-exit exceptions
 
                     pass
 
             self.markAsSaved()
 
@@ -365,42 +373,52 @@
                 # Any non-exit exceptions
 
                 mbox = AppQMessageBox(icon=AppQMessageBox.Icon.Critical)
                 mbox.setWindowTitle(_('Error Saving File'))
                 mbox.setText(_('Invalid server configuration'))
                 mbox.setInformativeText(str(ex))
 
-                # Show the MessageBox and wait for user to close it
-                mbox.exec()
+                # Show the MessageBox asynchronously
+                mbox.open()
 
     def setIndent(self):
-        code = self.indentSpinBox.exec()
-
-        if code == PySide6LegacyEnumValueWrapper(AppQDialog.DialogCode.Accepted):
-            plain = self.jsonEditor.toPlainText()
+        def handleResultCode(_indentSpinBox, code):
+            if code == PySide6LegacyEnumValueWrapper(AppQDialog.DialogCode.Accepted):
+                plain = self.jsonEditor.toPlainText()
 
-            try:
-                jsonObject = JSONEncoder.decode(plain)
-            except Exception as ex:
-                # Any non-exit exceptions
+                try:
+                    jsonObject = JSONEncoder.decode(plain)
+                except Exception as ex:
+                    # Any non-exit exceptions
 
-                mbox = JSONDecodeErrorMBox(icon=AppQMessageBox.Icon.Critical)
-                mbox.error = str(ex)
-                mbox.setWindowTitle(_('Error setting indent'))
-                mbox.setText(mbox.customText())
+                    mbox = JSONDecodeErrorMBox(icon=AppQMessageBox.Icon.Critical)
+                    mbox.error = str(ex)
+                    mbox.setWindowTitle(_('Error setting indent'))
+                    mbox.setText(mbox.customText())
+
+                    # Show the MessageBox asynchronously
+                    mbox.open()
+                else:
+                    text = JSONEncoder.encode(jsonObject, indent=_indentSpinBox.value())
 
-                # Show the MessageBox and wait for user to close it
-                mbox.exec()
+                    self.setPlainText(text, False)
             else:
-                text = JSONEncoder.encode(jsonObject, indent=self.indentSpinBox.value())
+                # Do nothing
+                pass
 
-                self.setPlainText(text, False)
-        else:
-            # Do nothing
-            pass
+        indentSpinBox = IndentSpinBox(parent=self)
+        indentSpinBox.finished.connect(
+            functools.partial(handleResultCode, indentSpinBox)
+        )
+
+        # dummy ref
+        setattr(self, '_IndentSpinBox', indentSpinBox)
+
+        # Show the MessageBox asynchronously
+        indentSpinBox.open()
 
     def showTabAndSpaces(self):
         textOption = QTextOption()
         textOption.setFlags(QTextOption.Flag.ShowTabsAndSpaces)
 
         self.jsonEditor.document().setDefaultTextOption(textOption)
         # Reset. Set
```

### Comparing `Furious-GUI-0.3.9/Furious/Window/UserSubsWindow.py` & `Furious-GUI-0.4.0/Furious/Window/UserSubsWindow.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,23 +45,25 @@
 
 class AddSubsDialog(AppQDialog):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.setWindowTitle(_('Add Subscription'))
 
-        self.remarkText = QLabel(_('Enter subscription remark:'))
+        self.remarkText = AppQLabel(_('Enter subscription remark:'))
         self.remarkEdit = QLineEdit()
 
-        self.webURLText = QLabel(_('Enter subscription URL:'))
+        self.webURLText = AppQLabel(_('Enter subscription URL:'))
         self.webURLEdit = QLineEdit()
 
-        self.dialogBtns = QDialogButtonBox(QtCore.Qt.Orientation.Horizontal)
-        self.dialogBtns.addButton(_('OK'), QDialogButtonBox.ButtonRole.AcceptRole)
-        self.dialogBtns.addButton(_('Cancel'), QDialogButtonBox.ButtonRole.RejectRole)
+        self.dialogBtns = AppQDialogButtonBox(QtCore.Qt.Orientation.Horizontal)
+        self.dialogBtns.addButton(_('OK'), AppQDialogButtonBox.ButtonRole.AcceptRole)
+        self.dialogBtns.addButton(
+            _('Cancel'), AppQDialogButtonBox.ButtonRole.RejectRole
+        )
         self.dialogBtns.accepted.connect(self.accept)
         self.dialogBtns.rejected.connect(self.reject)
 
         layout = QFormLayout()
         layout.addRow(self.remarkText)
         layout.addRow(self.remarkEdit)
         layout.addRow(self.webURLText)
@@ -76,25 +78,14 @@
 
     def subsRemark(self):
         return self.remarkEdit.text()
 
     def subsWebURL(self):
         return self.webURLEdit.text()
 
-    def retranslate(self):
-        self.setWindowTitle(_(self.windowTitle()))
-
-        self.remarkText.setText(_(self.remarkText.text()))
-        self.webURLText.setText(_(self.webURLText.text()))
-
-        for button in self.dialogBtns.buttons():
-            button.setText(_(button.text()))
-
-        moveToCenter(self)
-
 
 needTrans(
     'Edit Subscription',
     'Subscription List',
     'Add',
     'Delete',
 )
@@ -102,17 +93,17 @@
 
 class UserSubsWindow(AppQMainWindow):
     def __init__(self, *args, **kwargs):
         callback = kwargs.pop('deleteUniqueCallback', None)
 
         super().__init__(*args, **kwargs)
 
+        self.setWindowModality(QtCore.Qt.WindowModality.WindowModal)
         self.setWindowTitle(_('Edit Subscription'))
 
-        self.addSubsDialog = AddSubsDialog()
         self.userSubsQTableWidget = UserSubsQTableWidget(deleteUniqueCallback=callback)
 
         self.userSubsTab = AppQTabWidget(self)
         self.userSubsTab.addTab(self.userSubsQTableWidget, _('Subscription List'))
 
         # Buttons
         self.addButton = AppQPushButton(_('Add'))
@@ -140,30 +131,40 @@
             self.setGeometry(100, 100, *list(int(size) for size in windowSize))
         except Exception:
             # Any non-exit exceptions
 
             self.setGeometry(100, 100, 360 * GOLDEN_RATIO, 360)
 
     def addSubs(self):
-        choice = self.addSubsDialog.exec()
+        def handleResultCode(_addSubsDialog, code):
+            if code == PySide6LegacyEnumValueWrapper(AppQDialog.DialogCode.Accepted):
+                remark = _addSubsDialog.subsRemark()
+                webURL = _addSubsDialog.subsWebURL()
+
+                if remark:
+                    # Unique id. Used by display and deletion
+                    unique = str(uuid.uuid4())
+
+                    self.userSubsQTableWidget.appendNewItem(
+                        unique=unique, remark=remark, webURL=webURL
+                    )
+            else:
+                # Do nothing
+                pass
+
+        addSubsDialog = AddSubsDialog(parent=self)
+        addSubsDialog.finished.connect(
+            functools.partial(handleResultCode, addSubsDialog)
+        )
+
+        # dummy ref
+        setattr(self, '_addSubsDialog', addSubsDialog)
 
-        if choice == PySide6LegacyEnumValueWrapper(QDialog.DialogCode.Accepted):
-            remark = self.addSubsDialog.subsRemark()
-            webURL = self.addSubsDialog.subsWebURL()
-
-            if remark:
-                # Unique id. Used by display and deletion
-                unique = str(uuid.uuid4())
-
-                self.userSubsQTableWidget.appendNewItem(
-                    unique=unique, remark=remark, webURL=webURL
-                )
-        else:
-            # Do nothing
-            pass
+        # Show the MessageBox asynchronously
+        addSubsDialog.open()
 
     def deleteSelectedItem(self):
         self.userSubsQTableWidget.deleteSelectedItem()
 
     def keyPressEvent(self, event):
         if event.key() == QtCore.Qt.Key.Key_Delete:
             self.deleteSelectedItem()
```

### Comparing `Furious-GUI-0.3.9/Furious/Window/XrayAssetViewerWindow.py` & `Furious-GUI-0.4.0/Furious/Window/XrayAssetViewerWindow.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/Window/__init__.py` & `Furious-GUI-0.4.0/Furious/Window/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/__init__.py` & `Furious-GUI-0.4.0/Furious/__init__.py`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/Furious/__main__.py` & `Furious-GUI-0.4.0/Furious/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                                 ),
                                 os.uname(),
                             )
                         )
                     )
                 )
 
-            # Show the AppQMessageBox and wait for user to close it
+            # Show the MessageBox and wait for user to close it
             messageBox.exec()
         else:
             if exitcode == ApplicationFactory.ExitCode.AssertionError:
                 # Assertion error
                 text = _(
                     f'{APPLICATION_NAME} encountered an internal error and needs to be stopped'
                 )
@@ -119,18 +119,16 @@
                     _('Crash log has been saved to') + f' {crashLogFile}'
                 )
                 messageBox.addButton(
                     _('Open crash log'), AppQMessageBox.ButtonRole.AcceptRole
                 )
                 messageBox.addButton(_('OK'), AppQMessageBox.ButtonRole.RejectRole)
 
-                # Show the AppQMessageBox and wait for user to close it
-                choice = messageBox.exec()
-
-                if choice == PySide6LegacyEnumValueWrapper(
+                # Show the MessageBox and wait for user to close it
+                if messageBox.exec() == PySide6LegacyEnumValueWrapper(
                     AppQMessageBox.ButtonRole.AcceptRole
                 ):
                     # Open
                     if QDesktopServices.openUrl(
                         QtCore.QUrl.fromLocalFile(crashLogFile)
                     ):
                         logger.info(f'open crash log {crashLogFile} success')
@@ -138,15 +136,15 @@
                         logger.error(f'open crash log {crashLogFile} failed')
                 else:
                     # OK. Do nothing
                     pass
             else:
                 # Crash log not saved
 
-                # Show the AppQMessageBox and wait for user to close it
+                # Show the MessageBox and wait for user to close it
                 messageBox.exec()
 
         sys.exit(exitcode)
     except Exception:
         # Any non-exit exceptions
 
         traceback.print_exc()
```

### Comparing `Furious-GUI-0.3.9/Furious_GUI.egg-info/PKG-INFO` & `Furious-GUI-0.4.0/Furious_GUI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.3.9
+Version: 0.4.0
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.3.9/Furious_GUI.egg-info/SOURCES.txt` & `Furious-GUI-0.4.0/Furious_GUI.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -20,29 +20,32 @@
 Furious/Data/xray/iran.dat
 Furious/Externals/GenTranslation.py
 Furious/Externals/__init__.py
 Furious/Interface/Application.py
 Furious/Interface/ConfigurationFactory.py
 Furious/Interface/CoreFactory.py
 Furious/Interface/Encoder.py
+Furious/Interface/GuiEditorItemFactory.py
 Furious/Interface/ItemUpdateProtocol.py
 Furious/Interface/Storage.py
 Furious/Interface/UserServersTableItem.py
 Furious/Interface/__init__.py
 Furious/Library/Configuration.py
+Furious/Library/EmptyFactoryHelper.py
 Furious/Library/Encoder.py
 Furious/Library/Tcping.py
 Furious/Library/__init__.py
 Furious/PyFramework/Ancestors.py
 Furious/PyFramework/__init__.py
 Furious/QtFramework/Ancestors.py
 Furious/QtFramework/CoreProcess.py
 Furious/QtFramework/DNSResolver.py
 Furious/QtFramework/DynamicTheme.py
 Furious/QtFramework/DynamicTranslate.py
+Furious/QtFramework/GuiEditorXXX.py
 Furious/QtFramework/NetworkStateManager.py
 Furious/QtFramework/QtGui.py
 Furious/QtFramework/QtNetwork.py
 Furious/QtFramework/QtWidgets.py
 Furious/QtFramework/TextEditor.py
 Furious/QtFramework/TextEditorTheme.py
 Furious/QtFramework/UpdatesManager.py
@@ -69,14 +72,22 @@
 Furious/Utility/SystemProxy.py
 Furious/Utility/SystemRoutingTable.py
 Furious/Utility/SystemRuntime.py
 Furious/Utility/Utility.py
 Furious/Utility/__init__.py
 Furious/Widget/Application.py
 Furious/Widget/ConnectProgressBar.py
+Furious/Widget/GuiHysteria1.py
+Furious/Widget/GuiHysteria2.py
+Furious/Widget/GuiShadowsocks.py
+Furious/Widget/GuiTrojan.py
+Furious/Widget/GuiVLESS.py
+Furious/Widget/GuiVMess.py
+Furious/Widget/GuiVTLS.py
+Furious/Widget/GuiVTransport.py
 Furious/Widget/IndentSpinBox.py
 Furious/Widget/SystemTrayIcon.py
 Furious/Widget/UserServersQTableWidget.py
 Furious/Widget/UserSubsQTableWidget.py
 Furious/Widget/XrayAssetViewerQListWidget.py
 Furious/Widget/__init__.py
 Furious/Window/AppMainWindow.py
```

### Comparing `Furious-GUI-0.3.9/LICENSE` & `Furious-GUI-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/PKG-INFO` & `Furious-GUI-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Furious-GUI
-Version: 0.3.9
+Version: 0.4.0
 Summary: A PySide6-based cross platform GUI client that launches your beloved GFW to outer space.
 Home-page: https://github.com/LorenEteval/Furious
 Author: Loren Eteval
 Author-email: loren.eteval@proton.me
 License: GPL v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `Furious-GUI-0.3.9/README.md` & `Furious-GUI-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Furious-GUI-0.3.9/setup.py` & `Furious-GUI-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,24 +48,25 @@
         'darkdetect[macos-listener]; platform_system == "Darwin"',
     ],
     extras_require={
         'go1.20': [
             'Xray-core < 1.8.5',
             'hysteria > 1.3.5',
             'hysteria2 == 2.0.0.1',
-            'tun2socks > 2.5.1; platform_system != "Linux"',
+            'tun2socks > 2.5.1, <= 2.5.2; platform_system != "Linux"',
         ],
         'go1.21': [
             'Xray-core >= 1.8.5, < 1.8.8',
             'hysteria2 >= 2.0.4',
-            'tun2socks > 2.5.1; platform_system != "Linux"',
+            'tun2socks > 2.5.1, <= 2.5.2; platform_system != "Linux"',
         ],
         'go1.22': [
             'Xray-core >= 1.8.8',
             'hysteria2 >= 2.0.4',
+            'tun2socks > 2.5.2; platform_system != "Linux"',
         ],
     },
     entry_points={
         'gui_scripts': [
             'Furious = Furious.__main__:main',
         ],
     },
```

