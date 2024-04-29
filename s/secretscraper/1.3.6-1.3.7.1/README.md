# Comparing `tmp/secretscraper-1.3.6.tar.gz` & `tmp/secretscraper-1.3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secretscraper-1.3.6.tar", max compression
+gzip compressed data, was "secretscraper-1.3.7.1.tar", max compression
```

## Comparing `secretscraper-1.3.6.tar` & `secretscraper-1.3.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.6/LICENSE
--rw-r--r--   0        0        0     7600 2024-04-29 05:06:36.753419 secretscraper-1.3.6/README.md
--rw-r--r--   0        0        0     1561 2024-04-29 05:07:15.971653 secretscraper-1.3.6/pyproject.toml
--rw-r--r--   0        0        0       43 2024-04-29 05:07:15.968194 secretscraper-1.3.6/src/secretscraper/__init__.py
--rw-r--r--   0        0        0     7342 2024-04-28 10:34:57.446046 secretscraper-1.3.6/src/secretscraper/cmdline.py
--rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.6/src/secretscraper/config/__init__.py
--rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.6/src/secretscraper/config/settings.yml
--rw-r--r--   0        0        0     7291 2024-04-15 07:08:57.009196 secretscraper-1.3.6/src/secretscraper/coroutinue.py
--rw-r--r--   0        0        0    13871 2024-04-28 14:46:59.627655 secretscraper-1.3.6/src/secretscraper/crawler.py
--rw-r--r--   0        0        0     1364 2024-04-15 07:17:15.401289 secretscraper-1.3.6/src/secretscraper/entity.py
--rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.6/src/secretscraper/exception.py
--rw-r--r--   0        0        0    13970 2024-04-28 12:52:15.237040 secretscraper-1.3.6/src/secretscraper/facade.py
--rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.6/src/secretscraper/filter.py
--rw-r--r--   0        0        0     6185 2024-04-28 09:05:09.333925 secretscraper-1.3.6/src/secretscraper/handler.py
--rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.6/src/secretscraper/log.py
--rw-r--r--   0        0        0     8338 2024-04-28 10:09:13.958687 secretscraper-1.3.6/src/secretscraper/output_formatter.py
--rw-r--r--   0        0        0     1396 2024-04-26 08:09:43.131988 secretscraper-1.3.6/src/secretscraper/scanner.py
--rw-r--r--   0        0        0     4531 2024-04-28 08:44:21.841407 secretscraper-1.3.6/src/secretscraper/urlparser.py
--rw-r--r--   0        0        0     2073 2024-04-28 12:56:38.015644 secretscraper-1.3.6/src/secretscraper/util.py
--rw-r--r--   0        0        0     8535 1970-01-01 00:00:00.000000 secretscraper-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 13:21:30.604636 secretscraper-1.3.7.1/LICENSE
+-rw-r--r--   0        0        0     7688 2024-04-29 08:11:45.360134 secretscraper-1.3.7.1/README.md
+-rw-r--r--   0        0        0     1867 2024-04-29 08:14:33.413313 secretscraper-1.3.7.1/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-04-29 08:14:33.410081 secretscraper-1.3.7.1/src/secretscraper/__init__.py
+-rw-r--r--   0        0        0     7377 2024-04-29 07:51:50.571867 secretscraper-1.3.7.1/src/secretscraper/cmdline.py
+-rw-r--r--   0        0        0     1061 2024-04-16 09:41:18.245730 secretscraper-1.3.7.1/src/secretscraper/config/__init__.py
+-rw-r--r--   0        0        0     2506 2024-04-28 14:43:59.561661 secretscraper-1.3.7.1/src/secretscraper/config/settings.yml
+-rw-r--r--   0        0        0     7333 2024-04-29 07:57:01.589291 secretscraper-1.3.7.1/src/secretscraper/coroutinue.py
+-rw-r--r--   0        0        0    13941 2024-04-29 07:58:22.443148 secretscraper-1.3.7.1/src/secretscraper/crawler.py
+-rw-r--r--   0        0        0     1442 2024-04-29 06:01:04.289430 secretscraper-1.3.7.1/src/secretscraper/entity.py
+-rw-r--r--   0        0        0      675 2024-04-26 06:48:33.569989 secretscraper-1.3.7.1/src/secretscraper/exception.py
+-rw-r--r--   0        0        0    14024 2024-04-29 07:58:22.439882 secretscraper-1.3.7.1/src/secretscraper/facade.py
+-rw-r--r--   0        0        0     2161 2024-04-28 05:40:42.882294 secretscraper-1.3.7.1/src/secretscraper/filter.py
+-rw-r--r--   0        0        0     6527 2024-04-29 07:58:22.528282 secretscraper-1.3.7.1/src/secretscraper/handler.py
+-rw-r--r--   0        0        0     1863 2024-04-16 09:41:19.559435 secretscraper-1.3.7.1/src/secretscraper/log.py
+-rw-r--r--   0        0        0     8429 2024-04-29 07:58:22.445776 secretscraper-1.3.7.1/src/secretscraper/output_formatter.py
+-rw-r--r--   0        0        0     1438 2024-04-29 07:59:17.881407 secretscraper-1.3.7.1/src/secretscraper/scanner.py
+-rw-r--r--   0        0        0     4538 2024-04-29 07:57:20.130291 secretscraper-1.3.7.1/src/secretscraper/urlparser.py
+-rw-r--r--   0        0        0     2264 2024-04-29 08:04:46.278752 secretscraper-1.3.7.1/src/secretscraper/util.py
+-rw-r--r--   0        0        0     9086 1970-01-01 00:00:00.000000 secretscraper-1.3.7.1/PKG-INFO
```

### Comparing `secretscraper-1.3.6/LICENSE` & `secretscraper-1.3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.6/README.md` & `secretscraper-1.3.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,17 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.29 Version 1.3.7
+- Test on multiple python versions
+- Support python 3.9~3.11
 ## 2024.4.29 Version 1.3.6
 - Repackage
 
 ## 2024.4.28 Version 1.3.5
 - **New Features**
   - Support windows
   - Optimize crawler
