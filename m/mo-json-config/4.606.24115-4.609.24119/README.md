# Comparing `tmp/mo_json_config-4.606.24115.tar.gz` & `tmp/mo_json_config-4.609.24119.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_json_config-4.606.24115.tar", last modified: Wed Apr 24 23:36:06 2024, max compression
+gzip compressed data, was "mo_json_config-4.609.24119.tar", last modified: Sun Apr 28 22:32:27 2024, max compression
```

## Comparing `mo_json_config-4.606.24115.tar` & `mo_json_config-4.609.24119.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 23:36:06.052559 mo_json_config-4.606.24115/
--rw-rw-rw-   0        0        0    16725 2019-11-12 21:32:58.000000 mo_json_config-4.606.24115/LICENSE.txt
--rw-rw-rw-   0        0        0    11685 2024-04-24 23:36:06.051560 mo_json_config-4.606.24115/PKG-INFO
--rw-rw-rw-   0        0        0     9939 2024-03-08 02:34:29.000000 mo_json_config-4.606.24115/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 23:36:06.026620 mo_json_config-4.606.24115/mo_json_config/
--rw-rw-rw-   0        0        0    11234 2024-03-10 19:25:57.000000 mo_json_config-4.606.24115/mo_json_config/__init__.py
--rw-rw-rw-   0        0        0     2411 2023-04-29 14:14:40.000000 mo_json_config-4.606.24115/mo_json_config/configuration.py
--rw-rw-rw-   0        0        0      697 2023-06-02 01:48:46.000000 mo_json_config-4.606.24115/mo_json_config/convert.py
--rw-rw-rw-   0        0        0     3113 2024-03-08 02:34:29.000000 mo_json_config-4.606.24115/mo_json_config/ssm.py
-drwxrwxrwx   0        0        0        0 2024-04-24 23:36:06.049550 mo_json_config-4.606.24115/mo_json_config.egg-info/
--rw-rw-rw-   0        0        0    11685 2024-04-24 23:36:06.000000 mo_json_config-4.606.24115/mo_json_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2024-04-24 23:36:06.000000 mo_json_config-4.606.24115/mo_json_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 23:36:06.000000 mo_json_config-4.606.24115/mo_json_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      207 2024-04-24 23:36:06.000000 mo_json_config-4.606.24115/mo_json_config.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-24 23:36:06.000000 mo_json_config-4.606.24115/mo_json_config.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 23:36:06.052559 mo_json_config-4.606.24115/setup.cfg
--rw-rw-rw-   0        0        0    11541 2024-04-24 23:36:01.000000 mo_json_config-4.606.24115/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 22:32:27.535232 mo_json_config-4.609.24119/
+-rw-rw-rw-   0        0        0    16725 2019-11-12 21:32:58.000000 mo_json_config-4.609.24119/LICENSE.txt
+-rw-rw-rw-   0        0        0    11683 2024-04-28 22:32:27.534182 mo_json_config-4.609.24119/PKG-INFO
+-rw-rw-rw-   0        0        0     9937 2024-04-28 22:32:20.000000 mo_json_config-4.609.24119/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 22:32:27.518296 mo_json_config-4.609.24119/mo_json_config/
+-rw-rw-rw-   0        0        0    11437 2024-04-28 22:32:20.000000 mo_json_config-4.609.24119/mo_json_config/__init__.py
+-rw-rw-rw-   0        0        0     2409 2024-04-28 22:32:20.000000 mo_json_config-4.609.24119/mo_json_config/configuration.py
+-rw-rw-rw-   0        0        0      697 2023-06-02 01:48:46.000000 mo_json_config-4.609.24119/mo_json_config/convert.py
+-rw-rw-rw-   0        0        0     3111 2024-04-28 22:32:20.000000 mo_json_config-4.609.24119/mo_json_config/ssm.py
+drwxrwxrwx   0        0        0        0 2024-04-28 22:32:27.532680 mo_json_config-4.609.24119/mo_json_config.egg-info/
+-rw-rw-rw-   0        0        0    11683 2024-04-28 22:32:27.000000 mo_json_config-4.609.24119/mo_json_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-28 22:32:27.000000 mo_json_config-4.609.24119/mo_json_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 22:32:27.000000 mo_json_config-4.609.24119/mo_json_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      207 2024-04-28 22:32:27.000000 mo_json_config-4.609.24119/mo_json_config.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-28 22:32:27.000000 mo_json_config-4.609.24119/mo_json_config.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-28 22:32:27.535232 mo_json_config-4.609.24119/setup.cfg
+-rw-rw-rw-   0        0        0    11539 2024-04-28 22:32:23.000000 mo_json_config-4.609.24119/setup.py
```

### Comparing `mo_json_config-4.606.24115/LICENSE.txt` & `mo_json_config-4.609.24119/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mo_json_config-4.606.24115/PKG-INFO` & `mo_json_config-4.609.24119/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json-config
-Version: 4.606.24115
+Version: 4.609.24119
 Summary: More JSON Configuration! JSON configuration files with `$ref` and template overlays
 Home-page: https://github.com/klahnakoski/mo-json-config
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -15,18 +15,18 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: hjson
 Requires-Dist: mo-dots==9.606.24115
