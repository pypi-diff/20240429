# Comparing `tmp/zzd-cli-0.1.0.tar.gz` & `tmp/zzd-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zzd-cli-0.1.0.tar", last modified: Fri Mar  8 13:28:01 2024, max compression
+gzip compressed data, was "zzd-cli-0.2.0.tar", last modified: Mon Apr 29 07:29:39 2024, max compression
```

## Comparing `zzd-cli-0.1.0.tar` & `zzd-cli-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-03-08 13:28:01.535735 zzd-cli-0.1.0/
--rw-r--r--   0 qinyiqi    (501) staff       (20)      210 2024-03-08 13:28:01.535643 zzd-cli-0.1.0/PKG-INFO
--rw-r--r--   0 qinyiqi    (501) staff       (20)     3508 2024-03-08 10:29:30.000000 zzd-cli-0.1.0/README.md
--rw-r--r--   0 qinyiqi    (501) staff       (20)       38 2024-03-08 13:28:01.535768 zzd-cli-0.1.0/setup.cfg
--rw-r--r--   0 qinyiqi    (501) staff       (20)      496 2024-03-08 13:24:40.000000 zzd-cli-0.1.0/setup.py
-drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-03-08 13:28:01.534876 zzd-cli-0.1.0/zzd/
--rw-r--r--   0 qinyiqi    (501) staff       (20)        0 2024-02-24 09:26:56.000000 zzd-cli-0.1.0/zzd/__init__.py
--rw-r--r--   0 qinyiqi    (501) staff       (20)    36624 2024-03-08 13:27:48.000000 zzd-cli-0.1.0/zzd/cli.py
-drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-03-08 13:28:01.535517 zzd-cli-0.1.0/zzd_cli.egg-info/
--rw-r--r--   0 qinyiqi    (501) staff       (20)      210 2024-03-08 13:28:01.000000 zzd-cli-0.1.0/zzd_cli.egg-info/PKG-INFO
--rw-r--r--   0 qinyiqi    (501) staff       (20)      233 2024-03-08 13:28:01.000000 zzd-cli-0.1.0/zzd_cli.egg-info/SOURCES.txt
--rw-r--r--   0 qinyiqi    (501) staff       (20)        1 2024-03-08 13:28:01.000000 zzd-cli-0.1.0/zzd_cli.egg-info/dependency_links.txt
--rw-r--r--   0 qinyiqi    (501) staff       (20)       55 2024-03-08 13:28:01.000000 zzd-cli-0.1.0/zzd_cli.egg-info/entry_points.txt
--rw-r--r--   0 qinyiqi    (501) staff       (20)       55 2024-03-08 13:28:01.000000 zzd-cli-0.1.0/zzd_cli.egg-info/requires.txt
--rw-r--r--   0 qinyiqi    (501) staff       (20)        4 2024-03-08 13:28:01.000000 zzd-cli-0.1.0/zzd_cli.egg-info/top_level.txt
+drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-04-29 07:29:39.071671 zzd-cli-0.2.0/
+-rw-r--r--   0 qinyiqi    (501) staff       (20)      210 2024-04-29 07:29:39.071581 zzd-cli-0.2.0/PKG-INFO
+-rw-r--r--   0 qinyiqi    (501) staff       (20)     3508 2024-03-08 10:29:30.000000 zzd-cli-0.2.0/README.md
+-rw-r--r--   0 qinyiqi    (501) staff       (20)       38 2024-04-29 07:29:39.071702 zzd-cli-0.2.0/setup.cfg
+-rw-r--r--   0 qinyiqi    (501) staff       (20)      496 2024-04-29 07:29:31.000000 zzd-cli-0.2.0/setup.py
+drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-04-29 07:29:39.070878 zzd-cli-0.2.0/zzd/
+-rw-r--r--   0 qinyiqi    (501) staff       (20)        0 2024-02-24 09:26:56.000000 zzd-cli-0.2.0/zzd/__init__.py
+-rw-r--r--   0 qinyiqi    (501) staff       (20)    37655 2024-04-29 07:21:06.000000 zzd-cli-0.2.0/zzd/cli.py
+drwxr-xr-x   0 qinyiqi    (501) staff       (20)        0 2024-04-29 07:29:39.071466 zzd-cli-0.2.0/zzd_cli.egg-info/
+-rw-r--r--   0 qinyiqi    (501) staff       (20)      210 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/PKG-INFO
+-rw-r--r--   0 qinyiqi    (501) staff       (20)      233 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 qinyiqi    (501) staff       (20)        1 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 qinyiqi    (501) staff       (20)       55 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/entry_points.txt
+-rw-r--r--   0 qinyiqi    (501) staff       (20)       55 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/requires.txt
+-rw-r--r--   0 qinyiqi    (501) staff       (20)        4 2024-04-29 07:29:39.000000 zzd-cli-0.2.0/zzd_cli.egg-info/top_level.txt
```

### Comparing `zzd-cli-0.1.0/README.md` & `zzd-cli-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zzd-cli-0.1.0/zzd/cli.py` & `zzd-cli-0.2.0/zzd/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,21 @@
 # from pprint36 import pprint
 import chardet
 from bs4 import BeautifulSoup
 
 # brew update && brew upgrade openssl
 # pip install urllib3==1.26.16
 
