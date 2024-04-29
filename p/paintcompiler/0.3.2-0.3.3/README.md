# Comparing `tmp/paintcompiler-0.3.2.tar.gz` & `tmp/paintcompiler-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paintcompiler-0.3.2.tar", last modified: Tue Oct 31 08:38:04 2023, max compression
+gzip compressed data, was "paintcompiler-0.3.3.tar", last modified: Mon Apr 29 08:54:07 2024, max compression
```

## Comparing `paintcompiler-0.3.2.tar` & `paintcompiler-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-10-31 08:38:04.116967 paintcompiler-0.3.2/
--rw-r--r--   0 simon      (501) staff       (20)      584 2023-05-19 12:22:19.000000 paintcompiler-0.3.2/LICENSE
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-10-31 08:38:04.111420 paintcompiler-0.3.2/Lib/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-10-31 08:38:04.112131 paintcompiler-0.3.2/Lib/paintcompiler/
--rw-r--r--   0 simon      (501) staff       (20)    24820 2023-10-31 08:36:03.000000 paintcompiler-0.3.2/Lib/paintcompiler/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-10-31 08:38:04.114518 paintcompiler-0.3.2/Lib/paintcompiler.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)    14596 2023-10-31 08:38:04.000000 paintcompiler-0.3.2/Lib/paintcompiler.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      404 2023-10-31 08:38:04.000000 paintcompiler-0.3.2/Lib/paintcompiler.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-10-31 08:38:04.000000 paintcompiler-0.3.2/Lib/paintcompiler.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       92 2023-10-31 08:38:04.000000 paintcompiler-0.3.2/Lib/paintcompiler.egg-info/entry_points.txt
--rw-r--r--   0 simon      (501) staff       (20)       18 2023-10-31 08:38:04.000000 paintcompiler-0.3.2/Lib/paintcompiler.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)       30 2023-10-31 08:38:04.000000 paintcompiler-0.3.2/Lib/paintcompiler.egg-info/top_level.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-10-31 08:38:04.114702 paintcompiler-0.3.2/Lib/paintdecompiler/
--rw-r--r--   0 simon      (501) staff       (20)    12346 2023-09-18 13:27:40.000000 paintcompiler-0.3.2/Lib/paintdecompiler/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    14596 2023-10-31 08:38:04.116581 paintcompiler-0.3.2/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)    13628 2023-09-18 13:28:34.000000 paintcompiler-0.3.2/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-10-31 08:38:04.115982 paintcompiler-0.3.2/example/
--rw-r--r--   0 simon      (501) staff       (20)     6428 2023-05-22 13:33:48.000000 paintcompiler-0.3.2/example/COLRv1-Test.glyphs
--rw-r--r--   0 simon      (501) staff       (20)     1068 2023-05-22 13:34:22.000000 paintcompiler-0.3.2/example/build.sh
--rw-r--r--   0 simon      (501) staff       (20)     5641 2023-09-18 13:02:38.000000 paintcompiler-0.3.2/example/paints.py
--rw-r--r--   0 simon      (501) staff       (20)      418 2023-10-31 08:36:56.000000 paintcompiler-0.3.2/pyproject.toml
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-10-31 08:38:04.117021 paintcompiler-0.3.2/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-29 08:54:07.156537 paintcompiler-0.3.3/
+-rw-r--r--   0 simon      (501) staff       (20)      584 2023-05-19 12:22:19.000000 paintcompiler-0.3.3/LICENSE
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-29 08:54:07.153082 paintcompiler-0.3.3/Lib/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-29 08:54:07.153619 paintcompiler-0.3.3/Lib/paintcompiler/
+-rw-r--r--   0 simon      (501) staff       (20)    28146 2024-04-29 08:51:56.000000 paintcompiler-0.3.3/Lib/paintcompiler/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-29 08:54:07.156085 paintcompiler-0.3.3/Lib/paintcompiler.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)    16711 2024-04-29 08:54:07.000000 paintcompiler-0.3.3/Lib/paintcompiler.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      404 2024-04-29 08:54:07.000000 paintcompiler-0.3.3/Lib/paintcompiler.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2024-04-29 08:54:07.000000 paintcompiler-0.3.3/Lib/paintcompiler.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       92 2024-04-29 08:54:07.000000 paintcompiler-0.3.3/Lib/paintcompiler.egg-info/entry_points.txt
+-rw-r--r--   0 simon      (501) staff       (20)       18 2024-04-29 08:54:07.000000 paintcompiler-0.3.3/Lib/paintcompiler.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)       30 2024-04-29 08:54:07.000000 paintcompiler-0.3.3/Lib/paintcompiler.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-29 08:54:07.155002 paintcompiler-0.3.3/Lib/paintdecompiler/
+-rw-r--r--   0 simon      (501) staff       (20)    12346 2023-09-18 13:27:40.000000 paintcompiler-0.3.3/Lib/paintdecompiler/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    16711 2024-04-29 08:54:07.156296 paintcompiler-0.3.3/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)    15743 2024-04-29 08:28:19.000000 paintcompiler-0.3.3/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2024-04-29 08:54:07.155814 paintcompiler-0.3.3/example/
+-rw-r--r--   0 simon      (501) staff       (20)     6428 2023-05-22 13:33:48.000000 paintcompiler-0.3.3/example/COLRv1-Test.glyphs
+-rw-r--r--   0 simon      (501) staff       (20)     1068 2023-05-22 13:34:22.000000 paintcompiler-0.3.3/example/build.sh
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2024-04-29 08:52:14.000000 paintcompiler-0.3.3/example/paints.py
+-rw-r--r--   0 simon      (501) staff       (20)      418 2024-04-29 08:53:41.000000 paintcompiler-0.3.3/pyproject.toml
+-rw-r--r--   0 simon      (501) staff       (20)       38 2024-04-29 08:54:07.156578 paintcompiler-0.3.3/setup.cfg
```

### Comparing `paintcompiler-0.3.2/LICENSE` & `paintcompiler-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paintcompiler-0.3.2/Lib/paintcompiler/__init__.py` & `paintcompiler-0.3.3/Lib/paintcompiler/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,44 +5,59 @@
 from fontTools.varLib.varStore import OnlineVarStoreBuilder
 from fontTools.varLib.builder import buildDeltaSetIndexMap
 from fontTools.feaLib.variableScalar import VariableScalar
 from fontTools.varLib.instancer import _TupleVarStoreAdapter
 from fontTools.misc.fixedTools import floatToFixed, fixedToFloat
 from fontTools.ttLib.tables._f_v_a_r import Axis
 from typing import List
