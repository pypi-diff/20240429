# Comparing `tmp/magictk-1.0.1.58.tar.gz` & `tmp/magictk-1.0.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magictk-1.0.1.58.tar", last modified: Sat Apr 27 14:05:36 2024, max compression
+gzip compressed data, was "magictk-1.0.1.59.tar", last modified: Mon Apr 29 13:15:48 2024, max compression
```

## Comparing `magictk-1.0.1.58.tar` & `magictk-1.0.1.59.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:05:36.115414 magictk-1.0.1.58/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-27 14:05:35.000000 magictk-1.0.1.58/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-27 14:05:36.115414 magictk-1.0.1.58/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1683 2024-04-27 14:05:35.000000 magictk-1.0.1.58/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:05:36.115414 magictk-1.0.1.58/magictk/
--rw-r--r--   0 root         (0) root         (0)      514 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9695 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/_window_ctl.py
--rw-r--r--   0 root         (0) root         (0)    13250 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/_window_size.py
--rw-r--r--   0 root         (0) root         (0)     3363 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/basicwindow.py
--rw-r--r--   0 root         (0) root         (0)    17974 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/button.py
--rw-r--r--   0 root         (0) root         (0)    11247 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/checkbox.py
--rw-r--r--   0 root         (0) root         (0)     1944 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/color_tmpl.py
--rw-r--r--   0 root         (0) root         (0)    12242 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/entry.py
--rw-r--r--   0 root         (0) root         (0)      578 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/fontconfig.py
--rw-r--r--   0 root         (0) root         (0)     3725 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/frame.py
--rw-r--r--   0 root         (0) root         (0)    15906 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/icon.ico
--rw-r--r--   0 root         (0) root         (0)     1890 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/icon.py
--rw-r--r--   0 root         (0) root         (0)       70 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/mtk.py
--rw-r--r--   0 root         (0) root         (0)      720 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/photoload.py
--rw-r--r--   0 root         (0) root         (0)     5995 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/progressbar.py
--rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/res.pickle
--rw-r--r--   0 root         (0) root         (0)     8106 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/scrollbar.py
--rw-r--r--   0 root         (0) root         (0)     6178 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/select.py
--rw-r--r--   0 root         (0) root         (0)      372 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/style.py
--rw-r--r--   0 root         (0) root         (0)    11076 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/submenu.py
--rw-r--r--   0 root         (0) root         (0)    10245 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/window.py
--rw-r--r--   0 root         (0) root         (0)     2647 2024-04-27 14:05:35.000000 magictk-1.0.1.58/magictk/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 14:05:36.115414 magictk-1.0.1.58/magictk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      597 2024-04-27 14:05:36.000000 magictk-1.0.1.58/magictk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      629 2024-04-27 14:05:36.000000 magictk-1.0.1.58/magictk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 14:05:36.000000 magictk-1.0.1.58/magictk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-27 14:05:36.000000 magictk-1.0.1.58/magictk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 14:05:36.115414 magictk-1.0.1.58/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-27 14:05:35.000000 magictk-1.0.1.58/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:15:48.112697 magictk-1.0.1.59/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-04-29 13:15:47.000000 magictk-1.0.1.59/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-29 13:15:48.112697 magictk-1.0.1.59/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-04-29 13:15:47.000000 magictk-1.0.1.59/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:15:48.112697 magictk-1.0.1.59/magictk/
+-rw-r--r--   0 root         (0) root         (0)      514 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/_window_ctl.py
+-rw-r--r--   0 root         (0) root         (0)    13250 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/_window_size.py
+-rw-r--r--   0 root         (0) root         (0)     3363 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/basicwindow.py
+-rw-r--r--   0 root         (0) root         (0)    17993 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/button.py
+-rw-r--r--   0 root         (0) root         (0)    11247 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/checkbox.py
+-rw-r--r--   0 root         (0) root         (0)     2069 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/color_tmpl.py
+-rw-r--r--   0 root         (0) root         (0)    12242 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/entry.py
+-rw-r--r--   0 root         (0) root         (0)      578 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/fontconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/frame.py
+-rw-r--r--   0 root         (0) root         (0)    15906 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/icon.ico
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/icon.py
+-rw-r--r--   0 root         (0) root         (0)       70 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/mtk.py
+-rw-r--r--   0 root         (0) root         (0)      720 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/photoload.py
+-rw-r--r--   0 root         (0) root         (0)     5995 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/progressbar.py
+-rw-r--r--   0 root         (0) root         (0) 11073665 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/res.pickle
+-rw-r--r--   0 root         (0) root         (0)     8106 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/scrollbar.py
+-rw-r--r--   0 root         (0) root         (0)     6178 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/select.py
+-rw-r--r--   0 root         (0) root         (0)      372 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/style.py
+-rw-r--r--   0 root         (0) root         (0)    11076 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/submenu.py
+-rw-r--r--   0 root         (0) root         (0)    10245 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/window.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 13:15:48.112697 magictk-1.0.1.59/magictk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      629 2024-04-29 13:15:48.000000 magictk-1.0.1.59/magictk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-29 13:15:47.000000 magictk-1.0.1.59/magictk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 13:15:48.112697 magictk-1.0.1.59/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-29 13:15:47.000000 magictk-1.0.1.59/setup.py
```

### Comparing `magictk-1.0.1.58/PKG-INFO` & `magictk-1.0.1.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 1.0.1.58
+Version: 1.0.1.59
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-1.0.1.58/README.md` & `magictk-1.0.1.59/README.md`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/__init__.py` & `magictk-1.0.1.59/magictk/__init__.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/_window_ctl.py` & `magictk-1.0.1.59/magictk/_window_ctl.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/_window_size.py` & `magictk-1.0.1.59/magictk/_window_size.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/basicwindow.py` & `magictk-1.0.1.59/magictk/basicwindow.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/button.py` & `magictk-1.0.1.59/magictk/button.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,19 +301,19 @@
         for i in border_info:
             x_n = 0
             for j in i:
                 px = x+y_n+1
                 py = y+x_n+1
                 lcolor = j
                 g_color = color_tmpl.mix_color(
-                    "#FFFFFF", self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
+                    self._color_text, self.color[self._color_bd], int((1-lcolor/255)*1000)/1000)
                 f_color = color_tmpl.mix_color(
-                    "#FFFFFF", self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
+                    self._color_text, self.color[self._color_fg1], int((1-lcolor/255)*1000)/1000)
                 h_color = color_tmpl.mix_color(
-                    "#FFFFFF", self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
+                    self._color_text, self.color[self._color_fg2], int((1-lcolor/255)*1000)/1000)
 
                 obj = self.canvas.create_rectangle(
                     px, py, px, py, width=0, fill=g_color)
 
                 def update_color(obj, g_color, f_color, h_color):
                     if (self._is_hover == 2):
                         self.canvas.itemconfig(
@@ -382,15 +382,15 @@
                 self._fill_gc.append(g_color)
                 self._fill_fc.append(f_color)
                 self._fill_hc.append(h_color)
                 self._fill_obj.append(obj)
                 x_n += 1
             y_n += 1
 
-    def __init__(self, master=None, root_anim=None, color_type="primary", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None, iconname="", iconsize=24):
+    def __init__(self, master=None, root_anim=None, color_type="plain", w=80, h=30, text="Button", func=lambda s: print("Press"), color_list: dict = None, _dis_color=None, iconname="", iconsize=24):
         if (_dis_color is None):
             self._color_bd = color_type
             self._color_bg = color_type
             self._color_bg1 = color_type
             self._color_fg1 = color_type+"_light3"
             self._color_fg = color_type+"_dark"
             self._color_fg3 = color_type+"_light3"
```

