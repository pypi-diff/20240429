# Comparing `tmp/g3tables-0.1.2.tar.gz` & `tmp/g3tables-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3tables-0.1.2.tar", last modified: Tue Feb  6 17:25:49 2024, max compression
+gzip compressed data, was "g3tables-0.2.0.tar", last modified: Mon Apr 29 12:53:53 2024, max compression
```

## Comparing `g3tables-0.1.2.tar` & `g3tables-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,46 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:49.051818 g3tables-0.1.2/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3tables-0.1.2/LICENCE
--rw-rw-rw-   0        0        0      738 2024-02-06 17:25:49.038519 g3tables-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       81 2024-02-05 12:26:13.000000 g3tables-0.1.2/README.md
--rw-rw-rw-   0        0        0      983 2024-02-06 17:25:32.000000 g3tables-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-06 17:25:49.052817 g3tables-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:48.929975 g3tables-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:48.966528 g3tables-0.1.2/src/g3tables/
--rw-rw-rw-   0        0        0      493 2024-01-23 17:00:20.000000 g3tables-0.1.2/src/g3tables/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:48.998495 g3tables-0.1.2/src/g3tables/plc_composition_io_table/
--rw-rw-rw-   0        0        0      361 2024-01-30 11:09:40.000000 g3tables-0.1.2/src/g3tables/plc_composition_io_table/__init__.py
--rw-rw-rw-   0        0        0    14222 2024-01-30 12:43:53.000000 g3tables-0.1.2/src/g3tables/plc_composition_io_table/_extend_table.py
--rw-rw-rw-   0        0        0    17065 2024-01-31 23:06:02.000000 g3tables-0.1.2/src/g3tables/plc_composition_io_table/_table.py
--rw-rw-rw-   0        0        0     5535 2023-10-09 09:10:14.000000 g3tables-0.1.2/src/g3tables/plc_composition_io_table/io_signals.json
--rw-rw-rw-   0        0        0        0 2023-11-09 12:06:31.000000 g3tables-0.1.2/src/g3tables/py.typed
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:49.007360 g3tables-0.1.2/src/g3tables/sw_definition_table/
--rw-rw-rw-   0        0        0      182 2024-01-23 16:58:13.000000 g3tables-0.1.2/src/g3tables/sw_definition_table/__init__.py
--rw-rw-rw-   0        0        0    52329 2024-01-30 20:41:11.000000 g3tables-0.1.2/src/g3tables/sw_definition_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:49.017879 g3tables-0.1.2/src/g3tables/utils/
--rw-rw-rw-   0        0        0      146 2024-02-05 13:19:52.000000 g3tables-0.1.2/src/g3tables/utils/__init__.py
--rw-rw-rw-   0        0        0     1552 2024-01-03 13:08:04.000000 g3tables-0.1.2/src/g3tables/utils/_d2nd.py
--rw-rw-rw-   0        0        0     3706 2023-10-25 21:45:04.000000 g3tables-0.1.2/src/g3tables/utils/_interval.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:49.030890 g3tables-0.1.2/src/g3tables/utils/gdrive/
--rw-rw-rw-   0        0        0      147 2024-01-23 19:28:00.000000 g3tables-0.1.2/src/g3tables/utils/gdrive/__init__.py
--rw-rw-rw-   0        0        0     3365 2024-01-23 19:23:04.000000 g3tables-0.1.2/src/g3tables/utils/gdrive/_gdrive.py
--rw-rw-rw-   0        0        0     2360 2023-10-17 15:14:58.000000 g3tables-0.1.2/src/g3tables/utils/gdrive/creds.json
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:49.036888 g3tables-0.1.2/src/g3tables/visualization_table/
--rw-rw-rw-   0        0        0      207 2024-01-23 16:54:08.000000 g3tables-0.1.2/src/g3tables/visualization_table/__init__.py
--rw-rw-rw-   0        0        0     6194 2024-01-30 20:42:29.000000 g3tables-0.1.2/src/g3tables/visualization_table/_table.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:25:49.038519 g3tables-0.1.2/src/g3tables.egg-info/
--rw-rw-rw-   0        0        0      738 2024-02-06 17:25:48.000000 g3tables-0.1.2/src/g3tables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-02-06 17:25:48.000000 g3tables-0.1.2/src/g3tables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 17:25:48.000000 g3tables-0.1.2/src/g3tables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-02-06 17:25:48.000000 g3tables-0.1.2/src/g3tables.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-06 17:25:48.000000 g3tables-0.1.2/src/g3tables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:53.015962 g3tables-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3tables-0.2.0/LICENCE
+-rw-rw-rw-   0        0        0     1363 2024-04-29 12:53:53.012963 g3tables-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       81 2024-02-05 12:26:13.000000 g3tables-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1722 2024-04-26 09:21:54.000000 g3tables-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:53:53.016960 g3tables-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:51.958943 g3tables-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:52.005945 g3tables-0.2.0/src/g3tables/
+-rw-rw-rw-   0        0        0      550 2024-04-17 13:30:09.000000 g3tables-0.2.0/src/g3tables/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:52.204949 g3tables-0.2.0/src/g3tables/plc_composition_io_table/
+-rw-rw-rw-   0        0        0      361 2024-01-30 11:09:40.000000 g3tables-0.2.0/src/g3tables/plc_composition_io_table/__init__.py
+-rw-rw-rw-   0        0        0    14539 2024-04-17 23:31:56.000000 g3tables-0.2.0/src/g3tables/plc_composition_io_table/_extend_table.py
+-rw-rw-rw-   0        0        0    21360 2024-04-23 15:47:17.000000 g3tables-0.2.0/src/g3tables/plc_composition_io_table/_table.py
+-rw-rw-rw-   0        0        0     5535 2023-10-09 09:10:14.000000 g3tables-0.2.0/src/g3tables/plc_composition_io_table/io_signals.json
+-rw-rw-rw-   0        0        0        0 2023-11-09 12:06:31.000000 g3tables-0.2.0/src/g3tables/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:52.283946 g3tables-0.2.0/src/g3tables/sw_definition_table/
+-rw-rw-rw-   0        0        0      182 2024-01-23 16:58:13.000000 g3tables-0.2.0/src/g3tables/sw_definition_table/__init__.py
+-rw-rw-rw-   0        0        0    54470 2024-04-24 09:59:15.000000 g3tables-0.2.0/src/g3tables/sw_definition_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:52.822959 g3tables-0.2.0/src/g3tables/system_config/
+-rw-rw-rw-   0        0        0      225 2024-02-06 12:11:24.000000 g3tables-0.2.0/src/g3tables/system_config/__init__.py
+-rw-rw-rw-   0        0        0    15259 2024-04-26 09:28:53.000000 g3tables-0.2.0/src/g3tables/system_config/_cli.py
+-rw-rw-rw-   0        0        0    21817 2024-04-25 14:37:30.000000 g3tables-0.2.0/src/g3tables/system_config/_g3core_updater.py
+-rw-rw-rw-   0        0        0      972 2024-04-25 15:08:07.000000 g3tables-0.2.0/src/g3tables/system_config/_hw_connections.py
+-rw-rw-rw-   0        0        0     8599 2024-04-23 15:46:30.000000 g3tables-0.2.0/src/g3tables/system_config/_iomap_updater.py
+-rw-rw-rw-   0        0        0       74 2024-04-17 13:09:47.000000 g3tables-0.2.0/src/g3tables/system_config/_logger.py
+-rw-rw-rw-   0        0        0     7326 2024-04-20 10:49:38.000000 g3tables-0.2.0/src/g3tables/system_config/_sw_system_dict_wrapper.py
+-rw-rw-rw-   0        0        0     4132 2024-04-25 15:08:14.000000 g3tables-0.2.0/src/g3tables/system_config/_system_config_processor.py
+-rw-rw-rw-   0        0        0     1192 2024-04-17 13:14:39.000000 g3tables-0.2.0/src/g3tables/system_config/type_hinting.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:52.911980 g3tables-0.2.0/src/g3tables/utils/
+-rw-rw-rw-   0        0        0      146 2024-02-05 13:19:52.000000 g3tables-0.2.0/src/g3tables/utils/__init__.py
+-rw-rw-rw-   0        0        0     1552 2024-01-03 13:08:04.000000 g3tables-0.2.0/src/g3tables/utils/_d2nd.py
+-rw-rw-rw-   0        0        0     3706 2023-10-25 21:45:04.000000 g3tables-0.2.0/src/g3tables/utils/_interval.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:52.973959 g3tables-0.2.0/src/g3tables/utils/gdrive/
+-rw-rw-rw-   0        0        0      365 2024-03-10 17:32:39.000000 g3tables-0.2.0/src/g3tables/utils/gdrive/__init__.py
+-rw-rw-rw-   0        0        0     5172 2024-04-17 14:08:11.000000 g3tables-0.2.0/src/g3tables/utils/gdrive/_gdrive.py
+-rw-rw-rw-   0        0        0     1263 2024-03-10 16:29:47.000000 g3tables-0.2.0/src/g3tables/utils/gdrive/_update_creds.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:52.999958 g3tables-0.2.0/src/g3tables/visualization_table/
+-rw-rw-rw-   0        0        0      207 2024-01-23 16:54:08.000000 g3tables-0.2.0/src/g3tables/visualization_table/__init__.py
+-rw-rw-rw-   0        0        0    14811 2024-04-17 20:18:51.000000 g3tables-0.2.0/src/g3tables/visualization_table/_table.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:53:53.010962 g3tables-0.2.0/src/g3tables.egg-info/
+-rw-rw-rw-   0        0        0     1363 2024-04-29 12:53:51.000000 g3tables-0.2.0/src/g3tables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1290 2024-04-29 12:53:51.000000 g3tables-0.2.0/src/g3tables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:53:51.000000 g3tables-0.2.0/src/g3tables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-04-29 12:53:51.000000 g3tables-0.2.0/src/g3tables.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-04-29 12:53:51.000000 g3tables-0.2.0/src/g3tables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 12:53:51.000000 g3tables-0.2.0/src/g3tables.egg-info/top_level.txt
```

### Comparing `g3tables-0.1.2/LICENCE` & `g3tables-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `g3tables-0.1.2/src/g3tables/plc_composition_io_table/_extend_table.py` & `g3tables-0.2.0/src/g3tables/plc_composition_io_table/_extend_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,28 @@
         )
     parser.add_argument(
         'table_path',
         type=str,
         help='Path to the HW IO Table'
         )
     parser.add_argument(
-        '-re'
+        '-re',
         '--add-re-patterns',
         required=False,
         type=str,
         help='Path to the additional regex patterns file'
         )
+    parser.add_argument(
+        '--log-level',
+        type=str,
+        required=False,
+        default='INFO',
+        choices=['DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL'],
+        help='Set the logging level.'
+        )
     return parser.parse_args()
 
 
 class IOSignalPattern(typing.TypedDict):
     module: str
     connector: str
 
@@ -368,12 +376,12 @@
         output_file_path
         )
     table.save(output_file_path)
 
 
 def main() -> None:
     args = get_input_args()
+    logging.basicConfig(
+        level=args.log_level,
+        format='[%(name)s] %(levelname)s:%(message)s'
+        )
     extend_table(args.table_path, args.add_re_patterns)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `g3tables-0.1.2/src/g3tables/plc_composition_io_table/_table.py` & `g3tables-0.2.0/src/g3tables/plc_composition_io_table/_table.py`

 * *Files 23% similar despite different names*

```diff
@@ -107,40 +107,91 @@
 
 PLCCompositionIOTableColumnIndex: dict[str, int] = {
     memb: i + 1 for i, memb in enumerate(PLCCompositionIOTableColumn)
     }
 
 
 class PLCCompositionIOTable:
