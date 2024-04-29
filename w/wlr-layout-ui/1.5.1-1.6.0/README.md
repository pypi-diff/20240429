# Comparing `tmp/wlr_layout_ui-1.5.1.tar.gz` & `tmp/wlr_layout_ui-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.5.1.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.6.0.tar", max compression
```

## Comparing `wlr_layout_ui-1.5.1.tar` & `wlr_layout_ui-1.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.5.1/LICENSE
--rw-r--r--   0        0        0      558 2024-03-30 19:04:20.505512 wlr_layout_ui-1.5.1/README.md
--rw-r--r--   0        0        0      652 2024-04-24 21:18:42.614934 wlr_layout_ui-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     2435 2024-02-19 21:26:30.823859 wlr_layout_ui-1.5.1/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4249 2024-04-24 19:45:02.396301 wlr_layout_ui-1.5.1/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      387 2024-03-30 19:04:20.505512 wlr_layout_ui-1.5.1/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    23746 2024-04-24 21:18:19.084465 wlr_layout_ui-1.5.1/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      469 2023-10-24 21:30:47.569956 wlr_layout_ui-1.5.1/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5542 2024-04-24 19:21:05.917645 wlr_layout_ui-1.5.1/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.5.1/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1706 2024-03-30 19:04:20.505512 wlr_layout_ui-1.5.1/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4525 2024-04-24 20:29:33.972898 wlr_layout_ui-1.5.1/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12366 2024-03-30 19:04:20.505512 wlr_layout_ui-1.5.1/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1323 1970-01-01 00:00:00.000000 wlr_layout_ui-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.0/LICENSE
+-rw-r--r--   0        0        0      877 2024-04-29 21:22:39.498616 wlr_layout_ui-1.6.0/README.md
+-rw-r--r--   0        0        0      652 2024-04-29 21:33:09.851048 wlr_layout_ui-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2435 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.0/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4249 2024-04-29 20:48:36.973600 wlr_layout_ui-1.6.0/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.0/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    24752 2024-04-29 21:31:40.219241 wlr_layout_ui-1.6.0/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.0/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5508 2024-04-29 20:53:16.599453 wlr_layout_ui-1.6.0/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.0/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.0/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4529 2024-04-29 21:19:26.061682 wlr_layout_ui-1.6.0/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12366 2024-04-29 20:52:12.478107 wlr_layout_ui-1.6.0/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     1642 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.0/PKG-INFO
```

### Comparing `wlr_layout_ui-1.5.1/LICENSE` & `wlr_layout_ui-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.5.1/README.md` & `wlr_layout_ui-1.6.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 # Wlr layout UI
 
