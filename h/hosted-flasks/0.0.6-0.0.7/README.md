# Comparing `tmp/hosted-flasks-0.0.6.tar.gz` & `tmp/hosted-flasks-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosted-flasks-0.0.6.tar", last modified: Sun Apr 28 16:32:55 2024, max compression
+gzip compressed data, was "hosted-flasks-0.0.7.tar", last modified: Mon Apr 29 17:52:03 2024, max compression
```

## Comparing `hosted-flasks-0.0.6.tar` & `hosted-flasks-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.197870 hosted-flasks-0.0.6/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.193987 hosted-flasks-0.0.6/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.6/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.6/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.6/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-28 16:32:55.197740 hosted-flasks-0.0.6/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.194184 hosted-flasks-0.0.6/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.6/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.6/docs/conf.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.194901 hosted-flasks-0.0.6/hosted_flasks/
--rw-r--r--   0 xtof       (501) staff       (20)      294 2024-04-28 16:32:18.000000 hosted-flasks-0.0.6/hosted_flasks/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      702 2024-04-28 11:59:41.000000 hosted-flasks-0.0.6/hosted_flasks/__main__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.195713 hosted-flasks-0.0.6/hosted_flasks/frontpage/
--rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/index.html
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.196774 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/
--rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/android-chrome-192x192.png
--rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/android-chrome-512x512.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/apple-touch-icon.png
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.197010 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/css/
--rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/css/default.css
--rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-28 14:20:24.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/css/style.css
--rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/favicon-16x16.png
--rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/favicon-32x32.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/favicon.ico
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.197219 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/img/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/img/.gitkeep
--rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/img/logo.svg
--rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/robots.txt
--rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage/static/site.webmanifest
--rw-r--r--   0 xtof       (501) staff       (20)      830 2024-04-28 14:20:16.000000 hosted-flasks-0.0.6/hosted_flasks/frontpage.py
--rw-r--r--   0 xtof       (501) staff       (20)     2923 2024-04-28 16:07:41.000000 hosted-flasks-0.0.6/hosted_flasks/loader.py
--rw-r--r--   0 xtof       (501) staff       (20)     1562 2024-04-28 16:28:30.000000 hosted-flasks-0.0.6/hosted_flasks/monkeypatch.py
--rw-r--r--   0 xtof       (501) staff       (20)     1164 2024-04-28 12:33:30.000000 hosted-flasks-0.0.6/hosted_flasks/server.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.195600 hosted-flasks-0.0.6/hosted_flasks.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-28 16:32:55.000000 hosted-flasks-0.0.6/hosted_flasks.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     1139 2024-04-28 16:32:55.000000 hosted-flasks-0.0.6/hosted_flasks.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-28 16:32:55.000000 hosted-flasks-0.0.6/hosted_flasks.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-28 16:32:55.000000 hosted-flasks-0.0.6/hosted_flasks.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       36 2024-04-28 16:32:55.000000 hosted-flasks-0.0.6/hosted_flasks.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-28 16:32:55.000000 hosted-flasks-0.0.6/hosted_flasks.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-28 16:32:55.197926 hosted-flasks-0.0.6/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1639 2024-04-28 10:59:13.000000 hosted-flasks-0.0.6/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-28 16:32:55.197558 hosted-flasks-0.0.6/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.6/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1029 2024-04-28 14:42:09.000000 hosted-flasks-0.0.6/tests/test_environ_get.py
--rw-r--r--   0 xtof       (501) staff       (20)     3250 2024-04-28 16:06:39.000000 hosted-flasks-0.0.6/tests/test_loader.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.209757 hosted-flasks-0.0.7/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.204166 hosted-flasks-0.0.7/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.7/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 17:52:03.209620 hosted-flasks-0.0.7/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.204392 hosted-flasks-0.0.7/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/docs/conf.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.205727 hosted-flasks-0.0.7/hosted_flasks/
+-rw-r--r--   0 xtof       (501) staff       (20)      294 2024-04-29 17:51:23.000000 hosted-flasks-0.0.7/hosted_flasks/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      702 2024-04-28 11:59:41.000000 hosted-flasks-0.0.7/hosted_flasks/__main__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.206672 hosted-flasks-0.0.7/hosted_flasks/frontpage/
+-rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/index.html
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.208230 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/
+-rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/android-chrome-192x192.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/android-chrome-512x512.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/apple-touch-icon.png
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.208510 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/
+-rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/default.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-28 14:20:24.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/style.css
+-rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon-16x16.png
+-rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon-32x32.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon.ico
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.208763 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/img/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/img/.gitkeep
+-rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/img/logo.svg
+-rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/robots.txt
+-rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/site.webmanifest
+-rw-r--r--   0 xtof       (501) staff       (20)      830 2024-04-28 14:20:16.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3024 2024-04-29 17:51:35.000000 hosted-flasks-0.0.7/hosted_flasks/loader.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2262 2024-04-29 17:37:21.000000 hosted-flasks-0.0.7/hosted_flasks/monkeypatch.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1164 2024-04-28 17:43:02.000000 hosted-flasks-0.0.7/hosted_flasks/server.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.206540 hosted-flasks-0.0.7/hosted_flasks.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     1139 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       36 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-29 17:52:03.209824 hosted-flasks-0.0.7/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1639 2024-04-28 10:59:13.000000 hosted-flasks-0.0.7/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.209267 hosted-flasks-0.0.7/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1029 2024-04-28 14:42:09.000000 hosted-flasks-0.0.7/tests/test_environ_get.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3250 2024-04-28 16:06:39.000000 hosted-flasks-0.0.7/tests/test_loader.py
```

### Comparing `hosted-flasks-0.0.6/.github/README.md` & `hosted-flasks-0.0.7/.github/README.md`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/LICENSE.txt` & `hosted-flasks-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/PKG-INFO` & `hosted-flasks-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.6
+Version: 0.0.7
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.6/docs/conf.py` & `hosted-flasks-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/__main__.py` & `hosted-flasks-0.0.7/hosted_flasks/__main__.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/index.html` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/index.html`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/android-chrome-192x192.png` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/android-chrome-512x512.png` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/apple-touch-icon.png` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/css/default.css` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/default.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/css/style.css` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/style.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/favicon-16x16.png` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/favicon-32x32.png` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/favicon.ico` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage/static/img/logo.svg` & `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/frontpage.py` & `hosted-flasks-0.0.7/hosted_flasks/frontpage.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks/loader.py` & `hosted-flasks-0.0.7/hosted_flasks/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,16 @@
       spec.loader.exec_module(mod)
       # extract the handler from the mod using the appname
       self.handler = getattr(mod, appname)
     except FileNotFoundError:
       logger.warning(f"😞 '{module_path}' doesn't provide '__init__.py'")
     except AttributeError:
       logger.warning(f"😞 '{module_path}' doesn't provide flask object: {self.app}")
+    except Exception as ex:
+      logger.warning(f"😞 '{module_path}' failed to load due to {ex}")
 
 def add_app(name, src, **kwargs):
   app = HostedFlask(name, src, **kwargs)
   logger.info(f"🌍 added {app.name}")
 
 def get_apps(config=None, force=False):
   global apps
```

### Comparing `hosted-flasks-0.0.6/hosted_flasks/server.py` & `hosted-flasks-0.0.7/hosted_flasks/server.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/hosted_flasks.egg-info/PKG-INFO` & `hosted-flasks-0.0.7/hosted_flasks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.6
+Version: 0.0.7
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.6/hosted_flasks.egg-info/SOURCES.txt` & `hosted-flasks-0.0.7/hosted_flasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/setup.py` & `hosted-flasks-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/tests/test_environ_get.py` & `hosted-flasks-0.0.7/tests/test_environ_get.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.6/tests/test_loader.py` & `hosted-flasks-0.0.7/tests/test_loader.py`

 * *Files identical despite different names*

