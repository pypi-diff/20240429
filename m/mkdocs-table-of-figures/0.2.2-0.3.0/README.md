# Comparing `tmp/mkdocs-table-of-figures-0.2.2.tar.gz` & `tmp/mkdocs-table-of-figures-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.2.2.tar", last modified: Tue Apr 23 13:14:14 2024, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.3.0.tar", last modified: Mon Apr 29 08:20:37 2024, max compression
```

## Comparing `mkdocs-table-of-figures-0.2.2.tar` & `mkdocs-table-of-figures-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 13:14:14.898038 mkdocs-table-of-figures-0.2.2/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5928 2024-04-23 13:14:14.892710 mkdocs-table-of-figures-0.2.2/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1742 2024-04-23 13:06:41.000000 mkdocs-table-of-figures-0.2.2/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/license
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 13:14:14.801363 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)    11367 2024-04-23 13:03:08.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 13:14:14.877189 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5928 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-23 13:14:14.000000 mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5389 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-23 13:14:14.899039 mkdocs-table-of-figures-0.2.2/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.2.2/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:20:37.299451 mkdocs-table-of-figures-0.3.0/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.0/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     7295 2024-04-29 08:20:37.297451 mkdocs-table-of-figures-0.3.0/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     2023 2024-04-29 07:54:58.000000 mkdocs-table-of-figures-0.3.0/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.0/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:20:37.207121 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-23 06:07:49.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)    14143 2024-04-29 08:05:41.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:20:37.282668 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     7295 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-29 08:20:36.000000 mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6774 2024-04-29 08:04:51.000000 mkdocs-table-of-figures-0.3.0/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-29 08:20:37.300452 mkdocs-table-of-figures-0.3.0/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-29 07:55:08.000000 mkdocs-table-of-figures-0.3.0/setup.py
```

### Comparing `mkdocs-table-of-figures-0.2.2/PKG-INFO` & `mkdocs-table-of-figures-0.3.0/readme.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,156 +1,154 @@
-Metadata-Version: 2.1
-Name: mkdocs-table-of-figures
-Version: 0.2.2
-Summary: A MkDocs plugin listing all figures to create a table of figures page
-Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
-Author: Thibaud Briard
-Author-email: thibaud.brrd@eduge.ch
-License: MIT
-Keywords: mkdocs
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# mkdocs-table-of-figures
-
-This is a plugin that creates a `figcaption` with elements `alt` attribute or title and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
-
-## Setup
-
-### Installing using pip:
-
-`pip install mkdocs-table-of-figures`
-
-## Config
-
-You need to activate the plugin in `mkdocs.yml`:
-
-``` yaml
-plugins:
-  - table-of-figures:
-      title_label: "Table of figures of the documentation" # Optional --> Default : Table of Figures
-      figure_label: "Figure N°" # Optional --> Default : Figure
-      description_label: "Description of the figures" # Optional --> Default : Description
-
-      temp_dir: "folder_name" # Optional --> Default : temp_figures
-      file: "file_name" # Optional --> Default : figures.md
-
-      follow_nav_structure: true # Optional --> Default : true
-      
-      on_mermaid: true # Optional --> Default : false
-      on_codeblock: true # Optional --> Default : false
-      on_table: true # Optional --> Default : false
-```
-
-As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
-
-- `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
-- `figure_label` - This is the name given to every figure right before the auto-incremented number.
-- `description_label` - This is the label given to the column containing the description of each figure (alt text).
-- `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
-- `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
-- `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
-- `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
-- `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
-- `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
-
-## Usage
-
-The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
-
-There is two way of correctly rendering image stored within the docs:
-
-- Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
-- With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
-
-Concerning external images nothing change.
-
-You can set the `md_in_html` option like so :
-
-``` yaml
-markdown_extensions:
-  - md_in_html
-```
-
-Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
-
-## Support
-
-This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
-
-To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
-
-``` markdown
-    ``` php
-    <?php
-      $var = 42;
-    ?>
-    ```
-    The title of the code block go here
-```
-
-``` markdown
-    ``` mermaid
-    sequenceDiagram
-        participant Alice
-        participant Bob
-        Alice->>John: Hello John, how are you?
-        loop Healthcheck
-            John->>John: Fight against hypochondria
-        end
-        Note right of John: Rational thoughts <br/>prevail!
-        John-->>Alice: Great!
-        John->>Bob: How about you?
-        Bob-->>John: Jolly good!
-    ```
-    The title of the mermaid diagram go here
-```
-
-``` markdown
-    | Table   | Right | Center  | Left  |
-    | ------- | ----: | :-----: | :---- |
-    | A table |  With | Content | in it |
-    The title of the table go here
-```
-
-It will not work if there is a line between the element and the title.
-
-I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
-
-I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
-
-``` css
-figure.figure-mermaid {
-    margin: 0 1em;
-    width: 100%;
-}
-
-figure.figure-codeblock code {
-    text-align: initial;
-}
-```
-
-You can place the stylesheet in your `mkdocs.yml` at extra-css option
-
-``` yml
-extra_css:
-  - fix-mermaid-figure.css
-```
-
-## License
-
-This project is under MIT license. See the `license` file for more details.
-
-## See Also
-
-- [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
-- [MkDocs Website](http://www.mkdocs.org/)
-- [MkDocs-Material Documentation](https://squidfunk.github.io/mkdocs-material/)
-- [Mermaid Documentation](https://mermaid.org/intro/)
-
+# mkdocs-table-of-figures
+
+This is a plugin that creates a `figcaption` with elements `alt` attribute or title and lists all figures in files into a table of figures to be integrated in `Markdown` pages for MkDocs.
+
+## Setup
+
+### Installing using pip:
+
+`pip install mkdocs-table-of-figures`
+
+## Config
+
+You need to activate the plugin in `mkdocs.yml`:
+
+``` yaml
+plugins:
+  - table-of-figures:
+      title_label: "Table of figures of the documentation" # Optional --> Default : Table of Figures
+      figure_label: "Figure N°" # Optional --> Default : Figure
+      description_label: "Description of the figures" # Optional --> Default : Description
+      type_label: "Type of the figure" # Optional --> Default : Type
+      section_label: "Section of the figure" # Optional --> Default : Section
+
+      temp_dir: "folder_name" # Optional --> Default : temp_figures
+      file: "file_name" # Optional --> Default : figures.md
+
+      follow_nav_structure: true # Optional --> Default : true
+      
+      on_mermaid: true # Optional --> Default : false
+      on_codeblock: true # Optional --> Default : false
+      on_table: true # Optional --> Default : false
+
+      show_type: true # Optional --> Default : false
+      show_section: true # Optional --> Default : false
+
+      image_type_name: Image Figure # Optional --> Default : Image
+      mermaid_type_name: Mermaid Figure # Optional --> Default : Mermaid
+      codeblock_type_name: Codeblock Figure # Optional --> Default : Codeblock
+      table_type_name: Table Figure # Optional --> Default : Table
+```
+
+As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
+
+- `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
+- `figure_label` - This is the name given to every figure right before the auto-incremented number.
+- `description_label` - This is the label given to the column containing the description of each figure (alt text).
+- `type_label` - This is the label given to the cloumn containing the type of each figure (image, mermaid, codeblock, table).
+- `section_label` - This is the label given to the cloumn containing the section of each figure (the location relative to headings and pages navigation).
+- `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
+- `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
+- `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
+- `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
+- `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
+- `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
+- `show_type` - To enable the column showing info about the type of each figure (image, mermaid, codeblock, table).
+- `show_section` - To enable the column showing info about the section of each figure (the location relative to headings and pages navigation)
+- `image_type_name` - The label shown for each figure of type image
+- `mermaid_type_name` - The label shown for each figure of type mermaid
+- `codeblock_type_name` - The label shown for each figure of type codeblock
+- `table_type_name` - The label shown for each figure of type table
+
+## Usage
+
+The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
+
+There is two way of correctly rendering image stored within the docs:
+
+- Using url from base: this mean that you give the full path from the docs directory starting with `/` like this `/path/to/image/from/docs/image.png`
+- With the help of `md_in_html`: there is a `Markdown` extension that you can set in `mkdocs.yml` that allow the plugin to place `Markdown` in `HTML` which allow this plugin to let `MkDocs` set relative link in src attribute properly during `HTML` rendering
+
+Concerning external images nothing change.
+
+You can set the `md_in_html` option like so :
+
+``` yaml
+markdown_extensions:
+  - md_in_html
+```
+
+Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it has been set correctly in the config file.
+
+## Support
+
+This plugin currently supports markdown images, `mermaid` diagrams, code blocks and table.
+
+To make a `mermaid` diagram, code block or table detectable by this plugin, you need to give it a title at the line just below it like this:
+
+``` markdown
+    ``` php
+    <?php
+      $var = 42;
+    ?>
+    ```
+    The title of the code block go here
+```
+
+``` markdown
+    ``` mermaid
+    sequenceDiagram
+        participant Alice
+        participant Bob
+        Alice->>John: Hello John, how are you?
+        loop Healthcheck
+            John->>John: Fight against hypochondria
+        end
+        Note right of John: Rational thoughts <br/>prevail!
+        John-->>Alice: Great!
+        John->>Bob: How about you?
+        Bob-->>John: Jolly good!
+    ```
+    The title of the mermaid diagram go here
+```
+
+``` markdown
+    | Table   | Right | Center  | Left  |
+    | ------- | ----: | :-----: | :---- |
+    | A table |  With | Content | in it |
+    The title of the table go here
+```
+
+It will not work if there is a line between the element and the title.
+
+I highly recommend using `mkdocs-material` to use `mermaid` diagrams. For more info about `mermaid` diagrams, I invite you to check `mkdocs-material` and `mermaid`'s official documentation.
+
+I also recommend to add this stylesheet to prevent mermaid size from being reduced or code blocks from having code centered by mkdocs-material.
+
+``` css
+figure.figure-mermaid {
+    margin: 0 1em;
+    width: 100%;
+}
+
+figure.figure-codeblock code {
+    text-align: initial;
+}
+```
+
+You can place the stylesheet in your `mkdocs.yml` at extra-css option
+
+``` yml
+extra_css:
+  - fix-mermaid-figure.css
+```
+
+## License
+
+This project is under MIT license. See the `license` file for more details.
+
+## See Also
+
+- [GitLab Repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-table-of-figures/)
+- [MkDocs Website](http://www.mkdocs.org/)
+- [MkDocs-Material Documentation](https://squidfunk.github.io/mkdocs-material/)
+- [Mermaid Documentation](https://mermaid.org/intro/)
```

### Comparing `mkdocs-table-of-figures-0.2.2/changelog.md` & `mkdocs-table-of-figures-0.3.0/changelog.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.3.0] - 2024-04-29
+
+### Added
+
+- table column containing info abtout the type of figure
+- table column containing info abtout the section where the figure is located
+
+## [0.2.3] - 2024-04-28
+
+### Fixed
+
+- encoding error on file not part of the mkdocs navigation
+
 ## [0.2.2] - 2024-04-23
 
 ### Fixed
 
 - removed the gap in the indexing jump for navigation order created by ignored elements (elements without alt text or caption)
 
 ## [0.2.1] - 2024-04-19
```

### Comparing `mkdocs-table-of-figures-0.2.2/license` & `mkdocs-table-of-figures-0.3.0/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.3.0/mkdocs_table_of_figures/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,18 +18,26 @@
 # The plugin config options
 class TableOfFiguresConfig(base_config):
     temp_dir = c.Type(str, default='temp_figures')
     file = c.Type(str, default='figures.md')
     title_label = c.Type(str, default='Table of Figures')
     figure_label = c.Type(str, default='Figure')
     description_label = c.Type(str, default='Description')
+    type_label = c.Type(str, default='Type')
+    section_label = c.Type(str, default='Section')
     follow_nav_structure = c.Type(bool, default=True)
     on_mermaid = c.Type(bool, default=False)
     on_codeblock = c.Type(bool, default=False)
     on_table = c.Type(bool, default=False)
+    show_type = c.Type(bool, default=False)
+    image_type_name = c.Type(str, default='Image')
+    mermaid_type_name = c.Type(str, default='Mermaid')
+    codeblock_type_name = c.Type(str, default='Codeblock')
+    table_type_name = c.Type(str, default='Table')
+    show_section = c.Type(bool, default=False)
 
 # The plugin itself
 class TableOfFigures(base_plugin[TableOfFiguresConfig]):
     def __init__(self):
         self._logger = logging.getLogger('mkdocs.table-of-figures')
         self._logger.setLevel(logging.INFO)
 
@@ -85,15 +93,15 @@
         
         for index, nav_item in enumerate(nav_structure):
             addon = 0
             if nav_item.is_page:
                 if nav_item == page:
                     found = True
                 elif os.path.exists(os.path.join(self.docs_dir, nav_item.file.src_uri)):
-                    with open(os.path.join(self.docs_dir, nav_item.file.src_uri), 'r') as file:
+                    with open(os.path.join(self.docs_dir, nav_item.file.src_uri), 'r', errors='ignore') as file:
                         markdown = file.read()
 
                     pattern_img = r'!\[([^\]]+?)\]\((.+?)\)'
                     pattern_mermaid = r'^(``` ?(mermaid)\r?\n(.*?)```)$\r?\n^([^\n]+?)$'
                     pattern_codeblock = r'^(``` ?([^\r\n]*)\r?\n(.*?)```)$\r?\n^([^\n]+?)$'
                     pattern_table = r'^((?:\|[^|\r\n]*)+\|\r?\n(?:\|[-: ]*)+\|(?:\r?\n(?:\|[^|\r\n]*)+\|)*)\r?\n^([^|\n]+?)$'
                     
@@ -112,19 +120,19 @@
                 break
         return found, counter
 
     def on_page_markdown(self, markdown, page, config, files):
         if self.listening:
             if self.page == page.file:
                 self._logger.info(f'Populating table of figure file {self.config.file} with {len(self.figures)} figure{"s" if self.counter else ""} ')
-                markdown += f'| {self.config.figure_label} | {self.config.description_label} |\n'
-                markdown += f'| -------------------------- | ------------------------------- |\n'
+                markdown += f'| {self.config.figure_label} |{" " + self.config.type_label + " |" if self.config.show_type else ""} {self.config.description_label} |{" " + self.config.section_label + " |" if self.config.show_section else ""}\n'
+                markdown += f'| -------------------------- |{" :-------------------------------: |" if self.config.show_type else ""} ------------------------------- |{" ------------------------------- |" if self.config.show_section else ""}\n'
                 figures = sorted(self.figures, key=lambda figure: figure["number"])
                 for figure in figures:
-                    markdown += f'| [{self.config.figure_label} {figure["number"]}]({figure["link"]}) | {figure["description"]} |\n'
+                    markdown += f'| [{self.config.figure_label} {figure["number"]}]({figure["link"]}) |{" **" + figure["type"] + "** |" if self.config.show_type else ""} {figure["description"]} |{" `" + figure["section"]  + "` |" if self.config.show_section else ""}\n'
                 
                 self.listening = False
             else:
                 if self.config.follow_nav_structure and self.nav_structure:
                     found, counter = self.count_previous_figures(page, self.nav_structure)
                     if found:
                         self.counter = counter + 1
@@ -143,30 +151,56 @@
                     matches.extend(re.finditer(pattern_table, markdown, flags= re.MULTILINE | re.DOTALL)) if self.config.on_table else None
                     matches = sorted(matches, key=lambda x: x.start())
 
                     position_offset = 0
                     for match in matches:
                         checkpoint = markdown
 
+
                         try:
+                            # Find section
+                            section = ''
+                            header_level = 7
+                            lines = markdown[:match.start() + position_offset].split('\n')
+                            lines.reverse()
+                            for line in lines:
+                                if line.startswith('#') and (len(line) - len(line.lstrip('#'))) < header_level:
+                                    header_level = len(line) - len(line.lstrip('#'))
+                                    header_title = line.lstrip('#').strip()
+                                    if header_title != page.title or header_level > 1:
+                                        if section != '':
+                                            section = header_title + ' > ' +  section
+                                        else:
+                                            section = header_title
+                                    else:
+                                        header_level = 0
+                                    if header_level <= 1:
+                                        break
+                            current_section = page
+                            if current_section.parent is None:
+                                section = config.site_name + ' > ' + ((current_section.title + ' > ') if header_level != 1 else '') + section
+                            while current_section.parent is not None:
+                                current_section = current_section.parent
+                                section = current_section.title + ' > ' +  section
+                            # Generate link
                             link = f'{self.file_relative_path}{page.file.src_uri}#figure-{self.counter}'
                             replacement = match.group(0)
                             if match.re.pattern == pattern_img and match.group(1):
-                                self.figures.append({"number": self.counter, "description": match.group(1), "link": link})
+                                self.figures.append({"number": self.counter, "description": match.group(1), "link": link, "type": self.config.image_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  <img src="{config.site_url + match.group(2) if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                                 if self.keep_md_format:
                                     replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n![{match.group(1)}]({match.group(2)})\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                             elif (match.re.pattern == pattern_mermaid and match.group(4)) or (self.config.on_mermaid and match.re.pattern == pattern_codeblock and match.group(2) == 'mermaid' and match.group(4)):
-                                self.figures.append({"number": self.counter, "description": match.group(4), "link": link})
+                                self.figures.append({"number": self.counter, "description": match.group(4), "link": link, "type": self.config.mermaid_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-mermaid" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_codeblock and match.group(2) != 'mermaid' and match.group(4):
-                                self.figures.append({"number": self.counter, "description": match.group(4), "link": link})
+                                self.figures.append({"number": self.counter, "description": match.group(4), "link": link, "type": self.config.codeblock_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-codeblock" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(4)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_table and match.group(2):
-                                self.figures.append({"number": self.counter, "description": match.group(2), "link": link})
+                                self.figures.append({"number": self.counter, "description": match.group(2), "link": link, "type": self.config.table_type_name, "section": section})
                                 replacement = f'<figure id="figure-{self.counter}" class="figure-table" markdown>\n{match.group(1)}\n<figcaption>{self.config.figure_label} {self.counter} — {match.group(2)}</figcaption>\n</figure>'
                             
                             if replacement == match.group(0):
                                 self._logger.debug(f'Ignoring image/diagram at {self.file_relative_path}{page.file.src_uri}')
                             else:
                                 self._logger.debug(f'Formating image/diagram as figure at {self.file_relative_path}{page.file.src_uri}')
                                 self.counter += 1
```

### Comparing `mkdocs-table-of-figures-0.2.2/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.2.2
+Version: 0.3.0
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Keywords: mkdocs
 Platform: UNKNOWN
@@ -33,36 +33,54 @@
 
 ``` yaml
 plugins:
   - table-of-figures:
       title_label: "Table of figures of the documentation" # Optional --> Default : Table of Figures
       figure_label: "Figure N°" # Optional --> Default : Figure
       description_label: "Description of the figures" # Optional --> Default : Description
+      type_label: "Type of the figure" # Optional --> Default : Type
+      section_label: "Section of the figure" # Optional --> Default : Section
 
       temp_dir: "folder_name" # Optional --> Default : temp_figures
       file: "file_name" # Optional --> Default : figures.md
 
       follow_nav_structure: true # Optional --> Default : true
       
       on_mermaid: true # Optional --> Default : false
       on_codeblock: true # Optional --> Default : false
       on_table: true # Optional --> Default : false
+
+      show_type: true # Optional --> Default : false
+      show_section: true # Optional --> Default : false
+
+      image_type_name: Image Figure # Optional --> Default : Image
+      mermaid_type_name: Mermaid Figure # Optional --> Default : Mermaid
+      codeblock_type_name: Codeblock Figure # Optional --> Default : Codeblock
+      table_type_name: Table Figure # Optional --> Default : Table
 ```
 
 As you can see, every option is optional, but if you want to generate a table of figures in another language than English, you will need to set up label options.
 
 - `title_label` - This is the title (heading 1) given to the page that will contain the table of figures.
 - `figure_label` - This is the name given to every figure right before the auto-incremented number.
 - `description_label` - This is the label given to the column containing the description of each figure (alt text).
+- `type_label` - This is the label given to the cloumn containing the type of each figure (image, mermaid, codeblock, table).
+- `section_label` - This is the label given to the cloumn containing the section of each figure (the location relative to headings and pages navigation).
 - `temp_dir` - The temporary directory used to store the table of figures `Markdown` file before rendering to HTML. Only set this option if you already have a `temp_figures` folder in the root directory (same as `mkdocs.yml`), which you should not normally have.
 - `file` - The name of the `Markdown` file containing the table of figures. Only set this option if you already have a `figures.md` file in the `docs` directory.
 - `follow_nav_structure` - To order the figures in function of the navigation instead of alphabetical files order.
 - `on_mermaid` - To enable `mermaid` diagrams support, need to use of `md_in_html` `Markdown` extension.
 - `on_codeblock` - To enable code blocks support, need to use of `md_in_html` `Markdown` extension.
 - `on_table` - To enable tables support, need to use of `md_in_html` `Markdown` extension.
+- `show_type` - To enable the column showing info about the type of each figure (image, mermaid, codeblock, table).
+- `show_section` - To enable the column showing info about the section of each figure (the location relative to headings and pages navigation)
+- `image_type_name` - The label shown for each figure of type image
+- `mermaid_type_name` - The label shown for each figure of type mermaid
+- `codeblock_type_name` - The label shown for each figure of type codeblock
+- `table_type_name` - The label shown for each figure of type table
 
 ## Usage
 
 The plugin will only look for `Markdown` image composed of alt text. If you don't set any alt text for the `Markdown` image it will be ignored.
 
 There is two way of correctly rendering image stored within the docs:
```

### Comparing `mkdocs-table-of-figures-0.2.2/setup.py` & `mkdocs-table-of-figures-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.2.2',
+    version='0.3.0',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

