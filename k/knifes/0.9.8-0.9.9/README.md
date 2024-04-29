# Comparing `tmp/knifes-0.9.8.tar.gz` & `tmp/knifes-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knifes-0.9.8.tar", last modified: Tue Sep 19 03:13:21 2023, max compression
+gzip compressed data, was "knifes-0.9.9.tar", last modified: Tue Sep 19 03:39:00 2023, max compression
```

## Comparing `knifes-0.9.8.tar` & `knifes-0.9.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-09-19 03:13:21.532367 knifes-0.9.8/
--rw-r--r--   0 hwei       (501) staff       (20)      852 2023-09-19 03:13:21.532118 knifes-0.9.8/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.9.8/README.md
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-09-19 03:13:21.530689 knifes-0.9.8/knifes/
--rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.9.8/knifes/__init__.py
--rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.9.8/knifes/aes.py
--rw-r--r--   0 hwei       (501) staff       (20)      573 2023-07-29 07:38:53.000000 knifes-0.9.8/knifes/alarm.py
--rw-r--r--   0 hwei       (501) staff       (20)      624 2023-08-26 14:11:08.000000 knifes-0.9.8/knifes/constants.py
--rw-r--r--   0 hwei       (501) staff       (20)     7031 2023-08-28 06:02:17.000000 knifes-0.9.8/knifes/decorators.py
--rw-r--r--   0 hwei       (501) staff       (20)     8258 2023-09-19 03:09:05.000000 knifes-0.9.8/knifes/deploy.py
--rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.9.8/knifes/digests.py
--rw-r--r--   0 hwei       (501) staff       (20)      363 2023-02-01 04:12:33.000000 knifes-0.9.8/knifes/envconfig.py
--rw-r--r--   0 hwei       (501) staff       (20)     1722 2023-09-14 14:21:18.000000 knifes-0.9.8/knifes/file.py
--rw-r--r--   0 hwei       (501) staff       (20)     5108 2023-06-15 01:37:33.000000 knifes-0.9.8/knifes/getui.py
--rw-r--r--   0 hwei       (501) staff       (20)      884 2023-09-14 06:20:48.000000 knifes-0.9.8/knifes/i18n.py
--rw-r--r--   0 hwei       (501) staff       (20)     3002 2023-09-14 14:21:28.000000 knifes-0.9.8/knifes/jsons.py
--rw-r--r--   0 hwei       (501) staff       (20)      403 2023-07-29 07:38:53.000000 knifes-0.9.8/knifes/logging.py
--rw-r--r--   0 hwei       (501) staff       (20)     3194 2023-09-06 23:14:13.000000 knifes-0.9.8/knifes/luban.py
--rw-r--r--   0 hwei       (501) staff       (20)      474 2023-06-15 08:19:17.000000 knifes-0.9.8/knifes/media.py
--rw-r--r--   0 hwei       (501) staff       (20)      787 2023-08-26 07:57:47.000000 knifes-0.9.8/knifes/misc.py
--rw-r--r--   0 hwei       (501) staff       (20)      421 2023-08-04 10:48:49.000000 knifes-0.9.8/knifes/operators.py
--rw-r--r--   0 hwei       (501) staff       (20)      569 2022-11-23 13:58:35.000000 knifes-0.9.8/knifes/package.py
--rw-r--r--   0 hwei       (501) staff       (20)      872 2023-09-08 08:41:14.000000 knifes-0.9.8/knifes/paginator.py
--rw-r--r--   0 hwei       (501) staff       (20)      857 2023-08-26 07:58:46.000000 knifes-0.9.8/knifes/randoms.py
--rw-r--r--   0 hwei       (501) staff       (20)     1525 2023-08-26 08:02:46.000000 knifes-0.9.8/knifes/results.py
--rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.9.8/knifes/roar.py
--rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.9.8/knifes/shell.py
--rw-r--r--   0 hwei       (501) staff       (20)     2022 2023-07-31 14:57:01.000000 knifes-0.9.8/knifes/sms.py
--rw-r--r--   0 hwei       (501) staff       (20)     2547 2023-05-24 08:14:41.000000 knifes-0.9.8/knifes/status.py
--rw-r--r--   0 hwei       (501) staff       (20)      889 2023-02-01 04:20:34.000000 knifes-0.9.8/knifes/strings.py
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-09-19 03:13:21.531723 knifes-0.9.8/knifes/templatetags/
--rw-r--r--   0 hwei       (501) staff       (20)        0 2023-09-14 09:16:38.000000 knifes-0.9.8/knifes/templatetags/__init__.py
--rw-r--r--   0 hwei       (501) staff       (20)     1278 2023-09-14 23:48:17.000000 knifes-0.9.8/knifes/templatetags/locale.py
--rw-r--r--   0 hwei       (501) staff       (20)     1320 2023-08-26 08:00:10.000000 knifes-0.9.8/knifes/times.py
--rw-r--r--   0 hwei       (501) staff       (20)     3245 2023-06-15 07:38:41.000000 knifes-0.9.8/knifes/urls.py
--rw-r--r--   0 hwei       (501) staff       (20)     4396 2022-11-25 02:07:08.000000 knifes-0.9.8/knifes/useragent.py
-drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-09-19 03:13:21.531500 knifes-0.9.8/knifes.egg-info/
--rw-r--r--   0 hwei       (501) staff       (20)      852 2023-09-19 03:13:21.000000 knifes-0.9.8/knifes.egg-info/PKG-INFO
--rw-r--r--   0 hwei       (501) staff       (20)      741 2023-09-19 03:13:21.000000 knifes-0.9.8/knifes.egg-info/SOURCES.txt
--rw-r--r--   0 hwei       (501) staff       (20)        1 2023-09-19 03:13:21.000000 knifes-0.9.8/knifes.egg-info/dependency_links.txt
--rw-r--r--   0 hwei       (501) staff       (20)       42 2023-09-19 03:13:21.000000 knifes-0.9.8/knifes.egg-info/requires.txt
--rw-r--r--   0 hwei       (501) staff       (20)        7 2023-09-19 03:13:21.000000 knifes-0.9.8/knifes.egg-info/top_level.txt
--rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.9.8/pyproject.toml
--rw-r--r--   0 hwei       (501) staff       (20)       38 2023-09-19 03:13:21.532412 knifes-0.9.8/setup.cfg
--rw-r--r--   0 hwei       (501) staff       (20)     1064 2023-09-19 02:52:37.000000 knifes-0.9.8/setup.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-09-19 03:39:00.795445 knifes-0.9.9/
+-rw-r--r--   0 hwei       (501) staff       (20)      852 2023-09-19 03:39:00.795218 knifes-0.9.9/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      400 2022-09-02 05:25:28.000000 knifes-0.9.9/README.md
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-09-19 03:39:00.790164 knifes-0.9.9/knifes/
+-rw-r--r--   0 hwei       (501) staff       (20)        0 2022-01-21 03:14:54.000000 knifes-0.9.9/knifes/__init__.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1161 2022-02-16 14:49:04.000000 knifes-0.9.9/knifes/aes.py
+-rw-r--r--   0 hwei       (501) staff       (20)      573 2023-07-29 07:38:53.000000 knifes-0.9.9/knifes/alarm.py
+-rw-r--r--   0 hwei       (501) staff       (20)      624 2023-08-26 14:11:08.000000 knifes-0.9.9/knifes/constants.py
+-rw-r--r--   0 hwei       (501) staff       (20)     7031 2023-08-28 06:02:17.000000 knifes-0.9.9/knifes/decorators.py
+-rw-r--r--   0 hwei       (501) staff       (20)     8356 2023-09-19 03:38:13.000000 knifes-0.9.9/knifes/deploy.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1140 2022-10-14 05:30:31.000000 knifes-0.9.9/knifes/digests.py
+-rw-r--r--   0 hwei       (501) staff       (20)      363 2023-02-01 04:12:33.000000 knifes-0.9.9/knifes/envconfig.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1722 2023-09-14 14:21:18.000000 knifes-0.9.9/knifes/file.py
+-rw-r--r--   0 hwei       (501) staff       (20)     5108 2023-06-15 01:37:33.000000 knifes-0.9.9/knifes/getui.py
+-rw-r--r--   0 hwei       (501) staff       (20)      884 2023-09-14 06:20:48.000000 knifes-0.9.9/knifes/i18n.py
+-rw-r--r--   0 hwei       (501) staff       (20)     3002 2023-09-14 14:21:28.000000 knifes-0.9.9/knifes/jsons.py
+-rw-r--r--   0 hwei       (501) staff       (20)      403 2023-07-29 07:38:53.000000 knifes-0.9.9/knifes/logging.py
+-rw-r--r--   0 hwei       (501) staff       (20)     3194 2023-09-06 23:14:13.000000 knifes-0.9.9/knifes/luban.py
+-rw-r--r--   0 hwei       (501) staff       (20)      474 2023-06-15 08:19:17.000000 knifes-0.9.9/knifes/media.py
+-rw-r--r--   0 hwei       (501) staff       (20)      787 2023-08-26 07:57:47.000000 knifes-0.9.9/knifes/misc.py
+-rw-r--r--   0 hwei       (501) staff       (20)      421 2023-08-04 10:48:49.000000 knifes-0.9.9/knifes/operators.py
+-rw-r--r--   0 hwei       (501) staff       (20)      569 2022-11-23 13:58:35.000000 knifes-0.9.9/knifes/package.py
+-rw-r--r--   0 hwei       (501) staff       (20)      872 2023-09-08 08:41:14.000000 knifes-0.9.9/knifes/paginator.py
+-rw-r--r--   0 hwei       (501) staff       (20)      857 2023-08-26 07:58:46.000000 knifes-0.9.9/knifes/randoms.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1525 2023-08-26 08:02:46.000000 knifes-0.9.9/knifes/results.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2235 2022-05-30 13:46:32.000000 knifes-0.9.9/knifes/roar.py
+-rw-r--r--   0 hwei       (501) staff       (20)      446 2022-01-21 03:14:54.000000 knifes-0.9.9/knifes/shell.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2022 2023-07-31 14:57:01.000000 knifes-0.9.9/knifes/sms.py
+-rw-r--r--   0 hwei       (501) staff       (20)     2547 2023-05-24 08:14:41.000000 knifes-0.9.9/knifes/status.py
+-rw-r--r--   0 hwei       (501) staff       (20)      889 2023-02-01 04:20:34.000000 knifes-0.9.9/knifes/strings.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-09-19 03:39:00.794457 knifes-0.9.9/knifes/templatetags/
+-rw-r--r--   0 hwei       (501) staff       (20)        0 2023-09-14 09:16:38.000000 knifes-0.9.9/knifes/templatetags/__init__.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1278 2023-09-14 23:48:17.000000 knifes-0.9.9/knifes/templatetags/locale.py
+-rw-r--r--   0 hwei       (501) staff       (20)     1320 2023-08-26 08:00:10.000000 knifes-0.9.9/knifes/times.py
+-rw-r--r--   0 hwei       (501) staff       (20)     3245 2023-06-15 07:38:41.000000 knifes-0.9.9/knifes/urls.py
+-rw-r--r--   0 hwei       (501) staff       (20)     4396 2022-11-25 02:07:08.000000 knifes-0.9.9/knifes/useragent.py
+drwxr-xr-x   0 hwei       (501) staff       (20)        0 2023-09-19 03:39:00.791217 knifes-0.9.9/knifes.egg-info/
+-rw-r--r--   0 hwei       (501) staff       (20)      852 2023-09-19 03:39:00.000000 knifes-0.9.9/knifes.egg-info/PKG-INFO
+-rw-r--r--   0 hwei       (501) staff       (20)      741 2023-09-19 03:39:00.000000 knifes-0.9.9/knifes.egg-info/SOURCES.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        1 2023-09-19 03:39:00.000000 knifes-0.9.9/knifes.egg-info/dependency_links.txt
+-rw-r--r--   0 hwei       (501) staff       (20)       42 2023-09-19 03:39:00.000000 knifes-0.9.9/knifes.egg-info/requires.txt
+-rw-r--r--   0 hwei       (501) staff       (20)        7 2023-09-19 03:39:00.000000 knifes-0.9.9/knifes.egg-info/top_level.txt
+-rw-r--r--   0 hwei       (501) staff       (20)      103 2022-02-08 15:08:46.000000 knifes-0.9.9/pyproject.toml
+-rw-r--r--   0 hwei       (501) staff       (20)       38 2023-09-19 03:39:00.795485 knifes-0.9.9/setup.cfg
+-rw-r--r--   0 hwei       (501) staff       (20)     1064 2023-09-19 03:38:51.000000 knifes-0.9.9/setup.py
```

### Comparing `knifes-0.9.8/PKG-INFO` & `knifes-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knifes
-Version: 0.9.8
+Version: 0.9.9
 Summary: Swiss Army Knife
 Home-page: https://github.com/
 Author: knifes
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knifes-0.9.8/knifes/aes.py` & `knifes-0.9.9/knifes/aes.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/alarm.py` & `knifes-0.9.9/knifes/alarm.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/constants.py` & `knifes-0.9.9/knifes/constants.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/decorators.py` & `knifes-0.9.9/knifes/decorators.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/deploy.py` & `knifes-0.9.9/knifes/deploy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import sys
 import time
