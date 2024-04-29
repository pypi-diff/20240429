# Comparing `tmp/progress-table-2.0.0.tar.gz` & `tmp/progress-table-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progress-table-2.0.0.tar", last modified: Sun Apr 28 18:31:15 2024, max compression
+gzip compressed data, was "progress-table-2.1.0.tar", last modified: Sun Apr 28 20:33:36 2024, max compression
```

## Comparing `progress-table-2.0.0.tar` & `progress-table-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.0.0/LICENSE.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4852 2024-04-28 18:31:15.864310 progress-table-2.0.0/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4088 2024-04-28 18:30:30.000000 progress-table-2.0.0/README.md
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/progress_table/
--rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-28 18:30:30.000000 progress-table-2.0.0/progress_table/__init__.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/progress_table/v0/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.0.0/progress_table/v0/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.0.0/progress_table/v0/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.0.0/progress_table/v0/symbols.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/progress_table/v1/
--rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.0.0/progress_table/v1/__init__.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)    45615 2024-04-28 18:30:41.000000 progress-table-2.0.0/progress_table/v1/progress_table.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     5170 2024-04-28 18:30:30.000000 progress-table-2.0.0/progress_table/v1/styles.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/progress_table.egg-info/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4852 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/PKG-INFO
--rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.0.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
--rw-r--r--   0 gaha      (1000) gaha      (1000)      593 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/SOURCES.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/dependency_links.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/requires.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-28 18:31:15.000000 progress-table-2.0.0/progress_table.egg-info/top_level.txt
--rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.0.0/pyproject.toml
--rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-28 18:31:15.864310 progress-table-2.0.0/setup.cfg
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-09 23:00:39.000000 progress-table-2.0.0/setup.py
-drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 18:31:15.864310 progress-table-2.0.0/tests/
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.0.0/tests/test_docs_automated.py
--rw-r--r--   0 gaha      (1000) gaha      (1000)     1849 2024-04-28 18:30:30.000000 progress-table-2.0.0/tests/test_examples_automated.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.130510 progress-table-2.1.0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1052 2022-11-17 19:44:00.000000 progress-table-2.1.0/LICENSE.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-28 20:33:36.130510 progress-table-2.1.0/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4139 2024-04-28 20:30:22.000000 progress-table-2.1.0/README.md
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.127176 progress-table-2.1.0/progress_table/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      334 2024-04-28 20:30:31.000000 progress-table-2.1.0/progress_table/__init__.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.127176 progress-table-2.1.0/progress_table/v0/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-05 19:18:13.000000 progress-table-2.1.0/progress_table/v0/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    23444 2024-04-05 20:02:34.000000 progress-table-2.1.0/progress_table/v0/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     3028 2024-04-04 15:47:39.000000 progress-table-2.1.0/progress_table/v0/symbols.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.127176 progress-table-2.1.0/progress_table/v1/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       41 2024-04-04 15:47:39.000000 progress-table-2.1.0/progress_table/v1/__init__.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)    46788 2024-04-28 20:30:31.000000 progress-table-2.1.0/progress_table/v1/progress_table.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     5390 2024-04-28 20:30:31.000000 progress-table-2.1.0/progress_table/v1/styles.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.130510 progress-table-2.1.0/progress_table.egg-info/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4903 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/PKG-INFO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     4883 2024-03-12 12:10:39.000000 progress-table-2.1.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      593 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/SOURCES.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        1 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/dependency_links.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)        9 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/requires.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)       15 2024-04-28 20:33:36.000000 progress-table-2.1.0/progress_table.egg-info/top_level.txt
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      207 2024-03-11 20:11:56.000000 progress-table-2.1.0/pyproject.toml
+-rw-r--r--   0 gaha      (1000) gaha      (1000)      110 2024-04-28 20:33:36.130510 progress-table-2.1.0/setup.cfg
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1504 2024-04-09 23:00:39.000000 progress-table-2.1.0/setup.py
+drwxr-xr-x   0 gaha      (1000) gaha      (1000)        0 2024-04-28 20:33:36.130510 progress-table-2.1.0/tests/
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1804 2024-04-06 12:00:21.000000 progress-table-2.1.0/tests/test_docs_automated.py
+-rw-r--r--   0 gaha      (1000) gaha      (1000)     1867 2024-04-28 20:30:31.000000 progress-table-2.1.0/tests/test_examples_automated.py
```

### Comparing `progress-table-2.0.0/LICENSE.txt` & `progress-table-2.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.0.0/PKG-INFO` & `progress-table-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.0.0
+Version: 2.1.0
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -114,16 +114,16 @@
 Progress Table works correctly in most consoles, but there are some exceptions:
 
 * Some cloud logging consoles (e.g. kubernetes) don't support `\r` properly.
   You can still use ProgressTable, but with `interactive=0` option. This mode will not display progress bars.
 * Some consoles like `PyCharm Python Console` or `IDLE` don't support cursor movement.
   You can still use ProgressTable, but with `interactive=1` option. This mode displays only 1 progress bar at once.
 
