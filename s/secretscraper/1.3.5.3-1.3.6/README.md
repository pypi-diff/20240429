# Comparing `tmp/secretscraper-1.3.5.3.tar.gz` & `tmp/secretscraper-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.5.3.tar", max compression
+gzip compressed data, was "secretscraper-1.3.6.tar", max compression
```

## Comparing `secretscraper-1.3.5.3.tar` & `secretscraper-1.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.5.3/LICENSE
--rw-r--r--   0        0        0     8045 2024-04-28 15:15:35.500487 secretscraper-1.3.5.3/README.md
--rw-r--r--   0        0        0     1563 2024-04-28 15:17:36.365676 secretscraper-1.3.5.3/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-28 15:17:36.370896 secretscraper-1.3.5.3/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7342 2024-04-28 10:34:57.446046 secretscraper-1.3.5.3/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.5.3/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.5.3/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.5.3/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    13871 2024-04-28 14:46:59.627655 secretscraper-1.3.5.3/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.5.3/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.5.3/src/secretscraper/exception.py
--rw-r--r--   0        0        0    13970 2024-04-28 12:52:15.237040 secretscraper-1.3.5.3/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.5.3/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6185 2024-04-28 09:05:09.333925 secretscraper-1.3.5.3/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.5.3/src/secretscraper/log.py
--rw-r--r--   0        0        0     8338 2024-04-28 10:09:13.958687 secretscraper-1.3.5.3/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.5.3/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4531 2024-04-28 08:44:21.841407 secretscraper-1.3.5.3/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2073 2024-04-28 12:56:38.015644 secretscraper-1.3.5.3/src/secretscraper/util.py
--rw-r--r--   0        0        0     8982 1970-01-01 00:00:00.000000 secretscraper-1.3.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.6/LICENSE
+-rw-r--r--   0        0        0     7600 2024-04-29 05:06:36.753419 secretscraper-1.3.6/README.md
+-rw-r--r--   0        0        0     1561 2024-04-29 05:07:15.971653 secretscraper-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-29 05:07:15.968194 secretscraper-1.3.6/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7342 2024-04-28 10:34:57.446046 secretscraper-1.3.6/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.6/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.6/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.6/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    13871 2024-04-28 14:46:59.627655 secretscraper-1.3.6/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.6/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.6/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    13970 2024-04-28 12:52:15.237040 secretscraper-1.3.6/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.6/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6185 2024-04-28 09:05:09.333925 secretscraper-1.3.6/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.6/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8338 2024-04-28 10:09:13.958687 secretscraper-1.3.6/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.6/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4531 2024-04-28 08:44:21.841407 secretscraper-1.3.6/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2073 2024-04-28 12:56:38.015644 secretscraper-1.3.6/src/secretscraper/util.py
+-rw-r--r--   0        0        0     8535 1970-01-01 00:00:00.000000 secretscraper-1.3.6/PKG-INFO
```

### Comparing `secretscraper-1.3.5.3/LICENSE` & `secretscraper-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/README.md` & `secretscraper-1.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 ## Overview
 
 SecretScraper is a highly configurable web scrape tool that crawl links  from target websites and scrape sensitive
 data via regular expression.
 
 
+ <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://github.com/PadishahIII/SecretScraper/assets/83501709/d1aa763f-5711-47c4-8b8f-9309bac88ae2" width=800>
+
 ## Feature
 - Web crawler: extract links via both DOM hierarchy and regex
 - Support domain white list and black list
 - Support multiple targets, input target URLs from a file
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
@@ -46,51 +48,20 @@
 # urls
 http://scrapeme.live/1
 http://scrapeme.live/2
 http://scrapeme.live/3
 http://scrapeme.live/4
 http://scrapeme.live/1
 ```
-A sample output:
+Sample output:
 <img width="1125" alt="image" src="https://github.com/PadishahIII/SecretScraper/assets/83501709/00dd2053-7b9a-4ef3-a2b2-8c168e8ec0ee">
 
-```text
-> secretscraper -u http://127.0.0.1:8888
-Target urls num: 1
-Max depth: 1, Max page num: 1000
-Output file: /Users/padishah/Documents/Files/Python_WorkSpace/secretscraper/src/secretscraper/crawler.log
-Target URLs: http://127.0.0.1:8888
-
-1 URLs from http://127.0.0.1:8888 [200] (depth:0):
-http://127.0.0.1:8888/index.html [200]
-
-1 Domains:
-127.0.0.1:8888
-
-
-13 Secrets found in http://127.0.0.1:8888/1.js 200:
-Email: 3333333qqqxxxx@qq.com
-Shiro: =deleteme
-JS Map: xx/static/asdfaf.js.map
-Email: example@example.com
-Swagger: static/swagger-ui.html
-ID Card: 130528200011110000
-URL as a Value: redirect=http://
-Phone: 13273487666
-Internal IP:  192.168.1.1
-Cloud Key: Accesskeyid
-Cloud Key: AccessKeySecret
-Shiro: rememberme=
-Internal IP:  10.0.0.1
+<img width="990" alt="image" src="https://github.com/PadishahIII/SecretScraper/assets/83501709/fa733a3f-8a8a-4d79-814f-a4c115d1e056">
 
 
-1 JS from http://127.0.0.1:8888:
-http://127.0.0.1:8888/1.js [200]
-```
-
 All supported options:
 ```bash
 > secretscraper --help
 Usage: secretscraper [OPTIONS]
 
   Main commands
 
