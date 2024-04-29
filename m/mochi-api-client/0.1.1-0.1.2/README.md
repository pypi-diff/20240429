# Comparing `tmp/mochi-api-client-0.1.1.tar.gz` & `tmp/mochi-api-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mochi-api-client-0.1.1.tar", last modified: Thu Feb 22 14:15:42 2024, max compression
+gzip compressed data, was "mochi-api-client-0.1.2.tar", last modified: Mon Apr 29 09:20:53 2024, max compression
```

## Comparing `mochi-api-client-0.1.1.tar` & `mochi-api-client-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 14:15:44.000000 mochi-api-client-0.1.1/
--rw-rw-rw-   0        0        0    11558 2024-02-22 11:05:44.000000 mochi-api-client-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2560 2024-02-22 14:15:44.000000 mochi-api-client-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1706 2024-02-22 12:25:18.000000 mochi-api-client-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-22 14:15:44.000000 mochi-api-client-0.1.1/mochi/
--rw-rw-rw-   0        0        0        0 2024-02-22 11:06:34.000000 mochi-api-client-0.1.1/mochi/__init__.py
--rw-rw-rw-   0        0        0      468 2024-02-22 11:06:34.000000 mochi-api-client-0.1.1/mochi/auth.py
--rw-rw-rw-   0        0        0     5480 2024-02-22 14:13:28.000000 mochi-api-client-0.1.1/mochi/cards.py
--rw-rw-rw-   0        0        0      586 2024-02-22 11:06:34.000000 mochi-api-client-0.1.1/mochi/client.py
--rw-rw-rw-   0        0        0     2346 2024-02-22 14:13:18.000000 mochi-api-client-0.1.1/mochi/decks.py
--rw-rw-rw-   0        0        0     1074 2024-02-22 13:43:04.000000 mochi-api-client-0.1.1/mochi/models.py
--rw-rw-rw-   0        0        0     1141 2024-02-22 14:14:00.000000 mochi-api-client-0.1.1/mochi/template.py
-drwxrwxrwx   0        0        0        0 2024-02-22 14:15:44.000000 mochi-api-client-0.1.1/mochi_api_client.egg-info/
--rw-rw-rw-   0        0        0     2560 2024-02-22 14:15:42.000000 mochi-api-client-0.1.1/mochi_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2024-02-22 14:15:44.000000 mochi-api-client-0.1.1/mochi_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 14:15:42.000000 mochi-api-client-0.1.1/mochi_api_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-02-22 14:15:44.000000 mochi-api-client-0.1.1/mochi_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-22 14:15:44.000000 mochi-api-client-0.1.1/mochi_api_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-22 11:06:34.000000 mochi-api-client-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-22 14:15:44.000000 mochi-api-client-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1618 2024-02-22 14:14:58.000000 mochi-api-client-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2024-02-22 11:05:44.000000 mochi-api-client-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2560 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1706 2024-02-22 12:25:18.000000 mochi-api-client-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/mochi/
+-rw-rw-rw-   0        0        0        0 2024-02-22 11:06:34.000000 mochi-api-client-0.1.2/mochi/__init__.py
+-rw-rw-rw-   0        0        0      468 2024-02-22 11:06:34.000000 mochi-api-client-0.1.2/mochi/auth.py
+-rw-rw-rw-   0        0        0     5627 2024-02-24 17:17:02.000000 mochi-api-client-0.1.2/mochi/cards.py
+-rw-rw-rw-   0        0        0      586 2024-02-22 11:06:34.000000 mochi-api-client-0.1.2/mochi/client.py
+-rw-rw-rw-   0        0        0     2493 2024-04-18 09:26:02.000000 mochi-api-client-0.1.2/mochi/decks.py
+-rw-rw-rw-   0        0        0     1074 2024-02-22 13:43:04.000000 mochi-api-client-0.1.2/mochi/models.py
+-rw-rw-rw-   0        0        0     1141 2024-02-22 14:14:00.000000 mochi-api-client-0.1.2/mochi/template.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/mochi_api_client.egg-info/
+-rw-rw-rw-   0        0        0     2560 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/mochi_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/mochi_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/mochi_api_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/mochi_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/mochi_api_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-22 11:06:34.000000 mochi-api-client-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1618 2024-04-29 09:10:58.000000 mochi-api-client-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:20:54.000000 mochi-api-client-0.1.2/tests/
+-rw-rw-rw-   0        0        0     2358 2024-02-22 16:10:46.000000 mochi-api-client-0.1.2/tests/test_cards.py
+-rw-rw-rw-   0        0        0       92 2024-02-22 13:21:04.000000 mochi-api-client-0.1.2/tests/test_decks.py
+-rw-rw-rw-   0        0        0        0 2024-02-22 13:20:18.000000 mochi-api-client-0.1.2/tests/test_templates.py
```

### Comparing `mochi-api-client-0.1.1/LICENSE` & `mochi-api-client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mochi-api-client-0.1.1/PKG-INFO` & `mochi-api-client-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mochi-api-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python client for interacting with the Mochi API.
 Home-page: https://github.com/gsejas/mochi-api-client
 Author: Jorge Sequeira
 Author-email: jsequeira03@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `mochi-api-client-0.1.1/README.md` & `mochi-api-client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mochi-api-client-0.1.1/mochi/cards.py` & `mochi-api-client-0.1.2/mochi/cards.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,19 +46,21 @@
         :param content: _description_
         :type content: _type_
         :param deck_id: _description_
         :type deck_id: _type_
         :return: _description_
         :rtype: _type_
         """
+        # Convert underscores to hyphens in kwargs keys
+        kwargs_converted = {k.replace("_", "-"): v for k, v in kwargs.items()}
         # Combine required parameters with any additional keyword arguments
         payload = {
             "content": content,
             "deck-id": deck_id,
-            **kwargs,  # This adds the optional parameters to the payload
+            **kwargs_converted,  # This adds the optional parameters to the payload
         }
         response = self.session.post(self.base_url, json=payload)
         response.raise_for_status()
         return response.json()
 
     def get_card(self, card_id):
         """_summary_
```