```

### Comparing `secretscraper-1.3.6/pyproject.toml` & `secretscraper-1.3.7.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 [tool.poetry]
 name = "secretscraper"
-version = "1.3.6"
+version = "1.3.7.1"
 description = "SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression."
 readme = "README.md"
 authors = ["Padishah <straystrayer@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.11,<4.0"
+python = ">=3.9,<4.0"
 dynaconf = "^3.1.12"
 click = "^8.1.3"
 hyperscan = [
-    { version = "^0.7.7", platform = "darwin" },
-    { version = "^0.7.7", platform = "linux" }
+#    { version = "^0.7.0", platform = "darwin", python = "^3.9" },
+    { version = "^0.7.0", platform = "darwin", python = "^3.10" },
+    { version = "^0.7.7", platform = "darwin", python = "^3.11" },
+#    { version = "^0.7.0", platform = "linux", python = "^3.9" },
+    { version = "^0.7.0", platform = "linux", python = "^3.10" },
+    { version = "^0.7.7", platform = "linux", python = "^3.11" }
 ]
 bs4 = "^0.0.2"
 aiohttp = "^3.9.4"
-httpx = {extras = ["socks"], version = "^0.27.0"}
+httpx = { extras = ["socks"], version = "^0.27.0" }
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.4"
 isort = "^5.12.0"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.23.6"
 pytest-benchmark = "^4.0.0"
@@ -41,15 +45,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 [tool.pytest.ini_options]
 testpaths = "tests"
 python_files = "tests.py test_*.py *_tests.py"
 log_cli = true
-log_cli_level = "INFO"
+log_cli_level = "ERROR"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 addopts = "--durations=10 " #--full-trace --cov-report html --cov=src
 junit_duration_report = "total"
 filterwarnings = [
     "ignore"
 ]
```

### Comparing `secretscraper-1.3.6/src/secretscraper/cmdline.py` & `secretscraper-1.3.7.1/src/secretscraper/cmdline.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 @click.option("--detail", help="Show detailed result", is_flag=True)
 @click.option("-l", "--local", help="Local file or directory, scan local file/directory recursively ",
               type=click.Path(exists=True, file_okay=True, dir_okay=True, path_type=pathlib.Path))
 def main(**options):
     """Main commands"""
     if options["version"]:
         click.echo(__version__)
-        exit(1)
+        exit(0)
     if options["debug"]:
         settings.DEBUG = True
         settings.LOGLEVEL = "debug"
     if options["config"] is not None:
         if not options["config"].exists():
             click.echo(f"Error: config file not exists: {str(options['config'])}")
             return
@@ -203,12 +203,13 @@
     loaded: true
   - name: Shiro
     regex: (=deleteMe|rememberMe=)
     loaded: true
   - name: Suspicious API Key
     regex: "[\"'][0-9a-zA-Z]{32}['\"]"
     loaded: true
-"""
+""", encoding="utf8", errors="ignore"
     )
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `secretscraper-1.3.6/src/secretscraper/config/__init__.py` & `secretscraper-1.3.7.1/src/secretscraper/config/__init__.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.6/src/secretscraper/config/settings.yml` & `secretscraper-1.3.7.1/src/secretscraper/config/settings.yml`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.6/src/secretscraper/coroutinue.py` & `secretscraper-1.3.7.1/src/secretscraper/coroutinue.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     def __init__(
         self,
         num_workers: int,
         event_loop: asyncio.AbstractEventLoop,
         queue_capacity: int = 1000,
     ):
         self.event_loop = event_loop
