# Comparing `tmp/urlscan-1.0.1.tar.gz` & `tmp/urlscan-1.0.2.tar.gz`

## Comparing `urlscan-1.0.1.tar` & `urlscan-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     7322 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan.1
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/__init__.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/_version.py
--rw-r--r--   0        0        0    37006 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/urlchoose.py
--rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/urlscan.py
--rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 urlscan-1.0.1/urlscan/assets/tlds-alpha-by-domain.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 urlscan-1.0.1/.gitignore
--rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 urlscan-1.0.1/LICENSE
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 urlscan-1.0.1/README.md
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 urlscan-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8866 2020-02-02 00:00:00.000000 urlscan-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     7321 2020-02-02 00:00:00.000000 urlscan-1.0.2/urlscan.1
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 urlscan-1.0.2/urlscan/__init__.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 urlscan-1.0.2/urlscan/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 urlscan-1.0.2/urlscan/_version.py
+-rw-r--r--   0        0        0    36995 2020-02-02 00:00:00.000000 urlscan-1.0.2/urlscan/urlchoose.py
+-rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 urlscan-1.0.2/urlscan/urlscan.py
+-rw-r--r--   0        0        0     9912 2020-02-02 00:00:00.000000 urlscan-1.0.2/urlscan/assets/tlds-alpha-by-domain.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 urlscan-1.0.2/.gitignore
+-rw-r--r--   0        0        0    17987 2020-02-02 00:00:00.000000 urlscan-1.0.2/LICENSE
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 urlscan-1.0.2/README.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 urlscan-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9751 2020-02-02 00:00:00.000000 urlscan-1.0.2/PKG-INFO
```

### Comparing `urlscan-1.0.1/urlscan.1` & `urlscan-1.0.2/urlscan.1`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
     $ urlscan --run-safe 'xclip -i' --pipe file.txt
 .TP
 .B \-R, \-\-reverse
 Reverse displayed order of URLs.
 .TP
 .B \-r, \-\-run \<expression\>
 Execute \<expression\> in place of opening URL with a browser. Use {} in
-\<expression\> to substitute in the URL. Shell features such as \| and \> can be
+\<expression\> to substitute in the URL. Shell features such as | and \> can be
 used, but it is less secure. Examples:
 
     $ urlscan --run 'echo {} | xclip -i' file.txt
 .TP
 .B \-s, \-\-single
 Exit urlscan after opening or copying a single browser link.
```

