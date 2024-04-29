# Comparing `tmp/btex-0.2.4.tar.gz` & `tmp/btex-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btex-0.2.4.tar", max compression
+gzip compressed data, was "btex-0.2.5.tar", max compression
```

## Comparing `btex-0.2.4.tar` & `btex-0.2.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    19486 2024-02-22 14:16:41.939819 btex-0.2.4/btex/__init__.py
--rw-r--r--   0        0        0      362 2024-02-22 14:16:31.637231 btex-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       54 2024-02-14 17:00:31.123256 btex-0.2.4/README.md
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 btex-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    21987 2024-04-29 17:12:45.552196 btex-0.2.5/btex/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-29 17:14:18.595562 btex-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-02-14 17:00:31.123256 btex-0.2.5/README.md
+-rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 btex-0.2.5/PKG-INFO
```

### Comparing `btex-0.2.4/btex/__init__.py` & `btex-0.2.5/btex/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,72 @@
-from watchdog.observers.polling import PollingObserver as Observer
+import argparse
+import os
+import re
+import time
+from pathlib import Path
+
 from watchdog.events import LoggingEventHandler, FileSystemEvent
-import re, argparse, time, os
+from watchdog.observers.polling import PollingObserver as Observer
+
 
-def eval_main_scope(c, n, b, format) -> tuple[bool, list[bool, bool, bool, str], str]:
-    if format[0]:
-        if format[3] == '*':
-            if format[1]:
+class CustomComponent():
+    def __init__(
+            self,
+            name: str,
+            params: list[str],
+            body: str
+        ) -> None:
+        self.name = name
+        self.params = params
+        self.body = body
+
+    def call(self, params: dict[str, str]):
+        b = self.body
+        for param, value in params.items():
+            if param not in self.params:
+                print(f"Error in component {self.name}: parameter {param} isn't valid")
+                exit(1)
+            b = b.replace(f"@param {param}", value)
+        for p in self.params:
+            b = b.replace(f"@param {p}", "")
+        return exec_scope(resolve_scope(f"{{{b}}}"))
+
+
+def eval_main_scope(c, b, fformat: list) -> tuple[bool, list, str]:
+    if fformat[0]:
+        if fformat[3] == '*':
+            if fformat[1]:
                 if c == "*":
-                    return True, [format[0], False, True, format[3]], "bf{"
+                    return True, [fformat[0], False, True, fformat[3]], "bf{"
                 else:
-                    return True, [format[0], False, format[2], format[3]], "it{" + c
+                    return True, [fformat[0], False, fformat[2], fformat[3]], f"it{{{c}"
             else:
                 if c == "*":
-                    if format[2]:
+                    if fformat[2]:
                         return True, [True, False, False, '*'], ""
                     else:
                         return True, [False, False, False, ' '], "}"
                 else:
-                    return True, [format[0], False, format[2], format[3]], c
-        elif format[3] == "_":
+                    return True, [fformat[0], False, fformat[2], fformat[3]], c
+        elif fformat[3] == "_":
             if c == "_":
-                if format[2]:
+                if fformat[2]:
                     return True, [True, False, False, '_'], ""
                 else:
                     return True, [False, False, False, ' '], "}"
             else:
-                return True, [format[0], False, format[2], format[3]], c
+                return True, [fformat[0], False, fformat[2], fformat[3]], c
     if c == '*' and b != "\\":
         return True, [True, True, False, '*'], "\\text"
     elif c == '_' and b != "\\":
         return True, [True, False, False, '_'], "\\underline{"
     return False, [False, False, False, ' '], ""
 
