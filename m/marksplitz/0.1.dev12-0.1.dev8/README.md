# Comparing `tmp/marksplitz-0.1.dev12.tar.gz` & `tmp/marksplitz-0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marksplitz-0.1.dev12.tar", last modified: Mon Apr 29 17:03:12 2024, max compression
+gzip compressed data, was "marksplitz-0.1.dev8.tar", last modified: Sun Apr 14 15:38:55 2024, max compression
```

## Comparing `marksplitz-0.1.dev12.tar` & `marksplitz-0.1.dev8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-29 17:03:12.785107 marksplitz-0.1.dev12/
--rw-rw-r--   0 bill      (1000) bill      (1000)     1079 2024-02-17 16:02:31.000000 marksplitz-0.1.dev12/LICENSE.txt
--rw-r--r--   0 bill      (1000) bill      (1000)     4480 2024-04-29 17:03:12.785107 marksplitz-0.1.dev12/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)     2971 2024-04-28 03:03:58.000000 marksplitz-0.1.dev12/README.md
--rw-rw-r--   0 bill      (1000) bill      (1000)     1576 2024-04-13 15:30:00.000000 marksplitz-0.1.dev12/pyproject.toml
--rw-rw-r--   0 bill      (1000) bill      (1000)       38 2024-04-29 17:03:12.785107 marksplitz-0.1.dev12/setup.cfg
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-29 17:03:12.781107 marksplitz-0.1.dev12/src/
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-29 17:03:12.781107 marksplitz-0.1.dev12/src/marksplitz/
--rw-rw-r--   0 bill      (1000) bill      (1000)        0 2024-04-02 18:07:46.000000 marksplitz-0.1.dev12/src/marksplitz/__init__.py
--rw-rw-r--   0 bill      (1000) bill      (1000)    18380 2024-04-29 16:59:04.000000 marksplitz-0.1.dev12/src/marksplitz/marksplitz.py
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-29 17:03:12.785107 marksplitz-0.1.dev12/src/marksplitz.egg-info/
--rw-r--r--   0 bill      (1000) bill      (1000)     4480 2024-04-29 17:03:12.000000 marksplitz-0.1.dev12/src/marksplitz.egg-info/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)      347 2024-04-29 17:03:12.000000 marksplitz-0.1.dev12/src/marksplitz.egg-info/SOURCES.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        1 2024-04-29 17:03:12.000000 marksplitz-0.1.dev12/src/marksplitz.egg-info/dependency_links.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       58 2024-04-29 17:03:12.000000 marksplitz-0.1.dev12/src/marksplitz.egg-info/entry_points.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        8 2024-04-29 17:03:12.000000 marksplitz-0.1.dev12/src/marksplitz.egg-info/requires.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       11 2024-04-29 17:03:12.000000 marksplitz-0.1.dev12/src/marksplitz.egg-info/top_level.txt
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-29 17:03:12.785107 marksplitz-0.1.dev12/tests/
--rw-rw-r--   0 bill      (1000) bill      (1000)    10759 2024-04-28 03:13:23.000000 marksplitz-0.1.dev12/tests/test_marksplitz.py
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1079 2024-02-17 16:02:31.000000 marksplitz-0.1.dev8/LICENSE.txt
+-rw-r--r--   0 bill      (1000) bill      (1000)     3887 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)     2379 2024-04-14 14:57:01.000000 marksplitz-0.1.dev8/README.md
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1576 2024-04-13 15:30:00.000000 marksplitz-0.1.dev8/pyproject.toml
+-rw-rw-r--   0 bill      (1000) bill      (1000)       38 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/setup.cfg
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.386491 marksplitz-0.1.dev8/src/
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.386491 marksplitz-0.1.dev8/src/marksplitz/
+-rw-rw-r--   0 bill      (1000) bill      (1000)        0 2024-04-02 18:07:46.000000 marksplitz-0.1.dev8/src/marksplitz/__init__.py
+-rw-rw-r--   0 bill      (1000) bill      (1000)    17592 2024-04-14 15:29:33.000000 marksplitz-0.1.dev8/src/marksplitz/marksplitz.py
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/src/marksplitz.egg-info/
+-rw-r--r--   0 bill      (1000) bill      (1000)     3887 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)      347 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/SOURCES.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        1 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/dependency_links.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)       58 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/entry_points.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        8 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/requires.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)       11 2024-04-14 15:38:55.000000 marksplitz-0.1.dev8/src/marksplitz.egg-info/top_level.txt
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2024-04-14 15:38:55.390491 marksplitz-0.1.dev8/tests/
+-rw-rw-r--   0 bill      (1000) bill      (1000)     9974 2024-04-13 15:34:02.000000 marksplitz-0.1.dev8/tests/test_marksplitz.py
```

### Comparing `marksplitz-0.1.dev12/LICENSE.txt` & `marksplitz-0.1.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `marksplitz-0.1.dev12/PKG-INFO` & `marksplitz-0.1.dev8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marksplitz
-Version: 0.1.dev12
+Version: 0.1.dev8
 Summary: Command-line utility to split a Markdown file into linked static web pages.
 Author-email: Bill Melvin <bill@billmelvin.com>
 License: MIT License
         
         Copyright (c) 2024-present William Melvin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -21,27 +21,14 @@
 
 # marksplitz
 
 Command-line utility to split a Markdown file into linked static web pages.
 
 > Development work in progress.
 
-## Directive Comments
-
-The following HTML comments can be placed in the source Markdown document to alter the generated HTML.
-
-`<!-- title: new-title -->` 
-
-- Replace the default HTML **title** for the page.
-
-`<!-- class: class-1 class-2 -->` 
-
-- Add one or more classes to the `content` div.
-- Use to apply additional styles via a `custom.css` file. 
-
 ## Command-line Usage
 
 ```
 usage: marksplitz [-h] [-o OUTPUT_DIR] [-n OUTPUT_NAME] [-i IMAGES_SUBDIR]
                      [-c CSS_FILE]
                      markdown_file
 