-Requires-Dist: mo-files==6.606.24115
+Requires-Dist: mo-files==6.609.24119
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.606.24115
-Requires-Dist: mo-logs==8.606.24115
+Requires-Dist: mo-json==6.609.24119
+Requires-Dist: mo-logs==8.608.24119
 Requires-Dist: requests
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 Requires-Dist: keyring>=25.1.0; extra == "tests"
 Requires-Dist: boto3>=1.34.91; extra == "tests"
 Requires-Dist: pyyaml; extra == "tests"
 Requires-Dist: moto>=4.2.14; extra == "tests"
@@ -359,15 +359,15 @@
 
 ## Parameterized JSON
 
 The `param` scheme is a good way to set property values in a document, but sometimes that is not enough.  Sometimes you want to parameterize property names, or change the document structure in unconventional ways. For these cases, JSON documents are allowed named parameters at the unicode level. Parameters are surrounded by moustaches `{{.}}`:
 
 ```javascript
 {//above_example.json
-    {{var_name}}: "value"
+    {var_name}: "value"
 }
 ```
 
 Parameter replacement is performed on the unicode text before being interpreted by the JSON parser. It is your responsibility to ensure the parameter replacement will result in valid JSON.
 
 You pass the parameters by including them as URL parameters:
```

### Comparing `mo_json_config-4.606.24115/README.md` & `mo_json_config-4.609.24119/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 
 ## Parameterized JSON
 
 The `param` scheme is a good way to set property values in a document, but sometimes that is not enough.  Sometimes you want to parameterize property names, or change the document structure in unconventional ways. For these cases, JSON documents are allowed named parameters at the unicode level. Parameters are surrounded by moustaches `{{.}}`:
 
 ```javascript
 {//above_example.json
-    {{var_name}}: "value"
+    {var_name}: "value"
 }
 ```
 
 Parameter replacement is performed on the unicode text before being interpreted by the JSON parser. It is your responsibility to ensure the parameter replacement will result in valid JSON.
 
 You pass the parameters by including them as URL parameters:
```

### Comparing `mo_json_config-4.606.24115/mo_json_config/__init__.py` & `mo_json_config-4.609.24119/mo_json_config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,61 +22,67 @@
     get_attr,
     listwrap,
     unwraplist,
     dict_to_data,
 )
 from mo_files import File
 from mo_files.url import URL
+from mo_future import first
 from mo_json import json2value
 from mo_logs import Except, logger, get_stacktrace
 
 from mo_json_config.configuration import Configuration
 from mo_json_config.convert import ini2value
 from mo_json_config.ssm import get_ssm as _get_ssm
 
+CAN_NOT_READ_FILE = "Can not read file {filename}"
 DEBUG = False
 
 
 def get_file(file):
     file = File(file)
     return get("file://" + file.abs_path)
 
 
 def get(url):
     """
     USE json.net CONVENTIONS TO LINK TO INLINE OTHER JSON
     """
     url = str(url)
     if "://" not in url:
-        logger.error("{{url}} must have a prototcol (eg http://) declared", url=url)
+        logger.error("{url} must have a prototcol (eg http://) declared", url=url)
     path = (dict_to_data({"$ref": url}), None)
 
     if url.startswith("file://") and url[7] != "/":
         causes= []
         candidates = [os.path.dirname(os.path.abspath(get_stacktrace(start=1)[0]['file'])), os.getcwd()]
         for candidate in candidates:
             if os.sep == "\\":
                 base = URL("file:///" + candidate.replace(os.sep, "/").rstrip("/") + "/.")
             else:
                 base = URL("file://" + candidate.rstrip("/") + "/.")
             try:
                 phase1 = _replace_ref(path, base)
                 break
             except Exception as cause:
-                causes.append(cause)
+                if CAN_NOT_READ_FILE in cause:
+                    # lower priority cause
+                    causes.append(cause)
+                else:
+                    causes.insert(0, cause)
         else:
-            logger.error("problem replacing ref in {{url}}", url=url, cause=causes)
+            logger.error("problem replacing ref in {url}", url=url, cause=first(causes))
     else:
         phase1 = _replace_ref(path, URL(""))  # BLANK URL ONLY WORKS IF url IS ABSOLUTE
 
     try:
         phase2 = _replace_locals((phase1,None), url)
         return to_data(phase2)
     except Exception as cause:
