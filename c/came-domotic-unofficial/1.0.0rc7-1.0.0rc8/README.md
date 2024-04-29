# Comparing `tmp/came_domotic_unofficial-1.0.0rc7.tar.gz` & `tmp/came_domotic_unofficial-1.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "came_domotic_unofficial-1.0.0rc7.tar", max compression
+gzip compressed data, was "came_domotic_unofficial-1.0.0rc8.tar", max compression
```

## Comparing `came_domotic_unofficial-1.0.0rc7.tar` & `came_domotic_unofficial-1.0.0rc8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/LICENSE
--rw-r--r--   0        0        0     5155 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/README.rst
--rw-r--r--   0        0        0     1633 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/__init__.py
--rw-r--r--   0        0        0     9212 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/auth.py
--rw-r--r--   0        0        0     4893 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/came_domotic_api.py
--rw-r--r--   0        0        0     1771 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/errors.py
--rw-r--r--   0        0        0     6343 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models.py
--rw-r--r--   0        0        0     1333 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/__init__.py
--rw-r--r--   0        0        0     5249 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/came_entity.py
--rw-r--r--   0        0        0     8532 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/digital_input.py
--rw-r--r--   0        0        0     2768 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/enums.py
--rw-r--r--   0        0        0     2002 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/exceptions.py
--rw-r--r--   0        0        0     3589 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/feature.py
--rw-r--r--   0        0        0     1587 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/helpers.py
--rw-r--r--   0        0        0     5930 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/light.py
--rw-r--r--   0        0        0     6451 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/opening.py
--rw-r--r--   0        0        0     6912 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/scenario.py
--rw-r--r--   0        0        0     2902 2024-04-28 19:55:23.498479 came_domotic_unofficial-1.0.0rc7/pyproject.toml
--rw-r--r--   0        0        0     6534 1970-01-01 00:00:00.000000 came_domotic_unofficial-1.0.0rc7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-28 23:50:01.862023 came_domotic_unofficial-1.0.0rc8/LICENSE
+-rw-r--r--   0        0        0     5155 2024-04-28 23:50:01.862023 came_domotic_unofficial-1.0.0rc8/README.rst
+-rw-r--r--   0        0        0     1633 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/__init__.py
+-rw-r--r--   0        0        0     9212 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/auth.py
+-rw-r--r--   0        0        0     4893 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/came_domotic_api.py
+-rw-r--r--   0        0        0     1771 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/errors.py
+-rw-r--r--   0        0        0     6343 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models.py
+-rw-r--r--   0        0        0     1333 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/__init__.py
+-rw-r--r--   0        0        0     5249 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/came_entity.py
+-rw-r--r--   0        0        0     8532 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/digital_input.py
+-rw-r--r--   0        0        0     2768 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/enums.py
+-rw-r--r--   0        0        0     2002 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/exceptions.py
+-rw-r--r--   0        0        0     3589 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/feature.py
+-rw-r--r--   0        0        0     1587 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/helpers.py
+-rw-r--r--   0        0        0     5930 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/light.py
+-rw-r--r--   0        0        0     6451 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/opening.py
+-rw-r--r--   0        0        0     6912 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/scenario.py
+-rw-r--r--   0        0        0     2856 2024-04-28 23:50:01.866023 came_domotic_unofficial-1.0.0rc8/pyproject.toml
+-rw-r--r--   0        0        0     6483 1970-01-01 00:00:00.000000 came_domotic_unofficial-1.0.0rc8/PKG-INFO
```

### Comparing `came_domotic_unofficial-1.0.0rc7/LICENSE` & `came_domotic_unofficial-1.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/README.rst` & `came_domotic_unofficial-1.0.0rc8/README.rst`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/__init__.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/__init__.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/auth.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/auth.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/came_domotic_api.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/came_domotic_api.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/errors.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/errors.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/__init__.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/__init__.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/came_entity.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/came_entity.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/digital_input.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/digital_input.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/enums.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/enums.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/exceptions.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/exceptions.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/feature.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/feature.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/helpers.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/helpers.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/light.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/light.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/opening.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/opening.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/came_domotic_unofficial/models_OLD/scenario.py` & `came_domotic_unofficial-1.0.0rc8/came_domotic_unofficial/models_OLD/scenario.py`

 * *Files identical despite different names*

### Comparing `came_domotic_unofficial-1.0.0rc7/pyproject.toml` & `came_domotic_unofficial-1.0.0rc8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License. 
 
 [tool.poetry]
 name = "came_domotic_unofficial"
-version = "1.0.0rc7"
+version = "1.0.0rc8"
 description = "Python library to interact with a CAME ETI/Domo domotic server."
 license = "Apache-2.0"
 authors = ["camedomotic-unofficial <camedomotic-unofficial@gmail.com>"]
 maintainers = ["camedomotic-unofficial <camedomotic-unofficial@gmail.com>"]
 readme = "README.rst"
 
 homepage = "https://github.com/camedomotic-unofficial/came_domotic_unofficial"
@@ -34,15 +34,14 @@
     "home-assistant",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.12",
-    "Programming Language :: Python :: 3.13",
     "Topic :: Home Automation",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Operating System :: OS Independent",
 ]
 
 packages = [{ include = "came_domotic_unofficial" }]
```

### Comparing `came_domotic_unofficial-1.0.0rc7/PKG-INFO` & `came_domotic_unofficial-1.0.0rc8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: came_domotic_unofficial
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: Python library to interact with a CAME ETI/Domo domotic server.
 Home-page: https://github.com/camedomotic-unofficial/came_domotic_unofficial
 License: Apache-2.0
 Keywords: CAME,ETI/Domo,domotic,home automation,home assistant,home-assistant
 Author: camedomotic-unofficial
 Author-email: camedomotic-unofficial@gmail.com
 Maintainer: camedomotic-unofficial
@@ -12,15 +12,14 @@
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug tracker, https://github.com/camedomotic-unofficial/came_domotic_unofficial/issues
 Project-URL: Documentation, https://came-domotic-unofficial.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/camedomotic-unofficial/came_domotic_unofficial.git
```