@@ -70,16 +57,14 @@
                         exist, it is created with the default style.
 ```
 
 ## Reference
 
 ### CSS
 
-Customizing the generated HTML output requires using CSS.
-
 - MDN Guide: [Learn to style HTML using CSS](https://developer.mozilMDNla.org/en-US/docs/Learn/CSS)
 - MDN Reference: [CSS: Cascading Style Sheets](https://developer.mozilla.org/en-US/docs/Web/CSS)
   - [Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)
   - [Class selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors)
 
 ### Packages Used
 
@@ -87,10 +72,8 @@
     - [docs](https://mistune.lepture.com/en/latest/)
 
 ### Project Tools
 
 - [uv](https://github.com/astral-sh/uv#readme) - Environment management (in place of `pip`)
 - [Ruff](https://docs.astral.sh/ruff/) - Linter and code formatter
 - [pytest](https://docs.pytest.org/en/stable/) - Testing framework
-- [build](https://build.pypa.io/en/stable/index.html) - Python packaging build frontend
-- [twine](https://twine.readthedocs.io/en/latest/) - Utility for publishing Python packages
 - [Just](https://github.com/casey/just#readme) - Command runner
```

### Comparing `marksplitz-0.1.dev12/pyproject.toml` & `marksplitz-0.1.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `marksplitz-0.1.dev12/src/marksplitz/marksplitz.py` & `marksplitz-0.1.dev8/src/marksplitz/marksplitz.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from datetime import datetime
 from pathlib import Path
 from textwrap import dedent, indent
 from typing import NamedTuple
 
 import mistune
 
-APP_NAME = "marksplitz"
-
-__version__ = "0.1.dev12"
+__version__ = "0.1.dev8"
 
 
 run_dt = datetime.now()
 
 
 class AppOptions(NamedTuple):
     md_path: Path
@@ -29,87 +27,68 @@
 
 
 def html_style() -> str:
     """Return a default style for the HTML output as a string."""
     return dedent(
         """\
         body { font-family: sans-serif; }
-
         h1 {
             color: #004578;
             text-align: center;
         }
-
         h2 {
             color: #002452;
             margin-top: 2rem;
         }
-
         h3 { color: #001541; }
-
         img {
             border: 1px solid #dde;
             border-radius: 6px;
             height: auto;
-            max-width: 80%;
+            width: 80%;
         }
-
         li { margin-top: 0.8rem; }
-
         blockquote {
             border: 1px solid #b0e0e6;
             border-radius: 6px;
             color: darkslategray;
             padding: 0px 4px;
         }
-
         code {
             background-color: #eee;
             padding-left: 0.3rem;
             padding-right: 0.3rem;
             font-family: monospace;
         }
-
-        #container {
+        .container {
             margin: 0.3rem;
             display: flex;
             align-items: center;
             justify-content: center;
             min-height: 600px;
         }
-
-        #content {
+        .content {
             border: 1px solid silver;
-            padding: 2rem 10%;
-            width: 900px;
-            max-width: 90%;
+            padding: 2rem;
+            width: 800px;
         }
-
         .text-center { text-align: center; }
-
         .nav-link {
             padding-top: 2rem;
             width: 3rem;
         }
-
         .nav-link a {
             border: 1px solid silver;
             border-radius: 5px;
             font-size: 20px;
             font-weight: bold;
             margin: 0.5rem;
             padding: 0.5rem;
         }
-
         #nav-prev, #nav-next { visibility: hidden; }
-
-        #container.show-nav #nav-prev { visibility: visible; }
-
-        #container.show-nav #nav-next { visibility: visible; }
-
         a:link, a:visited {
             color: navy;
             text-decoration: none;
         }
         a:hover { text-decoration: underline; }
         """
     )
