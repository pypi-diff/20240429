# Comparing `tmp/antigranular_enterprise-1.0.1.tar.gz` & `tmp/antigranular_enterprise-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antigranular_enterprise-1.0.1.tar", max compression
+gzip compressed data, was "antigranular_enterprise-1.0.2.tar", max compression
```

## Comparing `antigranular_enterprise-1.0.1.tar` & `antigranular_enterprise-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      549 2024-04-24 12:04:17.396946 antigranular_enterprise-1.0.1/antigranular_enterprise/__init__.py
--rw-r--r--   0        0        0     4051 2024-04-24 07:56:20.265338 antigranular_enterprise-1.0.1/antigranular_enterprise/agent_client/agent_client.py
--rw-r--r--   0        0        0    23153 2024-04-25 05:59:35.607432 antigranular_enterprise-1.0.1/antigranular_enterprise/client.py
--rw-r--r--   0        0        0     5543 2024-04-02 13:06:51.888538 antigranular_enterprise-1.0.1/antigranular_enterprise/config/config.py
--rw-r--r--   0        0        0      975 2024-04-02 13:06:51.897906 antigranular_enterprise-1.0.1/antigranular_enterprise/magics/errors.py
--rw-r--r--   0        0        0     6829 2024-04-24 09:22:48.293354 antigranular_enterprise-1.0.1/antigranular_enterprise/magics/magics.py
--rw-r--r--   0        0        0        0 2024-04-02 13:06:51.902441 antigranular_enterprise-1.0.1/antigranular_enterprise/models/__init__.py
--rw-r--r--   0        0        0      657 2024-04-02 13:06:51.905464 antigranular_enterprise-1.0.1/antigranular_enterprise/models/models.py
--rw-r--r--   0        0        0      222 2024-04-02 13:06:51.909982 antigranular_enterprise-1.0.1/antigranular_enterprise/utils/error_print.py
--rw-r--r--   0        0        0      196 2024-04-02 13:06:51.918013 antigranular_enterprise-1.0.1/antigranular_enterprise/utils/print_request_id.py
--rw-r--r--   0        0        0    11558 2023-10-13 07:17:56.825501 antigranular_enterprise-1.0.1/LICENSE
--rw-r--r--   0        0        0     1401 2024-04-24 12:03:51.418557 antigranular_enterprise-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5381 2024-04-25 11:55:52.227581 antigranular_enterprise-1.0.1/README.md
--rw-r--r--   0        0        0     6759 1970-01-01 00:00:00.000000 antigranular_enterprise-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      549 2024-04-29 10:18:15.505562 antigranular_enterprise-1.0.2/antigranular_enterprise/__init__.py
+-rw-r--r--   0        0        0     4051 2024-04-24 07:56:20.265338 antigranular_enterprise-1.0.2/antigranular_enterprise/agent_client/agent_client.py
+-rw-r--r--   0        0        0    23271 2024-04-26 13:21:42.899612 antigranular_enterprise-1.0.2/antigranular_enterprise/client.py
+-rw-r--r--   0        0        0     5543 2024-04-02 13:06:51.888538 antigranular_enterprise-1.0.2/antigranular_enterprise/config/config.py
+-rw-r--r--   0        0        0      975 2024-04-02 13:06:51.897906 antigranular_enterprise-1.0.2/antigranular_enterprise/magics/errors.py
+-rw-r--r--   0        0        0     6829 2024-04-24 09:22:48.293354 antigranular_enterprise-1.0.2/antigranular_enterprise/magics/magics.py
+-rw-r--r--   0        0        0        0 2024-04-02 13:06:51.902441 antigranular_enterprise-1.0.2/antigranular_enterprise/models/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-02 13:06:51.905464 antigranular_enterprise-1.0.2/antigranular_enterprise/models/models.py
+-rw-r--r--   0        0        0      222 2024-04-02 13:06:51.909982 antigranular_enterprise-1.0.2/antigranular_enterprise/utils/error_print.py
+-rw-r--r--   0        0        0      196 2024-04-02 13:06:51.918013 antigranular_enterprise-1.0.2/antigranular_enterprise/utils/print_request_id.py
+-rw-r--r--   0        0        0    11558 2023-10-13 07:17:56.825501 antigranular_enterprise-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1401 2024-04-29 10:18:09.659269 antigranular_enterprise-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5381 2024-04-25 11:55:52.227581 antigranular_enterprise-1.0.2/README.md
+-rw-r--r--   0        0        0     6759 1970-01-01 00:00:00.000000 antigranular_enterprise-1.0.2/PKG-INFO
```

### Comparing `antigranular_enterprise-1.0.1/antigranular_enterprise/__init__.py` & `antigranular_enterprise-1.0.2/antigranular_enterprise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 from .client import login
 from .client import read_config
 from .client import write_config
 from .client import load_config
 # Package version dunder
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 # Package author dunder
 __author__ = "Oblivious Software Pvt. Ltd."
 
 # Package * imports dunder
 __all__ = ["login", "read_config", "write_config", "load_config", "__version__", "__author__"]
