# Comparing `tmp/wlr_layout_ui-1.6.0.tar.gz` & `tmp/wlr_layout_ui-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wlr_layout_ui-1.6.0.tar", max compression
+gzip compressed data, was "wlr_layout_ui-1.6.1.tar", max compression
```

## Comparing `wlr_layout_ui-1.6.0.tar` & `wlr_layout_ui-1.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.0/LICENSE
--rw-r--r--   0        0        0      877 2024-04-29 21:22:39.498616 wlr_layout_ui-1.6.0/README.md
--rw-r--r--   0        0        0      652 2024-04-29 21:33:09.851048 wlr_layout_ui-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2435 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.0/src/wlr_layout_ui/__init__.py
--rw-r--r--   0        0        0     4249 2024-04-29 20:48:36.973600 wlr_layout_ui-1.6.0/src/wlr_layout_ui/displaywidget.py
--rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.0/src/wlr_layout_ui/factories.py
--rw-r--r--   0        0        0    24752 2024-04-29 21:31:40.219241 wlr_layout_ui-1.6.0/src/wlr_layout_ui/gui.py
--rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.0/src/wlr_layout_ui/profiles.py
--rw-r--r--   0        0        0     5508 2024-04-29 20:53:16.599453 wlr_layout_ui-1.6.0/src/wlr_layout_ui/screens.py
--rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.0/src/wlr_layout_ui/settings.py
--rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.0/src/wlr_layout_ui/shapes.py
--rw-r--r--   0        0        0     4529 2024-04-29 21:19:26.061682 wlr_layout_ui-1.6.0/src/wlr_layout_ui/utils.py
--rw-r--r--   0        0        0    12366 2024-04-29 20:52:12.478107 wlr_layout_ui-1.6.0/src/wlr_layout_ui/widgets.py
--rw-r--r--   0        0        0     1642 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-08 16:08:47.075411 wlr_layout_ui-1.6.1/LICENSE
+-rw-r--r--   0        0        0      888 2024-04-29 21:35:54.187715 wlr_layout_ui-1.6.1/README.md
+-rw-r--r--   0        0        0      652 2024-04-29 21:37:08.252558 wlr_layout_ui-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2435 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.1/src/wlr_layout_ui/__init__.py
+-rw-r--r--   0        0        0     4249 2024-04-29 20:48:36.973600 wlr_layout_ui-1.6.1/src/wlr_layout_ui/displaywidget.py
+-rw-r--r--   0        0        0      388 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.1/src/wlr_layout_ui/factories.py
+-rw-r--r--   0        0        0    24772 2024-04-29 21:36:28.245076 wlr_layout_ui-1.6.1/src/wlr_layout_ui/gui.py
+-rw-r--r--   0        0        0      470 2024-04-29 20:52:12.471440 wlr_layout_ui-1.6.1/src/wlr_layout_ui/profiles.py
+-rw-r--r--   0        0        0     5508 2024-04-29 20:53:16.599453 wlr_layout_ui-1.6.1/src/wlr_layout_ui/screens.py
+-rw-r--r--   0        0        0      274 2024-04-08 23:21:29.224449 wlr_layout_ui-1.6.1/src/wlr_layout_ui/settings.py
+-rw-r--r--   0        0        0     1707 2024-04-29 20:52:12.474773 wlr_layout_ui-1.6.1/src/wlr_layout_ui/shapes.py
+-rw-r--r--   0        0        0     4529 2024-04-29 21:19:26.061682 wlr_layout_ui-1.6.1/src/wlr_layout_ui/utils.py
+-rw-r--r--   0        0        0    12366 2024-04-29 20:52:12.478107 wlr_layout_ui-1.6.1/src/wlr_layout_ui/widgets.py
+-rw-r--r--   0        0        0     1653 1970-01-01 00:00:00.000000 wlr_layout_ui-1.6.1/PKG-INFO
```

### Comparing `wlr_layout_ui-1.6.0/LICENSE` & `wlr_layout_ui-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.0/README.md` & `wlr_layout_ui-1.6.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - Load and save profiles
 - Set the screen settings
   - Layout: position, rotation and scale
   - Resolution
   - Refresh rate
 
 > [!note]
-> Non Hyprland should work without screen rotation support
+> Non Hyprland should work without screen rotation or scaling support
 
 ## Video / Demo
 
 A bit outdated, but still relevant.
 
 [![Video](https://img.youtube.com/vi/bJxVIu9cMzg/0.jpg)](https://www.youtube.com/watch?v=bJxVIu9cMzg)
```

### Comparing `wlr_layout_ui-1.6.0/pyproject.toml` & `wlr_layout_ui-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wlr-layout-ui"
-version = "1.6.0"
+version = "1.6.1"
 description = "A tiny GUI to configure screen layouts on wayland"
 authors = ["fdev31 <fdev31@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/fdev31/wlr-layout-ui"
 packages = [{include = "wlr_layout_ui", from = "src"}]
 license = "MIT"
```

### Comparing `wlr_layout_ui-1.6.0/src/wlr_layout_ui/__init__.py` & `wlr_layout_ui-1.6.1/src/wlr_layout_ui/__init__.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.0/src/wlr_layout_ui/displaywidget.py` & `wlr_layout_ui-1.6.1/src/wlr_layout_ui/displaywidget.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.0/src/wlr_layout_ui/gui.py` & `wlr_layout_ui-1.6.1/src/wlr_layout_ui/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,17 +170,17 @@
             style=Style(highlight=(200, 100, 150), color=(100, 200, 150)),
             togglable=True,
         )
 
         base_widgets: list[Widget] = [
             self.resolutions,
             self.freqs,
-            self.rotation,
         ]
         if config.get("hyprland"):
+            base_widgets.append(self.rotation)
             base_widgets.append(self.scale_ratio)
         base_widgets.append(self.on_off_but)
 
         self.settings_box = HBox(widgets=base_widgets)
         self.require_selected_item.add(self.settings_box)
         # }}}
```

### Comparing `wlr_layout_ui-1.6.0/src/wlr_layout_ui/screens.py` & `wlr_layout_ui-1.6.1/src/wlr_layout_ui/screens.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.0/src/wlr_layout_ui/shapes.py` & `wlr_layout_ui-1.6.1/src/wlr_layout_ui/shapes.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.0/src/wlr_layout_ui/utils.py` & `wlr_layout_ui-1.6.1/src/wlr_layout_ui/utils.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.0/src/wlr_layout_ui/widgets.py` & `wlr_layout_ui-1.6.1/src/wlr_layout_ui/widgets.py`

 * *Files identical despite different names*

### Comparing `wlr_layout_ui-1.6.0/PKG-INFO` & `wlr_layout_ui-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wlr-layout-ui
-Version: 1.6.0
+Version: 1.6.1
 Summary: A tiny GUI to configure screen layouts on wayland
 Home-page: https://github.com/fdev31/wlr-layout-ui
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,15 +28,15 @@
 - Load and save profiles
 - Set the screen settings
   - Layout: position, rotation and scale
   - Resolution
   - Refresh rate
 
 > [!note]
-> Non Hyprland should work without screen rotation support
+> Non Hyprland should work without screen rotation or scaling support
 
 ## Video / Demo
 
 A bit outdated, but still relevant.
 
 [![Video](https://img.youtube.com/vi/bJxVIu9cMzg/0.jpg)](https://www.youtube.com/watch?v=bJxVIu9cMzg)
```

