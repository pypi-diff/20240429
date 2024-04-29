# Comparing `tmp/typeahead-0.0.3.tar.gz` & `tmp/typeahead-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeahead-0.0.3.tar", last modified: Mon Apr 29 15:19:39 2024, max compression
+gzip compressed data, was "typeahead-0.0.4.tar", last modified: Mon Apr 29 15:54:30 2024, max compression
```

## Comparing `typeahead-0.0.3.tar` & `typeahead-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:19:39.455265 typeahead-0.0.3/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 15:19:39.451752 typeahead-0.0.3/PKG-INFO
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       38 2024-04-29 15:19:39.456265 typeahead-0.0.3/setup.cfg
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      725 2024-04-29 15:19:31.000000 typeahead-0.0.3/setup.py
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:19:39.333260 typeahead-0.0.3/typeahead/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       35 2024-04-29 15:19:06.000000 typeahead-0.0.3/typeahead/__init__.py
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)     3376 2024-01-19 11:27:49.000000 typeahead-0.0.3/typeahead/auto_complete.py
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:19:39.426569 typeahead-0.0.3/typeahead.egg-info/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 15:19:39.000000 typeahead-0.0.3/typeahead.egg-info/PKG-INFO
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      189 2024-04-29 15:19:39.000000 typeahead-0.0.3/typeahead.egg-info/SOURCES.txt
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        1 2024-04-29 15:19:39.000000 typeahead-0.0.3/typeahead.egg-info/dependency_links.txt
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       10 2024-04-29 15:19:39.000000 typeahead-0.0.3/typeahead.egg-info/top_level.txt
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:54:30.213531 typeahead-0.0.4/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 15:54:30.209188 typeahead-0.0.4/PKG-INFO
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       38 2024-04-29 15:54:30.215088 typeahead-0.0.4/setup.cfg
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      725 2024-04-29 15:54:26.000000 typeahead-0.0.4/setup.py
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:54:30.050862 typeahead-0.0.4/typeahead/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       35 2024-04-29 15:54:20.000000 typeahead-0.0.4/typeahead/__init__.py
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)     3315 2024-04-29 15:53:31.000000 typeahead-0.0.4/typeahead/auto_complete.py
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 15:54:30.172185 typeahead-0.0.4/typeahead.egg-info/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 15:54:29.000000 typeahead-0.0.4/typeahead.egg-info/PKG-INFO
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      189 2024-04-29 15:54:29.000000 typeahead-0.0.4/typeahead.egg-info/SOURCES.txt
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        1 2024-04-29 15:54:29.000000 typeahead-0.0.4/typeahead.egg-info/dependency_links.txt
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       10 2024-04-29 15:54:29.000000 typeahead-0.0.4/typeahead.egg-info/top_level.txt
```

### Comparing `typeahead-0.0.3/PKG-INFO` & `typeahead-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeahead
-Version: 0.0.3
+Version: 0.0.4
 Summary: Typeahead feature
 Home-page: UNKNOWN
 Author: techy_cereal 
 Author-email: alexanderjmilliken@gmail.com
 License: UNKNOWN
 Keywords: python,typeahead,auto complete
 Platform: UNKNOWN
```

### Comparing `typeahead-0.0.3/setup.py` & `typeahead-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Typeahead feature'
 
 # Setting up
 setup(
     name="typeahead",
     version=VERSION,
     author="techy_cereal ",
```

### Comparing `typeahead-0.0.3/typeahead/auto_complete.py` & `typeahead-0.0.4/typeahead/auto_complete.py`

 * *Files 13% similar despite different names*

```diff
@@ -92,16 +92,16 @@
     Args:
         msg (str): The message to complete.
 
     Returns:
         list: A list of possible completions for the message.
     """
     return trie.find_completions(msg)
+
+with open('words.txt', 'r') as file:
+	words = file.readlines()
+
 trie = Trie()
-trie.insert_string("hello")
-trie.insert_string("helium")
-trie.insert_string("help")
-trie.insert_string("helicopter")
-trie.insert_string("health")
-trie.insert_string("hat")
-trie.insert_string("at")
-trie.insert_string("ate")
+
+for word in words:
+	word = word.strip().lower()  # Preprocess the word
+	trie.insert_string(word)
```

### Comparing `typeahead-0.0.3/typeahead.egg-info/PKG-INFO` & `typeahead-0.0.4/typeahead.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeahead
-Version: 0.0.3
+Version: 0.0.4
 Summary: Typeahead feature
 Home-page: UNKNOWN
 Author: techy_cereal 
 Author-email: alexanderjmilliken@gmail.com
 License: UNKNOWN
 Keywords: python,typeahead,auto complete
 Platform: UNKNOWN
```