-vars = {
+
+VARS = {
     "textwidth": "\\textwidth",
     "infinity": "\\infty",
     "dot": "\\cdot",
     "percent": "\\%",
     "fs": " ",
     "fn": "\\\\",
     "perp": "\\perp",
@@ -45,330 +75,368 @@
     "Up": "\\Uparrow",
     "up": "\\Uparrow",
     "Down": "\\Downarrow",
     "down": "\\downarrow",
     "Left": "\\Leftarrow",
     "left": "\\leftarrow",
     "Right": "\\Rightarrow",
-    "right": "\\rightarrow"
+    "right": "\\rightarrow",
+    # relation operators
+    #
+    "nless": "\\nless",
+    "leq": "\\leq",
+    "leqslant": "\\leqslant",
+    "nleq": "\\nleq",
+    "nleqslant": "\\nleqslant",
+    #
+    "ngtr": "\\ngtr",
+    "geq": "\\geq",
+    "geqslant": "\\geqslant",
+    "ngeq": "\\ngeq",
+    "ngeqslant": "\\ngeqslant",
+    #
+    "doteq": "\\doteq",
+    "equiv": "\\equiv",
+    "approx": "\\approx",
+    "cong": "\\cong",
+    "simeq": "\\simeq",
+    "sim": "\\sim",
+    "propto": "\\propto",
+    "neq": "\\neq"
 }
 
-def resolve_scope(scope: str, isMath: bool = False):
+main_path = ""
+imports_to_watch = []
+customComponents: list[CustomComponent] = {}
+
+
+def resolve_scope(scope: str, is_math: bool = False):
     t = scope.replace("\n", "").replace("\t", "").replace("@", " \\@")
-    if not isMath:
+    if not is_math:
         t = t.replace("}", "}\\")
-    l = []
+    list_scope = []
     statement = ""
     opened = -1
-    format = [False, False, False, ' ']
+    fformat = [False, False, False, ' ']
     for i in range(len(t)):
         c = t[i]
-        n = t[i+1] if i+1 < len(t) else None
-        b = t[i-1] if i-1 >= 0 else None
-        isThisScope = opened == 0
+        n = t[i + 1] if i + 1 < len(t) else None
+        b = t[i - 1] if i - 1 >= 0 else None
+        is_this_scope = opened == 0
 
-        if isThisScope:
+        if is_this_scope:
             if c == '\\' and n == '\\' and b != "}":
                 statement += "\\\\"
                 continue
-            if isMath:
+            if is_math:
                 if c == "*":
                     statement += "\\times"
                     continue
                 if c == "/":
                     statement += "\\div"
                     continue
             else:
-                _continue, f, toadd = eval_main_scope(c, n, b, format)
-                format = f
+                _continue, f, toadd = eval_main_scope(c, b, fformat)
+                fformat = f
                 if toadd == "}":
                     statement = re.sub(r"}\\\\", "}", statement)
                     toeval = re.sub(r".*\\.*{", "", statement)
                     scope = resolve_scope(f"{{{toeval}}}")
-                    s = [exec_line(l)[0] for l in scope]
+                    s = [exec_line(line)[0] for line in scope]
                     prefix = re.findall(r".*\\.*{", statement)
                     statement = prefix[0] + replace_macros("".join(s))
                 statement += toadd
                 if _continue:
                     continue
         if (c == '\\' and n != '\\') and opened <= 0:
             if statement != "":
-                l.append(statement)
+                list_scope.append(statement)
             statement = ""
         elif c == '{':
             if opened != -1:
                 statement += c
             opened += 1
         elif c == '}':
             if opened != 0:
                 statement += c
             opened -= 1
         else:
             if statement == "" and c == ' ':
                 continue
             statement += c
     if statement != "":
-        l.append(statement)
-    return l
+        list_scope.append(statement)
+    return list_scope
+
 
 def replace_macros(line: str):
     t = str(line)
 
     s = re.sub(r"{.*}", "", t)
 
     matches = re.findall(r"\$\$\w*\$\$", s)
 
     for match in matches:
         var = match[2:-2]
-        if var in vars:
-            t = line.replace(match, vars[var])
+        if var in VARS:
+            t = t.replace(match, VARS[var])
 
     return t
 
+
 def eval_statement(line: str):
     t = replace_macros(line)
 
-    statement = [item for item in t.split(" ") if item != ""]
+    statement = [i for i in t.split(" ") if i != ""]
     return statement
 
+
 def exec_scope(scope):
     t = ""
     for s in scope:
         s2, newline = exec_line(s)
         t += s2
         if newline:
             t += "\n"
     return t
 
+
 def documentclass(_, args):
-    l = len(args)
+    length = len(args)
     global docclass
-    if l == 1:
+    if length == 1:
         docclass = f"\\documentclass{{{args[0]}}}"
     else:
         docclass = f"\\documentclass{args[0]}{{{args[1]}}}"
     return "", True
 
+
+def custom_component(_, args):
+    name = args[0]
+    if name[0] == "(":
+        print("Error in component: name can't be null")
+        exit(1)
+    string, params, _ = getparams(args[1:], False)
+    customParams = []
+    for param in params.replace(", ", ",").split(","):
+        if param == "":
+            continue
+        if param in customParams:
+            print(f"Error in component {name}: param with name {param} already exists")
+        customParams.append(param)
+    if name == "":
+        print("Error in component: name can't be null")
+        exit(1)
+    if name in customComponents:
+        print(f"Error in component: {name} already exists")
+        exit(1)
+    customComponents[name] = CustomComponent(name, customParams, "".join(resolve_scope(string)))
+    return "", False
+
+
+def use_custom_component(_, args):
+    name, params, _ = getparams(args, False)
+    p = {}
+    for param in params.replace(", ", ",").split(","):
+        if param == "":
+            continue
+        first, second = param.split("=")
+        p[first] = second
+    if name not in customComponents:
+        print(f"Error: invalid custom component: {name}")
+        exit(1)
+    return customComponents[name].call(p), True
+
+
 def document(_, args):
     scope = resolve_scope(" ".join(args))
     t = exec_scope(scope)
     return f"\\begin{{document}}\n\n{t}\n\\end{{document}}", True
 
+
 def latex(_, args):
     scope = " ".join(args).replace("}\\\\", "}")
     res = re.findall(r"(?<={)(.*)(?=})", scope)
     s = "".join(res).strip()
     return s, True
 
-def enumerate(_, args):
+
+def _enumerate(_, args):
     scope = resolve_scope(" ".join(args))
     t = exec_scope(scope)
     return f"\\begin{{enumerate}}\n{t}\n\\end{{enumerate}}", True
 
-def math(_, args):
-    string = " ".join(args).replace("}\\", "}")
 
+def getparams(args, has_label: bool = True) -> tuple[str, str, str]:
+    string = " ".join(args).replace("}\\", "}")
     match = re.match(r"\([^)]+\)", string)
     params = ""
     if match is not None:
-        params = string[match.start():match.end()][1:-1]
+        params = replace_macros(string[match.start():match.end()][1:-1])
         string = string[match.end():].strip()
 
     label = ""
 
+    if has_label:
+        for param in params.split(","):
+            if param == "":
+                continue
+            first, second = param.split("=")
+            if first == "label":
+                label = f"\\label{{{second}}}"
+    return string, params, label
+
+
+def usemath(args) -> tuple[str, str]:
+    string, params, label = getparams(args)
     for param in params.split(","):
         if param == "":
             continue
         first, second = param.split("=")
         if first == "label":
             label = f"\\label{{{second}}}"
-
     scope = resolve_scope(string, True)
-    tryImport("amsmath")
+    try_import("amsmath")
     t = exec_scope(scope).strip()
-    return f"\\begin{{equation}} {label}\n{t}\\end{{equation}}", True
+    return label, t
 
-def equations(_, args):
-    string = " ".join(args).replace("}\\", "}")
 
-    match = re.match(r"\([^)]+\)", string)
-    params = ""
-    if match is not None:
-        params = string[match.start():match.end()][1:-1]
-        string = string[match.end():].strip()
+def simplemathfunc(args, name) -> tuple[str, str]:
+    string = ' '.join(eval_statement(' '.join(args)))
 
-    label = ""
+    scope = resolve_scope(string.replace("\\", ""))
 
-    for param in params.split(","):
-        if param == "":
-            continue
-        first, second = param.split("=")
-        if first == "label":
-            label = f"\\label{{{second}}}"
+    if len(scope) != 2:
+        print(f"Error in {name}")
+        exit(1)
 
-    scope = resolve_scope(string, True)
-    tryImport("amsmath")
-    t = exec_scope(scope).strip()
+    first, second = scope
+
+    f = exec_scope(resolve_scope(first, True)).strip()
+
+    s = exec_scope(resolve_scope(second, True)).strip()
+
+    return f, s
+
+
+def math(_, args):
+    label, t = usemath(args)
+    return f"\\begin{{equation}} {label}\n{t}\\end{{equation}}", True
 
+
+def equations(_, args):
+    label, t = usemath(args)
     return f"\\begin{{align*}} {label}\n{t}\\end{{align*}}", True
 
+
 def center(_, args):
     scope = resolve_scope(" ".join(args))
     t = exec_scope(scope)
     return f"\\begin{{center}}\n{t}\n\\end{{center}}", True
 
+
 def sqrt(_, args):
     scope = resolve_scope("".join(args), True)
     t = exec_scope(scope)
     return f"\\sqrt{{{t[0:-1]}}}", True
 
+
 def _split(_, args):
-    tryImport("amsmath")
+    try_import("amsmath")
     scope = resolve_scope(" ".join(args), True)
     t = exec_scope(scope)
     return f"\\begin{{split}}\n{t}\\end{{split}}", True
 
+
 def item(_, args):
     scope = resolve_scope(" ".join(args))
     t = exec_scope(scope)
     return f"\\item {t[0:-3]}", True
 
-def binom(name, args):
-    tryImport("amsmath")
-    string = ' '.join(eval_statement(' '.join(args)))
-    
-    scope = resolve_scope(string.replace("\\", ""))
-
-    if len(scope) != 2:
-        print(f"Error in {name}")
-        exit(1)
-
-    first, second = scope
 
-    f = exec_scope(resolve_scope(first, True)).strip()
-
-    s = exec_scope(resolve_scope(second, True)).strip()
-        
+def binom(name, args):
+    try_import("amsmath")
+    f, s = simplemathfunc(args, name)
     return f"\\binom{{{f}}}{{{s}}}", True
 
-def frac(name, args):
-    string = ' '.join(eval_statement(' '.join(args)))
-    
-    scope = resolve_scope(string.replace("\\", ""))
-
-    if len(scope) != 2:
-        print(f"Error in {name}")
-        exit(1)
-
-    first, second = scope
-
-    f = exec_scope(resolve_scope(first, True)).strip()
 
-    s = exec_scope(resolve_scope(second, True)).strip()
-        
+def frac(name, args):
+    f, s = simplemathfunc(args, name)
     return f"\\frac{{{f}}}{{{s}}}", True
 
-def integral(name, args):
-    string = ' '.join(eval_statement(' '.join(args)))
-    
-    scope = resolve_scope(string.replace("\\", ""))
-
-    if len(scope) != 2:
-        print(f"Error in {name}")
-        exit(1)
-
-    first, second = scope
-
-    f = exec_scope(resolve_scope(first, True)).strip()
 
-    s = exec_scope(resolve_scope(second, True)).strip()
-        
+def integral(name, args):
+    f, s = simplemathfunc(args, name)
     return f"\\int_{{{f}}}^{{{s}}}", True
 
-def mathoperator(name, args):
-    string = ' '.join(eval_statement(' '.join(args)))
-    
-    scope = resolve_scope(string.replace("\\", ""))
-
-    if len(scope) != 2:
-        print(f"Error in {name}")
-        exit(1)
 
-    first, second = scope
+def limit(_, args):
+    scope = resolve_scope(" ".join(args))
+    f = exec_scope(scope)
+    return f"\\lim_{{{f}}}", True
 
-    f = exec_scope(resolve_scope(first, True)).strip()
 
-    s = exec_scope(resolve_scope(second, True)).strip()
-        
+def mathoperator(name, args):
+    f, s = simplemathfunc(args, name)
     return f"\\{name}_{{{f}}}^{{{s}}}", True
 
-def section(name, args):
-    string = ' '.join(eval_statement(' '.join(args)))
-    match = re.match(r"\([^)]+\)", string)
-    params = ""
-    if match is not None:
-        params = string[match.start():match.end()][1:-1]
-        string = string[match.end():].strip()
 
-    label = ""
+def section(name, args):
+    string, params, label = getparams(args)
 
     for param in params.split(","):
         if param == "":
             continue
         first, second = param.split("=")
         if first == "label":
             label = f"\\label{{{second}}}"
-    
+
     return f"\\{name}{{{string}}}{label}\n", True
 
+
 def figure(_, args):
-    tryImport("float")
-    string = ' '.join(eval_statement(' '.join(args)))
-    match = re.match(r"\([^)]+\)", string)
-    params = ""
-    if match is not None:
-        params = string[match.start():match.end()][1:-1]
-        string = string[match.end():]
+    try_import("float")
+    string, params, _ = getparams(args, False)
 
     c = exec_scope(resolve_scope(string))
 
     p = ""
     if params != "":
         p = f"[{params}]"
-    
+
     return f"\\begin{{figure}}{p}\n{c}\n\\end{{figure}}", True
 
+
 def subfigure(_, args):
-    tryImport("caption")
-    tryImport("subcaption")
-    string = ' '.join(eval_statement(' '.join(args)))
-    match = re.match(r"\([^)]+\)", string)
-    params = ""
-    if match is not None:
-        params = string[match.start():match.end()][1:-1]
-        string = string[match.end():]
+    try_import("caption")
+    try_import("subcaption")
 
+    string, params, label = getparams(args, False)
     c = exec_scope(resolve_scope(string))
 
-    p = ""
-    if params != "":
-        p = f"[{params}]"
-    
-    return f"\\begin{{subfigure}}{p}\n{c}\n\\end{{subfigure}}", True
+    position = ""
+    width = "1\\textwidth"
+    for param in params.split(","):
+        if params == "":
+            continue
+        if "=" in param:
+            first, second = param.split("=")
+            if first == "width":
+                width = second
+        else:
+            position = f"[{param.strip()}]"
+
+    return f"\\begin{{subfigure}}{position}{{{width}}}\n{c}\n\\end{{subfigure}}", True
+
 
 def wrapfigure(_, args):
-    tryImport("float")
-    tryImport("wrapfig")
-    string = ' '.join(eval_statement(' '.join(args)))
-    match = re.match(r"\([^)]+\)", string)
-    params = ""
-    if match is not None:
-        params = string[match.start():match.end()][1:-1]
-        string = string[match.end():]
+    try_import("float")
+    try_import("wrapfig")
 
+    string, params, label = getparams(args)
     c = exec_scope(resolve_scope(string))
 
     lineheight = ""
     position = "{r}"
     width = "{0.5\\textwidth}"
 
     for p in params.split(","):
@@ -385,29 +453,31 @@
         elif name == "position":
             position = f"{{{value}}}"
         elif name == "width":
             width = f"{{{value}}}"
         else:
             print(f"Invalid parameter for wrapfigure: {name}")
             exit(1)
-    
+
     return f"\\begin{{wrapfigure}}{lineheight}{position}{width}\n{c}\n\\end{{wrapfigure}}", True
 
+
 def href(name, args):
     if len(args) < 2:
         print(f"Error in {name}")
         exit(1)
     first, *second = args
     second = " ".join(second)
-    tryImport("hyperref")
+    try_import("hyperref")
     return f"\\href{{{first}}}{{{second}}}", False
 
+
 def code(_, args):
-    tryImport("xcolor")
-    tryImport("listings")
+    try_import("xcolor")
+    try_import("listings")
     string = ' '.join(eval_statement(''.join(args)))
     match = re.match(r"\([^)]+\)", string)
     params = ""
     if match is not None:
         params = string[match.start():match.end()][1:-1]
         string = string[match.end():]
 
@@ -418,65 +488,88 @@
             continue
         first, second = param.split("=")
         if first == "label":
             second = f"{{{second}}}"
         parsed[first] = second
 
     p = ','.join(f"{key}={val}" for key, val in parsed.items())
-    
+
     return f"\\lstinputlisting[{p}]{{{string}}}", True
 
+
 def _import(_, args):
-    if len(args) != 1:
+    """if len(args) != 1:
         print("How many fucking parameters did you put?")
         exit(1)
-    return f"\\usepackage{{{args[0]}}}", True
+    return f"\\usepackage{{{args[0]}}}", True"""
+    filename = args[0]
+    text = read(f"{main_path}/{filename}.btex")
+    scope = resolve_scope(f"{{{text}}}")
+    for line in scope:
+        statement = [i for i in line.split(" ") if i != ""]
+        if statement[0][0] == "@":
+            ref = statement[0][1:]
+            if ref != "component":
+                continue
+            items[ref](ref, statement[1:])
+    imports_to_watch.append(f"{filename}.btex")
+    return "", False
+
 
 def use(_, args):
-    tryImport("graphicx")
+    try_import("graphicx")
     s = ''.join(["{" + arg + "}" for arg in args])
     return f"\\graphicspath{{{s}}}", True
 
+
 def usegraphics(_, args):
     string = ' '.join(eval_statement(''.join(args)))
     string = replace_macros(string)
     match = re.match(r"\([^)]+\)", string)
     param = ""
     if match is not None:
         param = string[match.start():match.end()][1:-1]
         string = string[match.end():]
 
-    tryImport("graphicx")
+    try_import("graphicx")
 
     return f"\\includegraphics[{param}]{{{string}}}", True
 
+
 def sscript(name: str, args):
     s = ' '.join(args)
     return f"\\text{name}{{{s}}}", True
 
+
 def itself(name, _):
     return f"\\{name}", False
 
+
 def itselfnewline(name, _):
     return f"\\{name}", True
 
+
 def simpleassign(name, args):
     s = ' '.join(args)
     return f"\\{name}{{{s}}}", False
 
+
 def simpleassignnewline(name, args):
     s = ' '.join(args)
     return f"\\{name}{{{s}}}", True
 
+
 # TODO: add tables
 items = {
     "class": documentclass,
     "document": document,
     "latex": latex,
     "math": math,
+    "component": custom_component,
+    "usecomponent": use_custom_component,
     "equations": equations,
     "center": center,
     "figure": figure,
     "subfigure": subfigure,
     "wrapfigure": wrapfigure,
     "paragraph": section,
     "section": section,
@@ -491,26 +584,27 @@
     "frac": frac,
     "tableofcontents": itselfnewline,
     "maketitle": itselfnewline,
     "newpage": itselfnewline,
     "title": simpleassignnewline,
     "author": simpleassignnewline,
     "date": simpleassignnewline,
-    "list": enumerate,
+    "list": _enumerate,
     "item": item,
     "href": href,
     "code": code,
     "ref": simpleassign,
     "caption": simpleassignnewline,
     "centering": itselfnewline,
     "label": simpleassignnewline,
     "superscript": sscript,
     "subscript": sscript,
     "integral": integral,
     "sum": mathoperator,
+    "lim": limit,
     "prod": mathoperator,
     "cup": mathoperator,
     "cap": mathoperator,
     "oint": mathoperator,
     "coprod": mathoperator,
     # Texts
     "vspace": simpleassign,
@@ -524,91 +618,99 @@
     "LARGE": itselfnewline,
     "huge": itselfnewline,
     "Huge": itselfnewline,
     "hline": itselfnewline,
     "hfill": itselfnewline
 }
 
+
 def exec_line(line: str):
-    statement = [item for item in line.split(" ") if item != ""]
-    
+    statement = [i for i in line.split(" ") if i != ""]
+
     if statement[0][0] == "@":
         ref = statement[0][1:]
-        if not ref in items:
+        if ref not in items:
             print(f"Invalid expression: {ref}")
             exit(1)
         return items[ref](ref, statement[1:])
-    
+
     return replace_macros(" ".join(statement)), True
 
+
 docclass = ""
 
 imports = []
 
-def tryImport(module):
+
+def try_import(module):
     if module in imports:
         return
     imports.append(module)
 
+
 def eval_imports():
     final = ""
     for i in imports:
         label = f"\\usepackage{{{i}}}\n"
         if i == "hyperref":
             label += """
-\hypersetup{
+\\hypersetup{
     colorlinks=true,
     linkcolor=blue,
     filecolor=magenta,
     urlcolor=cyan,
     pdftitle={Overleaf Example},
     pdfpagemode=FullScreen,
 }\n
 """
         if i == "listings":
             label += """
-\definecolor{codegreen}{rgb}{0,0.6,0}
-\definecolor{codegray}{rgb}{0.5,0.5,0.5}
-\definecolor{codepurple}{rgb}{0.58,0,0.82}
-\definecolor{backcolour}{rgb}{0.95,0.95,0.92}
-
-\lstdefinestyle{mystyle}{
-    backgroundcolor=\color{backcolour},
-    commentstyle=\color{codegreen},
-    keywordstyle=\color{magenta},
-    numberstyle=\\tiny\color{codegray},
-    stringstyle=\color{codepurple},
+\\definecolor{codegreen}{rgb}{0,0.6,0}
+\\definecolor{codegray}{rgb}{0.5,0.5,0.5}
+\\definecolor{codepurple}{rgb}{0.58,0,0.82}
+\\definecolor{backcolour}{rgb}{0.95,0.95,0.92}
+
+\\lstdefinestyle{mystyle}{
+    backgroundcolor=\\color{backcolour},
+    commentstyle=\\color{codegreen},
+    keywordstyle=\\color{magenta},
+    numberstyle=\\tiny\\color{codegray},
+    stringstyle=\\color{codepurple},
     basicstyle=\\ttfamily\\footnotesize,
     breakatwhitespace=false,
     breaklines=true,
     captionpos=b,
     keepspaces=true,
     numbers=left,
     numbersep=5pt,
     showspaces=false,
     showstringspaces=false,
     showtabs=false,
     tabsize=2
 }
 
-\lstset{style=mystyle}
+\\lstset{style=mystyle}
 \n
 """
         final += label
     return final
 
+
 def read(f: str):
-    global text
+    text: str
 
     with open(f) as f:
         text = f.read()
 
     return text
 
-def compile(text: str, to: str):
+
+def compile_text(text: str, to: str):
+    customComponents.clear()
+    imports_to_watch.clear()
     split = resolve_scope(f"{{{text}}}")
 
     compiled = ""
 
     for i in split:
         s, newline = exec_line(i)
         compiled += s
@@ -616,67 +718,85 @@
             compiled += "\n"
 
     compiled = docclass + "\n" + eval_imports() + compiled
 
     with open(to, "w") as f:
         f.write(compiled)
 
+
 programs = {
-    "pdflatex": lambda include_dir, out_dir: f"pdflatex -file-line-error -interaction=nonstopmode -synctex=1 -output-format=pdf -quiet -include-directory={include_dir} -output-directory={out_dir}"
+    "pdflatex": lambda include_dir, out_dir: f"pdflatex -file-line-error -interaction=nonstopmode -synctex=1 "
+                                             f"-output-format=pdf -quiet -include-directory={include_dir} "
+                                             f"-output-directory={out_dir}"
 }
 
-def buildPdf(_from: str, file: str, program: str):
-    if not program in programs:
+
+def build_pdf(_from: str, file: str, program: str):
+    if program not in programs:
         print(f"Invalid program for building pdf: {program}")
         exit(1)
     include = os.path.abspath(os.path.dirname(_from))
     out = os.path.abspath(os.path.dirname(file))
     cmd = programs[program](include, out)
     os.system(f"{cmd} {file}")
     print("Built pdf")
 
-def doWork(_from: str, to: str, toPdf: bool, program: str):
+
+def do_work(_from: str, to: str, to_pdf: bool, program: str):
+    p = Path(_from)
+    global main_path
+    main_path = p.parent
     f = read(_from)
-    compile(f, to)
-    if toPdf:
-        buildPdf(_from, to, program)
+    compile_text(f, to)
+    if to_pdf:
+        build_pdf(_from, to, program)
+
 
 def cli():
     parser = argparse.ArgumentParser("btex")
-    
-    parser.add_argument("filename", help="An integer will be increased by 1 and printed.", type=str)
+
+    parser.add_argument("filename", help="btex filename", type=str)
     parser.add_argument("--to", help="file name output", default="out.tex", type=str)
     parser.add_argument("--watch", help="Watch file changes", action=argparse.BooleanOptionalAction, default=False)
-    parser.add_argument("--pdf", help="Auto build tex file to pdf", action=argparse.BooleanOptionalAction, default=False)
+    parser.add_argument("--pdf", help="Auto build tex file to pdf", action=argparse.BooleanOptionalAction,
+                        default=False)
     parser.add_argument("--program", help="What pdf building program to use", type=str, default="pdflatex")
     args = parser.parse_args()
-    
+
     filename = args.filename
     to = args.to
-    toPdf = args.pdf
+    to_pdf = args.pdf
     program = args.program
 
-    doWork(filename, to, toPdf, program)
+    do_work(filename, to, to_pdf, program)
 
     if args.watch:
         event_handler = LoggingEventHandler()
+
         def on_modified(event: FileSystemEvent):
-            if not event.src_path.endswith(filename):
+            src = event.src_path
+            is_main = src.endswith(filename)
+            is_other = False
+            for i in imports_to_watch:
+                if src.endswith(i):
+                    is_other = True
+                    break
+            if not is_main and not is_other:
                 return
-            doWork(filename, to, toPdf, program)
-        
+            do_work(filename, to, to_pdf, program)
+
         event_handler.on_modified = on_modified
-    
 
         observer = Observer()
-        observer.schedule(event_handler, ".", recursive=False)
+        observer.schedule(event_handler, ".", recursive=True)
         observer.start()
         print("Started listening to changes")
         try:
             while True:
                 time.sleep(1)
         except KeyboardInterrupt:
             observer.stop()
         observer.join()
 
+
 if __name__ == "__main__":
-    cli()
+    cli()
```

### Comparing `btex-0.2.4/PKG-INFO` & `btex-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btex
-Version: 0.2.4
+Version: 0.2.5
 Summary: A latex's superset
 Author: Tyger375
 Author-email: edoardo.takanen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```