-        self.workers: list[AsyncWorker] = []
+        self.workers: typing.List[AsyncWorker] = []
         self.num_workers: int = num_workers
         self.queue_capacity: int = queue_capacity
         self.task_queue: asyncio.Queue[AsyncTask] = asyncio.Queue(
             maxsize=self.queue_capacity
         )
 
         self.start()
@@ -99,17 +99,17 @@
         # self.event_loop.run_forever()
 
     async def submit(self, task: AsyncTask) -> asyncio.Future:
         """Submit one task"""
         await self.task_queue.put(task)
         return task.future
 
-    async def submit_all(self, tasks: list[AsyncTask]) -> list[asyncio.Future]:
+    async def submit_all(self, tasks: typing.List[AsyncTask]) -> typing.List[asyncio.Future]:
         """Submit multiple tasks"""
-        futures: list[asyncio.Future] = []
+        futures: typing.List[asyncio.Future] = []
         for task in tasks:
             await self.submit(task)
             futures.append(task.future)
         return futures
 
     async def shutdown(
         self, timeout: float = 0, cancel_queue: bool = False, cancel_tasks: bool = True
@@ -171,15 +171,15 @@
 
     async def submit(self, task: AsyncTask) -> asyncio.Future:
         """Submit one task"""
         future = await self.pool.submit(task)
         future.add_done_callback(self.done_queue.put_nowait)
         return future
 
-    async def submit_all(self, tasks: list[AsyncTask]) -> list[asyncio.Future]:
+    async def submit_all(self, tasks: typing.List[AsyncTask]) -> typing.List[asyncio.Future]:
         """Submit multiple tasks"""
         futures = await self.pool.submit_all(tasks)
         [future.add_done_callback(self.done_queue.put_nowait) for future in futures]
         return futures
 
     async def close(self) -> None:
         """Close all workers, cancel all futures that have not done"""
```

### Comparing `secretscraper-1.3.6/src/secretscraper/crawler.py` & `secretscraper-1.3.7.1/src/secretscraper/crawler.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 
 
 class Crawler:
     """Crawler interface"""
 
     def __init__(
         self,
-        start_urls: list[str],
+        start_urls: typing.List[str],
         # client: aiohttp.ClientSession,
         url_filter: URLFilter,
         parser: URLParser,
         handler: Handler,
-        # allowed_status: list[Range] = None,
+        # allowed_status: typing.List[Range] = None,
         max_page_num: int = 0,
         max_depth: int = 3,
         num_workers: int = 100,
         proxy: str = None,
         headers: dict = None,
         verbose: bool = False,
         timeout: float = 5,
         debug: bool = False,
         follow_redirects: bool = False,
-        dangerous_paths: list[str] = None,
+        dangerous_paths: typing.List[str] = None,
     ):
         """
 
         :param start_urls: urls to start crawl from
         # :param client: aiohttp client
         :param url_filter: determine whether a url should be crawled
         :param parser: extract child url nodes from html
@@ -84,22 +84,22 @@
         if self.debug:
             logger.setLevel(logging.DEBUG)
         self.follow_redirects = follow_redirects
 
         self.visited_urls: Set[URLNode] = set()
         self.found_urls: Set[URLNode] = set()  # newly found urls
         self.working_queue: queue.Queue[URLNode] = queue.Queue()  # BP queue
-        self.url_dict: dict[URLNode, set[URLNode]] = (
+        self.url_dict: typing.Dict[URLNode, typing.Set[URLNode]] = (
             dict()
         )  # url and all of its children url
-        self.js_dict: dict[URLNode, set[URLNode]] = (
+        self.js_dict: typing.Dict[URLNode, typing.Set[URLNode]] = (
             dict()
         )  # url and all of its children js
         self.total_page: int = 0  # total number of pages found, include error pages
-        self.url_secrets: dict[URLNode, set[Secret]] = (
+        self.url_secrets: typing.Dict[URLNode, typing.Set[Secret]] = (
             dict()
         )  # url and secrets found from it
         self._event_loop = asyncio.new_event_loop()
         # self.client: aiohttp.ClientSession = aiohttp.ClientSession(
         #     loop=self._event_loop
         # )  # assign event loop to client
         self.client: httpx.AsyncClient = AsyncClient(verify=False, proxies=self.proxy)
@@ -258,15 +258,15 @@
             # avoid enqueue urls with excessive depth
             # for non-html response, just record, no visit
             is_extending = True
         else:
             is_extending = False
 
         logger.debug(f"Extracting links from {url_node.url}")
-        url_children: set[URLNode] = self.parser.extract_urls(url_node, response_text)
+        url_children: typing.Set[URLNode] = self.parser.extract_urls(url_node, response_text)
         if len(url_children) > 0:
             self.url_dict[url_node] = set()
         elif is_html and (
             url_node not in self.url_dict.keys() or self.url_dict[url_node] is None
         ):
             self.url_dict[url_node] = set()
```

### Comparing `secretscraper-1.3.6/src/secretscraper/entity.py` & `secretscraper-1.3.7.1/src/secretscraper/entity.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Entity classes and factory methods."""
 
 import typing
 from dataclasses import dataclass, field
 from urllib.parse import ParseResult, urlparse
 
-URL: typing.TypeAlias = ParseResult
+try:
+    from typing import TypeAlias
+
+    URL: TypeAlias = ParseResult
+except ImportError:
+    URL = ParseResult
 
 
 @dataclass(unsafe_hash=True, eq=True)
 class URLNode:
     """URL node used in site map.
     Compare based on url_object.
     """
```

### Comparing `secretscraper-1.3.6/src/secretscraper/exception.py` & `secretscraper-1.3.7.1/src/secretscraper/exception.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.6/src/secretscraper/facade.py` & `secretscraper-1.3.7.1/src/secretscraper/facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import copy
 import functools
 import logging
 import pathlib
 import traceback
 import typing
 import warnings
-from urllib.parse import urlparse
 from collections import namedtuple
+from urllib.parse import urlparse
 
 import click
 import dynaconf
 
 from .crawler import Crawler
 from .exception import FacadeException, FileScannerException
 from .filter import (ChainedURLFilter, DomainBlackListURLFilter,
                      DomainWhiteListURLFilter)
 from .handler import get_regex_handler
 from .output_formatter import Formatter
 from .scanner import FileScanner
-from .urlparser import URLParser, RegexURLParser
+from .urlparser import RegexURLParser, URLParser
 from .util import Range, read_rules_from_setting, to_host_port
 
 logger = logging.getLogger(__name__)
 
 warnings.filterwarnings("ignore")  # ignore all warnings
 
 
@@ -54,15 +54,15 @@
 class CrawlerFacade:
     """Crawler facade"""
 
     def __init__(
         self,
         full_settings: dynaconf.Dynaconf,
         custom_settings: dict,
-        print_func: typing.Callable[[str], ...] = print,
+        print_func: typing.Callable[[str], typing.Any] = print,
     ) -> None:
         """
 
         :param full_settings: dynaconf.Dynaconf
         :param custom_settings: dict
         :param print_func: must be partial of click.echo()
         """
@@ -206,15 +206,15 @@
         )
         if outfile is not None:
             self.outfile = outfile
         print_config(f"Output file: {self.outfile}")
 
         # Status filter
         status: typing.Optional[str] = self.custom_settings.get("status", None)
