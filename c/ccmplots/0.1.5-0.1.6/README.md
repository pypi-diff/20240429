# Comparing `tmp/ccmplots-0.1.5.tar.gz` & `tmp/ccmplots-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccmplots-0.1.5.tar", last modified: Thu Sep 21 13:23:33 2023, max compression
+gzip compressed data, was "ccmplots-0.1.6.tar", last modified: Mon Apr 29 18:01:07 2024, max compression
```

## Comparing `ccmplots-0.1.5.tar` & `ccmplots-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-09-21 13:23:33.113312 ccmplots-0.1.5/
--rw-rw-r--   0 torben    (1000) torben    (1000)       25 2023-05-27 11:41:16.000000 ccmplots-0.1.5/MANIFEST.in
--rw-r--r--   0 torben    (1000) torben    (1000)      134 2023-09-21 13:23:33.113312 ccmplots-0.1.5/PKG-INFO
--rw-rw-r--   0 torben    (1000) torben    (1000)     1728 2023-07-08 16:50:52.000000 ccmplots-0.1.5/README.md
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-09-21 13:23:33.113312 ccmplots-0.1.5/ccmplots/
--rw-rw-r--   0 torben    (1000) torben    (1000)      942 2023-05-27 10:34:26.000000 ccmplots-0.1.5/ccmplots/__init__.py
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-09-21 13:23:33.113312 ccmplots-0.1.5/ccmplots/styles/
--rw-rw-r--   0 torben    (1000) torben    (1000)     1280 2023-07-08 16:47:19.000000 ccmplots-0.1.5/ccmplots/styles/ccm.mplstyle
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-09-21 13:23:33.113312 ccmplots-0.1.5/ccmplots/styles/customization/
--rw-rw-r--   0 torben    (1000) torben    (1000)      159 2023-09-21 13:19:55.000000 ccmplots-0.1.5/ccmplots/styles/customization/a4.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)      120 2023-07-08 17:14:31.000000 ccmplots-0.1.5/ccmplots/styles/customization/bw_palette.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)       85 2023-05-29 09:37:45.000000 ccmplots-0.1.5/ccmplots/styles/customization/large_font.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)       39 2023-05-27 13:56:20.000000 ccmplots-0.1.5/ccmplots/styles/customization/no-latex.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)      429 2023-05-29 08:08:15.000000 ccmplots-0.1.5/ccmplots/styles/customization/sans.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)       91 2023-05-27 13:50:17.000000 ccmplots-0.1.5/ccmplots/styles/customization/square.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)      107 2023-05-29 08:41:08.000000 ccmplots-0.1.5/ccmplots/styles/customization/tum4c.mplstyle
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-09-21 13:23:33.113312 ccmplots-0.1.5/ccmplots.egg-info/
--rw-r--r--   0 torben    (1000) torben    (1000)      134 2023-09-21 13:23:33.000000 ccmplots-0.1.5/ccmplots.egg-info/PKG-INFO
--rw-rw-r--   0 torben    (1000) torben    (1000)      570 2023-09-21 13:23:33.000000 ccmplots-0.1.5/ccmplots.egg-info/SOURCES.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)        1 2023-09-21 13:23:33.000000 ccmplots-0.1.5/ccmplots.egg-info/dependency_links.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)       55 2023-09-21 13:23:33.000000 ccmplots-0.1.5/ccmplots.egg-info/requires.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)        9 2023-09-21 13:23:33.000000 ccmplots-0.1.5/ccmplots.egg-info/top_level.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)      225 2023-09-21 13:21:54.000000 ccmplots-0.1.5/pyproject.toml
--rw-rw-r--   0 torben    (1000) torben    (1000)       38 2023-09-21 13:23:33.113312 ccmplots-0.1.5/setup.cfg
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2024-04-29 18:01:07.533819 ccmplots-0.1.6/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       25 2023-05-27 11:41:16.000000 ccmplots-0.1.6/MANIFEST.in
+-rw-r--r--   0 torben    (1000) torben    (1000)      134 2024-04-29 18:01:07.533819 ccmplots-0.1.6/PKG-INFO
+-rw-rw-r--   0 torben    (1000) torben    (1000)     1728 2023-07-08 16:50:52.000000 ccmplots-0.1.6/README.md
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2024-04-29 18:01:07.529819 ccmplots-0.1.6/ccmplots/
+-rw-rw-r--   0 torben    (1000) torben    (1000)      942 2023-05-27 10:34:26.000000 ccmplots-0.1.6/ccmplots/__init__.py
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2024-04-29 18:01:07.533819 ccmplots-0.1.6/ccmplots/styles/
+-rw-rw-r--   0 torben    (1000) torben    (1000)     1280 2023-07-08 16:47:19.000000 ccmplots-0.1.6/ccmplots/styles/ccm.mplstyle
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2024-04-29 18:01:07.533819 ccmplots-0.1.6/ccmplots/styles/customization/
+-rw-rw-r--   0 torben    (1000) torben    (1000)      159 2023-09-21 13:19:55.000000 ccmplots-0.1.6/ccmplots/styles/customization/a4.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      120 2023-07-08 17:14:31.000000 ccmplots-0.1.6/ccmplots/styles/customization/bw_palette.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      716 2024-04-29 17:58:29.000000 ccmplots-0.1.6/ccmplots/styles/customization/daniel_style.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       85 2023-05-29 09:37:45.000000 ccmplots-0.1.6/ccmplots/styles/customization/large_font.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       39 2023-05-27 13:56:20.000000 ccmplots-0.1.6/ccmplots/styles/customization/no-latex.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      429 2023-05-29 08:08:15.000000 ccmplots-0.1.6/ccmplots/styles/customization/sans.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       91 2023-05-27 13:50:17.000000 ccmplots-0.1.6/ccmplots/styles/customization/square.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      107 2023-05-29 08:41:08.000000 ccmplots-0.1.6/ccmplots/styles/customization/tum4c.mplstyle
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2024-04-29 18:01:07.533819 ccmplots-0.1.6/ccmplots.egg-info/
+-rw-r--r--   0 torben    (1000) torben    (1000)      134 2024-04-29 18:01:07.000000 ccmplots-0.1.6/ccmplots.egg-info/PKG-INFO
+-rw-rw-r--   0 torben    (1000) torben    (1000)      622 2024-04-29 18:01:07.000000 ccmplots-0.1.6/ccmplots.egg-info/SOURCES.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)        1 2024-04-29 18:01:07.000000 ccmplots-0.1.6/ccmplots.egg-info/dependency_links.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)       55 2024-04-29 18:01:07.000000 ccmplots-0.1.6/ccmplots.egg-info/requires.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)        9 2024-04-29 18:01:07.000000 ccmplots-0.1.6/ccmplots.egg-info/top_level.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)      225 2024-04-29 17:58:54.000000 ccmplots-0.1.6/pyproject.toml
+-rw-rw-r--   0 torben    (1000) torben    (1000)       38 2024-04-29 18:01:07.533819 ccmplots-0.1.6/setup.cfg
```

### Comparing `ccmplots-0.1.5/README.md` & `ccmplots-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ccmplots-0.1.5/ccmplots/__init__.py` & `ccmplots-0.1.6/ccmplots/__init__.py`

 * *Files identical despite different names*

### Comparing `ccmplots-0.1.5/ccmplots/styles/ccm.mplstyle` & `ccmplots-0.1.6/ccmplots/styles/ccm.mplstyle`

 * *Files identical despite different names*

### Comparing `ccmplots-0.1.5/ccmplots.egg-info/SOURCES.txt` & `ccmplots-0.1.6/ccmplots.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -6,12 +6,13 @@
 ccmplots.egg-info/SOURCES.txt
 ccmplots.egg-info/dependency_links.txt
 ccmplots.egg-info/requires.txt
 ccmplots.egg-info/top_level.txt
 ccmplots/styles/ccm.mplstyle
 ccmplots/styles/customization/a4.mplstyle
 ccmplots/styles/customization/bw_palette.mplstyle
+ccmplots/styles/customization/daniel_style.mplstyle
 ccmplots/styles/customization/large_font.mplstyle
 ccmplots/styles/customization/no-latex.mplstyle
 ccmplots/styles/customization/sans.mplstyle
 ccmplots/styles/customization/square.mplstyle
 ccmplots/styles/customization/tum4c.mplstyle
```

