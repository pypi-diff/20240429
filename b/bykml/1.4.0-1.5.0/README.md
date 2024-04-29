# Comparing `tmp/bykml-1.4.0.tar.gz` & `tmp/bykml-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bykml-1.4.0.tar", last modified: Mon Jan 22 16:57:11 2024, max compression
+gzip compressed data, was "bykml-1.5.0.tar", last modified: Mon Apr 29 09:50:11 2024, max compression
```

## Comparing `bykml-1.4.0.tar` & `bykml-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-22 16:57:11.028502 bykml-1.4.0/
--rw-rw-rw-   0        0        0     1061 2024-01-21 11:39:18.000000 bykml-1.4.0/LICENCE
--rw-rw-rw-   0        0        0       41 2024-01-22 13:48:38.000000 bykml-1.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1592 2024-01-22 16:57:11.026129 bykml-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1090 2024-01-22 11:09:53.000000 bykml-1.4.0/README.md
--rw-rw-rw-   0        0        0     1631 2024-01-22 16:56:39.000000 bykml-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-22 16:57:11.029162 bykml-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-22 16:57:10.992704 bykml-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2024-01-22 16:57:11.006353 bykml-1.4.0/src/bykml/
--rw-rw-rw-   0        0        0       21 2024-01-22 16:56:39.000000 bykml-1.4.0/src/bykml/__init__.py
--rw-rw-rw-   0        0        0       87 2024-01-21 11:33:23.000000 bykml-1.4.0/src/bykml/__main__.py
--rw-rw-rw-   0        0        0        0 2024-01-21 11:33:37.000000 bykml-1.4.0/src/bykml/config.toml
--rw-rw-rw-   0        0        0     1730 2024-01-22 16:36:57.000000 bykml-1.4.0/src/bykml/kmlfactory.py
-drwxrwxrwx   0        0        0        0 2024-01-22 16:57:11.023635 bykml-1.4.0/src/bykml.egg-info/
--rw-rw-rw-   0        0        0     1592 2024-01-22 16:57:10.000000 bykml-1.4.0/src/bykml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2024-01-22 16:57:10.000000 bykml-1.4.0/src/bykml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-22 16:57:10.000000 bykml-1.4.0/src/bykml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-01-22 16:57:10.000000 bykml-1.4.0/src/bykml.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2024-01-22 16:57:10.000000 bykml-1.4.0/src/bykml.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-01-22 16:57:10.000000 bykml-1.4.0/src/bykml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 09:50:11.629876 bykml-1.5.0/
+-rw-rw-rw-   0        0        0     1061 2024-01-21 11:39:18.000000 bykml-1.5.0/LICENCE
+-rw-rw-rw-   0        0        0       41 2024-01-22 13:48:38.000000 bykml-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1929 2024-04-29 09:50:11.625326 bykml-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1427 2024-04-29 09:34:53.000000 bykml-1.5.0/README.md
+-rw-rw-rw-   0        0        0     1631 2024-04-29 09:48:23.000000 bykml-1.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 09:50:11.629876 bykml-1.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 09:50:11.584340 bykml-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 09:50:11.602414 bykml-1.5.0/src/bykml/
+-rw-rw-rw-   0        0        0       21 2024-04-29 09:48:23.000000 bykml-1.5.0/src/bykml/__init__.py
+-rw-rw-rw-   0        0        0       87 2024-01-21 11:33:23.000000 bykml-1.5.0/src/bykml/__main__.py
+-rw-rw-rw-   0        0        0        0 2024-01-21 11:33:37.000000 bykml-1.5.0/src/bykml/config.toml
+-rw-rw-rw-   0        0        0     3186 2024-04-29 09:34:53.000000 bykml-1.5.0/src/bykml/kmlfactory.py
+drwxrwxrwx   0        0        0        0 2024-04-29 09:50:11.621990 bykml-1.5.0/src/bykml.egg-info/
+-rw-rw-rw-   0        0        0     1929 2024-04-29 09:50:11.000000 bykml-1.5.0/src/bykml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-04-29 09:50:11.000000 bykml-1.5.0/src/bykml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 09:50:11.000000 bykml-1.5.0/src/bykml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-29 09:50:11.000000 bykml-1.5.0/src/bykml.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2024-04-29 09:50:11.000000 bykml-1.5.0/src/bykml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 09:50:11.000000 bykml-1.5.0/src/bykml.egg-info/top_level.txt
```

### Comparing `bykml-1.4.0/LICENCE` & `bykml-1.5.0/LICENCE`

 * *Files identical despite different names*

### Comparing `bykml-1.4.0/PKG-INFO` & `bykml-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bykml
-Version: 1.4.0
+Version: 1.5.0
 Summary: the bykml library
 Author-email: Byron - Lloyd Wakeman <lloydwakemanbyron@gmail.com>
 Keywords: feed,bykml,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -16,15 +16,17 @@
 
 <h2>Introduction</h2>
 
 <p>bykml is a library to easily read, write and update KML files. 
 It's built around using dictionaries to easily replace values and add kml elements.</p>
 
 <h2>Documentation</h2>