+import re
 
 
 def compile_color(c):
     try:
         assert c[0] == "#"
         return tuple(int(x, 16) / 255 for x in [c[1:3], c[3:5], c[5:7], c[7:9]])
     except:
         raise ValueError(
             f"Could not understand color {c}; should be hex digits in form #RRGGBBAA"
         )
 
 
-def compile_colors(colors):
+def compile_palette_entry(colors):
     return [compile_color(c) for c in colors]
 
 
+def compile_palettes(entries):
+    # each element of the array should be the same length;
+    # if it is one, pad to the max length, if not raise an error
+    max_length = max(len(entry) for entry in entries)
+    for index, entry in enumerate(entries):
+        if len(entry) == 1:
+            entries[index] = entry * max_length
+        elif len(entry) != max_length:
+            raise ValueError(
+                f"Pallete index {index} specifies {len(entry)} palettes ({entry}), but should have {max_length}"
+            )
+    return [compile_palette_entry(colors) for colors in entries]
+
+
 class ColorLine:
     def __init__(self, start_or_stops, end=None, extend="pad"):
         if end is None:
             stops = start_or_stops
         else:
             stops = {0.0: start_or_stops, 1.0: end}
         self.colorstops = []
         self.needs_variable = False
         self.extend = extend
         if isinstance(stops, dict):
             stops = list(stops.items())
         for k, v in stops:
             alpha = 1.0
