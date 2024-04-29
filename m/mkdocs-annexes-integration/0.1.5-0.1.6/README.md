# Comparing `tmp/mkdocs-annexes-integration-0.1.5.tar.gz` & `tmp/mkdocs-annexes-integration-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-annexes-integration-0.1.5.tar", last modified: Wed Jun  7 13:16:02 2023, max compression
+gzip compressed data, was "mkdocs-annexes-integration-0.1.6.tar", last modified: Mon Apr 29 14:41:55 2024, max compression
```

## Comparing `mkdocs-annexes-integration-0.1.5.tar` & `mkdocs-annexes-integration-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-07 13:16:02.113484 mkdocs-annexes-integration-0.1.5/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-annexes-integration-0.1.5/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5325 2023-06-07 13:16:02.112484 mkdocs-annexes-integration-0.1.5/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1345 2023-06-07 13:13:31.000000 mkdocs-annexes-integration-0.1.5/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-annexes-integration-0.1.5/license
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-07 13:16:02.045695 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)    11775 2023-06-07 13:09:27.000000 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-07 13:16:02.101875 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5325 2023-06-07 13:16:01.000000 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      441 2023-06-07 13:16:01.000000 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-07 13:16:01.000000 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       93 2023-06-07 13:16:01.000000 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       32 2023-06-07 13:16:01.000000 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       27 2023-06-07 13:16:01.000000 mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     3815 2023-06-07 13:15:55.000000 mkdocs-annexes-integration-0.1.5/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-07 13:16:02.114484 mkdocs-annexes-integration-0.1.5/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1216 2023-06-07 12:35:43.000000 mkdocs-annexes-integration-0.1.5/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 14:40:40.973576 mkdocs-annexes-integration-0.1.6/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.6/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4150 2024-04-29 14:41:55.846781 mkdocs-annexes-integration-0.1.6/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1428 2024-04-29 14:33:40.000000 mkdocs-annexes-integration-0.1.6/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.6/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 14:40:40.865490 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 08:29:27.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8553 2024-04-29 14:36:11.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-29 14:41:55.831885 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4150 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      441 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       93 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       32 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       27 2024-04-29 14:41:55.000000 mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3536 2024-04-29 14:38:48.000000 mkdocs-annexes-integration-0.1.6/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-29 14:41:55.850778 mkdocs-annexes-integration-0.1.6/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1201 2024-04-29 14:37:54.000000 mkdocs-annexes-integration-0.1.6/setup.py
```

### Comparing `mkdocs-annexes-integration-0.1.5/PKG-INFO` & `mkdocs-annexes-integration-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,117 +1,107 @@
 Metadata-Version: 2.1
 Name: mkdocs-annexes-integration
