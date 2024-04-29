# Comparing `tmp/templated_setup-0.4.tar.gz` & `tmp/templated_setup-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.4.tar", last modified: Mon Apr 29 08:33:17 2024, max compression
+gzip compressed data, was "templated_setup-0.5.tar", last modified: Mon Apr 29 09:28:57 2024, max compression
```

## Comparing `templated_setup-0.4.tar` & `templated_setup-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:33:17.422818 templated_setup-0.4/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.4/LICENCE
--rw-rw-rw-   0        0        0     2557 2024-04-29 08:33:17.421790 templated_setup-0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 08:33:17.422818 templated_setup-0.4/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-04-29 08:32:57.000000 templated_setup-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:33:17.416488 templated_setup-0.4/templated_setup/
--rw-rw-rw-   0        0        0    16292 2024-04-29 08:32:46.000000 templated_setup-0.4/templated_setup/__init__.py
--rw-rw-rw-   0        0        0      170 2024-04-29 08:27:21.000000 templated_setup-0.4/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:33:17.420729 templated_setup-0.4/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2557 2024-04-29 08:33:17.000000 templated_setup-0.4/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-04-29 08:33:17.000000 templated_setup-0.4/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:33:17.000000 templated_setup-0.4/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 08:33:17.000000 templated_setup-0.4/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 09:28:57.873164 templated_setup-0.5/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.5/LICENCE
+-rw-rw-rw-   0        0        0     2557 2024-04-29 09:28:57.872145 templated_setup-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 09:28:57.873164 templated_setup-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-04-29 08:45:00.000000 templated_setup-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:28:57.867465 templated_setup-0.5/templated_setup/
+-rw-rw-rw-   0        0        0    17714 2024-04-29 09:28:39.000000 templated_setup-0.5/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0      170 2024-04-29 08:48:05.000000 templated_setup-0.5/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:28:57.872145 templated_setup-0.5/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2557 2024-04-29 09:28:57.000000 templated_setup-0.5/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-29 09:28:57.000000 templated_setup-0.5/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 09:28:57.000000 templated_setup-0.5/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 09:28:57.000000 templated_setup-0.5/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.4/LICENCE` & `templated_setup-0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.4/PKG-INFO` & `templated_setup-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.4
+Version: 0.5
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
 
-## V0.4 released on 29th/4/2024
+## V0.5 released on 29th/4/2024
 hopefully can be installed via pip now. ;p
```

### Comparing `templated_setup-0.4/README.md` & `templated_setup-0.5/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.4/templated_setup/__init__.py` & `templated_setup-0.5/templated_setup/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -172,304 +172,318 @@
 
 
 	@staticmethod
 	def __get_answer(question:"str", satisfy_func:"Callable[[str],tuple[bool,str]]") -> "str":
 		ans = ""
 		while True:
 
-			ans = input(question)
+			ans = input(f"> {question}")
 			is_valid, err_msg = satisfy_func(ans)
 
 			if is_valid:
 				break
 
-			print(err_msg)
+			print(f"] Error [{err_msg}]")
 		
 		return ans
 		f"[ END ] {Setup_Helper.__get_answer}"
 
 
 
 	@staticmethod
 	def __get_y_n(question:str) -> bool:
 		question = question + " (y/n) "
 		while True:
 
-			answer = input(question)
+			answer = input(f"> {question}")
 
 			if answer.lower() == "y":
 				return True
 
 			elif answer.lower() == "n":
 				return False
 
 			else:
-				print("Please enter 'y' or 'n'.")
+				print("] Please enter 'y' or 'n'.")
 
 		return None
 		f"[ END ] {Setup_Helper.__get_y_n}"
 
 
 
 	@classmethod
-	def __get_cached_data(cls):
-
-		json_data = None
+	def __reload_cached_data(cls):
 
 		try:
 			with open(CACHE_FILE_PATH, "r") as f:
 				json_data = json_x_load(f)
 		except FileNotFoundError:
 			with open(CACHE_FILE_PATH, "w") as f:
 				json_x_dump({}, f)
 			with open(CACHE_FILE_PATH, "r") as f:
 				json_data = json_x_load(f)
 
-		return json_data
+		cls._json_data = json_data
 
-		f"[ END ] {Setup_Helper.__get_cached_data}"
+		f"[ END ] {Setup_Helper.__reload_cached_data}"
 
 
 
 	@classmethod
 	def __load_date(cls, override=False):
 