-            if isinstance(v, (list, tuple)):
+            if isinstance(v, (list, tuple)) and isinstance(v[1], (float, int, dict)):
                 alpha = v[1]
                 v = v[0]
             if isinstance(alpha, (dict, str)):
                 self.needs_variable = True
             if isinstance(k, (dict, str)):
                 self.needs_variable = True
             self.colorstops.append((k, v, alpha))
@@ -102,15 +117,17 @@
         raise ValueError(f"Unknown units {units}")
     return default
 
 
 class PythonBuilder:
     def __init__(self, font: TTFont) -> None:
         self.font = font
+        self.explicit_palette = False
         self.palette = []
+        self.palette_flags = {}
         self.variations = []
         self.varindexbases = []
         self.deltaset: list[int] = []
         self.axes = []
         self.varstorebuilder = None
         if "fvar" in font:
             self.axes = font["fvar"].axes
@@ -140,15 +157,21 @@
             return v
 
         first_value = None
         values_dict = {}
 
         if isinstance(s, str):
             for values in s.split():
-                locations, value = values.split(":")
+                try:
+                    locations, value = values.split(":")
+                except ValueError:
+                    raise ValueError(
+                        f"Could not understand variable parameter {s}, "
+                        "should be of the form tag=value,tag=value:default"
+                    )
                 location = {}
                 for loc in locations.split(","):
                     axis, axis_loc = loc.split("=")
                     location[axis] = float(axis_loc)
                 values_dict[tuple(location.items())] = value
 
             logging.warning(f"Consider using dict {values_dict} instead of string {s}")
@@ -172,14 +195,25 @@
                 raise ValueError(f"No default value OR first value in '{s}'")
             v.add_value(default_location, converter(first_value))
         return v
 
     def get_palette_index(self, color):
         if color == "foreground":
             return 0xFFFF
+        if isinstance(color, int):
+            # Check if palette exists and is long enough
+            if color >= len(self.palette):
+                raise ValueError(
+                    f"Palette index {color} out of range; call SetColors first"
+                )
+        if self.explicit_palette:
+            raise ValueError(
+                "Color specified, but SetColors was called; "
+                "use palette index directly instead"
+            )
         if not isinstance(color, list):
             color = [color]
         if color not in self.palette:
             self.palette.append(color)
         return self.palette.index(color)
 
     def prepare_variables(self, variables):
@@ -602,19 +636,63 @@
         return {
             "Format": 32,
             "CompositeMode": mode,
             "SourcePaint": src,
             "BackdropPaint": dst,
         }
 
+    def SetColors(self, colors):
+        self.explicit_palette = True
+        # colors should be an array of strings or array of arrays
+        for index, color in enumerate(colors):
+            if not isinstance(color, list):
+                color = [color]
+            for c in color:
+                if not re.match(r"^#[0-9a-fA-F]{8}$", c):
+                    raise ValueError(
+                        f"Color {c} at index {index} is not a valid color; "
+                        "should be in the form #RRGGBBAA"
+                    )
+
+        self.palette = compile_palettes(colors)
+
+    def SetPaletteFlags(self, palette_index, flags):
+        if not self.palette:
+            raise ValueError("Use colors or SetPalette before SetPaletteFlags")
+        num_palettes = max(len(colors) for colors in self.palette)
+        if palette_index >= num_palettes:
+            raise ValueError(
+                f"Palette index {palette_index} out of range; "
+                f"should be less than {num_palettes}"
+            )
+        if flags not in ["light", "dark"]:
+            raise ValueError(f"Unknown palette flags {flags}")
+        if palette_index not in self.palette_flags:
+            self.palette_flags[palette_index] = 0
+        if flags == "light":
+            self.palette_flags[palette_index] |= 0x0001
+        else:
+            self.palette_flags[palette_index] |= 0x0002
+
+    def SetDarkMode(self, palette_index):
+        self.SetPaletteFlags(palette_index, "dark")
+
+    def SetLightMode(self, palette_index):
+        self.SetPaletteFlags(palette_index, "light")
+
     def build_palette(self):