@@ -129,29 +108,31 @@
 
 def html_head(
     title: str,
     page_num: int,
     prev_page: str,
     css_link: str,
     add_classes: str,
+    add_id: str,
 ) -> str:
     """Return the head section of an HTML file as a string.
 
-    The title is used as the page title. The page number is used to add a
-    class to the 'container' div. If a CSS link is provided, it is
+    The title is used as the page title. The page number is used to set the
+    'id' attribute of the 'container' div. If a CSS link is provided, it is
     included in the head section. If no CSS link is provided, a default style
     is embedded in the HTML output. If additional classes are provided, they
     are added to the 'content' div. If an 'add_id' is provided, it is added
     to the 'content' div.
 
     param title: The title of the page.
     param page_num: The page number.
     param prev_page: The filename of the previous page.
     param css_link: A link to a CSS file.
     param add_classes: Additional classes to add to the content div.
+    param add_id: An id to add to the content div.
     """
     s = dedent(
         f"""\
         <!DOCTYPE html>
         <html lang="en">
         <head>
         <title>{title}</title>
@@ -162,21 +143,23 @@
     if css_link:
         s += f"{css_link}\n"
     else:
         s += f"<style>\n{html_style()}</style>\n"
 
     s += '<link rel="stylesheet" type="text/css" href="custom.css">\n'
 
-    s += f'</head>\n<body>\n<div id="container" class="page-{page_num:03}">\n\n'
+    s += f'</head>\n<body>\n<div id="page-{page_num:03}" class="container">\n\n'
 
     s += nav_link_div("nav-prev", prev_page, "&larr;")
 
-    class_str = f' class="{add_classes}"' if add_classes else ""
+    class_str = f"content {add_classes}" if add_classes else "content"
+
+    id_str = f' id="{add_id}"' if add_id else ""
 
-    s += f'\n<div id="content"{class_str}>\n'
+    s += f'\n<div{id_str} class="{class_str}">\n'
 
     return s
 
 
 def script_keyboard_nav(prev_page: str, next_page: str) -> str:
     """Return a script to navigate using the left and right arrow keys.
 
@@ -186,31 +169,25 @@
     """
     if prev_page:
         case_prev = dedent(
             f"""\
             case "ArrowLeft":
                 window.location.href = "{prev_page}";
                 break;
-            case "PageUp":
-                window.location.href = "{prev_page}";
-                break;
             """
         )
     else:
         case_prev = ""
 
     if next_page:
         case_next = dedent(
             f"""\
             case "ArrowRight":
                 window.location.href = "{next_page}";
                 break;
-            case "PageDown":
-                window.location.href = "{next_page}";
-                break;
             """
         )
     else:
         case_next = ""
 
     s = dedent(
         """\
@@ -238,33 +215,34 @@
     )
     return s
 
 
 def script_nav_show_hide() -> str:
     """Return a script to show and hide navigation elements.
 
-    The script adds a class to the 'container' div when the mouse is moved
-    and removes the class after a delay. The class is used to show or hide
-    the navigation elements.
-
-    If a previous timeout exists, it is cleared before setting a new one.
-    Timeout is in milliseconds.
+    The script shows the navigation buttons when the mouse is moved
+    and hides them after a delay. If a previous timeout exists, it
+    is cleared before setting a new one. Timeout is in milliseconds.
+    The script is returned as a string.
     """
     return dedent(
         """\
         <script type="text/javascript">
-            var containerDiv = document.getElementById('container');
+            var navPrev = document.getElementById('nav-prev');
+            var navNext = document.getElementById('nav-next');
             var timeoutId;
             document.addEventListener('mousemove', function() {
-                containerDiv.classList.add('show-nav');
+                navPrev.style.visibility = 'visible';
+                navNext.style.visibility = 'visible';
                 if (timeoutId) {
                     clearTimeout(timeoutId);
                 }
                 timeoutId = setTimeout(function() {
-                    containerDiv.classList.remove('show-nav');
+                    navPrev.style.visibility = 'hidden';
+                    navNext.style.visibility = 'hidden';
                 }, 2000);
             });
         </script>
         """
     )
 
 
