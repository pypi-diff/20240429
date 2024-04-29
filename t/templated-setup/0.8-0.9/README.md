# Comparing `tmp/templated_setup-0.8.tar.gz` & `tmp/templated_setup-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.8.tar", last modified: Mon Apr 29 10:01:56 2024, max compression
+gzip compressed data, was "templated_setup-0.9.tar", last modified: Mon Apr 29 10:15:58 2024, max compression
```

## Comparing `templated_setup-0.8.tar` & `templated_setup-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 10:01:56.998884 templated_setup-0.8/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.8/LICENCE
--rw-rw-rw-   0        0        0     2564 2024-04-29 10:01:56.997838 templated_setup-0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 10:01:56.998884 templated_setup-0.8/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-04-29 08:45:00.000000 templated_setup-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:01:56.992205 templated_setup-0.8/templated_setup/
--rw-rw-rw-   0        0        0    18216 2024-04-29 10:00:40.000000 templated_setup-0.8/templated_setup/__init__.py
--rw-rw-rw-   0        0        0      177 2024-04-29 10:01:40.000000 templated_setup-0.8/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-04-29 10:01:56.997331 templated_setup-0.8/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2564 2024-04-29 10:01:56.000000 templated_setup-0.8/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-04-29 10:01:56.000000 templated_setup-0.8/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 10:01:56.000000 templated_setup-0.8/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 10:01:56.000000 templated_setup-0.8/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 10:15:58.017963 templated_setup-0.9/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.9/LICENCE
+-rw-rw-rw-   0        0        0     2564 2024-04-29 10:15:58.017963 templated_setup-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:15:58.018988 templated_setup-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-04-29 08:45:00.000000 templated_setup-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:15:58.012397 templated_setup-0.9/templated_setup/
+-rw-rw-rw-   0        0        0    18463 2024-04-29 10:14:53.000000 templated_setup-0.9/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0      177 2024-04-29 10:15:44.000000 templated_setup-0.9/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:15:58.016948 templated_setup-0.9/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2564 2024-04-29 10:15:57.000000 templated_setup-0.9/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-29 10:15:57.000000 templated_setup-0.9/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:15:57.000000 templated_setup-0.9/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 10:15:57.000000 templated_setup-0.9/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.8/LICENCE` & `templated_setup-0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.8/PKG-INFO` & `templated_setup-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.8
+Version: 0.9
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
 
-## V0.8 released on 29th/4/2024
+## V0.9 released on 29th/4/2024
 hopefully we will be able to install from pip. :p
```

### Comparing `templated_setup-0.8/README.md` & `templated_setup-0.9/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.8/templated_setup/__init__.py` & `templated_setup-0.9/templated_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,47 +213,47 @@
 	@classmethod
 	def __inner_reload_cached_data(cls):
 
 		try:
 			with open(CACHE_FILE_PATH, "r") as f:
 				json_data = json_x_load(f)
 		except FileNotFoundError:
-			if len(cls._json_data.keys()) == 0:
+			if cls._json_data and len(cls._json_data.keys()) == 0:
 				if cls._is_using_pip:
 					return
 				with open(CACHE_FILE_PATH, "w") as f:
 					json_x_dump({}, f)
 				with open(CACHE_FILE_PATH, "r") as f:
 					json_data = json_x_load(f)
 			else:
-				raise FileNotFoundError(f"File [{CACHE_FILE_PATH}] not found.")
+				return
 
 		cls._json_data = json_data
 
 		return None
 
 		f"[ END ] {Setup_Helper.__reload_cached_data}"
 
 
 	
 	@classmethod
 	def __reload_cached_data(cls):
-		cls.__inner_reload_cached_data()
 		cls._load_from_hardcoded()
 		return None
 		f"[ END ] {Setup_Helper.__reload_cached_data}"
 
 
 
 	@classmethod
 	def __load_date(cls, override=False):
 
 		cls.__reload_cached_data()
 
 		if not override:
+			assert cls._json_data
 			if "date" in cls._json_data:
 				cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._json_data["date"])
 			else:
 				while True:
 					new = cls.__inner_load_date()
 					confirmed = Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
@@ -271,14 +271,15 @@
 	@classmethod
 	def __inner_load_date(cls) -> "str":
 		do_want_to_use_current_date = Setup_Helper.__get_y_n("Would you like to use the current date?")
 		new = None
 		if do_want_to_use_current_date:
 
 			cls._date_of_last_modified = datetime_x_date.today()