-		json_data = cls.__get_cached_data()
+		cls.__reload_cached_data()
 
 		if not override:
-			if json_data and "date" in json_data:
-				cls._date_of_last_modified = datetime_x_date.fromisoformat(json_data["date"])
+			if "date" in cls._json_data:
+				cls._date_of_last_modified = datetime_x_date.fromisoformat(cls._json_data["date"])
 			else:
-				cls.__inner_load_date()
+				while True:
+					new = cls.__inner_load_date()
+					confirmed = Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
+					if confirmed:
+						break
+
 		else:
 			cls.__inner_load_date()
 
 		return None
 
 		f"[ END ] {Setup_Helper.__load_date}"
 
 
 
 	@classmethod
-	def __inner_load_date(cls):		
+	def __inner_load_date(cls) -> "str":
 		do_want_to_use_current_date = Setup_Helper.__get_y_n("Would you like to use the current date?")
-		json_data = cls.__get_cached_data()
-		while True:
-			if do_want_to_use_current_date:
+		new = None
+		if do_want_to_use_current_date:
 
-				cls._date_of_last_modified = datetime_x_date.today()
-				confirmed = Setup_Helper.__get_y_n(f"Is [{cls._date_of_last_modified}] Correct?")
-				json_data["date"] = cls._date_of_last_modified.isoformat()
-				if confirmed:
-					break
+			cls._date_of_last_modified = datetime_x_date.today()
+			cls._json_data["date"] = cls._date_of_last_modified.isoformat()
+			new = cls._date_of_last_modified.isoformat()
 
-			else:
+		else:
 
-				day = int(Setup_Helper.__get_answer(
-					"What day was it last modified? ",
-					lambda x: (x.isdigit(), "Please enter a number."))
-				)
-
-				month = int(Setup_Helper.__get_answer(
-					"What month was it last modified? ",
-					lambda x: (x.isdigit(), "Please enter a number."))
-				)
-
-				year = int(Setup_Helper.__get_answer(
-					"What year was it last modified? ",
-					lambda x: (x.isdigit(), "Please enter a number."))
-				)
-
-				try:
-					cls._date_of_last_modified = datetime_x_date(year, month, day)
-					confirmed = Setup_Helper.__get_y_n(f"Is [{cls._date_of_last_modified}] Correct?")
-					json_data["date"] = cls._date_of_last_modified.isoformat()
-					if confirmed:
-						break
+			day = int(Setup_Helper.__get_answer(
+				"What day was it last modified? ",
+				lambda x: (x.isdigit(), "Please enter a number."))
+			)
+
+			month = int(Setup_Helper.__get_answer(
+				"What month was it last modified? ",
+				lambda x: (x.isdigit(), "Please enter a number."))
+			)
+
+			year = int(Setup_Helper.__get_answer(
+				"What year was it last modified? ",
+				lambda x: (x.isdigit(), "Please enter a number."))
+			)
+
+			try:
+				cls._date_of_last_modified = datetime_x_date(year, month, day)
+				cls._json_data["date"] = cls._date_of_last_modified.isoformat()
+				new = cls._date_of_last_modified.isoformat()
 
-				except ValueError:
-					print("Invalid date. Please try again.")
-			
-			assert isinstance(cls._date_of_last_modified, datetime_x_date)
+			except ValueError:
+				print("] Error: Invalid date. Please try again.")
+		
 		with open(CACHE_FILE_PATH, "w") as f:
-			json_x_dump(json_data, f)
-		return None
+			json_x_dump(cls._json_data, f)
+		assert isinstance(new, str)
+		return new
 		f"[ END ] {Setup_Helper.__inner_load_date}"
 
 
 
 	@classmethod
 	def __load_version_number(cls, override=False):
 		
-		json_data = cls.__get_cached_data()
+		cls.__reload_cached_data()
 
 		if not override:
-			if json_data and "version_number" in json_data:
-				cls._version_number = json_data["version_number"]
+			if "version_number" in cls._json_data:
+				cls._version_number = cls._json_data["version_number"]
 			else:
-				cls.__inner_load_version_number()
+				while True:
+					new = cls.__inner_load_version_number()
+					confirmed = Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
+					if confirmed:
+						break
 		else:
 			cls.__inner_load_version_number()
 
 		return None
 	
 		f"[ END ] {Setup_Helper.__load_version_number}"
 
 
 
 	@classmethod
-	def __inner_load_version_number(cls):
+	def __inner_load_version_number(cls) -> "str":
 		
