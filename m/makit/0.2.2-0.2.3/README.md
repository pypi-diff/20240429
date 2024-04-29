# Comparing `tmp/makit-0.2.2.tar.gz` & `tmp/makit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makit-0.2.2.tar", last modified: Thu Apr 25 19:33:42 2024, max compression
+gzip compressed data, was "makit-0.2.3.tar", last modified: Mon Apr 29 11:58:30 2024, max compression
```

## Comparing `makit-0.2.2.tar` & `makit-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-25 19:33:42.535836 makit-0.2.2/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2024-04-23 09:01:38.000000 makit-0.2.2/LICENSE
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       36 2024-04-23 09:05:36.000000 makit-0.2.2/MANIFEST.in
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-25 19:33:42.535836 makit-0.2.2/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      494 2024-04-23 10:54:16.000000 makit-0.2.2/README.md
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-25 19:33:42.535836 makit-0.2.2/makeit/
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       50 2024-04-23 09:07:05.000000 makit-0.2.2/makeit/__init__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       68 2024-04-23 09:07:11.000000 makit-0.2.2/makeit/__main__.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      529 2024-04-25 19:28:17.000000 makit-0.2.2/makeit/main.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1773 2024-04-25 13:17:26.000000 makit-0.2.2/makeit/make.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 09:05:06.000000 makit-0.2.2/makeit/py.typed
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3030 2024-04-25 19:31:47.000000 makit-0.2.2/makeit/tui.py
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2024-04-25 19:32:06.000000 makit-0.2.2/makeit/version.py
-drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-25 19:33:42.535836 makit-0.2.2/makit.egg-info/
--rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-25 19:33:42.000000 makit-0.2.2/makit.egg-info/PKG-INFO
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      362 2024-04-25 19:33:42.000000 makit-0.2.2/makit.egg-info/SOURCES.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2024-04-25 19:33:42.000000 makit-0.2.2/makit.egg-info/dependency_links.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       69 2024-04-25 19:33:42.000000 makit-0.2.2/makit.egg-info/entry_points.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-25 19:33:42.000000 makit-0.2.2/makit.egg-info/requires.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        7 2024-04-25 19:33:42.000000 makit-0.2.2/makit.egg-info/top_level.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      822 2024-04-25 19:32:14.000000 makit-0.2.2/pyproject.toml
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-23 09:02:06.000000 makit-0.2.2/requirements.txt
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-25 19:33:42.535836 makit-0.2.2/setup.cfg
--rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-23 09:04:45.000000 makit-0.2.2/setup.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-29 11:58:30.976463 makit-0.2.3/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     1063 2024-04-23 09:01:38.000000 makit-0.2.3/LICENSE
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       36 2024-04-23 09:05:36.000000 makit-0.2.3/MANIFEST.in
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-29 11:58:30.976463 makit-0.2.3/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      494 2024-04-23 10:54:16.000000 makit-0.2.3/README.md
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-29 11:58:30.972463 makit-0.2.3/makeit/
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       50 2024-04-23 09:07:05.000000 makit-0.2.3/makeit/__init__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       68 2024-04-23 09:07:11.000000 makit-0.2.3/makeit/__main__.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      508 2024-04-29 11:54:51.000000 makit-0.2.3/makeit/main.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     2930 2024-04-29 11:55:32.000000 makit-0.2.3/makeit/make.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-23 09:05:06.000000 makit-0.2.3/makeit/py.typed
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)     3011 2024-04-29 11:55:50.000000 makit-0.2.3/makeit/tui.py
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       22 2024-04-29 11:57:56.000000 makit-0.2.3/makeit/version.py
+drwxrwxr-x   0 ireneusz  (1001) ireneusz  (1001)        0 2024-04-29 11:58:30.976463 makit-0.2.3/makit.egg-info/
+-rw-r--r--   0 ireneusz  (1001) ireneusz  (1001)      994 2024-04-29 11:58:30.000000 makit-0.2.3/makit.egg-info/PKG-INFO
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      362 2024-04-29 11:58:30.000000 makit-0.2.3/makit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        1 2024-04-29 11:58:30.000000 makit-0.2.3/makit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       69 2024-04-29 11:58:30.000000 makit-0.2.3/makit.egg-info/entry_points.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-29 11:58:30.000000 makit-0.2.3/makit.egg-info/requires.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)        7 2024-04-29 11:58:30.000000 makit-0.2.3/makit.egg-info/top_level.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)      822 2024-04-29 11:58:02.000000 makit-0.2.3/pyproject.toml
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       31 2024-04-29 11:41:19.000000 makit-0.2.3/requirements.txt
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-29 11:58:30.976463 makit-0.2.3/setup.cfg
+-rw-rw-r--   0 ireneusz  (1001) ireneusz  (1001)       38 2024-04-23 09:04:45.000000 makit-0.2.3/setup.py
```

### Comparing `makit-0.2.2/LICENSE` & `makit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `makit-0.2.2/PKG-INFO` & `makit-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: makit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Interactive Makefile step picker
 Author-email: igrek51 <igrek51.dev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/igrek51/makeit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nuclear>=2.1.0
-Requires-Dist: textual==0.57.1
+Requires-Dist: textual>=0.58.0
 
 # Makeit
 
 **makeit** is an interactive Makefile runner.
 
 <div align="center">
     <a href="https://github.com/igrek51/makeit">GitHub</a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: makit Version: 0.2.2 Summary: Interactive Makefile
+Metadata-Version: 2.1 Name: makit Version: 0.2.3 Summary: Interactive Makefile
 step picker Author-email: igrek51
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/igrek51/
 makeit Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: nuclear>=2.1.0 Requires-Dist: textual==0.57.1 # Makeit
+LICENSE Requires-Dist: nuclear>=2.1.0 Requires-Dist: textual>=0.58.0 # Makeit
 **makeit** is an interactive Makefile runner.
                                  _G_i_t_H_u_b - _P_y_P_I
 ![](./docs/img/screenshot.png) ## Installation ```shell pip3 install makit ```
 This will install `makeit` executable. ## Usage Run it in the directory of your
 Makefile: ```shell makeit ``` It will show a list of available Makefile steps.
 Pick one and hit Enter to run it with `make`.
```