+from os import path
 from prompt_toolkit.shortcuts import button_dialog
 from datetime import datetime, timedelta
 from knifes.file import read_file
 from knifes.shell import *
 systemd_template = """[Unit]
 Description={Description}.gunicorn.service
 ConditionPathExists={ConditionPathExists}
@@ -65,16 +66,16 @@
 
 def celery(project_dir, log_dir, project_name, operate, is_beat=False):
     if operate not in ('restart', 'stop', 'start'):
         print_err('not supported operate, only supports [start | restart | stop]')
         return
 
     type_ = 'beat' if is_beat else 'worker'
-    pid_file = f'{log_dir}celery_{type_}.pid'
-    log_file = f'{log_dir}celery_{type_}{"" if is_beat else "%I"}.log'
+    pid_file = path.join(log_dir, f'celery_{type_}.pid')
+    log_file = path.join(log_dir, f'celery_{type_}{"" if is_beat else "%I"}.log')
 
     # stop
     if operate in ('restart', 'stop'):
         pid = read_file(pid_file).strip()
         if not pid:
             print_err(f'[celery]restart/stop {type_} failed，pid not exists:{pid_file}')
             return
@@ -216,21 +217,18 @@
     if not reload_datetime:
         print_err('重启失败！重启失败！重启失败！')
         return
 
     print_succ('重启成功:{}'.format(reload_datetime))
 
     # 重启定时任务进程
-    celery(project_dir, log_dir, project_name, 'restart', False)
+    if path.exists(path.join(log_dir, 'celery_worker.pid')):
+        celery(project_dir, log_dir, project_name, 'restart', False)
 
-    result = button_dialog(
-        title='restart celery beat',
-        text='Do you want to restart celery beat?',
-        buttons=[
-            ('No', False),
-            ('Yes', True),
-        ]).run()
-    if result:
+    if path.exists(path.join(log_dir, 'celery_beat.pid')) and \
+            button_dialog(title='restart celery beat', text='Do you want to restart celery beat?', buttons=[('No', False), ('Yes', True)]).run():
         celery(project_dir, log_dir, project_name, 'restart', True)
 
 
 
+
+
```

### Comparing `knifes-0.9.8/knifes/digests.py` & `knifes-0.9.9/knifes/digests.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/file.py` & `knifes-0.9.9/knifes/file.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/getui.py` & `knifes-0.9.9/knifes/getui.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/i18n.py` & `knifes-0.9.9/knifes/i18n.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/jsons.py` & `knifes-0.9.9/knifes/jsons.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/luban.py` & `knifes-0.9.9/knifes/luban.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/misc.py` & `knifes-0.9.9/knifes/misc.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/package.py` & `knifes-0.9.9/knifes/package.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/paginator.py` & `knifes-0.9.9/knifes/paginator.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/randoms.py` & `knifes-0.9.9/knifes/randoms.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/results.py` & `knifes-0.9.9/knifes/results.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/roar.py` & `knifes-0.9.9/knifes/roar.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/sms.py` & `knifes-0.9.9/knifes/sms.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/status.py` & `knifes-0.9.9/knifes/status.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/strings.py` & `knifes-0.9.9/knifes/strings.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/templatetags/locale.py` & `knifes-0.9.9/knifes/templatetags/locale.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/times.py` & `knifes-0.9.9/knifes/times.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/urls.py` & `knifes-0.9.9/knifes/urls.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes/useragent.py` & `knifes-0.9.9/knifes/useragent.py`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/knifes.egg-info/PKG-INFO` & `knifes-0.9.9/knifes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knifes
-Version: 0.9.8
+Version: 0.9.9
 Summary: Swiss Army Knife
 Home-page: https://github.com/
 Author: knifes
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knifes-0.9.8/knifes.egg-info/SOURCES.txt` & `knifes-0.9.9/knifes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `knifes-0.9.8/setup.py` & `knifes-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="knifes",
-    version="0.9.8",
+    version="0.9.9",
     author="knifes",
     author_email="author@example.com",
     description="Swiss Army Knife",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/",
     classifiers=[
```

