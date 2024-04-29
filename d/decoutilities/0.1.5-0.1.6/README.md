# Comparing `tmp/decoutilities-0.1.5.tar.gz` & `tmp/decoutilities-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.1.5.tar", last modified: Mon Apr 29 10:48:12 2024, max compression
+gzip compressed data, was "decoutilities-0.1.6.tar", last modified: Mon Apr 29 10:58:47 2024, max compression
```

## Comparing `decoutilities-0.1.5.tar` & `decoutilities-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:48:12.490532 decoutilities-0.1.5/
--rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     3053 2024-04-29 10:48:12.472532 decoutilities-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2631 2024-04-26 14:17:02.000000 decoutilities-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 10:48:12.297532 decoutilities-0.1.5/decoutilities/
--rw-rw-rw-   0        0        0      809 2024-04-29 10:39:04.000000 decoutilities-0.1.5/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:48:12.419532 decoutilities-0.1.5/decoutilities/config/
--rw-rw-rw-   0        0        0       43 2024-04-29 10:47:46.000000 decoutilities-0.1.5/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.5/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.5/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:48:12.450531 decoutilities-0.1.5/decoutilities.egg-info/
--rw-rw-rw-   0        0        0     3053 2024-04-29 10:48:11.000000 decoutilities-0.1.5/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-29 10:48:11.000000 decoutilities-0.1.5/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:48:11.000000 decoutilities-0.1.5/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-29 10:48:11.000000 decoutilities-0.1.5/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 10:48:12.491531 decoutilities-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      680 2024-04-29 10:48:04.000000 decoutilities-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:58:47.155481 decoutilities-0.1.6/
+-rw-rw-rw-   0        0        0     1089 2024-04-26 12:51:10.000000 decoutilities-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     3116 2024-04-29 10:58:47.138488 decoutilities-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2645 2024-04-29 10:51:04.000000 decoutilities-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 10:58:46.938480 decoutilities-0.1.6/decoutilities/
+-rw-rw-rw-   0        0        0      428 2024-04-29 10:52:56.000000 decoutilities-0.1.6/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:58:47.090484 decoutilities-0.1.6/decoutilities/config/
+-rw-rw-rw-   0        0        0       76 2024-04-29 10:57:10.000000 decoutilities-0.1.6/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.1.6/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     4322 2024-04-26 08:53:27.000000 decoutilities-0.1.6/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:58:47.122482 decoutilities-0.1.6/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0     3116 2024-04-29 10:58:46.000000 decoutilities-0.1.6/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-04-29 10:58:46.000000 decoutilities-0.1.6/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:58:46.000000 decoutilities-0.1.6/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-29 10:58:46.000000 decoutilities-0.1.6/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:58:47.156481 decoutilities-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-04-29 10:58:03.000000 decoutilities-0.1.6/setup.py
```

### Comparing `decoutilities-0.1.5/LICENSE` & `decoutilities-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.5/PKG-INFO` & `decoutilities-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.5
-Summary: Enhance the readability of your code with decorators.
+Version: 0.1.6
+Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -61,15 +61,15 @@
 `decoutilities` provides a complex config system that allows you to easily manage configuration settings using decorators.
 
 #### configContainer
 
 The `configContainer` class is responsible for loading and saving configuration data from/to JSON or YAML files.
 
 ```python
-from decoutilities import configContainer
+from decoutilities.config import configContainer
 
 # Create a configContainer instance
 config_container = configContainer(path="config", filename="settings", type="json")
 
 # Register values
 config_container.registerValues({
     "api_key": "your_api_key",
@@ -84,15 +84,15 @@
 ```
 
 #### config
 
 The `config` class works in conjunction with `configContainer` to provide a decorator-based approach for registering settings.
 
 ```python
-from decoutilities import config, configContainer
+from decoutilities.config import config, configContainer
 
 # Create a configContainer instance
 config_container = configContainer(path="config", filename="settings", type="json")
 
 # Create a config instance
 config_instance = config(config_container)
```

### Comparing `decoutilities-0.1.5/README.md` & `decoutilities-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 `decoutilities` provides a complex config system that allows you to easily manage configuration settings using decorators.
 
 #### configContainer
 
 The `configContainer` class is responsible for loading and saving configuration data from/to JSON or YAML files.
 
 ```python
-from decoutilities import configContainer
+from decoutilities.config import configContainer
 
 # Create a configContainer instance
 config_container = configContainer(path="config", filename="settings", type="json")
 
 # Register values
 config_container.registerValues({
     "api_key": "your_api_key",
@@ -71,15 +71,15 @@
 ```
 
 #### config
 
 The `config` class works in conjunction with `configContainer` to provide a decorator-based approach for registering settings.
 
 ```python
-from decoutilities import config, configContainer
+from decoutilities.config import config, configContainer
 
 # Create a configContainer instance
 config_container = configContainer(path="config", filename="settings", type="json")
 
 # Create a config instance
 config_instance = config(config_container)
```

### Comparing `decoutilities-0.1.5/decoutilities/config/config.py` & `decoutilities-0.1.6/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.5/decoutilities/config/configContainer.py` & `decoutilities-0.1.6/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.1.5/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.1.6/decoutilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.1.5
-Summary: Enhance the readability of your code with decorators.
+Version: 0.1.6
+Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -61,15 +61,15 @@
 `decoutilities` provides a complex config system that allows you to easily manage configuration settings using decorators.
 
 #### configContainer
 
 The `configContainer` class is responsible for loading and saving configuration data from/to JSON or YAML files.
 
 ```python
-from decoutilities import configContainer
+from decoutilities.config import configContainer
 
 # Create a configContainer instance
 config_container = configContainer(path="config", filename="settings", type="json")
 
 # Register values
 config_container.registerValues({
     "api_key": "your_api_key",
@@ -84,15 +84,15 @@
 ```
 
 #### config
 
 The `config` class works in conjunction with `configContainer` to provide a decorator-based approach for registering settings.
 
 ```python
-from decoutilities import config, configContainer
+from decoutilities.config import config, configContainer
 
 # Create a configContainer instance
 config_container = configContainer(path="config", filename="settings", type="json")
 
 # Create a config instance
 config_instance = config(config_container)
```

