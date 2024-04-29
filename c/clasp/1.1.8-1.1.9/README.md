# Comparing `tmp/clasp-1.1.8.tar.gz` & `tmp/clasp-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clasp-1.1.8.tar", last modified: Tue Jun 21 11:09:27 2022, max compression
+gzip compressed data, was "clasp-1.1.9.tar", last modified: Mon Mar 20 15:24:39 2023, max compression
```

## Comparing `clasp-1.1.8.tar` & `clasp-1.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2022-06-21 11:09:27.321577 clasp-1.1.8/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     1490 2022-06-21 11:09:01.000000 clasp-1.1.8/HISTORY.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    14847 2019-03-05 16:30:33.000000 clasp-1.1.8/LICENSE
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      217 2019-03-05 16:30:33.000000 clasp-1.1.8/MANIFEST.in
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     5729 2022-06-21 11:09:27.321739 clasp-1.1.8/PKG-INFO
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     4998 2020-09-28 10:43:02.000000 clasp-1.1.8/README.rst
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2022-06-21 11:09:27.310417 clasp-1.1.8/clasp/
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)      327 2022-06-21 11:08:41.000000 clasp-1.1.8/clasp/__init__.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    12186 2021-09-02 13:25:08.000000 clasp-1.1.8/clasp/click_callbacks.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    21584 2022-06-21 11:06:04.000000 clasp-1.1.8/clasp/click_ext.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     1202 2020-09-28 10:43:02.000000 clasp-1.1.8/clasp/click_types.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)    20866 2020-10-10 08:55:41.000000 clasp-1.1.8/clasp/script_tools.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     4637 2020-10-10 07:46:02.000000 clasp-1.1.8/clasp/sphinx_click_ext.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     1119 2020-09-28 10:43:02.000000 clasp-1.1.8/clasp/templates.py
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2022-06-21 11:09:27.314702 clasp-1.1.8/clasp.egg-info/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     5729 2022-06-21 11:09:26.000000 clasp-1.1.8/clasp.egg-info/PKG-INFO
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      778 2022-06-21 11:09:27.000000 clasp-1.1.8/clasp.egg-info/SOURCES.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)        1 2022-06-21 11:09:26.000000 clasp-1.1.8/clasp.egg-info/dependency_links.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       56 2022-06-21 11:09:26.000000 clasp-1.1.8/clasp.egg-info/entry_points.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       55 2022-06-21 11:09:27.000000 clasp-1.1.8/clasp.egg-info/requires.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)        6 2022-06-21 11:09:27.000000 clasp-1.1.8/clasp.egg-info/top_level.txt
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)        1 2019-03-05 16:32:59.000000 clasp-1.1.8/clasp.egg-info/zip-safe
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2022-06-21 11:09:27.319748 clasp-1.1.8/docs/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      608 2019-03-05 16:30:33.000000 clasp-1.1.8/docs/Makefile
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2022-06-21 11:09:27.305700 clasp-1.1.8/docs/_build/
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2022-06-21 11:09:27.305785 clasp-1.1.8/docs/_build/html/
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2022-06-21 11:09:27.320727 clasp-1.1.8/docs/_build/html/_static/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      286 2022-03-25 14:00:20.000000 clasp-1.1.8/docs/_build/html/_static/file.png
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       90 2022-03-25 14:00:20.000000 clasp-1.1.8/docs/_build/html/_static/minus.png
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       90 2022-03-25 14:00:20.000000 clasp-1.1.8/docs/_build/html/_static/plus.png
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      130 2020-09-28 10:43:02.000000 clasp-1.1.8/docs/clasp.click_callbacks.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      112 2019-03-05 16:30:33.000000 clasp-1.1.8/docs/clasp.click_ext.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      121 2019-03-05 16:30:33.000000 clasp-1.1.8/docs/clasp.script_tools.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      135 2019-03-05 16:30:33.000000 clasp-1.1.8/docs/clasp.sphinx_click_ext.rst
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     5955 2020-09-28 10:43:02.000000 clasp-1.1.8/docs/conf.py
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       12 2019-03-05 16:30:33.000000 clasp-1.1.8/docs/genindex.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      137 2019-08-23 23:03:34.000000 clasp-1.1.8/docs/history.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      324 2020-09-28 10:43:02.000000 clasp-1.1.8/docs/index.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      769 2019-03-05 16:30:33.000000 clasp-1.1.8/docs/make.bat
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       14 2019-03-05 16:30:33.000000 clasp-1.1.8/docs/search.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)       25 2019-03-05 16:30:33.000000 clasp-1.1.8/docs/todo.rst
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)      432 2022-06-21 11:09:27.322374 clasp-1.1.8/setup.cfg
--rwxr-xr-x   0 stephenwasilewski   (501) staff       (20)     2081 2022-06-21 11:08:41.000000 clasp-1.1.8/setup.py
-drwxr-xr-x   0 stephenwasilewski   (501) staff       (20)        0 2022-06-21 11:09:27.321036 clasp-1.1.8/tests/
--rw-r--r--   0 stephenwasilewski   (501) staff       (20)     1999 2022-06-20 11:25:22.000000 clasp-1.1.8/tests/test_script_tools.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-03-20 15:24:39.764062 clasp-1.1.9/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     1571 2023-03-20 15:11:34.000000 clasp-1.1.9/HISTORY.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    14847 2023-03-01 14:08:57.000000 clasp-1.1.9/LICENSE
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      217 2023-03-01 14:08:57.000000 clasp-1.1.9/MANIFEST.in
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     5708 2023-03-20 15:24:39.764125 clasp-1.1.9/PKG-INFO
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     4997 2023-03-01 14:08:57.000000 clasp-1.1.9/README.rst
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-03-20 15:24:39.760634 clasp-1.1.9/clasp/
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)      328 2023-03-20 15:10:53.000000 clasp-1.1.9/clasp/__init__.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    12186 2023-03-01 14:08:57.000000 clasp-1.1.9/clasp/click_callbacks.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    20383 2023-03-19 11:44:59.000000 clasp-1.1.9/clasp/click_ext.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     1202 2023-03-01 14:08:57.000000 clasp-1.1.9/clasp/click_types.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)    20868 2023-03-20 15:15:24.000000 clasp-1.1.9/clasp/script_tools.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     4637 2023-03-01 14:08:57.000000 clasp-1.1.9/clasp/sphinx_click_ext.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     1119 2023-03-01 14:08:57.000000 clasp-1.1.9/clasp/templates.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-03-20 15:24:39.761611 clasp-1.1.9/clasp.egg-info/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     5708 2023-03-20 15:24:39.000000 clasp-1.1.9/clasp.egg-info/PKG-INFO
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      778 2023-03-20 15:24:39.000000 clasp-1.1.9/clasp.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)        1 2023-03-20 15:24:39.000000 clasp-1.1.9/clasp.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       56 2023-03-20 15:24:39.000000 clasp-1.1.9/clasp.egg-info/entry_points.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       55 2023-03-20 15:24:39.000000 clasp-1.1.9/clasp.egg-info/requires.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)        6 2023-03-20 15:24:39.000000 clasp-1.1.9/clasp.egg-info/top_level.txt
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)        1 2023-03-01 14:09:19.000000 clasp-1.1.9/clasp.egg-info/zip-safe
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-03-20 15:24:39.763341 clasp-1.1.9/docs/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      608 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/Makefile
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-03-20 15:24:39.758336 clasp-1.1.9/docs/_build/
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-03-20 15:24:39.758382 clasp-1.1.9/docs/_build/html/
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-03-20 15:24:39.763693 clasp-1.1.9/docs/_build/html/_static/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      286 2023-02-28 08:12:06.000000 clasp-1.1.9/docs/_build/html/_static/file.png
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       90 2023-02-28 08:12:06.000000 clasp-1.1.9/docs/_build/html/_static/minus.png
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       90 2023-02-28 08:12:06.000000 clasp-1.1.9/docs/_build/html/_static/plus.png
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      130 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/clasp.click_callbacks.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      112 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/clasp.click_ext.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      121 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/clasp.script_tools.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      135 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/clasp.sphinx_click_ext.rst
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     5955 2023-03-20 15:13:52.000000 clasp-1.1.9/docs/conf.py
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       12 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/genindex.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      137 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/history.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      340 2023-03-20 15:13:17.000000 clasp-1.1.9/docs/index.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      769 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/make.bat
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       14 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/search.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)       25 2023-03-01 14:08:57.000000 clasp-1.1.9/docs/todo.rst
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)      432 2023-03-20 15:24:39.764386 clasp-1.1.9/setup.cfg
+-rwxr-xr-x   0 stephenwasilewski   (503) staff       (20)     2081 2023-03-20 15:10:53.000000 clasp-1.1.9/setup.py
+drwxr-xr-x   0 stephenwasilewski   (503) staff       (20)        0 2023-03-20 15:24:39.763801 clasp-1.1.9/tests/
+-rw-r--r--   0 stephenwasilewski   (503) staff       (20)     1999 2023-03-01 14:08:57.000000 clasp-1.1.9/tests/test_script_tools.py
```

### Comparing `clasp-1.1.8/HISTORY.rst` & `clasp-1.1.9/HISTORY.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 
 =======
 History
 =======
 