-		while True:
-
-			cls._version_number = Setup_Helper.__get_answer(
-				"What is the version number? ",
-				Version.validate_version_number
-			)
-
-			confirmed = Setup_Helper.__get_y_n(f"Is [{cls._version_number}] Correct?")
-			if confirmed:
-				break
-
-		json_data = cls.__get_cached_data()
-		json_data["version_number"] = cls._version_number
+		cls._version_number = Setup_Helper.__get_answer(
+			"What is the version number? ",
+			Version.validate_version_number
+		)
+		cls._json_data["version_number"] = cls._version_number
 
 		with open(CACHE_FILE_PATH, "w") as f:
-			json_x_dump(json_data, f)
+			json_x_dump(cls._json_data, f)
 
-		return None
+		return cls._version_number
 
 		f"[ END ] {Setup_Helper.__inner_load_version_number}"
 
 
 
 	@classmethod
 	def __load_notes(cls, override=False):
 
-		json_data = cls.__get_cached_data()
+		cls.__reload_cached_data()
 
 		if not override:
-			if json_data and "notes" in json_data:
-				cls._notes = json_data["notes"]
+			if "notes" in cls._json_data:
+				cls._notes = cls._json_data["notes"]
 			else:
-				cls.__inner_load_notes()
+				while True:
+					new = cls.__inner_load_notes()
+					confirmed = Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
+					if confirmed:
+						break
 		else:
 			cls.__inner_load_notes()
 
 		return None
 
 		f"[ END ] {Setup_Helper.__load_notes}"
 
 
 
 	@classmethod
-	def __inner_load_notes(cls):
+	def __inner_load_notes(cls) -> "str":
 		
-		cls._notes = input("Enter the release notes: ")
-
-		json_data = cls.__get_cached_data()
-		json_data["notes"] = cls._notes
+		cls._notes = Setup_Helper.__get_answer(
+			"Enter the release notes: ",
+			lambda x: (len(x) > 0, "Notes cannot be empty.")
+		)
+		cls._json_data["notes"] = cls._notes
 
 		with open(CACHE_FILE_PATH, "w") as f:
-			json_x_dump(json_data, f)
+			json_x_dump(cls._json_data, f)
 
-		return None
+		return cls._notes
 
 		f"[ END ] {Setup_Helper.__inner_load_notes}"
 
 
 
 	@classmethod
-	def __load_readme_file_path(cls):
+	def __load_readme_file_path(cls, override=False):
 		
-		json_data = cls.__get_cached_data()
+		cls.__reload_cached_data()
 
-		if json_data and "readme_file_path" in json_data:
-			cls._readme_file_path = json_data["readme_file_path"]
+		if not override:
+			if "readme_file_path" in cls._json_data:
+				cls._readme_file_path = cls._json_data["readme_file_path"]
+			else:
+				while True:
+					new = cls.__inner_load_readme_file_path()
+					confirmed = Setup_Helper.__get_y_n(f"Is [{new}] Correct?")
+					if confirmed:
+						break
 		else:
 			cls.__inner_load_readme_file_path()
 
 		return None
 
 		f"[ END ] {Setup_Helper.__load_readme_file_path}"
 
 
 
 	@classmethod
-	def __inner_load_readme_file_path(cls):
-
-		cls._readme_file_path = input("Enter the path to the README file: ")
+	def __inner_load_readme_file_path(cls) -> "str":
 
-		json_data = cls.__get_cached_data()
-		json_data["readme_file_path"] = cls._readme_file_path
+		cls._readme_file_path = Setup_Helper.__get_answer(
+			"Enter the path to the README file: ",
+			lambda x: (os.path.exists(x), "File does not exist.")
+		)
+		cls._json_data["readme_file_path"] = cls._readme_file_path
 
 		with open(CACHE_FILE_PATH, "w") as f:
-			json_x_dump(json_data, f)
+			json_x_dump(cls._json_data, f)
 
-		return None
+		return cls._readme_file_path
 
 		f"[ END ] {Setup_Helper.__inner_load_readme_file_path}"
 
 
 
 	@classmethod
 	def __load_parameters(cls):
 		if cls._is_using_pip:
 			json_data = cls._json_data_when_using_pip
+			assert json_data is not None
 			cls._date_of_last_modified = datetime_x_date.fromisoformat(json_data["date"])
 			cls._version_number = json_data["version_number"]
 			cls._notes = json_data["notes"]
 			cls._readme_file_path = json_data["readme_file_path"]
 			return
 		user_wants_to_change_params = False
 		while True:
 