### Comparing `makit-0.2.2/makeit/tui.py` & `makit-0.2.3/makeit/tui.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,24 +12,25 @@
         self.selected_step: MakeStep | None = None
         self.chosen_step: MakeStep | None = None
         self.post_logs: list[str] = []
 
     def compose(self) -> ComposeResult:
         self.screen.styles.border = ("hidden", 'white')
 
-        header = Label(' Makefile targets:')
+        header = Label(f' {len(self.steps)} Makefile targets:')
         header.styles.width = '100%'
         header.styles.color = 'royalblue'
 
         list_children: list[ListItem] = [ListItem(Label(' ' + step.name)) for step in self.steps]
         listview = ListView(
             *list_children,
             id="steps-list",
         )
         listview.styles.height = max(len(self.steps), 1) + 1
+        listview.styles.max_height = "50vh"
 
         summary_header = Label("", id="summary-header")
         summary_header.styles.color = 'royalblue'
         summary_header.styles.text_style = 'bold'
 
         summary_comment = Label("", id="summary-comment")
         summary_comment.styles.color = 'lightslategray'
@@ -58,23 +59,23 @@
             self.query_one("#summary", Label).update(summary)
 
     def on_list_view_selected(self, event: ListView.Selected):
         self.chosen_step = self._get_selected_step()
         self.exit()
     
     def _get_selected_step(self) -> MakeStep | None:
-        listview: ListView = self.query_one("#steps-list", ListView)
-        selected_index: int = listview.index or 0
+        selected_index: int = self._get_listview().index or 0
         if selected_index < 0 or selected_index >= len(self.steps):
             return None
         return self.steps[selected_index]
 
+    def _get_listview(self) -> ListView:
+        return self.query_one("#steps-list", ListView)
+
     def on_key(self, event: events.Key) -> None:
         # self.post_logs.append(str(event))
         if event.key in {'q', 'escape'}:
             self.exit()
         elif event.key == 'home':
-            listview: ListView = self.query_one("#steps-list", ListView)
-            listview.index = 0
+            self._get_listview().index = 0
         elif event.key == 'end':
-            listview: ListView = self.query_one("#steps-list", ListView)
-            listview.index = len(self.steps) - 1
+            self._get_listview().index = len(self.steps) - 1
```

### Comparing `makit-0.2.2/makit.egg-info/PKG-INFO` & `makit-0.2.3/makit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: makit
-Version: 0.2.2
+Version: 0.2.3
 Summary: Interactive Makefile step picker
 Author-email: igrek51 <igrek51.dev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/igrek51/makeit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nuclear>=2.1.0
-Requires-Dist: textual==0.57.1
+Requires-Dist: textual>=0.58.0
 
 # Makeit
 
 **makeit** is an interactive Makefile runner.
 
 <div align="center">
     <a href="https://github.com/igrek51/makeit">GitHub</a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: makit Version: 0.2.2 Summary: Interactive Makefile
+Metadata-Version: 2.1 Name: makit Version: 0.2.3 Summary: Interactive Makefile
 step picker Author-email: igrek51
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/igrek51/
 makeit Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: nuclear>=2.1.0 Requires-Dist: textual==0.57.1 # Makeit
+LICENSE Requires-Dist: nuclear>=2.1.0 Requires-Dist: textual>=0.58.0 # Makeit
 **makeit** is an interactive Makefile runner.
                                  _G_i_t_H_u_b - _P_y_P_I
 ![](./docs/img/screenshot.png) ## Installation ```shell pip3 install makit ```
 This will install `makeit` executable. ## Usage Run it in the directory of your
 Makefile: ```shell makeit ``` It will show a list of available Makefile steps.
 Pick one and hit Enter to run it with `make`.
```

### Comparing `makit-0.2.2/pyproject.toml` & `makit-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "makit"
-version = "0.2.2"  # also in makeit/version.py
+version = "0.2.3"  # also in makeit/version.py
 description = "Interactive Makefile step picker"
 license = {text = "MIT"}
 authors = [
     { name = "igrek51", email = "igrek51.dev@gmail.com" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