+1.1.9
+-----
+added context to print_except to clean temporary files unless debug
+
 1.1.8
 -----
 added extendedinterpolation to config parser ${section:variable}
 
 1.1.7
 -----
 bugfix in invoke_dependency
```

### Comparing `clasp-1.1.8/LICENSE` & `clasp-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clasp-1.1.8/PKG-INFO` & `clasp-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: clasp
-Version: 1.1.8
+Version: 1.1.9
 Summary: clasp is  tools for command line and subprocess script development
 Home-page: https://bitbucket.org/stephenwasilewski/clasp
 Author: Stephen Wasilewski
 Author-email: stephanwaz@gmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: documentation, https://clasp.readthedocs.io/
 Keywords: clasp
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -79,15 +78,15 @@
             except click.Abort:
                 raise
             except Exception as ex:
                 clk.print_except(ex, kwargs['debug'])
         return 'XXX', kwargs, ctx
     
     
-    @main.resultcallback()
+    @main.result_callback
     @click.pass_context
     def printconfig(ctx, opts, **kwargs):
         """callback to save config file"""
         try:
             clk.tmp_clean(opts[2])
         except Exception:
             pass
@@ -179,9 +178,7 @@
 -------
 
 | Copyright (c) 2018 Stephen Wasilewski
 | This Source Code Form is subject to the terms of the Mozilla Public
 | License, v. 2.0. If a copy of the MPL was not distributed with this
 | file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-