+
+# PATTERN = r'(?<!zzd.one:8000)(/media/)'
 # BASE = "http://zzd.one:8000/"
+# CODEBASE = "http://code.zzd.one:8000/"
+PATTERN = r'(?<!zzd.show)(/media/)'
 BASE = "https://zzd.show/"
+CODEBASE = "https://code.zzd.show/"
 
 ENDPOINTS = {
     'web': 'users/cli/', 
     'tokenverify': 'users/cli/tokenverify/',
     'login': 'users/cli/login/',
     'list': 'shows/cli/list/',
     'clone': 'shows/cli/clone/',
@@ -282,15 +287,41 @@
 def get_compiled_name(rawname, generic):
     sld = rawname.split('.')
     ext = sld.pop()
     nm = '.'.join(sld) + '_' + ext + '.' + generic
     return nm
 
 
-def html_embrace(compiled: bool, cdndt, title, html, css_refs, js_refs):
+def process_media_links(raw_text):
+    # Regular expression to target /media/ that appears at the start of the path or after a space or quote,
+    # and not part of a full URL (by checking it's not immediately following ':' or a slash)
+    pattern = r'(?<![:/.\w])(/media/)'
+    # Replacement string with the desired URL prefix
+    replacement = 'https://code.zzd.show/media/'
+    # Using re.sub() to replace the matched patterns in the string
+    return re.sub(pattern, replacement, raw_text)
+
+
+# print(process_media_links('''
+# <div class="content">
+# <img src="https://cdn.io/media/portray/ksenia.jpg"/>
+# </div>
+
+# <div class="content">
+# <img src="/media/portray/ksenia.jpg"/>
+# </div>
+
+# div{
+#     background: url('/media/portray/ksenia.jpg');
+# }
+# '''))
+# exit()
+
+def html_embrace(compiled: bool, cdndt, title, _html, css_refs, js_refs):
+    html = process_media_links(_html)
     css_blocks = '\n'
     js_blocks = '\n'
     if cdndt:
         cdn_css = cdndt.get('css')
         cdn_js = cdndt.get('js')
         if cdn_css:
             for cdn in cdn_css:
@@ -399,23 +430,23 @@
         for filename, dt in ddt.items():
             unplug = dt.get('unplug')
             raw = dt.get('raw')
             compiled = dt.get('compiled')
             filepath = os.path.join(generic_dir, filename)
             if commit:
                 with open(filepath, 'w', encoding="utf-8") as f:
-                    f.write(raw)
+                    f.write(process_media_links(raw))
             if compiled:
                 compiled_dir = os.path.join(generic_dir, 'compiled')
                 compiled_name = get_compiled_name(filename, generic)
                 compiled_path = os.path.join(compiled_dir, compiled_name)
                 if commit:
                     os.makedirs(compiled_dir, exist_ok=True)
                     with open(compiled_path, 'w', encoding="utf-8") as f:
-                        f.write(compiled)
+                        f.write(process_media_links(compiled))
                 _sld = compiled_path.split('/')
                 _sld.pop(0)
                 relative_path = '/'.join(_sld)
                 if generic == 'css':
                     css_refs.append(relative_path)
                 elif generic == 'js':
                     js_refs.append(relative_path)
@@ -450,15 +481,15 @@
         if commit:
             with open(filepath, 'w', encoding="utf-8") as f:
                 if not compiled:
                     # html
                     f.write(html_embrace(False, data['cdns'], data['title'], raw, css_refs, js_refs))
                 else:
                     # pug, etc (handled in previous condition, only compiled parsed)
-                    f.write(raw)
+                    f.write(process_media_links(raw))
 
 
 # exit()
 
 @zzd.command(help="唯一参数，可以是一个序号或者一个链接")
 @click.argument('demo', type=str)
 def clone(demo):
```

