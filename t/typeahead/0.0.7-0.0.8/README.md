# Comparing `tmp/typeahead-0.0.7.tar.gz` & `tmp/typeahead-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeahead-0.0.7.tar", last modified: Mon Apr 29 20:18:23 2024, max compression
+gzip compressed data, was "typeahead-0.0.8.tar", last modified: Mon Apr 29 20:19:57 2024, max compression
```

## Comparing `typeahead-0.0.7.tar` & `typeahead-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 20:18:23.131121 typeahead-0.0.7/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 20:18:23.127120 typeahead-0.0.7/PKG-INFO
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       38 2024-04-29 20:18:23.133120 typeahead-0.0.7/setup.cfg
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      784 2024-04-29 20:12:59.000000 typeahead-0.0.7/setup.py
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 20:18:23.011077 typeahead-0.0.7/typeahead/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       35 2024-04-29 15:54:20.000000 typeahead-0.0.7/typeahead/__init__.py
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)     3317 2024-04-29 20:14:09.000000 typeahead-0.0.7/typeahead/auto_complete.py
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)    75152 2024-04-29 15:52:43.000000 typeahead-0.0.7/typeahead/words.txt
-drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 20:18:23.102961 typeahead-0.0.7/typeahead.egg-info/
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 20:18:22.000000 typeahead-0.0.7/typeahead.egg-info/PKG-INFO
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      209 2024-04-29 20:18:22.000000 typeahead-0.0.7/typeahead.egg-info/SOURCES.txt
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        1 2024-04-29 20:18:22.000000 typeahead-0.0.7/typeahead.egg-info/dependency_links.txt
--rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       10 2024-04-29 20:18:22.000000 typeahead-0.0.7/typeahead.egg-info/top_level.txt
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 20:19:56.640454 typeahead-0.0.8/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 20:19:56.637456 typeahead-0.0.8/PKG-INFO
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       38 2024-04-29 20:19:56.641480 typeahead-0.0.8/setup.cfg
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      784 2024-04-29 20:19:34.000000 typeahead-0.0.8/setup.py
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 20:19:56.518621 typeahead-0.0.8/typeahead/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       35 2024-04-29 15:54:20.000000 typeahead-0.0.8/typeahead/__init__.py
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)     3515 2024-04-29 20:19:22.000000 typeahead-0.0.8/typeahead/auto_complete.py
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)    75152 2024-04-29 15:52:43.000000 typeahead-0.0.8/typeahead/words.txt
+drwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        0 2024-04-29 20:19:56.612927 typeahead-0.0.8/typeahead.egg-info/
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      568 2024-04-29 20:19:56.000000 typeahead-0.0.8/typeahead.egg-info/PKG-INFO
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)      209 2024-04-29 20:19:56.000000 typeahead-0.0.8/typeahead.egg-info/SOURCES.txt
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)        1 2024-04-29 20:19:56.000000 typeahead-0.0.8/typeahead.egg-info/dependency_links.txt
+-rwxrwxrwx   0 techycereal  (1000) techycereal  (1000)       10 2024-04-29 20:19:56.000000 typeahead-0.0.8/typeahead.egg-info/top_level.txt
```

### Comparing `typeahead-0.0.7/PKG-INFO` & `typeahead-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeahead
-Version: 0.0.7
+Version: 0.0.8
 Summary: Typeahead feature
 Home-page: UNKNOWN
 Author: techy_cereal 
 Author-email: alexanderjmilliken@gmail.com
 License: UNKNOWN
 Keywords: python,typeahead,auto complete
 Platform: UNKNOWN
```

### Comparing `typeahead-0.0.7/setup.py` & `typeahead-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Typeahead feature'
 
 # Setting up
 setup(
     name="typeahead",
     version=VERSION,
     author="techy_cereal ",
```

### Comparing `typeahead-0.0.7/typeahead/auto_complete.py` & `typeahead-0.0.8/typeahead/auto_complete.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import urllib.request
 class TrieNode:
     """A node in the trie structure."""
 
     def __init__(self):
         """Initialize the TrieNode with a children dictionary and an end-of-string flag."""
         self.children = {}  # Dictionary to store child nodes
         self.end_of_string = False  # Flag to indicate the end of a word
@@ -93,15 +94,22 @@
         msg (str): The message to complete.
 
     Returns:
         list: A list of possible completions for the message.
     """
     return trie.find_completions(msg)
 
-with open('./words.txt', 'r') as file:
-	words = file.readlines()
+
+
+url = "https://github.com/techycereal/autocompletion/blob/main/server-side/typeahead/words.txt"
+
+with urllib.request.urlopen(url) as file:
+	words = file.read().decode('utf-8').splitlines()
+
+# Now you can use the list of words
+print(words)
 
 trie = Trie()
 
 for word in words:
 	word = word.strip().lower()  # Preprocess the word
 	trie.insert_string(word)
```

### Comparing `typeahead-0.0.7/typeahead/words.txt` & `typeahead-0.0.8/typeahead/words.txt`

 * *Files identical despite different names*

### Comparing `typeahead-0.0.7/typeahead.egg-info/PKG-INFO` & `typeahead-0.0.8/typeahead.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeahead
-Version: 0.0.7
+Version: 0.0.8
 Summary: Typeahead feature
 Home-page: UNKNOWN
 Author: techy_cereal 
 Author-email: alexanderjmilliken@gmail.com
 License: UNKNOWN
 Keywords: python,typeahead,auto complete
 Platform: UNKNOWN
```