-
```

### Comparing `clasp-1.1.8/README.rst` & `clasp-1.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             except click.Abort:
                 raise
             except Exception as ex:
                 clk.print_except(ex, kwargs['debug'])
         return 'XXX', kwargs, ctx
     
     
-    @main.resultcallback()
+    @main.result_callback
     @click.pass_context
     def printconfig(ctx, opts, **kwargs):
         """callback to save config file"""
         try:
             clk.tmp_clean(opts[2])
         except Exception:
             pass
```

### Comparing `clasp-1.1.8/clasp/click_callbacks.py` & `clasp-1.1.9/clasp/click_callbacks.py`

 * *Files identical despite different names*

### Comparing `clasp-1.1.8/clasp/click_ext.py` & `clasp-1.1.9/clasp/click_ext.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,24 @@
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 # =======================================================================
 
 """extension and interface for parsing with click and configparse
 
 imports callbacks into namespace for convenience
 """
-import types
 from builtins import str
 import configparser
 from configparser import ExtendedInterpolation
 import collections
 import traceback
 import functools
 import shutil
 
 import sphinx.builders.text
 import sphinx.writers.text
-from docutils.parsers.rst import Parser as RSTParser
-import docutils.utils
-from docutils.frontend import OptionParser
 
 import clasp.click_callbacks
 from clasp.click_callbacks import *
 
 callback_help = clasp.click_callbacks.__doc__
 
 
@@ -114,15 +110,15 @@
 @main.command()
 @click.argument('arg1')
 @clk.shared_decs(clk.command_decs('0.1', wrap=True))
 def XXX(ctx, arg1, **kwargs):
     pass
 
 
-@main.resultcallback()
+@main.result_callback
 @click.pass_context
 def printconfig(ctx, opts, **kwargs):
     """callback to save config file"""
     try:
         clk.tmp_clean(opts[2])
     except Exception:
         pass