### Comparing `magictk-1.0.1.58/magictk/checkbox.py` & `magictk-1.0.1.59/magictk/checkbox.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/color_tmpl.py` & `magictk-1.0.1.59/magictk/color_tmpl.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     "danger_dark": "#C45656",
     "info": "#909399",
     "info_light": "#E9E9EB",
     "info_light2": "#F4F4F5",
     "info_light3": "#B1B3B8",
     "info_dark": "#73767A",
     "plain": "#606266",
+    "plain_light": "#C6E2FF",
+    "plain_light2": "#ECF5FF",
+    "plain_light3": "#79BBFF",
+    "plain_dark": "#337ECC",
     "primary_text": "#303133",
     "regular_text": "#606266",
     "secondary_text": "#909399",
     "placeholder": "#C0C4CC",
     "placeholder_light": "#F5F7FA",
     "border_base": "#DCDFE6",
     "border_light": "#E4E7ED",
```

### Comparing `magictk-1.0.1.58/magictk/entry.py` & `magictk-1.0.1.59/magictk/entry.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/fontconfig.py` & `magictk-1.0.1.59/magictk/fontconfig.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/frame.py` & `magictk-1.0.1.59/magictk/frame.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/icon.ico` & `magictk-1.0.1.59/magictk/icon.ico`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/icon.py` & `magictk-1.0.1.59/magictk/icon.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/photoload.py` & `magictk-1.0.1.59/magictk/photoload.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/progressbar.py` & `magictk-1.0.1.59/magictk/progressbar.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/res.pickle` & `magictk-1.0.1.59/magictk/res.pickle`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/scrollbar.py` & `magictk-1.0.1.59/magictk/scrollbar.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/select.py` & `magictk-1.0.1.59/magictk/select.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/submenu.py` & `magictk-1.0.1.59/magictk/submenu.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/window.py` & `magictk-1.0.1.59/magictk/window.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk/workspace.py` & `magictk-1.0.1.59/magictk/workspace.py`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/magictk.egg-info/PKG-INFO` & `magictk-1.0.1.59/magictk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: magictk
-Version: 1.0.1.58
+Version: 1.0.1.59
 Summary: Some tkinter weights look like element-plus
 Home-page: http://git.hmtsai.cn/cxykevin/magictk.git
 Author: cxykevin|git.hmtsai.cn
 Author-email: cxykevin@yeah.net
 License: GPLv2
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `magictk-1.0.1.58/magictk.egg-info/SOURCES.txt` & `magictk-1.0.1.59/magictk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magictk-1.0.1.58/setup.py` & `magictk-1.0.1.59/setup.py`

 * *Files identical despite different names*

