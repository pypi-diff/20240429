# Comparing `tmp/pydeflate-1.3.8.tar.gz` & `tmp/pydeflate-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydeflate-1.3.8.tar", max compression
+gzip compressed data, was "pydeflate-1.3.9.tar", max compression
```

## Comparing `pydeflate-1.3.8.tar` & `pydeflate-1.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1070 2023-07-06 12:30:27.744440 pydeflate-1.3.8/LICENSE
--rw-r--r--   0        0        0     8999 2023-07-06 12:30:27.744440 pydeflate-1.3.8/README.md
--rw-r--r--   0        0        0       25 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/.pydeflate_data/README.md
--rw-r--r--   0        0        0      817 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/deflate/__init__.py
--rw-r--r--   0        0        0    11850 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/deflate/deflate.py
--rw-r--r--   0        0        0     2684 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/deflate/deflator.py
--rw-r--r--   0        0        0        0 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/get_data/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/get_data/deflate_data.py
--rw-r--r--   0        0        0    12091 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/get_data/exchange_data.py
--rw-r--r--   0        0        0     2693 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/get_data/imf_data.py
--rw-r--r--   0        0        0     7535 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/get_data/oecd_data.py
--rw-r--r--   0        0        0     2103 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/get_data/wb_data.py
--rw-r--r--   0        0        0      894 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/pydeflate_config.py
--rw-r--r--   0        0        0      133 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/settings/emu.json
--rw-r--r--   0        0        0      911 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/settings/oecd_codes.json
--rw-r--r--   0        0        0       47 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/tools/__init__.py
--rw-r--r--   0        0        0     5465 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/tools/exchange.py
--rw-r--r--   0        0        0     2110 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/tools/update_data.py
--rw-r--r--   0        0        0     1573 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pydeflate/utils.py
--rw-r--r--   0        0        0     1049 2023-07-06 12:30:27.744440 pydeflate-1.3.8/pyproject.toml
--rw-r--r--   0        0        0    10028 1970-01-01 00:00:00.000000 pydeflate-1.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-12-11 14:25:14.349584 pydeflate-1.3.9/LICENSE
+-rw-r--r--   0        0        0     8999 2023-12-11 14:25:14.349584 pydeflate-1.3.9/README.md
+-rw-r--r--   0        0        0       25 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/.pydeflate_data/README.md
+-rw-r--r--   0        0        0      817 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/deflate/__init__.py
+-rw-r--r--   0        0        0    11850 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/deflate/deflate.py
+-rw-r--r--   0        0        0     2684 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/deflate/deflator.py
+-rw-r--r--   0        0        0        0 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/get_data/__init__.py
+-rw-r--r--   0        0        0     2285 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/get_data/deflate_data.py
+-rw-r--r--   0        0        0    12091 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/get_data/exchange_data.py
+-rw-r--r--   0        0        0     2693 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/get_data/imf_data.py
+-rw-r--r--   0        0        0     7535 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/get_data/oecd_data.py
+-rw-r--r--   0        0        0     2103 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/get_data/wb_data.py
+-rw-r--r--   0        0        0      894 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/pydeflate_config.py
+-rw-r--r--   0        0        0      133 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/settings/emu.json
+-rw-r--r--   0        0        0      911 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/settings/oecd_codes.json
+-rw-r--r--   0        0        0       47 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/tools/__init__.py
+-rw-r--r--   0        0        0     5465 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/tools/exchange.py
+-rw-r--r--   0        0        0     2110 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/tools/update_data.py
+-rw-r--r--   0        0        0     1573 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pydeflate/utils.py
+-rw-r--r--   0        0        0     1038 2023-12-11 14:25:14.353584 pydeflate-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0    10067 1970-01-01 00:00:00.000000 pydeflate-1.3.9/PKG-INFO
```

### Comparing `pydeflate-1.3.8/LICENSE` & `pydeflate-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/README.md` & `pydeflate-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/__init__.py` & `pydeflate-1.3.9/pydeflate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = """Jorge Rivera"""
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 
 from pydeflate.deflate.deflate import deflate
 from pydeflate.tools.exchange import exchange
 from pydeflate.tools.update_data import update_all_data, warn_updates
 from pydeflate.get_data.oecd_data import update_dac1
 from pydeflate import get_data
```

### Comparing `pydeflate-1.3.8/pydeflate/deflate/deflate.py` & `pydeflate-1.3.9/pydeflate/deflate/deflate.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/deflate/deflator.py` & `pydeflate-1.3.9/pydeflate/deflate/deflator.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/get_data/deflate_data.py` & `pydeflate-1.3.9/pydeflate/get_data/deflate_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/get_data/exchange_data.py` & `pydeflate-1.3.9/pydeflate/get_data/exchange_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/get_data/imf_data.py` & `pydeflate-1.3.9/pydeflate/get_data/imf_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/get_data/oecd_data.py` & `pydeflate-1.3.9/pydeflate/get_data/oecd_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/get_data/wb_data.py` & `pydeflate-1.3.9/pydeflate/get_data/wb_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/pydeflate_config.py` & `pydeflate-1.3.9/pydeflate/pydeflate_config.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/settings/oecd_codes.json` & `pydeflate-1.3.9/pydeflate/settings/oecd_codes.json`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/tools/exchange.py` & `pydeflate-1.3.9/pydeflate/tools/exchange.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/tools/update_data.py` & `pydeflate-1.3.9/pydeflate/tools/update_data.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pydeflate/utils.py` & `pydeflate-1.3.9/pydeflate/utils.py`

 * *Files identical despite different names*

### Comparing `pydeflate-1.3.8/pyproject.toml` & `pydeflate-1.3.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydeflate"
-version = "1.3.8"
+version = "1.3.9"
 description = "Package to convert current prices figures to constant prices and vice versa"
 authors = ["Jorge Rivera <jorge.rivera@one.org>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: End Users/Desktop',
@@ -17,28 +17,28 @@
 
 packages = [
     { include = "pydeflate" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-numpy = "^1.24.1"
-pandas = "^1.5.3"
+numpy = "^1.26"
+pandas = "^2"
 beautifulsoup4 = "^4.12"
 weo = "^0.7.4"
 xlrd = "^2.0.1"
 country-converter = "^1"
 requests = "^2.28.2"
-pyarrow = "^12.0"
-bblocks = "^1.1"
+pyarrow = "^14.0"
+bblocks = "^1.2"
 
 
 [tool.poetry.dev-dependencies]
 bump2version = "^1.0.1"
-black = "^22.12.0"
+black = "^23"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `pydeflate-1.3.8/PKG-INFO` & `pydeflate-1.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pydeflate
-Version: 1.3.8
+Version: 1.3.9
 Summary: Package to convert current prices figures to constant prices and vice versa
 License: MIT
 Author: Jorge Rivera
 Author-email: jorge.rivera@one.org
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bblocks (>=1.1,<2.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: bblocks (>=1.2,<2.0)
 Requires-Dist: beautifulsoup4 (>=4.12,<5.0)
 Requires-Dist: country-converter (>=1,<2)
-Requires-Dist: numpy (>=1.24.1,<2.0.0)
-Requires-Dist: pandas (>=1.5.3,<2.0.0)
-Requires-Dist: pyarrow (>=12.0,<13.0)
+Requires-Dist: numpy (>=1.26,<2.0)
+Requires-Dist: pandas (>=2,<3)
+Requires-Dist: pyarrow (>=14.0,<15.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: weo (>=0.7.4,<0.8.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # pydeflate
```