+			assert cls._json_data
 			cls._json_data["date"] = cls._date_of_last_modified.isoformat()
 			new = cls._date_of_last_modified.isoformat()
 
 		else:
 
 			day = int(Setup_Helper.__get_answer(
 				"What day was it last modified? ",
@@ -293,14 +294,15 @@
 			year = int(Setup_Helper.__get_answer(
 				"What year was it last modified? ",
 				lambda x: (x.isdigit(), "Please enter a number."))
 			)
 
 			try:
 				cls._date_of_last_modified = datetime_x_date(year, month, day)
+				assert cls._json_data
 				cls._json_data["date"] = cls._date_of_last_modified.isoformat()
 				new = cls._date_of_last_modified.isoformat()
 
 			except ValueError:
 				print("] Error: Invalid date. Please try again.")
 		
 		with open(CACHE_FILE_PATH, "w") as f:
@@ -313,14 +315,15 @@
 
 	@classmethod
 	def __load_version_number(cls, override=False):
 		
 		cls.__reload_cached_data()
 
 		if not override:
+			assert cls._json_data
 			if "version_number" in cls._json_data:
 				cls._version_number = cls._json_data["version_number"]
 			else:
 				while True:
 					new = cls.__inner_load_version_number()
 					confirmed = Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
@@ -337,14 +340,15 @@
 	@classmethod
 	def __inner_load_version_number(cls) -> "str":
 		
 		cls._version_number = Setup_Helper.__get_answer(
 			"What is the version number? ",
 			Version.validate_version_number
 		)
+		assert cls._json_data
 		cls._json_data["version_number"] = cls._version_number
 
 		with open(CACHE_FILE_PATH, "w") as f:
 			json_x_dump(cls._json_data, f)
 
 		return cls._version_number
 
@@ -354,14 +358,15 @@
 
 	@classmethod
 	def __load_notes(cls, override=False):
 
 		cls.__reload_cached_data()
 
 		if not override:
+			assert cls._json_data
 			if "notes" in cls._json_data:
 				cls._notes = cls._json_data["notes"]
 			else:
 				while True:
 					new = cls.__inner_load_notes()
 					confirmed = Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
@@ -378,14 +383,15 @@
 	@classmethod
 	def __inner_load_notes(cls) -> "str":
 		
 		cls._notes = Setup_Helper.__get_answer(
 			"Enter the release notes: ",
 			lambda x: (len(x) > 0, "Notes cannot be empty.")
 		)
+		assert cls._json_data
 		cls._json_data["notes"] = cls._notes
 
 		with open(CACHE_FILE_PATH, "w") as f:
 			json_x_dump(cls._json_data, f)
 
 		return cls._notes
 
@@ -395,14 +401,15 @@
 
 	@classmethod
 	def __load_readme_file_path(cls, override=False):
 		
 		cls.__reload_cached_data()
 
 		if not override:
+			assert cls._json_data
 			if "readme_file_path" in cls._json_data:
 				cls._readme_file_path = cls._json_data["readme_file_path"]
 			else:
 				while True:
 					new = cls.__inner_load_readme_file_path()
 					confirmed = Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
 					if confirmed:
@@ -419,14 +426,15 @@
 	@classmethod
 	def __inner_load_readme_file_path(cls) -> "str":
 
 		cls._readme_file_path = Setup_Helper.__get_answer(
 			"Enter the path to the README file: ",
 			lambda x: (os.path.exists(x), "File does not exist.")
 		)
+		assert cls._json_data
 		cls._json_data["readme_file_path"] = cls._readme_file_path
 
 		with open(CACHE_FILE_PATH, "w") as f:
 			json_x_dump(cls._json_data, f)
 
 		return cls._readme_file_path
 
@@ -548,15 +556,18 @@
 	@classmethod
 	def _load_from_hardcoded(cls):
 
 		cls._is_using_pip = False
 		if "PIP_BUILD_TRACKER" in os.environ.keys():
 			cls._is_using_pip = True
 
-		cls._json_data = None
+		try:
+			__ = cls._json_data
+		except AttributeError:
+			cls._json_data = None
 		cls.__inner_reload_cached_data()
 		json_data = {} if not cls._json_data else cls._json_data
 		needs_update = False
 
 		# Before uploading to PyPi, we need to hardcode the values in a source file.
 		from . import _hardcoded
 		with open(_hardcoded.__file__, "r") as f:
@@ -574,14 +585,15 @@
 			contents = f.read()
 			splitted = contents.split("\n")[1:-2]
 			json_str = "\n".join(splitted)
 			print(json_str)
 			json_data = json_x_loads(json_str)
 
 		assert json_data is not None
+		cls._json_data = json_data
 
 		if cls._is_using_pip:
 			cls._json_data_when_using_pip = json_data
 			return None
 
 		cls._date_of_last_modified = datetime_x_date.fromisoformat(j_data.get("date", None))
 		cls._version_number = j_data.get("version_number", None)
```

### Comparing `templated_setup-0.8/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.9/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.8
+Version: 0.9
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
 
-## V0.8 released on 29th/4/2024
+## V0.9 released on 29th/4/2024
 hopefully we will be able to install from pip. :p
```

