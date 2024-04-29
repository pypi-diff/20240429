# Comparing `tmp/webdriver_browser-0.1.6.tar.gz` & `tmp/webdriver_browser-0.1.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_browser-0.1.6.tar", max compression
+gzip compressed data, was "webdriver_browser-0.1.6.post1.tar", max compression
```

## Comparing `webdriver_browser-0.1.6.tar` & `webdriver_browser-0.1.6.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1089 2024-01-19 15:17:22.905063 webdriver_browser-0.1.6/LICENSE
--rw-r--r--   0        0        0      817 2024-04-26 14:33:45.538128 webdriver_browser-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      603 2024-04-26 13:47:48.636884 webdriver_browser-0.1.6/README.md
--rw-r--r--   0        0        0    15859 2024-04-27 16:06:17.768675 webdriver_browser-0.1.6/webdriver_browser/__init__.py
--rw-r--r--   0        0        0     4121 2024-04-26 13:38:52.072068 webdriver_browser-0.1.6/webdriver_browser/chrome.py
--rw-r--r--   0        0        0     1142 2024-04-26 13:35:59.627517 webdriver_browser-0.1.6/webdriver_browser/edge.py
--rw-r--r--   0        0        0     3095 2024-04-26 13:35:45.583395 webdriver_browser-0.1.6/webdriver_browser/firefox.py
--rw-r--r--   0        0        0     5484 2024-01-19 15:17:22.915062 webdriver_browser-0.1.6/webdriver_browser/patch.py
--rw-r--r--   0        0        0     6191 2024-01-19 15:17:22.917572 webdriver_browser-0.1.6/webdriver_browser/rsync.py
--rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 webdriver_browser-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-01-19 15:17:22.905063 webdriver_browser-0.1.6.post1/LICENSE
+-rw-r--r--   0        0        0      823 2024-04-29 09:31:06.915976 webdriver_browser-0.1.6.post1/pyproject.toml
+-rw-r--r--   0        0        0      603 2024-04-26 13:47:48.636884 webdriver_browser-0.1.6.post1/README.md
+-rw-r--r--   0        0        0    15894 2024-04-29 09:37:27.274886 webdriver_browser-0.1.6.post1/webdriver_browser/__init__.py
+-rw-r--r--   0        0        0     4308 2024-04-29 09:37:45.967698 webdriver_browser-0.1.6.post1/webdriver_browser/chrome.py
+-rw-r--r--   0        0        0     1228 2024-04-29 09:33:53.996527 webdriver_browser-0.1.6.post1/webdriver_browser/edge.py
+-rw-r--r--   0        0        0     3145 2024-04-29 09:34:01.999825 webdriver_browser-0.1.6.post1/webdriver_browser/firefox.py
+-rw-r--r--   0        0        0     5484 2024-01-19 15:17:22.915062 webdriver_browser-0.1.6.post1/webdriver_browser/patch.py
+-rw-r--r--   0        0        0     6191 2024-01-19 15:17:22.917572 webdriver_browser-0.1.6.post1/webdriver_browser/rsync.py
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 webdriver_browser-0.1.6.post1/PKG-INFO
```

### Comparing `webdriver_browser-0.1.6/LICENSE` & `webdriver_browser-0.1.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_browser-0.1.6/pyproject.toml` & `webdriver_browser-0.1.6.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webdriver-browser"
-version = "0.1.6"
+version = "0.1.6.post1"
 description = "More convenient methods for creating multiple selenium browsers."
 authors = ["Invoker Bot <invoker-bot@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `webdriver_browser-0.1.6/README.md` & `webdriver_browser-0.1.6.post1/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_browser-0.1.6/webdriver_browser/__init__.py` & `webdriver_browser-0.1.6.post1/webdriver_browser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,19 +40,21 @@
     proxy_server: str = None
     extensions_dirs: list[str] = None
     headless: bool = False
     force_selenium_wire: bool = False
     wait_timeout: float = 15.0
     compressed: bool = False
     singleton: bool = False
+    disable_image: bool = False
     undetected_chrome_driver: bool = None
 
 
 class RemoteBrowser(ABC):  # pylint: disable=too-many-public-methods
     """Remote browser"""
+    browser_names = {'msedge', 'chrome', 'firefox', 'firefox-bin'}
 
     def __init__(self, options: BrowserOptions = None, driver_manager: DriverManager = None):
         if options is None:
             options = BrowserOptions()
         self.options = options
         if options.singleton:
             self.kill_all_browser()
@@ -141,21 +143,20 @@
         """Default driver manager"""
 
     @classmethod
     def use_seleniumwire(cls, options: BrowserOptions):
         """Use seleniumwire or not"""
         return options.force_selenium_wire or (options.proxy_server is not None and options.proxy_server.find('@') != -1)
 
-    @staticmethod
-    def kill_all_browser():
+    @classmethod
+    def kill_all_browser(cls):
         """Kill all browsers"""
-        browser_names = {'msedge', 'chrome', 'firefox', 'firefox-bin'}
         for proc in psutil.process_iter(['pid', 'name']):
             proc_name = proc.info['name'].split('.')[0].lower()
-            if proc_name in browser_names:
+            if proc_name in cls.browser_names:
                 try:
                     process = psutil.Process(proc.info['pid'])
                     process.terminate()
                 except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                     logger.warning("zombie process: %s(%s)", proc_name, proc.info['pid'])
 
     @classmethod
```

### Comparing `webdriver_browser-0.1.6/webdriver_browser/chrome.py` & `webdriver_browser-0.1.6.post1/webdriver_browser/chrome.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 import seleniumwire.undetected_chromedriver as wire_uc
 from webdriver_manager.chrome import ChromeDriverManager
 from . import RemoteBrowser, BrowserOptions
 
 
 class ChromeBrowser(RemoteBrowser):
     """Chrome browser"""
+    browser_names = {'chrome', 'googlechrome', 'google-chrome', 'gc'}
 
     @classmethod
     def config_driver_options(cls, options: BrowserOptions, driver_options: webdriver.ChromeOptions):
         """Driver options"""
         driver_options.add_argument("--lang=en")
         driver_options.add_argument("--no-first-run")
         driver_options.add_argument("--disable-notifications")
         driver_options.add_argument("--ignore-certificate-errors")
+        if options.disable_image:
+            driver_options.add_argument('--blink-settings=imagesEnabled=false')
         if options.headless:
             driver_options.add_argument("--headless")
             driver_options.add_argument("--no-sandbox")
             driver_options.add_argument("--disable-dev-shm-usage")
             driver_options.add_argument("--disable-gpu")
         if options.data_dir is not None:
             driver_options.add_argument(f"--user-data-dir={cls.get_data_dir(options.data_dir)}")
```

### Comparing `webdriver_browser-0.1.6/webdriver_browser/edge.py` & `webdriver_browser-0.1.6.post1/webdriver_browser/edge.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from webdriver_manager.microsoft import EdgeChromiumDriverManager
 from seleniumwire import webdriver as wire_webdriver
 from .chrome import ChromeBrowser
 
 
 class EdgeBrowser(ChromeBrowser):
     """Edge browser"""
+    browser_names = {'edge', 'msedge', 'microsoftedge', 'ms-edge', 'microsoft-edge'}
 
     @classmethod
     def driver_options(cls, options):
         driver_options = webdriver.EdgeOptions()
         return cls.config_driver_options(options, driver_options)
 
     @classmethod
```

### Comparing `webdriver_browser-0.1.6/webdriver_browser/firefox.py` & `webdriver_browser-0.1.6.post1/webdriver_browser/firefox.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from seleniumwire import webdriver as wire_webdriver
 from webdriver_manager.firefox import GeckoDriverManager
 from . import RemoteBrowser
 
 
 class FirefoxBrowser(RemoteBrowser):
     """Firefox browser"""
+    browser_names = {'firefox', 'mozilla', 'ff'}
 
     @classmethod
     def driver_options(cls, options):
         """Driver options"""
         driver_options = webdriver.FirefoxOptions()
         driver_options.accept_insecure_certs = True
         driver_options.headless = options.headless
```

### Comparing `webdriver_browser-0.1.6/webdriver_browser/patch.py` & `webdriver_browser-0.1.6.post1/webdriver_browser/patch.py`

 * *Files identical despite different names*

### Comparing `webdriver_browser-0.1.6/webdriver_browser/rsync.py` & `webdriver_browser-0.1.6.post1/webdriver_browser/rsync.py`

 * *Files identical despite different names*

### Comparing `webdriver_browser-0.1.6/PKG-INFO` & `webdriver_browser-0.1.6.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver-browser
-Version: 0.1.6
+Version: 0.1.6.post1
 Summary: More convenient methods for creating multiple selenium browsers.
 License: MIT
 Author: Invoker Bot
 Author-email: invoker-bot@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

