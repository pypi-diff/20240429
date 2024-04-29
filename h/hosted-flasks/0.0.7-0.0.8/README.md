# Comparing `tmp/hosted-flasks-0.0.7.tar.gz` & `tmp/hosted-flasks-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosted-flasks-0.0.7.tar", last modified: Mon Apr 29 17:52:03 2024, max compression
+gzip compressed data, was "hosted-flasks-0.0.8.tar", last modified: Mon Apr 29 19:41:37 2024, max compression
```

## Comparing `hosted-flasks-0.0.7.tar` & `hosted-flasks-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.209757 hosted-flasks-0.0.7/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.204166 hosted-flasks-0.0.7/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.7/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 17:52:03.209620 hosted-flasks-0.0.7/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.204392 hosted-flasks-0.0.7/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/docs/conf.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.205727 hosted-flasks-0.0.7/hosted_flasks/
--rw-r--r--   0 xtof       (501) staff       (20)      294 2024-04-29 17:51:23.000000 hosted-flasks-0.0.7/hosted_flasks/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)      702 2024-04-28 11:59:41.000000 hosted-flasks-0.0.7/hosted_flasks/__main__.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.206672 hosted-flasks-0.0.7/hosted_flasks/frontpage/
--rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/index.html
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.208230 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/
--rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/android-chrome-192x192.png
--rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/android-chrome-512x512.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/apple-touch-icon.png
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.208510 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/
--rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/default.css
--rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-28 14:20:24.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/style.css
--rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon-16x16.png
--rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon-32x32.png
--rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon.ico
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.208763 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/img/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/img/.gitkeep
--rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/img/logo.svg
--rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/robots.txt
--rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage/static/site.webmanifest
--rw-r--r--   0 xtof       (501) staff       (20)      830 2024-04-28 14:20:16.000000 hosted-flasks-0.0.7/hosted_flasks/frontpage.py
--rw-r--r--   0 xtof       (501) staff       (20)     3024 2024-04-29 17:51:35.000000 hosted-flasks-0.0.7/hosted_flasks/loader.py
--rw-r--r--   0 xtof       (501) staff       (20)     2262 2024-04-29 17:37:21.000000 hosted-flasks-0.0.7/hosted_flasks/monkeypatch.py
--rw-r--r--   0 xtof       (501) staff       (20)     1164 2024-04-28 17:43:02.000000 hosted-flasks-0.0.7/hosted_flasks/server.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.206540 hosted-flasks-0.0.7/hosted_flasks.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)     1139 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       36 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-29 17:52:03.000000 hosted-flasks-0.0.7/hosted_flasks.egg-info/top_level.txt
--rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-29 17:52:03.209824 hosted-flasks-0.0.7/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1639 2024-04-28 10:59:13.000000 hosted-flasks-0.0.7/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 17:52:03.209267 hosted-flasks-0.0.7/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.7/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1029 2024-04-28 14:42:09.000000 hosted-flasks-0.0.7/tests/test_environ_get.py
--rw-r--r--   0 xtof       (501) staff       (20)     3250 2024-04-28 16:06:39.000000 hosted-flasks-0.0.7/tests/test_loader.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.020411 hosted-flasks-0.0.8/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.016322 hosted-flasks-0.0.8/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     1033 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1057 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)      121 2024-04-27 13:30:32.000000 hosted-flasks-0.0.8/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 19:41:37.020279 hosted-flasks-0.0.8/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.016533 hosted-flasks-0.0.8/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1149 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/docs/conf.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.017288 hosted-flasks-0.0.8/hosted_flasks/
+-rw-r--r--   0 xtof       (501) staff       (20)      429 2024-04-29 19:38:18.000000 hosted-flasks-0.0.8/hosted_flasks/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)      702 2024-04-28 11:59:41.000000 hosted-flasks-0.0.8/hosted_flasks/__main__.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.018122 hosted-flasks-0.0.8/hosted_flasks/frontpage/
+-rw-r--r--   0 xtof       (501) staff       (20)     1462 2024-04-27 13:00:36.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/index.html
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.019221 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/
+-rw-rw-r--   0 xtof       (501) staff       (20)    17742 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/android-chrome-192x192.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    53448 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/android-chrome-512x512.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15929 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/apple-touch-icon.png
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.019514 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/
+-rw-r--r--   0 xtof       (501) staff       (20)     5011 2023-12-06 14:26:46.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/default.css
+-rw-r--r--   0 xtof       (501) staff       (20)     1216 2024-04-28 14:20:24.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/style.css
+-rw-rw-r--   0 xtof       (501) staff       (20)      821 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon-16x16.png
+-rw-rw-r--   0 xtof       (501) staff       (20)     1907 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon-32x32.png
+-rw-rw-r--   0 xtof       (501) staff       (20)    15406 2024-04-27 08:53:20.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon.ico
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.019731 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/img/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-12-06 14:26:46.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/img/.gitkeep
+-rw-r--r--   0 xtof       (501) staff       (20)    20142 2024-04-27 12:20:37.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/img/logo.svg
+-rw-r--r--   0 xtof       (501) staff       (20)       78 2023-12-06 14:26:46.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/robots.txt
+-rw-rw-r--   0 xtof       (501) staff       (20)      359 2024-04-27 13:15:48.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage/static/site.webmanifest
+-rw-r--r--   0 xtof       (501) staff       (20)      830 2024-04-28 14:20:16.000000 hosted-flasks-0.0.8/hosted_flasks/frontpage.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3021 2024-04-29 19:32:45.000000 hosted-flasks-0.0.8/hosted_flasks/loader.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2335 2024-04-29 19:37:42.000000 hosted-flasks-0.0.8/hosted_flasks/monkeypatch.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1753 2024-04-29 19:33:59.000000 hosted-flasks-0.0.8/hosted_flasks/server.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.017987 hosted-flasks-0.0.8/hosted_flasks.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     1807 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)     1139 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       62 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       36 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       25 2024-04-29 19:41:36.000000 hosted-flasks-0.0.8/hosted_flasks.egg-info/top_level.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2024-04-29 19:41:37.020470 hosted-flasks-0.0.8/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1639 2024-04-28 10:59:13.000000 hosted-flasks-0.0.8/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2024-04-29 19:41:37.020078 hosted-flasks-0.0.8/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2024-03-13 07:52:10.000000 hosted-flasks-0.0.8/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1029 2024-04-29 19:40:04.000000 hosted-flasks-0.0.8/tests/test_environ_get.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3678 2024-04-29 19:35:16.000000 hosted-flasks-0.0.8/tests/test_loader.py
```

### Comparing `hosted-flasks-0.0.7/.github/README.md` & `hosted-flasks-0.0.8/.github/README.md`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/LICENSE.txt` & `hosted-flasks-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/PKG-INFO` & `hosted-flasks-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.7
+Version: 0.0.8
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.7/docs/conf.py` & `hosted-flasks-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/__main__.py` & `hosted-flasks-0.0.8/hosted_flasks/__main__.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/index.html` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/index.html`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/android-chrome-192x192.png` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/android-chrome-512x512.png` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/apple-touch-icon.png` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/default.css` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/default.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/css/style.css` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/css/style.css`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon-16x16.png` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon-32x32.png` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/favicon.ico` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage/static/img/logo.svg` & `hosted-flasks-0.0.8/hosted_flasks/frontpage/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/frontpage.py` & `hosted-flasks-0.0.8/hosted_flasks/frontpage.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/hosted_flasks/loader.py` & `hosted-flasks-0.0.8/hosted_flasks/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,20 +67,20 @@
       spec.loader.exec_module(mod)
       # extract the handler from the mod using the appname
       self.handler = getattr(mod, appname)
     except FileNotFoundError:
       logger.warning(f"😞 '{module_path}' doesn't provide '__init__.py'")
     except AttributeError:
       logger.warning(f"😞 '{module_path}' doesn't provide flask object: {self.app}")