-        logger.error("problem replacing locals in\n{{phase1}}", phase1=phase1, cause=cause)
+        logger.error("problem replacing locals in\n{phase1}", phase1=phase1, cause=cause)
 
 
 def expand(doc, doc_url="param://", params=None):
     """
     ASSUMING YOU ALREADY PULED THE doc FROM doc_url, YOU CAN STILL USE THE
     EXPANDING FEATURE
 
@@ -84,15 +90,15 @@
 
     :param doc: THE DATA STRUCTURE FROM JSON SOURCE
     :param doc_url: THE URL THIS doc CAME FROM (DEFAULT USES params AS A DOCUMENT SOURCE)
     :param params: EXTRA PARAMETERS NOT FOUND IN THE doc_url PARAMETERS (WILL SUPERSEDE PARAMETERS FROM doc_url)
     :return: EXPANDED JSON-SERIALIZABLE STRUCTURE
     """
     if "://" not in doc_url:
-        logger.error("{{url}} must have a protocol (eg https://) declared", url=doc_url)
+        logger.error("{url} must have a protocol (eg https://) declared", url=doc_url)
 
     url = URL(doc_url)
     url.query = set_default(url.query, params)
     phase1 = _replace_ref((doc, None), url)  # BLANK URL ONLY WORKS IF url IS ABSOLUTE
     phase2 = _replace_locals((phase1,None), url)
     return to_data(phase2)
 
@@ -151,39 +157,39 @@
             if not ref.scheme:
                 # SCHEME RELATIVE IMPLIES SAME PROTOCOL AS LAST TIME, WHICH
                 # REQUIRES THE CURRENT DOCUMENT'S SCHEME
                 ref.scheme = url.scheme
 
             # FIND THE SCHEME AND LOAD IT
             if ref.scheme not in scheme_loaders:
-                raise logger.error("unknown protocol {{scheme}}", scheme=ref.scheme)
+                raise logger.error("unknown protocol {scheme}", scheme=ref.scheme)
             try:
                 new_value = scheme_loaders[ref.scheme](ref, (node, path), url)
                 ref_found = True
             except Exception as cause:
                 ref_error = Except.wrap(cause)
                 continue
 
             if ref.fragment:
                 new_value = get_attr(new_value, ref.fragment)
 
-            DEBUG and logger.note("Replace {{ref}} with {{new_value}}", ref=ref, new_value=new_value)
+            DEBUG and logger.note("Replace {ref} with {new_value}", ref=ref, new_value=new_value)
 
             if not output:
                 output = new_value
             elif isinstance(output, str):
                 pass  # WE HAVE A VALUE
             else:
                 set_default(output, new_value)
 
         if not ref_found:
             raise ref_error
         if ref_remain:
             output["$ref"] = unwraplist(ref_remain)
-        DEBUG and logger.note("Return {{output}}", output=output)
+        DEBUG and logger.note("Return {output}", output=output)
         return output
     elif is_list(node):
         output = [_replace_ref((n, path), url) for n in node]
         return output
 
     return node
 
@@ -275,28 +281,28 @@
         else:
             parent = url.path.rstrip("/").split("/")[:-1]
             ref.path = "/".join(parent) + "/" + ref.path
 
     path = ref.path if os.sep != "\\" else ref.path[1::].replace("/", "\\")
 
     try:
-        DEBUG and logger.note("reading file {{path}}", path=path)
+        DEBUG and logger.note("reading file {path}", path=path)
         content = File(path).read()
     except Exception as e:
         content = None
-        logger.error("Could not read file {{filename}}", filename=File(path).os_path, cause=e)
+        logger.error(CAN_NOT_READ_FILE, filename=File(path).os_path, cause=e)
 
     try:
         new_value = json2value(content, params=ref.query, flexible=True, leaves=True)
     except Exception as e:
         e = Except.wrap(e)
         try:
             new_value = ini2value(content)
         except Exception:
-            raise logger.error("Can not read {{file}}", file=path, cause=e)
+            raise logger.error(CAN_NOT_READ_FILE, filename=path, cause=e)
     new_value = _replace_ref((new_value, path), ref)
     return new_value
 
 
 def get_http(ref, doc_path, url):
     import requests
 
@@ -306,15 +312,15 @@
 
 
 def _get_env(ref, doc_path, url):
     # GET ENVIRONMENT VARIABLES
     ref = ref.host
     raw_value = os.environ.get(ref)
     if not raw_value:
-        logger.error("expecting environment variable with name {{env_var}}", env_var=ref)
+        logger.error("expecting environment variable with name {env_var}", env_var=ref)
 
     try:
         new_value = json2value(raw_value)
     except Exception as e:
         new_value = raw_value
     return new_value
 