-        palette = [compile_colors(stop) for stop in self.palette]
+        palette = compile_palettes(self.palette)
         t_palette = list(map(list, zip(*palette)))
         if t_palette:
             self.font["CPAL"] = buildCPAL(t_palette)
+        if self.palette_flags:
+            self.font["CPAL"].version = 1
+            self.font["CPAL"].paletteTypes = [
+                self.palette_flags.get(i, 0) for i in range(len(t_palette))
+            ]
 
     def build_colr(self, glyphs):
         store = self.varstorebuilder.finish()
         mapping = store.optimize()
         self.deltaset = [mapping[v] for v in self.deltaset]
         self.font["COLR"] = buildCOLR(
             glyphs,
@@ -622,15 +700,20 @@
             varIndexMap=buildDeltaSetIndexMap(self.deltaset),
             version=1,
         )
 
 
 def compile_paints(font, python_code):
     builder = PythonBuilder(font)
-    methods = [x for x in dir(builder) if x.startswith("Paint")]
+    methods = [x for x in dir(builder) if x.startswith("Paint")] + [
+        "SetColors",
+        "SetPaletteFlags",
+        "SetDarkMode",
+        "SetLightMode",
+    ]
     this_locals = {"glyphs": {}, "font": font, "ColorLine": ColorLine}
     for method in methods:
         this_locals[method] = getattr(builder, method)
     exec(python_code, this_locals, this_locals)
 
     builder.build_colr(this_locals["glyphs"])
     builder.build_palette()
```

### Comparing `paintcompiler-0.3.2/Lib/paintcompiler.egg-info/PKG-INFO` & `paintcompiler-0.3.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: paintcompiler
-Version: 0.3.2
-Summary: Paint compiler for COLRv1 fonts
-Author-email: Simon Cozens <simon@simon-cozens.org>
-License: Apache Software License 2.0
-        
-        Copyright (c) 2023, Simon Cozens
-        
-        Licensed under the Apache License, Version 2.0 (the "License");
-        you may not use this file except in compliance with the License.
-        You may obtain a copy of the License at
-        
-        http://www.apache.org/licenses/LICENSE-2.0
-        
-        Unless required by applicable law or agreed to in writing, software
-        distributed under the License is distributed on an "AS IS" BASIS,
-        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-        See the License for the specific language governing permissions and
-        limitations under the License.
-        
-        
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: fontTools>=4.37.3
-
 # Paint compiler for COLRv1 fonts
 
 ```sh
 % paintcompiler --output "Example-Color.ttf" Example-Mono.ttf
 ```
 
 There's a huge amount of very clever and pretty things you can do with the [COLRv1 font fonmat](https://github.com/googlefonts/colr-gradients-spec/blob/main/OFF_AMD2_WD.md). However, most font editors only expose a very small subset of the capabilities of the format. This is largely because, due to the fact that COLRv1 is so rich and extensive, it's not easy to produce a user interface which exposes all the functionality in a flexible way.
@@ -276,21 +250,100 @@
 
 ```python
 PaintComposite(mode, src_paint, dst_paint)
 ```
 
 Composites the source paint onto the destination paint. `mode` must be one of `'clear', 'src', 'dest', 'src_over', 'dest_over', 'src_in', 'dest_in', 'src_out', 'dest_out', 'src_atop', 'dest_atop', 'xor', 'plus', 'screen', 'overlay', 'darken', 'lighten', 'color_dodge', 'color_burn', 'hard_light', 'soft_light', 'difference', 'exclusion', 'multiply', 'hsl_hue', 'hsl_saturation', 'hsl_color', 'hsl_luminosity'`.
 
