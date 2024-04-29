# Comparing `tmp/progress-table-2.1.0.tar.gz` & `tmp/progress-table-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-2.1.0.tar", last modified: Sun Apr 28 20:33:36 2024, max compression
+gzip compressed data, was "progress-table-2.2.0.tar", last modified: Mon Apr 29 17:54:07 2024, max compression
```

## Comparing `progress-table-2.1.0.tar` & `progress-table-2.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.130510 progress-table-2.1.0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.1.0/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-28 20:33:36.130510 progress-table-2.1.0/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4139 2024-04-28 20:30:22.000000 progress-table-2.1.0/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.127176 progress-table-2.1.0/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-28 20:30:31.000000 progress-table-2.1.0/progress_table/__init__.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.127176 progress-table-2.1.0/progress_table/v0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.1.0/progress_table/v0/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.1.0/progress_table/v0/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.1.0/progress_table/v0/symbols.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.127176 progress-table-2.1.0/progress_table/v1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.1.0/progress_table/v1/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    46788 2024-04-28 20:30:31.000000 progress-table-2.1.0/progress_table/v1/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     5390 2024-04-28 20:30:31.000000 progress-table-2.1.0/progress_table/v1/styles.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.130510 progress-table-2.1.0/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.1.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      593 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.1.0/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-28 20:33:36.130510 progress-table-2.1.0/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-09 23:00:39.000000 progress-table-2.1.0/setup.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.130510 progress-table-2.1.0/tests/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.1.0/tests/test_docs_automated.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-28 20:30:31.000000 progress-table-2.1.0/tests/test_examples_automated.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.2.0/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-29 17:54:07.200280 progress-table-2.2.0/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4139 2024-04-28 20:30:22.000000 progress-table-2.2.0/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-29 17:54:03.000000 progress-table-2.2.0/progress_table/__init__.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/progress_table/v0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.2.0/progress_table/v0/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.2.0/progress_table/v0/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.2.0/progress_table/v0/symbols.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/progress_table/v1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.2.0/progress_table/v1/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1500 2024-04-29 17:54:03.000000 progress-table-2.2.0/progress_table/v1/common.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    46305 2024-04-29 17:54:03.000000 progress-table-2.2.0/progress_table/v1/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     7400 2024-04-29 17:54:03.000000 progress-table-2.2.0/progress_table/v1/styles.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.2.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      621 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-29 17:54:07.000000 progress-table-2.2.0/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.2.0/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-29 17:54:07.200280 progress-table-2.2.0/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-09 23:00:39.000000 progress-table-2.2.0/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-29 17:54:07.200280 progress-table-2.2.0/tests/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.2.0/tests/test_docs_automated.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-28 20:30:31.000000 progress-table-2.2.0/tests/test_examples_automated.py
```

### Comparing `progress-table-2.1.0/LICENSE.txt` & `progress-table-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.1.0/PKG-INFO` & `progress-table-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.1.0
+Version: 2.2.0
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-2.1.0/README.md` & `progress-table-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `progress-table-2.1.0/progress_table/v0/progress_table.py` & `progress-table-2.2.0/progress_table/v0/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.1.0/progress_table/v0/symbols.py` & `progress-table-2.2.0/progress_table/v0/symbols.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.1.0/progress_table/v1/progress_table.py` & `progress-table-2.2.0/progress_table/v1/progress_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,38 +8,21 @@
 import math
 import os
 import shutil
 import sys
 import time
 from dataclasses import dataclass
 from threading import Thread
-from typing import Any, Callable, Iterable, Sized, Type, Union
+from typing import Any, Callable, Iterable, Sized, Type
 
-from colorama import Back, Fore, Style
+from colorama import Style
 
-from . import styles
-
-ALL_COLOR_NAME = [x for x in dir(Fore) if not x.startswith("__")]
-ALL_STYLE_NAME = [x for x in dir(Style) if not x.startswith("__")]
-ALL_COLOR_STYLE_NAME = ALL_COLOR_NAME + ALL_STYLE_NAME
-
-ALL_COLOR = [getattr(Fore, x) for x in ALL_COLOR_NAME] + [getattr(Back, x) for x in ALL_COLOR_NAME]
-ALL_STYLE = [getattr(Style, x) for x in ALL_STYLE_NAME]
-ALL_COLOR_STYLE = ALL_COLOR + ALL_STYLE
-
-COLORAMA_TRANSLATE = {
-    "bold": "bright",
-}
-
-NoneType = type(None)
-ColorFormat = Union[str, tuple, list, NoneType]
-ColorFormatTuple = (str, tuple, list, NoneType)
-
-EPS = 1e-9
-CURSOR_UP = "\033[A"
+from progress_table.v1 import styles
+from progress_table.v1.common import CURSOR_UP, ColorFormat, ColorFormatTuple, maybe_convert_to_colorama
+from progress_table.v1.styles import parse_pbar_style
 
 # Flags that indicate if the warning was already triggered
 WARNED_PBAR_HIDDEN = False
 
 ################
 ## V2 version ##
 ################
@@ -87,37 +70,14 @@
             return aggregate_min
         else:
             raise ValueError(f"Unknown aggregate type string: {aggregate}")
     else:
         raise ValueError(f"Unknown aggregate type: {type(aggregate)}")
 
 
-def maybe_convert_to_colorama_str(color: str) -> str:
-    # Translation layer to fix unintuitive colorama names
-    color = COLORAMA_TRANSLATE.get(color.lower(), color)
-
-    if isinstance(color, str):
-        if hasattr(Fore, color.upper()):
-            return getattr(Fore, color.upper())
-        if hasattr(Style, color.upper()):
-            return getattr(Style, color.upper())
-
-    assert color in ALL_COLOR_STYLE, f"Color {color!r} incorrect! Available: {' '.join(ALL_COLOR_STYLE_NAME)}"
-    return color
-
-
-def maybe_convert_to_colorama(color: ColorFormat) -> str:
-    if color is None or color == "":
-        return ""
-    if isinstance(color, str):
-        color = color.split(" ")
-    results = [maybe_convert_to_colorama_str(x) for x in color]
-    return "".join(results)
-
-
 def get_default_format_func(decimal_places):
     def fmt(x) -> str:
         if isinstance(x, int):
             return str(x)
         else:
             try:
                 return format(x, f".{decimal_places}f")
@@ -154,22 +114,20 @@
         default_header_color: ColorFormat = None,
         default_row_color: ColorFormat = None,
         pbar_show_throughput: bool = True,
         pbar_show_progress: bool = False,
         pbar_show_percents: bool = False,
         pbar_show_eta: bool = False,
         pbar_embedded: bool = True,
-        pbar_color_filled: ColorFormat = None,
-        pbar_color_empty: ColorFormat = None,
+        pbar_style: str | Type[styles.PbarStyleBase] = "square",
+        pbar_style_embed: str | Type[styles.PbarStyleBase] = "embed",
         print_header_on_top: bool = True,
         print_header_every_n_rows: int = 30,
         custom_cell_format: Callable[[Any], str] | None = None,
         table_style: str | Type[styles.TableStyleBase] = "round",
-        pbar_style: str | Type[styles.PbarStyleBase] = "normal",
-        pbar_style_embed: str | Type[styles.PbarStyleBase] = "embed",
         file=None,
         # Deprecated arguments
         custom_format: None = None,
         embedded_progress_bar: None = None,
         print_row_on_update: None = None,
     ):
         """Progress Table instance.
@@ -213,16 +171,14 @@
             pbar_show_progress: Show progress in the progress bar, for example 10/40. Defaults to True.
             pbar_show_percents: Show percents in the progress bar, for example 25%. Defaults to False.
             pbar_show_eta: Show estimated time of finishing in the progress bar, for example 10s. Defaults to False.
             pbar_embedded: If True, changes the way the first (non-nested) progress bar looks.
                            Embedded version is more subtle, but does not prevent the current row from being displayed.
                            If False, the progress bar covers the current row, preventing the user from seeing values
                            that are being updated until the progress bar finishes. The default is True.
-            pbar_color_filled: Default color of the filled part of the progress bars.
-            pbar_color_empty: Default color of the empty part of the progress bars.
             print_header_every_n_rows: 30 by default. When table has a lot of rows, it can be useful to remind what the header is.
                                        If True, hedaer will be displayed periodically after the selected number of rows. 0 to supress.
             custom_cell_format: A function that defines how to get str value to display from a cell content.
                                 This function should be universal and work for all datatypes as inputs.
                                 It takes one value as an input and returns string as an output.
             table_style: Change the borders of the table. Either a string or 'TableStyleBase' type class.
             pbar_style: Change the style of the progress bar. Either a string or 'PbarStyleBase' type class.
@@ -234,23 +190,22 @@
         if custom_format is not None:
             logging.warning("Argument `custom_format` is deprecated. Use `custom_cell_format` instead!")
         if embedded_progress_bar is not None:
             logging.warning("Argument `embedded_progress_bar` is deprecated. Use `pbar_embedded` instead!")
         if print_row_on_update is not None:
             logging.warning("Argument `print_row_on_update` is deprecated. Specify `interactive` instead!")
 
-        self.table_style = styles.figure_table_style(table_style)
-        self.pbar_style = styles.figure_pbar_style(pbar_style)
-        self.pbar_style_embed = styles.figure_pbar_style(pbar_style_embed)
+        self.table_style = styles.parse_table_style(table_style)
+
+        self.pbar_style = styles.parse_pbar_style(pbar_style)
+        self.pbar_style_embed = styles.parse_pbar_style(pbar_style_embed)
 
         assert isinstance(default_row_color, ColorFormatTuple), "Row color has to be a color format!"  # type: ignore
         assert isinstance(default_column_color, ColorFormatTuple), "Column color has to be a color format!"  # type: ignore
         assert isinstance(default_header_color, ColorFormatTuple), "Header color has to be a color format!"  # type: ignore
-        assert isinstance(pbar_color_filled, ColorFormatTuple)
-        assert isinstance(pbar_color_empty, ColorFormatTuple)
 
         # Default values for column and
         self.column_width = default_column_width
         self.column_color = default_column_color
         self.column_alignment = default_column_alignment
         self.column_aggregate = default_column_aggregate
         self.row_color = default_row_color
@@ -286,16 +241,14 @@
 
         self.custom_cell_format = custom_cell_format or get_default_format_func(num_decimal_places)
         self.pbar_show_throughput: bool = pbar_show_throughput
         self.pbar_show_progress: bool = pbar_show_progress
         self.pbar_show_percents: bool = pbar_show_percents
         self.pbar_show_eta: bool = pbar_show_eta
         self.pbar_embedded: bool = pbar_embedded
-        self.pbar_color_filled = pbar_color_filled
-        self.pbar_color_empty = pbar_color_empty
 
         self.refresh_rate: int = refresh_rate
 
         self._CURSOR_ROW = 0
         self._RENDERER_RUNNING = False
 
         # Interactivity settings
@@ -809,41 +762,45 @@
 
     def pbar(
         self,
         iterable: Iterable | int,
         *range_args,
         position=None,
         static=False,
-        color_filled="",
-        color_empty="",
         total=None,
         refresh_rate=None,
         description="",
         show_throughput=None,
         show_progress=None,
         show_percents=None,
         show_eta=None,
+        style=None,
+        style_embed=None,
+        color=None,
+        color_empty=None,
     ):
         """Create iterable progress bar object.
 
         Args:
             iterable: Iterable to iterate over. If None, it will be created from as range(iterable, *range_args).
             range_args: Optional arguments for range function.
             position: Level of the progress bar. If not provided, it will be set automatically.
             static: If True, the progress bar will stick to the row with index given by position.
                     If False, the position will be interpreted as the offset from the last row.
-            color_filled: Color of the filled part of the progress bar.
-            color_empty: Color of the empty part of the progress bar.
             total: Total number of iterations. If not provided, it will be calculated from the length of the iterable.
             refresh_rate: The maximal number of times per second the progress bar will be refreshed.
             description: Custom description of the progress bar that will be shown as prefix.
             show_throughput: If True, the throughput will be displayed.
             show_progress: If True, the progress will be displayed.
             show_percents: If True, the percentage of the progress will be displayed.
             show_eta: If True, the estimated time of finishing will be displayed.
+            style: Style of the progress bar. If None, the default style will be used.
+            style_embed: Style of the embedded progress bar. If None, the default style will be used.
+            color: Color of the progress bar. This overrides the default color.
+            color_empty: Color of the empty progress bar. This overrides the default color.
         """
         if isinstance(iterable, int):
             iterable = range(iterable, *range_args)
 
         if self.interactive == 0:
             global WARNED_PBAR_HIDDEN
             if not WARNED_PBAR_HIDDEN:
@@ -853,22 +810,27 @@
         if static is True and position is None:
             raise ValueError("For static pbar position cannot be None!")
         if position is None:
             position = 0 if self.interactive < 2 else len(self._active_pbars) + 1 - self.pbar_embedded
 
         total = total if total is not None else (len(iterable) if isinstance(iterable, Sized) else 0)
 
+        style = parse_pbar_style(style) if style else self.pbar_style
+        style_embed = parse_pbar_style(style_embed) if style_embed else self.pbar_style_embed
+
         pbar = TableProgressBar(
             iterable=iterable,
             table=self,
             total=total,
+            style=style,
+            style_embed=style_embed,
+            color=color,
+            color_empty=color_empty,
             position=position,
             static=static,
-            color_filled=color_filled or self.pbar_color_filled,
-            color_empty=color_empty or self.pbar_color_empty,
             description=description,
             show_throughput=show_throughput if show_throughput is not None else self.pbar_show_throughput,
             show_progress=show_progress if show_progress is not None else self.pbar_show_progress,
             show_percents=show_percents if show_percents is not None else self.pbar_show_percents,
             show_eta=show_eta if show_eta is not None else self.pbar_show_eta,
         )
         self._active_pbars.append(pbar)
@@ -882,15 +844,17 @@
 class TableProgressBar:
     def __init__(
         self,
         iterable,
         *,
         table,
         total,
-        color_filled,
+        style,
+        style_embed,
+        color,
         color_empty,
         position,
         static,
         description,
         show_throughput,
         show_progress,
         show_percents,
@@ -899,19 +863,29 @@
         self.iterable: Iterable | None = iterable
 
         self._step: int = 0
         self._total: int = total
         self._creation_time: float = time.perf_counter()
         self._last_refresh_time: float = -float("inf")
 
+        self.style = style
+        self.style_embed = style_embed
+
+        # Modyfing styles
+        if color:
+            color = maybe_convert_to_colorama(color)
+            self.style.color = color
+            self.style_embed.color = color
+        if color_empty:
+            color_empty = maybe_convert_to_colorama(color_empty)
+            self.style.color_empty = color_empty
+            self.style_embed.color_empty = color_empty
+
         self.position: int = position
         self.static: bool = static
-
-        self.color_filled: str = maybe_convert_to_colorama(color_filled)
-        self.color_empty: str = maybe_convert_to_colorama(color_empty)
         self.table: ProgressTableV1 = table
         self.description: str = description
         self.show_throughput: bool = show_throughput
         self.show_progress: bool = show_progress
         self.show_percents: bool = show_percents
         self.show_eta: bool = show_eta
         self._is_active: bool = True
@@ -989,41 +963,52 @@
 
         tot_width = tot_width - len(infobar)
         if not total:
             step = self._step % tot_width
             total = tot_width
 
         num_filled = math.ceil(step / total * tot_width)
+        frac_missing = step / total * tot_width - num_filled
         num_empty = tot_width - num_filled
 
         if embed_str is not None:
             row_str = embed_str
             row_str = row_str[2 + len(infobar) :]
 
             filled_part = row_str[:num_filled]
             if len(filled_part) > 0 and filled_part[-1] == " ":
-                filled_part = filled_part[:-1] + self.table.pbar_style_embed.head
-            filled_part = filled_part.replace(" ", self.table.pbar_style_embed.filled)
+                head = self.style_embed.head
+                if isinstance(head, (tuple, list)):
+                    head = head[round(frac_missing * len(head))]
+                filled_part = filled_part[:-1] + head
+            filled_part = filled_part.replace(" ", self.style_embed.filled)
             empty_part = row_str[num_filled:-1]
+            color_filled = self.style_embed.color
+            color_empty = self.style_embed.color_empty
         else:
-            filled_part = self.table.pbar_style.filled * num_filled
+            filled_part = self.style.filled * num_filled
             if len(filled_part) > 0:
-                filled_part = filled_part[:-1] + self.table.pbar_style.head
-            empty_part = self.table.pbar_style.empty * num_empty
+                head = self.style.head
+                if isinstance(head, (tuple, list)):
+                    head = head[round(frac_missing * len(head))]
+                filled_part = filled_part[:-1] + head
+            empty_part = self.style.empty * num_empty
+            color_filled = self.style.color
+            color_empty = self.style.color_empty
 
         pbar_body = "".join(
             [
                 self.table.table_style.vertical,
                 infobar,
-                self.color_filled,
+                color_filled,
                 filled_part,
-                Style.RESET_ALL if self.color_filled else "",
-                self.color_empty,
+                Style.RESET_ALL if color_filled else "",
+                color_empty,
                 empty_part,
-                Style.RESET_ALL if self.color_empty else "",
+                Style.RESET_ALL if color_empty else "",
                 self.table.table_style.vertical,
             ]
         )
         pbar.append(pbar_body)
         self._cleaning_str = " " * len(pbar_body)
         return "".join(pbar)
```

### Comparing `progress-table-2.1.0/progress_table.egg-info/PKG-INFO` & `progress-table-2.2.0/progress_table.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.1.0
+Version: 2.2.0
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `progress-table-2.1.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO` & `progress-table-2.2.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO`

 * *Files identical despite different names*

### Comparing `progress-table-2.1.0/progress_table.egg-info/SOURCES.txt` & `progress-table-2.2.0/progress_table.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 progress_table.egg-info/dependency_links.txt
 progress_table.egg-info/requires.txt
 progress_table.egg-info/top_level.txt
 progress_table/v0/__init__.py
 progress_table/v0/progress_table.py
 progress_table/v0/symbols.py
 progress_table/v1/__init__.py
+progress_table/v1/common.py
 progress_table/v1/progress_table.py
 progress_table/v1/styles.py
 tests/test_docs_automated.py
 tests/test_examples_automated.py
```

### Comparing `progress-table-2.1.0/setup.py` & `progress-table-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.1.0/tests/test_docs_automated.py` & `progress-table-2.2.0/tests/test_docs_automated.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.1.0/tests/test_examples_automated.py` & `progress-table-2.2.0/tests/test_examples_automated.py`

 * *Files identical despite different names*