-    except Exception as ex:
-      logger.warning(f"😞 '{module_path}' failed to load due to {ex}")
+    except Exception:
+      logger.exception(f"😞 '{module_path}' failed to load due to")
 
 def add_app(name, src, **kwargs):
   app = HostedFlask(name, src, **kwargs)
-  logger.info(f"🌍 added {app.name}")
+  logger.info(f"🌍 loaded app: {app.name}")
 
 def get_apps(config=None, force=False):
   global apps
 
   if force:
     apps.clear()
```

### Comparing `hosted-flasks-0.0.7/hosted_flasks/monkeypatch.py` & `hosted-flasks-0.0.8/hosted_flasks/monkeypatch.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,31 +16,36 @@
 
 class Environment(UserDict):
 
   def __init__(self, *args, **kwargs):
     self._debug = False
     super().__init__(*args, **kwargs)
 
+  def _get_raw(self, key):
+    # utility to access env var without looking up the calling app
+    return super().__getitem__(key)  # pragma: no cover
+
+  def _log(self, msg):
+    if self._debug:
+      logger.info(msg) # pragma: no cover
+
   def _get_calling_app(self):
     # walk up the stack to find a frame that originated in one of the hosted
     # flasks. if so, use its name as a prefix for retrieving an app specific
     # version of the environment variable
     frames = inspect.stack()[2:]
     for caller in frames:
