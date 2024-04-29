# Comparing `tmp/templated_setup-0.3.tar.gz` & `tmp/templated_setup-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "templated_setup-0.3.tar", last modified: Mon Apr 29 08:25:26 2024, max compression
+gzip compressed data, was "templated_setup-0.4.tar", last modified: Mon Apr 29 08:33:17 2024, max compression
```

## Comparing `templated_setup-0.3.tar` & `templated_setup-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 08:25:26.300521 templated_setup-0.3/
--rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.3/LICENCE
--rw-rw-rw-   0        0        0     2557 2024-04-29 08:25:26.300007 templated_setup-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 08:25:26.300521 templated_setup-0.3/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-04-29 08:25:03.000000 templated_setup-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:25:26.294333 templated_setup-0.3/templated_setup/
--rw-rw-rw-   0        0        0    16662 2024-04-29 08:25:00.000000 templated_setup-0.3/templated_setup/__init__.py
--rw-rw-rw-   0        0        0      170 2024-04-29 08:18:53.000000 templated_setup-0.3/templated_setup/_hardcoded.py
-drwxrwxrwx   0        0        0        0 2024-04-29 08:25:26.298479 templated_setup-0.3/templated_setup.egg-info/
--rw-rw-rw-   0        0        0     2557 2024-04-29 08:25:26.000000 templated_setup-0.3/templated_setup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-04-29 08:25:26.000000 templated_setup-0.3/templated_setup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 08:25:26.000000 templated_setup-0.3/templated_setup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 08:25:26.000000 templated_setup-0.3/templated_setup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 08:33:17.422818 templated_setup-0.4/
+-rw-rw-rw-   0        0        0    25652 2024-03-14 11:21:06.000000 templated_setup-0.4/LICENCE
+-rw-rw-rw-   0        0        0     2557 2024-04-29 08:33:17.421790 templated_setup-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2172 2024-04-29 06:54:31.000000 templated_setup-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 08:33:17.422818 templated_setup-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-04-29 08:32:57.000000 templated_setup-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:33:17.416488 templated_setup-0.4/templated_setup/
+-rw-rw-rw-   0        0        0    16292 2024-04-29 08:32:46.000000 templated_setup-0.4/templated_setup/__init__.py
+-rw-rw-rw-   0        0        0      170 2024-04-29 08:27:21.000000 templated_setup-0.4/templated_setup/_hardcoded.py
+drwxrwxrwx   0        0        0        0 2024-04-29 08:33:17.420729 templated_setup-0.4/templated_setup.egg-info/
+-rw-rw-rw-   0        0        0     2557 2024-04-29 08:33:17.000000 templated_setup-0.4/templated_setup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-04-29 08:33:17.000000 templated_setup-0.4/templated_setup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 08:33:17.000000 templated_setup-0.4/templated_setup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 08:33:17.000000 templated_setup-0.4/templated_setup.egg-info/top_level.txt
```

### Comparing `templated_setup-0.3/LICENCE` & `templated_setup-0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `templated_setup-0.3/PKG-INFO` & `templated_setup-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.3
+Version: 0.4
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
 
-## V0.3 released on 29th/4/2024
+## V0.4 released on 29th/4/2024
 hopefully can be installed via pip now. ;p
```

### Comparing `templated_setup-0.3/README.md` & `templated_setup-0.4/README.md`

 * *Files identical despite different names*

### Comparing `templated_setup-0.3/templated_setup/__init__.py` & `templated_setup-0.4/templated_setup/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -524,25 +524,21 @@
 			with open(_hardcoded.__file__, "w") as f:
 				json_str = json_x_dumps(json_data, indent=4)
 				f.write(f"\"\"\"\n{json_str}\n\"\"\"\n")
 		with open(_hardcoded.__file__, "r") as f:
 			contents = f.read()
 			splitted = contents.split("\n")[1:-2]
 			json_str = "\n".join(splitted)
+			print(json_str)
 			json_data = json_x_loads(json_str)
 
 		assert json_data is not None
 
-		print(" ".join(sys.argv))
 		cls._is_using_pip = False
-		if "egg_info" in " ".join(sys.argv):
-			cls._is_using_pip = True
-		if "egg-info" in " ".join(sys.argv):
-			cls._is_using_pip = True
-		if "setup.py bdist_wheel --dist-dir " in " ".join(sys.argv):
+		if "PIP_BUILD_TRACKER" in os.environ.keys():
 			cls._is_using_pip = True
 
 		if cls._is_using_pip:
 			cls._json_data_when_using_pip = json_data
 			return None
 
 		cls._date_of_last_modified = j_data.get("date", None)
@@ -608,16 +604,14 @@
 		long_description += f"\n## V{cls._version.version_number} released on {cls._version.repr_date()}\n"
 		long_description += cls._notes
 
 		if not cls._is_using_pip:
 			print(f"Current Directory: [{os.path.abspath(os.getcwd())}].")
 			is_root_of_project = Setup_Helper.__get_y_n("Is this the root of the project?")
 		else:
-			if not os.path.exists("templated_setup.egg-info"):
-				raise FileNotFoundError("The `templated_setup.egg-info` directory does not exist. Please run this script from the root of the project directory.")
 			if not os.path.exists("setup.py"):
 				raise FileNotFoundError("The `setup.py` file does not exist. Please run this script from the root of the project directory.")
 			if not os.path.exists("templated_setup/_hardcoded.py"):
 				raise FileNotFoundError("The `_hardcoded.py` file does not exist. Please run this script from the root of the project directory.")
 			is_root_of_project = True
 
 		if not is_root_of_project:
```

### Comparing `templated_setup-0.3/templated_setup.egg-info/PKG-INFO` & `templated_setup-0.4/templated_setup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: templated_setup
-Version: 0.3
+Version: 0.4
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
 
-## V0.3 released on 29th/4/2024
+## V0.4 released on 29th/4/2024
 hopefully can be installed via pip now. ;p
```

