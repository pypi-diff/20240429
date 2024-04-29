# Comparing `tmp/templated_setup-0.5.tar.gz` & `tmp/templated_setup-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.5.tar", last modified: Mon Apr 29 09:28:57 2024, max compression
+gzip compressed data, was "templated_setup-0.6.tar", last modified: Mon Apr 29 09:35:15 2024, max compression
```

## Comparing `templated_setup-0.5.tar` & `templated_setup-0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 09:28:57.873164 templated_setup-0.5/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.5/LICENCE
--rw-rw-rw-   0        0        0     2557 2024-04-29 09:28:57.872145 templated_setup-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 09:28:57.873164 templated_setup-0.5/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-04-29 08:45:00.000000 templated_setup-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 09:28:57.867465 templated_setup-0.5/templated_setup/
--rw-rw-rw-   0        0        0    17714 2024-04-29 09:28:39.000000 templated_setup-0.5/templated_setup/__init__.py
--rw-rw-rw-   0        0        0      170 2024-04-29 08:48:05.000000 templated_setup-0.5/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-04-29 09:28:57.872145 templated_setup-0.5/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2557 2024-04-29 09:28:57.000000 templated_setup-0.5/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-04-29 09:28:57.000000 templated_setup-0.5/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 09:28:57.000000 templated_setup-0.5/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 09:28:57.000000 templated_setup-0.5/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 09:35:15.960331 templated_setup-0.6/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.6/LICENCE
+-rw-rw-rw-   0        0        0     2557 2024-04-29 09:35:15.959789 templated_setup-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 09:35:15.961345 templated_setup-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-04-29 08:45:00.000000 templated_setup-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:35:15.954191 templated_setup-0.6/templated_setup/
+-rw-rw-rw-   0        0        0    17713 2024-04-29 09:31:01.000000 templated_setup-0.6/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0      170 2024-04-29 08:48:05.000000 templated_setup-0.6/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:35:15.959282 templated_setup-0.6/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2557 2024-04-29 09:35:15.000000 templated_setup-0.6/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-29 09:35:15.000000 templated_setup-0.6/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 09:35:15.000000 templated_setup-0.6/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 09:35:15.000000 templated_setup-0.6/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.5/LICENCE` & `templated_setup-0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.5/PKG-INFO` & `templated_setup-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.5
+Version: 0.6
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Standardized `setup.py`
@@ -65,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.5 released on 29th/4/2024
+## V0.6 released on 29th/4/2024
 hopefully can be installed via pip now. ;p
```

### Comparing `templated_setup-0.5/README.md` & `templated_setup-0.6/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.5/templated_setup/__init__.py` & `templated_setup-0.6/templated_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -416,26 +416,26 @@
 
 		f"[ END ] {Setup_Helper.__inner_load_readme_file_path}"
 
 
 
 	@classmethod
 	def __load_parameters(cls):
+		cls._load_from_hardcoded()
 		if cls._is_using_pip:
 			json_data = cls._json_data_when_using_pip
 			assert json_data is not None
 			cls._date_of_last_modified = datetime_x_date.fromisoformat(json_data["date"])
 			cls._version_number = json_data["version_number"]
 			cls._notes = json_data["notes"]
 			cls._readme_file_path = json_data["readme_file_path"]
 			return
 		user_wants_to_change_params = False
 		while True:
 
-			cls._load_from_hardcoded()
 
 			cls.__clear_screen()
 			print(f"\n\n] Current Infos:")
 			print(f"]] Date:              [{cls._date_of_last_modified}]")
 			print(f"]] Version Number:    [{cls._version_number}]")
 			print(f"]] Notes:             [{cls._notes}]")
 			print(f"]] Readme File Path:  [{cls._readme_file_path}]")
```

### Comparing `templated_setup-0.5/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.6/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.5
+Version: 0.6
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENCE
 
 # Standardized `setup.py`
@@ -65,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.5 released on 29th/4/2024
+## V0.6 released on 29th/4/2024
 hopefully can be installed via pip now. ;p
```