-      if self._debug:
-        logger.info(f"matching {caller.filename}")
+      self._log(f"matching {caller.filename}")
       for app in loader.apps: # access apps directly to avoid loop with get_apps
         try:
-          if self._debug:
-            logger.info(f"  against {app.src.parent}")
+          self._log(f"  against {app.src.parent}")
           calling_app = Path(caller.filename).relative_to(app.src.parent).parts[0]
           # we found a frame that originated in a hosted flask app's src
           # the root of this path is the app folder and also the prefix name
-          if self._debug:
-            logger.info(f"  SUCCESS: {calling_app}")
+          self._log(f"  SUCCESS: {calling_app}")
           return calling_app
         except ValueError: # pathlib: does not start with...
           pass
     return None
   
   def __setitem__(self, key, value):
     # in case of a call from a hosted flask app, add a prefix
@@ -50,27 +55,24 @@
     super().__setitem__(key, value)
 
   def __getitem__(self, key):
     # in case of a call from a hosted flask app, try a prefix first
     calling_app = self._get_calling_app()
     if calling_app:
       app_key = f"{calling_app.upper()}_{key}"
-      if self._debug:
-        logger.info(f"  trying to get {app_key}")
+      self._log(f"  trying to get {app_key}")
       try:
         value = super().__getitem__(app_key)
-        if self._debug:
-          logger.info(f"  SUCCESS {app_key} = {value}")
+        self._log(f"  SUCCESS {app_key} = {value}")
         return value
       except KeyError:
         pass
 
     # fall back to the non-prefixed variable
-    if self._debug:
-      logger.info(f"  FAIL: trying {key}")
+    self._log(f"  FAIL: trying {key}")
     try:
       value = super().__getitem__(key)
     except KeyError:
       raise KeyError
 
     return value
```

### Comparing `hosted-flasks-0.0.7/hosted_flasks.egg-info/PKG-INFO` & `hosted-flasks-0.0.8/hosted_flasks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosted-flasks
-Version: 0.0.7
+Version: 0.0.8
 Summary: serve flask apps side by side
 Home-page: https://github.com/christophevg/hosted-flasks
 Author: Christophe VG
 License: MIT
 Description: # Hosted Flasks
         
         > serve flask apps side by side
```

### Comparing `hosted-flasks-0.0.7/hosted_flasks.egg-info/SOURCES.txt` & `hosted-flasks-0.0.8/hosted_flasks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/setup.py` & `hosted-flasks-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/tests/test_environ_get.py` & `hosted-flasks-0.0.8/tests/test_environ_get.py`

 * *Files identical despite different names*

### Comparing `hosted-flasks-0.0.7/tests/test_loader.py` & `hosted-flasks-0.0.8/tests/test_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,32 @@
   path: /dummy
 """
   config.write_text(content)
   
   apps = get_apps(config, force=True)
   assert len(apps) == 0
 
+def test_app_that_throws_exception_is_not_loaded(tmp_path):
+  # add dummy implementation, without exposing a Flask object
+  dummy = tmp_path / "dummy"
+  dummy.mkdir()
+  init = dummy / "__init__.py"
+  init.write_text("raise KeyError")
+
+  config = tmp_path / "hosted-flasks.yaml"
+  content = """
+dummy:
+  src: dummy
+  path: /dummy
+"""
+  config.write_text(content)
+  
+  apps = get_apps(config, force=True)
+  assert len(apps) == 0
+
 def test_app_with_not_default_appname(tmp_path):
   app_name = "custom_app"
   folder = tmp_path / app_name
   folder.mkdir()
   init = folder / "__init__.py"
   init.write_text("""
 from flask import Flask
```

