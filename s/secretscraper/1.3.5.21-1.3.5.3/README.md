# Comparing `tmp/secretscraper-1.3.5.21.tar.gz` & `tmp/secretscraper-1.3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.5.21.tar", max compression
+gzip compressed data, was "secretscraper-1.3.5.3.tar", max compression
```

## Comparing `secretscraper-1.3.5.21.tar` & `secretscraper-1.3.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.5.21/LICENSE
--rw-r--r--   0        0        0     8045 2024-04-28 15:15:35.500487 secretscraper-1.3.5.21/README.md
--rw-r--r--   0        0        0     1564 2024-04-28 14:48:27.584726 secretscraper-1.3.5.21/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-28 14:48:27.582340 secretscraper-1.3.5.21/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7342 2024-04-28 10:34:57.446046 secretscraper-1.3.5.21/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.5.21/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.5.21/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.5.21/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    13871 2024-04-28 14:46:59.627655 secretscraper-1.3.5.21/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.5.21/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.5.21/src/secretscraper/exception.py
--rw-r--r--   0        0        0    13970 2024-04-28 12:52:15.237040 secretscraper-1.3.5.21/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.5.21/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6185 2024-04-28 09:05:09.333925 secretscraper-1.3.5.21/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.5.21/src/secretscraper/log.py
--rw-r--r--   0        0        0     8338 2024-04-28 10:09:13.958687 secretscraper-1.3.5.21/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.5.21/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4531 2024-04-28 08:44:21.841407 secretscraper-1.3.5.21/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2073 2024-04-28 12:56:38.015644 secretscraper-1.3.5.21/src/secretscraper/util.py
--rw-r--r--   0        0        0     8983 1970-01-01 00:00:00.000000 secretscraper-1.3.5.21/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.5.3/LICENSE
+-rw-r--r--   0        0        0     8045 2024-04-28 15:15:35.500487 secretscraper-1.3.5.3/README.md
+-rw-r--r--   0        0        0     1563 2024-04-28 15:17:36.365676 secretscraper-1.3.5.3/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-28 15:17:36.370896 secretscraper-1.3.5.3/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7342 2024-04-28 10:34:57.446046 secretscraper-1.3.5.3/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.5.3/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.5.3/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.5.3/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    13871 2024-04-28 14:46:59.627655 secretscraper-1.3.5.3/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.5.3/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.5.3/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    13970 2024-04-28 12:52:15.237040 secretscraper-1.3.5.3/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.5.3/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6185 2024-04-28 09:05:09.333925 secretscraper-1.3.5.3/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.5.3/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8338 2024-04-28 10:09:13.958687 secretscraper-1.3.5.3/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.5.3/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4531 2024-04-28 08:44:21.841407 secretscraper-1.3.5.3/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2073 2024-04-28 12:56:38.015644 secretscraper-1.3.5.3/src/secretscraper/util.py
+-rw-r--r--   0        0        0     8982 1970-01-01 00:00:00.000000 secretscraper-1.3.5.3/PKG-INFO
```

### Comparing `secretscraper-1.3.5.21/LICENSE` & `secretscraper-1.3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/README.md` & `secretscraper-1.3.5.3/README.md`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/pyproject.toml` & `secretscraper-1.3.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.5.21"
+version = "1.3.5.3"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.5.21/src/secretscraper/cmdline.py` & `secretscraper-1.3.5.3/src/secretscraper/cmdline.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/config/__init__.py` & `secretscraper-1.3.5.3/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/config/settings.yml` & `secretscraper-1.3.5.3/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/coroutinue.py` & `secretscraper-1.3.5.3/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/crawler.py` & `secretscraper-1.3.5.3/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/entity.py` & `secretscraper-1.3.5.3/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/exception.py` & `secretscraper-1.3.5.3/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/facade.py` & `secretscraper-1.3.5.3/src/secretscraper/facade.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/filter.py` & `secretscraper-1.3.5.3/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/handler.py` & `secretscraper-1.3.5.3/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/log.py` & `secretscraper-1.3.5.3/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/output_formatter.py` & `secretscraper-1.3.5.3/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/scanner.py` & `secretscraper-1.3.5.3/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/urlparser.py` & `secretscraper-1.3.5.3/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/src/secretscraper/util.py` & `secretscraper-1.3.5.3/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.5.21/PKG-INFO` & `secretscraper-1.3.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.5.21
+Version: 1.3.5.3
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