-> By default `interactive=2`. You can change the default `interactive` by
-> setting `PTABLE_INTERACTIVE` environment variable, e.g. `PTABLE_INTERACTIVE=1`.
+> By default `interactive=2`. You can change the default `interactive` with an argument when creating the table object
+> or by setting `PTABLE_INTERACTIVE` environment variable, e.g. `PTABLE_INTERACTIVE=1`.
 
 ## Installation
 
 Install Progress Table easily with pip:
 
 ```
 pip install progress-table
```

### Comparing `progress-table-2.0.0/README.md` & `progress-table-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 Progress Table works correctly in most consoles, but there are some exceptions:
 
 * Some cloud logging consoles (e.g. kubernetes) don't support `\r` properly.
   You can still use ProgressTable, but with `interactive=0` option. This mode will not display progress bars.
 * Some consoles like `PyCharm Python Console` or `IDLE` don't support cursor movement.
   You can still use ProgressTable, but with `interactive=1` option. This mode displays only 1 progress bar at once.
 
-> By default `interactive=2`. You can change the default `interactive` by
-> setting `PTABLE_INTERACTIVE` environment variable, e.g. `PTABLE_INTERACTIVE=1`.
+> By default `interactive=2`. You can change the default `interactive` with an argument when creating the table object
+> or by setting `PTABLE_INTERACTIVE` environment variable, e.g. `PTABLE_INTERACTIVE=1`.
 
 ## Installation
 
 Install Progress Table easily with pip:
 
 ```
 pip install progress-table
```

### Comparing `progress-table-2.0.0/progress_table/v0/progress_table.py` & `progress-table-2.1.0/progress_table/v0/progress_table.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.0.0/progress_table/v0/symbols.py` & `progress-table-2.1.0/progress_table/v0/symbols.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.0.0/progress_table/v1/progress_table.py` & `progress-table-2.1.0/progress_table/v1/progress_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,21 +147,23 @@
         interactive: int = int(os.environ.get("PTABLE_INTERACTIVE", 2)),
         refresh_rate: int = 20,
         num_decimal_places: int = 4,
         default_column_width: int | None = None,
         default_column_color: ColorFormat = None,
         default_column_alignment: str | None = None,
         default_column_aggregate: str | None = None,
+        default_header_color: ColorFormat = None,
         default_row_color: ColorFormat = None,
         pbar_show_throughput: bool = True,
         pbar_show_progress: bool = False,
         pbar_show_percents: bool = False,
         pbar_show_eta: bool = False,
         pbar_embedded: bool = True,
-        pbar_color: ColorFormat = None,
+        pbar_color_filled: ColorFormat = None,
+        pbar_color_empty: ColorFormat = None,
         print_header_on_top: bool = True,
         print_header_every_n_rows: int = 30,
         custom_cell_format: Callable[[Any], str] | None = None,
         table_style: str | Type[styles.TableStyleBase] = "round",
         pbar_style: str | Type[styles.PbarStyleBase] = "normal",
         pbar_style_embed: str | Type[styles.PbarStyleBase] = "embed",
         file=None,