-<p>Currently in progess...</p>
+<p>kmlfactory file inside the bykml package has a KmlFactory class and a placemark_template function 
+used to create placemarks and add to the 
+</p>
 
 <h2>Install</h2>
 <p>You can install the package with ```pip install bykml```</p>
 
 <h2>Dependencies</h2>
 <ul>
     <li><a href="https://pypi.org/project/xmltodict/">xmltodict</a></li>
@@ -34,14 +36,25 @@
 <p>Due to the nature of dictionaries of only being able to have one key per value.
 This subsequently means that lists have to be used to have multiple items within the same kml tag.
 For example if we have a 'Folder' tag which will contain a number of placemarks, 
 we cannot have a nested folder with multiple placemarks inside.
 This is currently being reviewed for a solution.</p>
 
 <h2>Changelog</h2>
+<h3>1.5.0 (29/04/2024)</h3>
+<ul>
+    <li>Updated placemark template to accept images</li>
+    <li>Updated function comments</li>
+</ul>
+
+<h3>1.4.0 (22/01/2024)</h3>
+<ul>
+    <li>Added kmlfactory</li>
+</ul>
+
 <h3>1.3.0 (22/01/2024)</h3>
 <ul>
     <li>Updated README</li>
 </ul>
 
 <h3>1.2.0 (22/01/2024)</h3>
 <ul>
```

#### html2text {}

```diff
@@ -1,29 +1,35 @@
-Metadata-Version: 2.1 Name: bykml Version: 1.4.0 Summary: the bykml library
+Metadata-Version: 2.1 Name: bykml Version: 1.5.0 Summary: the bykml library
 Author-email: Byron - Lloyd Wakeman
 gmail.com> Keywords: feed,bykml,tutorial Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENCE Requires-Dist: xmltodict Provides-Extra: dev
 Requires-Dist: bumpver; extra == "dev"
 ********** IInnttrroodduuccttiioonn **********
 bykml is a library to easily read, write and update KML files. It's built
 around using dictionaries to easily replace values and add kml elements.
 ********** DDooccuummeennttaattiioonn **********
-Currently in progess...
+kmlfactory file inside the bykml package has a KmlFactory class and a
+placemark_template function used to create placemarks and add to the
 ********** IInnssttaallll **********
 You can install the package with ```pip install bykml```
 ********** DDeeppeennddeenncciieess **********
     * _x_m_l_t_o_d_i_c_t
 ********** LLiimmiittaattiioonnss **********
 Due to the nature of dictionaries of only being able to have one key per value.
 This subsequently means that lists have to be used to have multiple items
 within the same kml tag. For example if we have a 'Folder' tag which will
 contain a number of placemarks, we cannot have a nested folder with multiple
 placemarks inside. This is currently being reviewed for a solution.
 ********** CChhaannggeelloogg **********
