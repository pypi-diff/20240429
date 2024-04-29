# Comparing `tmp/munud-0.2.2.tar.gz` & `tmp/munud-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "munud-0.2.2.tar", max compression
+gzip compressed data, was "munud-0.2.3.tar", max compression
```

## Comparing `munud-0.2.2.tar` & `munud-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2024-04-26 14:48:53.558390 munud-0.2.2/LICENSE
--rw-r--r--   0        0        0     7081 2024-04-26 14:48:53.559390 munud-0.2.2/README.md
--rw-r--r--   0        0        0     1219 2024-04-26 14:48:53.560390 munud-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       48 2024-04-26 14:48:53.560390 munud-0.2.2/src/munud/__init__.py
--rw-r--r--   0        0        0     7483 2024-04-26 14:48:53.560390 munud-0.2.2/src/munud/cgen.py
--rw-r--r--   0        0        0     4547 2024-04-26 14:48:53.560390 munud-0.2.2/src/munud/cgen_types.py
--rw-r--r--   0        0        0     7861 2024-04-26 14:48:53.560390 munud-0.2.2/src/munud/main.py
--rw-r--r--   0        0        0     5334 2024-04-26 14:48:53.560390 munud-0.2.2/src/munud/munud.py
--rw-r--r--   0        0        0    12280 2024-04-26 14:48:53.560390 munud-0.2.2/src/munud/munud_types.py
--rw-r--r--   0        0        0      711 2024-04-26 14:48:53.560390 munud-0.2.2/src/munud/utils.py
--rw-r--r--   0        0        0     7950 1970-01-01 00:00:00.000000 munud-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-29 15:53:28.086902 munud-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7081 2024-04-29 15:53:28.086902 munud-0.2.3/README.md
+-rw-r--r--   0        0        0     1219 2024-04-29 15:53:28.087902 munud-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-04-29 15:53:28.087902 munud-0.2.3/src/munud/__init__.py
+-rw-r--r--   0        0        0     7793 2024-04-29 15:53:28.087902 munud-0.2.3/src/munud/cgen.py
+-rw-r--r--   0        0        0     4547 2024-04-29 15:53:28.087902 munud-0.2.3/src/munud/cgen_types.py
+-rw-r--r--   0        0        0     7861 2024-04-29 15:53:28.087902 munud-0.2.3/src/munud/main.py
+-rw-r--r--   0        0        0     5334 2024-04-29 15:53:28.087902 munud-0.2.3/src/munud/munud.py
+-rw-r--r--   0        0        0    12280 2024-04-29 15:53:28.087902 munud-0.2.3/src/munud/munud_types.py
+-rw-r--r--   0        0        0      711 2024-04-29 15:53:28.087902 munud-0.2.3/src/munud/utils.py
+-rw-r--r--   0        0        0     7950 1970-01-01 00:00:00.000000 munud-0.2.3/PKG-INFO
```

### Comparing `munud-0.2.2/LICENSE` & `munud-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `munud-0.2.2/README.md` & `munud-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `munud-0.2.2/pyproject.toml` & `munud-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "munud"
-version = "0.2.2"
+version = "0.2.3"
 description = "Building sub-byte payloads, and generating according C code"
 authors = ["Ulysse Moreau <u.moreau@hexa-h.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
```

### Comparing `munud-0.2.2/src/munud/cgen.py` & `munud-0.2.3/src/munud/cgen.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,18 +156,28 @@
         safety_mask (bool, optional): Add a safety mask (0xff) when writing to the patload. Defaults to True.
         payload_type (str, optional): The type of the payload. Defaults to "uint8_t*".
         struct_name (str, optional): The name of the struct. Defaults to "Payload".
 
     Returns:
         str: The according c code.
     """
+
     generated_c_code = ""
+
+    header_guard = "DEFAULT_MUNUD_HEADER_GUARD_H"
+
+    if namespace:
+        header_guard = f"{namespace.upper()}_H"
+
     generated_c_code += get_header_with_date()
     generated_c_code += get_includes(no_assert=use_assert)
 
+    generated_c_code += f"\n#ifndef {header_guard}"
+    generated_c_code += f"\n#define {header_guard}\n"
+
     funcs_prefix = ""
 
     if namespace:
         if cpp:
             generated_c_code += f"\nnamespace {namespace} {{"
         else:
             funcs_prefix = namespace
@@ -277,9 +287,12 @@
         generated_c_code += str(encode_all)
 
     if namespace and cpp:
         generated_c_code += "\n"
         generated_c_code += f"\n}} // namespace {namespace}"
 
     generated_c_code += "\n"
+    generated_c_code += "\n"
+
+    generated_c_code += f"#endif //{header_guard}\n"
 
     return generated_c_code
```

### Comparing `munud-0.2.2/src/munud/cgen_types.py` & `munud-0.2.3/src/munud/cgen_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 def get_header_with_date():
     return HEADER.format(datetime.datetime.now().strftime("%m/%d/%Y at %H:%M:%S"))
 
 
 def get_includes(no_assert=False):
     if no_assert:
         return """
-#include "stdint.h"
+#include <stdint.h>
         """
     else:
 
         return """
-#include "assert.h"
-#include "stdint.h"
+#include <assert.h>
+#include <stdint.h>
         """
 
 
 PAYLOAD_TYPE = "uint8_t*"
 
 
 class CFuncArg:
```

### Comparing `munud-0.2.2/src/munud/main.py` & `munud-0.2.3/src/munud/main.py`

 * *Files identical despite different names*

### Comparing `munud-0.2.2/src/munud/munud.py` & `munud-0.2.3/src/munud/munud.py`

 * *Files identical despite different names*

### Comparing `munud-0.2.2/src/munud/munud_types.py` & `munud-0.2.3/src/munud/munud_types.py`

 * *Files identical despite different names*

### Comparing `munud-0.2.2/src/munud/utils.py` & `munud-0.2.3/src/munud/utils.py`

 * *Files identical despite different names*

### Comparing `munud-0.2.2/PKG-INFO` & `munud-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: munud
-Version: 0.2.2
+Version: 0.2.3
 Summary: Building sub-byte payloads, and generating according C code
 License: MIT
 Author: Ulysse Moreau
 Author-email: u.moreau@hexa-h.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