@@ -286,16 +264,16 @@
     return s
 
 
 def write_index(out_path: Path, items: list[tuple[str, str]]) -> None:
     """Write an index file with links to the pages.
 
     The file is named 'index.html' and is written to the output directory.
-    The parameter 'items' is a list of tuples containing the filename,
-    title, and heading level of each page.
+    The parameter 'items' is a list of tuples containing the filename and
+    title of each page.
     """
     index_file = out_path / "index.html"
     print(f"Writing '{index_file}'")
     with index_file.open("w") as f:
         f.write(
             dedent(
                 """\
@@ -307,54 +285,37 @@
                     body { font-family: sans-serif; }
                     li {
                         border: 1px solid #dde;
                         border-radius: 5px;
                         margin: 0.3rem;
                         padding: 0.3rem;
                     }
-                    #container { display: flex; justify-content: center; }
-                    #content { max-width: 900px; }
-                    #foot {
-                        border-top: 1px solid gray;
-                        font-family: monospace;
-                        font-size: small;
-                        margin-top: 3rem;
-                        padding-top: 1rem;
-                    }
+                    .container { display: flex; justify-content: center; }
+                    .content { max-width: 900px; }
                     a:link, a:visited { color: navy; text-decoration: none; }
                     a:hover { text-decoration: underline; }
                   </style>
-                  <link rel="stylesheet" type="text/css" href="custom.css">
                   <base target="_blank">
                 </head>
                 <body>
-                <div id="container">
-                <div id="content">
+                <div class="container">
+                <div class="content">
                 <h1>Index of Pages</h1>
                 <ol>
                 """
             )
         )
 
-        for filename, title, level in items:
-            f.write(
-                f'  <li class="index-lev-{level}"><a href="{filename}">{title}</a>'
-                "</li>\n"
-            )
+        for filename, title in items:
+            f.write(f'  <li><a href="{filename}">{title}</a></li>\n')
 