-Version: 0.1.5
-Summary: A MkDocs plugin transforming annexes files into images or code blocks to be integrated in markdown pages
+Version: 0.1.6
+Summary: A MkDocs plugin transforming annexes files into images to be integrated in markdown pages
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
-Description: # mkdocs-annexes-integration
-        
-        This is a plugin that transforms annex files into images or code blocks to be integrated in Markdown pages for MkDocs.
-        
-        ## Setup
-        
-        ### Before installing
-        
-        Before installing this plugin you need to install `poppler-utils` as it is used by `pdf2image` that is required to use this plugin.
-        
-        #### Install on Linux :
-        
-        Note: *It depend on your Linux OS*
-        
-        ``` sh
-        sudo apt-get install poppler-utils
-        ```
-        
-        ``` sh
-        sudo yum install poppler-utils
-        ```
-        
-        #### Install on MacOS :
-        
-        ``` sh
-        brew install poppler
-        ```
-        
-        #### Install on Windows :
-        
-        On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
-        
-        ### Installing using pip:
-        
-        `pip install mkdocs-annexes-integration`
-        
-        ## Config
-        
-        You need to activate the plugin in `mkdocs.yml`:
-        
-        ```yaml
-        plugins:
-          - annexes-integration:
-              annexes: # Required (at least 1)
-                - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
-                - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
-                - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
-                - Title of the code file annex:
-                    src: ../src/path/to/a/code/file.py
-                    dest: dest/path/to/a/code/file.py
-                - Title of the code directory annex:
-                    src: ../src/path/to/a/code/directory
-                    dest: dest/path/to/a/code/directory
-                # others annexes...
-              temp_dir: "folder_name" # Optional --> Default : temp_annexes
-              enabled_if_env: ENABLE_ANNEXES_INTEGRATION # Optional
-        ```
-        
-        As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
-        
-        Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
-        
-        - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file or directory associated to it's title. Each file in a directory will integrated in subsection of the same document with a heading 2 containing the relative path of the file from the given directory.
-        - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
-        - `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
-        
-        ## Usage
-        
-        Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
-        
-        This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
-        
-        ## Support
-        
-        This plugin currently support two type of files :
-        
-        - **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
-        
-        - **Code files**: The plugin will put the content of the code file into a codeblock to be integrated on a page
-        
-        Currently supported code files are :
-         - CSharp (.cs)
-         - CSS (.css)
-         - Dart (.dart)
-         - HTML (.html)
-         - Javascript (.js)
-         - JSON (.json)
-         - PHP (.php)
-         - Python (.py)
-        
-        ## License
-        
-        This project is under MIT license see: `license` file for more detail.
-        
-        ## See Also
-        
-        - [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
-        - [mkdocs website](http://www.mkdocs.org/)
-        - [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
 Keywords: mkdocs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# mkdocs-annexes-integration
+
+This is a plugin that transforms annex files into images to be integrated in Markdown pages for MkDocs.
+
+## Setup
+
+### Before installing
+
+Before installing this plugin you need to install `poppler-utils` as it is used by `pdf2image` that is required to use this plugin.
+
+#### Install on Linux :
+
+Note: *It depend on your Linux OS*
+
+``` sh
+sudo apt-get install poppler-utils
+```
+
+``` sh
+sudo yum install poppler-utils
+```
+
+#### Install on MacOS :
+
+``` sh
+brew install poppler
+```
+
+#### Install on Windows :
+
+On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
+
+### Installing using pip:
+
+`pip install mkdocs-annexes-integration`
+
+## Config
+
+You need to activate the plugin in `mkdocs.yml`:
+
+```yaml
+plugins:
+  - annexes-integration:
+      annexes: # Required (at least 1)
+        - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
+        - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
+        - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
+        - Title of the annex:
+            src: ../src/path/to/an/annex/file1.py
+            dest: dest/path/to/an/annex/file1.py
+        # others annexes...
+      temp_dir: "folder_name" # Optional --> Default : temp_annexes
+      enabled_if_env: ENABLE_PDF_EXPORT # Optional
+```
+
+As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
+
+Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
+
+- `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
+- `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
+- `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
+
+## Usage
+
+Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
+
+This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
+
+It is also strongly recommended to use it with `mkdocs-material` plugin. Using this plugin without `mkdocs-material` may result in unecessary page break between annex title and annex images.
+
+## Support
+
+This plugin currently support PDF files :
+
+- **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
+
+## License
+
+This project is under MIT license see: `license` file for more detail.
+
+## See Also
+
+- [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
+- [mkdocs website](http://www.mkdocs.org/)
+- [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
+- [mkdocs material plugin](https://github.com/squidfunk/mkdocs-material)
+
```

### Comparing `mkdocs-annexes-integration-0.1.5/changelog.md` & `mkdocs-annexes-integration-0.1.6/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
-## [0.1.5] - 2023-06-07
+## [0.1.5] - 2024-04-29
 
-### Added
+### Removed
+
+- Support for code files as it is already supported by `mkdocs-material`
+
+### Fixed
 
-- Support for giving directory instead of each files separatly
+- Size of image to big to be used in `mkdocs-with-pdf`
 
 ## [0.1.4] - 2023-05-17
 
 ### Added
 
 - Support for enabling by environement variable
```

### Comparing `mkdocs-annexes-integration-0.1.5/license` & `mkdocs-annexes-integration-0.1.6/license`

 * *Files identical despite different names*

### Comparing `mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration/plugin.py` & `mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration/plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,95 +60,57 @@
             # Generate markdown files for each annex
             try:
                 for annex in self.config.annexes:
                     title, path = list(annex.items())[0]
                     self._logger.info(f'Integrating annex "{title}"')
                     # Determine source and destination path from path option
                     src, dest = self.get_src_and_dest(path)
+                    # Get extension of file
+                    extension = os.path.splitext(src)[1][1:]
                     # Get absolute path to original file
                     original = os.path.join(config.docs_dir, src)
                     # Get absolute path to generated markdown
                     embedded = f'{os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])}.md'
                     # skip if original file don't exist
                     if os.path.exists(original):
-                        if os.path.isfile(original):
-                            # Get extension of file
-                            extension = os.path.splitext(src)[1][1:]
-                            # Check if file is code file or pdf
-                            if extension in ['cs', 'css', 'dart', 'html', 'js', 'json', 'php', 'py', 'sql']:
-                                # For code files content are put ina codeblock
-                                self._logger.info(f'    With content as code block')
-                                with open(original, 'r') as file:
-                                    content = file.read()
-                                # Create a markdown file that take care of showing source code annex
-                                if not os.path.exists(os.path.dirname(embedded)):
-                                    os.makedirs(os.path.dirname(embedded))
-                                with open(embedded, 'w') as f:
-                                    # write the title and the content to the file
-                                    f.write(f'# {title}\n\n``` {extension}\n{content}\n```\n')
-                            elif extension in ['pdf']:
-                                # For PDF files each page are transformed into images
-                                self._logger.info(f'    With each pages as images')
-                                # Get absolute path for PDF directory
-                                root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
-                                # Get absolute path for PDF images directory
-                                source = os.path.join(root, 'source')
-                                # Create a root folder containing the annex
-                                if not os.path.exists(root):
-                                    os.makedirs(root)
-                                # Save pages as images in the pdf
-                                images = convert_from_path(original)
-                                # Create source folder to save images
-                                if not os.path.exists(source):
-                                    os.mkdir(source)
-                                # Create a markdown file that take care of showing PDF annex
-                                with open(embedded, 'w') as f:
-                                    # Write the title to the file
-                                    f.write(f'# {title}\n\n')
-
-                                    for i in range(len(images)):
-                                        # Add leading zeros to the page number
-                                        filename = f'page_{i + 1:04}.png'
-                                        images[i].save(f'{source}/{filename}', 'PNG')
-                                        files.append(File(os.path.join(os.path.splitext(dest)[0], f'source/{filename}'), src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
-
-                                        # Write the image link to the file
-                                        f.write(f'![Page {i+1}](./{os.path.basename(os.path.splitext(dest)[0])}/source/{filename})\n')
-                            else:
-                                self._logger.warning(f'file {src} extension isn\'t supported (yet) --> skipped')
-                            # Removing originals files from list of mkdocs files if they were in the docs directory originaly
-                            if os.path.isfile(os.path.join(config.docs_dir, dest)):
-                                self._logger.info(f'    Remvoing original annex {src} from processed files list')
-                                files.remove(files.get_file_from_path(src))
-                        elif os.path.isdir(original):
+                        # Check if file is a PDF
+                        if extension in ['pdf']:
+                            # For PDF files each page are transformed into images
+                            self._logger.info(f'    With each pages as images')
+                            # Get absolute path for PDF directory
+                            root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
+                            # Get absolute path for PDF images directory
+                            source = os.path.join(root, 'source')
+                            # Create a root folder containing the annex
+                            if not os.path.exists(root):
+                                os.makedirs(root)
+                            # Save pages as images in the pdf
+                            images = convert_from_path(original, size=(None, 800))
+                            # Create source folder to save images
+                            if not os.path.exists(source):
+                                os.mkdir(source)
+                            # Create a markdown file that take care of showing PDF annex
                             with open(embedded, 'w') as f:
-                                # write the title and the content to the file
+                                # Write the title to the file
                                 f.write(f'# {title}\n\n')
-                            # Iterate trought directory
-                            for original_directory, _, original_files in os.walk(original):
-                                for original_file in original_files:
-                                    rel_file = os.path.join(original_directory[len(original):], original_file)
-                                    original_file = os.path.join(original_directory, original_file)
-                                    self._logger.info(f'    For file {rel_file}')
 
-                                    # Get extension of file
-                                    extension = os.path.splitext(original_file)[1][1:]
-                                    if extension in ['cs', 'css', 'dart', 'html', 'js', 'json', 'php', 'py', 'sql']:
-                                        # For code files content are put ina codeblock
-                                        self._logger.info(f'        With content as code block')
-                                        with open(original_file, 'r') as file:
-                                            content = file.read()
-                                        # Create a markdown file that take care of showing source code annex
-                                        if not os.path.exists(os.path.dirname(embedded)):
-                                            os.makedirs(os.path.dirname(embedded))
-                                        with open(embedded, 'a') as f:
-                                            # write the title and the content to the file
-                                            f.write(f'## {os.path.splitext(rel_file)[0]}\n\n``` {extension}\n{content}\n```\n')
-                                    else:
-                                        self._logger.warning(f'file {src} extension isn\'t supported (yet) --> skipped')
+                                for i in range(len(images)):
+                                    # Add leading zeros to the page number
+                                    filename = f'page_{i + 1:04}.png'
+                                    images[i].save(f'{source}/{filename}', 'PNG')
+                                    files.append(File(os.path.join(os.path.splitext(dest)[0], f'source/{filename}'), src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
+
+                                    # Write the image link to the file
+                                    f.write(f'![Page {i+1}](./{os.path.basename(os.path.splitext(dest)[0])}/source/{filename})\n')
+                        else:
+                            self._logger.warning(f'file {src} extension isn\'t supported --> skipped')
+                        # Removing originals files from list of mkdocs files if they were in the docs directory originaly
+                        if os.path.isfile(os.path.join(config.docs_dir, dest)):
+                            self._logger.info(f'    Remvoing original annex {src} from processed files list')
+                            files.remove(files.get_file_from_path(src))
                         # Adding embedded files in list of mkdocs files
                         path = f'{os.path.splitext(dest)[0]}.md'
                         self._logger.info(f'    Adding embedded annex {dest} to processed files list')
                         files.append(File(path, src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
                     else:
                         self._logger.warning(f'{src} file doesn\'t exist at {original} --> skipped')
             except Exception as e:
```

### Comparing `mkdocs-annexes-integration-0.1.5/mkdocs_annexes_integration.egg-info/PKG-INFO` & `mkdocs-annexes-integration-0.1.6/mkdocs_annexes_integration.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,117 +1,107 @@
 Metadata-Version: 2.1
 Name: mkdocs-annexes-integration
-Version: 0.1.5
-Summary: A MkDocs plugin transforming annexes files into images or code blocks to be integrated in markdown pages
+Version: 0.1.6
+Summary: A MkDocs plugin transforming annexes files into images to be integrated in markdown pages
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
-Description: # mkdocs-annexes-integration
-        
-        This is a plugin that transforms annex files into images or code blocks to be integrated in Markdown pages for MkDocs.
-        
-        ## Setup
-        
-        ### Before installing
-        
-        Before installing this plugin you need to install `poppler-utils` as it is used by `pdf2image` that is required to use this plugin.
-        
-        #### Install on Linux :
-        
-        Note: *It depend on your Linux OS*
-        
-        ``` sh
-        sudo apt-get install poppler-utils
-        ```
-        
-        ``` sh
-        sudo yum install poppler-utils
-        ```
-        
-        #### Install on MacOS :
-        
-        ``` sh
-        brew install poppler
-        ```
-        
-        #### Install on Windows :
-        
-        On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
-        
-        ### Installing using pip:
-        
-        `pip install mkdocs-annexes-integration`
-        
-        ## Config
-        
-        You need to activate the plugin in `mkdocs.yml`:
-        
-        ```yaml
-        plugins:
-          - annexes-integration:
-              annexes: # Required (at least 1)
-                - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
-                - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
-                - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
-                - Title of the code file annex:
-                    src: ../src/path/to/a/code/file.py
-                    dest: dest/path/to/a/code/file.py
-                - Title of the code directory annex:
-                    src: ../src/path/to/a/code/directory
-                    dest: dest/path/to/a/code/directory
-                # others annexes...
-              temp_dir: "folder_name" # Optional --> Default : temp_annexes
-              enabled_if_env: ENABLE_ANNEXES_INTEGRATION # Optional
-        ```
-        
-        As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
-        
-        Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
-        
-        - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file or directory associated to it's title. Each file in a directory will integrated in subsection of the same document with a heading 2 containing the relative path of the file from the given directory.
-        - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
-        - `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
-        
-        ## Usage
-        
-        Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
-        
-        This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
-        
-        ## Support
-        
-        This plugin currently support two type of files :
-        
-        - **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
-        
-        - **Code files**: The plugin will put the content of the code file into a codeblock to be integrated on a page
-        
-        Currently supported code files are :
-         - CSharp (.cs)
-         - CSS (.css)
-         - Dart (.dart)
-         - HTML (.html)
-         - Javascript (.js)
-         - JSON (.json)
-         - PHP (.php)
-         - Python (.py)
-        
-        ## License
-        
-        This project is under MIT license see: `license` file for more detail.
-        
-        ## See Also
-        
-        - [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
-        - [mkdocs website](http://www.mkdocs.org/)
-        - [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
 Keywords: mkdocs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+
+# mkdocs-annexes-integration
+
+This is a plugin that transforms annex files into images to be integrated in Markdown pages for MkDocs.
+
+## Setup
+
+### Before installing
+
+Before installing this plugin you need to install `poppler-utils` as it is used by `pdf2image` that is required to use this plugin.
+
+#### Install on Linux :
+
+Note: *It depend on your Linux OS*
+
+``` sh
+sudo apt-get install poppler-utils
+```
+
+``` sh
+sudo yum install poppler-utils
+```
+
+#### Install on MacOS :
+
+``` sh
+brew install poppler
+```
+
+#### Install on Windows :
+
+On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
+
+### Installing using pip:
+
+`pip install mkdocs-annexes-integration`
+
+## Config
+
+You need to activate the plugin in `mkdocs.yml`:
+
+```yaml
+plugins:
+  - annexes-integration:
+      annexes: # Required (at least 1)
+        - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
+        - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
+        - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
+        - Title of the annex:
+            src: ../src/path/to/an/annex/file1.py
+            dest: dest/path/to/an/annex/file1.py
+        # others annexes...
+      temp_dir: "folder_name" # Optional --> Default : temp_annexes
+      enabled_if_env: ENABLE_PDF_EXPORT # Optional
+```
+
+As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
+
+Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
+
+- `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
+- `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
+- `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
+
+## Usage
+
+Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
+
+This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
+
+It is also strongly recommended to use it with `mkdocs-material` plugin. Using this plugin without `mkdocs-material` may result in unecessary page break between annex title and annex images.
+
+## Support
+
+This plugin currently support PDF files :
+
+- **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
+
+## License
+
+This project is under MIT license see: `license` file for more detail.
+
+## See Also
+
+- [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
+- [mkdocs website](http://www.mkdocs.org/)
+- [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
+- [mkdocs material plugin](https://github.com/squidfunk/mkdocs-material)
+
```

### Comparing `mkdocs-annexes-integration-0.1.5/readme.md` & `mkdocs-annexes-integration-0.1.6/readme.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,87 @@
-# mkdocs-annexes-integration
-
-This is a plugin that transforms annex files into images or code blocks to be integrated in Markdown pages for MkDocs.
-
-## Setup
-
-### Before installing
-
-Before installing this plugin you need to install `poppler-utils` as it is used by `pdf2image` that is required to use this plugin.
-
-#### Install on Linux :
-
-Note: *It depend on your Linux OS*
-
-``` sh
-sudo apt-get install poppler-utils
-```
-
-``` sh
-sudo yum install poppler-utils
-```
-
-#### Install on MacOS :
-
-``` sh
-brew install poppler
-```
-
-#### Install on Windows :
-
-On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
-
-### Installing using pip:
-
-`pip install mkdocs-annexes-integration`
-
-## Config
-
-You need to activate the plugin in `mkdocs.yml`:
-
-```yaml
-plugins:
-  - annexes-integration:
-      annexes: # Required (at least 1)
-        - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
-        - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
-        - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
-        - Title of the code file annex:
-            src: ../src/path/to/a/code/file.py
-            dest: dest/path/to/a/code/file.py
-        - Title of the code directory annex:
-            src: ../src/path/to/a/code/directory
-            dest: dest/path/to/a/code/directory
-        # others annexes...
-      temp_dir: "folder_name" # Optional --> Default : temp_annexes
-      enabled_if_env: ENABLE_ANNEXES_INTEGRATION # Optional
-```
-
-As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
-
-Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
-
-- `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file or directory associated to it's title. Each file in a directory will integrated in subsection of the same document with a heading 2 containing the relative path of the file from the given directory.
-- `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
-- `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
-
-## Usage
-
-Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
-
-This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
-
-## Support
-
-This plugin currently support two type of files :
-
-- **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
-
-- **Code files**: The plugin will put the content of the code file into a codeblock to be integrated on a page
-
-Currently supported code files are :
- - CSharp (.cs)
- - CSS (.css)
- - Dart (.dart)
- - HTML (.html)
- - Javascript (.js)
- - JSON (.json)
- - PHP (.php)
- - Python (.py)
-
-## License
-
-This project is under MIT license see: `license` file for more detail.
-
-## See Also
-
-- [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
-- [mkdocs website](http://www.mkdocs.org/)
-- [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
+# mkdocs-annexes-integration
+
+This is a plugin that transforms annex files into images to be integrated in Markdown pages for MkDocs.
+
+## Setup
+
+### Before installing
+
+Before installing this plugin you need to install `poppler-utils` as it is used by `pdf2image` that is required to use this plugin.
+
+#### Install on Linux :
+
+Note: *It depend on your Linux OS*
+
+``` sh
+sudo apt-get install poppler-utils
+```
+
+``` sh
+sudo yum install poppler-utils
+```
+
+#### Install on MacOS :
+
+``` sh
+brew install poppler
+```
+
+#### Install on Windows :
+
+On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
+
+### Installing using pip:
+
+`pip install mkdocs-annexes-integration`
+
+## Config
+
+You need to activate the plugin in `mkdocs.yml`:
+
+```yaml
+plugins:
+  - annexes-integration:
+      annexes: # Required (at least 1)
+        - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
+        - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
+        - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
+        - Title of the annex:
+            src: ../src/path/to/an/annex/file1.py
+            dest: dest/path/to/an/annex/file1.py
+        # others annexes...
+      temp_dir: "folder_name" # Optional --> Default : temp_annexes
+      enabled_if_env: ENABLE_PDF_EXPORT # Optional
+```
+
+As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
+
+Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
+
+- `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
+- `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
+- `enabled_if_env` - Setting this option will enable the build only if there is an environment variable set to 1. Integrations of PDF can slow down build process and it's pretty useful to be fast when doing modification to mkdocs files when doing mkdocs serve.
+
+## Usage
+
+Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
+
+This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
+
+It is also strongly recommended to use it with `mkdocs-material` plugin. Using this plugin without `mkdocs-material` may result in unecessary page break between annex title and annex images.
+
+## Support
+
+This plugin currently support PDF files :
+
+- **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
+
+## License
+
+This project is under MIT license see: `license` file for more detail.
+
+## See Also
+
+- [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
+- [mkdocs website](http://www.mkdocs.org/)
+- [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
+- [mkdocs material plugin](https://github.com/squidfunk/mkdocs-material)
```

### Comparing `mkdocs-annexes-integration-0.1.5/setup.py` & `mkdocs-annexes-integration-0.1.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-annexes-integration',
-    version='0.1.5',
-    description='A MkDocs plugin transforming annexes files into images or code blocks to be integrated in markdown pages',
+    version='0.1.6',
+    description='A MkDocs plugin transforming annexes files into images to be integrated in markdown pages',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
     license='MIT',
```