+    """
+    `PLCCompositionIOTable` is a representation of the G3 Project PLC
+    Composition and IO table. It allows access to the data of the hardware
+    cabinet sheets in the form of a `pandas.DataFrame`.
+
+    Note that the "razitko", "TSC-NxG_T11", "TSC-NxG_T22", "TSC-NxG_T22_20",
+    "template units", "units", "objedn", "List1", and "power" sheets are not
+    represented within the dictionary.
+    """
     NAME_PATTERN = 'plc_composition'
+    """
+    The pattern that the name of the SW Definition table must match to be
+    automatically recognized in a Google Drive folder.
+    """
     HEADER_ROW = 11
+    """
+    The row index of the header row in the table.
+    """
     EXCLUDE_SHEETS = [
         'razitko',
         'TSC-NxG_T11',
         'TSC-NxG_T22',
         'TSC-NxG_T22_20',
         'template units',
         'units',
         'objedn',
         'List1',
         'power'
         ]
+    """
+    Sheets that are not represented in the data dictionary of
+    a `PLCCompositionIOTable` instance.
+    """
 
     def __init__(self, data: pd.DataFrame) -> None:
+        """
+        Standard initializer of a `PLCCompositionIOTable` instance. Although it
+        can be used directly, alternative class constructors `from_local` and
+        `from_gdrive` are adviced instead.
+
+        Args:
+            data (dict[str, pd.DataFrame]): a dict, where keys are\
+            sheets names and values are the `pandas.DataFrame` objects\
+            representing the sheet data.
+        """
         self.data = data
 
     @classmethod
     def is_name_valid(cls, name: str) -> bool:
