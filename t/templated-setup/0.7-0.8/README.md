# Comparing `tmp/templated_setup-0.7.tar.gz` & `tmp/templated_setup-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.7.tar", last modified: Mon Apr 29 09:47:01 2024, max compression
+gzip compressed data, was "templated_setup-0.8.tar", last modified: Mon Apr 29 10:01:56 2024, max compression
```

## Comparing `templated_setup-0.7.tar` & `templated_setup-0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 09:47:01.398523 templated_setup-0.7/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.7/LICENCE
--rw-rw-rw-   0        0        0     2563 2024-04-29 09:47:01.397319 templated_setup-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 09:47:01.398523 templated_setup-0.7/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-04-29 08:45:00.000000 templated_setup-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 09:47:01.391717 templated_setup-0.7/templated_setup/
--rw-rw-rw-   0        0        0    17793 2024-04-29 09:46:49.000000 templated_setup-0.7/templated_setup/__init__.py
--rw-rw-rw-   0        0        0      176 2024-04-29 09:45:58.000000 templated_setup-0.7/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-04-29 09:47:01.396303 templated_setup-0.7/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2563 2024-04-29 09:47:01.000000 templated_setup-0.7/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-04-29 09:47:01.000000 templated_setup-0.7/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 09:47:01.000000 templated_setup-0.7/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 09:47:01.000000 templated_setup-0.7/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 10:01:56.998884 templated_setup-0.8/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.8/LICENCE
+-rw-rw-rw-   0        0        0     2564 2024-04-29 10:01:56.997838 templated_setup-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:01:56.998884 templated_setup-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-04-29 08:45:00.000000 templated_setup-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:01:56.992205 templated_setup-0.8/templated_setup/
+-rw-rw-rw-   0        0        0    18216 2024-04-29 10:00:40.000000 templated_setup-0.8/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0      177 2024-04-29 10:01:40.000000 templated_setup-0.8/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:01:56.997331 templated_setup-0.8/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2564 2024-04-29 10:01:56.000000 templated_setup-0.8/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-29 10:01:56.000000 templated_setup-0.8/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:01:56.000000 templated_setup-0.8/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 10:01:56.000000 templated_setup-0.8/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.7/LICENCE` & `templated_setup-0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.7/PKG-INFO` & `templated_setup-0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.7
+Version: 0.8
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
 
-## V0.7 released on 29th/4/2024
-hopefully we be able to install from pip now. ;p
+## V0.8 released on 29th/4/2024
+hopefully we will be able to install from pip. :p
```

### Comparing `templated_setup-0.7/README.md` & `templated_setup-0.8/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.7/templated_setup/__init__.py` & `templated_setup-0.8/templated_setup/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,32 +207,46 @@
 
 		return None
 		f"[ END ] {Setup_Helper.__get_y_n}"
 
 
 
 	@classmethod
-	def __reload_cached_data(cls):
+	def __inner_reload_cached_data(cls):
 
 		try:
 			with open(CACHE_FILE_PATH, "r") as f:
 				json_data = json_x_load(f)
 		except FileNotFoundError:
-			with open(CACHE_FILE_PATH, "w") as f:
-				json_x_dump({}, f)
-			with open(CACHE_FILE_PATH, "r") as f:
-				json_data = json_x_load(f)
+			if len(cls._json_data.keys()) == 0:
+				if cls._is_using_pip:
+					return
+				with open(CACHE_FILE_PATH, "w") as f:
+					json_x_dump({}, f)
+				with open(CACHE_FILE_PATH, "r") as f:
+					json_data = json_x_load(f)
+			else:
+				raise FileNotFoundError(f"File [{CACHE_FILE_PATH}] not found.")
 
 		cls._json_data = json_data
 
 		return None
 
 		f"[ END ] {Setup_Helper.__reload_cached_data}"
 
 
+	
+	@classmethod
+	def __reload_cached_data(cls):
+		cls.__inner_reload_cached_data()
+		cls._load_from_hardcoded()
+		return None
+		f"[ END ] {Setup_Helper.__reload_cached_data}"
+
+
 
 	@classmethod
 	def __load_date(cls, override=False):
 
 		cls.__reload_cached_data()
 
 		if not override:
@@ -418,15 +432,15 @@
 
 		f"[ END ] {Setup_Helper.__inner_load_readme_file_path}"
 
 
 
 	@classmethod
 	def __load_parameters(cls):
-		cls._load_from_hardcoded()
+		cls.__inner_reload_cached_data()
 		if cls._is_using_pip:
 			json_data = cls._json_data_when_using_pip
 			assert json_data is not None
 			cls._date_of_last_modified = datetime_x_date.fromisoformat(json_data["date"])
 			cls._version_number = json_data["version_number"]
 			cls._notes = json_data["notes"]
 			cls._readme_file_path = json_data["readme_file_path"]
@@ -478,15 +492,14 @@
 				break
 			else:
 				user_wants_to_change_params = True
 				print("] Error: Please enter the information again.")
 				time_x_sleep(0.8)
 				cls.__clear_screen()
 
-		cls._load_from_hardcoded()
 		return None
 	
 		f"[ END ] {Setup_Helper.__load_parameters}"
 
 
 
 	@staticmethod
@@ -535,28 +548,29 @@
 	@classmethod
 	def _load_from_hardcoded(cls):
 
 		cls._is_using_pip = False
 		if "PIP_BUILD_TRACKER" in os.environ.keys():
 			cls._is_using_pip = True
 
-		cls.__reload_cached_data()
-		json_data = cls._json_data
+		cls._json_data = None
+		cls.__inner_reload_cached_data()
+		json_data = {} if not cls._json_data else cls._json_data
 		needs_update = False
 
 		# Before uploading to PyPi, we need to hardcode the values in a source file.
 		from . import _hardcoded
 		with open(_hardcoded.__file__, "r") as f:
 			contents = f.read()
 			splitted = contents.split("\n")[1:-2]
 			json_str = "\n".join(splitted)
 			j_data = json_x_loads(json_str)
 			if j_data != json_data:
 				needs_update = True
-		if needs_update:
+		if needs_update and len(json_data.keys()) == 4:
 			with open(_hardcoded.__file__, "w") as f:
 				json_str = json_x_dumps(json_data, indent=4)
 				f.write(f"\"\"\"\n{json_str}\n\"\"\"\n")
 		with open(_hardcoded.__file__, "r") as f:
 			contents = f.read()
 			splitted = contents.split("\n")[1:-2]
 			json_str = "\n".join(splitted)
```

### Comparing `templated_setup-0.7/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.8/templated_setup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.7
+Version: 0.8
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
 
-## V0.7 released on 29th/4/2024
-hopefully we be able to install from pip now. ;p
+## V0.8 released on 29th/4/2024
+hopefully we will be able to install from pip. :p
```

