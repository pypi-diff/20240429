# Comparing `tmp/matricula_online_scraper-0.2.2.tar.gz` & `tmp/matricula_online_scraper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matricula_online_scraper-0.2.2.tar", max compression
+gzip compressed data, was "matricula_online_scraper-0.3.0.tar", max compression
```

## Comparing `matricula_online_scraper-0.2.2.tar` & `matricula_online_scraper-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1069 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/LICENSE
--rw-r--r--   0        0        0     2337 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/__init__.py
--rw-r--r--   0        0        0       65 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/__main__.py
--rw-r--r--   0        0        0        0 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/cli/__init__.py
--rw-r--r--   0        0        0     5816 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/cli/fetch.py
--rw-r--r--   0        0        0      707 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/cli/utils.py
--rwxr-xr-x   0        0        0     1123 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/main.py
--rw-r--r--   0        0        0        0 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/__init__.py
--rw-r--r--   0        0        0     3191 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/locations_spider.py
--rw-r--r--   0        0        0     4000 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/parish_registers_spider.py
--rw-r--r--   0        0        0      856 2024-04-26 09:00:25.992085 matricula_online_scraper-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 matricula_online_scraper-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2337 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/cli/__init__.py
+-rw-r--r--   0        0        0     2065 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/cli/common.py
+-rw-r--r--   0        0        0     5772 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/cli/fetch.py
+-rw-r--r--   0        0        0      707 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/cli/utils.py
+-rwxr-xr-x   0        0        0     1123 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/main.py
+-rw-r--r--   0        0        0        0 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/spiders/__init__.py
+-rw-r--r--   0        0        0     3191 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/spiders/locations_spider.py
+-rw-r--r--   0        0        0     4000 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/matricula_online_scraper/spiders/parish_registers_spider.py
+-rw-r--r--   0        0        0      856 2024-04-29 05:46:03.314635 matricula_online_scraper-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 matricula_online_scraper-0.3.0/PKG-INFO
```

### Comparing `matricula_online_scraper-0.2.2/LICENSE` & `matricula_online_scraper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.2.2/README.md` & `matricula_online_scraper-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.2.2/matricula_online_scraper/cli/fetch.py` & `matricula_online_scraper-0.3.0/matricula_online_scraper/cli/fetch.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,29 +8,36 @@
 from scrapy import crawler  # pylint: disable=import-error # type: ignore
 from rich import print  # pylint: disable=redefined-builtin
 from matricula_online_scraper.spiders.locations_spider import LocationsSpider
 from matricula_online_scraper.spiders.parish_registers_spider import (
     ParishRegistersSpider,
 )
 from .utils import URL
+from .common import (
+    DEFAULT_SCRAPER_LOG_LEVEL,
+    DEFAULT_SCRAPER_SILENT,
+    DEFAULT_OUTPUT_FILE_FORMAT,
+    DEFAUL_APPEND,
+    LogLevelOption,
+    OutputFileNameArgument,
+    OutputFileFormatOption,
+    SilentOption,
+    AppendOption,
+    file_format_to_scrapy,
+)
 
-app = typer.Typer()
-
-SilentOption = Annotated[
-    bool, typer.Option(help="Disable all output from the scraper.")
-]
-DEFAULT_SCRAPER_SILENT = True
 