-An simple GUI to setup the screens layout on wlroots based systems.
+An simple GUI to setup the screens layout on wlroots based systems and X11 (using xrandr), Hyprland is the first class user.
+
+## Features
+
+- Load and save profiles
+- Set the screen settings
+  - Layout: position, rotation and scale
+  - Resolution
+  - Refresh rate
+
+> [!note]
+> Non Hyprland should work without screen rotation support
+
+## Video / Demo
+
+A bit outdated, but still relevant.
 
 [![Video](https://img.youtube.com/vi/bJxVIu9cMzg/0.jpg)](https://www.youtube.com/watch?v=bJxVIu9cMzg)
 
 ## Requires
 
 - wlr-randr (if not using Hyprland >= 0.37)
 - Python: pyglet, tomli
```

### Comparing `wlr_layout_ui-1.5.1/pyproject.toml` & `wlr_layout_ui-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.5.1"
+version = "1.6.0"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
 license = "MIT"
```

### Comparing `wlr_layout_ui-1.5.1/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.6.0/src/wlr_layout_ui/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import sys
 import time
 
 import pyglet
 
 from .gui import UI
-from .settings import UI_RATIO, PROG_NAME, LEGACY, reload_pre_commands
 from .screens import displayInfo, load
-from .utils import make_command, Rect
+from .settings import LEGACY, PROG_NAME, UI_RATIO, reload_pre_commands
+from .utils import Rect, make_command
 
 try:
     import setproctitle
 
     setproctitle.setproctitle(PROG_NAME)
 except ImportError:
     pass
```

### Comparing `wlr_layout_ui-1.5.1/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.6.0/src/wlr_layout_ui/displaywidget.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.5.1/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.6.0/src/wlr_layout_ui/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,37 @@
-import time
 import math
 import os
 import re
+import time
 
 import pyglet
 
-from .widgets import Button, HBox, VBox, Dropdown, Style, Widget
-from .settings import FONT, WINDOW_MARGIN, UI_RATIO, LEGACY, PROG_NAME
-from .settings import ALLOW_DESELECT, reload_pre_commands
 from .displaywidget import GuiScreen
-from .utils import sorted_resolutions, sorted_frequencies, find_matching_mode
-from .utils import compute_bounding_box, trim_rects_flip_y, make_command, Rect
-from .profiles import save_profile, load_profiles
+from .profiles import load_profiles, save_profile
 from .screens import displayInfo, load
+from .settings import (
+    ALLOW_DESELECT,
+    FONT,
+    LEGACY,
+    PROG_NAME,
+    UI_RATIO,
+    WINDOW_MARGIN,
+    reload_pre_commands,
+)
+from .utils import (
+    Rect,
+    compute_bounding_box,
+    config,
+    find_matching_mode,
+    make_command,
+    sorted_frequencies,
+    sorted_resolutions,
+    trim_rects_flip_y,
+)
+from .widgets import Button, Dropdown, HBox, Style, VBox, Widget
 
 hex_re = re.compile("^[0-9x]+$")
 
 CONFIRM_DELAY = 20
 
 
 def get_size(screen, scale=0):
@@ -102,22 +117,23 @@
         self.resolutions = Dropdown(
             ref_rect.copy(),
             label="Resolution",
             options=[],
             onchange=self.action_update_screen_spec,
             # invert=True,
         )
+        ref_rect.width = int(ref_rect.width * 0.7)
         self.freqs = Dropdown(
             ref_rect.copy(),
             label="Rate",
             options=[],
             onchange=self.action_update_mode,
             # invert=True,
         )
-        ref_rect.width //= 2
+
         self.rotation = Dropdown(
             ref_rect.copy(),
             label="Rotation",
             options=[
                 {"name": "0", "value": 0},
                 {"name": "90", "value": 1},
                 {"name": "180", "value": 2},
@@ -126,27 +142,49 @@
                 {"name": "flip 90", "value": 5},
                 {"name": "flip 180", "value": 6},
                 {"name": "flip 270", "value": 7},
             ],
             onchange=self.action_update_rotation,
             # invert=True,
         )
+        ref_rect.width = int(ref_rect.width * 0.8)
+        self.scale_ratio = Dropdown(
+            ref_rect.copy(),
+            label="Scale",
+            options=[
+                {"name": "100%", "value": 1},
+                {"name": "90%", "value": 0.833333},
+                {"name": "80%", "value": 0.666667},
+                {"name": "120%", "value": 1.2},
+                {"name": "150%", "value": 1.5},
+                {"name": "200%", "value": 2.0},
+            ],
+            onchange=self.action_update_scale,
+            # invert=True,
+        )
         ref_rect.width //= 2
         self.on_off_but = Button(
             ref_rect.copy(),
             label="On",
             toggled_label="Off",
             action=self.action_toggle_screen_power,
             style=Style(highlight=(200, 100, 150), color=(100, 200, 150)),
             togglable=True,
         )
 
-        self.settings_box = HBox(
-            widgets=[self.resolutions, self.freqs, self.rotation, self.on_off_but]
-        )
+        base_widgets: list[Widget] = [
+            self.resolutions,
+            self.freqs,
+            self.rotation,
+        ]
+        if config.get("hyprland"):
+            base_widgets.append(self.scale_ratio)
+        base_widgets.append(self.on_off_but)
+
+        self.settings_box = HBox(widgets=base_widgets)
         self.require_selected_item.add(self.settings_box)
         # }}}
 
         self._widgets: list[Widget] = [
             self.action_box,
             self.settings_box,
             self.sidepanel,
@@ -216,15 +254,15 @@
                 )
                 if is_rotated:
                     y -= screen.mode.height - screen.mode.width
 
                 rect = Rect(
                     int(x / UI_RATIO),
                     -int(y / UI_RATIO) - h,
-                    int((screen.mode.width / UI_RATIO) / screen.scale),
+                    w,
                     h,
                 )
             else:
                 rect = Rect(
                     int(x / UI_RATIO),
                     int(y / UI_RATIO),
                     int((max_width / UI_RATIO) / screen.scale),
@@ -598,14 +636,20 @@
                     found.screen.available,
                     (info["width"], info["height"]),
                     info["freq"],
                 )
                 found.target_rect = srect
         self.center_layout()
 
+    def action_update_scale(self):
+        monitor = self.selected_item
+        assert monitor
+        monitor.screen.scale = self.scale_ratio.get_value()
+        monitor.target_rect.width, monitor.target_rect.height = get_size(monitor.screen)
+
     def action_update_frequencies(self, screen, mode=None):
         if mode is None:
             cur_mode = screen.screen.mode.width, screen.screen.mode.height
         else:
             cur_mode = mode
         freqs = sorted_frequencies(screen.screen.available, cur_mode[0], cur_mode[1])
         self.freqs.options = [{"name": f"{r:.2f} Hz", "value": r} for r in freqs]
```

### Comparing `wlr_layout_ui-1.5.1/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.6.0/src/wlr_layout_ui/screens.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+import difflib
+import json
 import os
 import re
-import json
-from typing import Tuple
 import subprocess
-import difflib
+from dataclasses import dataclass, field
+from typing import Tuple
 
 from .utils import config
-from dataclasses import dataclass, field
 
 __all__ = ["Mode", "Screen", "load", "LEGACY"]
 
 LEGACY = not os.environ.get("WAYLAND_DISPLAY", False)
 MODE_RE = re.compile(r"^(?P<width>\d+)x(?P<height>\d+)(?P<x>[+-]\d+)(?P<y>[+-]\d+)$")
 
 
@@ -81,18 +81,17 @@
         displayInfo.clear()
 
     try:
         version = json.loads(subprocess.getoutput("hyprctl -j version"))["tag"]
         version = version[1:].split(".")
         major = int(version[0])
         minor = int(version[1])
-        _patch = int(version[2])
         new_hyprland = major == 0 and minor >= 37 or major > 0
     except (KeyError, json.JSONDecodeError):
-        new_hyprland = False
+        new_hyprland = True
 
     if new_hyprland:
         config["hyprland"] = True
         load_from_hyprctl()
         return
 
     out = subprocess.getoutput("xrandr" if LEGACY else "wlr-randr")
```

### Comparing `wlr_layout_ui-1.5.1/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.6.0/src/wlr_layout_ui/shapes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import cache
+
 from .factories import makeCircle, makeRectangle
 
 
 @cache
 def makeRoundedRectangle(rect, radius, color):
     return RoundedRectangle(rect, radius, color)
```

### Comparing `wlr_layout_ui-1.5.1/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.6.0/src/wlr_layout_ui/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     command = ['hyprctl --batch "']
 
     for screen, rect in zip(screens, screens_rect):
         if not screen.active:
             command.append(f"keyword monitor {screen.uid},disable ;")
             continue
         command.append(
-            f"keyword monitor {screen.uid},{screen.mode},{int(rect.x)}x{int(rect.y)},{screen.scale},transform,{screen.transform} ;"
+            f"keyword monitor {screen.uid},{screen.mode},{int(rect.x)}x{int(rect.y)},{screen.scale:.6f},transform,{screen.transform} ;"
         )
 
     cmd = " ".join(command + ['"'])
     return cmd
 
 
 def make_command_legacy(screens, rects, wayland=False):
```

### Comparing `wlr_layout_ui-1.5.1/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.6.0/src/wlr_layout_ui/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 
 from pyglet.shapes import Triangle
 
+from .factories import makeLabel, makeRectangle
 from .settings import FONT, WIDGETS_RADIUS
-from .utils import brighten, Rect
 from .shapes import RoundedRectangle
-from .factories import makeRectangle, makeLabel
+from .utils import Rect, brighten
 
 
 class Widget:
     def __init__(self, rect, style):
         self.rect = rect
         self.style = style if style else Style()
         self.valign = "bottom"
```

### Comparing `wlr_layout_ui-1.5.1/PKG-INFO` & `wlr_layout_ui-1.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.5.1
+Version: 1.6.0
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,30 @@
 Requires-Dist: pyglet (>=2.0.0,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Wlr layout UI
 
-An simple GUI to setup the screens layout on wlroots based systems.
+An simple GUI to setup the screens layout on wlroots based systems and X11 (using xrandr), Hyprland is the first class user.
+
+## Features
+
+- Load and save profiles
+- Set the screen settings
+  - Layout: position, rotation and scale
+  - Resolution
+  - Refresh rate
+
+> [!note]
+> Non Hyprland should work without screen rotation support
+
+## Video / Demo
+
+A bit outdated, but still relevant.
 
 [![Video](https://img.youtube.com/vi/bJxVIu9cMzg/0.jpg)](https://www.youtube.com/watch?v=bJxVIu9cMzg)
 
 ## Requires
 
 - wlr-randr (if not using Hyprland >= 0.37)
 - Python: pyglet, tomli
```