```

### Comparing `antigranular_enterprise-1.0.1/antigranular_enterprise/agent_client/agent_client.py` & `antigranular_enterprise-1.0.2/antigranular_enterprise/agent_client/agent_client.py`

 * *Files identical despite different names*

### Comparing `antigranular_enterprise-1.0.1/antigranular_enterprise/client.py` & `antigranular_enterprise-1.0.2/antigranular_enterprise/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,15 +196,19 @@
                         raise requests.exceptions.HTTPError(
                             f"Error while starting a new session in server status code: {res.status_code} message: {res.text}"
                         )
                     self.session_id = json.loads(res.text)["session_id"]
                 except Exception as err:
                     raise ConnectionError(f"Error calling /start-session: {str(err)}")
             else:
-                eprint("Error during API key authentication. Please ensure login approval on AGENT Console.")
+                message = "Error during API key authentication. Please ensure login approval on AGENT Console."
+                if get_ipython():
+                    eprint(message)
+                else:
+                    raise SystemExit(eprint(message))
 
         except Exception as err:
             raise ConnectionError(f"Error while creating client: {str(err)}")
     
     def __process_message(self, data: Dict[str, Any]) -> None:
         approval_status = data.get('approval_status')
         if approval_status == 'approved':
@@ -274,18 +278,18 @@
                                 print(message["content"]["text"])
                     elif message["msg_type"] == "error":
                         tb_str = ""
                         for tb in message["content"]["traceback"]:
                             tb_str += tb
 
                         if return_output:
-                            return_value += tb_str
+                            raise SystemExit(tb_str)
                         else:
                             print(tb_str)
-                        return None if return_value == '' else return_value
+                            return None
                     elif message["msg_type"] == "ag_export_value":
                         try:
                             data = message["content"]
                             for name, value in data.items():
                                 globals_dict[name] = pickle.loads(base64.b64decode(value))
                                 print(
                                     "Setting up exported variable in local environment:",
```

### Comparing `antigranular_enterprise-1.0.1/antigranular_enterprise/config/config.py` & `antigranular_enterprise-1.0.2/antigranular_enterprise/config/config.py`

 * *Files identical despite different names*

### Comparing `antigranular_enterprise-1.0.1/antigranular_enterprise/magics/errors.py` & `antigranular_enterprise-1.0.2/antigranular_enterprise/magics/errors.py`

 * *Files identical despite different names*

### Comparing `antigranular_enterprise-1.0.1/antigranular_enterprise/magics/magics.py` & `antigranular_enterprise-1.0.2/antigranular_enterprise/magics/magics.py`

 * *Files identical despite different names*

### Comparing `antigranular_enterprise-1.0.1/antigranular_enterprise/models/models.py` & `antigranular_enterprise-1.0.2/antigranular_enterprise/models/models.py`

 * *Files identical despite different names*

### Comparing `antigranular_enterprise-1.0.1/LICENSE` & `antigranular_enterprise-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antigranular_enterprise-1.0.1/pyproject.toml` & `antigranular_enterprise-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "antigranular_enterprise"
-version = "1.0.1"
+version = "1.0.2"
 description = "Antigranular Enterprise is a robust, scalable version of the Antigranular platform. It combines the power of differential privacy, providing a secure environment for handling and unlocking the full potential of unseen data. With enhanced features and dedicated support, Antigranular Enterprise is the ideal solution for businesses seeking to leverage the power of data privacy and security."
 authors = ["Oblivious Software Pvt. Ltd. <support@oblivious.com>"]
 readme = "README.md"
 packages = [{include = "antigranular_enterprise"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `antigranular_enterprise-1.0.1/README.md` & `antigranular_enterprise-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `antigranular_enterprise-1.0.1/PKG-INFO` & `antigranular_enterprise-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antigranular_enterprise
-Version: 1.0.1
+Version: 1.0.2
 Summary: Antigranular Enterprise is a robust, scalable version of the Antigranular platform. It combines the power of differential privacy, providing a secure environment for handling and unlocking the full potential of unseen data. With enhanced features and dedicated support, Antigranular Enterprise is the ideal solution for businesses seeking to leverage the power of data privacy and security.
 Author: Oblivious Software Pvt. Ltd.
 Author-email: support@oblivious.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