+## Specifying colors
+
+There are multiple ways of specifying colors to be used to paint your glyphs,
+depending on the complexity of your project. For simple projects, where there
+are few colors and a single color palette, you may find it easiest to specify
+colors directly using a hex string of the form `#RRGGBBAA`, as we have done
+so far in these examples:
+
+```python
+    PaintGlyph("square", PaintSolid("#FF0000FF"))
+```
+
+If you wish to use multiple palettes, you can write a list of strings instead
+of a single string:
+
+```python
+    PaintGlyph("square", PaintSolid([
+        "#FF0000FF",  # Red in pallete 0
+        "#00FF00FF",  # Green in pallete 1
+    ]))
+```
+
+You may to a certain extent mix these two styles: if you have
+
+```python
+    PaintGlyph("square", PaintSolid("#FF0000FF"))
+    ...
+    PaintGlyph("triangle", PaintSolid([
+        "#00FF00FF",
+        "#0000FFFF",
+    ]))
+```
+
+then `square` will be red in both palettes, but triangle will be blue in palette 0
+but blue in pallete 1. However, this will give an error:
+
+```python
+    PaintGlyph("square", PaintSolid([
+        "#FF0000FF",
+        "#00FF00FF",
+        "#0000FFFF",
+    ]))
+    ...
+    PaintGlyph("triangle", PaintSolid([
+        "#00FF00FF",
+        "#0000FFFF",
+        # It's not clear what color should be used for palette 2 here.
+    ]))
+```
+
+For more complex projects, it may be easier to declare your color palettes
+in advance, and give numeric indices into the palette. You do this with the
+`SetColors` function. However, note that the palettes are specified as a
+list of *entries*, just like we have been doing so far.
+
+```python
+SetColors([
+    ["#FF000000FF", "#00FF000FF"],
+    "#0000FFFF",
+])
+
+PaintGlyph("square", 0) # Entry 0 -> red in palette 0, green in palette 1
+PaintGlyph("circle", 1) # Entry 1 -> blue in both palettes
+```
+
+OpenType allows for the designer to specify that certain palettes (not colors!)
+are designed for light-mode or dark-mode interfaces - or even both. You can set
+this information in the font with the `SetDarkMode` and `SetLightMode` functions.
+These take a *palette index* and must be called after colors have been set up:
+
+```python
+SetColors([
+    ["#FF000000FF", "#00FF000FF"],
+    "#0000FFFF",
+])
+SetLightMode(0)  # Red and blue
+SetDarkMode(1)   # Green and blue
+```
+
 ## Why not just use `fontTools.colorLib.builder`?
 
 `paintcompiler` does use the fontTools color builder underneath to construct the COLR tables, but it adds a few helpful facilities on top:
 
 * `paintcompiler` provides a command line interface to add COLR tables. This command line interface allows adding synthetic axes.
 
-* Color palettes are built automatically, so you don't have to assign each color to an index and carry that index around - just specify the color directly. (You can still specify user-selected alternate color palettes by writing the color as an array of options.)
+* Color palettes are built automatically, and with the flexibility described above.
 
 * In `paintcompiler`, paint operations are functions; this makes the syntax considerably less verbose and easier to follow. Compare
 
 ```python
 PaintColrLayers([
     PaintGlyph("square", PaintSolid("#FF0000FF")),
     PaintGlyph("circle", PaintSolid("#0000FFFF"))
```

### Comparing `paintcompiler-0.3.2/Lib/paintdecompiler/__init__.py` & `paintcompiler-0.3.3/Lib/paintdecompiler/__init__.py`

 * *Files identical despite different names*

### Comparing `paintcompiler-0.3.2/PKG-INFO` & `paintcompiler-0.3.3/Lib/paintcompiler.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paintcompiler
-Version: 0.3.2
+Version: 0.3.3
 Summary: Paint compiler for COLRv1 fonts
 Author-email: Simon Cozens <simon@simon-cozens.org>
 License: Apache Software License 2.0
         
         Copyright (c) 2023, Simon Cozens
         
         Licensed under the Apache License, Version 2.0 (the "License");
@@ -276,21 +276,100 @@
 
 ```python
 PaintComposite(mode, src_paint, dst_paint)
 ```
 
 Composites the source paint onto the destination paint. `mode` must be one of `'clear', 'src', 'dest', 'src_over', 'dest_over', 'src_in', 'dest_in', 'src_out', 'dest_out', 'src_atop', 'dest_atop', 'xor', 'plus', 'screen', 'overlay', 'darken', 'lighten', 'color_dodge', 'color_burn', 'hard_light', 'soft_light', 'difference', 'exclusion', 'multiply', 'hsl_hue', 'hsl_saturation', 'hsl_color', 'hsl_luminosity'`.
 
