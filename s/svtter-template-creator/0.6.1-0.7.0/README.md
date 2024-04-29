# Comparing `tmp/svtter_template_creator-0.6.1.tar.gz` & `tmp/svtter_template_creator-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svtter_template_creator-0.6.1.tar", max compression
+gzip compressed data, was "svtter_template_creator-0.7.0.tar", max compression
```

## Comparing `svtter_template_creator-0.6.1.tar` & `svtter_template_creator-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-04-16 08:26:32.251785 svtter_template_creator-0.6.1/LICENSE
--rw-r--r--   0        0        0      579 2024-04-16 08:47:34.010358 svtter_template_creator-0.6.1/README.md
--rw-r--r--   0        0        0     1059 2024-04-26 01:50:24.077126 svtter_template_creator-0.6.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:47:34.010890 svtter_template_creator-0.6.1/src/__init__.py
--rw-r--r--   0        0        0       22 2024-04-16 08:47:34.011171 svtter_template_creator-0.6.1/src/svtter_template_creator/__init__.py
--rw-r--r--   0        0        0     1612 2024-04-26 01:46:50.589328 svtter_template_creator-0.6.1/src/svtter_template_creator/__main__.py
--rw-r--r--   0        0        0     1166 2024-04-26 01:46:50.589723 svtter_template_creator-0.6.1/src/svtter_template_creator/lib.py
--rw-r--r--   0        0        0     1333 2024-04-26 01:46:50.589979 svtter_template_creator-0.6.1/src/svtter_template_creator/repl.py
--rw-r--r--   0        0        0        0 2024-04-16 08:47:34.011838 svtter_template_creator-0.6.1/src/svtter_template_creator/tests/__init__.py
--rw-r--r--   0        0        0      823 2024-04-26 01:46:50.590344 svtter_template_creator-0.6.1/src/svtter_template_creator/utils.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 svtter_template_creator-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-04-29 13:34:16.816864 svtter_template_creator-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1172 2024-04-29 13:40:02.486624 svtter_template_creator-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      612 2024-04-29 13:34:16.817863 svtter_template_creator-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 13:34:16.819878 svtter_template_creator-0.7.0/src/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-29 13:40:02.487163 svtter_template_creator-0.7.0/src/svtter_template_creator/__init__.py
+-rw-r--r--   0        0        0     1690 2024-04-29 13:34:16.820864 svtter_template_creator-0.7.0/src/svtter_template_creator/__main__.py
+-rw-r--r--   0        0        0     1241 2024-04-29 13:38:36.000121 svtter_template_creator-0.7.0/src/svtter_template_creator/lib.py
+-rw-r--r--   0        0        0     1377 2024-04-29 13:34:16.821869 svtter_template_creator-0.7.0/src/svtter_template_creator/repl.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:34:16.821869 svtter_template_creator-0.7.0/src/svtter_template_creator/tests/__init__.py
+-rw-r--r--   0        0        0      854 2024-04-29 13:34:16.822866 svtter_template_creator-0.7.0/src/svtter_template_creator/utils.py
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 svtter_template_creator-0.7.0/PKG-INFO
```

### Comparing `svtter_template_creator-0.6.1/LICENSE` & `svtter_template_creator-0.7.0/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023-2024 svtter
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023-2024 svtter
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `svtter_template_creator-0.6.1/src/svtter_template_creator/lib.py` & `svtter_template_creator-0.7.0/src/svtter_template_creator/lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-import typing as t
-from warnings import warn
-import tomli
-import pathlib
-import os
-
-
-def get_dict():
-    warn("get_dict is deprecated, use read_repo instead")
-
-    prefix = os.getenv("TC_URL", "git@github.com:svtter")
-
-    template_dict = {
-        "django": "{prefix}/cookiecutter-django.git".format(prefix=prefix),
-        "package": "{prefix}/cookiecutter-pypackage.git".format(prefix=prefix),
-        "compose": "{prefix}/cookiecutter-compose.git".format(prefix=prefix),
-    }
-    return template_dict
-
-
-def create(name) -> None:
-    """
-    create template via name
-    """
-    # repo: dict[name, url]
-    template_dict = read_repo()
-
-    template = template_dict.get(name, None)
-    if template is None:
-        raise ValueError(f"template {name} not found")
-    os.system(f"cookiecutter {template}")
-
-
-def get_choice() -> t.List[str]:
-    """get the choice from toml file"""
-    repos = read_repo()
-    return list(repos.keys())
-
-
-def read_repo() -> t.Dict[str, str]:
-    """get the repos from toml file"""
-    c_path = pathlib.Path.home() / ".config" / "tt.toml"
-    with open(c_path, "rb") as fp:
-        config = tomli.load(fp)
-
-    return config["repos"]
+import typing as t
+from warnings import warn
+from cookiecutter.main import cookiecutter
+import tomli
+import pathlib
+import os
+
+
+def get_dict():
+    warn("get_dict is deprecated, use read_repo instead")
+
+    prefix = os.getenv("TC_URL", "git@github.com:svtter")
+
+    template_dict = {
+        "django": "{prefix}/cookiecutter-django.git".format(prefix=prefix),
+        "package": "{prefix}/cookiecutter-pypackage.git".format(prefix=prefix),
+        "compose": "{prefix}/cookiecutter-compose.git".format(prefix=prefix),
+    }
+    return template_dict
+
+
+def create(name) -> None:
+    """
+    create template via name
+    """
+    # repo: dict[name, url]
+    template_dict = read_repo()
+
+    template = template_dict.get(name, None)
+    if template is None:
+        raise ValueError(f"template {name} not found")
+    cookiecutter(template)
+
+
+def get_choice() -> t.List[str]:
+    """get the choice from toml file"""
+    repos = read_repo()
+    return list(repos.keys())
+
+
+def read_repo() -> t.Dict[str, str]:
+    """get the repos from toml file"""
+    c_path = pathlib.Path.home() / ".config" / "tt.toml"
+    with open(c_path, "rb") as fp:
+        config = tomli.load(fp)
+
+    return config["repos"]
```