### Comparing `mochi-api-client-0.1.1/mochi/client.py` & `mochi-api-client-0.1.2/mochi/client.py`

 * *Files identical despite different names*

### Comparing `mochi-api-client-0.1.1/mochi/decks.py` & `mochi-api-client-0.1.2/mochi/decks.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,20 @@
             "archived?": true,
             "trashed?": "2012-04-23T18:25:43.511Z",
             "show-sides?": true,
             "sort-by-direction": true,
             "review-reverse?": true
         }
         """
+        # Convert underscores to hyphens in kwargs keys
+        kwargs_converted = {k.replace("_", "-"): v for k, v in kwargs.items()}
         # Combine required parameters with any additional keyword arguments
         payload = {
             "name": name,
-            **kwargs,  # This adds the optional parameters to the payload
+            **kwargs_converted,  # This adds the optional parameters to the payload
         }
         response = self.session.post(self.base_url, json=payload)
         response.raise_for_status()
         return response.json()
 
     def get_deck(self, deck_id):
         """Retrieves a deck that already exists. The returned data will look identical to the data returned from the deck creation request.
```

### Comparing `mochi-api-client-0.1.1/mochi/models.py` & `mochi-api-client-0.1.2/mochi/models.py`

 * *Files identical despite different names*

### Comparing `mochi-api-client-0.1.1/mochi/template.py` & `mochi-api-client-0.1.2/mochi/template.py`

 * *Files identical despite different names*

### Comparing `mochi-api-client-0.1.1/mochi_api_client.egg-info/PKG-INFO` & `mochi-api-client-0.1.2/mochi_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mochi-api-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python client for interacting with the Mochi API.
 Home-page: https://github.com/gsejas/mochi-api-client
 Author: Jorge Sequeira
 Author-email: jsequeira03@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `mochi-api-client-0.1.1/setup.py` & `mochi-api-client-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mochi-api-client",  # Name of your package
-    version="0.1.1",  # Initial release version
+    version="0.1.2",  # Initial release version
     author="Jorge Sequeira",  # Your name or your organization's name
     author_email="jsequeira03@gmail.com",  # Your contact email
     description="A Python client for interacting with the Mochi API.",  # A short description of the project
     long_description=open("README.md").read(),  # A long description from your README.md
     long_description_content_type="text/markdown",  # Specifies that the long description is in Markdown
     url="https://github.com/gsejas/mochi-api-client",  # Project home page or repository URL
     packages=find_packages(),  # Automatically find and include all packages in the project
```