@@ -211,14 +213,16 @@
             pbar_show_progress: Show progress in the progress bar, for example 10/40. Defaults to True.
             pbar_show_percents: Show percents in the progress bar, for example 25%. Defaults to False.
             pbar_show_eta: Show estimated time of finishing in the progress bar, for example 10s. Defaults to False.
             pbar_embedded: If True, changes the way the first (non-nested) progress bar looks.
                            Embedded version is more subtle, but does not prevent the current row from being displayed.
                            If False, the progress bar covers the current row, preventing the user from seeing values
                            that are being updated until the progress bar finishes. The default is True.
+            pbar_color_filled: Default color of the filled part of the progress bars.
+            pbar_color_empty: Default color of the empty part of the progress bars.
             print_header_every_n_rows: 30 by default. When table has a lot of rows, it can be useful to remind what the header is.
                                        If True, hedaer will be displayed periodically after the selected number of rows. 0 to supress.
             custom_cell_format: A function that defines how to get str value to display from a cell content.
                                 This function should be universal and work for all datatypes as inputs.
                                 It takes one value as an input and returns string as an output.
             table_style: Change the borders of the table. Either a string or 'TableStyleBase' type class.
             pbar_style: Change the style of the progress bar. Either a string or 'PbarStyleBase' type class.
@@ -236,21 +240,25 @@
 
         self.table_style = styles.figure_table_style(table_style)
         self.pbar_style = styles.figure_pbar_style(pbar_style)
         self.pbar_style_embed = styles.figure_pbar_style(pbar_style_embed)
 
         assert isinstance(default_row_color, ColorFormatTuple), "Row color has to be a color format!"  # type: ignore
         assert isinstance(default_column_color, ColorFormatTuple), "Column color has to be a color format!"  # type: ignore
+        assert isinstance(default_header_color, ColorFormatTuple), "Header color has to be a color format!"  # type: ignore
+        assert isinstance(pbar_color_filled, ColorFormatTuple)
+        assert isinstance(pbar_color_empty, ColorFormatTuple)
 
         # Default values for column and
         self.column_width = default_column_width
         self.column_color = default_column_color
         self.column_alignment = default_column_alignment
         self.column_aggregate = default_column_aggregate
         self.row_color = default_row_color
+        self.header_color = default_header_color
 
         # We are storing column configs
         self.column_widths: dict[str, int] = {}
         self.column_colors: dict[str, str] = {}
         self.column_alignments: dict[str, str] = {}
         self.column_aggregates: dict[str, Callable] = {}
         self.column_names: list[str] = []  # Names serve as keys for column configs
@@ -278,15 +286,16 @@
 
         self.custom_cell_format = custom_cell_format or get_default_format_func(num_decimal_places)
         self.pbar_show_throughput: bool = pbar_show_throughput
         self.pbar_show_progress: bool = pbar_show_progress
         self.pbar_show_percents: bool = pbar_show_percents
         self.pbar_show_eta: bool = pbar_show_eta
         self.pbar_embedded: bool = pbar_embedded
-        self.pbar_color = pbar_color
+        self.pbar_color_filled = pbar_color_filled
+        self.pbar_color_empty = pbar_color_empty
 
         self.refresh_rate: int = refresh_rate
 
         self._CURSOR_ROW = 0
         self._RENDERER_RUNNING = False
 
         # Interactivity settings
@@ -782,31 +791,34 @@
         return self._get_bar(self.table_style.up_right, self.table_style.no_down, self.table_style.up_left)
 
     def _get_bar_mid(self):
         return self._get_bar(self.table_style.no_left, self.table_style.all, self.table_style.no_right)
 
     def _get_header(self):
         content = []
+        colors = self.column_colors if self.header_color is None else self._resolve_row_color_dict(self.header_color)
+
         for column in self.column_names:
