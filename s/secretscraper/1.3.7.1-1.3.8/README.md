# Comparing `tmp/secretscraper-1.3.7.1.tar.gz` & `tmp/secretscraper-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.7.1.tar", max compression
+gzip compressed data, was "secretscraper-1.3.8.tar", max compression
```

## Comparing `secretscraper-1.3.7.1.tar` & `secretscraper-1.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.7.1/LICENSE
--rw-r--r--   0        0        0     7688 2024-04-29 08:11:45.360134 secretscraper-1.3.7.1/README.md
--rw-r--r--   0        0        0     1867 2024-04-29 08:14:33.413313 secretscraper-1.3.7.1/pyproject.toml
--rw-r--r--   0        0        0       45 2024-04-29 08:14:33.410081 secretscraper-1.3.7.1/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7377 2024-04-29 07:51:50.571867 secretscraper-1.3.7.1/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.7.1/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.7.1/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.7.1/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    13941 2024-04-29 07:58:22.443148 secretscraper-1.3.7.1/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.7.1/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.7.1/src/secretscraper/exception.py
--rw-r--r--   0        0        0    14024 2024-04-29 07:58:22.439882 secretscraper-1.3.7.1/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.7.1/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.7.1/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.7.1/src/secretscraper/log.py
--rw-r--r--   0        0        0     8429 2024-04-29 07:58:22.445776 secretscraper-1.3.7.1/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.7.1/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4538 2024-04-29 07:57:20.130291 secretscraper-1.3.7.1/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2264 2024-04-29 08:04:46.278752 secretscraper-1.3.7.1/src/secretscraper/util.py
--rw-r--r--   0        0        0     9086 1970-01-01 00:00:00.000000 secretscraper-1.3.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.8/LICENSE
+-rw-r--r--   0        0        0     7904 2024-04-29 11:46:22.977178 secretscraper-1.3.8/README.md
+-rw-r--r--   0        0        0     1865 2024-04-29 11:45:35.229587 secretscraper-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-04-29 11:45:35.226567 secretscraper-1.3.8/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7415 2024-04-29 11:35:42.170573 secretscraper-1.3.8/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.8/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.8/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.8/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    13941 2024-04-29 07:58:22.443148 secretscraper-1.3.8/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.8/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.8/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14069 2024-04-29 11:41:55.192819 secretscraper-1.3.8/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.8/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.8/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1893 2024-04-29 11:33:44.901874 secretscraper-1.3.8/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8429 2024-04-29 07:58:22.445776 secretscraper-1.3.8/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.8/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4538 2024-04-29 07:57:20.130291 secretscraper-1.3.8/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2264 2024-04-29 08:04:46.278752 secretscraper-1.3.8/src/secretscraper/util.py
+-rw-r--r--   0        0        0     9300 1970-01-01 00:00:00.000000 secretscraper-1.3.8/PKG-INFO
```

### Comparing `secretscraper-1.3.7.1/LICENSE` & `secretscraper-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/README.md` & `secretscraper-1.3.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # SecretScraper
 
 ![Tests](https://github.com/PadishahIII/SecretScraper/actions/workflows/main.yml/badge.svg)
+![Pypi Python Version](https://img.shields.io/pypi/pyversions/secretscraper.svg?style=plastic)
 
 ## Overview
 
 SecretScraper is a highly configurable web scrape tool that crawl links  from target websites and scrape sensitive
 data via regular expression.
 
 
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://github.com/PadishahIII/SecretScraper/assets/83501709/d1aa763f-5711-47c4-8b8f-9309bac88ae2" width=800>
 
 ## Feature
 - Web crawler: extract links via both DOM hierarchy and regex
 - Support domain white list and black list
 - Support multiple targets, input target URLs from a file
+- Support local file scan
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
 
 ## Prerequisite
 - Platform: Test on MaxOS, Ubuntu and Windows.
-- Python Version >= 3.11
+- Python Version >= 3.9
 
 ## Usage
 
 ### Install
 
 ```bash
 pip install secretscraper
@@ -205,14 +207,17 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.29 Version 1.3.8
+- Optimize log output
+- Optimize the performance of `--debug` option
 ## 2024.4.29 Version 1.3.7
 - Test on multiple python versions
 - Support python 3.9~3.11
 ## 2024.4.29 Version 1.3.6
 - Repackage
 
 ## 2024.4.28 Version 1.3.5
```

### Comparing `secretscraper-1.3.7.1/pyproject.toml` & `secretscraper-1.3.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.7.1"
+version = "1.3.8"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
```

### Comparing `secretscraper-1.3.7.1/src/secretscraper/cmdline.py` & `secretscraper-1.3.8/src/secretscraper/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from click import Context
 from dynaconf.base import Settings
 
 from secretscraper import __version__
 from secretscraper.config import settings
 from secretscraper.exception import FacadeException
 from secretscraper.facade import CrawlerFacade, FileScannerFacade
-from secretscraper.log import init_log
 
 facade_settings = settings  # for unit test
 facade_obj = None
 
 
 # @click.group(invoke_without_command=True)
 # @click.pass_context
@@ -104,34 +103,38 @@
 @click.option("-l", "--local", help="Local file or directory, scan local file/directory recursively ",
               type=click.Path(exists=True, file_okay=True, dir_okay=True, path_type=pathlib.Path))
 def main(**options):
     """Main commands"""
     if options["version"]:
         click.echo(__version__)
         exit(0)
-    if options["debug"]:
-        settings.DEBUG = True
-        settings.LOGLEVEL = "debug"
+    # load config file
     if options["config"] is not None:
         if not options["config"].exists():
             click.echo(f"Error: config file not exists: {str(options['config'])}")
             return
         settings.load_file(path=str(options["config"]))
     else:
         file = pathlib.Path() / "settings.yml"
         generate_configuration(file)
         settings.load_file(path=str(file.absolute()))
+
+    if options["debug"]:
+        settings['debug'] = True
+        settings['loglevel'] = "debug"
+
     options_dict = dict()
     for key, value in options.items():
         if value is not None:
             options_dict[key] = value
     # settings.update(options_dict)
     try:
         global facade_settings, facade_obj
         print_func = functools.partial(click.echo, color=True)
+        from secretscraper.log import init_log
         init_log()
         if options['local'] is not None:
             facade = FileScannerFacade(settings, options_dict, print_func)
         else:
             facade = CrawlerFacade(settings, options_dict, print_func=print_func)
         facade_obj = facade
         facade_settings = facade.settings
@@ -154,15 +157,15 @@
 loglevel: warning
 logpath: log
 
 proxy: "" # http://127.0.0.1:7890
 max_depth: 1 # 0 for no limit
 max_page_num: 1000 # 0 for no limit
 timeout: 5
-follow_redirects: false
+follow_redirects: true
 workers_num: 1000
 headers:
   Accept: "*/*"
   Cookie: ""
   User-Agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/80.0.3987.87 Safari/537.36 SE 2.X MetaSr 1.0
 
 urlFind:
```

### Comparing `secretscraper-1.3.7.1/src/secretscraper/config/__init__.py` & `secretscraper-1.3.8/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/config/settings.yml` & `secretscraper-1.3.8/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/coroutinue.py` & `secretscraper-1.3.8/src/secretscraper/coroutinue.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/crawler.py` & `secretscraper-1.3.8/src/secretscraper/crawler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/entity.py` & `secretscraper-1.3.8/src/secretscraper/entity.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/exception.py` & `secretscraper-1.3.8/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/facade.py` & `secretscraper-1.3.8/src/secretscraper/facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,39 +88,39 @@
                                     f"Target URLs: {', '.join(self.crawler.start_urls)}",
                                     bold=True,
                                     blink=True,
                                     )
                 self.crawler.start()
                 if self.detail_output:
                     # print_func_colorful(self.print_func,f"Total page: {self.crawler.total_page}")
-                    self.formatter.output_url_hierarchy(self.crawler.url_dict, True)
+                    f.write(self.formatter.output_url_hierarchy(self.crawler.url_dict, True))
 
                     if not self.hide_regex:
                         print_func_colorful(f, self.print_func,
                                             f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
                                             )
                     print_func_colorful(f, self.print_func, f"{self.formatter.output_js(self.crawler.js_dict)}")
-                    self.formatter.output_found_domains(list(self.crawler.found_urls), True)
+                    f.write(self.formatter.output_found_domains(list(self.crawler.found_urls), True))
                 else:
                     # tidy output
                     # URLs per domain
                     domains = set()
                     for url in self.crawler.start_urls:
                         try:
                             obj = urlparse(url)
                             domain, _ = to_host_port(obj.netloc)
                             if len(domain) > 0:
                                 domains.add(domain.strip())
                         except:
                             pass
-                    self.formatter.output_url_per_domain(domains, self.crawler.url_dict)
+                    f.write(self.formatter.output_url_per_domain(domains, self.crawler.url_dict))
                     # JS per domain
-                    self.formatter.output_url_per_domain(domains, self.crawler.js_dict, "JS")
+                    f.write(self.formatter.output_url_per_domain(domains, self.crawler.js_dict, "JS"))
                     # Domains
-                    self.formatter.output_found_domains(list(self.crawler.found_urls), True)
+                    f.write(self.formatter.output_found_domains(list(self.crawler.found_urls), True))
                     # Secrets
                     if not self.hide_regex:
                         print_func_colorful(f, self.print_func,
                                             f"{self.formatter.output_secrets(self.crawler.url_secrets)}"
                                             )
             except KeyboardInterrupt:
                 self.print_func("\nExiting...")
```

### Comparing `secretscraper-1.3.7.1/src/secretscraper/filter.py` & `secretscraper-1.3.8/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/handler.py` & `secretscraper-1.3.8/src/secretscraper/handler.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/log.py` & `secretscraper-1.3.8/src/secretscraper/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 import logging
 import os
 from logging.config import dictConfig
 
 from secretscraper.config import settings
 
-os.makedirs(settings.LOGPATH, exist_ok=True)
+
+# os.makedirs(settings.LOGPATH, exist_ok=True) # not make new dir for log
 
 
 def verbose_formatter(verbose: int) -> str:
     """formatter factory"""
     if verbose is True:
         return "verbose"
     return "simple"
```

### Comparing `secretscraper-1.3.7.1/src/secretscraper/output_formatter.py` & `secretscraper-1.3.8/src/secretscraper/output_formatter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/scanner.py` & `secretscraper-1.3.8/src/secretscraper/scanner.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/urlparser.py` & `secretscraper-1.3.8/src/secretscraper/urlparser.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/src/secretscraper/util.py` & `secretscraper-1.3.8/src/secretscraper/util.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.7.1/PKG-INFO` & `secretscraper-1.3.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.7.1
+Version: 1.3.8
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,34 +23,36 @@
 Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; python_version >= "3.11" and python_version < "4.0" and sys_platform == "darwin"
 Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; python_version >= "3.11" and python_version < "4.0" and sys_platform == "linux"
 Description-Content-Type: text/markdown
 
 # SecretScraper
 
 ![Tests](https://github.com/PadishahIII/SecretScraper/actions/workflows/main.yml/badge.svg)
+![Pypi Python Version](https://img.shields.io/pypi/pyversions/secretscraper.svg?style=plastic)
 
 ## Overview
 
 SecretScraper is a highly configurable web scrape tool that crawl links  from target websites and scrape sensitive
 data via regular expression.
 
 
  <img alt="Shows an illustrated sun in light mode and a moon with stars in dark mode." src="https://github.com/PadishahIII/SecretScraper/assets/83501709/d1aa763f-5711-47c4-8b8f-9309bac88ae2" width=800>
 
 ## Feature
 - Web crawler: extract links via both DOM hierarchy and regex
 - Support domain white list and black list
 - Support multiple targets, input target URLs from a file
+- Support local file scan
 - Scalable customization: header, proxy, timeout, cookie, scrape depth, follow redirect, etc.
 - Built-in regex to search for sensitive information
 - Flexible configuration in yaml format
 
 ## Prerequisite
 - Platform: Test on MaxOS, Ubuntu and Windows.
-- Python Version >= 3.11
+- Python Version >= 3.9
 
 ## Usage
 
 ### Install
 
 ```bash
 pip install secretscraper
@@ -231,14 +233,17 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.29 Version 1.3.8
+- Optimize log output
+- Optimize the performance of `--debug` option
 ## 2024.4.29 Version 1.3.7
 - Test on multiple python versions
 - Support python 3.9~3.11
 ## 2024.4.29 Version 1.3.6
 - Repackage
 
 ## 2024.4.28 Version 1.3.5
```