@@ -331,15 +337,15 @@
         username, service_name = service_name.split("@")
     else:
         username = ref.query.username
 
     raw_value = keyring.get_password(service_name, username)
     if not raw_value:
         logger.error(
-            "expecting password in the keyring for service_name={{service_name}} and username={{username}}",
+            "expecting password in the keyring for service_name={service_name} and username={username}",
             service_name=service_name,
             username=username,
         )
 
     try:
         new_value = json2value(raw_value)
     except Exception as e:
```

### Comparing `mo_json_config-4.606.24115/mo_json_config/configuration.py` & `mo_json_config-4.609.24119/mo_json_config/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from mo_logs import logger
 from mo_logs.strings import wordify
 
 
 class Configuration(Mapping):
     def __init__(self, config, path="."):
         if not isinstance(config, Mapping) and not is_data(config):
-            logger.error("Expecting data, not {{config}}", config=config)
+            logger.error("Expecting data, not {config}", config=config)
         self._path = path
         self._lookup = leaves_to_data({
             join_field(wordify(path)): value for path, value in Data(**config).leaves()
         })
 
     def __iter__(self):
         return (k for k, _ in self._lookup.leaves())
```

### Comparing `mo_json_config-4.606.24115/mo_json_config/convert.py` & `mo_json_config-4.609.24119/mo_json_config/convert.py`

 * *Files identical despite different names*

### Comparing `mo_json_config-4.606.24115/mo_json_config/ssm.py` & `mo_json_config-4.609.24119/mo_json_config/ssm.py`

 * *Files 8% similar despite different names*

```diff
@@ -92,10 +92,10 @@
             result = describe_parameters(NextToken=next_token, MaxResults=10, ParameterFilters=filters)
     except Exception as cause:
         has_failed = True
         logger.warning("Could not get ssm parameters", cause=cause)
         return output
 
     if len(output) == 0:
-        logger.error("No ssm parameters found at {{path}}", path=ref.path)
+        logger.error("No ssm parameters found at {path}", path=ref.path)
     return output
```

### Comparing `mo_json_config-4.606.24115/mo_json_config.egg-info/PKG-INFO` & `mo_json_config-4.609.24119/mo_json_config.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-json-config
-Version: 4.606.24115
+Version: 4.609.24119
 Summary: More JSON Configuration! JSON configuration files with `$ref` and template overlays
 Home-page: https://github.com/klahnakoski/mo-json-config
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries
@@ -15,18 +15,18 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: hjson
 Requires-Dist: mo-dots==9.606.24115
-Requires-Dist: mo-files==6.606.24115
+Requires-Dist: mo-files==6.609.24119
 Requires-Dist: mo-future==7.584.24095
-Requires-Dist: mo-json==6.606.24115
-Requires-Dist: mo-logs==8.606.24115
+Requires-Dist: mo-json==6.609.24119
+Requires-Dist: mo-logs==8.608.24119
 Requires-Dist: requests
 Provides-Extra: tests
 Requires-Dist: mo-testing>=8.591.24112; extra == "tests"
 Requires-Dist: keyring>=25.1.0; extra == "tests"
 Requires-Dist: boto3>=1.34.91; extra == "tests"
 Requires-Dist: pyyaml; extra == "tests"
 Requires-Dist: moto>=4.2.14; extra == "tests"
@@ -359,15 +359,15 @@
 
 ## Parameterized JSON
 
 The `param` scheme is a good way to set property values in a document, but sometimes that is not enough.  Sometimes you want to parameterize property names, or change the document structure in unconventional ways. For these cases, JSON documents are allowed named parameters at the unicode level. Parameters are surrounded by moustaches `{{.}}`:
 
 ```javascript
 {//above_example.json
-    {{var_name}}: "value"
+    {var_name}: "value"
 }
 ```
 
 Parameter replacement is performed on the unicode text before being interpreted by the JSON parser. It is your responsibility to ensure the parameter replacement will result in valid JSON.
 
 You pass the parameters by including them as URL parameters:
```

### Comparing `mo_json_config-4.606.24115/setup.py` & `mo_json_config-4.609.24119/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 4 - Beta","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","Programming Language :: Python :: 3.10","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More JSON Configuration! JSON configuration files with `$ref` and template overlays',
     extras_require={"tests":["mo-testing>=8.591.24112","keyring>=25.1.0","boto3>=1.34.91","pyyaml","moto>=4.2.14"]},
-    install_requires=["hjson","mo-dots==9.606.24115","mo-files==6.606.24115","mo-future==7.584.24095","mo-json==6.606.24115","mo-logs==8.606.24115","requests"],
+    install_requires=["hjson","mo-dots==9.606.24115","mo-files==6.609.24119","mo-future==7.584.24095","mo-json==6.609.24119","mo-logs==8.608.24119","requests"],
     license='MPL 2.0',