-        allowed_status: typing.Optional[list[Range]] = None
+        allowed_status: typing.Optional[typing.List[Range]] = None
         if status is not None:
             for status_ex in status.split(","):
                 status_ex = status_ex.strip()
                 if status_ex.__contains__("-"):
                     min_status = status_ex.split("-")[0]
                     max_status = status_ex.split("-")[1]
                     if min_status >= max_status:
@@ -249,29 +249,29 @@
 
         # Verbose
         verbose: typing.Optional[bool] = self.custom_settings.get("verbose", None)
         if verbose is not None:
             self.settings["verbose"] = verbose
 
         # Read rules from config file
-        rules: dict[str, str] = read_rules_from_setting(self.settings)
+        rules: typing.Dict[str, str] = read_rules_from_setting(self.settings)
         handler = get_regex_handler(rules)
 
         # Read url/js regex
-        rules: list[str] = self.settings.get("urlFind")
+        rules: typing.List[str] = self.settings.get("urlFind")
         rules.extend(self.settings.get("jsFind"))
         rules_dict = {f"urlFinder_{i}": rule for i, rule in enumerate(rules)}
         parser = RegexURLParser(get_regex_handler(rules_dict, type_="regex"))
 
         # Detailed output
         if self.custom_settings.get("detail", False) is True:
             self.detail_output = True
 
         # Dangerous paths
-        dangerous_paths: list[str] = list()
+        dangerous_paths: typing.List[str] = list()
         if self.settings.get("dangerousPath", None) is not None:
             dangerous_paths.extend(set(self.settings("dangerousPath")))
 
         crawler = Crawler(
             start_urls=list(start_urls),
             url_filter=urlfilter,
             # parser=URLParser(),
@@ -282,27 +282,27 @@
             num_workers=self.settings.get("workers_num"),
             proxy=self.settings.get("proxy"),
             headers=headers,
             verbose=self.settings.get("verbose"),
             timeout=self.settings.get("timeout"),
             debug=self.debug,
             follow_redirects=self.settings["follow_redirects"],
-            dangerous_paths = dangerous_paths
+            dangerous_paths=dangerous_paths
         )
         return crawler
 
 
 class FileScannerFacade:
     """Facade for local file scanner"""
 
     def __init__(
         self,
         full_settings: dynaconf.Dynaconf,
         custom_settings: dict,
-        print_func: typing.Callable[[str], ...] = print,
+        print_func: typing.Callable[[str], typing.Any] = print,
     ):
         self.settings = full_settings
         self.custom_settings = custom_settings
         self.print_func = print_func
         self.outfile = pathlib.Path(__file__).parent / "scanner.log"
 
         self.formatter = Formatter()