### Comparing `urlscan-1.0.1/urlscan/__main__.py` & `urlscan-1.0.2/urlscan/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                            help="Pipe URLs to stdout")
     arg_parse.add_argument('--dedupe', '-d', dest="dedupe",
                            action='store_true', default=False,
                            help="Remove duplicate URLs from list")
     arg_parse.add_argument('--regex', '-E',
                            help="Alternate custom regex to be used for all "
                            "kinds of matching. "
-                           "For example: --regex 'https?://.+\.\w+'")
+                           r"For example: --regex 'https?://.+\.\w+'")
     arg_parse.add_argument('--run', '-r',
                            help="Alternate command to run on selected URL "
                            "instead of opening URL in browser. Use {} to "
                            "represent the URL value in the expression. "
                            "For example: --run 'echo {} | xclip -i'")
     arg_parse.add_argument('--run-safe', '-f', dest="runsafe",
                            help="Alternate command to run on selected URL "
```

### Comparing `urlscan-1.0.1/urlscan/urlchoose.py` & `urlscan-1.0.2/urlscan/urlchoose.py`

 * *Files 1% similar despite different names*

```diff
@@ -695,15 +695,15 @@
         self.top.base_widget.footer = footerwid
         search_items = []
         for grp in self.items_org:
             done = False
             for idx, item in enumerate(grp):
                 if isinstance(item, urwid.Columns):
                     for col_idx, col in enumerate(item.contents):
-                        if isinstance(col[0], urwid.decoration.AttrMap):
+                        if isinstance(col[0], urwid.AttrMap):
                             grp[idx][col_idx].set_label(splittext(col[0].base_widget.label,
                                                                   self.search_string,
                                                                   ''))
                             if self.search_string.lower() in col[0].base_widget.label.lower():
                                 grp[idx][col_idx].set_label(splittext(col[0].base_widget.label,
                                                                       self.search_string,
                                                                       'search'))
```

### Comparing `urlscan-1.0.1/urlscan/urlscan.py` & `urlscan-1.0.2/urlscan/urlscan.py`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.1/urlscan/assets/tlds-alpha-by-domain.txt` & `urlscan-1.0.2/urlscan/assets/tlds-alpha-by-domain.txt`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.1/LICENSE` & `urlscan-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `urlscan-1.0.1/README.md` & `urlscan-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Urlscan
 
+[![main](https://github.com/firecat53/urlscan/actions/workflows/main.yml/badge.svg)](https://github.com/firecat53/urlscan/actions/workflows/main.yml)
+
 ## Contributors
 
 Scott Hansen \<tech@firecat53.net\> (Author and Maintainer)
 
 Maxime Chatelle \<xakz@rxsoft.eu\> (Debian Maintainer)
 
 Daniel Burrows \<dburrows@debian.org\> (Original Author)
@@ -68,18 +70,18 @@
 - Queue multiple URLs for opening and open them all at once with `a` and `o`.
 
 ## Installation and setup
 
 To install urlscan, install from your distribution repositories, from Pypi, or do
 a local development install with pip -e:
 
-    pipx install urlscan 
-    
+    pipx install urlscan
+
     OR
-    
+
     pip install --user urlscan
 
     OR
 
     cd <path/to/urlscan> && pip install --user -e .
 
 **NOTE**
@@ -93,14 +95,23 @@
 
     macro attach,compose \cb "<pipe-entry> urlscan<Enter>" "call urlscan to
     extract URLs out of a message"
 
 Once this is done, Control-b while reading mail in mutt will automatically
 invoke urlscan on the message.
 
+> Note for Neomutt users: [As of version
+> `2023-05-17`](https://github.com/neomutt/neomutt/releases/tag/20230517) true
+> color support was implemented. If you are using true color support with Neomutt,
+> or are encountering the error `setupterm: could not find terminfo database`,
+> then you should also add `TERM=xterm-256color` to your macro in `.muttrc`.
+> See more here [#135](https://github.com/firecat53/urlscan/issues/135). For example:
+> `macro index,pager  \cb "<pipe-message>  TERM=xterm-256color urlscan<Enter>" "call urlscan to
+extract URLs out of a message"`
+
 To choose a particular browser, set the environment variable BROWSER. If BROWSER
 is not set, xdg-open will control which browser is used, if it's available.:
 
     export BROWSER=/usr/bin/epiphany
 
 
 ## Command Line usage
@@ -196,10 +207,12 @@
 - multipart/alternative sections are handled by descending into all the
   sub-parts, rather than just picking one, which may lead to URLs and context
   appearing twice. (Bypass this by selecting the '--dedupe' option)
 
 ## Build/development
 
 - pyproject.toml is configured for [hatch][2] for building and submitting to pypi.
+- flake.nix is available for a development shell or building/testing the package
+  if desired. `nix develop`
 
 [1]: http://urwid.org/manual/displayattributes.html#display-attributes  "Urwid display attributes"
 [2]: https://hatch.pypa.io/latest/  "Hatch"
```

### Comparing `urlscan-1.0.1/pyproject.toml` & `urlscan-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "urlscan"
 dynamic = ["version"]
 description = "View/select the URLs in an email message or file"
 readme = "README.md"
-license = "GPL-2.0"
+license = "GPL-2.0-or-later"
 authors = [
     { name = "Scott Hansen", email = "tech@firecat53.net" },
 ]
 keywords = [
     "email",
     "mutt",
     "tmux",
@@ -26,14 +26,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Utilities",
 ]
 dependencies = [
     "urwid>=1.2.1",
 ]
 
 [project.scripts]
```

### Comparing `urlscan-1.0.1/PKG-INFO` & `urlscan-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: urlscan
-Version: 1.0.1
+Version: 1.0.2
 Summary: View/select the URLs in an email message or file
 Project-URL: Homepage, https://github.com/firecat53/urlscan
 Author-email: Scott Hansen <tech@firecat53.net>
-License-Expression: GPL-2.0
+License-Expression: GPL-2.0-or-later
 License-File: LICENSE
 Keywords: email,mutt,tmux,urlscan,urlview
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Console :: Curses
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: urwid>=1.2.1
 Description-Content-Type: text/markdown
 
 # Urlscan
 
+[![main](https://github.com/firecat53/urlscan/actions/workflows/main.yml/badge.svg)](https://github.com/firecat53/urlscan/actions/workflows/main.yml)
+
 ## Contributors
 
 Scott Hansen \<tech@firecat53.net\> (Author and Maintainer)
 
 Maxime Chatelle \<xakz@rxsoft.eu\> (Debian Maintainer)
 
 Daniel Burrows \<dburrows@debian.org\> (Original Author)
@@ -92,18 +95,18 @@
 - Queue multiple URLs for opening and open them all at once with `a` and `o`.
 
 ## Installation and setup
 
 To install urlscan, install from your distribution repositories, from Pypi, or do
 a local development install with pip -e:
 
-    pipx install urlscan 
-    
+    pipx install urlscan
+
     OR
-    
+
     pip install --user urlscan
 
     OR
 
     cd <path/to/urlscan> && pip install --user -e .
 
 **NOTE**
@@ -117,14 +120,23 @@
 
     macro attach,compose \cb "<pipe-entry> urlscan<Enter>" "call urlscan to
     extract URLs out of a message"
 
 Once this is done, Control-b while reading mail in mutt will automatically
 invoke urlscan on the message.
 
+> Note for Neomutt users: [As of version
+> `2023-05-17`](https://github.com/neomutt/neomutt/releases/tag/20230517) true
+> color support was implemented. If you are using true color support with Neomutt,
+> or are encountering the error `setupterm: could not find terminfo database`,
+> then you should also add `TERM=xterm-256color` to your macro in `.muttrc`.
+> See more here [#135](https://github.com/firecat53/urlscan/issues/135). For example:
+> `macro index,pager  \cb "<pipe-message>  TERM=xterm-256color urlscan<Enter>" "call urlscan to
+extract URLs out of a message"`
+
 To choose a particular browser, set the environment variable BROWSER. If BROWSER
 is not set, xdg-open will control which browser is used, if it's available.:
 
     export BROWSER=/usr/bin/epiphany
 
 
 ## Command Line usage
@@ -220,10 +232,12 @@
 - multipart/alternative sections are handled by descending into all the
   sub-parts, rather than just picking one, which may lead to URLs and context
   appearing twice. (Bypass this by selecting the '--dedupe' option)
 
 ## Build/development
 
 - pyproject.toml is configured for [hatch][2] for building and submitting to pypi.
+- flake.nix is available for a development shell or building/testing the package
+  if desired. `nix develop`
 
 [1]: http://urwid.org/manual/displayattributes.html#display-attributes  "Urwid display attributes"
 [2]: https://hatch.pypa.io/latest/  "Hatch"
```

