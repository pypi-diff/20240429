# Comparing `tmp/templated_setup-0.1.tar.gz` & `tmp/templated_setup-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.1.tar", last modified: Mon Apr 29 07:03:18 2024, max compression
+gzip compressed data, was "templated_setup-0.2.tar", last modified: Mon Apr 29 08:20:27 2024, max compression
```

## Comparing `templated_setup-0.1.tar` & `templated_setup-0.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 07:03:18.783371 templated_setup-0.1/
--rw-rw-rw-   0        0        0     2496 2024-04-29 07:03:18.782355 templated_setup-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 07:03:18.783888 templated_setup-0.1/setup.cfg
--rw-rw-rw-   0        0        0      288 2024-04-29 07:03:09.000000 templated_setup-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:03:18.777064 templated_setup-0.1/templated_setup/
--rw-rw-rw-   0        0        0    13509 2024-04-29 07:03:08.000000 templated_setup-0.1/templated_setup/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 07:03:18.781332 templated_setup-0.1/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2496 2024-04-29 07:03:18.000000 templated_setup-0.1/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-29 07:03:18.000000 templated_setup-0.1/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 07:03:18.000000 templated_setup-0.1/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 07:03:18.000000 templated_setup-0.1/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 08:20:27.035032 templated_setup-0.2/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.2/LICENCE
+-rw-rw-rw-   0        0        0     2557 2024-04-29 08:20:27.034519 templated_setup-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:20:27.035542 templated_setup-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-04-29 08:20:12.000000 templated_setup-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:20:27.029085 templated_setup-0.2/templated_setup/
+-rw-rw-rw-   0        0        0    16659 2024-04-29 08:20:12.000000 templated_setup-0.2/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0      170 2024-04-29 08:18:53.000000 templated_setup-0.2/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:20:27.033470 templated_setup-0.2/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2557 2024-04-29 08:20:26.000000 templated_setup-0.2/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-29 08:20:26.000000 templated_setup-0.2/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:20:26.000000 templated_setup-0.2/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 08:20:26.000000 templated_setup-0.2/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.1/PKG-INFO` & `templated_setup-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: templated_setup
-Version: 0.1
-Summary: A quick and easy replacement for some `setup.py` implementations.
-Author: matrikater (Joel Watson)
-Author-email: administraitor@matriko.xyz
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
 # Standardized `setup.py`
 
 ## Overview
 
 This project contains a Python-based setup automation tool designed to help streamline the process of preparing and managing project setups. It includes utilities for handling versioning, dates, notes, and README files, leveraging a dynamic caching system to maintain state across sessions.
 
 ## Word of Caution
@@ -63,10 +55,7 @@
 Contributions are welcome! For feature requests, bug reports, or questions, please submit an issue.
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
-
-## V0.1 released on 29th/4/2024
-init
```

### Comparing `templated_setup-0.1/README.md` & `templated_setup-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: templated_setup
+Version: 0.2
+Summary: A quick and easy replacement for some `setup.py` implementations.
+Author: matrikater (Joel Watson)
+Author-email: administraitor@matriko.xyz
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENCE
+
 # Standardized `setup.py`
 
 ## Overview
 
 This project contains a Python-based setup automation tool designed to help streamline the process of preparing and managing project setups. It includes utilities for handling versioning, dates, notes, and README files, leveraging a dynamic caching system to maintain state across sessions.
 
 ## Word of Caution
@@ -55,7 +64,10 @@
 Contributions are welcome! For feature requests, bug reports, or questions, please submit an issue.
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
+
+## V0.2 released on 29th/4/2024
+hopefully can be installed via pip now. ;p
```

### Comparing `templated_setup-0.1/templated_setup/__init__.py` & `templated_setup-0.2/templated_setup/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,41 @@
 from dataclasses import dataclass as dataclass_x_dataclass
-from json import load as json_x_load, dump as json_x_dump
+from json import load as json_x_load, dump as json_x_dump, loads as json_x_loads, dumps as json_x_dumps
 from datetime import date as datetime_x_date
 from time import sleep as time_x_sleep
 from typing import Callable, overload
 from setuptools import setup
 import shutil
 import sys
 import os
 
 
 
 
 
 
 
-CACHE_FILE_PATH = ".templated_setup_cache.json"
+CACHE_FILE_PATH = ""
+LEGAL_NOTICE = """
+==================================
+Legal Notice for `templated_setup`
+==================================
+
+By using this software, you, the user, acknowledge and agree that you are solely responsible for the content that is published using this tool.
+The software is provided "as is", and the developers make no representations or warranties of any kind regarding its use.
+
+You assume all responsibility and risk for the use of this software and the materials you create or publish with it.
+
+The developers shall not be liable for any claims, damages, or other liabilities arising from the use of the software or content published therein.
+
+========================
+THANK YOU AND TAKE CARE!
+========================
+
+"""
 
 
 
 
 
 
 
@@ -392,14 +409,21 @@
 
 		f"[ END ] {Setup_Helper.__inner_load_readme_file_path}"
 
 
 
 	@classmethod
 	def __load_parameters(cls):