-            value = self._apply_cell_formatting(column, column, color=self.column_colors[column])
+            value = self._apply_cell_formatting(column, column, color=colors[column])
             content.append(value)
         s = "".join(["\r", self.table_style.vertical, self.table_style.vertical.join(content), self.table_style.vertical])
         return s
 
     ##################
     ## PROGRESS BAR ##
     ##################
 
     def pbar(
         self,
         iterable: Iterable | int,
         *range_args,
         position=None,
         static=False,
-        color="",
+        color_filled="",
+        color_empty="",
         total=None,
         refresh_rate=None,
         description="",
         show_throughput=None,
         show_progress=None,
         show_percents=None,
         show_eta=None,
@@ -815,15 +827,16 @@
 
         Args:
             iterable: Iterable to iterate over. If None, it will be created from as range(iterable, *range_args).
             range_args: Optional arguments for range function.
             position: Level of the progress bar. If not provided, it will be set automatically.
             static: If True, the progress bar will stick to the row with index given by position.
                     If False, the position will be interpreted as the offset from the last row.
-            color: Color of the progress bar.
+            color_filled: Color of the filled part of the progress bar.
+            color_empty: Color of the empty part of the progress bar.
             total: Total number of iterations. If not provided, it will be calculated from the length of the iterable.
             refresh_rate: The maximal number of times per second the progress bar will be refreshed.
             description: Custom description of the progress bar that will be shown as prefix.
             show_throughput: If True, the throughput will be displayed.
             show_progress: If True, the progress will be displayed.
             show_percents: If True, the percentage of the progress will be displayed.
             show_eta: If True, the estimated time of finishing will be displayed.
@@ -846,15 +859,16 @@
 
         pbar = TableProgressBar(
             iterable=iterable,
             table=self,
             total=total,
             position=position,
             static=static,
-            color=color or self.pbar_color,
+            color_filled=color_filled or self.pbar_color_filled,
+            color_empty=color_empty or self.pbar_color_empty,
             description=description,
             show_throughput=show_throughput if show_throughput is not None else self.pbar_show_throughput,
             show_progress=show_progress if show_progress is not None else self.pbar_show_progress,
             show_percents=show_percents if show_percents is not None else self.pbar_show_percents,
             show_eta=show_eta if show_eta is not None else self.pbar_show_eta,
         )
         self._active_pbars.append(pbar)
@@ -868,15 +882,16 @@
 class TableProgressBar:
     def __init__(
         self,
         iterable,
         *,
         table,
         total,
-        color,
+        color_filled,
+        color_empty,
         position,
         static,
         description,
         show_throughput,
         show_progress,
         show_percents,
         show_eta,
@@ -887,15 +902,16 @@
         self._total: int = total
         self._creation_time: float = time.perf_counter()
         self._last_refresh_time: float = -float("inf")
 
         self.position: int = position
         self.static: bool = static
 
-        self.color: str = maybe_convert_to_colorama(color)
+        self.color_filled: str = maybe_convert_to_colorama(color_filled)
+        self.color_empty: str = maybe_convert_to_colorama(color_empty)
         self.table: ProgressTableV1 = table
         self.description: str = description
         self.show_throughput: bool = show_throughput
         self.show_progress: bool = show_progress
         self.show_percents: bool = show_percents
         self.show_eta: bool = show_eta
         self._is_active: bool = True
@@ -994,18 +1010,20 @@
                 filled_part = filled_part[:-1] + self.table.pbar_style.head
             empty_part = self.table.pbar_style.empty * num_empty
 
         pbar_body = "".join(
             [
                 self.table.table_style.vertical,
                 infobar,
-                self.color,
+                self.color_filled,
                 filled_part,
-                Style.RESET_ALL if self.color else "",
+                Style.RESET_ALL if self.color_filled else "",
+                self.color_empty,
                 empty_part,
+                Style.RESET_ALL if self.color_empty else "",
                 self.table.table_style.vertical,
             ]
         )
         pbar.append(pbar_body)
         self._cleaning_str = " " * len(pbar_body)
         return "".join(pbar)
```

### Comparing `progress-table-2.0.0/progress_table/v1/styles.py` & `progress-table-2.1.0/progress_table/v1/styles.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,23 +48,30 @@
 class PbarStyleNormal(PbarStyleBase):
     name = "normal"
     filled = "■"
     empty = "□"
     head = "◩"
 
 
+class PbarStyleShort(PbarStyleBase):
+    name = "short"
+    filled = "▬"
+    empty = "▭"
+    head = "▬"
+
+
 class PbarStyleNormalClean(PbarStyleBase):
     name = "normal clean"
     filled = "■"
     empty = " "
     head = "◩"
 
 
 class PbarStyleCircle(PbarStyleBase):
-    name = "cirlce"
+    name = "circle"
     filled = "●"
     empty = "○"
     head = "◉"
 
 
 class PbarStyleCircleClean(PbarStyleBase):
     name = "circle clean"
@@ -90,14 +97,21 @@
 class PbarStyleEmbed(PbarStyleBase):
     name = "embed"
     filled = "ꞏ"
     empty = " "
     head = ">"
 
 
+class PbarStyleRich(PbarStyleBase):
+    name = "rich"
+    filled = "━"
+    empty = " "
+    head = "━"
+
+
 class PbarStyleNone(PbarStyleBase):
     name = "hidden"
     filled = " "
     empty = " "
     head = " "
```

### Comparing `progress-table-2.0.0/progress_table.egg-info/PKG-INFO` & `progress-table-2.1.0/progress_table.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progress-table
-Version: 2.0.0
+Version: 2.1.0
 Summary: Display progress as a pretty table in the command line.
 Home-page: https://github.com/gahaalt/progress-table.git
 Author: Szymon Mikler
 Author-email: sjmikler@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -114,16 +114,16 @@
 Progress Table works correctly in most consoles, but there are some exceptions:
 
 * Some cloud logging consoles (e.g. kubernetes) don't support `\r` properly.
   You can still use ProgressTable, but with `interactive=0` option. This mode will not display progress bars.
 * Some consoles like `PyCharm Python Console` or `IDLE` don't support cursor movement.
   You can still use ProgressTable, but with `interactive=1` option. This mode displays only 1 progress bar at once.
 
-> By default `interactive=2`. You can change the default `interactive` by
-> setting `PTABLE_INTERACTIVE` environment variable, e.g. `PTABLE_INTERACTIVE=1`.
+> By default `interactive=2`. You can change the default `interactive` with an argument when creating the table object
+> or by setting `PTABLE_INTERACTIVE` environment variable, e.g. `PTABLE_INTERACTIVE=1`.
 
 ## Installation
 
 Install Progress Table easily with pip:
 
 ```
 pip install progress-table
```

### Comparing `progress-table-2.0.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO` & `progress-table-2.1.0/progress_table.egg-info/PKG-INFO.sync-conflict-20240314-015933-NXTV2IO`

 * *Files identical despite different names*

### Comparing `progress-table-2.0.0/progress_table.egg-info/SOURCES.txt` & `progress-table-2.1.0/progress_table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progress-table-2.0.0/setup.py` & `progress-table-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.0.0/tests/test_docs_automated.py` & `progress-table-2.1.0/tests/test_docs_automated.py`

 * *Files identical despite different names*

### Comparing `progress-table-2.0.0/tests/test_examples_automated.py` & `progress-table-2.1.0/tests/test_examples_automated.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib
 import sys
 from glob import glob
 from io import StringIO
 
 EXPECTED_OUTPUTS = {
     "examples.training": "14af860a37118c16aec4604e5629e5ed",
-    "examples.tictactoe": "056841a6cbf7456cd3daacbff356088a",
+    "examples.tictactoe": "378133fb7804a678282564d751068531",
     "examples.brown2d": "c0f37fdfcfc2db6ef465473c67c05d83",
 }
 
 
 def capture_example_stdout(main_fn):
     # To eliminate run to run variation of the example outputs we need to be independent from the execution speed
     # This includes removing the influence of:
@@ -23,15 +23,15 @@
         pbar_show_throughput=False,
         refresh_rate=0,
     )
 
     # We will replace stdout with custom StringIO and check whether example stdout is as expected
     out_buffer = StringIO()
     sys.stdout = out_buffer
-    main_fn(random_seed=42, **override_kwds)
+    main_fn(random_seed=42, sleep_duration=0, **override_kwds)
     sys.stdout = sys.__stdout__
     return out_buffer.getvalue()
 
 
 def test_all_examples():
     # Testing whether examples run exactly as intended
```

