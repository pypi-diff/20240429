# Comparing `tmp/colorful_logging-0.8.tar.gz` & `tmp/colorful_logging-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful_logging-0.8.tar", last modified: Sun Apr 28 07:43:20 2024, max compression
+gzip compressed data, was "colorful_logging-0.9.tar", last modified: Mon Apr 29 09:56:53 2024, max compression
```

## Comparing `colorful_logging-0.8.tar` & `colorful_logging-0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:43:20.319387 colorful_logging-0.8/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1864 2024-04-28 07:43:20.319387 colorful_logging-0.8/PKG-INFO
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1076 2024-04-28 07:36:59.000000 colorful_logging-0.8/README.md
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:43:20.319387 colorful_logging-0.8/colorful_logging/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       32 2024-04-28 07:42:33.000000 colorful_logging-0.8/colorful_logging/__init__.py
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     5410 2024-04-28 07:23:22.000000 colorful_logging-0.8/colorful_logging/colorful_logging.py
-drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-28 07:43:20.319387 colorful_logging-0.8/colorful_logging.egg-info/
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1864 2024-04-28 07:43:20.000000 colorful_logging-0.8/colorful_logging.egg-info/PKG-INFO
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      244 2024-04-28 07:43:20.000000 colorful_logging-0.8/colorful_logging.egg-info/SOURCES.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-28 07:43:20.000000 colorful_logging-0.8/colorful_logging.egg-info/dependency_links.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       17 2024-04-28 07:43:20.000000 colorful_logging-0.8/colorful_logging.egg-info/top_level.txt
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       38 2024-04-28 07:43:20.319387 colorful_logging-0.8/setup.cfg
--rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1086 2024-04-28 07:42:09.000000 colorful_logging-0.8/setup.py
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-29 09:56:53.839105 colorful_logging-0.9/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     2288 2024-04-29 09:56:53.839105 colorful_logging-0.9/PKG-INFO
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1500 2024-04-29 09:55:59.000000 colorful_logging-0.9/README.md
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-29 09:56:53.839105 colorful_logging-0.9/colorful_logging/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       32 2024-04-28 07:42:33.000000 colorful_logging-0.9/colorful_logging/__init__.py
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     6363 2024-04-29 09:52:05.000000 colorful_logging-0.9/colorful_logging/colorful_logging.py
+drwxrwxr-x   0 zamoosh   (1000) zamoosh   (1000)        0 2024-04-29 09:56:53.839105 colorful_logging-0.9/colorful_logging.egg-info/
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     2288 2024-04-29 09:56:53.000000 colorful_logging-0.9/colorful_logging.egg-info/PKG-INFO
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)      244 2024-04-29 09:56:53.000000 colorful_logging-0.9/colorful_logging.egg-info/SOURCES.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)        1 2024-04-29 09:56:53.000000 colorful_logging-0.9/colorful_logging.egg-info/dependency_links.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       17 2024-04-29 09:56:53.000000 colorful_logging-0.9/colorful_logging.egg-info/top_level.txt
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)       38 2024-04-29 09:56:53.839105 colorful_logging-0.9/setup.cfg
+-rw-rw-r--   0 zamoosh   (1000) zamoosh   (1000)     1086 2024-04-29 08:48:01.000000 colorful_logging-0.9/setup.py
```

### Comparing `colorful_logging-0.8/PKG-INFO` & `colorful_logging-0.9/colorful_logging.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: colorful_logging
-Version: 0.8
+Name: colorful-logging
+Version: 0.9
 Summary: A library to print colorful
 Home-page: https://github.com/zamoosh/colorful_logging
 Author: zamoosh
 Author-email: moyi.pary@gmail.com
 License: MIT
 Keywords: colorful logging,color printing,color output
 Platform: UNKNOWN
