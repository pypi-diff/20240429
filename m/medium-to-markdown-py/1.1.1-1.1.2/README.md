# Comparing `tmp/medium_to_markdown_py-1.1.1.tar.gz` & `tmp/medium_to_markdown_py-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_to_markdown_py-1.1.1.tar", last modified: Mon Apr 29 12:54:54 2024, max compression
+gzip compressed data, was "medium_to_markdown_py-1.1.2.tar", last modified: Mon Apr 29 13:19:19 2024, max compression
```

## Comparing `medium_to_markdown_py-1.1.1.tar` & `medium_to_markdown_py-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 12:54:54.639310 medium_to_markdown_py-1.1.1/
--rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.1/LICENSE
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-29 12:54:54.639227 medium_to_markdown_py-1.1.1/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      640 2024-04-28 14:43:34.000000 medium_to_markdown_py-1.1.1/README.md
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 12:54:54.638018 medium_to_markdown_py-1.1.1/medium_to_markdown/
--rw-r--r--   0 shin       (501) staff       (20)     7607 2024-04-29 12:54:04.000000 medium_to_markdown_py-1.1.1/medium_to_markdown/Parser.py
--rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-29 12:54:36.000000 medium_to_markdown_py-1.1.1/medium_to_markdown/__init__.py
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 12:54:54.639005 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      364 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/SOURCES.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/dependency_links.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/not-zip-safe
--rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/requires.txt
--rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/top_level.txt
--rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-29 12:54:54.639526 medium_to_markdown_py-1.1.1/setup.cfg
--rw-r--r--   0 shin       (501) staff       (20)      612 2024-04-29 12:54:37.000000 medium_to_markdown_py-1.1.1/setup.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 13:19:19.902653 medium_to_markdown_py-1.1.2/
+-rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.2/LICENSE
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-29 13:19:19.902592 medium_to_markdown_py-1.1.2/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      670 2024-04-29 13:19:17.000000 medium_to_markdown_py-1.1.2/README.md
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 13:19:19.901506 medium_to_markdown_py-1.1.2/medium_to_markdown/
+-rw-r--r--   0 shin       (501) staff       (20)     7724 2024-04-29 13:18:14.000000 medium_to_markdown_py-1.1.2/medium_to_markdown/Parser.py
+-rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-29 13:18:34.000000 medium_to_markdown_py-1.1.2/medium_to_markdown/__init__.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 13:19:19.902381 medium_to_markdown_py-1.1.2/medium_to_markdown_py.egg-info/
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-29 13:19:19.000000 medium_to_markdown_py-1.1.2/medium_to_markdown_py.egg-info/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      364 2024-04-29 13:19:19.000000 medium_to_markdown_py-1.1.2/medium_to_markdown_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-29 13:19:19.000000 medium_to_markdown_py-1.1.2/medium_to_markdown_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.2/medium_to_markdown_py.egg-info/not-zip-safe
+-rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-29 13:19:19.000000 medium_to_markdown_py-1.1.2/medium_to_markdown_py.egg-info/requires.txt
+-rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-29 13:19:19.000000 medium_to_markdown_py-1.1.2/medium_to_markdown_py.egg-info/top_level.txt
+-rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-29 13:19:19.902859 medium_to_markdown_py-1.1.2/setup.cfg
+-rw-r--r--   0 shin       (501) staff       (20)      612 2024-04-29 13:18:39.000000 medium_to_markdown_py-1.1.2/setup.py
```

### Comparing `medium_to_markdown_py-1.1.1/LICENSE` & `medium_to_markdown_py-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.1.1/README.md` & `medium_to_markdown_py-1.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 The command-line interface (CLI) accepts a Medium blog post URL and a filename as input and generates the Markdown content.
 
 ``` python
 from medium_to_markdown.Parser import MediumParser
 
 url = "https://~~~~"
 filename = ""
+output_dir ="medium/origin_md"
 is_image_download = True
 ssl_verify = True
 
-parser = MediumParser(url, filename, is_image_download, ssl_verify)
+parser = MediumParser(url, output_dir, filename, is_image_download, ssl_verify)
 
-if parser.parse_and_savefile():
+if parser.parse():
     print("Parsing is done.")
 
 ```
```

### Comparing `medium_to_markdown_py-1.1.1/medium_to_markdown/Parser.py` & `medium_to_markdown_py-1.1.2/medium_to_markdown/Parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,27 +39,29 @@
                 
             self.output_filename = f"{self.current_date}-{self.output_filename}"
 
 
     def parse(self,is_save=True):
         """
         Parses the Medium post, saves it as a Markdown file, and returns True if successful, False otherwise.
+        Parameters:
+        - is_save (bool): Flag indicating whether to save the output Markdown file. Default is True.
         """
         try:
             dom = self.get_dom(self.url)
             self.get_meta(dom)
             
             if self.output_filename == "":
                 self.output_filename = re.sub(r'[<>:"/\\|?*]', '', self.title).replace(" ", "_")
                 output_filename = f"{self.OUTPUT_DIR}/{self.current_date}-{self.output_filename}.md"
             else:
                 output_filename = f"{self.OUTPUT_DIR}/{self.output_filename}.md"
                 
             
-                parsed_post = self.parse_medium_post(dom)
+            parsed_post = self.parse_medium_post(dom)
                 
             if is_save:
                 if not os.path.exists(os.path.dirname(output_filename)):
                     os.makedirs(os.path.dirname(output_filename))
                 with open(output_filename, "w", encoding='utf-8') as f:
                     f.write(parsed_post)
                 return True
```

### Comparing `medium_to_markdown_py-1.1.1/setup.py` & `medium_to_markdown_py-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medium_to_markdown_py',
-    version='1.1.1',
+    version='1.1.2',
     description='medium-to-medium_to_markdown_py-py is a Python package that converts Medium articles to Markdown format.',
     author='knowslog',
     author_email='scshin88@gmail.com',
     url='https://github.com/tourbut/medium-to-markdown_python',
     install_requires=['beautifulsoup4', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['medium', 'knowslog', 'markdown', 'medium to markdown'],
```