+			cls._load_from_hardcoded()
+
+			cls.__clear_screen()
+			print(f"\n\n] Current Infos:")
+			print(f"]] Date:              [{cls._date_of_last_modified}]")
+			print(f"]] Version Number:    [{cls._version_number}]")
+			print(f"]] Notes:             [{cls._notes}]")
+			print(f"]] Readme File Path:  [{cls._readme_file_path}]")
+			print(f"\n")
+
 			if user_wants_to_change_params:
 				options = [
-					["Date", 		lambda: cls.__load_date(override=True)],
-					["Version Number", 	lambda: cls.__load_version_number(override=True)],
-					["Notes", 		lambda: cls.__load_notes(override=True)]
+					["Last Modified Date", 		lambda: cls.__load_date(override=True)],
+					["Current Version Number", 	lambda: cls.__load_version_number(override=True)],
+					["Current Release Notes", 	lambda: cls.__load_notes(override=True)],
+					["README File Path", 		lambda: cls.__load_readme_file_path(override=True)]
 				]
-				print("What would you like to do?")
+				print("] What would you like to do?")
 				for i, [opt, __] in enumerate(options):
-					print(f" - [{i+1}] Change {opt},")
-				print(f" - {len(options)+1}] Go Back.")
+					print(f"]] - [{i+1}] Change {opt},")
+				print(f"]] - [{len(options)+1}] Go Back.")
 				choice = int(Setup_Helper.__get_answer(
 					"Enter the number of your choice: ",
 					lambda x: (
 						x.isdigit() and 0 < int(x) <= len(options)+1,
-						"Invalid choice. Please try again.")
+						"Invalid choice. Please try again."
 					)
-				)
+				))
 				if choice == len(options)+1:
 					user_wants_to_change_params = False
 					continue
 				callback = options[choice-1][1]
 				callback()
-
+				continue
 
 
 			cls.__load_date()
 			cls.__load_version_number()
 			cls.__load_notes()
 			cls.__load_readme_file_path()
 
-			print(f"\n\n")
-			print(f"Date:              [{cls._date_of_last_modified}]")
-			print(f"Version Number:    [{cls._version_number}]")
-			print(f"Notes:             [{cls._notes}]")
-			print(f"Readme File Path:  [{cls._readme_file_path}]")
-			print(f"\n")
-
 			confirmed = Setup_Helper.__get_y_n("Is this information correct?")
 			if confirmed:
 				break
 			else:
 				user_wants_to_change_params = True
-				print("Please enter the information again.")
+				print("] Error: Please enter the information again.")
+				time_x_sleep(0.8)
+				cls.__clear_screen()
 
 
 	
 		f"[ END ] {Setup_Helper.__load_parameters}"
 
 
 
@@ -504,15 +518,27 @@
 			__ = cls.__activated_already
 		except AttributeError:
 			cls.__activated_already = None
 		if cls.__activated_already:
 			raise Exception("This class is a singleton and can only be activated once.")
 		cls.__activated_already = True
 
-		json_data = Setup_Helper.__get_cached_data()
+		cls._load_from_hardcoded()
+
+		return None
+	
+		f"[ END ] {Setup_Helper.init}"
+
+
+
+	@classmethod
+	def _load_from_hardcoded(cls):
+
+		Setup_Helper.__reload_cached_data()
+		json_data = cls._json_data
 		needs_update = False
 
 		# Before uploading to PyPi, we need to hardcode the values in a source file.
 		from . import _hardcoded
 		with open(_hardcoded.__file__, "r") as f:
 			contents = f.read()
 			splitted = contents.split("\n")[1:-2]
@@ -544,26 +570,39 @@
 		cls._date_of_last_modified = j_data.get("date", None)
 		cls._version_number = j_data.get("version_number", None)
 		cls._notes = j_data.get("notes", None)
 		cls._readme_file_path = j_data.get("readme_file_path", None)
 
 		return None
 	
-		f"[ END ] {Setup_Helper.init}"
+		f"[ END ] {Setup_Helper._load_from_hardcoded}"
 
 
 
 	@classmethod
 	def setup(cls, name:"str", author:"str", description:"str", **kwargs_for_setup_tools) -> "None":
 		
+		Setup_Helper.__clear_screen()
+
 		if not cls.__activated_already:
 			raise Exception("You must call `init` before calling `setup`.")
 
 		if not cls._is_using_pip:
