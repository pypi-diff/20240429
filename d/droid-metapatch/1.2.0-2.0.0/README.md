# Comparing `tmp/droid_metapatch-1.2.0.tar.gz` & `tmp/droid_metapatch-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "droid_metapatch-1.2.0.tar", max compression
+gzip compressed data, was "droid_metapatch-2.0.0.tar", max compression
```

## Comparing `droid_metapatch-1.2.0.tar` & `droid_metapatch-2.0.0.tar`

### file list

```diff
@@ -1,9 +1,29 @@
--rw-r--r--   0        0        0    12277 2024-04-08 09:00:49.052750 droid_metapatch-1.2.0/README.md
--rw-r--r--   0        0        0      155 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/__init__.py
--rw-r--r--   0        0        0     2533 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/base.py
--rwxr-xr-x   0        0        0     9650 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/cli_util.py
--rw-r--r--   0        0        0    11837 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/metapatch.py
--rw-r--r--   0        0        0     6928 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/options.py
--rw-r--r--   0        0        0      697 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/metapatch/utils.py
--rw-r--r--   0        0        0      493 2024-04-08 09:00:49.056750 droid_metapatch-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    12888 1970-01-01 00:00:00.000000 droid_metapatch-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/LICENSE
+-rw-r--r--   0        0        0    22794 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/README.md
+-rw-r--r--   0        0        0      366 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/__init__.py
+-rw-r--r--   0        0        0     2533 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/base.py
+-rw-r--r--   0        0        0     2029 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/circuits/README.md
+-rw-r--r--   0        0        0     2547 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/circuits/__init__.py
+-rw-r--r--   0        0        0     6255 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/circuits/base.py
+-rw-r--r--   0        0        0    15356 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/circuits/clock.py
+-rw-r--r--   0        0        0    53179 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/circuits/cv.py
+-rw-r--r--   0        0        0     9625 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/circuits/deprecated.py
+-rw-r--r--   0        0        0    23303 2024-04-29 12:50:45.155803 droid_metapatch-2.0.0/metapatch/circuits/logic.py
+-rw-r--r--   0        0        0   178579 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/circuits/midi.py
+-rw-r--r--   0        0        0    22942 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/circuits/modulation.py
+-rw-r--r--   0        0        0    19455 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/circuits/other.py
+-rw-r--r--   0        0        0    37744 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/circuits/pitch.py
+-rw-r--r--   0        0        0   149008 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/circuits/sequencing.py
+-rw-r--r--   0        0        0   145502 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/circuits/ui.py
+-rwxr-xr-x   0        0        0     3473 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/cli_util.py
+-rw-r--r--   0        0        0      149 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/factory/__init__.py
+-rw-r--r--   0        0        0     6591 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/factory/boilerplate.py
+-rw-r--r--   0        0        0     3380 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/factory/context.py
+-rw-r--r--   0        0        0     4281 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/factory/formatting.py
+-rw-r--r--   0        0        0     7437 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/factory/patch_factory.py
+-rw-r--r--   0        0        0     4565 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/factory/patch_parser.py
+-rw-r--r--   0        0        0    19131 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/metapatch.py
+-rw-r--r--   0        0        0     7849 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/options.py
+-rw-r--r--   0        0        0      697 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/metapatch/utils.py
+-rw-r--r--   0        0        0      706 2024-04-29 12:50:45.159803 droid_metapatch-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    23405 1970-01-01 00:00:00.000000 droid_metapatch-2.0.0/PKG-INFO
```

### Comparing `droid_metapatch-1.2.0/metapatch/base.py` & `droid_metapatch-2.0.0/metapatch/base.py`

 * *Files identical despite different names*

### Comparing `droid_metapatch-1.2.0/metapatch/options.py` & `droid_metapatch-2.0.0/metapatch/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,26 +167,52 @@
     Args:
         description: Description of the variable
         section: The name of the configuration pane where this option should be shown.
 
     A number of different option types can be generated. Without any further
     options, the option will be a boolean true/false.
 
-    Number Option:
-        minimum: integer
-        maximum: integer
-
-    Enumeration Option:
-        choices: List of tuples. The Tuples define (value, description)
-
-    Default:
-        You can specify a default, otherwise it will be derived as follows:
-        Bool: True
-        Number: Lowest number
-        Enum: First value.
+    ### Boolean Option
+
+    Example:
+    ```python
+    enable_arpeggiator: bool = metapatch.option("Enable arpeggiator")
+    ```
+
+    ### Number Option
+    - minimum: integer
+    - maximum: integer
+
+    Example:
+    ```python
+    midi_channel: int = metaclass.option("MIDI channel", minimum=1, maximum=16)
+    ```
+
+    ### Enumeration Option
+    - choices: List of tuples. The Tuples define (value, description)
+
+    Example:
+    ```python
+    clock_source: str = metapatch.option(
+        "Clock Source",
+        choices=[("internal", "Internal clock"), ("external", "External clock")]
+    )
+    ```
+
+
+    ### Defaults
+    You can specify a default for any option, otherwise it will be derived as follows:
+    - Bool: True
+    - Number: Lowest number
+    - Enum: First value.
+
+    Example:
+    ```python
+    enable_arpeggiator: bool = metapatch.option("Enable arpeggiator", default=True)
+    ```
 
     """
     params: Dict[str, Any] = {
         "title": description,
         "section": section,
     }
     bases: Tuple[type, ...]
@@ -229,9 +255,18 @@
 
 def preset(title: str, parameters: Dict[str, Any]) -> Preset:
     """Define a preset.
 
     Args:
         title: The name of the preset.
         parameter: A dictionary containing parameter to value mappings.
+
+    This helper function allows you to define presets for your patch generators.
+    Presets are essentially just predefined values for your options defined as a python
+    dictionary.
+
+    See `metapatch.option` for how to define options.
+
+    Example:
+        simple = metapatch.preset("The simplest version", {"voices": 1, "clock_source": "internal"})
     """
     return Preset(title, parameters)
```

### Comparing `droid_metapatch-1.2.0/metapatch/utils.py` & `droid_metapatch-2.0.0/metapatch/utils.py`

 * *Files identical despite different names*