@@ -135,68 +131,30 @@
     main()'''
 
 
 def click_ext(click):
     """customize click help messages and bash complete"""
     orig_init = click.core.Option.__init__
 
-    parser = RSTParser()
-    cmpt = (RSTParser,)
-    settings = OptionParser(components=cmpt).get_default_values()
-    settings.tab_size = 4
-    document = docutils.utils.new_document('<rst-doc>', settings)
-
-    app = types.SimpleNamespace(
-            srcdir=None,
-            confdir=None,
-            outdir=None,
-            doctreedir="/",
-            events=None,
-            warn=None,
-            config=types.SimpleNamespace(
-                    text_newlines="native",
-                    text_sectionchars="=",
-                    text_add_secnumbers=False,
-                    text_secnumber_suffix=".",
-                    ),
-            tags=set(),
-            registry=types.SimpleNamespace(
-                    create_translator=lambda s, something,
-                    new_builder: sphinx.writers.text.TextTranslator(
-                            document, new_builder
-                            )
-                    ),
-            )
-    builder = sphinx.builders.text.TextBuilder(app)
-
     def new_init(self, *args, **kwargs):
         orig_init(self, *args, **kwargs)
         if 'show_default' not in kwargs:
             self.show_default = True
 
     def format_help_text(self, ctx, formatter):
         """modified help text formatter for compatibility with sphinx-click."""
         if self.help:
             formatter.write_paragraph()
-            rst = _process_as_rst(self.help)
+            rst = self.help
             formatter.indent()
             for line in rst.splitlines():
                 formatter.write_text(line)
             formatter.dedent()
             formatter.write_paragraph()
 
-    def _process_as_rst(text):
-        parser.parse(text.replace("*", "\\*"), document)
-        translator = sphinx.writers.text.TextTranslator(document,
-                                                        builder)
-        document.walkabout(translator)
-        rst = translator.body.replace("\n\n", "\n")
-        document.clear()
-        return rst
-
     def format_options(self, ctx, formatter):
         """Writes all the options into the formatter if they exist."""
         opts = []
         twidth = max(shutil.get_terminal_size((80, 20)).columns, 80)
         sphinx.writers.text.MAXWIDTH = twidth - 10
         for param in self.get_params(ctx):
             rv = param.get_help_record(ctx)
@@ -218,24 +176,25 @@
         seps = [(i[0], (f"\n{i[1]}" , '')) for i in index_seps(opts)]
         opts = [i[-1] for i in sorted(opts + seps, key=lambda x: (x[0], x[1]))]
         if opts:
             with formatter.section('Options'):
                 indent = ' '*formatter.current_indent
                 for opt in opts:
                     formatter.write(f"{indent}{opt[0]}\n")
-                    rst = _process_as_rst(opt[1])
+                    rst = opt[1]
                     formatter.indent()
                     formatter.indent()
                     formatter.width = (sphinx.writers.text.MAXWIDTH +
                                        formatter.current_indent*2)
                     for line in rst.splitlines():
                         formatter.write_text(line)
                     formatter.dedent()
                     formatter.dedent()
                     formatter.write("\n")
+
     click.core.Option.__init__ = new_init
     click.core.Command.format_help_text = format_help_text
     click.core.Command.format_options = format_options
 
     return click
 
 
@@ -270,18 +229,18 @@
             else:
                 try:
                     func(ctx, *args, **kwargs)
                 except click.Abort:
                     raise
                 except click.exceptions.Exit as ex:
                     if ex.exit_code != 0:
-                        print_except(ex, kwargs['debug'])
+                        print_except(ex, kwargs['debug'], ctx=ctx)
                         raise click.Abort
                 except Exception as ex:
-                    print_except(ex, kwargs['debug'])
+                    print_except(ex, kwargs['debug'], ctx=ctx)
                     raise click.Abort
             return cname, kwargs, ctx
         return handle_call
     return wrapped_call
 
 
 def main_decs(v, writeconfig=True):
@@ -357,19 +316,22 @@
         return f
     return decorate
 
 
 def tmp_clean(ctx):
     """remove files placed int temps context object
     (called at end of scripts)"""
-    for i in ctx.obj['temps']:
-        try:
-            os.remove(i)
-        except Exception:
-            pass
+    try:
+        for i in ctx.obj['temps']:
+            try:
+                os.remove(i)
+            except Exception:
+                pass
+    except (KeyError, TypeError):
+        pass
 
 
 def invoke_dependency(ctx, cmd, *args, **kwargs):
     kws = ctx.parent.command.commands[cmd.name].context_settings['default_map']
     for p in ctx.parent.command.commands[cmd.name].params:
         try:
             kws[p.name] = p.process_value(ctx.parent, kws[p.name])
@@ -378,26 +340,30 @@
     kws.update(**kwargs)
     cmd.callback(*args, **kws)
 
 
 def read_section(Config, dict1, section, options):
     for option in options:
         try:
-            opt = Config.get(section, option)
+            try:
+                opt = Config.get(section, option)
+            except configparser.InterpolationSyntaxError:
+                opt = Config.get(section, option, raw=True)
             if re.match(r'.+_\d+', option):
                 opto = option.rsplit("_", 1)[0]
                 try:
                     dict1[opto].append(opt)
                 except Exception:
                     dict1[opto] = [opt]
             elif opt == "None":
                 dict1[option] = None
             else:
                 dict1[option] = opt
         except Exception as ex:
+            print(ex.__class__)
             click.echo("exception on {}! {}".format(option, ex), err=True)
             dict1[option] = None
     return dict1
 
 
 def ConfigSectionMap(Config, section):
     """maps ConfigParser section to dict"""
@@ -616,18 +582,20 @@
     else:
         f = open(outconfig, 'w')
         f.write(comments)
         Parser.write(f)
         f.close()
 
 
-def print_except(ex, debug=False):
+def print_except(ex, debug=False, ctx=None):
     """general human readable exception message"""
     if debug:
         traceback.print_exc()
+    elif ctx is not None:
+        tmp_clean(ctx)
     click.echo("\n**************\n**************", err=True)
     click.echo("Execution failed:", err=True)
     click.echo("{}: {}".format(type(ex).__name__, ex), err=True)
     click.echo("**************\n**************\n", err=True)
 
 
 def formatarg_line(v, i=None, idx=None):
```

### Comparing `clasp-1.1.8/clasp/click_types.py` & `clasp-1.1.9/clasp/click_types.py`

 * *Files identical despite different names*

### Comparing `clasp-1.1.8/clasp/script_tools.py` & `clasp-1.1.9/clasp/script_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # =======================================================================
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 # =======================================================================
 
 """library of functions helpful for cli script development and parallel
-computing particulary w/ subprocess calls."""
+computing particulary with subprocess calls."""
 import sys
 import shlex
 import subprocess
 import inspect
 import tempfile
 from glob import glob
 import os
```

### Comparing `clasp-1.1.8/clasp/sphinx_click_ext.py` & `clasp-1.1.9/clasp/sphinx_click_ext.py`

 * *Files identical despite different names*

### Comparing `clasp-1.1.8/clasp/templates.py` & `clasp-1.1.9/clasp/templates.py`

 * *Files identical despite different names*

### Comparing `clasp-1.1.8/clasp.egg-info/PKG-INFO` & `clasp-1.1.9/clasp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: clasp
-Version: 1.1.8
+Version: 1.1.9
 Summary: clasp is  tools for command line and subprocess script development
 Home-page: https://bitbucket.org/stephenwasilewski/clasp
 Author: Stephen Wasilewski
 Author-email: stephanwaz@gmail.com
 License: Mozilla Public License 2.0 (MPL 2.0)
 Project-URL: documentation, https://clasp.readthedocs.io/
 Keywords: clasp
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
@@ -79,15 +78,15 @@
             except click.Abort:
                 raise
             except Exception as ex:
                 clk.print_except(ex, kwargs['debug'])
         return 'XXX', kwargs, ctx
     
     
-    @main.resultcallback()
+    @main.result_callback
     @click.pass_context
     def printconfig(ctx, opts, **kwargs):
         """callback to save config file"""
         try:
             clk.tmp_clean(opts[2])
         except Exception:
             pass
@@ -179,9 +178,7 @@
 -------
 
 | Copyright (c) 2018 Stephen Wasilewski
 | This Source Code Form is subject to the terms of the Mozilla Public
 | License, v. 2.0. If a copy of the MPL was not distributed with this
 | file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-
-
```

### Comparing `clasp-1.1.8/clasp.egg-info/SOURCES.txt` & `clasp-1.1.9/clasp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clasp-1.1.8/docs/Makefile` & `clasp-1.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clasp-1.1.8/docs/conf.py` & `clasp-1.1.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 author = u"Stephen Wasilewski"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `clasp-1.1.8/docs/make.bat` & `clasp-1.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clasp-1.1.8/setup.py` & `clasp-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,10 +56,10 @@
     data_files=data_files,
     package_data=package_data,
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://bitbucket.org/stephenwasilewski/clasp',
     project_urls= {'documentation': 'https://clasp.readthedocs.io/'},
-    version='1.1.8',
+    version='1.1.9',
     zip_safe=True,
 )
```

### Comparing `clasp-1.1.8/tests/test_script_tools.py` & `clasp-1.1.9/tests/test_script_tools.py`

 * *Files identical despite different names*

