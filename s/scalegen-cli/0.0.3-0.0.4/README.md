# Comparing `tmp/scalegen-cli-0.0.3.tar.gz` & `tmp/scalegen-cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalegen-cli-0.0.3.tar", last modified: Thu Apr 25 11:39:02 2024, max compression
+gzip compressed data, was "scalegen-cli-0.0.4.tar", last modified: Mon Apr 29 10:36:46 2024, max compression
```

## Comparing `scalegen-cli-0.0.3.tar` & `scalegen-cli-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.416766 scalegen-cli-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 11:39:02.416766 scalegen-cli-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.408766 scalegen-cli-0.0.3/scalegen_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-25 11:39:02.000000 scalegen-cli-0.0.3/scalegen_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 11:39:02.416766 scalegen-cli-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/.git
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/api/
--rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/common/
--rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 11:39:02.412766 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/jc/
--rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/datamodels/jc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/datamodels/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/sg_finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)    25159 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/sg_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/visualisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-04-25 11:38:55.000000 scalegen-cli-0.0.3/st_cli/workstation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.014954 scalegen-cli-0.0.4/scalegen_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 10:36:46.000000 scalegen-cli-0.0.4/scalegen_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-29 10:36:46.000000 scalegen-cli-0.0.4/scalegen_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:36:46.000000 scalegen-cli-0.0.4/scalegen_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 10:36:46.000000 scalegen-cli-0.0.4/scalegen_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-29 10:36:46.000000 scalegen-cli-0.0.4/scalegen_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 10:36:46.000000 scalegen-cli-0.0.4/scalegen_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/st_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/st_cli/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/.git
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    13925 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:36:46.018954 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/jc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/datamodels/jc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/datamodels/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/sg_finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25159 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/sg_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-04-29 10:36:39.000000 scalegen-cli-0.0.4/st_cli/workstation.py
```

### Comparing `scalegen-cli-0.0.3/scalegen_cli.egg-info/SOURCES.txt` & `scalegen-cli-0.0.4/scalegen_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/setup.py` & `scalegen-cli-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/client.py` & `scalegen-cli-0.0.4/st_cli/client.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/datamodels/.gitignore` & `scalegen-cli-0.0.4/st_cli/datamodels/.gitignore`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/datamodels/datamodels/api/__init__.py` & `scalegen-cli-0.0.4/st_cli/datamodels/datamodels/api/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/datamodels/datamodels/cli/__init__.py` & `scalegen-cli-0.0.4/st_cli/datamodels/datamodels/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/datamodels/datamodels/common/__init__.py` & `scalegen-cli-0.0.4/st_cli/datamodels/datamodels/common/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/datamodels/datamodels/jc/__init__.py` & `scalegen-cli-0.0.4/st_cli/datamodels/datamodels/jc/__init__.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/job.py` & `scalegen-cli-0.0.4/st_cli/job.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/launch.py` & `scalegen-cli-0.0.4/st_cli/launch.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/list.py` & `scalegen-cli-0.0.4/st_cli/list.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/login.py` & `scalegen-cli-0.0.4/st_cli/login.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/main.py` & `scalegen-cli-0.0.4/st_cli/main.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/sg_finetune.py` & `scalegen-cli-0.0.4/st_cli/sg_finetune.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/sg_inference.py` & `scalegen-cli-0.0.4/st_cli/sg_inference.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/stop.py` & `scalegen-cli-0.0.4/st_cli/stop.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/utils.py` & `scalegen-cli-0.0.4/st_cli/utils.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/view.py` & `scalegen-cli-0.0.4/st_cli/view.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/visualisation.py` & `scalegen-cli-0.0.4/st_cli/visualisation.py`

 * *Files identical despite different names*

### Comparing `scalegen-cli-0.0.3/st_cli/workstation.py` & `scalegen-cli-0.0.4/st_cli/workstation.py`

 * *Files identical despite different names*