-        foot_div = (
-            f'<div id="foot">\nCreated by {APP_NAME} '
-            f"v{__version__} at {run_dt.strftime('%Y-%m-%d %H:%M')}\n"
-            "</div>\n"
-        )
         f.write(
             dedent(
-                f"""\
+                """\
                 </ol>
-                {foot_div}
                 </div>
                 </div>
                 </body>
                 </html>
                 """
             )
         )
@@ -480,68 +441,55 @@
             if not src_file.is_file():
                 continue
             dst_file = dst_path / src_file.name
             print(f"Copy '{src_file}'\n  to '{dst_file}'")
             shutil.copy2(src_file, dst_file)
 
 
-def get_page_heading(num: int, text: str) -> tuple[str, int]:
-    """Return the first heading in the text and its heading-level.
+def get_page_title(num: int, text: str) -> str:
+    """Return the first heading in the text as the page title.
 
-    If there is no heading, return a default heading level and title.
+    If there is no heading, return a default title.
     """
-    heading_level = 1
     lines = text.splitlines()
     for line in lines:
         s = line.strip()
         if s.startswith("#"):
-            a = s.split(" ", 1)
-            heading_level = a[0].count("#")
-            return (a[1].strip(), heading_level)
-    return (f"Page {num}", heading_level)
+            return s.split(" ", 1)[1]
+    return f"Page {num}"
 
 
-def extract_title_comments(num: int, text: str) -> tuple[str, str, int]:
+def extract_title_comments(num: int, text: str) -> tuple[str, str]:
     """Extract the title from a comment in the text.
 
     Returns a tuple of the text, with title-comments removed, and the title
     extracted from the comments.
 
     There should only be one title comment in the text. If there is more than
     one, the last one is used.
 
-    If there is no title comment, the first Markdown heading in the text is used
-    as the title.
-
-    The headling level is based on the first Markdown heading in the text.
-
-    Returns a tuple of the text, the title, and the heading level.
+    The text and title are returned as strings.
     """
     title = ""
 
-    # TODO: Should a title-comment also be able to set heading-level?
-    # If so, leading '#' characters could be used same as in Markdown.
-
     # Look for, and remove, a title comment.
     out_lines = []
     lines = text.splitlines(keepends=True)
     for line in lines:
         s = line.strip()
         if s.startswith("<!-- title: "):
             title = s[12:-3].strip()
         else:
             out_lines.append(line)
 
-    heading, heading_level = get_page_heading(num, text)
-
     # If there was no title comment, use the first heading as the title.
     if not title:
-        title = heading
+        title = get_page_title(num, text)
 
-    return "".join(out_lines), title, heading_level
+    return "".join(out_lines), title
 
 
 def extract_class_comments(text: str) -> tuple[str, str]:
     """Extract classes from comments in the text.
 
     Returns a tuple of the text, with class-comments removed, and the
     classes extracted from the comments. If there are multiple classes
@@ -558,14 +506,35 @@
             classes = s[12:-3].strip()
         else:
             out_lines.append(line)
 
     return "".join(out_lines), classes
 
 
+def extract_id_comments(text: str) -> tuple[str, str]:
+    """Extract an id from a comment in the text.
+
+    Returns a tuple of the text, with id-comments removed, and the id
+    extracted from the comments.
+
+    The text and id are returned as strings.
+    """
+    id_str = ""
+    out_lines = []
+    lines = text.splitlines(keepends=True)
+    for line in lines:
+        s = line.strip()
+        if s.startswith("<!-- id: "):
+            id_str = s[9:-3].strip()
+        else:
+            out_lines.append(line)
+
+    return "".join(out_lines), id_str
+
+
 def add_target_blank(html: str) -> str:
     """Add 'target="_blank"' to all external links in the HTML."""
     return html.replace('<a href="http', '<a target="_blank" href="http')
 
 
 def main(arglist=None) -> int:
     """Split a Markdown file into linked HTML pages."""
@@ -599,26 +568,28 @@
             )
         else:
             css_link = ""
 
         index_items = []
 
         for num, text in enumerate(pages, start=1):
-            md, pg_title, heading_level = extract_title_comments(num, text)
+            md, pg_title = extract_title_comments(num, text)
 
             md, add_classes = extract_class_comments(md)
 
+            md, add_id = extract_id_comments(md)
+
             filename, prev_page, next_page = output_filenames(
                 opts.output_name, num, len(pages)
             )
 
-            index_items.append((filename, pg_title, heading_level))
+            index_items.append((filename, pg_title))
 
             html = html_head(
-                f"{num}. {pg_title}", num, prev_page, css_link, add_classes
+                f"{num}. {pg_title}", num, prev_page, css_link, add_classes, add_id
             )
 
             html += mistune.html(md)
 
             html = add_target_blank(html)
 
             html += html_tail(prev_page, next_page)
```

### Comparing `marksplitz-0.1.dev12/src/marksplitz.egg-info/PKG-INFO` & `marksplitz-0.1.dev8/src/marksplitz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marksplitz
-Version: 0.1.dev12
+Version: 0.1.dev8
 Summary: Command-line utility to split a Markdown file into linked static web pages.
 Author-email: Bill Melvin <bill@billmelvin.com>
 License: MIT License
         
         Copyright (c) 2024-present William Melvin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -21,27 +21,14 @@
 
 # marksplitz
 
 Command-line utility to split a Markdown file into linked static web pages.
 
 > Development work in progress.
 
-## Directive Comments
-
-The following HTML comments can be placed in the source Markdown document to alter the generated HTML.
-
-`<!-- title: new-title -->` 
-
-- Replace the default HTML **title** for the page.
-
-`<!-- class: class-1 class-2 -->` 
-
-- Add one or more classes to the `content` div.
-- Use to apply additional styles via a `custom.css` file. 
-
 ## Command-line Usage
 
 ```
 usage: marksplitz [-h] [-o OUTPUT_DIR] [-n OUTPUT_NAME] [-i IMAGES_SUBDIR]
                      [-c CSS_FILE]
                      markdown_file
 
@@ -70,16 +57,14 @@
                         exist, it is created with the default style.
 ```
 
 ## Reference
 
 ### CSS
 
-Customizing the generated HTML output requires using CSS.
-
 - MDN Guide: [Learn to style HTML using CSS](https://developer.mozilMDNla.org/en-US/docs/Learn/CSS)
 - MDN Reference: [CSS: Cascading Style Sheets](https://developer.mozilla.org/en-US/docs/Web/CSS)
   - [Basic concepts of flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout/Basic_concepts_of_flexbox)
   - [Class selectors](https://developer.mozilla.org/en-US/docs/Web/CSS/Class_selectors)
 
 ### Packages Used
 
@@ -87,10 +72,8 @@
     - [docs](https://mistune.lepture.com/en/latest/)
 
 ### Project Tools
 
 - [uv](https://github.com/astral-sh/uv#readme) - Environment management (in place of `pip`)
 - [Ruff](https://docs.astral.sh/ruff/) - Linter and code formatter
 - [pytest](https://docs.pytest.org/en/stable/) - Testing framework
-- [build](https://build.pypa.io/en/stable/index.html) - Python packaging build frontend
-- [twine](https://twine.readthedocs.io/en/latest/) - Utility for publishing Python packages
 - [Just](https://github.com/casey/just#readme) - Command runner
```

### Comparing `marksplitz-0.1.dev12/tests/test_marksplitz.py` & `marksplitz-0.1.dev8/tests/test_marksplitz.py`

 * *Files 11% similar despite different names*

```diff
@@ -286,19 +286,19 @@
     # assert (out_dir / "page-001.html").exists()
     assert (out_dir / "page-002.html").exists()
     assert (out_dir / "page-003.html").exists()
 
     # text1 = (out_dir / "page-001.html").read_text()
 
     text2 = (out_dir / "page-002.html").read_text()
-    assert 'id="content" class="class-1"' in text2
+    assert 'class="content class-1"' in text2
     assert "<!-- class:" not in text2
 
     text3 = (out_dir / "page-003.html").read_text()
-    assert 'id="content" class="class-1 class-2"' in text3
+    assert 'class="content class-1 class-2"' in text3
     assert "<!-- class:" not in text3
 
 
 def test_creates_index_html(tmp_markdown_file):
     md_file = tmp_markdown_file
 
     out_dir = md_file.parent / "Output"
@@ -332,76 +332,29 @@
 
     index_text = index_file.read_text()
     assert '<a href="page-001.html">Test</a>' in index_text
     assert '<a href="page-002.html">Page 2</a>' in index_text
     assert '<a href="page-003.html">This Title</a>' in index_text
 
 
-def test_index_item_levels(tmp_path):
-    md_file = tmp_path / "test.md"
-    md_file.write_text(
-        dedent(
-            """
-            # Test
-
-            ## Section 1
-
-            Section 1 content.
-
-            ---
-
-            ## Section 2
-
-            Section 2 content.
-
-            ---
-
-            ### Section 2.1
-
-            Section 2.1 content.
-
-            ---
-
-            #### Section 2.1.1
-
-            Section 2.1.1 content.
-
-            ---
-
-            ### Section 2.2
-
-            Section 2.2 content.
-
-            ---
-
-            ## Section 3
-
-            Section 3 content.
+def test_id_comments(tmp_markdown_file):
+    md_file = tmp_markdown_file
 
-            """
-        )
-    )
+    md_file.write_text(md_file.read_text() + "\n<!-- id: my-id -->\n")
 
     out_dir = md_file.parent / "Output"
     out_dir.mkdir()
 
     args = [str(md_file), "-o", str(out_dir)]
     marksplitz.main(args)
 
-    index_file = out_dir / "index.html"
-    assert index_file.exists()
+    assert (out_dir / "page-002.html").exists()
+    text2 = (out_dir / "page-002.html").read_text()
+    assert 'div class="content' in text2
+    # Also check that the page id is in the 'container' div.
+    assert 'div id="page-002" class="container' in text2
 
-    index_text = index_file.read_text()
-    assert '<link rel="stylesheet" type="text/css" href="custom.css">' in index_text
-    assert '<li class="index-lev-1"><a href="page-001.html">Test</a>' in index_text
-    assert '<li class="index-lev-2"><a href="page-002.html">Section 2</a>' in index_text
-    assert (
-        '<li class="index-lev-3"><a href="page-003.html">Section 2.1</a>' in index_text
-    )
-    assert (
-        '<li class="index-lev-4"><a href="page-004.html">Section 2.1.1</a>'
-        in index_text
-    )
-    assert (
-        '<li class="index-lev-3"><a href="page-005.html">Section 2.2</a>' in index_text
-    )
-    assert '<li class="index-lev-2"><a href="page-006.html">Section 3</a>' in index_text
+    assert (out_dir / "page-003.html").exists()
+    text3 = (out_dir / "page-003.html").read_text()
+    assert 'div id="my-id" class="content' in text3
+    assert "<!-- id:" not in text3
+    assert 'div id="page-003" class="container' in text3
```

