# Comparing `tmp/natter-0.0.1.tar.gz` & `tmp/natter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "natter-0.0.1.tar", last modified: Thu Apr 25 10:44:59 2024, max compression
+gzip compressed data, was "natter-0.0.2.tar", last modified: Mon Apr 29 13:54:02 2024, max compression
```

## Comparing `natter-0.0.1.tar` & `natter-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-25 10:44:59.556878 natter-0.0.1/
--rw-r--r--   0 davep      (501) staff       (20)     1527 2024-04-25 10:44:59.556804 natter-0.0.1/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      141 2024-04-25 10:37:26.000000 natter-0.0.1/README.md
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-25 10:44:59.555132 natter-0.0.1/natter/
--rw-r--r--   0 davep      (501) staff       (20)      492 2024-04-24 08:03:34.000000 natter-0.0.1/natter/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)      461 2024-04-24 16:49:29.000000 natter-0.0.1/natter/__main__.py
--rw-r--r--   0 davep      (501) staff       (20)      573 2024-04-24 16:49:29.000000 natter-0.0.1/natter/app.py
--rw-r--r--   0 davep      (501) staff       (20)        0 2024-04-24 08:03:55.000000 natter-0.0.1/natter/py.typed
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-25 10:44:59.556068 natter-0.0.1/natter/screens/
--rw-r--r--   0 davep      (501) staff       (20)      296 2024-04-24 08:08:42.000000 natter-0.0.1/natter/screens/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     3366 2024-04-25 10:26:23.000000 natter-0.0.1/natter/screens/main.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-25 10:44:59.556409 natter-0.0.1/natter/widgets/
--rw-r--r--   0 davep      (501) staff       (20)      377 2024-04-25 08:15:44.000000 natter-0.0.1/natter/widgets/__init__.py
--rw-r--r--   0 davep      (501) staff       (20)     1058 2024-04-25 08:18:49.000000 natter-0.0.1/natter/widgets/output.py
--rw-r--r--   0 davep      (501) staff       (20)     1361 2024-04-24 16:49:29.000000 natter-0.0.1/natter/widgets/user_input.py
-drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-25 10:44:59.556572 natter-0.0.1/natter.egg-info/
--rw-r--r--   0 davep      (501) staff       (20)     1527 2024-04-25 10:44:59.000000 natter-0.0.1/natter.egg-info/PKG-INFO
--rw-r--r--   0 davep      (501) staff       (20)      415 2024-04-25 10:44:59.000000 natter-0.0.1/natter.egg-info/SOURCES.txt
--rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-25 10:44:59.000000 natter-0.0.1/natter.egg-info/dependency_links.txt
--rw-r--r--   0 davep      (501) staff       (20)       47 2024-04-25 10:44:59.000000 natter-0.0.1/natter.egg-info/entry_points.txt
--rw-r--r--   0 davep      (501) staff       (20)       23 2024-04-25 10:44:59.000000 natter-0.0.1/natter.egg-info/requires.txt
--rw-r--r--   0 davep      (501) staff       (20)        7 2024-04-25 10:44:59.000000 natter-0.0.1/natter.egg-info/top_level.txt
--rw-r--r--   0 davep      (501) staff       (20)      124 2024-04-25 10:40:26.000000 natter-0.0.1/pyproject.toml
--rw-r--r--   0 davep      (501) staff       (20)     1476 2024-04-25 10:44:59.557162 natter-0.0.1/setup.cfg
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-29 13:54:02.852994 natter-0.0.2/
+-rw-r--r--   0 davep      (501) staff       (20)     1489 2024-04-29 13:54:02.852896 natter-0.0.2/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      141 2024-04-25 10:37:26.000000 natter-0.0.2/README.md
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-29 13:54:02.850931 natter-0.0.2/natter/
+-rw-r--r--   0 davep      (501) staff       (20)      492 2024-04-29 13:53:21.000000 natter-0.0.2/natter/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)      461 2024-04-24 16:49:29.000000 natter-0.0.2/natter/__main__.py
+-rw-r--r--   0 davep      (501) staff       (20)      609 2024-04-25 16:03:27.000000 natter-0.0.2/natter/app.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-29 13:54:02.851751 natter-0.0.2/natter/data/
+-rw-r--r--   0 davep      (501) staff       (20)      355 2024-04-26 14:02:09.000000 natter-0.0.2/natter/data/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     1250 2024-04-26 14:04:27.000000 natter-0.0.2/natter/data/locations.py
+-rw-r--r--   0 davep      (501) staff       (20)        0 2024-04-24 08:03:55.000000 natter-0.0.2/natter/py.typed
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-29 13:54:02.851958 natter-0.0.2/natter/screens/
+-rw-r--r--   0 davep      (501) staff       (20)      296 2024-04-24 08:08:42.000000 natter-0.0.2/natter/screens/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     6910 2024-04-29 11:00:26.000000 natter-0.0.2/natter/screens/main.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-29 13:54:02.852454 natter-0.0.2/natter/widgets/
+-rw-r--r--   0 davep      (501) staff       (20)      395 2024-04-29 09:51:10.000000 natter-0.0.2/natter/widgets/__init__.py
+-rw-r--r--   0 davep      (501) staff       (20)     3953 2024-04-29 10:51:56.000000 natter-0.0.2/natter/widgets/output.py
+-rw-r--r--   0 davep      (501) staff       (20)     1783 2024-04-29 09:55:27.000000 natter-0.0.2/natter/widgets/user_input.py
+drwxr-xr-x   0 davep      (501) staff       (20)        0 2024-04-29 13:54:02.852642 natter-0.0.2/natter.egg-info/
+-rw-r--r--   0 davep      (501) staff       (20)     1489 2024-04-29 13:54:02.000000 natter-0.0.2/natter.egg-info/PKG-INFO
+-rw-r--r--   0 davep      (501) staff       (20)      464 2024-04-29 13:54:02.000000 natter-0.0.2/natter.egg-info/SOURCES.txt
+-rw-r--r--   0 davep      (501) staff       (20)        1 2024-04-29 13:54:02.000000 natter-0.0.2/natter.egg-info/dependency_links.txt
+-rw-r--r--   0 davep      (501) staff       (20)       47 2024-04-29 13:54:02.000000 natter-0.0.2/natter.egg-info/entry_points.txt
+-rw-r--r--   0 davep      (501) staff       (20)       54 2024-04-29 13:54:02.000000 natter-0.0.2/natter.egg-info/requires.txt
+-rw-r--r--   0 davep      (501) staff       (20)        7 2024-04-29 13:54:02.000000 natter-0.0.2/natter.egg-info/top_level.txt
+-rw-r--r--   0 davep      (501) staff       (20)      124 2024-04-25 10:40:26.000000 natter-0.0.2/pyproject.toml
+-rw-r--r--   0 davep      (501) staff       (20)     1432 2024-04-29 13:54:02.853258 natter-0.0.2/setup.cfg
```

### Comparing `natter-0.0.1/PKG-INFO` & `natter-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natter
-Version: 0.0.1
+Version: 0.0.2
 Summary: A terminal-based ollama chat interface
 Home-page: https://github.com/davep/natter
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,26 +15,26 @@
 Keywords: terminal
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Terminals
 Classifier: Typing :: Typed