@@ -234,14 +205,17 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.29 Version 1.3.6
+- Repackage
+
 ## 2024.4.28 Version 1.3.5
 - **New Features**
   - Support windows
   - Optimize crawler
   - Prettify output, add `--detail` option
   - Generate default configuration to settings.yml
   - Avoid requesting dangerous paths
```

### Comparing `secretscraper-1.3.5.3/pyproject.toml` & `secretscraper-1.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.5.3"
+version = "1.3.6"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.5.3/src/secretscraper/cmdline.py` & `secretscraper-1.3.6/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/config/__init__.py` & `secretscraper-1.3.6/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/config/settings.yml` & `secretscraper-1.3.6/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/coroutinue.py` & `secretscraper-1.3.6/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/crawler.py` & `secretscraper-1.3.6/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/entity.py` & `secretscraper-1.3.6/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/exception.py` & `secretscraper-1.3.6/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/facade.py` & `secretscraper-1.3.6/src/secretscraper/facade.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/filter.py` & `secretscraper-1.3.6/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/handler.py` & `secretscraper-1.3.6/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/log.py` & `secretscraper-1.3.6/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/output_formatter.py` & `secretscraper-1.3.6/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/scanner.py` & `secretscraper-1.3.6/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/urlparser.py` & `secretscraper-1.3.6/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/src/secretscraper/util.py` & `secretscraper-1.3.6/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.3/PKG-INFO` & `secretscraper-1.3.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.5.3
+Version: 1.3.6
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -26,14 +26,16 @@
 
 ## Overview
 
 SecretScraper is a highly configurable web scrape tool that crawl links  from target websites and scrape sensitive
 data via regular expression.
 
 
+ <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://github.com/PadishahIII/SecretScraper/assets/83501709/d1aa763f-5711-47c4-8b8f-9309bac88ae2" width=800>
+
 ## Feature
 - Web crawler: extract links via both DOM hierarchy and regex
 - Support domain white list and black list
 - Support multiple targets, input target URLs from a file
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
@@ -68,51 +70,20 @@
 # urls
 http://scrapeme.live/1
 http://scrapeme.live/2
 http://scrapeme.live/3
 http://scrapeme.live/4
 http://scrapeme.live/1
 ```
-A sample output:
+Sample output:
 <img width="1125" alt="image" src="https://github.com/PadishahIII/SecretScraper/assets/83501709/00dd2053-7b9a-4ef3-a2b2-8c168e8ec0ee">
 
-```text
-> secretscraper -u http://127.0.0.1:8888
-Target urls num: 1
-Max depth: 1, Max page num: 1000
-Output file: /Users/padishah/Documents/Files/Python_WorkSpace/secretscraper/src/secretscraper/crawler.log
-Target URLs: http://127.0.0.1:8888
-
-1 URLs from http://127.0.0.1:8888 [200] (depth:0):
-http://127.0.0.1:8888/index.html [200]
-
-1 Domains:
-127.0.0.1:8888
-
-
-13 Secrets found in http://127.0.0.1:8888/1.js 200:
-Email: 3333333qqqxxxx@qq.com
-Shiro: =deleteme
-JS Map: xx/static/asdfaf.js.map
-Email: example@example.com
-Swagger: static/swagger-ui.html
-ID Card: 130528200011110000
-URL as a Value: redirect=http://
-Phone: 13273487666
-Internal IP:  192.168.1.1
-Cloud Key: Accesskeyid
-Cloud Key: AccessKeySecret
-Shiro: rememberme=
-Internal IP:  10.0.0.1
+<img width="990" alt="image" src="https://github.com/PadishahIII/SecretScraper/assets/83501709/fa733a3f-8a8a-4d79-814f-a4c115d1e056">
 
 
-1 JS from http://127.0.0.1:8888:
-http://127.0.0.1:8888/1.js [200]
-```
-
 All supported options:
 ```bash
 > secretscraper --help
 Usage: secretscraper [OPTIONS]
 
   Main commands
 
@@ -256,14 +227,17 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.29 Version 1.3.6
+- Repackage
+
 ## 2024.4.28 Version 1.3.5
 - **New Features**
   - Support windows
   - Optimize crawler
   - Prettify output, add `--detail` option
   - Generate default configuration to settings.yml
   - Avoid requesting dangerous paths
```

