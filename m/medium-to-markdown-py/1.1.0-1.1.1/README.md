# Comparing `tmp/medium_to_markdown_py-1.1.0.tar.gz` & `tmp/medium_to_markdown_py-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_to_markdown_py-1.1.0.tar", last modified: Sun Apr 28 14:43:41 2024, max compression
+gzip compressed data, was "medium_to_markdown_py-1.1.1.tar", last modified: Mon Apr 29 12:54:54 2024, max compression
```

## Comparing `medium_to_markdown_py-1.1.0.tar` & `medium_to_markdown_py-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:43:41.611638 medium_to_markdown_py-1.1.0/
--rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.0/LICENSE
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-28 14:43:41.611565 medium_to_markdown_py-1.1.0/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      640 2024-04-28 14:43:34.000000 medium_to_markdown_py-1.1.0/README.md
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:43:41.609990 medium_to_markdown_py-1.1.0/medium_to_markdown/
--rw-r--r--   0 shin       (501) staff       (20)     7314 2024-04-28 14:42:30.000000 medium_to_markdown_py-1.1.0/medium_to_markdown/Parser.py
--rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-28 14:43:18.000000 medium_to_markdown_py-1.1.0/medium_to_markdown/__init__.py
-drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-28 14:43:41.611351 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/
--rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/PKG-INFO
--rw-r--r--   0 shin       (501) staff       (20)      364 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/SOURCES.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/dependency_links.txt
--rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/not-zip-safe
--rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/requires.txt
--rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.0/medium_to_markdown_py.egg-info/top_level.txt
--rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-28 14:43:41.611860 medium_to_markdown_py-1.1.0/setup.cfg
--rw-r--r--   0 shin       (501) staff       (20)      612 2024-04-28 14:43:14.000000 medium_to_markdown_py-1.1.0/setup.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 12:54:54.639310 medium_to_markdown_py-1.1.1/
+-rw-r--r--   0 shin       (501) staff       (20)    35148 2024-04-28 04:31:04.000000 medium_to_markdown_py-1.1.1/LICENSE
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-29 12:54:54.639227 medium_to_markdown_py-1.1.1/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      640 2024-04-28 14:43:34.000000 medium_to_markdown_py-1.1.1/README.md
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 12:54:54.638018 medium_to_markdown_py-1.1.1/medium_to_markdown/
+-rw-r--r--   0 shin       (501) staff       (20)     7607 2024-04-29 12:54:04.000000 medium_to_markdown_py-1.1.1/medium_to_markdown/Parser.py
+-rw-r--r--   0 shin       (501) staff       (20)       21 2024-04-29 12:54:36.000000 medium_to_markdown_py-1.1.1/medium_to_markdown/__init__.py
+drwxr-xr-x   0 shin       (501) staff       (20)        0 2024-04-29 12:54:54.639005 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/
+-rw-r--r--   0 shin       (501) staff       (20)      446 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/PKG-INFO
+-rw-r--r--   0 shin       (501) staff       (20)      364 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/SOURCES.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/dependency_links.txt
+-rw-r--r--   0 shin       (501) staff       (20)        1 2024-04-28 14:43:41.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/not-zip-safe
+-rw-r--r--   0 shin       (501) staff       (20)       24 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/requires.txt
+-rw-r--r--   0 shin       (501) staff       (20)       19 2024-04-29 12:54:54.000000 medium_to_markdown_py-1.1.1/medium_to_markdown_py.egg-info/top_level.txt
+-rw-r--r--   0 shin       (501) staff       (20)       79 2024-04-29 12:54:54.639526 medium_to_markdown_py-1.1.1/setup.cfg
+-rw-r--r--   0 shin       (501) staff       (20)      612 2024-04-29 12:54:37.000000 medium_to_markdown_py-1.1.1/setup.py
```

### Comparing `medium_to_markdown_py-1.1.0/LICENSE` & `medium_to_markdown_py-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.1.0/README.md` & `medium_to_markdown_py-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `medium_to_markdown_py-1.1.0/medium_to_markdown/Parser.py` & `medium_to_markdown_py-1.1.1/medium_to_markdown/Parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,64 +7,69 @@
 import re
 
 class MediumParser:
     
     IMAGE_SEQUENCE = 0
     OUTPUT_DIR = "medium/origin_md"
     
-    def __init__(self, url, output_filename="", is_image_download=False,ssl_verify=False,headers={'User-Agent': 'Mozilla/5.0'}):
+    def __init__(self, url, output_dir = "medium/origin_md",output_filename="", is_image_download=False,ssl_verify=False,headers={'User-Agent': 'Mozilla/5.0'}):
         """
             Initialize a MediumParser object.
 
             Parameters:
             - url (str): The URL of the Medium article to convert to Markdown.
+            - output_dir (str): The directory where the output Markdown file will be saved. Default is 'medium/origin_md'.
             - output_filename (str): The desired filename for the output Markdown file. If not provided, a default filename will be used.
             - is_image_download (bool): Flag indicating whether to download images referenced in the article. Default is False.
             - ssl_verify (bool): Flag indicating whether to verify SSL certificates when making requests. Default is False.
             - headers (dict): Custom headers to include in the HTTP requests. Default is {'User-Agent': 'Mozilla/5.0'}.
         """
         self.url = url
         self.is_image_download = is_image_download
         self.ssl_verify = ssl_verify
         self.headers = headers
         self.current_date = datetime.now().strftime("%Y-%m-%d")
         self.title=""
         self.author=""
         self.output_filename=output_filename
+        self.OUTPUT_DIR = output_dir
         
         if self.output_filename != "":
             if self.output_filename.endswith(".md"):
                 self.output_filename = self.output_filename[:-3]
                 
             self.output_filename = f"{self.current_date}-{self.output_filename}"
 
 
-    def parse_and_savefile(self):
+    def parse(self,is_save=True):
         """
         Parses the Medium post, saves it as a Markdown file, and returns True if successful, False otherwise.
         """
         try:
             dom = self.get_dom(self.url)
             self.get_meta(dom)
             
             if self.output_filename == "":
                 self.output_filename = re.sub(r'[<>:"/\\|?*]', '', self.title).replace(" ", "_")
                 output_filename = f"{self.OUTPUT_DIR}/{self.current_date}-{self.output_filename}.md"
             else:
                 output_filename = f"{self.OUTPUT_DIR}/{self.output_filename}.md"
                 
-            parsed_post = self.parse_medium_post(dom)
             
-            if not os.path.exists(os.path.dirname(output_filename)):
-                os.makedirs(os.path.dirname(output_filename))
-            
-            with open(output_filename, "w", encoding='utf-8') as f:
-                f.write(parsed_post)
+                parsed_post = self.parse_medium_post(dom)
                 
-            return True
+            if is_save:
+                if not os.path.exists(os.path.dirname(output_filename)):
+                    os.makedirs(os.path.dirname(output_filename))
+                with open(output_filename, "w", encoding='utf-8') as f:
+                    f.write(parsed_post)
+                return True
+            else:
+                return parsed_post
+            
         except Exception as e:
             print(f"An error occurred: {e}")
             return False
 
     def get_dom(self,url):
         response = requests.get(url, verify=self.ssl_verify,headers=self.headers)
         response.raise_for_status()
```

### Comparing `medium_to_markdown_py-1.1.0/setup.py` & `medium_to_markdown_py-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='medium_to_markdown_py',
-    version='1.1.0',
+    version='1.1.1',
     description='medium-to-medium_to_markdown_py-py is a Python package that converts Medium articles to Markdown format.',
     author='knowslog',
     author_email='scshin88@gmail.com',
     url='https://github.com/tourbut/medium-to-markdown_python',
     install_requires=['beautifulsoup4', 'requests'],
     packages=find_packages(exclude=[]),
     keywords=['medium', 'knowslog', 'markdown', 'medium to markdown'],
```

