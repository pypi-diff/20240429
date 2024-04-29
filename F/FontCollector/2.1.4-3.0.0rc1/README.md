# Comparing `tmp/FontCollector-2.1.4.tar.gz` & `tmp/fontcollector-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FontCollector-2.1.4.tar", last modified: Sun Oct 29 16:14:59 2023, max compression
+gzip compressed data, was "fontcollector-3.0.0rc1.tar", last modified: Mon Apr 29 17:46:32 2024, max compression
```

## Comparing `FontCollector-2.1.4.tar` & `fontcollector-3.0.0rc1.tar`

### file list

```diff
@@ -1,33 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 16:14:59.671954 FontCollector-2.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 16:14:59.667954 FontCollector-2.1.4/FontCollector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2023-10-29 16:14:59.000000 FontCollector-2.1.4/FontCollector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-10-29 16:14:59.000000 FontCollector-2.1.4/FontCollector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 16:14:59.000000 FontCollector-2.1.4/FontCollector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-29 16:14:59.000000 FontCollector-2.1.4/FontCollector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-10-29 16:14:59.000000 FontCollector-2.1.4/FontCollector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-29 16:14:59.000000 FontCollector-2.1.4/FontCollector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-10-29 16:14:49.000000 FontCollector-2.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2023-10-29 16:14:59.671954 FontCollector-2.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2023-10-29 16:14:49.000000 FontCollector-2.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 16:14:59.667954 FontCollector-2.1.4/font_collector/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9553 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/ass_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/ass_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/font.py
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/font_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    37326 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/font_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/font_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7278 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/mkvpropedit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/parse_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-10-29 16:14:49.000000 FontCollector-2.1.4/font_collector/usage_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-10-29 16:14:49.000000 FontCollector-2.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-29 16:14:59.671954 FontCollector-2.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 16:14:59.671954 FontCollector-2.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-10-29 16:14:49.000000 FontCollector-2.1.4/tests/test_ass_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     9589 2023-10-29 16:14:49.000000 FontCollector-2.1.4/tests/test_font.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2023-10-29 16:14:49.000000 FontCollector-2.1.4/tests/test_font_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-10-29 16:14:49.000000 FontCollector-2.1.4/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/FontCollector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 17:46:32.000000 fontcollector-3.0.0rc1/FontCollector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.247258 fontcollector-3.0.0rc1/font_collector/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.247258 fontcollector-3.0.0rc1/font_collector/ass/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/abc_ass_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/ass_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/ass_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/ass/usage_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.247258 fontcollector-3.0.0rc1/font_collector/font/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12333 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/abc_font_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/chinese_variant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/cmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/factory_abc_font_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35666 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/font_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9924 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/lcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/normal_font_face.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy_libass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/selection_strategy/font_selection_strategy_vsfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/font/variable_font_face.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/mkvpropedit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/parse_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/font_collector/system_lang/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/abc_system_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/linux_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/mac_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/system_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/font_collector/system_lang/windows_lang.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-29 17:46:27.000000 fontcollector-3.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:46:32.251258 fontcollector-3.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-29 17:46:28.000000 fontcollector-3.0.0rc1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-29 17:46:28.000000 fontcollector-3.0.0rc1/tests/test_mkvpropedit.py
```

### Comparing `FontCollector-2.1.4/FontCollector.egg-info/PKG-INFO` & `fontcollector-3.0.0rc1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,11 @@
-Metadata-Version: 2.1
-Name: FontCollector
-Version: 2.1.4
-Summary: FontCollector for Advanced SubStation Alpha file.
-Author-email: moi15moi <moi15moismokerlolilol@gmail.com>
-License: MIT
-Project-URL: Source, https://github.com/moi15moi/FontCollector/
-Project-URL: Tracker, https://github.com/moi15moi/FontCollector/issues/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Other Audience
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: ass
-Requires-Dist: ass-tag-analyzer
-Requires-Dist: fontTools>=4.38.0
-Requires-Dist: freetype-py
-Requires-Dist: FindSystemFontsFilename>=0.1.2
-
 # FontCollector