+******** 11..55..00 ((2299//0044//22002244)) ********
+    * Updated placemark template to accept images
+    * Updated function comments
+******** 11..44..00 ((2222//0011//22002244)) ********
+    * Added kmlfactory
 ******** 11..33..00 ((2222//0011//22002244)) ********
     * Updated README
 ******** 11..22..00 ((2222//0011//22002244)) ********
     * Updated maintainers
 ******** 11..11..00 ((2211//0011//22002244)) ********
     * Initial release
```

### Comparing `bykml-1.4.0/README.md` & `bykml-1.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 <h2>Introduction</h2>
 
 <p>bykml is a library to easily read, write and update KML files. 
 It's built around using dictionaries to easily replace values and add kml elements.</p>
 
 <h2>Documentation</h2>
-<p>Currently in progess...</p>
+<p>kmlfactory file inside the bykml package has a KmlFactory class and a placemark_template function 
+used to create placemarks and add to the 
+</p>
 
 <h2>Install</h2>
 <p>You can install the package with ```pip install bykml```</p>
 
 <h2>Dependencies</h2>
 <ul>
     <li><a href="https://pypi.org/project/xmltodict/">xmltodict</a></li>
@@ -18,14 +20,25 @@
 <p>Due to the nature of dictionaries of only being able to have one key per value.
 This subsequently means that lists have to be used to have multiple items within the same kml tag.
 For example if we have a 'Folder' tag which will contain a number of placemarks, 
 we cannot have a nested folder with multiple placemarks inside.
 This is currently being reviewed for a solution.</p>
 
 <h2>Changelog</h2>
+<h3>1.5.0 (29/04/2024)</h3>
+<ul>
+    <li>Updated placemark template to accept images</li>
+    <li>Updated function comments</li>
+</ul>
+
+<h3>1.4.0 (22/01/2024)</h3>
+<ul>
+    <li>Added kmlfactory</li>
+</ul>
+
 <h3>1.3.0 (22/01/2024)</h3>
 <ul>
     <li>Updated README</li>
 </ul>
 
 <h3>1.2.0 (22/01/2024)</h3>
 <ul>
```

#### html2text {}

```diff
@@ -1,22 +1,28 @@
 ********** IInnttrroodduuccttiioonn **********
 bykml is a library to easily read, write and update KML files. It's built
 around using dictionaries to easily replace values and add kml elements.
 ********** DDooccuummeennttaattiioonn **********
-Currently in progess...
+kmlfactory file inside the bykml package has a KmlFactory class and a
+placemark_template function used to create placemarks and add to the
 ********** IInnssttaallll **********
 You can install the package with ```pip install bykml```
 ********** DDeeppeennddeenncciieess **********
     * _x_m_l_t_o_d_i_c_t
 ********** LLiimmiittaattiioonnss **********
 Due to the nature of dictionaries of only being able to have one key per value.
 This subsequently means that lists have to be used to have multiple items
 within the same kml tag. For example if we have a 'Folder' tag which will
 contain a number of placemarks, we cannot have a nested folder with multiple
 placemarks inside. This is currently being reviewed for a solution.
 ********** CChhaannggeelloogg **********
+******** 11..55..00 ((2299//0044//22002244)) ********
+    * Updated placemark template to accept images
+    * Updated function comments
+******** 11..44..00 ((2222//0011//22002244)) ********
+    * Added kmlfactory
 ******** 11..33..00 ((2222//0011//22002244)) ********
     * Updated README
 ******** 11..22..00 ((2222//0011//22002244)) ********
     * Updated maintainers
 ******** 11..11..00 ((2211//0011//22002244)) ********
     * Initial release
```

### Comparing `bykml-1.4.0/pyproject.toml` & `bykml-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bykml"
-version = "1.4.0"
+version = "1.5.0"
 description = "the bykml library"
 readme = "README.md"
 authors = [{ name = "Byron - Lloyd Wakeman", email = "lloydwakemanbyron@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -28,27 +28,27 @@
 #[project.urls]
 #Homepage = "https://github.com/realpython/bykml"
 
 [project.scripts]
 realpython = "bykml.__main__:main"
 
 [tool.bumpver]
-current_version = "1.4.0"
+current_version = "1.5.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "src/bykml/__init__.py" = ["{version}"]
 
 #[tool.bumpver]
-#current_version = "1.4.0"
+#current_version = "1.5.0"
 #version_pattern = "MAJOR.MINOR.PATCH"
 #commit_message = "bump version {old_version} -> {new_version}"
 #tag_message = "{new_version}"
 #tag_scope = "default"
 #pre_commit_hook = ""
 #post_commit_hook = ""
 #commit = true
```

### Comparing `bykml-1.4.0/src/bykml/kmlfactory.py` & `bykml-1.5.0/src/bykml/kmlfactory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,59 @@
 import xmltodict
 
 
-def placemark_template(placemark_name, description, longitude, latitude, altitude, color="FF00FEB7"):
-    return {
-        "name": placemark_name,
-        "open": 1,
-        "Placemark": {
+def placemark_template(placemark_name, description, longitude, latitude, altitude, icon="", color="FF00FEB7"):
+    """
+    Placemark template is what will get passed through to the add_element function to be added to the kml document
+    :param placemark_name: The name of the placemark that will show up on Google (if empty input "")
+    :param description: Description of the placemark that will show when the user clicks on the placemark
+    :param longitude: The longitude of the placemark
+    :param latitude: The latitude of the placemark
+    :param altitude: The altitude of the placemark
+    :param icon: Optional parameter of a placemark image, such as http://maps.google.com/mapfiles/kml/shapes/caution.png
+    :param color: Color of the placemark as a html color value, default is FF00FEB7
+    :return: Dictionary of the placemark
+    """
+    if icon != "":
+        return {
             "name": placemark_name,
-            "description": description,
-            "Style": {
-                "IconStyle": {
-                    "color": color
+            "open": 1,
+            "Placemark": {
+                "name": placemark_name,
+                "description": description,
+                "Style": {
+                    "IconStyle": {
+                        "color": color,
+                        "Icon": {
+                            "href": icon
+                        }
+                    }
+                },
+                "Point": {
+                    "coordinates": str(f"{longitude},{latitude},{altitude}")
+                }
+            }
+        }
+    else:
+        return {
+            "name": placemark_name,
+            "open": 1,
+            "Placemark": {
+                "name": placemark_name,
+                "description": description,
+                "Style": {
+                    "IconStyle": {
+                        "color": color,
+                    }
+                },
+                "Point": {
+                    "coordinates": str(f"{longitude},{latitude},{altitude}")
                 }
-            },
-            "Point": {
-                "coordinates": str(f"{longitude},{latitude},{altitude}")
             }
         }
-    }
 
 
 class KmlFactory:
     def __init__(self, document_name):
         self.kml_dict = {
             "kml": {
                 "@xmlns": "http://www.opengis.net/kml/2.2",
@@ -44,10 +76,10 @@
             file.write(xml_content)
 
     def add_element(self, dict_element):
         """
         Add an element to the kml document in the form of a dict.
         You can pass through your custom dictionary or use one of the templates in the kmlfactory package.
         :param dict_element:
-        :return:
+        :return: None
         """
         self.kml_dict["kml"]["Document"]["Folder"].append(dict_element)
```

### Comparing `bykml-1.4.0/src/bykml.egg-info/PKG-INFO` & `bykml-1.5.0/src/bykml.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bykml
-Version: 1.4.0
+Version: 1.5.0
 Summary: the bykml library
 Author-email: Byron - Lloyd Wakeman <lloydwakemanbyron@gmail.com>
 Keywords: feed,bykml,tutorial
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -16,15 +16,17 @@
 
 <h2>Introduction</h2>
 
 <p>bykml is a library to easily read, write and update KML files. 
 It's built around using dictionaries to easily replace values and add kml elements.</p>
 
 <h2>Documentation</h2>
-<p>Currently in progess...</p>
+<p>kmlfactory file inside the bykml package has a KmlFactory class and a placemark_template function 
+used to create placemarks and add to the 
+</p>
 
 <h2>Install</h2>
 <p>You can install the package with ```pip install bykml```</p>
 
 <h2>Dependencies</h2>
 <ul>
     <li><a href="https://pypi.org/project/xmltodict/">xmltodict</a></li>
@@ -34,14 +36,25 @@
 <p>Due to the nature of dictionaries of only being able to have one key per value.
 This subsequently means that lists have to be used to have multiple items within the same kml tag.
 For example if we have a 'Folder' tag which will contain a number of placemarks, 
 we cannot have a nested folder with multiple placemarks inside.
 This is currently being reviewed for a solution.</p>
 
 <h2>Changelog</h2>
+<h3>1.5.0 (29/04/2024)</h3>
+<ul>
+    <li>Updated placemark template to accept images</li>
+    <li>Updated function comments</li>
+</ul>
+
+<h3>1.4.0 (22/01/2024)</h3>
+<ul>
+    <li>Added kmlfactory</li>
+</ul>
+
 <h3>1.3.0 (22/01/2024)</h3>
 <ul>
     <li>Updated README</li>
 </ul>
 
 <h3>1.2.0 (22/01/2024)</h3>
 <ul>
```

#### html2text {}

```diff
@@ -1,29 +1,35 @@
-Metadata-Version: 2.1 Name: bykml Version: 1.4.0 Summary: the bykml library
+Metadata-Version: 2.1 Name: bykml Version: 1.5.0 Summary: the bykml library
 Author-email: Byron - Lloyd Wakeman
 gmail.com> Keywords: feed,bykml,tutorial Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENCE Requires-Dist: xmltodict Provides-Extra: dev
 Requires-Dist: bumpver; extra == "dev"
 ********** IInnttrroodduuccttiioonn **********
 bykml is a library to easily read, write and update KML files. It's built
 around using dictionaries to easily replace values and add kml elements.
 ********** DDooccuummeennttaattiioonn **********
-Currently in progess...
+kmlfactory file inside the bykml package has a KmlFactory class and a
+placemark_template function used to create placemarks and add to the
 ********** IInnssttaallll **********
 You can install the package with ```pip install bykml```
 ********** DDeeppeennddeenncciieess **********
     * _x_m_l_t_o_d_i_c_t
 ********** LLiimmiittaattiioonnss **********
 Due to the nature of dictionaries of only being able to have one key per value.
 This subsequently means that lists have to be used to have multiple items
 within the same kml tag. For example if we have a 'Folder' tag which will
 contain a number of placemarks, we cannot have a nested folder with multiple
 placemarks inside. This is currently being reviewed for a solution.
 ********** CChhaannggeelloogg **********
+******** 11..55..00 ((2299//0044//22002244)) ********
+    * Updated placemark template to accept images
+    * Updated function comments
+******** 11..44..00 ((2222//0011//22002244)) ********
+    * Added kmlfactory
 ******** 11..33..00 ((2222//0011//22002244)) ********
     * Updated README
 ******** 11..22..00 ((2222//0011//22002244)) ********
     * Updated maintainers
 ******** 11..11..00 ((2211//0011//22002244)) ********
     * Initial release
```