+## Specifying colors
+
+There are multiple ways of specifying colors to be used to paint your glyphs,
+depending on the complexity of your project. For simple projects, where there
+are few colors and a single color palette, you may find it easiest to specify
+colors directly using a hex string of the form `#RRGGBBAA`, as we have done
+so far in these examples:
+
+```python
+    PaintGlyph("square", PaintSolid("#FF0000FF"))
+```
+
+If you wish to use multiple palettes, you can write a list of strings instead
+of a single string:
+
+```python
+    PaintGlyph("square", PaintSolid([
+        "#FF0000FF",  # Red in pallete 0
+        "#00FF00FF",  # Green in pallete 1
+    ]))
+```
+
+You may to a certain extent mix these two styles: if you have
+
+```python
+    PaintGlyph("square", PaintSolid("#FF0000FF"))
+    ...
+    PaintGlyph("triangle", PaintSolid([
+        "#00FF00FF",
+        "#0000FFFF",
+    ]))
+```
+
+then `square` will be red in both palettes, but triangle will be blue in palette 0
+but blue in pallete 1. However, this will give an error:
+
+```python
+    PaintGlyph("square", PaintSolid([
+        "#FF0000FF",
+        "#00FF00FF",
+        "#0000FFFF",
+    ]))
+    ...
+    PaintGlyph("triangle", PaintSolid([
+        "#00FF00FF",
+        "#0000FFFF",
+        # It's not clear what color should be used for palette 2 here.
+    ]))
+```
+
+For more complex projects, it may be easier to declare your color palettes
+in advance, and give numeric indices into the palette. You do this with the
+`SetColors` function. However, note that the palettes are specified as a
+list of *entries*, just like we have been doing so far.
+
+```python
+SetColors([
+    ["#FF000000FF", "#00FF000FF"],
+    "#0000FFFF",
+])
+
+PaintGlyph("square", 0) # Entry 0 -> red in palette 0, green in palette 1
+PaintGlyph("circle", 1) # Entry 1 -> blue in both palettes
+```
+
+OpenType allows for the designer to specify that certain palettes (not colors!)
+are designed for light-mode or dark-mode interfaces - or even both. You can set
+this information in the font with the `SetDarkMode` and `SetLightMode` functions.
+These take a *palette index* and must be called after colors have been set up:
+
+```python
+SetColors([
+    ["#FF000000FF", "#00FF000FF"],
+    "#0000FFFF",
+])
+SetLightMode(0)  # Red and blue
+SetDarkMode(1)   # Green and blue
+```
+
 ## Why not just use `fontTools.colorLib.builder`?
 
 `paintcompiler` does use the fontTools color builder underneath to construct the COLR tables, but it adds a few helpful facilities on top:
 
 * `paintcompiler` provides a command line interface to add COLR tables. This command line interface allows adding synthetic axes.
 
-* Color palettes are built automatically, so you don't have to assign each color to an index and carry that index around - just specify the color directly. (You can still specify user-selected alternate color palettes by writing the color as an array of options.)
+* Color palettes are built automatically, and with the flexibility described above.
 
 * In `paintcompiler`, paint operations are functions; this makes the syntax considerably less verbose and easier to follow. Compare
 
 ```python
 PaintColrLayers([
     PaintGlyph("square", PaintSolid("#FF0000FF")),
     PaintGlyph("circle", PaintSolid("#0000FFFF"))
```