@@ -340,22 +340,22 @@
             "outfile", None
         )
         if outfile is not None:
             self.outfile = outfile
         print_config(f"Output file: {self.outfile}")
 
         # Read rules from config file
-        rules: dict[str, str] = read_rules_from_setting(self.settings)
+        rules: typing.Dict[str, str] = read_rules_from_setting(self.settings)
         handler = get_regex_handler(rules)
 
         # Get all files from directory
         base: typing.Optional[pathlib.Path] = self.custom_settings.get('local', None)
         if base is None:
             raise FacadeException(f"Internal error: No base directory")
-        targets: list[pathlib.Path] = list()
+        targets: typing.List[pathlib.Path] = list()
         if base.is_file():
             targets.append(base)
         else:
             for path in base.rglob("*"):
                 if path.is_file():
                     targets.append(path)
```

### Comparing `secretscraper-1.3.6/src/secretscraper/filter.py` & `secretscraper-1.3.7.1/src/secretscraper/filter.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.6/src/secretscraper/handler.py` & `secretscraper-1.3.7.1/src/secretscraper/handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """Handler module for extracting data from HTML pages and other text files crawled from website"""
 
 import queue
 import re
 import sys
 import typing
-from typing import Protocol
+from typing import Protocol, Union
 
 from bs4 import BeautifulSoup, NavigableString, Tag
 
 from secretscraper.entity import Secret
 from secretscraper.exception import HandlerException
 
 # T = typing.TypeVar("T")
 # IterableAsyncOrSync: typing.TypeAlias = typing.Iterable[T] | typing.AsyncIterable[T]
-BSResult = Tag | NavigableString | None
+BSResult = Union[Tag, NavigableString, None]
 
 
 class Handler(Protocol):
     """Base class for different types of handlers"""
 
     def handle(self, text: str) -> typing.Iterable[Secret]: ...
 
 
 class ReRegexHandler(Handler):
     """ Regex handler using the `re` module, simple but have lowest performance."""
 
-    def __init__(self, rules: dict[str, str], flags: int = 0):
+    def __init__(self, rules: typing.Dict[str, str], flags: int = 0):
         """
 
         :param rules: rules dictionary with keys indicating type and values indicating the regex
         """
         self.types = list(rules.keys())
         regexes = list(rules.values())
-        self.regexes: list[re.Pattern] = list()
+        self.regexes: typing.List[re.Pattern] = list()
         for regex in regexes:
             self.regexes.append(re.compile(regex, flags=flags | re.IGNORECASE))
 
     def handle(self, text: str) -> typing.Iterable[Secret]:
         """Extract secret data"""
-        result_list: list[Secret] = list()
+        result_list: typing.List[Secret] = list()
         for index, regex in enumerate(self.regexes):
             # match = regex.search(text)
             # if match is not None:
             #     secret_data = match.group(0)
             #     secret_type = self.types[index]
             #     secret = Secret(type=secret_type, data=secret_data)
             #     result_list.append(secret)
@@ -54,45 +54,48 @@
                     secret = Secret(type=secret_type, data=secret_data)
                     result_list.append(secret)
         return result_list
 
 
 if not sys.platform.startswith("win"):
     # hyperscan does not support windows
-    import hyperscan
+    try:
+        import hyperscan
+    except ImportError:
+        hyperscan = None
 
 
     class HyperscanRegexHandler(Handler):
         """Regex handler using `hyperscan` module"""
 
         def __init__(
-            self, rules: dict[str, str], lazy_init: bool = False, hs_flag: int = 0
+            self, rules: typing.Dict[str, str], lazy_init: bool = False, hs_flag: int = 0
         ):
             """
 
             :param rules: regex rules dictionary with keys indicating type and values indicating the regex
             :param lazy_init: True for deferring the initialization to actively call the init() method, otherwise initialize immediately
             :param hs_flag: hyperscan flag perform to every expressions
             """
             # self.output_queue: queue.Queue[Secret] = queue.Queue()
             self.rules = rules
             self._init: bool = False
             self._hs_flag: int = (
                 hs_flag | hyperscan.HS_FLAG_SOM_LEFTMOST | hyperscan.HS_FLAG_CASELESS
             )
             self._db: typing.Optional[hyperscan.Database] = None
-            self.patterns: dict[int, bytes] = dict()  # pattern id => regex in bytes
-            self.types: dict[int, str] = dict()  # pattern id => type
+            self.patterns: typing.Dict[int, bytes] = dict()  # pattern id => regex in bytes
+            self.types: typing.Dict[int, str] = dict()  # pattern id => type
             if not lazy_init:
                 self.init()
 
         def init(self):
             """Initialize the hyperscan database."""
             self._db = hyperscan.Database()
