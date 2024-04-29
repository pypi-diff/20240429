# Comparing `tmp/anemoi-utils-0.1.3.tar.gz` & `tmp/anemoi_utils-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi-utils-0.1.3.tar", last modified: Fri Apr 19 08:36:07 2024, max compression
+gzip compressed data, was "anemoi_utils-0.1.6.tar", last modified: Mon Apr 29 14:02:27 2024, max compression
```

## Comparing `anemoi-utils-0.1.3.tar` & `anemoi_utils-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:07.721926 anemoi-utils-0.1.3/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/anemoi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/humanize.py
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/anemoi/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/anemoi_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:36:07.000000 anemoi-utils-0.1.3/anemoi_utils.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:36:07.725926 anemoi-utils-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-19 08:35:55.000000 anemoi-utils-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.863407 anemoi_utils-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.851407 anemoi_utils-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-04-29 14:02:27.863407 anemoi_utils-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.855407 anemoi_utils-0.1.6/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/checkpoints.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/dates.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/grib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/humanize.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/provenance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/modules/text.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:02:27.863407 anemoi_utils-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.851407 anemoi_utils-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.851407 anemoi_utils-0.1.6/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.859407 anemoi_utils-0.1.6/src/anemoi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi/utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/grib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8606 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/src/anemoi/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.859407 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15090 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 14:02:27.000000 anemoi_utils-0.1.6/src/anemoi_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:02:27.859407 anemoi_utils-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-29 14:02:15.000000 anemoi_utils-0.1.6/tests/test_utils.py
```

### Comparing `anemoi-utils-0.1.3/LICENSE` & `anemoi_utils-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi-utils-0.1.3/PKG-INFO` & `anemoi_utils-0.1.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: anemoi-utils
-Version: 0.1.3
-Summary: A package to hold various functions to support training of ML models on ECMWF data.
-Home-page: https://github.com/ecmwf/anemoi-utils
-Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
-Author-email: software.support@ecmwf.int
-License: Apache License Version 2.0
-Keywords: tool
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: text
-Provides-Extra: provenance
-Provides-Extra: dev
-Provides-Extra: all
-License-File: LICENSE
-
 # anemoi-utils
 
 **DISCLAIMER**
 This project is **BETA** and will be **Experimental** for the foreseeable future.
 Interfaces and functionality are likely to change, and the project itself may be scrapped.
 **DO NOT** use this software in any project/software that is operational.
```

### Comparing `anemoi-utils-0.1.3/anemoi/utils/checkpoints.py` & `anemoi_utils-0.1.6/src/anemoi/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `anemoi-utils-0.1.3/anemoi/utils/humanize.py` & `anemoi_utils-0.1.6/src/anemoi/utils/humanize.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 # This software is licensed under the terms of the Apache Licence Version 2.0
 # which can be obtained at http://www.apache.org/licenses/LICENSE-2.0.
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation
 # nor does it submit to any jurisdiction.
 #
 
-"""
-Generate human readable strings
-"""
+"""Generate human readable strings"""
 
 import datetime
 import re
 from collections import defaultdict
 
 
 def bytes(n: float) -> str:
@@ -84,15 +82,14 @@
 
 def seconds(seconds: float) -> str:
     """Convert a number of seconds to a human readable string
 
     >>> seconds(4000)
     '1 hour 6 minutes 40 seconds'
 
-
     Parameters
     ----------
     seconds : float
         The number of seconds
 
     Returns
     -------
@@ -143,28 +140,14 @@
 
 
 def number(value):
     return f"{value:,}"
 
 
 def plural(value, what):
-    """_summary_
-
-    Parameters
-    ----------
-    value : _type_
-        _description_
-    what : _type_
-        _description_
-
-    Returns
-    -------
-    _type_
-        _description_
-    """
     return f"{number(value)} {what}{_plural(value)}"
 
 
 DOW = [
     "Monday",
     "Tuesday",
     "Wednesday",
@@ -205,15 +188,14 @@
 
     return "th"
 
 
 def when(then, now=None, short=True):
     """Generate a human readable string for a date, relative to now
 
-
     >>> when(datetime.datetime.now() - datetime.timedelta(hours=2))
     '2 hours ago'
 
     >>> when(datetime.datetime.now() - datetime.timedelta(days=1))
     'yesterday at 08:46'
 
     >>> when(datetime.datetime.now() - datetime.timedelta(days=5))
@@ -350,26 +332,60 @@
                 d[i - 1, j - 1] + cost,
             )
 
     return d[m, n]
 
 
 def did_you_mean(word, vocabulary):
+    """Pick the closest word in a vocabulary
+
+    >>> did_you_mean("aple", ["banana", "lemon", "apple", "orange"])
+    'apple'
+
+    Parameters
+    ----------
+    word : str
+        The word to look for
+    vocabulary : list of strings
+        The list of known words
+
+    Returns
+    -------
+    str
+        The closest word in the vocabulary
+    """
     _, best = min((string_distance(word, w), w) for w in vocabulary)
     # if distance < min(len(word), len(best)):
     return best
 
 
 def dict_to_human(query):
     lst = [f"{k}={v}" for k, v in sorted(query.items())]
 
     return list_to_human(lst)
 
 
 def list_to_human(lst, conjunction="and"):
+    """Convert a list of strings to a human readable string
+
+    >>> list_to_human(["banana", "lemon", "apple", "orange"])
+    'banana, lemon, apple and orange'
+
+    Parameters
+    ----------
+    lst : list of str
+        The list of strings to concatenate
+    conjunction : str, optional
+        The word to connect the last word in the list (like "or" or "and"), by default "and"
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
     if not lst:
         return "??"
 
     if len(lst) > 2:
         lst = [", ".join(lst[:-1]), lst[-1]]
 
     return f" {conjunction} ".join(lst)
```