-			print(LEGAL_NOTICE)
+			for c in LEGAL_NOTICE:
+				print(c, end="", flush=True)
+				time_x_sleep(0.00075)
+			print("\n")
+			time_x_sleep(0.5)
+			print(".", end="", flush=True)
+			time_x_sleep(0.5)
+			print(".", end="", flush=True)
+			time_x_sleep(0.5)
+			print(".", end="", flush=True)
+			time_x_sleep(0.8)
+
 
 		cls._name = name
 		cls._author = author
 		cls._description = description
 
 		Setup_Helper.__load_parameters()
 		assert isinstance(cls._date_of_last_modified, datetime_x_date)
@@ -601,42 +640,57 @@
 		assert isinstance(cls._readme_file_path, str)
 
 		long_description = Setup_Helper.__init_description(cls._readme_file_path)
 		long_description += f"\n## V{cls._version.version_number} released on {cls._version.repr_date()}\n"
 		long_description += cls._notes
 
 		if not cls._is_using_pip:
-			print(f"Current Directory: [{os.path.abspath(os.getcwd())}].")
+			Setup_Helper.__clear_screen()
+			print(f"Current Directory: [{os.path.abspath(os.getcwd())}].\n\n")
 			is_root_of_project = Setup_Helper.__get_y_n("Is this the root of the project?")
+			Setup_Helper.__clear_screen()
 		else:
 			if not os.path.exists("setup.py"):
 				raise FileNotFoundError("The `setup.py` file does not exist. Please run this script from the root of the project directory.")
 			if not os.path.exists("templated_setup/_hardcoded.py"):
 				raise FileNotFoundError("The `_hardcoded.py` file does not exist. Please run this script from the root of the project directory.")
 			is_root_of_project = True
 
 		if not is_root_of_project:
 			raise Exception("This script must be run from the root of the project directory.")
 		
 		separator = "\\" if os.name == "nt" else "/"
 
+		dirs_to_remove = [
+			"dist",
+			"build",
+			f"{cls._name}.egg-info"
+		]
+
+
 		if not cls._is_using_pip:
-			print(f"WARNING: ABOUT TO REMOVE THE `{os.getcwd()}{separator}dist` DIRECTORY!!")
-			print("YOU HAVE 3 SECONDS TO CANCEL...")
 			try:
-				time_x_sleep(3)
+				for d in dirs_to_remove:
+					if os.path.exists(d):
+						print(f"\n] WARNING: ABOUT TO REMOVE THE `{os.getcwd()}{separator}{d}` DIRECTORY!!")
+						print("] YOU HAVE 3 SECONDS TO CANCEL...")
+						time_x_sleep(3)
+						shutil.rmtree(d, ignore_errors=True)
 			except KeyboardInterrupt:
-				print("Cancelled.")
+				print("] Cancelled.")
 				exit(0)
-
-		shutil.rmtree("dist", ignore_errors=True)
+			Setup_Helper.__clear_screen()
 
 		if not cls._is_using_pip:
 			cls._old_sys_argv = sys.argv
 			sys.argv = [sys.argv[0], "sdist"]
+			do_proceed = Setup_Helper.__get_y_n("Would you like to proceed with the build?")
+			if not do_proceed:
+				exit(0)
+			Setup_Helper.__clear_screen()
 
 		setup(
 			name=cls._name,
 			version=cls._version.version_number,
 			author=cls._author,
 			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
@@ -649,29 +703,24 @@
 		else:
 			return
 
 		do_publish = Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
 
-		input("Press Enter to continue... ")
 		Setup_Helper.__clear_screen()
 
-		print(f"\tDescription is readable below...\n{long_description}")
+		print(f"] Description is readable below...\n{long_description}")
 		print()
 
 		do_proceed = Setup_Helper.__get_y_n("Would you like to proceed?")
 		if not do_proceed:
 			exit(0)
 
 		Setup_Helper.__clear_screen()
-		print("WAITING 5 SECONDS.")
-		print("THIS IS YOUR LAST CHANCE TO CANCEL...")
-		print()
-		time_x_sleep(5)
 
 		os.system(f"{sys.executable} -m twine upload --verbose --repository pypi dist/*")
 
 		sys.argv = cls._old_sys_argv
 
 		return None
```

### Comparing `templated_setup-0.4/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.5/templated_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.4
+Version: 0.5
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
 
-## V0.4 released on 29th/4/2024
+## V0.5 released on 29th/4/2024
 hopefully can be installed via pip now. ;p
```