-LogLevelOption = Annotated[str, typer.Option(help="Set the log level for the crawler.")]
-DEFAULT_SCRAPER_LOG_LEVEL = "ERROR"
+app = typer.Typer()
 
 
 @app.command()
 def location(
-    output_file: Annotated[Path, typer.Argument()],
+    output_file_name: OutputFileNameArgument = Path("matricula_locations"),
+    output_file_format: OutputFileFormatOption = DEFAULT_OUTPUT_FILE_FORMAT,
+    append: AppendOption = DEFAUL_APPEND,
     place: Annotated[
         Optional[str], typer.Option(help="Full text search for a location.")
     ] = None,
     diocese: Annotated[
         Optional[int],
         typer.Option(
             help="Enum value of the diocese. (See their website for the list of dioceses.)"
@@ -54,30 +61,23 @@
 
     If none of the search parameters are provided, all available locations will be scraped.
 
     Example:
     >>> matricula-online-scraper fetch location ./output.jsonl
     """
 
-    # user specified only a filename, not a complete path
-    if output_file.suffix == "":
-        print(f"[yellow]Output file has no type suffix: {output_file}[/yellow]")
-        output_file = output_file.with_suffix(".jsonl")
-        print(
-            f"Adding '.jsonl' suffix to the output file. New path: {output_file.absolute()}"
-        )
-
-    # atm only jsonl is supported
-    if output_file.suffix != ".jsonl":
-        print(f"[red]Output file type must be '.jsonl': {output_file}[/red]")
-        raise typer.Exit()
+    output_path_str = str(output_file_name.absolute()) + "." + output_file_format
+    output_path = Path(output_path_str)
 
     # check if output file already exists
-    if output_file.exists():
-        print(f"[red]Output file already exists: {output_file.absolute()}[/red]")
+    if output_path.exists() and not append:
+        print(
+            f"[red]Output file already exists: {output_path.absolute()}."
+            " Use the option '--append' if you want to append to the file.[/red]"
+        )
         raise typer.Exit()
 
     # all search parameters are unused => fetching everything takes some time
     if (
         place is None
         or place == ""
         and diocese is None
@@ -88,15 +88,19 @@
             "[yellow]No search parameters provided. Fetching all available locations."
             "This might take some time.[/yellow]"
         )
 
     try:
         process = crawler.CrawlerProcess(
             settings={
-                "FEEDS": {str(output_file.absolute()): {"format": "jsonlines"}},
+                "FEEDS": {
+                    str(output_path.absolute()): {
+                        "format": file_format_to_scrapy(output_file_format)
+                    }
+                },
                 "LOG_LEVEL": log_level,
                 "LOG_ENABLED": not silent,
             },
         )
 
         process.crawl(  # type: ignore
             LocationsSpider,
@@ -105,71 +109,70 @@
             date_filter=date_filter,
             date_range=date_range or (0, 9999),
         )
         process.start()
 
         print(
             "[green]Scraping completed successfully. "
-            f"Output saved to: {output_file.absolute()}[/green]"
+            f"Output saved to: {output_path.absolute()}[/green]"
         )
 
     except Exception as exception:
         print("[red]An unknown error occurred while scraping.[/red]")
         raise typer.Exit(code=1) from exception
 
 
 @app.command()
 def parish(
-    output_file: Annotated[Path, typer.Argument()],
     urls: Annotated[
         List[URL],
         typer.Option("--url", "-u", parser=URL, help="One ore more URLs to scrape."),
     ],
+    output_file_name: OutputFileNameArgument = Path("matricula_parishes"),
+    output_file_format: OutputFileFormatOption = DEFAULT_OUTPUT_FILE_FORMAT,
+    append: AppendOption = DEFAUL_APPEND,
     log_level: LogLevelOption = DEFAULT_SCRAPER_LOG_LEVEL,
     silent: SilentOption = DEFAULT_SCRAPER_SILENT,
 ):
     """
     Scrape a parish register
     """
 
-    # user specified only a filename, not a complete path
-    if output_file.suffix == "":
-        print(f"[yellow]Output file has no type suffix: {output_file}[/yellow]")
-        output_file = output_file.with_suffix(".jsonl")
-        print(
-            f"Adding '.jsonl' suffix to the output file. New path: {output_file.absolute()}"
-        )
-
-    # atm only jsonl is supported
-    if output_file.suffix != ".jsonl":
-        print(f"[red]Output file type must be '.jsonl': {output_file}[/red]")
-        raise typer.Exit()
+    output_path_str = str(output_file_name.absolute()) + "." + output_file_format
+    output_path = Path(output_path_str)
 
     # check if output file already exists
-    if output_file.exists():
-        print(f"[red]Output file already exists: {output_file.absolute()}[/red]")
+    if output_path.exists() and not append:
+        print(
+            f"[red]Output file already exists: {output_path.absolute()}."
+            " Use the option '--append' if you want to append to the file.[/red]"
+        )
         raise typer.Exit()
 
     if len(urls) <= 0:
         print("[red]No URLs provided to scrape.[/red]")
         raise typer.Exit()
 
     try:
         process = crawler.CrawlerProcess(
             settings={
-                "FEEDS": {str(output_file.absolute()): {"format": "jsonlines"}},
+                "FEEDS": {
+                    str(output_path.absolute()): {
+                        "format": file_format_to_scrapy(output_file_format)
+                    }
+                },
                 "LOG_LEVEL": log_level,
                 "LOG_ENABLED": not silent,
             }
         )
 
         process.crawl(ParishRegistersSpider, start_urls=[str(url) for url in urls])  # type: ignore
         process.start()
 
         print(
             "[green]Scraping completed successfully. "
-            f"Output saved to: {output_file.absolute()}[/green]"
+            f"Output saved to: {output_path.absolute()}[/green]"
         )
 
     except Exception as exception:
         print("[red]An unknown error occurred while scraping.[/red]")
         raise typer.Exit(code=1) from exception
```

### Comparing `matricula_online_scraper-0.2.2/matricula_online_scraper/cli/utils.py` & `matricula_online_scraper-0.3.0/matricula_online_scraper/cli/utils.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.2.2/matricula_online_scraper/main.py` & `matricula_online_scraper-0.3.0/matricula_online_scraper/main.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/locations_spider.py` & `matricula_online_scraper-0.3.0/matricula_online_scraper/spiders/locations_spider.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.2.2/matricula_online_scraper/spiders/parish_registers_spider.py` & `matricula_online_scraper-0.3.0/matricula_online_scraper/spiders/parish_registers_spider.py`

 * *Files identical despite different names*

### Comparing `matricula_online_scraper-0.2.2/pyproject.toml` & `matricula_online_scraper-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matricula-online-scraper"
-version = "0.2.2"
+version = "0.3.0"
 description = "Command Line Interface tool for scraping Matricula Online https://data.matricula-online.eu."
 repository = "https://github.com/lsg551/matricula-online-scraper"
 authors = ["Luis Schulte"]
 license = "MIT"
 readme = "README.md"
 keywords = ["matricula-online", "matricula", "scraper", "parish-registers"]
 classifiers = [
```

### Comparing `matricula_online_scraper-0.2.2/PKG-INFO` & `matricula_online_scraper-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matricula-online-scraper
-Version: 0.2.2
+Version: 0.3.0
 Summary: Command Line Interface tool for scraping Matricula Online https://data.matricula-online.eu.
 Home-page: https://github.com/lsg551/matricula-online-scraper
 License: MIT
 Keywords: matricula-online,matricula,scraper,parish-registers
 Author: Luis Schulte
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 3 - Alpha
```