-Requires-Python: <3.13,>=3.8
+Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: textual>=0.48.2
 Requires-Dist: ollama
+Requires-Dist: xdg-base-dirs
+Requires-Dist: textual-fspicker
 
 # Natter
 
 A wee experimental terminal-based chat client, built to mess around with the
 Python Ollama library.
 
 [//]: # (README.md ends here)
```

### Comparing `natter-0.0.1/natter/app.py` & `natter-0.0.2/natter/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,13 +9,15 @@
 from .screens import Main
 
 
 ##############################################################################
 class Natter(App[None]):
     """The Natter application."""
 
+    ENABLE_COMMAND_PALETTE = False
+
     def on_mount(self) -> None:
         """Show the main screen once the app is mounted."""
         self.push_screen(Main())
 
 
 ### app.py ends here
```

### Comparing `natter-0.0.1/natter.egg-info/PKG-INFO` & `natter-0.0.2/natter.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: natter
-Version: 0.0.1
+Version: 0.0.2
 Summary: A terminal-based ollama chat interface
 Home-page: https://github.com/davep/natter
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -15,26 +15,26 @@
 Keywords: terminal
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Environment :: Console
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Terminals
 Classifier: Typing :: Typed
-Requires-Python: <3.13,>=3.8
+Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: textual>=0.48.2
 Requires-Dist: ollama
+Requires-Dist: xdg-base-dirs
+Requires-Dist: textual-fspicker
 
 # Natter
 
 A wee experimental terminal-based chat client, built to mess around with the
 Python Ollama library.
 
 [//]: # (README.md ends here)
```

### Comparing `natter-0.0.1/setup.cfg` & `natter-0.0.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Environment :: Console
 	Development Status :: 3 - Alpha
 	Intended Audience :: End Users/Desktop
 	Natural Language :: English
 	Operating System :: OS Independent
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3.12
 	Topic :: Internet
 	Topic :: Terminals
 	Typing :: Typed
 project_urls = 
@@ -33,18 +31,20 @@
 	Issues = https://github.com/davep/natter/issues
 	Discussions = https://github.com/davep/natter/discussions
 
 [options]
 packages = find:
 platforms = any
 include_package_data = True
-python_requires = >=3.8,<3.13
+python_requires = >=3.10,<3.13
 install_requires = 
 	textual>=0.48.2
 	ollama
+	xdg-base-dirs
+	textual-fspicker
 
 [options.entry_points]
 console_scripts = 
 	natter = natter.__main__:run
 
 [egg_info]
 tag_build =
```