### Comparing `paintcompiler-0.3.2/README.md` & `paintcompiler-0.3.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: paintcompiler
+Version: 0.3.3
+Summary: Paint compiler for COLRv1 fonts
+Author-email: Simon Cozens <simon@simon-cozens.org>
+License: Apache Software License 2.0
+        
+        Copyright (c) 2023, Simon Cozens
+        
+        Licensed under the Apache License, Version 2.0 (the "License");
+        you may not use this file except in compliance with the License.
+        You may obtain a copy of the License at
+        
+        http://www.apache.org/licenses/LICENSE-2.0
+        
+        Unless required by applicable law or agreed to in writing, software
+        distributed under the License is distributed on an "AS IS" BASIS,
+        WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+        See the License for the specific language governing permissions and
+        limitations under the License.
+        
+        
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: fontTools>=4.37.3
+
 # Paint compiler for COLRv1 fonts
 
 ```sh
 % paintcompiler --output "Example-Color.ttf" Example-Mono.ttf
 ```
 
 There's a huge amount of very clever and pretty things you can do with the [COLRv1 font fonmat](https://github.com/googlefonts/colr-gradients-spec/blob/main/OFF_AMD2_WD.md). However, most font editors only expose a very small subset of the capabilities of the format. This is largely because, due to the fact that COLRv1 is so rich and extensive, it's not easy to produce a user interface which exposes all the functionality in a flexible way.
@@ -250,21 +276,100 @@
 
 ```python
 PaintComposite(mode, src_paint, dst_paint)
 ```
 
 Composites the source paint onto the destination paint. `mode` must be one of `'clear', 'src', 'dest', 'src_over', 'dest_over', 'src_in', 'dest_in', 'src_out', 'dest_out', 'src_atop', 'dest_atop', 'xor', 'plus', 'screen', 'overlay', 'darken', 'lighten', 'color_dodge', 'color_burn', 'hard_light', 'soft_light', 'difference', 'exclusion', 'multiply', 'hsl_hue', 'hsl_saturation', 'hsl_color', 'hsl_luminosity'`.
 
+## Specifying colors
+
+There are multiple ways of specifying colors to be used to paint your glyphs,
+depending on the complexity of your project. For simple projects, where there
+are few colors and a single color palette, you may find it easiest to specify
+colors directly using a hex string of the form `#RRGGBBAA`, as we have done
+so far in these examples:
+
+```python
+    PaintGlyph("square", PaintSolid("#FF0000FF"))
+```
+
+If you wish to use multiple palettes, you can write a list of strings instead
+of a single string:
+
+```python
+    PaintGlyph("square", PaintSolid([
+        "#FF0000FF",  # Red in pallete 0
+        "#00FF00FF",  # Green in pallete 1
+    ]))
+```
+
+You may to a certain extent mix these two styles: if you have
+
+```python
+    PaintGlyph("square", PaintSolid("#FF0000FF"))
+    ...
+    PaintGlyph("triangle", PaintSolid([
+        "#00FF00FF",
+        "#0000FFFF",
+    ]))
+```
+
+then `square` will be red in both palettes, but triangle will be blue in palette 0
+but blue in pallete 1. However, this will give an error:
+
+```python
+    PaintGlyph("square", PaintSolid([
+        "#FF0000FF",
+        "#00FF00FF",
+        "#0000FFFF",
+    ]))
+    ...
+    PaintGlyph("triangle", PaintSolid([
+        "#00FF00FF",
+        "#0000FFFF",
+        # It's not clear what color should be used for palette 2 here.
+    ]))
+```
+
+For more complex projects, it may be easier to declare your color palettes
+in advance, and give numeric indices into the palette. You do this with the
+`SetColors` function. However, note that the palettes are specified as a
+list of *entries*, just like we have been doing so far.
+
+```python
+SetColors([
+    ["#FF000000FF", "#00FF000FF"],
+    "#0000FFFF",
+])
+
+PaintGlyph("square", 0) # Entry 0 -> red in palette 0, green in palette 1
+PaintGlyph("circle", 1) # Entry 1 -> blue in both palettes
+```
+
+OpenType allows for the designer to specify that certain palettes (not colors!)
+are designed for light-mode or dark-mode interfaces - or even both. You can set
+this information in the font with the `SetDarkMode` and `SetLightMode` functions.
+These take a *palette index* and must be called after colors have been set up:
+
+```python
+SetColors([
+    ["#FF000000FF", "#00FF000FF"],
+    "#0000FFFF",
+])
+SetLightMode(0)  # Red and blue
+SetDarkMode(1)   # Green and blue
+```
+
 ## Why not just use `fontTools.colorLib.builder`?
 
 `paintcompiler` does use the fontTools color builder underneath to construct the COLR tables, but it adds a few helpful facilities on top:
 
 * `paintcompiler` provides a command line interface to add COLR tables. This command line interface allows adding synthetic axes.
 