@@ -18,37 +18,42 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 
 # This is just a simple library to print colorful using sys.stderr to write.
 
 ```python
-from colorful_logging.colorful_logging import color_print
+from colorful_logging.colorful_logging import color_print, c_print
 
-# color_print(
-# text: str = your text
-# color: str = 'red', 'blue', ...
-# fmt: bool = True or False
-# lvl: str -> it's just a simple naming when using the "fmt=True"
-# )
-
-
-# for example:
-color_print(
-    text='ali is good',
-    color='cyan',
-    fmt=True,
-    lvl='ALI LEVEL'
-)
+# color_print(*values: tuple[Any, ...])
+# c_print(*values: tuple[Any, ...])
+# ['red', 'green', 'yellow', 'blue', 'pink', 'cyan', 'gray', 'black', 'dark red', 'dark green', 'dark yellow', 'dark blue', 'dark pink', 'dark cyan', 'bright black', 'underline']
+
+l = [1, 2, 3]
+
+# === FOR EXAMPLE === #
+
+color_print('ali is good', l, 'cyan')
 # will produce (with colored text): 
-# ALI LEVEL    24-02-06 18:49:15, File "where the color print executed", Line 1, in "the module", msg: ali is good
+# ali is good [1, 2, 3]
+
+
+c_print(l, 'sample text', 'green')
+# will produce (with colored text): 
+# [1, 2, 3] sample text
+```
 
+### If your input color not found, function will print the color name. for example:
 
-# here also you can use it without formatting the line: 
-color_print('ali is good', 'bold')
+```python
+from colorful_logging.colorful_logging import color_print, c_print
+
+color_print('ali is good', 'cyann')
+# will produce
+# ali is good cyann
 ```
 
 ## To get specific color:
 
 ```python
 from colorful_logging.colorful_logging import get_color
 
@@ -67,8 +72,15 @@
 p = Person(name="ali", age=18)
 
 colorized_elem = colorize("pink", p)
 
 print(f"hello {colorized_elem}")
 ```
 
+## Possible colors:
+
+```
+['red', 'green', 'yellow', 'blue', 'pink', 'cyan', 'gray', 'black', 'dark red', 'dark green', 'dark yellow', 'dark blue', 'dark pink', 'dark cyan', 'bright black', 'underline']
+```
+
+
```

### Comparing `colorful_logging-0.8/colorful_logging/colorful_logging.py` & `colorful_logging-0.9/colorful_logging/colorful_logging.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,39 +67,75 @@
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt, datefmt=self.DATE_FORMAT)
         return formatter.format(record)
 
 
-def color_print(text: str, color: str = RESET, fmt: bool = False, lvl: str = "LOG") -> None:
+# def color_print(text: str, color: str = RESET, fmt: bool = False, lvl: str = "LOG") -> None:
+#     """
+#     Possible values for is as follows:
+#     ['red', 'green', 'yellow', 'blue', 'pink', 'cyan', 'gray', 'black', 'dark red', 'dark green', 'dark yellow', 'dark blue', 'dark pink', 'dark cyan', 'bright black']
+#     """
+#     global possible_colors
+#
+#     color = color.lower()
+#     out_text: str = text
+#     if color in possible_colors:
+#         color = possible_colors[color]
+#         out_text = f"{color}{text}"
+#     if fmt:
+#         # has a bug, when we have '%' in string. need to be fixed
+#         out_text = f"{color}"
+#         now = datetime.datetime.now().strftime('%y-%m-%d %H:%M:%S')
+#         frame = currentframe()
+#         line = f'{frame.f_back.f_lineno}'
+#         fn = f'{sys._getframe().f_back.f_code.co_name}'
+#         out_text += f'{lvl}    {now}, File "%s", Line {line}, in "{fn}", msg: {text}'
+#         file = f'{UNDERLINE}{stack()[1].filename.split("/")[-1]}{RESET}{color}'
+#         out_text = out_text % file
+#     out_text += RESET
+#     out_text += "\n"
+#     sys.stderr.write(out_text)
+
+
+def color_print(*values):
+    c_print(*values)
+
+
+def c_print(*values):
     """
+    Just like print in python, you can pass it any object.
+    Note that the last item on values, should be a color_name, otherwise, it will simply print it.
+
+
     Possible values for is as follows:
-    ['red', 'green', 'yellow', 'blue', 'pink', 'cyan', 'gray', 'black', 'dark red', 'dark green', 'dark yellow', 'dark blue', 'dark pink', 'dark cyan', 'bright black']
+    ['red', 'green', 'yellow', 'blue', 'pink', 'cyan', 'gray', 'black', 'dark red', 'dark green', 'dark yellow', 'dark blue', 'dark pink', 'dark cyan', 'bright black', 'underline']
     """
+
     global possible_colors
 
-    color = color.lower()
-    out_text: str = text
+    items = list(values)
+    color = items[-1]
     if color in possible_colors:
         color = possible_colors[color]