+        """
+        Check if the provided name matches the PLC Composition and IO table
+        name pattern.
+
+        Args:
+            name (str): The name to validate.
+
+        Returns:
+            bool: True if the name is valid, False otherwise.
+        """
         name_formatted = name.strip().replace(' ', '_').casefold()
         return cls.NAME_PATTERN in name_formatted
 
     @classmethod
     def from_local(
         cls, path: str, sheet_name: str | typing.Iterable[str]
     ) -> typing.Self:
+        """
+        Create a `PLCCompositionIOTable` instance from a local Excel file.
+
+        Args:
+            local_path (str): The local file path to the Excel file containing\
+                the PLC Composition and IO table data.
+
+        Returns:
+            Self: An instance of `PLCCompositionIOTable` initialized\
+                with data from the specified local Excel file.
+        """
         if isinstance(sheet_name, str):
             sheet_name = [sheet_name]
         else:
             sheet_name = [name for name in sheet_name]
         logger.info(
             'Reading PLC Composition IO table cabitet "%s" data from local '
             'path: "%s"', ", ".join(sheet_name), path
@@ -162,14 +213,25 @@
         sheets_concat = formatter(sheets)
         return cls(sheets_concat)
 
     @classmethod
     def from_gdrive(
         cls, gdrive_table_name: str, sheet_name: str | typing.Iterable[str]
     ) -> typing.Self:
+        """
+        Create a `PLCCompositionIOTable` instance from a Google Drive file.
+
+        Args:
+            gdrive_table_name (str): The name of the table in Google Drive\
+                containing the PLC Composition and IO table data.
+
+        Returns:
+            Self: An instance of `PLCCompositionIOTable` initialized\
+                with data from the specified Google Drive file.
+        """
         if isinstance(sheet_name, str):
             sheet_name = [sheet_name]
         logger.info(
             'Reading PLC Composition IO table cabitet "%s" data from Google '
             'Drive: "%s"', ", ".join(sheet_name), gdrive_table_name
             )
         try:
@@ -193,25 +255,57 @@
         sheets_concat = formatter(sheets, include_only=sheet_name)
         return cls(sheets_concat)
 
     @classmethod
     def load(
         cls, path: str, sheet_name: str | typing.Iterable[str]
     ) -> typing.Self:
+        """
+        Load a SW Definition table from a local file or Google Drive.
+
+        Args:
+            path (str): Path to the SW Definition table file. If the path ends\
+                with '.xlsx', the table is loaded from a local file.\
+                Otherwise, the table is loaded from Google Drive.
+
+        Returns:
+            typing.Self: An instance of `SWDefinitionTable` initialized with\
+                data from the specified file.
+        """
         if path.endswith('.xlsx'):
             return cls.from_local(path, sheet_name)
         return cls.from_gdrive(path, sheet_name)
 
     @staticmethod
     def get_column_index(column: str | PLCCompositionIOTableColumn) -> int:
+        """
+        Get the index of a column in the PLC Composition and IO table.
+
+        Args:
+            column (str | PLCCompositionIOTableColumn): The column name or\
+                enumeration member.
+
+        Returns:
+            int: The index of the column in the table.
+        """
         column = PLCCompositionIOTableColumn(column)
         return PLCCompositionIOTableColumnIndex[column]
 
     @staticmethod
     def get_column_letter(column: str | PLCCompositionIOTableColumn) -> str:
+        """
+        Get the column letter of a column in the PLC Composition and IO table.
+
+        Args:
+            column (str | PLCCompositionIOTableColumn): The column name or\
+                enumeration member.
+
+        Returns:
+            str: The column letter of the column in the table.
+        """
         column = PLCCompositionIOTableColumn(column)
         return get_column_letter(PLCCompositionIOTableColumnIndex[column])
 
     @staticmethod
     def _get_plc_unit_type(row) -> str | None:
         unit_type = row[PLCCompositionIOTableColumn.PLC_UNIT]
         if PLCCompositionIOTableFormatter.is_plc_unit_type(unit_type):
@@ -231,39 +325,62 @@
 
     def _is_terminal_equivalent(self, terminal1: str, terminal2: str) -> bool:
         prefix1 = self._extract_prefix(terminal1)
         prefix2 = self._extract_prefix(terminal2)
         return prefix1 == prefix2
 
     def iter_plc_units(self) -> typing.Iterator[tuple[str, str, str]]:
-        """-> type, cabinet, name suffix"""
+        """
+        Iterate over the PLC units in the table.
+
+        Yields:
+            typing.Iterator[tuple[str, str, str]]: An iterator over the PLC\
+                units in the table. Each iteration yields a tuple containing\
+                the PLC unit type, the cabinet name, and the terminal suffix.
+        """
         suffix_prev = ''
         for _, row in self.data.iterrows():
             plc_unit_type = self._get_plc_unit_type(row)
             if not plc_unit_type:
                 continue
             suffix = row[PLCCompositionIOTableColumn.PLC_UNIT_SUFFIX]
             cabinet = row[PLCCompositionIOTableColumn.CABINET]
             if suffix == suffix_prev:
                 continue
             else:
                 suffix_prev = suffix
             yield plc_unit_type, cabinet, suffix
 
     def get_sl8101_name(self) -> str | None:
+        """
+        Get the name of the "X20cSL8101" PLC unit.
+
+        Returns:
+            str | None: The name of the "X20cSL8101" PLC unit if found,\
+                otherwise None.
+        """
         logger.info('Searching for the "X20cSL8101" PLC unit')
         for unit_type, cabinet, terminal in self.iter_plc_units():
             if 'sl8101' in unit_type.lower():
                 sl8101 = self._get_plc_unit_name(unit_type, cabinet, terminal)
-                logger.info('Found the "X20cSL8101" PLC unit "%s"', sl8101)
+                logger.debug('Found the "X20cSL8101" PLC unit "%s"', sl8101)
                 return sl8101
-        logger.info('Could not find the "X20cSL8101" PLC unit')
+        logger.warning('Could not find the "X20cSL8101" PLC unit')
         return None
 
     def get_iomapping(self) -> dict[str, dict[str, str]]:
+        """
+        Get the IO mapping data from the PLC Composition and IO table.
+
+        Returns:
+            dict[str, dict[str, str]]: A dictionary containing the IO mapping\
+                data. The keys are the software device type and name, and\
+                the values are dictionaries containing the software signal\
+                mapped to the hardware signal.
+        """
 
         def get_i_prefix(signal_name: str) -> str:
             logger.debug(
                 'Matching hardware signal "%s" IO mapping prefix', signal_name
                 )
             name = signal_name.lower()
             if "digitalinput" in name:
@@ -305,15 +422,15 @@
             hw_module_name = self._get_plc_unit_name(
                 hw_unit_type, cabinet, name_suffix
                 )
             hw_signal_name = row[PLCCompositionIOTableColumn.SIGNAL_NAME]
             prefix = get_i_prefix(hw_signal_name)
             hw_signal = f'{prefix}."{hw_module_name}".{hw_signal_name}'
             mapping_key = f'{sw_device_type}/{sw_device_name}'
-            logger.info(
+            logger.debug(
                 'Found IO mapping data for device "%s": "%s" -> "%s"',
                 mapping_key, sw_signal, hw_signal
                 )
             device_mapping = mapping.setdefault(mapping_key, dict())
             device_mapping[sw_signal] = hw_signal
         return mapping
```

### Comparing `g3tables-0.1.2/src/g3tables/plc_composition_io_table/io_signals.json` & `g3tables-0.2.0/src/g3tables/plc_composition_io_table/io_signals.json`

 * *Files identical despite different names*

### Comparing `g3tables-0.1.2/src/g3tables/sw_definition_table/_table.py` & `g3tables-0.2.0/src/g3tables/sw_definition_table/_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,50 +19,64 @@
     table. It allows access to the data of the 'Common' sheet and software zone
     configuration sheets in the form of a `pandas.DataFrame` dictionary.
 
     Note that the "Title", "Identification", and "Worksheet explanation" sheets
     are not represented within  the dictionary.
     """
     NAME_PATTERN = 'project_sw_definition'
+    """
+    The pattern that the name of the SW Definition table must match to be
+    automatically recognized in a Google Drive folder.
+    """
     EXCLUDED_SHEETS = ['Title', 'Identification', 'Worksheet explanation']
     """
     Sheets that are not represented in the data dictionary of
     a `SWDefinitionTable` instance.
     """
 
     def __init__(self, data: dict[str, pd.DataFrame]) -> None:
         """
         Standard initializer of a `SWDefinitionTable` instance. Although it
         can be used directly, alternative class constructors `from_local` and
         `from_gdrive` are adviced instead.
 
         Args:
-            data (dict[str, pd.DataFrame]): a dict, where keys are sheets names
-            and values are the `pandas.DataFrame` objects representing the
-            sheet data.
+            data (dict[str, pd.DataFrame]): a dict, where keys are\
+            sheets names and values are the `pandas.DataFrame` objects\
+            representing the sheet data.
         """
         self._data = data
 
     @classmethod
     def is_name_valid(cls, name: str) -> bool:
+        """
+        Check if the provided name matches the SW Definition table
+        name pattern.
+
+        Args:
+            name (str): The name to validate.
+
+        Returns:
+            bool: True if the name is valid, False otherwise.
+        """
         name_formatted = name.strip().replace(' ', '_').casefold()
         return cls.NAME_PATTERN in name_formatted
 
     @classmethod
     def from_local(cls, path: str) -> typing.Self:
         """
         Create a `SWDefinitionTable` instance from a local Excel file.
 
         Args:
-            local_path (str): The local file path to the Excel file containing
-            the SW Definition table.
+            local_path (str): The local file path to the Excel file containing\
+                the SW Definition table.
 
         Returns:
-            SWDefinitionTable: An instance of `SWDefinitionTable` initialized
-            with data from the specified local Excel file.
+            Self: An instance of `SWDefinitionTable` initialized\
+                with data from the specified local Excel file.
         """
         logger.info('Reading SW Definition table from local path: %s', path)
         formatter = SWDefinitionSheetFormatter
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             sheets_all = pd.read_excel(path, sheet_name=None)
             sheets = formatter.remove_excluded_sheets(sheets_all)
@@ -72,20 +86,20 @@
 
     @classmethod
     def from_gdrive(cls, gdrive_table_name: str) -> typing.Self:
         """
         Create a `SWDefinitionTable` instance from a Google Drive file.
 
         Args:
-            gdrive_table_name (str): The name of the table in Google Drive
-            containing the SW Definition table.
+            gdrive_table_name (str): The name of the table in Google Drive\
+                containing the SW Definition table.
 
         Returns:
-            SWDefinitionTable: An instance of `SWDefinitionTable` initialized
-            with data from the specified Google Drive file.
+            SWDefinitionTable: An instance of `SWDefinitionTable` initialized\
+                with data from the specified Google Drive file.
         """
         logger.info(
             'Reading SW Definition table from Google Drive: %s',
             gdrive_table_name
             )
         sheets_all = get_table_data_from_gdrive(
             gdrive_table_name,
@@ -95,20 +109,33 @@
         sheets = formatter.remove_excluded_sheets(sheets_all)  # type: ignore
         for sheet_name, sheet_data in sheets.items():
             sheets[sheet_name] = formatter.process_sheet_init(sheet_data)
         return cls(sheets)
 
     @classmethod
     def load(cls, path: str) -> typing.Self:
+        """
+        Load a SW Definition table from a local file or Google Drive.
+
+        Args:
+            path (str): Path to the SW Definition table file. If the path ends\
+                with '.xlsx', the table is loaded from a local file.\
+                Otherwise, the table is loaded from Google Drive.
+
+        Returns:
+            typing.Self: An instance of `SWDefinitionTable` initialized with\
+                data from the specified file.
+        """
         if path.endswith('.xlsx'):
             return cls.from_local(path)
         return cls.from_gdrive(path)
 
     @property
     def sheet_names(self) -> list[str]:
+        """Names of the sheets contained within the SW Definition table."""
         return [name for name in self._data.keys()]
 
     def get_sheet_data(self, sheet_name: str) -> pd.DataFrame:
         """
         Retrieves data for a specific sheet.
 
         Args:
@@ -128,33 +155,34 @@
 
     def get_system_sheets(self, system_name: str) -> dict[str, pd.DataFrame]:
         """
         Gets the sheets' data associated with a given system name. Note that
         the system name is not validated.
 
         Args:
-            system_name (str): The name of the system for which to retrieve
-            sheets.
+            system_name (str): The name of the system for which to retrieve\
+                sheets.
 
         Returns:
-            dict[str, pd.DataFrame]: A dictionary of sheets belonging to the
-            given system.
-
+            dict[str, pd.DataFrame]: A dictionary of sheets belonging to\
+                the given system.
         """
         sheets = {}
         for sheet_name, sheet_data in self._data.items():
             if sheet_name != 'Common':
                 system_connector = self.get_connected_system(sheet_name)
                 if system_connector != system_name:
                     continue
             sheets[sheet_name] = sheet_data
         if len(sheets) < 2:
-            logger.warning(
-                'No zone sheets were found for system "%s"', system_name
+            logger.error(
+                'No zone sheets were found for system "%s". Aborting',
+                system_name
                 )
+            exit(1)
         return sheets
 
     def get_connected_devices(
         self, zone_name: str, connector: str
     ) -> list[str]:
         """
         Retrieve connected device names based on the zone name and the type of
@@ -217,51 +245,64 @@
             raise AttributeError(
                 f'Sheet "{zone_name}" system connector is ambiguous '
                 f'({len(system_connector)} connectors found: {connectors}).'
                 )
         return system_connector[-1]
 
     def get_connected_commfunc_brc(self, zone_name: str) -> str | None:
+        """
+        Get the name of the BRC comm function connector if a TrackCircuit
+        detector is present in the specified zone. If no TrackCircuit detector
+        is found, the method returns None.
+
+        Args:
+            zone_name (str): Name of the zone to query for\
+                the BRC comm function.
+
+        Returns:
+            str | None: The name of the BRC comm function connector if a\
+                TrackCircuit detector is present, otherwise None.
+        """
         logger.debug(
             'Looking for a BRC comm function within the "Common" sheet.'
             )
         common_data = self.get_sheet_data('Common')
         commfunc_row = common_data.loc[('CommFunction', 'general/name'), 1:]
         commfunc_brc = None
         column_index = 1
         while True:
             if column_index not in commfunc_row:
                 break
             cell_value = commfunc_row[column_index]
-            if not cell_value:
-                continue
-            if 'brc' in str(cell_value).lower():
+            if cell_value and 'brc' in str(cell_value).lower():
                 commfunc_brc = cell_value
                 break
             column_index += 1
         if not commfunc_brc:
             logger.debug(
                 'No BRC comm function was found within the "Common" sheet.'
                 )
             return None
         assert isinstance(commfunc_brc, str)
         logger.debug('Found a BRC comm function within the "Common" sheet.')
         logger.debug(
             'Looking for a TrackCircuit detector within zone "%s".', zone_name
             )
         zone_data = self.get_sheet_data(zone_name)
-        detector_type_rows = zone_data.loc[('Detector', 'general/type'), 1:]
+        detector_type_row = zone_data.loc[('Detector', 'general/type'), 1:]
+        assert isinstance(detector_type_row, pd.Series)
         column_index = 1
         while True:
-            if column_index not in detector_type_rows:
+            if column_index not in detector_type_row:
                 break
-            cell_value = detector_type_rows[column_index]
+            cell_value = detector_type_row[column_index]
+            assert isinstance(cell_value, str)
             if not cell_value:
                 continue
-            if str(cell_value).lower() == 'trackcircuit':
+            if cell_value.lower() == 'trackcircuit':
                 logger.debug(
                     'Found a TrackCircuit detector within zone "%s".',
                     zone_name
                     )
                 return commfunc_brc
             column_index += 1
         logger.debug(
@@ -316,21 +357,22 @@
             zone_name (str): Name of the zone to query for cabinet names.
 
         Returns:
             list[str]: List of the found cabinet names.
         """
         logger.debug('Retrieving cabinet names for zone "%s".', zone_name)
         zone_data = self.get_sheet_data(zone_name)
-        conn_rows = zone_data.loc[('Cabinet', 'general/name'), 1:]
+        conn_row = zone_data.loc[('Cabinet', 'general/name'), 1:]
+        assert isinstance(conn_row, pd.Series)
         values: list[str] = []
         column_index = 1
         while True:
             if column_index not in zone_data:
                 break
-            cell_value = conn_rows[column_index]
+            cell_value = conn_row[column_index]
             assert isinstance(cell_value, str)
             if cell_value and (cell_value not in values):
                 values.append(cell_value)
             column_index += 1
         logger.debug(
             'Retrieved cabinet names "%s" for zone "%s"', values, zone_name
             )
@@ -338,20 +380,20 @@
 
     def to_dict(self, system_name: str) -> dict[str, dict]:
         """
         Converts the system sheets' data to a pure tree-like dictionary
         representation.
 
         Args:
-            system_name (str): The name of the system for which to generate
-            the dictionary.
+            system_name (str): The name of the system for which to generate\
+                the dictionary.
 
         Returns:
-            dict[str, dict]: The dictionary representation of the system's
-            sheets' data.
+            dict[str, dict]: The dictionary representation of the system's\
+                sheets' data.
         """
         # get unprocessed system sheets related to the system
         sheets = self.get_system_sheets(system_name)
         # process zone sheets and gather connected comm functions
         zone_sheets_converted: dict[str, dict] = {}
         commfunc_names = []
         for sheet_name, sheet_data in sheets.items():
@@ -432,14 +474,23 @@
         sanitized_key = re.sub('_+', '_', sanitized_key)
         # add 'general' prefix to the formatted key
         sanitized_key = f'general/{sanitized_key}'
         return sanitized_key
 
     @staticmethod
     def format_module_name(module_name: str) -> tuple[str, str]:
+        """
+        Split the module name into metamodule and module parts.
+
+        Args:
+            module_name (str): The original module name.
+
+        Returns:
+            tuple[str, str]: The metamodule and module parts of the name.
+        """
         if ':' not in module_name:  # No metamodule present
             if '.' in module_name:
                 metamodule = ':'.join(module_name.split('.'))
             elif '/' in module_name:
                 metamodule = ':'.join(module_name.split('/'))
             else:
                 metamodule = module_name
@@ -544,14 +595,15 @@
         subs_keys = sheet['Parameter'].apply(cls.format_module_key)
         sheet['Key'] = sheet['Key'].fillna(subs_keys)
         mask = sheet['Key'] == ''
         sheet.loc[mask, 'Key'] = subs_keys[mask]
         # set multiindex to 'Module' + 'Key' columns
         logger.debug("Setting multiindex to ['Module', 'Key'].")
         sheet = sheet.set_index(['Module', 'Key'])
+        sheet = sheet.sort_index()
         return sheet
 
     @classmethod
     def process_sheet_dict_conv(cls, sheet: pd.DataFrame) -> pd.DataFrame:
         """
         Process a DataFrame representing a sheet, dropping irrelevant data
         and formatting columns and cells.
@@ -632,33 +684,34 @@
             logger.debug(
                 'Updated device varname: "%s" -> "%s"', varname, formatted
                 )
         return formatted
 
     @classmethod
     def _update_varnames(
-        cls, devices: dict[str, dict], parent_varname: str = ''
+        cls, device_data: dict[str, dict], parent_varname: str = ''
     ) -> None:
-        for device_data in devices.values():
-            varname_old = device_data.get('general', {}).get('varname')
-            if varname_old is None:
-                continue
-            if parent_varname:
-                varname_new = f'{parent_varname}_{varname_old}'
-                device_data['general']['varname'] = varname_new
-                logger.debug(
-                    'Updated device varname: "%s" -> "%s"',
-                    varname_old, varname_new
-                    )
-            else:
-                varname_new = varname_old
-            children = device_data.get('children')
-            if children:
-                for child in children.values():
-                    cls._update_varnames(child, varname_new)
+        varname_old = device_data.get('general', {}).get('varname')
+        if varname_old is None:
+            # continue
+            return
+        if parent_varname:
+            varname_new = f'{parent_varname}_{varname_old}'
+            device_data['general']['varname'] = varname_new
+            logger.debug(
+                'Updated device varname: "%s" -> "%s"',
+                varname_old, varname_new
+                )
+        else:
+            varname_new = varname_old
+        children = device_data.get('children')
+        if children:
+            for child_module in children.values():
+                for child_device in child_module.values():
+                    cls._update_varnames(child_device, varname_new)
 
     @classmethod
     def update_varnames(cls, nested_structure: dict[str, dict]) -> None:
         """
         Update the variable names in the nested structure by appending
         their parent varnames.
 
@@ -668,21 +721,22 @@
         """
         special_varnames = {
             "Zone": "Zone",
             "System": "System",
             "SystemSafety": "SystemSafety"
             }
         logger.debug("Updating varnames in the nested structure.")
-        for module_name, module_data in nested_structure.items():
-            for device_data in module_data.values():
-                if module_name in special_varnames:
-                    varname = special_varnames[module_name]
-                    device_data['general']['varname'] = varname
-                else:
-                    cls._update_varnames(device_data)
+        for zone_name, zone_data in nested_structure.items():
+            for module_name, module_data in zone_data.items():
+                for device_data in module_data.values():
+                    if module_name in special_varnames:
+                        varname = special_varnames[module_name]
+                        device_data['general']['varname'] = varname
+                    else:
+                        cls._update_varnames(device_data)
         logger.debug("Finished updating varnames in the nested structure.")
 
     @staticmethod
     def format_device_connector(connector: str, log: bool = True) -> str:
         """
         Process a string interval by removing all non-alphanumeric characters
         from each interval item (whitespaces and hyphens are replaced with
@@ -1241,15 +1295,18 @@
         Args:
             project_name (str): The name of the project.
             system_name (str): The name of the system.
             common_data (dict): The common data structure where
             the SHV device ID is to be updated.
         """
         broker = f'{project_name}{system_name}-broker'
-        common_data['SHV']['SHV']['control/config/deviceID'] = broker
+        try:
+            common_data['SHV']['SHV']['control/config/deviceID'] = broker
+        except KeyError:
+            logger.warning('Failed to update SHV Device ID broker name.')
 
     def to_dict_common(
         self, system_name: str, commfunc_names: list[str]
     ) -> dict[str, dict]:
         """
         Convert the "Common" sheet data into a nested dictionary structure for
         a specific system.
```

### Comparing `g3tables-0.1.2/src/g3tables/utils/_d2nd.py` & `g3tables-0.2.0/src/g3tables/utils/_d2nd.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.1.2/src/g3tables/utils/_interval.py` & `g3tables-0.2.0/src/g3tables/utils/_interval.py`

 * *Files identical despite different names*

### Comparing `g3tables-0.1.2/src/g3tables.egg-info/SOURCES.txt` & `g3tables-0.2.0/src/g3tables.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -2,23 +2,33 @@
 README.md
 pyproject.toml
 src/g3tables/__init__.py
 src/g3tables/py.typed
 src/g3tables.egg-info/PKG-INFO
 src/g3tables.egg-info/SOURCES.txt
 src/g3tables.egg-info/dependency_links.txt
+src/g3tables.egg-info/entry_points.txt
 src/g3tables.egg-info/requires.txt
 src/g3tables.egg-info/top_level.txt
 src/g3tables/plc_composition_io_table/__init__.py
 src/g3tables/plc_composition_io_table/_extend_table.py
 src/g3tables/plc_composition_io_table/_table.py
 src/g3tables/plc_composition_io_table/io_signals.json
 src/g3tables/sw_definition_table/__init__.py
 src/g3tables/sw_definition_table/_table.py
+src/g3tables/system_config/__init__.py
+src/g3tables/system_config/_cli.py
+src/g3tables/system_config/_g3core_updater.py
+src/g3tables/system_config/_hw_connections.py
+src/g3tables/system_config/_iomap_updater.py
+src/g3tables/system_config/_logger.py
+src/g3tables/system_config/_sw_system_dict_wrapper.py
+src/g3tables/system_config/_system_config_processor.py
+src/g3tables/system_config/type_hinting.py
 src/g3tables/utils/__init__.py
 src/g3tables/utils/_d2nd.py
 src/g3tables/utils/_interval.py
 src/g3tables/utils/gdrive/__init__.py
 src/g3tables/utils/gdrive/_gdrive.py
-src/g3tables/utils/gdrive/creds.json
+src/g3tables/utils/gdrive/_update_creds.py
 src/g3tables/visualization_table/__init__.py
 src/g3tables/visualization_table/_table.py
```