-            flags: list[int] = [self._hs_flag for _ in range(len(self.rules))]
+            flags: typing.List[int] = [self._hs_flag for _ in range(len(self.rules))]
             for index, type_str in enumerate(self.rules):
                 regex = self.rules.get(type_str)
                 self.patterns[index] = regex.encode("utf-8")
                 self.types[index] = type_str
 
             self._db.compile(
                 expressions=list(self.patterns.values()),
@@ -107,15 +110,15 @@
             """Extract secret data via the pre-compiled hyperscan database
 
             This method is IO-bound.
             """
             if not self._init:
                 raise HandlerException("Hyperscan database is not initialized")
 
-            results: list[Secret] = list()
+            results: typing.List[Secret] = list()
 
             def on_match(
                 id: int,
                 froms: int,
                 to: int,
                 flags: int,
                 context: typing.Optional[typing.Any] = None,
@@ -131,37 +134,43 @@
             return results
 
 
 class BSHandler(Handler):
     """BeautifulSoup handler that filter html elements on demand"""
 
     def __init__(
-        self, filter_func: typing.Callable[[BeautifulSoup], list[BSResult]]
+        self, filter_func: typing.Callable[[BeautifulSoup], typing.List[BSResult]]
     ) -> None:
         self.filter = filter_func
 
     def handle(self, text: str) -> typing.Iterable[Secret]:
         """Extract secret data via filter
 
         :type text: str
         :param text: should be in html format
         """
         soup = BeautifulSoup(text, "html.parser")
-        result: list[BSResult] = self.filter(soup)
-        results: list[Secret] = list()
+        result: typing.List[BSResult] = self.filter(soup)
+        results: typing.List[Secret] = list()
         if result is not None:
             secret = Secret(type="HTML Element", data=result)
             results.append(secret)
         return results
 
 
-def get_regex_handler(rules: dict[str, str], type_: str = "", *args, **kwargs) -> Handler:
+def get_regex_handler(rules: typing.Dict[str, str], type_: str = "", *args, **kwargs) -> Handler:
     """Return regex handler on current platform"""
     if len(type_) == 0:
-        if sys.platform.startswith("win"):
+        is_hyperscan = False
+        try:
+            import hyperscan
+            is_hyperscan = True
+        except ImportError:
+            is_hyperscan = False
+        if sys.platform.startswith("win") or not is_hyperscan:
             return ReRegexHandler(rules, *args, **kwargs)
         else:
             return HyperscanRegexHandler(rules, *args, **kwargs)
     else:
         if type == "regex":
             return ReRegexHandler(rules, *args, **kwargs)
         elif type == "hyperscan":
```

### Comparing `secretscraper-1.3.6/src/secretscraper/log.py` & `secretscraper-1.3.7.1/src/secretscraper/log.py`

 * *Files identical despite different names*

### Comparing `secretscraper-1.3.6/src/secretscraper/output_formatter.py` & `secretscraper-1.3.7.1/src/secretscraper/output_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 
 class Formatter:
     """Colorful output for terminal and non-colorful output for out-file"""
 
     def __init__(
         self,
-        allowed_status: list[Range] = None,
+        allowed_status: typing.List[Range] = None,
     ) -> None:
         """
 
         :param allowed_status: filter response status. None for display all
         """
         self._allowed_status = allowed_status
 
     @property
-    def allowed_status(self) -> list[Range]:
+    def allowed_status(self) -> typing.List[Range]:
         return self._allowed_status
 
     @allowed_status.setter
-    def allowed_status(self, allowed_status: list[Range]):
+    def allowed_status(self, allowed_status: typing.List[Range]):
         self._allowed_status = allowed_status
 
     def format_colorful_status(self, status: str) -> str:
         try:
             status = int(status)
         except Exception:
             return status
@@ -82,15 +82,15 @@
             result = f"\n{len(urls)} Domains:\n{found_urls_str}\n"
             click.echo(f"{len(urls)} Domains:")
             click.echo(self.format_normal_result(f"{found_urls_str}"))
             click.echo("")
             return result
 
     def output_url_hierarchy(
-        self, url_dict: dict[URLNode, typing.Iterable[URLNode]], is_print: bool = False
+        self, url_dict: typing.Dict[URLNode, typing.Iterable[URLNode]], is_print: bool = False
     ) -> str:
         """Output the url hierarchy"""
         if not is_print:
             url_hierarchy = ""
             for base, urls in url_dict.items():
                 url_set = {
                     f"{str(url.url)} [{str(url.response_status)}]"
@@ -118,19 +118,19 @@
                     + self.format_colorful_status(base.response_status)
                     + f"] (depth:{base.depth}):\n{urls_str}"
                 )
 
             return url_hierarchy
 
     def output_url_per_domain(
-        self, domains: set[str], url_dict: dict[URLNode, typing.Iterable[URLNode]], url_type: str = "URL"
+        self, domains: typing.Set[str], url_dict: typing.Dict[URLNode, typing.Iterable[URLNode]], url_type: str = "URL"
     ) -> str:
         """Output the URLs for differenct domains"""
         url_hierarchy = ""
-        domain_secrets: dict[str, list[URLNode]] = dict()
+        domain_secrets: typing.Dict[str, typing.List[URLNode]] = dict()
         for base, urls in url_dict.items():
             domain, _ = to_host_port(base.url_object.netloc)
             if domain not in domains:
                 domain = "Other"
             if domain not in domain_secrets:
                 domain_secrets[domain] = list()
             domain_secrets[domain].extend(list(urls))
@@ -148,15 +148,15 @@
             urls_str = "\n".join(url_set)
             url_hierarchy += f"\n{len(url_set)} {url_type} from {domain}:\n{urls_str}\n"
         click.echo(url_hierarchy)
 
         return url_hierarchy
 
     def output_js(
-        self, js_dict: dict[URLNode, typing.Iterable[URLNode]], is_print: bool = False
+        self, js_dict: typing.Dict[URLNode, typing.Iterable[URLNode]], is_print: bool = False
     ) -> str:
         """Output the url hierarchy"""
         if is_print:
             js_str = ""
             for base, urls in js_dict.items():
                 url_set = {
                     f"{str(url.url)} [{str(url.response_status)}]"
@@ -178,18 +178,18 @@
                     if self.filter(url)
                 }
                 urls_str = "\n".join(url_set)
                 js_str += f"\n{len(url_set)} JS from {base.url}:\n{urls_str}\n"
             return js_str
 
     def output_secrets(
-        self, url_secrets: dict[URLNode, typing.Iterable[Secret]]
+        self, url_secrets: typing.Dict[URLNode, typing.Iterable[Secret]]
     ) -> str:
         """Output all secrets found
-        :type secrets: dict[str, set[Secret]]
+        :type secrets: typing.Dict[str, typing.Set[Secret]]
         :param secrets: dict keys indicate url and values indicate the secrets found from the url
 
         """
         url_secrets_str = ""
         if len(url_secrets.values()) == 0:
             return "No secrets found.\n"
         for url, secrets in url_secrets.items():
@@ -197,15 +197,15 @@
                 secret_set = {
                     f"{str(secret.type)}: {str(secret.data)}" for secret in secrets
                 }
                 secrets_str = "\n".join(secret_set)
                 url_secrets_str += f"\n{len(secret_set)} Secrets found in {url.url} [{self.format_colorful_status(str(url.response_status))}]:\n{secrets_str}\n"
         return url_secrets_str
 
-    def output_local_scan_secrets(self, path_secrets: dict[pathlib.Path, typing.Iterable[Secret]]) -> str:
+    def output_local_scan_secrets(self, path_secrets: typing.Dict[pathlib.Path, typing.Iterable[Secret]]) -> str:
         """Display all secrets found in local file"""
         if len(path_secrets) == 0:
             click.echo("No secrets found.\n")
         result = ""
         for path, secrets in path_secrets.items():
             if secrets is not None and len(list(secrets)) > 0:
                 secret_set = {
```

### Comparing `secretscraper-1.3.6/src/secretscraper/scanner.py` & `secretscraper-1.3.7.1/src/secretscraper/scanner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 """Local file scanner, find secrets within local files"""
 import logging
 import mimetypes
 import pathlib
+import typing
 
 from .entity import Secret
 from .exception import FileScannerException
 from .handler import Handler
 
 logger = logging.getLogger(__name__)
 
 
 class FileScanner:
     """Extract secrets from local files"""
 
     def __init__(
         self,
-        targets: list[pathlib.Path],
+        targets: typing.List[pathlib.Path],
         handler: Handler,
     ):
         """
 
         :param targets: target files to scan
         :param handler:
         :param verbose:
         """
         self.targets = targets
         self.handler = handler
 
-        self.secrets: dict[pathlib.Path, set[Secret]] = {}
+        self.secrets: typing.Dict[pathlib.Path, typing.Set[Secret]] = {}
 
     def start(self):
         """Start scanning"""
 
         for file in self.targets:
             if not file.exists():
                 raise FileScannerException(f"Fail to open {file.name}")
             if not file.is_file():
                 raise FileScannerException(f"Internal error: got a directory: {file.name}")
             # pass non-text file
             content: str = file.read_text(encoding="utf8", errors="ignore")
             logger.debug(f"Read file content: {len(content)}bytes from {file.name}")
-            secrets: set[Secret] = set(list(self.handler.handle(content)))
+            secrets: typing.Set[Secret] = set(list(self.handler.handle(content)))
             if len(secrets) > 0:
                 self.secrets[file] = secrets
                 logger.debug(f"Found {len(secrets)} secrets from {file.name}")
```

### Comparing `secretscraper-1.3.6/src/secretscraper/urlparser.py` & `secretscraper-1.3.7.1/src/secretscraper/urlparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Extract URL nodes in HTML page."""
 
 from typing import Set
 from urllib.parse import ParseResult, urlparse
 
 from bs4 import BeautifulSoup
 
+from .entity import URL, Secret, URLNode
 from .handler import Handler
-from .entity import URL, URLNode, Secret
 from .util import is_static_resource, sanitize_url
 
 
 class URLParser:
     """Extract URL nodes in HTML"""
 
     def __init__(self):
@@ -103,15 +103,15 @@
         super().__init__()
 
     def extract_urls(self, base_url: URLNode, text: str) -> Set[URLNode]:
         """Extract URLs via regex and HTML node"""
         found_urls: Set[URLNode] = set()
         current_depth = base_url.depth + 1
 
-        links: set[Secret] = set(self.handler.handle(text))
+        links: typing.Set[Secret] = set(self.handler.handle(text))
         for link in links:
             link = link.data
             if len(link) == 0:
                 continue
             obj = urlparse(link)
             # ignore static resource
             if is_static_resource(obj.path):
```

### Comparing `secretscraper-1.3.6/src/secretscraper/util.py` & `secretscraper-1.3.7.1/src/secretscraper/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Common utility functions."""
 
-from collections import namedtuple
 import re
+import typing
+from collections import namedtuple
 from urllib.parse import urlparse
 
-from dynaconf import LazySettings
+# from dynaconf import LazySettings
 
 from .entity import URL
 from .exception import SecretScraperException
 
 Range = namedtuple("Range", ["start", "end"])
 
 
-def read_rules_from_setting(settings: LazySettings) -> dict[str, str]:
+def read_rules_from_setting(settings) -> typing.Dict[str, str]:
     """Read rules from settings
 
     :param settings: Dynaconf settings
-    :return dict[str, str]: key for rule name and value for regex literal
+    :return typing.Dict[str, str]: key for rule name and value for regex literal
     """
     rules_dict = dict()
     try:
         rules = settings.RULES
         for rule in rules:
             name = rule.get("name")
             regex = rule.get("regex")
@@ -39,15 +40,15 @@
     exts = ['.png', '.jpg', '.jpeg', '.gif', '.css', '.ico', ".dtd", '.svg']
     for ext in exts:
         if path.endswith(ext):
             return True
     return False
 
 
-def to_host_port(netloc: str) -> tuple[str, str]:
+def to_host_port(netloc: str) -> typing.Tuple[str, str]:
     """Convert netloc to host and port"""
     r = netloc.split(":")
     if len(r) == 1:
         return r[0], ""
     if len(r) == 2:
         return r[0].strip(), r[1].strip()
     return '', ''
@@ -70,7 +71,16 @@
     try:
         obj = urlparse(url)
         if obj.netloc.startswith("127.0.0.1") or obj.netloc.startswith("localhost"):
             return ""
     except:
         pass
     return url
+
+
+def is_hyperscan() -> bool:
+    """Check if hyperscan is usable"""
+    try:
+        import hyperscan
+        return True
+    except ImportError:
+        return False
```

### Comparing `secretscraper-1.3.6/PKG-INFO` & `secretscraper-1.3.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: secretscraper
-Version: 1.3.6
+Version: 1.3.7.1
 Summary: SecretScraper is a web scraper tool that can scrape the content through target websites and extract secret information via regular expression.
 License: MIT
 Author: Padishah
 Author-email: straystrayer@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.4,<4.0.0)
 Requires-Dist: bs4 (>=0.0.2,<0.0.3)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dynaconf (>=3.1.12,<4.0.0)
 Requires-Dist: httpx[socks] (>=0.27.0,<0.28.0)
-Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; sys_platform == "darwin"
-Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; sys_platform == "linux"
+Requires-Dist: hyperscan (>=0.7.0,<0.8.0) ; python_version >= "3.10" and python_version < "4.0" and sys_platform == "darwin"
+Requires-Dist: hyperscan (>=0.7.0,<0.8.0) ; python_version >= "3.10" and python_version < "4.0" and sys_platform == "linux"
+Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; python_version >= "3.11" and python_version < "4.0" and sys_platform == "darwin"
+Requires-Dist: hyperscan (>=0.7.7,<0.8.0) ; python_version >= "3.11" and python_version < "4.0" and sys_platform == "linux"
 Description-Content-Type: text/markdown
 
 # SecretScraper
 
 ![Tests](https://github.com/PadishahIII/SecretScraper/actions/workflows/main.yml/badge.svg)
 
 ## Overview
@@ -227,14 +231,17 @@
 - [x] Support windows
 - [x] Scan local file
 - [x] Extract links via regex
 
 ---
 
 # Change Log
+## 2024.4.29 Version 1.3.7
+- Test on multiple python versions
+- Support python 3.9~3.11
 ## 2024.4.29 Version 1.3.6
 - Repackage
 
 ## 2024.4.28 Version 1.3.5
 - **New Features**
   - Support windows
   - Optimize crawler
```