-        out_text = f"{color}{text}"
-    if fmt:
-        # has a bug, when we have '%' in string. need to be fixed
-        out_text = f"{color}"
-        now = datetime.datetime.now().strftime('%y-%m-%d %H:%M:%S')
-        frame = currentframe()
-        line = f'{frame.f_back.f_lineno}'
-        fn = f'{sys._getframe().f_back.f_code.co_name}'
-        out_text += f'{lvl}    {now}, File "%s", Line {line}, in "{fn}", msg: {text}'
-        file = f'{UNDERLINE}{stack()[1].filename.split("/")[-1]}{RESET}{color}'
-        out_text = out_text % file
-    out_text += RESET
-    out_text += "\n"
-    sys.stderr.write(out_text)
+        items.pop()
+    else:
+        color = ""
+
+    final_text = ""
+    for i in items:
+        final_text += str(i)
+        final_text += " "
+
+    final_text = final_text[:len(final_text) - 1]
+    final_text = color + final_text + get_color("reset")
+    print(final_text)
+
+    return
 
 
 def get_color(color: str) -> str:
     """
     Get the color from possible colors:
     Possible values for is as follows:
     ['red', 'green', 'yellow', 'blue', 'pink', 'cyan', 'gray', 'black', 'dark red', 'dark green', 'dark yellow', 'dark blue', 'dark pink', 'dark cyan', 'bright black']
```

### Comparing `colorful_logging-0.8/colorful_logging.egg-info/PKG-INFO` & `colorful_logging-0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: colorful-logging
-Version: 0.8
+Name: colorful_logging
+Version: 0.9
 Summary: A library to print colorful
 Home-page: https://github.com/zamoosh/colorful_logging
 Author: zamoosh
 Author-email: moyi.pary@gmail.com
 License: MIT
 Keywords: colorful logging,color printing,color output
 Platform: UNKNOWN
@@ -18,37 +18,42 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 
 # This is just a simple library to print colorful using sys.stderr to write.
 
 ```python
-from colorful_logging.colorful_logging import color_print
+from colorful_logging.colorful_logging import color_print, c_print
 
-# color_print(
-# text: str = your text
-# color: str = 'red', 'blue', ...
-# fmt: bool = True or False
-# lvl: str -> it's just a simple naming when using the "fmt=True"
-# )
-
-
-# for example:
-color_print(
-    text='ali is good',
-    color='cyan',
-    fmt=True,
-    lvl='ALI LEVEL'
-)
+# color_print(*values: tuple[Any, ...])
+# c_print(*values: tuple[Any, ...])
+# ['red', 'green', 'yellow', 'blue', 'pink', 'cyan', 'gray', 'black', 'dark red', 'dark green', 'dark yellow', 'dark blue', 'dark pink', 'dark cyan', 'bright black', 'underline']
+
+l = [1, 2, 3]
+
+# === FOR EXAMPLE === #
+
+color_print('ali is good', l, 'cyan')
 # will produce (with colored text): 
-# ALI LEVEL    24-02-06 18:49:15, File "where the color print executed", Line 1, in "the module", msg: ali is good
+# ali is good [1, 2, 3]
+
+
+c_print(l, 'sample text', 'green')
+# will produce (with colored text): 
+# [1, 2, 3] sample text
+```
 
+### If your input color not found, function will print the color name. for example:
 
-# here also you can use it without formatting the line: 
-color_print('ali is good', 'bold')
+```python
+from colorful_logging.colorful_logging import color_print, c_print
+
+color_print('ali is good', 'cyann')
+# will produce
+# ali is good cyann
 ```
 
 ## To get specific color:
 
 ```python
 from colorful_logging.colorful_logging import get_color
 
@@ -67,8 +72,15 @@
 p = Person(name="ali", age=18)
 
 colorized_elem = colorize("pink", p)
 
 print(f"hello {colorized_elem}")
 ```
 
+## Possible colors:
+
+```
+['red', 'green', 'yellow', 'blue', 'pink', 'cyan', 'gray', 'black', 'dark red', 'dark green', 'dark yellow', 'dark blue', 'dark pink', 'dark cyan', 'bright black', 'underline']
+```
+
+
```

### Comparing `colorful_logging-0.8/setup.py` & `colorful_logging-0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = ""
 with open('README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='colorful_logging',
-    version='0.8',
+    version='0.9',
     packages=['colorful_logging'],
     install_requires=[],
     url='https://github.com/zamoosh/colorful_logging',
     author='zamoosh',
     author_email='moyi.pary@gmail.com',
     description='A library to print colorful',
     long_description_content_type="text/markdown",
```