-* Color palettes are built automatically, so you don't have to assign each color to an index and carry that index around - just specify the color directly. (You can still specify user-selected alternate color palettes by writing the color as an array of options.)
+* Color palettes are built automatically, and with the flexibility described above.
 
 * In `paintcompiler`, paint operations are functions; this makes the syntax considerably less verbose and easier to follow. Compare
 
 ```python
 PaintColrLayers([
     PaintGlyph("square", PaintSolid("#FF0000FF")),
     PaintGlyph("circle", PaintSolid("#0000FFFF"))
```

### Comparing `paintcompiler-0.3.2/example/COLRv1-Test.glyphs` & `paintcompiler-0.3.3/example/COLRv1-Test.glyphs`

 * *Files identical despite different names*

### Comparing `paintcompiler-0.3.2/example/build.sh` & `paintcompiler-0.3.3/example/build.sh`

 * *Files identical despite different names*

### Comparing `paintcompiler-0.3.2/example/paints.py` & `paintcompiler-0.3.3/example/paints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-BLUE = "#4285F4FF"
-GREEN = "#34A853FF"
-RED = "#EA4335FF"
+BLUE = ["#4285F4FF", "#02317DFF"]
+GREEN = "#035719FF"
+RED = ["#EA4335FF", "#8C0D03FF"]
 
 
 ax = {}
 
 for axis in font["fvar"].axes:
     tag = axis.axisTag
     ax[tag] = {
@@ -166,17 +166,15 @@
         PaintScale(1.2, 0.8, (300, 200), BLUESQUARE),
     ]
 )
 
 glyphs["p19_PaintVarScaleAroundCenter"] = PaintColrLayers(
     [
         REDSQUARE,
-        PaintScale(
-            ax["SCLX"], ax["SCLY"], (ax["STAX"], ax["STAY"]), BLUESQUARE
-        ),
+        PaintScale(ax["SCLX"], ax["SCLY"], (ax["STAX"], ax["STAY"]), BLUESQUARE),
     ]
 )
 
 glyphs["p20_PaintScaleUniform"] = PaintColrLayers(
     [
         REDSQUARE,
         PaintScale(0.8, BLUESQUARE),
@@ -196,17 +194,15 @@
         PaintScale(0.8, BLUESQUARE, center=(300, 250)),
     ]
 )
 
 glyphs["p23_PaintVarScaleUniformAroundCenter"] = PaintColrLayers(
     [
         REDSQUARE,
-        PaintScale(
-            ax["SCLX"], BLUESQUARE, center= (ax["STAX"], ax["STAY"])
-        ),
+        PaintScale(ax["SCLX"], BLUESQUARE, center=(ax["STAX"], ax["STAY"])),
     ]
 )
 
 glyphs["p24_PaintRotate"] = PaintColrLayers(
     [
         REDSQUARE,
         PaintRotate(-15, BLUESQUARE),
@@ -255,18 +251,19 @@
         PaintSkew(-15, 10, BLUESQUARE, center=(350, 200)),
     ]
 )
 
 glyphs["p31_PaintVarSkewAroundCenter"] = PaintColrLayers(
     [
         REDSQUARE,
-        PaintSkew(
-            ax["STAA"], ax["ENDA"], BLUESQUARE, center=(ax["STAX"], ax["STAY"])
-        ),
+        PaintSkew(ax["STAA"], ax["ENDA"], BLUESQUARE, center=(ax["STAX"], ax["STAY"])),
     ]
 )
 
 glyphs["p32_PaintComposite"] = PaintComposite(
     "multiply",
     PaintComposite("dest_out", GREENSTAR, BLUECIRCLE),
     REDSQUARE,
 )
+
+SetLightMode(0)
+SetDarkMode(1)
```