+		if cls._is_using_pip:
+			json_data = cls._json_data_when_using_pip
+			cls._date_of_last_modified = datetime_x_date.fromisoformat(json_data["date"])
+			cls._version_number = json_data["version_number"]
+			cls._notes = json_data["notes"]
+			cls._readme_file_path = json_data["readme_file_path"]
+			return
 		user_wants_to_change_params = False
 		while True:
 
 			if user_wants_to_change_params:
 				options = [
 					["Date", 		lambda: cls.__load_date(override=True)],
 					["Version Number", 	lambda: cls.__load_version_number(override=True)],
@@ -436,14 +460,15 @@
 			print(f"Readme File Path:  [{cls._readme_file_path}]")
 			print(f"\n")
 
 			confirmed = Setup_Helper.__get_y_n("Is this information correct?")
 			if confirmed:
 				break
 			else:
+				user_wants_to_change_params = True
 				print("Please enter the information again.")
 
 
 	
 		f"[ END ] {Setup_Helper.__load_parameters}"
 
 
@@ -464,33 +489,89 @@
 
 
 	#################
 	# INSTANTIATION #
 	#################
 	
 
+
 	@classmethod
-	def setup(cls, name:"str", author:"str", description:"str", **kwargs_for_setup_tools) -> "None":
+	def init(cls, cache_file_path_:"str") -> "None":
 
-		cls.name = name
-		cls.author = author
-		cls.description = description
+		global CACHE_FILE_PATH
+		CACHE_FILE_PATH = cache_file_path_
 
 		try:
 			__ = cls.__activated_already
 		except AttributeError:
 			cls.__activated_already = None
 		if cls.__activated_already:
 			raise Exception("This class is a singleton and can only be activated once.")
-
 		cls.__activated_already = True
-		cls._date_of_last_modified = None
-		cls._version_number = None
-		cls._notes = None
-		cls._readme_file_path = None
+
+		json_data = Setup_Helper.__get_cached_data()
+		needs_update = False
+
+		# Before uploading to PyPi, we need to hardcode the values in a source file.
+		from . import _hardcoded
+		with open(_hardcoded.__file__, "r") as f:
+			contents = f.read()
+			splitted = contents.split("\n")[1:-2]
+			json_str = "\n".join(splitted)
+			j_data = json_x_loads(json_str)
+			if j_data != json_data:
+				needs_update = True
+		if needs_update:
+			with open(_hardcoded.__file__, "w") as f:
+				json_str = json_x_dumps(json_data, indent=4)
+				f.write(f"\"\"\"\n{json_str}\n\"\"\"\n")
+		with open(_hardcoded.__file__, "r") as f:
+			contents = f.read()
+			splitted = contents.split("\n")[1:-2]
+			json_str = "\n".join(splitted)
+			json_data = json_x_loads(json_str)
+
+		assert json_data is not None
+
+		print(" ".join(sys.argv))
+		cls._is_using_pip = False
+		if "egg_info" in " ".join(sys.argv):
+			cls._is_using_pip = True
+		if "egg-info" in " ".join(sys.argv):
+			cls._is_using_pip = True
+		if "setup.py bdist_wheel --dist-dir " in " ".join(sys.argv):
+			cls._is_using_pip = True
+
+		if cls._is_using_pip:
+			cls._json_data_when_using_pip = j_data
+			return None
+
+		cls._date_of_last_modified = j_data.get("date", None)
+		cls._version_number = j_data.get("version_number", None)
+		cls._notes = j_data.get("notes", None)
+		cls._readme_file_path = j_data.get("readme_file_path", None)
+
+		return None
+	
+		f"[ END ] {Setup_Helper.init}"
+
+
+
+	@classmethod
+	def setup(cls, name:"str", author:"str", description:"str", **kwargs_for_setup_tools) -> "None":
+		
+		if not cls.__activated_already:
+			raise Exception("You must call `init` before calling `setup`.")
+
+		if not cls._is_using_pip:
+			print(LEGAL_NOTICE)
+
+		cls._name = name
+		cls._author = author
+		cls._description = description
 
 		Setup_Helper.__load_parameters()
 		assert isinstance(cls._date_of_last_modified, datetime_x_date)
 		assert isinstance(cls._version_number, str)
 		assert isinstance(cls._notes, str)
 		assert isinstance(cls._readme_file_path, str)
 
@@ -523,73 +604,80 @@
 		assert isinstance(cls._notes, str)
 		assert isinstance(cls._readme_file_path, str)
 
 		long_description = Setup_Helper.__init_description(cls._readme_file_path)
 		long_description += f"\n## V{cls._version.version_number} released on {cls._version.repr_date()}\n"
 		long_description += cls._notes
 
-		print()
-		print("WARNING!! ::: ")
-		print("          ::: THIS SCRIPT WILL DELETE THE `dist` DIRECTORY...")
-		print("          ::: FOR SAFETY, PLEASE MAKE SURE YOU COMMIT YOUR CHANGES BEFORE RUNNING THIS SCRIPT.")
-		print("          ::: ")
-		print("          ::: ALSO, MAKE SURE YOU ARE IN THE ROOT OF THE PROJECT DIRECTORY.")
-		print("          ::: ")
-		print()
-
-		print(f"Current Directory: [{os.path.abspath(os.getcwd())}].")
-		is_root_of_project = Setup_Helper.__get_y_n("Is this the root of the project?")
+		if not cls._is_using_pip:
+			print(f"Current Directory: [{os.path.abspath(os.getcwd())}].")
+			is_root_of_project = Setup_Helper.__get_y_n("Is this the root of the project?")
+		else:
+			if not os.path.exists("templated_setup.egg-info"):
+				raise FileNotFoundError("The `templated_setup.egg-info` directory does not exist. Please run this script from the root of the project directory.")
+			if not os.path.exists("setup.py"):
+				raise FileNotFoundError("The `setup.py` file does not exist. Please run this script from the root of the project directory.")
+			if not os.path.exists("templated_setup/_hardcoded.py"):
+				raise FileNotFoundError("The `_hardcoded.py` file does not exist. Please run this script from the root of the project directory.")
+			is_root_of_project = True
 
 		if not is_root_of_project:
 			raise Exception("This script must be run from the root of the project directory.")
 		
 		separator = "\\" if os.name == "nt" else "/"
 
-		print(f"WARNING: ABOUT TO REMOVE THE `{os.getcwd()}{separator}dist` DIRECTORY!!")
-		print("YOU HAVE 3 SECONDS TO CANCEL...")
-		try:
-			time_x_sleep(3)
-		except KeyboardInterrupt:
-			print("Cancelled.")
-			exit(0)
+		if not cls._is_using_pip:
+			print(f"WARNING: ABOUT TO REMOVE THE `{os.getcwd()}{separator}dist` DIRECTORY!!")
+			print("YOU HAVE 3 SECONDS TO CANCEL...")
+			try:
+				time_x_sleep(3)
+			except KeyboardInterrupt:
+				print("Cancelled.")
+				exit(0)
 
 		shutil.rmtree("dist", ignore_errors=True)
 
-		cls._old_sys_argv = sys.argv
-		sys.argv = [sys.argv[0], "sdist"]
+		if not cls._is_using_pip:
+			cls._old_sys_argv = sys.argv
+			sys.argv = [sys.argv[0], "sdist"]
 
 		setup(
-			name=cls.name,
+			name=cls._name,
 			version=cls._version.version_number,
-			author=cls.author,
-			description=cls.description,
+			author=cls._author,
+			description=cls._description,
 			long_description_content_type="text/markdown; charset=UTF-8; variant=GFM",
 			long_description=long_description,
 			**kwargs_for_setup_tools,
 		)
 
-		print("\n] Setup complete.\n\n")
+		if not cls._is_using_pip:
+			print("\n] Setup complete.\n\n")
+		else:
+			return
 
 		do_publish = Setup_Helper.__get_y_n("Would you like to publish to PyPi?")
 		if not do_publish:
 			exit(0)
 
 		input("Press Enter to continue... ")
 		Setup_Helper.__clear_screen()
 
 		print(f"\tDescription is readable below...\n{long_description}")
 		print()
 
-		did_check_version = Setup_Helper.__get_y_n("Did you update the version information?")
-		if not did_check_version:
+		do_proceed = Setup_Helper.__get_y_n("Would you like to proceed?")
+		if not do_proceed:
 			exit(0)
 
-		again_to_be_sure = Setup_Helper.__get_y_n("ARE YOU SURE YOU WANT TO PUBLISH?")
-		if not again_to_be_sure:
-			exit(0)
+		Setup_Helper.__clear_screen()
+		print("WAITING 5 SECONDS.")
+		print("THIS IS YOUR LAST CHANCE TO CANCEL...")
+		print()
+		time_x_sleep(5)
 
 		os.system(f"{sys.executable} -m twine upload --verbose --repository pypi dist/*")
 
 		sys.argv = cls._old_sys_argv
 
 		return None
```

### Comparing `templated_setup-0.1/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.2/templated_setup.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.1
+Version: 0.2
 Summary: A quick and easy replacement for some `setup.py` implementations.
 Author: matrikater (Joel Watson)
 Author-email: administraitor@matriko.xyz
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+License-File: LICENCE
 
 # Standardized `setup.py`
 
 ## Overview
 
 This project contains a Python-based setup automation tool designed to help streamline the process of preparing and managing project setups. It includes utilities for handling versioning, dates, notes, and README files, leveraging a dynamic caching system to maintain state across sessions.
 
@@ -64,9 +65,9 @@
 
 > Actually I would be happy to have some help with this project as making a `setup.py` every time is a bit boring.
 
 ## License
 
 This project is licensed under the GPLv2 License - see the [LICENSE](LICENSE) file for details.
 
-## V0.1 released on 29th/4/2024
-init
+## V0.2 released on 29th/4/2024
+hopefully can be installed via pip now. ;p
```