### Comparing `anemoi-utils-0.1.3/anemoi/utils/provenance.py` & `anemoi_utils-0.1.6/src/anemoi/utils/provenance.py`

 * *Files identical despite different names*

### Comparing `anemoi-utils-0.1.3/anemoi/utils/text.py` & `anemoi_utils-0.1.6/src/anemoi/utils/text.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,34 +11,38 @@
 
 import sys
 from collections import defaultdict
 
 # https://en.wikipedia.org/wiki/Box-drawing_character
 
 
-def dotted_line(n=84) -> str:
-    """_summary_
+def dotted_line(width=84) -> str:
+    """Return a dotted line using '┈'
+
+    >>> dotted_line(40)
+    ┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈┈
 
     Parameters
     ----------
-    n : int, optional
-        _description_, by default 84
+    width : int, optional
+        Number of characters, by default 84
 
     Returns
     -------
     str
-        _description_
+        The dotted line
     """
-    return "┈" * n
+
+    return "┈" * width
 
 
 def boxed(text, min_width=80, max_width=80) -> str:
     """Put a box around a text
 
-    >>> print(boxed("Hello,\\nWorld!", max_width=40))
+    >>> boxed("Hello,\\nWorld!", max_width=40)
     ┌──────────────────────────────────────────┐
     │ Hello,                                   │
     │ World!                                   │
     └──────────────────────────────────────────┘
 
     Parameters
     ----------
@@ -233,26 +237,44 @@
             "actor": self._actor.as_dict(),
             "kids": [k.to_json(depth + 1) for k in self._kids],
             "depth": depth,
         }
 
 
 def table(rows, header, align, margin=0):
-    """_summary_
+    """Format a table
+
+    >>> table([['Aa', 12, 5],
+               ['B', 120, 1],
+               ['C', 9, 123]],
+               ['C1', 'C2', 'C3'],
+               ['<', '>', '>']))
+        C1 │  C2 │  C3
+        ───┼─────┼────
+        Aa │  12 │   5
+        B  │ 120 │   1
+        C  │   9 │ 123
+        ───┴─────┴────
 
     Parameters
     ----------
-    rows : _type_
-        _description_
-    header : _type_
-        _description_
-    align : _type_
-        _description_
+    rows : list of lists (or tuples)
+        The rows of the table
+    header : A list or tuple of strings
+        The header of the table
+    align : A list of '<', '>', or '^'
+        To align the columns to the left, right, or center
     margin : int, optional
-        _description_, by default 0
+        Extra spaces on the left side of the table, by default 0
+
+
+    Returns
+    -------
+    str
+        A table as a string
     """
 
     def _(x):
         try:
             x = float(x)
         except Exception:
             pass
@@ -273,17 +295,23 @@
 
     all_rows = [header] + tmp
 
     lens = [max(len(x) for x in col) for col in zip(*all_rows)]
 
     result = []
     for i, row in enumerate(all_rows):
-        result.append(
-            " │ ".join([x.ljust(i) if align[j] == "<" else x.rjust(i) for j, (x, i) in enumerate(zip(row, lens))])
-        )
+
+        def _(x, i, j):
+            if align[j] == "<":
+                return x.ljust(i)
+            if align[j] == ">":
+                return x.rjust(i)
+            return x.center(i)
+
+        result.append(" │ ".join([_(x, i, j) for j, (x, i) in enumerate(zip(row, lens))]))
         if i == 0:
             result.append("─┼─".join(["─" * i for i in lens]))
 
     result.append("─┴─".join(["─" * i for i in lens]))
 
     if margin:
         result = [margin * " " + x for x in result]
```

