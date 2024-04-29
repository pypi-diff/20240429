# Comparing `tmp/jsonUts-1.0.1.tar.gz` & `tmp/jsonUts-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonUts-1.0.1.tar", last modified: Fri Apr 19 21:47:04 2024, max compression
+gzip compressed data, was "jsonUts-1.0.2.tar", last modified: Mon Apr 29 13:50:15 2024, max compression
```

## Comparing `jsonUts-1.0.1.tar` & `jsonUts-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-19 21:47:04.930778 jsonUts-1.0.1/
--rw-rw-rw-   0        0        0       83 2024-04-19 21:46:49.000000 jsonUts-1.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 jsonUts-1.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 jsonUts-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1648 2024-04-19 21:47:04.926785 jsonUts-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2024-04-19 21:45:12.000000 jsonUts-1.0.1/README.md
--rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 jsonUts-1.0.1/commands.txt
-drwxrwxrwx   0        0        0        0 2024-04-19 21:47:04.884779 jsonUts-1.0.1/jsonUts/
--rw-rw-rw-   0        0        0     2386 2024-04-19 21:47:01.000000 jsonUts-1.0.1/jsonUts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-19 21:47:04.917778 jsonUts-1.0.1/jsonUts.egg-info/
--rw-rw-rw-   0        0        0     1648 2024-04-19 21:47:04.000000 jsonUts-1.0.1/jsonUts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-04-19 21:47:04.000000 jsonUts-1.0.1/jsonUts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-19 21:47:04.000000 jsonUts-1.0.1/jsonUts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-19 21:47:04.000000 jsonUts-1.0.1/jsonUts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-19 21:47:04.931778 jsonUts-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      765 2024-04-19 21:31:46.000000 jsonUts-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:50:15.532738 jsonUts-1.0.2/
+-rw-rw-rw-   0        0        0       83 2024-04-19 21:46:49.000000 jsonUts-1.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-04-26 21:06:44.000000 jsonUts-1.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-26 21:06:44.000000 jsonUts-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1648 2024-04-29 13:50:15.530739 jsonUts-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2024-04-19 21:45:12.000000 jsonUts-1.0.2/README.md
+-rw-rw-rw-   0        0        0      212 2024-04-16 22:37:47.000000 jsonUts-1.0.2/commands.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 13:50:15.501739 jsonUts-1.0.2/jsonUts/
+-rw-rw-rw-   0        0        0     2649 2024-04-29 13:49:37.000000 jsonUts-1.0.2/jsonUts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 13:50:15.528735 jsonUts-1.0.2/jsonUts.egg-info/
+-rw-rw-rw-   0        0        0     1648 2024-04-29 13:50:15.000000 jsonUts-1.0.2/jsonUts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-04-29 13:50:15.000000 jsonUts-1.0.2/jsonUts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 13:50:15.000000 jsonUts-1.0.2/jsonUts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-29 13:50:15.000000 jsonUts-1.0.2/jsonUts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 13:50:15.532738 jsonUts-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      765 2024-04-19 21:31:46.000000 jsonUts-1.0.2/setup.py
```

### Comparing `jsonUts-1.0.1/LICENCE.txt` & `jsonUts-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `jsonUts-1.0.1/PKG-INFO` & `jsonUts-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonUts
-Version: 1.0.1
+Version: 1.0.2
 Summary: Json package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: jsonUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jsonUts-1.0.1/README.md` & `jsonUts-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jsonUts-1.0.1/jsonUts/__init__.py` & `jsonUts-1.0.2/jsonUts/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version = '1.0.1'
+version = '1.0.2'
 
 
 
 class JsonData:
     original_keys = []
     keys = []
 
@@ -39,34 +39,49 @@
 def adjustKey(key,trim_keys=True,lower=False,char_space='_'):
     val = key if not trim_keys else key.strip().replace(' ', char_space)
     val = val if not lower else val.lower()
     return val
 
 
 def jsonToObj(json_data,trim_keys=True,lower_keys=False,char_space='_'):
-    obj = JsonData()
-    keys = []
-    new_keys = []
-    for key in json_data.keys():
-        new_key = adjustKey(key,trim_keys,lower_keys,char_space)
-        keys.append(key)
-        new_keys.append(new_key)
-        if  isinstance(json_data[key], dict) :
-            value = jsonToObj(json_data[key])
-            setattr(obj,new_key,value )
-        elif isinstance(json_data[key], list):
-            lista=[]
-            for item in json_data[key]:
-                lista.append(jsonToObj(item))
-            setattr(obj,new_key,lista)
-        else:
-            setattr(obj,new_key,json_data[key] )
-    obj.original_keys = keys
-    obj.keys = new_keys
-    return obj
+    
+    if isinstance(json_data, dict) :
+        keys,new_keys = [],[]
+        obj = JsonData()
+
+        for key in json_data.keys():
+            new_key = adjustKey(key,trim_keys,lower_keys,char_space)
+            keys.append(key)
+            new_keys.append(new_key)
+
+            setattr(obj,new_key,jsonToObj(json_data[key],trim_keys,lower_keys,char_space))
+
+        obj.original_keys = keys
+        obj.keys = new_keys
+        return obj
+
+    elif isinstance(json_data, list):
+        lista=[]
+        for item in json_data:
+            lista.append(jsonToObj(item,trim_keys,lower_keys,char_space))
+        return lista
+    else:
+        return json_data
+
+
+
+
+# data = [
+#     {
+#         "ID": "420c68d4-f939-4bb9-a11b-01df26bef000", 
+#         "CPF": "49951376886", 
+#         "DATANASCIMENTO": "2002-06-28T06:00:00", 
+#         "NOME": "Richard Lima Barboza", 
+#         "BOT": ["consultaRestricao"]
+#     }]
 
 
 
 # data =  {
 #     "pessoa":{
 #         "nome":"melque",
 #         "idade": 30
@@ -76,12 +91,12 @@
 #         {"marca":"Lamborghini","ano":2018}
 #     ],
 #     "profissao":"Desenvolvedor de Software",
 #     "Teste":123,
 #     "with space":"hehe"
 # }
 
-# dataO = jsonToObj(data)
+#dataO = jsonToObj(data)
 
-# pass
+#pass
```

### Comparing `jsonUts-1.0.1/jsonUts.egg-info/PKG-INFO` & `jsonUts-1.0.2/jsonUts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonUts
-Version: 1.0.1
+Version: 1.0.2
 Summary: Json package
 Home-page: 
 Author: Melque Lima
 Author-email: melque_ex@yahoo.com.br
 License: MIT
 Keywords: jsonUts
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jsonUts-1.0.1/setup.py` & `jsonUts-1.0.2/setup.py`

 * *Files identical despite different names*