-    long_description='# More JSON Configuration!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-json-config.svg)](https://pypi.org/project/mo-json-config/)\n[![Build Status](https://github.com/klahnakoski/mo-json-config/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-json-config/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-json-config/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-json-config?branch=dev)\n\nA JSON template format intended for configuration files.\n\n## Motivation\n\nThis module reads JSON files and expands references found within. It is much like the IETF\'s  [JSON Reference](https://tools.ietf.org/html/draft-pbryan-zyp-json-ref-03) specification, but with the following differences:\n\n1. This module uses the dot (`.`) as a path separator in the URL fragment. For example, an absolute reference looks like `{"$ref": "#message.type.name"}`, and a relative reference looks like `{"$ref": "#..type.name"}`.   This syntax better matches that used by Javascript.\n2. The properties found in a `$ref` object are not ignored. Rather, they are to *override* the referenced object properties. This allows you to reference a default document, and replace the particular properties as needed. *more below*\n3. References can accept URL parameters: JSON is treated like a string template for more sophisticated value replacement. *see below*\n4. You can reference files and environment variables in addition to general URLs.\n\n## Quick guide\n\nLoad your configuration file:\n\n```python\nimport mo_json_config\n\nconfig = mo_json_config.get("file://my_config.json")\n```\n\nYou may use the global `configuration` object for case-insensitive lookup:\n\n\n```python\nfrom mo_json_config import configuration\n\n# use |= operator to add more configuration\nconfiguration |= {"some":{"deep":"value"}}\n\nassert configuration.someDeep == "value"\n\n```\n\n\n\n\n## Schemes\n\nThis module can load configuration from a number of sources, and you can access them via URI scheme.  Beyond the common `file` and `http` schemes, there are\n\n\n### Environment Variables\n\nUse the `env` scheme for accessing environment variables:\n\n    {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "env://MAIL_PASSWORD"}\n    }\n\n\n### Keystore Values\n\nThe [keyring](https://pypi.org/project/keyring/) library can be used with the `keyring` scheme:\n \n    {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "keyring://ekyle@mail.example.com"}\n    }\n\nThe host is in `<username>@<server_name>` format; invoking `keyring.get_password(server_name, username)`.  You may also set the username as a parameter:\n\n\n    {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "keyring://mail.example.com?username=ekyle"}\n    }\n\n> Be sure to `pip install keyring` to use keyring\n\n\n### AWS SSM\n\nThe `ssm` scheme can be used to read from the AWS parameter store.  Here is an example that will read all parameters that start with "/configuration" and adds them to the global configuration object:\n\n```python\nfrom mo_json_config import get, configuration\n\nconfiguration |= get("ssm:///configuration")\n```\n  \n\n## Using references in config files\n\nThe `$ref` property is special. Its value is interpreted as a URL pointing to more JSON\n\n\n### Absolute Internal Reference\n\nThe simplest form of URL is an absolute reference to a node in the same\ndocument:\n\n\n    {\n        "message": "Hello world",\n        "repeat": {"$ref": "#message"}\n    }\n\n\nThe reference must start with `#`, and the object with the `$ref` is replaced\nwith the value it points to:\n\n\n    {\n        "message": "Hello world",\n        "repeat": "Hello world"\n    }\n\n\n### Relative Internal References\n\nReferences that start with dot (`.`) are relative, with each additional dot\nreferring to successive parents.   In this case the `..` refers to the\nref-object\'s parent, and expands just like the previous example:\n\n\n    {\n        "message": "Hello world",\n        "repeat": {"$ref": "#..message"}\n    }\n\n\n### File References\n\nConfiguration is often stored on the local file system. You can in-line the\nJSON found in a file by using the `file://` scheme:\n\nIt is good practice to store sensitive data in a secure place...\n\n\n    {# LOCATED IN C:\\users\\kyle\\password.json\n        "host": "database.example.com",\n        "username": "kyle",\n        "password": "pass123"\n    }\n\n...and then refer to it in your configuration file:\n\n\n    {\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file:///C:/users/kyle/password.json"\n    }\n\n\nwhich will be expanded at run-time to:\n\n\n    {\n        "host": "example.com",\n        "port": "8080",\n        "username": "kyle",\n        "password": "pass123"\n    }\n\n\nPlease notice the triple slash (`///`) is referring to an absolute file\nreference.\n\n### References To Objects\n\nRef-objects that point to other objects (dicts) are not replaced completely,\nbut rather are merged with the target; with the ref-object\nproperties taking precedence.   This is seen in the example above: The "host"\nproperty is not overwritten by the target\'s.\n\n### Relative File Reference\n\nHere is the same, using a relative file reference; which is relative to the\nfile that contains this JSON\n\n\n    {#LOCATED IN C:\\users\\kyle\\dev-debug.json\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file://password.json"\n    }\n    \n\n### Home Directory Reference\n\nYou may also use the tilde (`~`) to refer to the current user\'s home directory.\nHere is the same again, but this example can be anywhere in the file system.\n\n\n    {\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file://~/password.json"\n    }\n\n\n### HTTP Reference\n\nConfiguration can be stored remotely, especially in the case of larger\nconfigurations which are too unwieldy to inline:\n\n\n    {\n        "schema":{"$ref": "https://example.com/sources/my_db.json"}\n    }\n\n\n### Scheme-Relative Reference\n\nYou are also able to leave the scheme off, so that whole constellations of\nconfiguration files can refer to each other no matter if they are on the local\nfile system, or remote:\n\n\n    {# LOCATED AT SOMEWHERE AT http://example.com\n        "schema":{"$ref": "///sources/my_db.json"}\n    }\n\n\nAnd, of course, relative references are also allowed:\n\n\n    {# LOCATED AT http://example.com/sources/dev-debug.json\n        "schema":{"$ref": "//sources/my_db.json"}\n    }\n\n\n### Fragment Reference\n\nSome remote configuration files are quite large...\n\n    {# LOCATED IN C:\\users\\kyle\\password.json\n        "database":{\n            "username": "kyle",\n            "password": "pass123"\n        },\n        "email":{\n            "username": "ekyle",\n            "password": "pass123"\n        }\n    }\n\n... and you only need one fragment. For this use the hash (`#`) followed by\nthe dot-delimited path into the document:\n\n    {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "//~/password.json#email.password"}\n    }\n\n### Parameters Reference\n\nYou can reference the variables found in `$ref` URL by using the `param` scheme. For example, the following JSON document demands that it be provided with a `password` parameter:  \n\n    { # LOCATED AT http://example.com/machine_config.json\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "param:///password"}\n    }\n\n> The `param` scheme only accepts dot-delimited paths.\n\nThe above parametric JSON can be expanded with a $ref\n\n\t{"config": {\n\t\t"$ref": "http://example.com/machine_config.json?password=pass123"\n\t}}\n\nexpands to \n\n    {"config": {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": "pass123"\n    }}\n\nURL parameters and `$ref` properties can conflict. Let\'s consider \n\n\t{"config": {\n\t\t"$ref": "http://example.com/machine_config.json?password=pass123",\n\t\t"password": "123456"\n\t}}\n\nthe URL paramters are used to expand the given document, **then** the `$ref` properties override the contents of the document:\n\n    {"config": {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": "123456"\n    }}\n\n\n## Comments\n\nEnd-of-line Comments are allowed, using either `#` or `//` prefix:\n\n```\n    "key1": "value1",  //Comment 1\n```\n\n```\n    "key1": "value1",  # Comment 1\n```\n\nMultiline comments are also allowed, using either Python\'s triple-quotes\n(`""" ... """`) or Javascript\'s block quotes `/*...*/`\n\n```\n{\n    "key1": /* Comment 1 */ "value1",\n}\n```\n\n```\n    "key1": """Comment 1""" "value1",\n```\n\n\n## Parameterized JSON\n\nThe `param` scheme is a good way to set property values in a document, but sometimes that is not enough.  Sometimes you want to parameterize property names, or change the document structure in unconventional ways. For these cases, JSON documents are allowed named parameters at the unicode level. Parameters are surrounded by moustaches `{{.}}`:\n\n```javascript\n{//above_example.json\n    {{var_name}}: "value"\n}\n```\n\nParameter replacement is performed on the unicode text before being interpreted by the JSON parser. It is your responsibility to ensure the parameter replacement will result in valid JSON.\n\nYou pass the parameters by including them as URL parameters:\n\n\t{"$ref": "//~/above_example.json?var_name=%22hello%22"}\n\nWhich will expand to\n\n    {\n        "hello": "value"\n    }\n\nThe pipe (`|`) symbol can be used to perform some common conversions\n\n\n    {\n        {{var_name|quote}}: "value"\n    }\n\nThe `quote` transformation will deal with quoting, so ...\n\n\t{"$ref": "//~/above_example.json?var_name=hello"}\n\n... expands to the same:\n\n    {\n        "hello": "value"\n    }\n\nPlease see [`expand_template()` in the `strings` module](https://github.com/klahnakoski/mo-logs/blob/dev/mo_logs/strings.py) for more on the parameter replacement, and transformations available\n\n',
+    long_description='# More JSON Configuration!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-json-config.svg)](https://pypi.org/project/mo-json-config/)\n[![Build Status](https://github.com/klahnakoski/mo-json-config/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/klahnakoski/mo-json-config/actions/workflows/build.yml)\n[![Coverage Status](https://coveralls.io/repos/github/klahnakoski/mo-json-config/badge.svg?branch=dev)](https://coveralls.io/github/klahnakoski/mo-json-config?branch=dev)\n\nA JSON template format intended for configuration files.\n\n## Motivation\n\nThis module reads JSON files and expands references found within. It is much like the IETF\'s  [JSON Reference](https://tools.ietf.org/html/draft-pbryan-zyp-json-ref-03) specification, but with the following differences:\n\n1. This module uses the dot (`.`) as a path separator in the URL fragment. For example, an absolute reference looks like `{"$ref": "#message.type.name"}`, and a relative reference looks like `{"$ref": "#..type.name"}`.   This syntax better matches that used by Javascript.\n2. The properties found in a `$ref` object are not ignored. Rather, they are to *override* the referenced object properties. This allows you to reference a default document, and replace the particular properties as needed. *more below*\n3. References can accept URL parameters: JSON is treated like a string template for more sophisticated value replacement. *see below*\n4. You can reference files and environment variables in addition to general URLs.\n\n## Quick guide\n\nLoad your configuration file:\n\n```python\nimport mo_json_config\n\nconfig = mo_json_config.get("file://my_config.json")\n```\n\nYou may use the global `configuration` object for case-insensitive lookup:\n\n\n```python\nfrom mo_json_config import configuration\n\n# use |= operator to add more configuration\nconfiguration |= {"some":{"deep":"value"}}\n\nassert configuration.someDeep == "value"\n\n```\n\n\n\n\n## Schemes\n\nThis module can load configuration from a number of sources, and you can access them via URI scheme.  Beyond the common `file` and `http` schemes, there are\n\n\n### Environment Variables\n\nUse the `env` scheme for accessing environment variables:\n\n    {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "env://MAIL_PASSWORD"}\n    }\n\n\n### Keystore Values\n\nThe [keyring](https://pypi.org/project/keyring/) library can be used with the `keyring` scheme:\n \n    {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "keyring://ekyle@mail.example.com"}\n    }\n\nThe host is in `<username>@<server_name>` format; invoking `keyring.get_password(server_name, username)`.  You may also set the username as a parameter:\n\n\n    {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "keyring://mail.example.com?username=ekyle"}\n    }\n\n> Be sure to `pip install keyring` to use keyring\n\n\n### AWS SSM\n\nThe `ssm` scheme can be used to read from the AWS parameter store.  Here is an example that will read all parameters that start with "/configuration" and adds them to the global configuration object:\n\n```python\nfrom mo_json_config import get, configuration\n\nconfiguration |= get("ssm:///configuration")\n```\n  \n\n## Using references in config files\n\nThe `$ref` property is special. Its value is interpreted as a URL pointing to more JSON\n\n\n### Absolute Internal Reference\n\nThe simplest form of URL is an absolute reference to a node in the same\ndocument:\n\n\n    {\n        "message": "Hello world",\n        "repeat": {"$ref": "#message"}\n    }\n\n\nThe reference must start with `#`, and the object with the `$ref` is replaced\nwith the value it points to:\n\n\n    {\n        "message": "Hello world",\n        "repeat": "Hello world"\n    }\n\n\n### Relative Internal References\n\nReferences that start with dot (`.`) are relative, with each additional dot\nreferring to successive parents.   In this case the `..` refers to the\nref-object\'s parent, and expands just like the previous example:\n\n\n    {\n        "message": "Hello world",\n        "repeat": {"$ref": "#..message"}\n    }\n\n\n### File References\n\nConfiguration is often stored on the local file system. You can in-line the\nJSON found in a file by using the `file://` scheme:\n\nIt is good practice to store sensitive data in a secure place...\n\n\n    {# LOCATED IN C:\\users\\kyle\\password.json\n        "host": "database.example.com",\n        "username": "kyle",\n        "password": "pass123"\n    }\n\n...and then refer to it in your configuration file:\n\n\n    {\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file:///C:/users/kyle/password.json"\n    }\n\n\nwhich will be expanded at run-time to:\n\n\n    {\n        "host": "example.com",\n        "port": "8080",\n        "username": "kyle",\n        "password": "pass123"\n    }\n\n\nPlease notice the triple slash (`///`) is referring to an absolute file\nreference.\n\n### References To Objects\n\nRef-objects that point to other objects (dicts) are not replaced completely,\nbut rather are merged with the target; with the ref-object\nproperties taking precedence.   This is seen in the example above: The "host"\nproperty is not overwritten by the target\'s.\n\n### Relative File Reference\n\nHere is the same, using a relative file reference; which is relative to the\nfile that contains this JSON\n\n\n    {#LOCATED IN C:\\users\\kyle\\dev-debug.json\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file://password.json"\n    }\n    \n\n### Home Directory Reference\n\nYou may also use the tilde (`~`) to refer to the current user\'s home directory.\nHere is the same again, but this example can be anywhere in the file system.\n\n\n    {\n        "host": "example.com",\n        "port": "8080",\n        "$ref": "file://~/password.json"\n    }\n\n\n### HTTP Reference\n\nConfiguration can be stored remotely, especially in the case of larger\nconfigurations which are too unwieldy to inline:\n\n\n    {\n        "schema":{"$ref": "https://example.com/sources/my_db.json"}\n    }\n\n\n### Scheme-Relative Reference\n\nYou are also able to leave the scheme off, so that whole constellations of\nconfiguration files can refer to each other no matter if they are on the local\nfile system, or remote:\n\n\n    {# LOCATED AT SOMEWHERE AT http://example.com\n        "schema":{"$ref": "///sources/my_db.json"}\n    }\n\n\nAnd, of course, relative references are also allowed:\n\n\n    {# LOCATED AT http://example.com/sources/dev-debug.json\n        "schema":{"$ref": "//sources/my_db.json"}\n    }\n\n\n### Fragment Reference\n\nSome remote configuration files are quite large...\n\n    {# LOCATED IN C:\\users\\kyle\\password.json\n        "database":{\n            "username": "kyle",\n            "password": "pass123"\n        },\n        "email":{\n            "username": "ekyle",\n            "password": "pass123"\n        }\n    }\n\n... and you only need one fragment. For this use the hash (`#`) followed by\nthe dot-delimited path into the document:\n\n    {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "//~/password.json#email.password"}\n    }\n\n### Parameters Reference\n\nYou can reference the variables found in `$ref` URL by using the `param` scheme. For example, the following JSON document demands that it be provided with a `password` parameter:  \n\n    { # LOCATED AT http://example.com/machine_config.json\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": {"$ref": "param:///password"}\n    }\n\n> The `param` scheme only accepts dot-delimited paths.\n\nThe above parametric JSON can be expanded with a $ref\n\n\t{"config": {\n\t\t"$ref": "http://example.com/machine_config.json?password=pass123"\n\t}}\n\nexpands to \n\n    {"config": {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": "pass123"\n    }}\n\nURL parameters and `$ref` properties can conflict. Let\'s consider \n\n\t{"config": {\n\t\t"$ref": "http://example.com/machine_config.json?password=pass123",\n\t\t"password": "123456"\n\t}}\n\nthe URL paramters are used to expand the given document, **then** the `$ref` properties override the contents of the document:\n\n    {"config": {\n        "host": "mail.example.com",\n        "username": "ekyle",\n        "password": "123456"\n    }}\n\n\n## Comments\n\nEnd-of-line Comments are allowed, using either `#` or `//` prefix:\n\n```\n    "key1": "value1",  //Comment 1\n```\n\n```\n    "key1": "value1",  # Comment 1\n```\n\nMultiline comments are also allowed, using either Python\'s triple-quotes\n(`""" ... """`) or Javascript\'s block quotes `/*...*/`\n\n```\n{\n    "key1": /* Comment 1 */ "value1",\n}\n```\n\n```\n    "key1": """Comment 1""" "value1",\n```\n\n\n## Parameterized JSON\n\nThe `param` scheme is a good way to set property values in a document, but sometimes that is not enough.  Sometimes you want to parameterize property names, or change the document structure in unconventional ways. For these cases, JSON documents are allowed named parameters at the unicode level. Parameters are surrounded by moustaches `{{.}}`:\n\n```javascript\n{//above_example.json\n    {var_name}: "value"\n}\n```\n\nParameter replacement is performed on the unicode text before being interpreted by the JSON parser. It is your responsibility to ensure the parameter replacement will result in valid JSON.\n\nYou pass the parameters by including them as URL parameters:\n\n\t{"$ref": "//~/above_example.json?var_name=%22hello%22"}\n\nWhich will expand to\n\n    {\n        "hello": "value"\n    }\n\nThe pipe (`|`) symbol can be used to perform some common conversions\n\n\n    {\n        {{var_name|quote}}: "value"\n    }\n\nThe `quote` transformation will deal with quoting, so ...\n\n\t{"$ref": "//~/above_example.json?var_name=hello"}\n\n... expands to the same:\n\n    {\n        "hello": "value"\n    }\n\nPlease see [`expand_template()` in the `strings` module](https://github.com/klahnakoski/mo-logs/blob/dev/mo_logs/strings.py) for more on the parameter replacement, and transformations available\n\n',
     long_description_content_type='text/markdown',
     name='mo-json-config',
     packages=["mo_json_config"],
     url='https://github.com/klahnakoski/mo-json-config',
-    version='4.606.24115'
+    version='4.609.24119'
 )
```