+[![FontCollector test code coverage](https://img.shields.io/codecov/c/github/moi15moi/FontCollector)](https://app.codecov.io/github/moi15moi/FontCollector)
+[![FontCollector mypy verification](https://img.shields.io/badge/mypy-checked-blue)](https://github.com/moi15moi/FontCollector/actions?query=branch:main)
+
 FontCollector for Advanced SubStation Alpha file.
 This tool allows to recover and/or mux the fonts necessary in an mkv.
 ## Installation
 ```
 pip install FontCollector
 ```
 ## Dependencies
@@ -42,27 +20,30 @@
 FontCollector for Advanced SubStation Alpha file.
 
 options:
   -h, --help            show this help message and exit
   --input [INPUT ...], -i [INPUT ...]
                         Subtitles file. Must be an ASS file/directory. You can specify more than one .ass file/path.
                         If no argument is specified, it will take all the font in the current path.
-  -mkv MKV              
+  -mkv MKV
                         Video where the fonts will be merge. Must be a Matroska file.
   --output OUTPUT, -o OUTPUT
                         Destination path of the font. If -o and -mkv aren't specified, it will be the current path.
   -mkvpropedit MKVPROPEDIT
                         Path to mkvpropedit.exe if not in variable environments. If -mkv is not specified, it will do
                         nothing.
-  --delete-fonts, -d    
+  --delete-fonts, -d
                         If -d is specified, it will delete the font attached to the mkv before merging the new needed
                         font. If -mkv is not specified, it will do nothing.
-  --additional-fonts ADDITIONAL_FONTS [ADDITIONAL_FONTS ...]
+  --additional-fonts ADDITIONAL_FONTS [ADDITIONAL_FONTS ...], -add-fonts ADDITIONAL_FONTS [ADDITIONAL_FONTS ...]
                         May be a directory containing font files or a single font file. You can specify more than one
                         additional-fonts.
+                        If it is a directory, it won't search recursively for fonts
+  --additional-fonts-recursive ADDITIONAL_FONTS_RECURSIVE [ADDITIONAL_FONTS_RECURSIVE ...], -add-fonts-rec ADDITIONAL_FONTS_RECURSIVE [ADDITIONAL_FONTS_RECURSIVE ...]
+                        Path to font directory, which will be recursively searched for fonts.
   --exclude-system-fonts
                         If specified, FontCollector won't use the system font to find the font used by an .ass file.
   --collect-draw-fonts
                         If specified, FontCollector will collect the font used by the draw. For more detail when this
                         is usefull, see: https://github.com/libass/libass/issues/617
 ```
 ## Examples
```

### Comparing `FontCollector-2.1.4/LICENSE` & `fontcollector-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `FontCollector-2.1.4/PKG-INFO` & `fontcollector-3.0.0rc1/FontCollector.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 Metadata-Version: 2.1
 Name: FontCollector
-Version: 2.1.4
+Version: 3.0.0rc1
 Summary: FontCollector for Advanced SubStation Alpha file.
 Author-email: moi15moi <moi15moismokerlolilol@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/moi15moi/FontCollector/
 Project-URL: Tracker, https://github.com/moi15moi/FontCollector/issues/
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Other Audience
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ass
 Requires-Dist: ass-tag-analyzer
 Requires-Dist: fontTools>=4.38.0
 Requires-Dist: freetype-py
 Requires-Dist: FindSystemFontsFilename>=0.1.2
+Requires-Dist: langcodes
 
 # FontCollector
+[![FontCollector test code coverage](https://img.shields.io/codecov/c/github/moi15moi/FontCollector)](https://app.codecov.io/github/moi15moi/FontCollector)
+[![FontCollector mypy verification](https://img.shields.io/badge/mypy-checked-blue)](https://github.com/moi15moi/FontCollector/actions?query=branch:main)
+
 FontCollector for Advanced SubStation Alpha file.
 This tool allows to recover and/or mux the fonts necessary in an mkv.
 ## Installation
 ```
 pip install FontCollector
 ```
 ## Dependencies
@@ -42,27 +50,30 @@
 FontCollector for Advanced SubStation Alpha file.
 
 options:
   -h, --help            show this help message and exit
   --input [INPUT ...], -i [INPUT ...]
                         Subtitles file. Must be an ASS file/directory. You can specify more than one .ass file/path.
                         If no argument is specified, it will take all the font in the current path.
-  -mkv MKV              
+  -mkv MKV
                         Video where the fonts will be merge. Must be a Matroska file.
   --output OUTPUT, -o OUTPUT
                         Destination path of the font. If -o and -mkv aren't specified, it will be the current path.
   -mkvpropedit MKVPROPEDIT
                         Path to mkvpropedit.exe if not in variable environments. If -mkv is not specified, it will do
                         nothing.
-  --delete-fonts, -d    
+  --delete-fonts, -d
                         If -d is specified, it will delete the font attached to the mkv before merging the new needed
                         font. If -mkv is not specified, it will do nothing.
-  --additional-fonts ADDITIONAL_FONTS [ADDITIONAL_FONTS ...]
+  --additional-fonts ADDITIONAL_FONTS [ADDITIONAL_FONTS ...], -add-fonts ADDITIONAL_FONTS [ADDITIONAL_FONTS ...]
                         May be a directory containing font files or a single font file. You can specify more than one
                         additional-fonts.
+                        If it is a directory, it won't search recursively for fonts
+  --additional-fonts-recursive ADDITIONAL_FONTS_RECURSIVE [ADDITIONAL_FONTS_RECURSIVE ...], -add-fonts-rec ADDITIONAL_FONTS_RECURSIVE [ADDITIONAL_FONTS_RECURSIVE ...]
+                        Path to font directory, which will be recursively searched for fonts.
   --exclude-system-fonts
                         If specified, FontCollector won't use the system font to find the font used by an .ass file.
   --collect-draw-fonts
                         If specified, FontCollector will collect the font used by the draw. For more detail when this
                         is usefull, see: https://github.com/libass/libass/issues/617
 ```
 ## Examples
```

### Comparing `FontCollector-2.1.4/font_collector/font_parser.py` & `fontcollector-3.0.0rc1/font_collector/font/font_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,71 @@
-import freetype
-import logging
-from .exceptions import NameNotFoundException
+from __future__ import annotations
+from ..exceptions import InvalidNameRecord, InvalidVariableFontFaceException
+from .cmap import CMap
+from .name import Name, NameID, PlatformID
 from ctypes import byref, c_uint, create_string_buffer
-from enum import IntEnum
-from io import BufferedReader
-from pathlib import Path
-from typing import Any, Dict, List, Optional, Set, Tuple
-from fontTools.ttLib.ttFont import TTFont
+from fontTools.ttLib.tables._c_m_a_p import CmapSubtable
 from fontTools.ttLib.tables._n_a_m_e import NameRecord
+from fontTools.ttLib.ttFont import TTFont
 from fontTools.varLib.instancer.names import ELIDABLE_AXIS_VALUE_NAME
-from freetype import FT_Face, FT_Get_Glyph_Name
+from freetype import (
+    Face,
+    FT_Face,
+    FT_Get_Glyph_Name,
+)
+from freetype.ft_enums.ft_style_flags import FT_STYLE_FLAGS
+from itertools import product
+from langcodes import Language
+from pathlib import Path
 from struct import error as struct_error
-
-_logger = logging.getLogger(__name__)
-
-
-class NameID(IntEnum):
-    COPYRIGHT = 0
-    FAMILY_NAME = 1
-    SUBFAMILY_NAME = 2
-    UNIQUE_ID = 3
-    FULL_NAME = 4
-    VERSION_STRING = 5
-    POSTSCRIPT_NAME = 6
-    TRADEMARK = 7
-    MANUFACTURER = 8
-    DESIGNER = 9
-    DESCRIPTION = 10
-    VENDOR_URL = 11
-    DESIGNER_URL = 12
-    LICENSE_DESCRIPTION = 13
-    LICENSE_URL = 14
-    TYPOGRAPHIC_FAMILY_NAME = 16
-    TYPOGRAPHIC_SUBFAMILY_NAME = 17
-    MAC_FULL_NAME = 18
-    SAMPLE_TEXT = 19
-    POSTSCRIPT_CID_FINDFONT_NAME = 20
-    WWS_FAMILY_NAME = 21
-    WWS_SUBFAMILY_NAME = 22
-    LIGHT_BACKGROUND = 23
-    DARK_BACKGROUND = 24
-    VARIATIONS_PREFIX_NAME = 25
+from typing import Any, Dict, List, Optional, Set, Tuple
 
 
 class FontParser:
+    """
+    A utility class providing static methods for proper font parsing.
+    """
+
     DEFAULT_WEIGHT = 400
     DEFAULT_ITALIC = False
-
-    CMAP_ENCODING_MAP = {
-        1: {  # Mac
+    CMAP_ENCODING_MAP: Dict[PlatformID, Dict[int, str]] = {
+        PlatformID.MACINTOSH: {
             0: "mac_roman",
         },
-        3: {  # Microsoft
+        PlatformID.MICROSOFT: {
             0: "unknown",
             1: "unicode",
             2: "cp932",
             3: "cp936",
             4: "cp950",
             5: "cp949",
             6: "cp1361",
             10: "unicode",
         },
     }
 
-    @staticmethod
-    def is_truetype(font: TTFont) -> bool:
-        """
-        Parameters:
-            font (TTFont): An fontTools object
-        Returns:
-            An boolean that indicate if the font is an Truetype font or not.
-            If not, then, it is an Opentype font.
-        """
-        return "glyf" in font
 
     @staticmethod
     def is_valid_variable_font(font: TTFont) -> bool:
         """
-        Parameters:
-            font (TTFont): An fontTools object
+        Args:
+            font: The font to be validated
         Returns:
             An boolean that indicate if the font is an variable font or not.
         """
 
         if "fvar" not in font or "STAT" not in font:
             return False
 
         if font["STAT"].table is None:
             return False
 
+        if font["STAT"].table.DesignAxisRecord is None:
+            raise InvalidVariableFontFaceException("The font has a stat table, but it doesn't have any DesignAxisRecord")
+
         for axe in font["fvar"].axes:
             if not (axe.minValue <= axe.defaultValue <= axe.maxValue):
                 return False
 
         if font["STAT"].table.AxisValueArray is not None:
             for axis_value in font["STAT"].table.AxisValueArray.AxisValue:
                 if axis_value.Format in (1, 2, 3, 4):
@@ -100,54 +73,57 @@
                         return False
                 else:
                     return False
 
         return True
 
     @staticmethod
-    def get_var_font_family_prefix(font: TTFont) -> str:
-        """
-        From: https://github.com/fonttools/fonttools/blob/3c4cc71504774d1ae4f1e59e3ef3b97e194c1c91/Lib/fontTools/varLib/instancer/names.py#L267-L269
+    def get_var_font_family_prefix(names: List[NameRecord], platform_id: PlatformID) -> List[Name]:
+        """Extracts variable font family prefix names based on the provided NameRecord list and platform ID.
 
-        Parameters:
-            font (TTFont): An fontTools object
+        Args:
+            names: A list of NameRecord objects.
+            platform_id: The platform ID specifying the target platform for family name extraction.
         Returns:
-            The family name prefix.
+            A list of Name objects representing variable font family prefix names.
         """
-        try:
-            family_prefix = FontParser.get_name_by_id(
-                NameID.TYPOGRAPHIC_FAMILY_NAME, font["name"].names
-            )
-        except NameNotFoundException:
-            family_prefix = FontParser.get_name_by_id(
-                NameID.FAMILY_NAME, font["name"].names
-            )
+        family_prefix = FontParser.get_filtered_names(names, platformID=platform_id, nameID=NameID.TYPOGRAPHIC_FAMILY_NAME)
+
+        if not family_prefix:
+            family_prefix = FontParser.get_filtered_names(names, platformID=platform_id, nameID=NameID.FAMILY_NAME)
 
         return family_prefix
 
     @staticmethod
     def get_distance_between_axis_value_and_coordinates(
         font: TTFont, coordinates: Dict[str, float], axis_value: Any, axis_format: int
     ) -> float:
-        """
-        Parameters:
-            ttfont (TTFont): An fontTools object
-            coordinates (Dict[str, float]): The coordinates of an NamedInstance in the fvar table.
-            axis_value (Any): An AxisValue
-            axis_format (int): The AxisValue Format.
-                Since the AxisValue from AxisValueRecord of an AxisValue Format 4 doesn't contain an Format attribute, this parameter is needed.
+        """Calculate the distance between an axis value and coordinates of a NamedInstance in a variable font.
+
+        This method is inspired by how GDI parses Variable Fonts. Ensure to call FontParser.is_valid_variable_font()
+        before using this method.
+
+        Args:
+            font: A fontTools object representing the font.
+            coordinates: The coordinates of a NamedInstance in the fvar table.
+            axis_value: An AxisValue object representing the font axis value.
+                Even if the type is Any, it isn't. It is AxisValueRecord, but fontTools create this class dynamically.
+            axis_format (int): The AxisValue format.
         Returns:
-            The distance between_axis_value_and_coordinates
+            The calculated distance between the specified axis value and coordinates.
         """
+        try:
+            axis_tag = font["STAT"].table.DesignAxisRecord.Axis[axis_value.AxisIndex].AxisTag
+        except IndexError:
+            raise InvalidVariableFontFaceException(f"The DesignAxisRecord doesn't contain an axis at the index {axis_value.AxisIndex}")
 
-        axis_tag = (
-            font["STAT"].table.DesignAxisRecord.Axis[axis_value.AxisIndex].AxisTag
-        )
+        # If the coordinates cannot be found, default to 0
         instance_value = coordinates.get(axis_tag, 0)
 
+        clamped_axis_value: float
         if axis_format == 2:
             clamped_axis_value = max(
                 min(instance_value, axis_value.RangeMaxValue),
                 axis_value.RangeMinValue,
             )
         else:
             clamped_axis_value = axis_value.Value
@@ -160,58 +136,57 @@
         else:
             adjust = 0
 
         distance = delta_square * 2 + adjust
 
         return distance
 
+
     @staticmethod
-    def get_axis_value_from_coordinates(
-        ttfont: TTFont, coordinates: Dict[str, float]
-    ) -> List[Any]:
-        """
-        Parameters:
-            ttfont (TTFont): An fontTools object
-            coordinates (Dict[str, float]): The coordinates of an NamedInstance in the fvar table.
+    def get_axis_value_from_coordinates(font: TTFont, coordinates: Dict[str, float]) -> List[Any]:
+        """Retrieve AxisValue objects linked to the specified coordinates in the fvar table.
+        Ensure to call FontParser.is_valid_variable_font() before using this method.
+
+        Args:
+            font: A fontTools object representing the font.
+            coordinates: The coordinates of a NamedInstance in the fvar table.
         Returns:
-            An list who contain all the AxisValue linked to the coordinates.
+            A list containing all the AxisValue objects that has the closest distance
+            to the provided coordinates.
         """
-
         distances_for_axis_values: List[Tuple[float, Any]] = []
 
-        if ttfont["STAT"].table.AxisValueArray is None:
+        if font["STAT"].table.AxisValueArray is None:
             return distances_for_axis_values
 
-        for axis_value in ttfont["STAT"].table.AxisValueArray.AxisValue:
+        for axis_value in font["STAT"].table.AxisValueArray.AxisValue:
 
             if axis_value.Format == 4:
-                distance = 0
+                distance = 0.0
 
                 for axis_value_format_4 in axis_value.AxisValueRecord:
                     distance += (
                         FontParser.get_distance_between_axis_value_and_coordinates(
-                            ttfont, coordinates, axis_value_format_4, axis_value.Format
+                            font, coordinates, axis_value_format_4, axis_value.Format
                         )
                     )
 
                 distances_for_axis_values.append((distance, axis_value))
 
             else:
                 distance = FontParser.get_distance_between_axis_value_and_coordinates(
-                    ttfont, coordinates, axis_value, axis_value.Format
+                    font, coordinates, axis_value, axis_value.Format
                 )
                 distances_for_axis_values.append((distance, axis_value))
 
         # Sort by ASC
         distances_for_axis_values.sort(key=lambda distance: distance[0])
 
         axis_values_coordinate_matches: List[Any] = []
-        is_axis_useds: List[bool] = [False] * len(
-            ttfont["STAT"].table.DesignAxisRecord.Axis
-        )
+        is_axis_useds: List[bool] = [False] * len(font["STAT"].table.DesignAxisRecord.Axis)
 
         for distance, axis_value in distances_for_axis_values:
             if axis_value.Format == 4:
 
                 # The AxisValueRecord can have "internal" duplicate axis, but it cannot have duplicate Axis with the other AxisValue
                 is_any_duplicate_axis = False
                 for axis_value_format_4 in axis_value.AxisValueRecord:
@@ -227,293 +202,214 @@
             else:
                 if not is_axis_useds[axis_value.AxisIndex]:
                     is_axis_useds[axis_value.AxisIndex] = True
                     axis_values_coordinate_matches.append(axis_value)
 
         return axis_values_coordinate_matches
 
+
     @staticmethod
     def get_axis_value_table_property(
-        ttfont: TTFont, axis_values: List[Any], family_name_prefix: str
-    ) -> Tuple[str, str, float, bool]:
-        """
-        Parameters:
-            ttfont (TTFont): An fontTools object
-            axis_values (List[Any]): An list of AxisValue.
-            family_name_prefix (str): The variable family name prefix.
-                Ex: For the name "Alegreya Italic", "Alegreya" is the family name prefix.
+        font: TTFont, axis_values: List[Any]
+    ) -> Tuple[List[Name], List[Name], float, bool]:
+        """Retrieve font properties such as family name, full name, weight, and italic based on axis values.
+        Ensure to call FontParser.is_valid_variable_font() before using this method.
+
+        Args:
+            font: A fontTools object representing the font.
+            axis_values: A list of AxisValue object representing the font axis value.
         Returns:
-            An FontFace that represent the axis_values.
+            A tuple containing the family name, the full name, the weight, and italic.
         """
-
         axis_values.sort(
-            key=lambda axis_value: ttfont["STAT"]
+            key=lambda axis_value: font["STAT"]
             .table.DesignAxisRecord.Axis[
                 min(
                     axis_value.AxisValueRecord,
-                    key=lambda axis_value_format_4: ttfont["STAT"]
+                    key=lambda axis_value_format_4: font["STAT"]
                     .table.DesignAxisRecord.Axis[axis_value_format_4.AxisIndex]
                     .AxisOrdering,
                 ).AxisIndex
             ]
             .AxisOrdering
             if axis_value.Format == 4
-            else ttfont["STAT"]
+            else font["STAT"]
             .table.DesignAxisRecord.Axis[axis_value.AxisIndex]
             .AxisOrdering
         )
 
-        family_axis_value = []
-        fullname_axis_value = []
         weight = FontParser.DEFAULT_WEIGHT
         italic = FontParser.DEFAULT_ITALIC
 
-        for axis_value in axis_values:
+        axis_values_names: List[List[Name]] = []
+        family_name_axis_value_index: List[bool] = [False] * len(axis_values)
+        fullname_axis_value_index: List[bool] = [False] * len(axis_values)
+
+
+        for i, axis_value in enumerate(axis_values):
+
+            axis_value_name = FontParser.get_filtered_names(font["name"].names, platformID=PlatformID.MICROSOFT, nameID=axis_value.ValueNameID)
+            if not axis_value_name:
+                raise InvalidVariableFontFaceException("An axis value has an invalid ValueNameID")
+            axis_values_names.append(axis_value_name)
 
             # If the Format 4 only contain only 1 AxisValueRecord, it will treat it as an single AxisValue like the Format 1, 2 or 3.
             if axis_value.Format == 4 and len(axis_value.AxisValueRecord) > 1:
-                if not axis_value.Flags & ELIDABLE_AXIS_VALUE_NAME:
-                    family_axis_value.append(axis_value)
-                    fullname_axis_value.append(axis_value)
+                if not (axis_value.Flags & ELIDABLE_AXIS_VALUE_NAME):
+                    family_name_axis_value_index[i] = True
+                    fullname_axis_value_index[i] = True
             else:
                 if axis_value.Format == 2:
                     value = axis_value.NominalValue
                     axis_index = axis_value.AxisIndex
                 elif axis_value.Format in (1, 3):
                     value = axis_value.Value
                     axis_index = axis_value.AxisIndex
                 elif axis_value.Format == 4:
                     value = axis_value.AxisValueRecord[0].Value
                     axis_index = axis_value.AxisValueRecord[0].AxisIndex
 
-                if (
-                    ttfont["STAT"].table.DesignAxisRecord.Axis[axis_index].AxisTag
-                    == "wght"
-                ):
+                if font["STAT"].table.DesignAxisRecord.Axis[axis_index].AxisTag == "wght":
                     weight = value
-                elif (
-                    ttfont["STAT"].table.DesignAxisRecord.Axis[axis_index].AxisTag
-                    == "ital"
-                ):
+                elif font["STAT"].table.DesignAxisRecord.Axis[axis_index].AxisTag == "ital":
                     italic = value == 1
 
                 if not (axis_value.Flags & ELIDABLE_AXIS_VALUE_NAME):
-                    fullname_axis_value.append(axis_value)
+                    fullname_axis_value_index[i] = True
 
                     use_in_family_name = True
-                    if (
-                        ttfont["STAT"].table.DesignAxisRecord.Axis[axis_index].AxisTag
-                        == "wght"
-                    ):
+                    if font["STAT"].table.DesignAxisRecord.Axis[axis_index].AxisTag == "wght":
                         use_in_family_name = value not in (400, 700)
-                    elif (
-                        ttfont["STAT"].table.DesignAxisRecord.Axis[axis_index].AxisTag
-                        == "ital"
-                    ):
+                    elif font["STAT"].table.DesignAxisRecord.Axis[axis_index].AxisTag == "ital":
                         use_in_family_name = value not in (0, 1)
 
                     if use_in_family_name:
-                        family_axis_value.append(axis_value)
+                        family_name_axis_value_index[i] = True
 
-        try:
-            family_name = f'{family_name_prefix} {" ".join(FontParser.get_name_by_id(axis_value.ValueNameID, ttfont["name"].names) for axis_value in family_axis_value)}'.strip(
-                " "
-            )
-        except NameNotFoundException:
-            family_name = family_name_prefix
+        family_name: List[Name] = []
+        fullname: List[Name] = []
 
-        if len(fullname_axis_value) == 0:
-            try:
-                full_name = f"{family_name_prefix} {FontParser.get_name_by_id(ttfont['STAT'].table.ElidedFallbackNameID, ttfont['name'].names)}".strip(
-                    " "
-                )
-            except NameNotFoundException:
-                weight = FontParser.DEFAULT_WEIGHT
-                italic = FontParser.DEFAULT_ITALIC
-                full_name = f"{family_name_prefix} Regular"
-
-        else:
-            try:
-                full_name = f'{family_name_prefix} {" ".join(FontParser.get_name_by_id(axis_value.ValueNameID, ttfont["name"].names) for axis_value in fullname_axis_value)}'.strip(
-                    " "
-                )
-            except NameNotFoundException:
-                weight = FontParser.DEFAULT_WEIGHT
-                italic = FontParser.DEFAULT_ITALIC
+        # Generate family_name an fullname
+        for item in product(*axis_values_names):
+            langs: Set[Language] = set()
+            for element in item:
+                langs.add(element.lang_code)
+
+            family_name_str = " ".join([element.value for i, element in enumerate(item) if family_name_axis_value_index[i]])
+            fullname_str = " ".join([element.value for i, element in enumerate(item) if fullname_axis_value_index[i]])
+
+            family_name.extend([Name(family_name_str, lang) for lang in langs])
+            fullname.extend([Name(fullname_str, lang) for lang in langs])
+
+        if all(not element for element in fullname_axis_value_index):
+            # Fallback if all the element have the flag ELIDABLE_AXIS_VALUE_NAME
+            if hasattr(font['STAT'].table, "ElidedFallbackNameID"):
+                elided_fallback_name = FontParser.get_filtered_names(font['name'].names, platformID=PlatformID.MICROSOFT, nameID=font['STAT'].table.ElidedFallbackNameID)
 
-                try:
-                    full_name = f"{family_name_prefix} {FontParser.get_name_by_id(ttfont['STAT'].table.ElidedFallbackNameID, ttfont['name'].names)}".strip(
-                        " "
-                    )
-                except NameNotFoundException:
-                    full_name = f"{family_name_prefix} Regular"
+                if elided_fallback_name:
+                    fullname = elided_fallback_name
+                else:
+                    # The elided_fallback_name haven't been found
+                    weight = FontParser.DEFAULT_WEIGHT
+                    italic = FontParser.DEFAULT_ITALIC
+                    fullname = [Name(f"Regular", Language.get("en-US"))]
+            else:
+                fullname = [Name(f"Normal", Language.get("en-US"))]
 
-        return family_name, full_name, weight, italic
+        # Remove duplicate name while preserving the order
+        family_name = list(dict.fromkeys(family_name))
+        fullname = list(dict.fromkeys(fullname))
+
+        return family_name, fullname, weight, italic
 
-    @staticmethod
-    def sort_naming_table(names: List[NameRecord]) -> List[NameRecord]:
-        """
-        Parameters:
-            names (List[NameRecord]): Naming table
-        Returns:
-            The sorted naming table
-        """
-
-        def is_english(name: NameRecord) -> bool:
-            # From https://gitlab.freedesktop.org/fontconfig/fontconfig/-/blob/d863f6778915f7dd224c98c814247ec292904e30/src/fcfreetype.c#L1111-1125
-            return (name.platformID, name.langID) in ((1, 0), (3, 0x409))
-
-        # From	https://gitlab.freedesktop.org/fontconfig/fontconfig/-/blob/d863f6778915f7dd224c98c814247ec292904e30/src/fcfreetype.c#L1078
-        # 		https://github.com/freetype/freetype/blob/b98dd169a1823485e35b3007ce707a6712dcd525/include/freetype/ttnameid.h#L86-L91
-        PLATFORM_ID_APPLE_UNICODE = 0
-        PLATFORM_ID_MACINTOSH = 1
-        PLATFORM_ID_ISO = 2
-        PLATFORM_ID_MICROSOFT = 3
-        PLATFORM_ID_ORDER = [
-            PLATFORM_ID_MICROSOFT,
-            PLATFORM_ID_APPLE_UNICODE,
-            PLATFORM_ID_MACINTOSH,
-            PLATFORM_ID_ISO,
-        ]
-
-        return sorted(
-            names,
-            key=lambda name: (
-                PLATFORM_ID_ORDER.index(name.platformID),
-                name.nameID,
-                name.platEncID,
-                -is_english(name),
-                name.langID,
-            ),
-        )
 
     @staticmethod
-    def get_name_by_id(nameID: int, names: List[NameRecord]) -> str:
-        """
-        Parameters:
-            nameID (int): ID of the name you search
-            names (List[NameRecord]): Naming table
-        Returns:
-            The decoded name
-        """
-
-        names = list(filter(lambda name: name.nameID == nameID, names))
-        names = FontParser.sort_naming_table(names)
-
-        for name in names:
-            try:
-                name_str = FontParser.get_decoded_name(name)
-            except UnicodeDecodeError:
-                continue
+    def get_filtered_names(
+        names_record: List[NameRecord],
+        platformID: Optional[PlatformID] = None,
+        platEncID: Optional[int] = None,
+        nameID: Optional[NameID] = None,
+        langID: Optional[int] = None,
+        skip_unsupported_name_record: bool = True
+    ) -> List[Name]:
+        """Retrieve and decode NameRecord objects based on specified filtering criteria.
+        Is it the same criteria has: https://learn.microsoft.com/en-us/typography/opentype/spec/name#name-records
+
+        Args:
+            names_record: A list of NameRecord objects representing the naming table.
+            platformID: Filter the names_record by platformID.
+            platEncID: Filter the names_record by platEncID.
+            nameID: Filter the names_record by nameID.
+            langID: Filter the names_record by langID.
+            skip_unsupported_name_record: When trying to decode NameRecord, the exception InvalidNameRecord can be raised.
+                If this argument is true, then it will ignore the exception and discard the NameRecord.
+        Returns:
+            A list of the decoded NameRecord objects that have been filtered.
+        """
+        names: List[Name] = []
+
+        for name_record in names_record:
+            if (
+                (platformID is None or name_record.platformID == platformID) and
+                (platEncID is None or name_record.platEncID == platEncID) and
+                (nameID is None or name_record.nameID == nameID) and
+                (langID is None or name_record.langID == langID)
+            ):
+                try:
+                    names.append(Name.from_name_record(name_record))
+                except InvalidNameRecord:
+                    if not skip_unsupported_name_record:
+                        raise
 
-            return name_str
+        return names
 
-        raise NameNotFoundException(
-            f"The NamingTable doesn't contain the NameID {nameID}"
-        )
 
     @staticmethod
-    def get_decoded_name(name: NameRecord) -> str:
+    def get_font_italic_bold_property_with_freetype(
+        font_path: Path, font_index: int
+    ) -> Tuple[bool, bool, int]:
         """
-        Parameters:
-            names (NameRecord): Name record from the naming record
+        Args:
+            font_path: Font path.
+            font_index: Font index.
         Returns:
-            The decoded name
+            is_italic, is_glyphs_emboldened, weight
         """
+        font = Face(font_path.open("rb"), font_index)
+        is_italic = bool(font.style_flags & FT_STYLE_FLAGS["FT_STYLE_FLAG_ITALIC"])
+        is_glyphs_emboldened = bool(font.style_flags & FT_STYLE_FLAGS["FT_STYLE_FLAG_BOLD"])
+        weight = 700 if is_glyphs_emboldened else 400
 
-        encoding = FontParser.get_name_encoding(name)
+        return is_italic, is_glyphs_emboldened, weight
 
-        if name.platformID == 3 and encoding != "utf_16_be":
-            # I spoke with a Microsoft employee and he told me that GDI performed this processing:
-            name_to_decode = name.string.replace(b"\x00", b"")
-        else:
-            name_to_decode = name.string
-
-        return name_to_decode.decode(encoding)
 
     @staticmethod
-    def get_font_postscript_property(font_path: str, font_index: int) -> Optional[str]:
+    def get_font_italic_bold_property_microsoft_platform(
+        font: TTFont, font_path: Path, font_index: int
+    ) -> Tuple[bool, bool, int]:
         """
-        Parameters:
-            font_path (str): Font path.
-            font_index (int): Font index.
+        Args:
+            font: An fontTools object
+            font_path: Font path.
+            font_index: Font index.
         Returns:
-            The postscript name
+            is_italic, is_glyphs_emboldened, weight
         """
-        try:
-            # Like libass, we use freetype: https://github.com/libass/libass/blob/a2b39cde4ecb74d5e6fccab4a5f7d8ad52b2b1a4/libass/ass_fontselect.c#L326
-            postscriptNameByte = freetype.Face(
-                Path(font_path).open("rb"), font_index
-            ).postscript_name
-        except OSError:
-            _logger.warning(
-                f'Error: Please report this error on github. Attach this font "{font_path}" in your issue and say that the postscript has not been correctly decoded'
-            )
-
-        if postscriptNameByte is not None:
-            try:
-                postscriptName = postscriptNameByte.decode("ASCII")
-            except UnicodeDecodeError:
-                _logger.warning(
-                    f'Error: Please report this error on github. Attach this font "{font_path}" in your issue and say that the postscript has not been correctly decoded'
-                )
-
-            if postscriptName is not None:
-                return postscriptName
-
-        return None
-
-    @staticmethod
-    def get_font_italic_bold_property(
-        font: TTFont, font_path: str, font_index: int
-    ) -> Tuple[bool, int]:
-        """
-        Parameters:
-            font (TTFont): An fontTools object
-            font_path (str): Font path.
-            font_index (int): Font index.
-        Returns:
-            is_italic, weight
-        """
-
-        def get_font_italic_bold_property_with_freetype(
-            font_path: str, font_index: int
-        ) -> Tuple[bool, int]:
-            font = freetype.Face(Path(font_path).open("rb"), font_index)
-            # From: https://github.com/libass/libass/blob/a2b39cde4ecb74d5e6fccab4a5f7d8ad52b2b1a4/libass/ass_fontselect.c#L318
-            is_italic = bool(
-                font.style_flags & freetype.ft_enums.ft_style_flags.FT_STYLE_FLAG_ITALIC
-            )
-            # From: https://github.com/libass/libass/blob/a2b39cde4ecb74d5e6fccab4a5f7d8ad52b2b1a4/libass/ass_font.c#L523
-            weight = (
-                700
-                if bool(
-                    font.style_flags
-                    & freetype.ft_enums.ft_style_flags.FT_STYLE_FLAG_BOLD
-                )
-                else 400
-            )
-
-            return is_italic, weight
 
         if "OS/2" in font:
             try:
                 # https://docs.microsoft.com/en-us/typography/opentype/spec/os2#fss
                 is_italic = bool(font["OS/2"].fsSelection & 1)
-
+                is_glyphs_emboldened = bool(font["OS/2"].fsSelection & 1 << 5)
                 # https://docs.microsoft.com/en-us/typography/opentype/spec/os2#usweightclass
                 weight = font["OS/2"].usWeightClass
             except struct_error:
-                is_italic, weight = get_font_italic_bold_property_with_freetype(
-                    font_path, font_index
-                )
+                is_italic, is_glyphs_emboldened, weight = FontParser.get_font_italic_bold_property_with_freetype(font_path, font_index)
         else:
-            is_italic, weight = get_font_italic_bold_property_with_freetype(
-                font_path, font_index
-            )
+            is_italic, is_glyphs_emboldened, weight = FontParser.get_font_italic_bold_property_with_freetype(font_path, font_index)
 
         # See https://github.com/libass/libass/pull/676
         if weight == 1:
             weight = 100
         elif weight == 2:
             weight = 200
         elif weight == 3:
@@ -527,180 +423,154 @@
         elif weight == 7:
             weight = 700
         elif weight == 8:
             weight = 800
         elif weight == 9:
             weight = 900
 
-        return is_italic, weight
+        return is_italic, is_glyphs_emboldened, weight
+
 
     @staticmethod
-    def get_font_family_fullname_property(
-        names: List[NameRecord],
-    ) -> Tuple[Set[str], Set[str]]:
+    def get_font_italic_bold_property_mac_platform(
+        font: TTFont, font_path: Path, font_index: int
+    ) -> Tuple[bool, bool, int]:
         """
-        Parameters:
-            names (List[NameRecord]): Naming table
+        Args:
+            font: An fontTools object
+            font_path: Font path.
+            font_index: Font index.
         Returns:
-            All decoded families and fullnames that are from microsoft platform
+            is_italic, is_glyphs_emboldened, weight
         """
+        if "head" in font:
+            try:
+                # https://learn.microsoft.com/en-us/typography/opentype/spec/head
+                # https://github.com/libass/libass/issues/679#issuecomment-1404520010
+                is_italic = bool(font["head"].macStyle & 1 << 1)
+                is_glyphs_emboldened = bool(font["head"].macStyle & 1)
+                weight = 800 if is_glyphs_emboldened else 400
+            except struct_error:
+                is_italic, is_glyphs_emboldened, weight = FontParser.get_font_italic_bold_property_with_freetype(font_path, font_index)
+        else:
+            is_italic, is_glyphs_emboldened, weight = FontParser.get_font_italic_bold_property_with_freetype(font_path, font_index)
 
-        # https://github.com/libass/libass/blob/a2b39cde4ecb74d5e6fccab4a5f7d8ad52b2b1a4/libass/ass_fontselect.c#L258-L344
-        MAX = 100
-        families = set()
-        fullnames = set()
-
-        for name in names:
-
-            if name.platformID == 3 and (
-                name.nameID == NameID.FAMILY_NAME or name.nameID == NameID.FULL_NAME
-            ):
-
-                try:
-                    name_str = FontParser.get_decoded_name(name)
-                except UnicodeDecodeError:
-                    continue
-
-                if name.nameID == 1 and len(families) < MAX:
-                    families.add(name_str)
-                elif name.nameID == 4 and len(fullnames) < MAX:
-                    fullnames.add(name_str)
-
-        return families, fullnames
+        return is_italic, is_glyphs_emboldened, weight
 
 
     @staticmethod
     def get_symbol_cmap_encoding(face: FT_Face) -> Optional[str]:
         """
-        Parameters:
-            face (FT_Face): An Font face
+        Args:
+            face: An Font face
         Returns:
             The cmap ansi code page encoding.
             If it couldn't guess the encoding, it return None.
-                It can return none if the font is those case if the font doesn't use any unique character of an ansi code page.
+                It can return none if the font doesn't use any unique character of an ansi code page.
                     Note: Chinese (cp936 or cp950) and Korean (cp949) doesn't contain any unique character.
                           So, we can't recognized them.
             Libass currently has an issue about this problem: https://github.com/libass/libass/issues/319
             When Libass will add the logic with the track language, this method will be deprecated.
         """
         font_glyph_names: Set[str] = set()
         # This is a limit set by adobe: http://adobe-type-tools.github.io/afdko/OpenTypeFeatureFileSpecification.html#2fi-glyph-name
         buffer_max = 64
         for i in range(face.contents.num_glyphs):
             buffer = create_string_buffer(buffer_max)
             error = FT_Get_Glyph_Name(face, c_uint(i), byref(buffer), c_uint(buffer_max))
 
             if error:
                 continue
-            font_glyph_names.add(buffer.value.decode("ascii").lower())
+            font_glyph_names.add(buffer.value.decode("ascii").casefold())
 
-        count_codepage: dict[str, int] = {}
+        count_codepage: Dict[str, int] = {}
         for code_page, glyph_names in UNIQUE_ADOBE_GLYPH_NAME_BY_CODE_PAGE.items():
             count = sum(1 for font_glyph_name in font_glyph_names if font_glyph_name in glyph_names)
             count_codepage[code_page] = count
+
+        if len(count_codepage) == 0:
+            return None
         # If there is a tie, prefer codepage different then cp1252
         codepage_encoding = max(count_codepage, key=lambda codepage: (count_codepage[codepage], codepage != 'cp1252'))
 
-        if count_codepage[codepage_encoding]:
-            return codepage_encoding
-
-        return None
+        return codepage_encoding
 
 
     @staticmethod
-    def get_cmap_encoding(platform_id: int, encoding_id: int) -> Optional[str]:
-        """
-        Parameters:
-            platform_id (int): CMAP platform id
-            encoding_id (int): CMAP encoding id
-        Returns:
-            The cmap codepoint encoding.
-            If GDI does not support the platform_id and/or platform_encoding_id, return None.
+    def get_supported_cmaps(font: TTFont) -> List[CMap]:
         """
-        return FontParser.CMAP_ENCODING_MAP.get(platform_id, {}).get(encoding_id, None)
+        Retrieve supported CMaps from a TrueType font.
 
-    @staticmethod
-    def get_name_encoding(name: NameRecord) -> Optional[str]:
-        """
-        Parameters:
-            names (NameRecord): Name record from the naming record
+        Args:
+            font: A fontTools object representing the font.
         Returns:
-            The cmap codepoint encoding.
-            If GDI does not support the name, return None.
+            A list of supported CMaps.
+            - To determine which CMaps are supported, refer to FontParser.get_cmap_encoding().
+            - If any Microsoft CMaps are present, only those will be returned.
+            - If no Microsoft CMaps are found, the method will only return Macintosh CMaps if they are present.
         """
-        # From: https://github.com/MicrosoftDocs/typography-issues/issues/956#issuecomment-1205678068
-        if name.platformID == 3:
-            if name.platEncID == 3:
-                return "cp936"
-            elif name.platEncID == 4:
-                if name.nameID == 2:
-                    return "utf_16_be"
-                else:
-                    return "cp950"
-            elif name.platEncID == 5:
-                if name.nameID == 2:
-                    return "utf_16_be"
-                else:
-                    return "cp949"
-            else:
-                return "utf_16_be"
-        elif name.platformID == 1 and name.platEncID == 0:
-            # From: https://github.com/libass/libass/issues/679#issuecomment-1442262479
-            return "iso-8859-1"
+        microsoft_cmaps: List[CMap] = []
+        macintosh_cmaps: List[CMap] = []
 
-        return None
+        cmap_tables: List[CmapSubtable] = font["cmap"].tables
 
-    @staticmethod
-    def is_file_truetype_collection(file: BufferedReader) -> bool:
-        file.seek(0)
-        return b"ttcf" == file.read(4)
+        for table in cmap_tables:
+            encoding = FontParser.get_cmap_encoding(table.platformID, table.platEncID)
+            if encoding is not None:
+                cmap = CMap(table.platformID, table.platEncID)
+                if table.platformID == PlatformID.MICROSOFT:
+                    microsoft_cmaps.append(cmap)
+                elif table.platformID == PlatformID.MACINTOSH:
+                    macintosh_cmaps.append(cmap)
+        return macintosh_cmaps if len(microsoft_cmaps) == 0 else microsoft_cmaps
 
-    @staticmethod
-    def is_file_truetype(file: BufferedReader) -> bool:
-        file.seek(0)
-        return b"\x00\x01\x00\x00" == file.read(4)
-
-    @staticmethod
-    def is_file_opentype(file: BufferedReader) -> bool:
-        file.seek(0)
-        return b"OTTO" == file.read(4)
 
     @staticmethod
-    def is_file_font(filepath: str) -> bool:
-        with open(filepath, "rb") as fontFile:
-            return (
-                FontParser.is_file_truetype(fontFile)
-                or FontParser.is_file_opentype(fontFile)
-                or FontParser.is_file_truetype_collection(fontFile)
-            )
+    def get_cmap_encoding(platform_id: int, encoding_id: int) -> Optional[str]:
+        """
+        Args:
+            platform_id: CMap platform id
+            encoding_id: CMap encoding id
+        Returns:
+            The cmap encoding.
+            If GDI does not support the platform_id and/or platform_encoding_id, return None.
+            Warning, if it return "unknown", it means that the cmap is from a symbol font.
+                Call get_symbol_cmap_encoding() to know what is the encoding.
+        Notes:
+            - GDI only supports all encodings for the Microsoft CMap.
+            - For the Macintosh platform, it only supports the platform encoding 1.
+        """
+        if platform_id in FontParser.CMAP_ENCODING_MAP:
+            return FontParser.CMAP_ENCODING_MAP[PlatformID(platform_id)].get(encoding_id, None)
+        return None
 
 
 # The Chinese (cp936 or cp950) and Korean (cp949) aren't in this dict since they doesn't have any unique char.
 # This dict have been generated with "proof/[Symbol Font] Find unique char by ansi code page.py"
 # The name of those glyph is from this list: https://raw.githubusercontent.com/adobe-type-tools/agl-aglfn/4036a9ca80a62f64f9de4f7321a9a045ad0ecfd6/glyphlist.txt
 UNIQUE_ADOBE_GLYPH_NAME_BY_CODE_PAGE: dict[str, Set[str]] = {
-    "cp874": {'angkhankhuthai', 'lolingthai', 'thanthakhatthai', 'phosamphaothai', 'phophanthai', 'paiyannoithai', 'phinthuthai', 'threethai', 'kokaithai', 'topatakthai', 'lochulathai', 'nonuthai', 'thothungthai', 'lakkhangyaothai', 'ngonguthai', 'thothanthai', 'khokhaithai', 'khokhwaithai', 'oangthai', 'sixthai', 'saraueethai', 'saraaathai', 'wowaenthai', 'chochangthai', 'fourthai', 'maihanakatthai', 'nonenthai', 'maiekthai', 'sosalathai', 'sorusithai', 'saraamthai', 'saraethai', 'saraithai', 'fofanthai', 'fofathai', 'poplathai', 'thothongthai', 'roruathai', 'chochingthai', 'nikhahitthai', 'saraiithai', 'yamakkanthai', 'luthai', 'onethai', 'sosothai', 'maitaikhuthai', 'seventhai', 'khorakhangthai', 'yoyingthai', 'sarauthai', 'dochadathai', 'ruthai', 'maichattawathai', 
+    "cp874": {'angkhankhuthai', 'lolingthai', 'thanthakhatthai', 'phosamphaothai', 'phophanthai', 'paiyannoithai', 'phinthuthai', 'threethai', 'kokaithai', 'topatakthai', 'lochulathai', 'nonuthai', 'thothungthai', 'lakkhangyaothai', 'ngonguthai', 'thothanthai', 'khokhaithai', 'khokhwaithai', 'oangthai', 'sixthai', 'saraueethai', 'saraaathai', 'wowaenthai', 'chochangthai', 'fourthai', 'maihanakatthai', 'nonenthai', 'maiekthai', 'sosalathai', 'sorusithai', 'saraamthai', 'saraethai', 'saraithai', 'fofanthai', 'fofathai', 'poplathai', 'thothongthai', 'roruathai', 'chochingthai', 'nikhahitthai', 'saraiithai', 'yamakkanthai', 'luthai', 'onethai', 'sosothai', 'maitaikhuthai', 'seventhai', 'khorakhangthai', 'yoyingthai', 'sarauthai', 'dochadathai', 'ruthai', 'maichattawathai',
     'bobaimaithai', 'sarauethai', 'saraaimaimuanthai', 'chochoethai', 'twothai', 'sarauuthai', 'phophungthai', 'saraothai', 'khomutthai', 'thophuthaothai', 'fongmanthai', 'fivethai', 'honokhukthai', 'zerothai', 'maiyamokthai', 'hohipthai', 'khokhonthai', 'ninethai', 'bahtthai', 'saraaethai', 'dodekthai', 'chochanthai', 'eightthai', 'yoyakthai', 'khokhuatthai', 'saraaimaimalaithai', 'maithothai', 'thothahanthai', 'sosuathai', 'saraathai', 'totaothai', 'maitrithai', 'momathai', 'thonangmonthothai'},
 
     "cp932": {'nekatakanahalfwidth', 'okatakanahalfwidth', 'yukatakanahalfwidth', 'sekatakanahalfwidth', 'hakatakanahalfwidth', 'sakatakanahalfwidth', 'yokatakanahalfwidth', 'mekatakanahalfwidth', 'osmallkatakanahalfwidth', 'sokatakanahalfwidth', 'wakatakanahalfwidth', 'hokatakanahalfwidth', 'ismallkatakanahalfwidth', 'rakatakanahalfwidth', 'katahiraprolongmarkhalfwidth', 'ikatakanahalfwidth', 'nakatakanahalfwidth', 'mikatakanahalfwidth', 'kikatakanahalfwidth', 'tikatakanahalfwidth', 'tusmallkatakanahalfwidth', 'semivoicedmarkkanahalfwidth', 'sikatakanahalfwidth', 'middledotkatakanahalfwidth', 'mokatakanahalfwidth', 'ekatakanahalfwidth', 'hekatakanahalfwidth', 'tekatakanahalfwidth', 'wokatakanahalfwidth', 'makatakanahalfwidth', 'asmallkatakanahalfwidth', 'tokatakanahalfwidth', 'cornerbracketlefthalfwidth', 'mukatakanahalfwidth', 'kukatakanahalfwidth', 'yusmallkatakanahalfwidth', 'yosmallkatakanahalfwidth', 'nokatakanahalfwidth', 'kekatakanahalfwidth', 'takatakanahalfwidth', 'rikatakanahalfwidth', 'ukatakanahalfwidth', 'cornerbracketrighthalfwidth', 'braceleftmid', 'esmallkatakanahalfwidth', 'tukatakanahalfwidth', 'rukatakanahalfwidth', 'nukatakanahalfwidth', 'bracelefttp', 'voicedmarkkanahalfwidth', 'rokatakanahalfwidth', 'kokatakanahalfwidth', 'usmallkatakanahalfwidth', 'bracketleftbt', 'hukatakanahalfwidth', 'kakatakanahalfwidth', 'sukatakanahalfwidth', 'hikatakanahalfwidth', 'periodhalfwidth', 'braceleftbt', 'yasmallkatakanahalfwidth', 'nkatakanahalfwidth', 'rekatakanahalfwidth', 'yakatakanahalfwidth', 'ideographiccommaleft', 'akatakanahalfwidth', 'nikatakanahalfwidth'},
 
     "cp1250": {'lacute', 'tcedilla', 'dcaron', 'breve', 'lcaron', 'uhungarumlaut', 'racute', 'tcommaaccent', 'ecaron', 'hungarumlaut', 'uring', 'tcaron', 'ncaron', 'rcaron', 'odblacute', 'udblacute', 'ohungarumlaut'},
 
     "cp1251": {'acyrillic', 'efcyrillic', 'afii10055', 'afii10069', 'afii10097', 'afii10037', 'afii10085', 'afii10053', 'kjecyrillic', 'afii10096', 'afii10019', 'afii10086', 'afii10030', 'afii10034', 'iucyrillic', 'elcyrillic', 'ushortcyrillic', 'afii10052', 'afii10036', 'shchacyrillic', 'iishortcyrillic', 'afii10105', 'afii10061', 'afii10026', 'ercyrillic', 'tecyrillic', 'afii10060', 'afii10106', 'afii10028', 'afii10098', 'afii10042', 'yicyrillic', 'afii10193', 'emcyrillic', 'jecyrillic', 'afii10021', 'afii10054', 'afii10101', 'encyrillic', 'afii10022', 'becyrillic', 'njecyrillic', 'softsigncyrillic', 'afii10075', 'afii10100', 'afii10068', 'afii10089', 'afii10065', 'afii61352', 'iicyrillic', 'iecyrillic', 'afii10088', 'tshecyrillic', 'afii10059', 'vecyrillic', 'zhecyrillic', 'afii10102', 'afii10099', 'iocyrillic', 'pecyrillic', 'afii10050', 'afii10048', 'afii10080', 'gecyrillic', 'afii10035', 'djecyrillic', 'ucyrillic', 'afii10066', 'afii10027', 'afii10045', 'afii10082', 'afii10017', 'afii10076', 'afii10067', 'afii10087', 'iacyrillic', 'afii10024', 'dzhecyrillic', 'afii10058', 'afii10029', 'afii10110', 'afii10084', 'afii10095', 'afii10040', 'yericyrillic', 'afii10072', 'afii10109', 'gjecyrillic', 'ljecyrillic', 'afii10074', 'afii10081', 'dzecyrillic', 'afii10093', 'khacyrillic', 'afii10023', 'afii10079', 'afii10031', 'afii10047', 'escyrillic', 'decyrillic', 'afii10062', 'afii10070', 'afii10049', 'tsecyrillic', 'afii10094', 'afii10025', 'afii10041', 'afii10077', 'afii10073', 'afii10038', 'gheupturncyrillic', 'ereversedcyrillic', 'kacyrillic', 'afii10107', 'afii10108', 'ocyrillic', 'afii10145', 'afii10103', 'afii10032', 'shacyrillic', 'checyrillic', 'afii10090', 'numero', 'zecyrillic', 'afii10104', 'afii10092', 'afii10083', 'afii10056', 'afii10039', 'hardsigncyrillic', 'afii10044', 'afii10078', 'afii10018', 'icyrillic', 'afii10043', 'afii10091', 'afii10046', 'afii10057', 'afii10051', 'afii10071', 'ecyrillic', 'afii10020', 'afii10033'},
 
     "cp1252": {'thorn', 'eth'},
 
     "cp1253": {'sigmafinal', 'iotatonos', 'pi', 'kappa', 'dieresistonos', 'lambda', 'chi', 'sigma', 'delta', 'psi', 'rho', 'sigma1', 'epsilontonos', 'alphatonos', 'epsilon', 'beta', 'deltagreek', 'zeta', 'iotadieresis', 'upsilontonos', 'afii00208', 'omicrontonos', 'iota', 'alpha', 'omega', 'omicron', 'gamma', 'upsilon', 'omegagreek', 'tonos', 'omegatonos', 'upsilondieresistonos', 'theta', 'nu', 'dialytikatonos', 'phi', 'mu', 'etatonos', 'iotadieresistonos', 'tau', 'upsilondieresis', 'horizontalbar', 'xi', 'eta', 'mugreek'},
 
     "cp1254": {'gbreve', 'dotlessi', 'idot', 'idotaccent'},
 
-    "cp1255": {'daletsegol', 'het', 'vav', 'reshhatafpatahhebrew', 'reshtserehebrew', 'zayinhebrew', 'tsere12', 'hatafsegolhebrew', 'reshholam', 'afii57678', 'tsere', 'qamatsqatanhebrew', 'daletpatah', 'qamatsqatanquarterhebrew', 'daletholamhebrew', 'finaltsadi', 'afii57668', 'pehebrew', 'mem', 'afii57803', 'qubutsquarterhebrew', 'rafe', 'qamats', 'hiriqhebrew', 'qoftsere', 'hatafsegol30', 'zayin', 'hiriqquarterhebrew', 'afii57670', 'afii57671', 'afii57801', 'afii57636', 'hatafqamats34', 'patahquarterhebrew', 'qamatswidehebrew', 'dalethiriq', 'qubuts31', 'afii57672', 'hehebrew', 'qofsegolhebrew', 'afii57680', 'holamquarterhebrew', 'reshqamats', 'afii57717', 'qofpatahhebrew', 'qofhiriq', 'tserehebrew', 'hiriq', 'qubutshebrew', 'kafhebrew', 'nun', 'afii57689', 'shindothebrew', 'afii57793', 'qubuts18', 'pe', 'memhebrew', 'yodhebrew', 'daletpatahhebrew', 'finalmemhebrew', 'finalpehebrew', 'hatafsegolquarterhebrew', 'qamatsqatannarrowhebrew', 'afii57645', 'shevaquarterhebrew', 'dalethebrew', 'patahwidehebrew', 'dalethatafsegol', 'lamedholamdageshhebrew', 'afii57664', 'shevahebrew', 'afii57842', 'finalkafsheva', 'tsere1e', 'hiriqnarrowhebrew', 'sheva22', 'tethebrew', 'hatafqamats28', 'hatafqamats', 'segolnarrowhebrew', 'afii57804', 'gershayimhebrew', 'tav', 'nunhebrew', 'holamhebrew', 'afii57716', 'patahnarrowhebrew', 'he', 'rafehebrew', 'qofsegol', 'afii57687', 'hatafqamatsnarrowhebrew', 'qofqamatshebrew', 'dalet', 'qubutswidehebrew', 'vavhebrew', 'qofshevahebrew', 'gimelhebrew', 'dalethiriqhebrew', 'patah', 'sheqelhebrew', 'qofholam', 'ayinhebrew', 'segol13', 'reshhebrew', 'finalnun', 'newsheqelsign', 'hatafsegol', 'hatafsegol24', 'sofpasuqhebrew', 'qamats1c', 'dalethatafpatah', 'reshshevahebrew', 'sheva2e', 'reshhatafsegolhebrew', 'afii57839', 'afii57681', 'hatafqamatsquarterhebrew', 'afii57667', 'lamedhebrew', 'qofpatah', 'tserewidehebrew', 'finalnunhebrew', 'sheva', 'daletqubutshebrew', 'finaltsadihebrew', 'qamatsde', 'tsadihebrew', 'finalkafshevahebrew', 'hatafqamatswidehebrew', 'reshhatafpatah', 'afii57794', 'reshqubuts', 'samekh', 'sheqel', 'finalpe', 'shevawidehebrew', 'segol', 'reshhiriq', 
-    'holamwidehebrew', 'qamatsquarterhebrew', 'lamedholamhebrew', 'afii57841', 'vavyodhebrew', 'hatafqamats1b', 'hatafsegolnarrowhebrew', 'afii57795', 'hatafpatahhebrew', 'qofhatafpatah', 'finalkafqamats', 'shinhebrew', 'afii57684', 'reshqamatshebrew', 'hatafqamatshebrew', 'afii57806', 'shevanarrowhebrew', 'sindothebrew', 'patah2a', 'segolhebrew', 'afii57798', 'qofhatafpatahhebrew', 'afii57800', 'qamatsqatanwidehebrew', 'hiriq14', 'qofqubuts', 'hatafpatah', 'hatafpatahnarrowhebrew', 'reshholamhebrew', 'afii57675', 'samekhhebrew', 'shin', 'tavhebrew', 'holam', 'finalkafhebrew', 'finalkafqamatshebrew', 'afii57679', 'tserequarterhebrew', 'holamnarrowhebrew', 'hatafsegolwidehebrew', 'qamatsnarrowhebrew', 'segolquarterhebrew', 'hatafpatahwidehebrew', 'tet', 'hiriq21', 'qamats27', 'afii57674', 'dalethatafpatahhebrew', 'bet', 'bethebrew', 'afii57685', 'yod', 'lamedholamdagesh', 'gereshhebrew', 'alef', 'daletqubuts', 'segol2c', 'qoftserehebrew', 'afii57677', 'finalkaf', 'daletqamatshebrew', 'ayin', 'hatafpatah16', 'paseqhebrew', 'qubuts25', 'tsere2b', 'afii57802', 'afii57669', 'dalethatafsegolhebrew', 'qofhatafsegolhebrew', 'daletqamats', 'qofholamhebrew', 'qamats10', 'afii57718', 'yodyodhebrew', 'afii57807', 'afii57799', 'qofhiriqhebrew', 'qofqubutshebrew', 'tsadi', 'qubutsnarrowhebrew', 'maqafhebrew', 'reshsegolhebrew', 'holam26', 'sheva15', 'lamedholam', 'vavvavhebrew', 'reshqubutshebrew', 'patah11', 'patah1d', 'kaf', 'daletshevahebrew', 'qamats1a', 'sheva115', 'dalettserehebrew', 'qofsheva', 'hethebrew', 'segol1f', 'hiriq2d', 
+    "cp1255": {'daletsegol', 'het', 'vav', 'reshhatafpatahhebrew', 'reshtserehebrew', 'zayinhebrew', 'tsere12', 'hatafsegolhebrew', 'reshholam', 'afii57678', 'tsere', 'qamatsqatanhebrew', 'daletpatah', 'qamatsqatanquarterhebrew', 'daletholamhebrew', 'finaltsadi', 'afii57668', 'pehebrew', 'mem', 'afii57803', 'qubutsquarterhebrew', 'rafe', 'qamats', 'hiriqhebrew', 'qoftsere', 'hatafsegol30', 'zayin', 'hiriqquarterhebrew', 'afii57670', 'afii57671', 'afii57801', 'afii57636', 'hatafqamats34', 'patahquarterhebrew', 'qamatswidehebrew', 'dalethiriq', 'qubuts31', 'afii57672', 'hehebrew', 'qofsegolhebrew', 'afii57680', 'holamquarterhebrew', 'reshqamats', 'afii57717', 'qofpatahhebrew', 'qofhiriq', 'tserehebrew', 'hiriq', 'qubutshebrew', 'kafhebrew', 'nun', 'afii57689', 'shindothebrew', 'afii57793', 'qubuts18', 'pe', 'memhebrew', 'yodhebrew', 'daletpatahhebrew', 'finalmemhebrew', 'finalpehebrew', 'hatafsegolquarterhebrew', 'qamatsqatannarrowhebrew', 'afii57645', 'shevaquarterhebrew', 'dalethebrew', 'patahwidehebrew', 'dalethatafsegol', 'lamedholamdageshhebrew', 'afii57664', 'shevahebrew', 'afii57842', 'finalkafsheva', 'tsere1e', 'hiriqnarrowhebrew', 'sheva22', 'tethebrew', 'hatafqamats28', 'hatafqamats', 'segolnarrowhebrew', 'afii57804', 'gershayimhebrew', 'tav', 'nunhebrew', 'holamhebrew', 'afii57716', 'patahnarrowhebrew', 'he', 'rafehebrew', 'qofsegol', 'afii57687', 'hatafqamatsnarrowhebrew', 'qofqamatshebrew', 'dalet', 'qubutswidehebrew', 'vavhebrew', 'qofshevahebrew', 'gimelhebrew', 'dalethiriqhebrew', 'patah', 'sheqelhebrew', 'qofholam', 'ayinhebrew', 'segol13', 'reshhebrew', 'finalnun', 'newsheqelsign', 'hatafsegol', 'hatafsegol24', 'sofpasuqhebrew', 'qamats1c', 'dalethatafpatah', 'reshshevahebrew', 'sheva2e', 'reshhatafsegolhebrew', 'afii57839', 'afii57681', 'hatafqamatsquarterhebrew', 'afii57667', 'lamedhebrew', 'qofpatah', 'tserewidehebrew', 'finalnunhebrew', 'sheva', 'daletqubutshebrew', 'finaltsadihebrew', 'qamatsde', 'tsadihebrew', 'finalkafshevahebrew', 'hatafqamatswidehebrew', 'reshhatafpatah', 'afii57794', 'reshqubuts', 'samekh', 'sheqel', 'finalpe', 'shevawidehebrew', 'segol', 'reshhiriq',
+    'holamwidehebrew', 'qamatsquarterhebrew', 'lamedholamhebrew', 'afii57841', 'vavyodhebrew', 'hatafqamats1b', 'hatafsegolnarrowhebrew', 'afii57795', 'hatafpatahhebrew', 'qofhatafpatah', 'finalkafqamats', 'shinhebrew', 'afii57684', 'reshqamatshebrew', 'hatafqamatshebrew', 'afii57806', 'shevanarrowhebrew', 'sindothebrew', 'patah2a', 'segolhebrew', 'afii57798', 'qofhatafpatahhebrew', 'afii57800', 'qamatsqatanwidehebrew', 'hiriq14', 'qofqubuts', 'hatafpatah', 'hatafpatahnarrowhebrew', 'reshholamhebrew', 'afii57675', 'samekhhebrew', 'shin', 'tavhebrew', 'holam', 'finalkafhebrew', 'finalkafqamatshebrew', 'afii57679', 'tserequarterhebrew', 'holamnarrowhebrew', 'hatafsegolwidehebrew', 'qamatsnarrowhebrew', 'segolquarterhebrew', 'hatafpatahwidehebrew', 'tet', 'hiriq21', 'qamats27', 'afii57674', 'dalethatafpatahhebrew', 'bet', 'bethebrew', 'afii57685', 'yod', 'lamedholamdagesh', 'gereshhebrew', 'alef', 'daletqubuts', 'segol2c', 'qoftserehebrew', 'afii57677', 'finalkaf', 'daletqamatshebrew', 'ayin', 'hatafpatah16', 'paseqhebrew', 'qubuts25', 'tsere2b', 'afii57802', 'afii57669', 'dalethatafsegolhebrew', 'qofhatafsegolhebrew', 'daletqamats', 'qofholamhebrew', 'qamats10', 'afii57718', 'yodyodhebrew', 'afii57807', 'afii57799', 'qofhiriqhebrew', 'qofqubutshebrew', 'tsadi', 'qubutsnarrowhebrew', 'maqafhebrew', 'reshsegolhebrew', 'holam26', 'sheva15', 'lamedholam', 'vavvavhebrew', 'reshqubutshebrew', 'patah11', 'patah1d', 'kaf', 'daletshevahebrew', 'qamats1a', 'sheva115', 'dalettserehebrew', 'qofsheva', 'hethebrew', 'segol1f', 'hiriq2d',
     'afii57673', 'afii57797', 'dalettsere', 'qofhebrew', 'hiriqwidehebrew', 'reshhiriqhebrew', 'tserenarrowhebrew', 'patahhebrew', 'reshhatafsegol', 'daletholam', 'reshpatah', 'qubuts', 'afii57665', 'hatafpatah23', 'afii57658', 'gimel', 'daletsheva', 'hatafpatahquarterhebrew', 'alefhebrew', 'siluqlefthebrew', 'reshsegol', 'qofqamats', 'hatafsegol17', 'afii57676', 'afii57688', 'lamed', 'qof', 'reshpatahhebrew', 'afii57683', 'segolwidehebrew', 'finalmem', 'qofhatafsegol', 'dageshhebrew', 'afii57686', 'qamatshebrew', 'qamats33', 'qamats29', 'afii57682', 'daletsegolhebrew', 'reshtsere', 'holam32', 'afii57690', 'afii57666', 'dagesh', 'holam19', 'siluqhebrew', 'afii57796', 'resh', 'reshsheva', 'hatafpatah2f'},
 
-    "cp1256": {'afii57449', 'afii57440', 'afii57450', 'beharabic', 'afii57419', 'sadarabic', 'meemarabic', 'afii57508', 'afii57512', 'semicolonarabic', 'afii57423', 'dadarabic', 'taharabic', 'afii57442', 'afii57513', 'afii57448', 'gafarabic', 'ddalarabic', 'afii57446', 'afii57441', 'afii57430', 'lamarabic', 'afii57470', 'afii57421', 'dammalowarabic', 'alefmaksuraarabic', 'hamzadammaarabic', 
+    "cp1256": {'afii57449', 'afii57440', 'afii57450', 'beharabic', 'afii57419', 'sadarabic', 'meemarabic', 'afii57508', 'afii57512', 'semicolonarabic', 'afii57423', 'dadarabic', 'taharabic', 'afii57442', 'afii57513', 'afii57448', 'gafarabic', 'ddalarabic', 'afii57446', 'afii57441', 'afii57430', 'lamarabic', 'afii57470', 'afii57421', 'dammalowarabic', 'alefmaksuraarabic', 'hamzadammaarabic',
     'afii57426', 'noonarabic', 'dammatanarabic', 'zerowidthnonjoiner', 'tehmarbutaarabic', 'qafarabic', 'hamzaarabic', 'afii57454', 'hamzafathatanarabic', 'dalarabic', 'jeemarabic', 'afii57506', 'afii57458', 'afii57445', 'rehyehaleflamarabic', 'hamzalowkasraarabic', 'afii57519', 'afii57412', 'noonghunnaarabic', 'hamzasukunarabic', 'shaddafathatanarabic', 'zainarabic', 'afii57444', 'alefhamzabelowarabic', 'feharabic', 'fathaarabic', 'afii61664', 'afii57415', 'afii57403', 'kashidaautoarabic', 'afii57422', 'wawarabic', 'afii57409', 'sukunarabic', 'kafarabic', 'tcheharabic', 'afii57453', 'afii57433', 'yeharabic', 'jeharabic', 'hehaltonearabic', 'afii57411', 'alefmaddaabovearabic', 'afii57432', 'alefhamzaabovearabic', 'afii57511', 'afii57414', 'hamzadammatanarabic', 'shaddaarabic', 'khaharabic', 'rreharabic', 'kashidaautonosidebearingarabic', 'kasratanarabic', 'teharabic', 'peharabic', 'afii57429', 'afii57452', 'hamzalowkasratanarabic', 'haaltonearabic', 'heharabic', 'fathatanarabic', 'questionarabic', 'kasraarabic', 'afii57420', 'afii57418', 'tatweelarabic', 'fathalowarabic', 'afii57451', 'afii57507', 'afii57455', 'wawhamzaabovearabic', 'afii57416', 'dammatanaltonearabic', 'afii57424', 'afii57410', 'afii57388', 'thalarabic', 'afii57443', 'haharabic', 'commaarabic', 'afii57413', 'sheenarabic', 'ainarabic', 'afii57417', 'hamzafathaarabic', 'yehhamzaabovearabic', 'afii57456', 'afii57428', 'afii57425', 'alefarabic', 'zaharabic', 'tteharabic', 'hamzalowarabic', 'ghainarabic', 'afii57514', 'reharabic', 'yehbarreearabic', 'afii57509', 'afii301', 'dammaarabic', 'afii57427', 'afii57457', 'afii57431', 'afii57407', 'seenarabic', 'afii57434', 'theharabic'},
 
     "cp1257": {'ncommaaccent', 'rcedilla', 'lcedilla', 'emacron', 'ncedilla', 'iogonek', 'edotaccent', 'kcommaaccent', 'amacron', 'uogonek', 'gcommaaccent', 'kcedilla', 'rcommaaccent', 'umacron', 'gcedilla', 'omacron', 'edot', 'imacron', 'lcommaaccent'},
 
     "cp1258": {'tildecmb', 'gravecomb', 'dong', 'acutecmb', 'gravecmb', 'dotbelowcmb', 'uhorn', 'acutecomb', 'hookcmb', 'ohorn', 'hookabovecomb', 'tildecomb', 'dotbelowcomb'}
-}
+}
```

### Comparing `FontCollector-2.1.4/font_collector/parse_arguments.py` & `fontcollector-3.0.0rc1/font_collector/parse_arguments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import os
-from .font import Font
-from .font_loader import FontLoader
 from .mkvpropedit import Mkvpropedit
 from argparse import ArgumentParser
 from pathlib import Path
-from typing import List, Set, Tuple, Union
+from typing import Iterable, List, Tuple, Union
 
 
-def _parse_input_file(ass_input: List[Path]) -> List[Path]:
-
-    if len(ass_input) == 0:
-        return [Path(file) for file in os.listdir(os.getcwd()) if file.endswith(".ass")]
+def __parse_input_file(ass_input: List[Path]) -> List[Path]:
 
     ass_files_path = []
     for input in ass_input:
-        if os.path.isfile(input):
-            if input.name.endswith(".ass"):
-                ass_files_path.append(Path(input))
+        if input.is_file():
+            if input.suffix.casefold() == ".ass":
+                ass_files_path.append(input)
             else:
                 raise FileExistsError("Error: The input file is not an .ass file.")
-        elif os.path.isdir(input):
-            for file in os.listdir(input):
-                if file.endswith(".ass"):
-                    ass_files_path.append(Path(os.path.join(input, file)))
+        elif input.is_dir():
+            for file in input.iterdir():
+                if file.suffix.casefold() == ".ass":
+                    ass_files_path.append(file)
         else:
             raise FileNotFoundError(
                 f"Error: The input file/folder {input.name} does not exist."
             )
 
     return ass_files_path
 
 
 def parse_arguments() -> Tuple[
     List[Path],
     Path,
     Union[Path, None],
     bool,
-    Set[Path],
+    Iterable[Path],
+    Iterable[Path],
+    bool,
     bool,
     bool
 ]:
     """
     Returns:
         ass_files_path, output_directory, mkv_path, delete_fonts, additional_fonts, use_system_fonts
     """
@@ -50,15 +47,15 @@
     parser.add_argument(
         "--input",
         "-i",
         nargs="*",
         type=Path,
         required=True,
         help="""
-    Subtitles file. Must be an ASS file/directory. You can specify more than one .ass file/path. If no argument is specified, it will take all the font in the current path.
+    Subtitles file. Must be an ASS file/directory. You can specify more than one .ass file/path.
     """,
     )
     parser.add_argument(
         "-mkv",
         type=Path,
         help="""
     Video where the fonts will be merge. Must be a Matroska file.
@@ -86,18 +83,31 @@
         action="store_true",
         help="""
     If -d is specified, it will delete the font attached to the mkv before merging the new needed font. If -mkv is not specified, it will do nothing.
     """,
     )
     parser.add_argument(
         "--additional-fonts",
+        "-add-fonts",
         nargs="+",
+        default=set(),
         type=Path,
         help="""
     May be a directory containing font files or a single font file. You can specify more than one additional-fonts.
+    If it is a directory, it won't search recursively for fonts
+    """,
+    )
+    parser.add_argument(
+        "--additional-fonts-recursive",
+        "-add-fonts-rec",
+        nargs="+",
+        default=set(),
+        type=Path,
+        help="""
+    Path to font directory, which will be recursively searched for fonts.
     """,
     )
     parser.add_argument(
         "--exclude-system-fonts",
         action="store_false",
         help="""
     If specified, FontCollector won't use the system font to find the font used by an .ass file.
@@ -106,39 +116,48 @@
     parser.add_argument(
         "--collect-draw-fonts",
         action="store_true",
         help="""
     If specified, FontCollector will collect the font used by the draw. For more detail when this is usefull, see: https://github.com/libass/libass/issues/617
     """,
     )
+    parser.add_argument(
+        "--dont-convert-variable-to-collection",
+        action="store_false",
+        help="""
+    If specified, FontCollector won't convert variable font to a font collection. see: https://github.com/libass/libass/issues/386
+    """,
+    )
 
     args = parser.parse_args()
 
     # Parse args
-    ass_files_path = _parse_input_file(args.input)
+    ass_files_path = __parse_input_file(args.input)
 
-    output_directory = args.output
+    if len(ass_files_path) == 0:
+        raise RuntimeError("The specified file(s)/folder(s) doesn't exist or the folder(s) doesn't contains any .ass file.")
 
+    output_directory = args.output
     mkv_path = args.mkv
-    if mkv_path:
-        if args.mkvpropedit is not None:
-            Mkvpropedit.path = args.mkvpropedit
-
     delete_fonts = args.delete_fonts
-
-    if args.additional_fonts is not None:
-        additional_fonts = args.additional_fonts
-    else:
-        additional_fonts = set()
-
+    additional_fonts = args.additional_fonts
+    additional_fonts_recursive = args.additional_fonts_recursive
     use_system_fonts = args.exclude_system_fonts
     collect_draw_fonts = args.collect_draw_fonts
+    convert_variable_to_collection = args.dont_convert_variable_to_collection
+
+    if args.mkvpropedit:
+        if not mkv_path:
+            raise RuntimeError("-mkvpropedit requires --mkv option.")
+        Mkvpropedit.path = args.mkvpropedit
 
     return (
         ass_files_path,
         output_directory,
         mkv_path,
         delete_fonts,
         additional_fonts,
+        additional_fonts_recursive,
         use_system_fonts,
-        collect_draw_fonts
+        collect_draw_fonts,
+        convert_variable_to_collection
     )
```