### Comparing `svtter_template_creator-0.6.1/src/svtter_template_creator/repl.py` & `svtter_template_creator-0.7.0/src/svtter_template_creator/repl.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import sys
-import prompt_toolkit as pt
-import pathlib as p
-from prompt_toolkit import completion as cmp
-from prompt_toolkit import history as hst
-from prompt_toolkit import auto_suggest
-from svtter_template_creator import lib
-
-
-cmd_list = ["help", "create"]
-
-
-class SimpleCompleter(cmp.Completer):
-    def get_completions(self, document, complete_event):
-        word_before_cursor = document.get_word_before_cursor()
-        for command in cmd_list:
-            if command.startswith(word_before_cursor):
-                yield cmp.Completion(command, -len(word_before_cursor))
-
-
-def repl():
-    session = pt.PromptSession(
-        history=hst.FileHistory(str(p.Path.home() / ".config" / "tt" / "history.txt")),
-        completer=SimpleCompleter(),
-        auto_suggest=auto_suggest.AutoSuggestFromHistory(),
-    )
-
-    while True:
-        try:
-            cmd_str = session.prompt("tt> ")
-            if cmd_str.strip() == "exit":
-                break
-            else:
-                cmd, args = cmd_str.split(" ")
-                if cmd not in cmd_list:
-                    print(f"error cmd: {cmd}")
-                else:
-                    lib.create(args)
-        except EOFError:
-            return
-        except KeyboardInterrupt:
-            continue
-        except Exception as e:
-            print(e, file=sys.stderr)
+import sys
+import prompt_toolkit as pt
+import pathlib as p
+from prompt_toolkit import completion as cmp
+from prompt_toolkit import history as hst
+from prompt_toolkit import auto_suggest
+from svtter_template_creator import lib
+
+
+cmd_list = ["help", "create"]
+
+
+class SimpleCompleter(cmp.Completer):
+    def get_completions(self, document, complete_event):
+        word_before_cursor = document.get_word_before_cursor()
+        for command in cmd_list:
+            if command.startswith(word_before_cursor):
+                yield cmp.Completion(command, -len(word_before_cursor))
+
+
+def repl():
+    session = pt.PromptSession(
+        history=hst.FileHistory(str(p.Path.home() / ".config" / "tt" / "history.txt")),
+        completer=SimpleCompleter(),
+        auto_suggest=auto_suggest.AutoSuggestFromHistory(),
+    )
+
+    while True:
+        try:
+            cmd_str = session.prompt("tt> ")
+            if cmd_str.strip() == "exit":
+                break
+            else:
+                cmd, args = cmd_str.split(" ")
+                if cmd not in cmd_list:
+                    print(f"error cmd: {cmd}")
+                else:
+                    lib.create(args)
+        except EOFError:
+            return
+        except KeyboardInterrupt:
+            continue
+        except Exception as e:
+            print(e, file=sys.stderr)
```

### Comparing `svtter_template_creator-0.6.1/src/svtter_template_creator/utils.py` & `svtter_template_creator-0.7.0/src/svtter_template_creator/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import pathlib as p
-import typing as t
-from collections import namedtuple
-
-default = """[repos]
-compose='git@github.com:svtter/cookiecutter-compose.git'
-django='git@github.com:svtter/cookiecutter-django.git'
-package='git@github.com:svtter/cookiecutter-pypackage.git'
-"""
-
-
-def create_config():
-    """
-    create a config folder
-    """
-    p.Path.home().joinpath(".config", "tt").mkdir(parents=True, exist_ok=True)
-    tt_file = p.Path.home().joinpath(".config", "tt.toml")
-
-    if tt_file.exists():
-        return
-    tt_file.write_text(default)
-
-
-Config = namedtuple("Config", ["path", "content"])
-
-
-def get_config() -> Config:
-    p.Path.home().joinpath(".config", "tt").mkdir(parents=True, exist_ok=True)
-    tt_file = p.Path.home().joinpath(".config", "tt.toml")
-
-    return Config(str(tt_file), tt_file.read_text())
+import pathlib as p
+import typing as t
+from collections import namedtuple
+
+default = """[repos]
+compose='git@github.com:svtter/cookiecutter-compose.git'
+django='git@github.com:svtter/cookiecutter-django.git'
+package='git@github.com:svtter/cookiecutter-pypackage.git'
+"""
+
+
+def create_config():
+    """
+    create a config folder
+    """
+    p.Path.home().joinpath(".config", "tt").mkdir(parents=True, exist_ok=True)
+    tt_file = p.Path.home().joinpath(".config", "tt.toml")
+
+    if tt_file.exists():
+        return
+    tt_file.write_text(default)
+
+
+Config = namedtuple("Config", ["path", "content"])
+
+
+def get_config() -> Config:
+    p.Path.home().joinpath(".config", "tt").mkdir(parents=True, exist_ok=True)
+    tt_file = p.Path.home().joinpath(".config", "tt.toml")
+
+    return Config(str(tt_file), tt_file.read_text())
```

### Comparing `svtter_template_creator-0.6.1/PKG-INFO` & `svtter_template_creator-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: svtter_template_creator
-Version: 0.6.1
+Version: 0.7.0
 Summary: 
 Keywords: template,django
 Author: svtter
 Author-email: svtter@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
```

