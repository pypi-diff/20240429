# Comparing `tmp/inferless_cli-1.1.2.tar.gz` & `tmp/inferless_cli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferless_cli-1.1.2.tar", max compression
+gzip compressed data, was "inferless_cli-1.1.3.tar", max compression
```

## Comparing `inferless_cli-1.1.2.tar` & `inferless_cli-1.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    10052 2024-04-22 04:37:30.629340 inferless_cli-1.1.2/README.md
--rw-r--r--   0        0        0       37 2024-04-26 08:38:38.118679 inferless_cli-1.1.2/inferless_cli/__init__.py
--rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.2/inferless_cli/__main__.py
--rw-r--r--   0        0        0     7282 2024-04-22 04:37:30.630760 inferless_cli-1.1.2/inferless_cli/main.py
--rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.2/inferless_cli/prompts/__init__.py
--rw-r--r--   0        0        0    23068 2024-04-26 09:57:42.716132 inferless_cli-1.1.2/inferless_cli/prompts/deploy.py
--rw-r--r--   0        0        0     1802 2024-04-08 10:17:33.453829 inferless_cli-1.1.2/inferless_cli/prompts/export.py
--rw-r--r--   0        0        0    11391 2024-03-13 14:35:01.214724 inferless_cli-1.1.2/inferless_cli/prompts/init.py
--rw-r--r--   0        0        0     3779 2024-03-13 03:53:05.727048 inferless_cli-1.1.2/inferless_cli/prompts/log.py
--rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.2/inferless_cli/prompts/login.py
--rw-r--r--   0        0        0    15846 2024-03-26 03:45:26.809903 inferless_cli-1.1.2/inferless_cli/prompts/model.py
--rw-r--r--   0        0        0    18882 2024-04-26 08:39:22.573369 inferless_cli-1.1.2/inferless_cli/prompts/run.py
--rw-r--r--   0        0        0     5984 2024-03-13 03:53:05.727966 inferless_cli-1.1.2/inferless_cli/prompts/runtime.py
--rw-r--r--   0        0        0     2026 2024-03-13 03:53:05.728163 inferless_cli-1.1.2/inferless_cli/prompts/secret.py
--rw-r--r--   0        0        0     4231 2024-03-26 03:45:26.810630 inferless_cli-1.1.2/inferless_cli/prompts/token.py
--rw-r--r--   0        0        0    22032 2024-03-26 03:45:26.810909 inferless_cli-1.1.2/inferless_cli/prompts/volume.py
--rw-r--r--   0        0        0     1699 2024-03-13 03:53:05.729058 inferless_cli-1.1.2/inferless_cli/prompts/workspace.py
--rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.2/inferless_cli/utils/__init__.py
--rw-r--r--   0        0        0     2870 2024-03-13 03:53:05.729413 inferless_cli-1.1.2/inferless_cli/utils/api.py
--rw-r--r--   0        0        0    14752 2024-04-08 10:17:33.455242 inferless_cli-1.1.2/inferless_cli/utils/constants.py
--rw-r--r--   0        0        0     1068 2024-03-26 03:50:38.927856 inferless_cli-1.1.2/inferless_cli/utils/convertors.py
--rw-r--r--   0        0        0     7174 2024-03-26 03:45:26.811483 inferless_cli-1.1.2/inferless_cli/utils/credentials.py
--rw-r--r--   0        0        0    28795 2024-04-26 08:32:53.056800 inferless_cli-1.1.2/inferless_cli/utils/helpers.py
--rw-r--r--   0        0        0    26839 2024-04-26 09:17:36.749109 inferless_cli-1.1.2/inferless_cli/utils/services.py
--rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.2/inferless_cli/utils/validators.py
--rw-r--r--   0        0        0      671 2024-04-26 08:38:30.382551 inferless_cli-1.1.2/pyproject.toml
--rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10052 2024-04-29 12:49:54.154706 inferless_cli-1.1.3/README.md
+-rw-r--r--   0        0        0       37 2024-04-29 12:49:54.155009 inferless_cli-1.1.3/inferless_cli/__init__.py
+-rw-r--r--   0        0        0       50 2024-03-13 03:52:17.953547 inferless_cli-1.1.3/inferless_cli/__main__.py
+-rw-r--r--   0        0        0     7282 2024-04-29 12:49:54.155402 inferless_cli-1.1.3/inferless_cli/main.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:51:47.516671 inferless_cli-1.1.3/inferless_cli/prompts/__init__.py
+-rw-r--r--   0        0        0    23068 2024-04-29 12:49:54.155748 inferless_cli-1.1.3/inferless_cli/prompts/deploy.py
+-rw-r--r--   0        0        0     1802 2024-04-29 12:49:54.156043 inferless_cli-1.1.3/inferless_cli/prompts/export.py
+-rw-r--r--   0        0        0    11391 2024-04-29 12:49:54.156678 inferless_cli-1.1.3/inferless_cli/prompts/init.py
+-rw-r--r--   0        0        0     3779 2024-04-29 12:49:54.157030 inferless_cli-1.1.3/inferless_cli/prompts/log.py
+-rw-r--r--   0        0        0      854 2024-03-13 03:51:54.338936 inferless_cli-1.1.3/inferless_cli/prompts/login.py
+-rw-r--r--   0        0        0    15846 2024-04-29 12:49:54.157620 inferless_cli-1.1.3/inferless_cli/prompts/model.py
+-rw-r--r--   0        0        0    18882 2024-04-29 12:49:54.157892 inferless_cli-1.1.3/inferless_cli/prompts/run.py
+-rw-r--r--   0        0        0     5984 2024-04-29 12:49:54.158229 inferless_cli-1.1.3/inferless_cli/prompts/runtime.py
+-rw-r--r--   0        0        0     2026 2024-04-29 12:49:54.158392 inferless_cli-1.1.3/inferless_cli/prompts/secret.py
+-rw-r--r--   0        0        0     4231 2024-04-29 12:49:54.158770 inferless_cli-1.1.3/inferless_cli/prompts/token.py
+-rw-r--r--   0        0        0    22319 2024-04-29 12:49:54.159108 inferless_cli-1.1.3/inferless_cli/prompts/volume.py
+-rw-r--r--   0        0        0     1699 2024-04-29 12:49:54.159427 inferless_cli-1.1.3/inferless_cli/prompts/workspace.py
+-rw-r--r--   0        0        0        0 2024-03-13 03:52:07.884835 inferless_cli-1.1.3/inferless_cli/utils/__init__.py
+-rw-r--r--   0        0        0     2870 2024-04-29 12:49:54.159619 inferless_cli-1.1.3/inferless_cli/utils/api.py
+-rw-r--r--   0        0        0    14752 2024-04-29 12:49:54.160026 inferless_cli-1.1.3/inferless_cli/utils/constants.py
+-rw-r--r--   0        0        0     1068 2024-04-29 12:49:54.160238 inferless_cli-1.1.3/inferless_cli/utils/convertors.py
+-rw-r--r--   0        0        0     7179 2024-04-29 12:49:54.160563 inferless_cli-1.1.3/inferless_cli/utils/credentials.py
+-rw-r--r--   0        0        0    28795 2024-04-29 12:49:54.160943 inferless_cli-1.1.3/inferless_cli/utils/helpers.py
+-rw-r--r--   0        0        0    26839 2024-04-29 12:49:54.161332 inferless_cli-1.1.3/inferless_cli/utils/services.py
+-rw-r--r--   0        0        0     7065 2024-03-13 03:52:15.076191 inferless_cli-1.1.3/inferless_cli/utils/validators.py
+-rw-r--r--   0        0        0      671 2024-04-29 12:49:54.162514 inferless_cli-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 inferless_cli-1.1.3/PKG-INFO
```

### Comparing `inferless_cli-1.1.2/README.md` & `inferless_cli-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/main.py` & `inferless_cli-1.1.3/inferless_cli/main.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/deploy.py` & `inferless_cli-1.1.3/inferless_cli/prompts/deploy.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/export.py` & `inferless_cli-1.1.3/inferless_cli/prompts/export.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/init.py` & `inferless_cli-1.1.3/inferless_cli/prompts/init.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/log.py` & `inferless_cli-1.1.3/inferless_cli/prompts/log.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/login.py` & `inferless_cli-1.1.3/inferless_cli/prompts/login.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/model.py` & `inferless_cli-1.1.3/inferless_cli/prompts/model.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/run.py` & `inferless_cli-1.1.3/inferless_cli/prompts/run.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/runtime.py` & `inferless_cli-1.1.3/inferless_cli/prompts/runtime.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/secret.py` & `inferless_cli-1.1.3/inferless_cli/prompts/secret.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/token.py` & `inferless_cli-1.1.3/inferless_cli/prompts/token.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/volume.py` & `inferless_cli-1.1.3/inferless_cli/prompts/volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,23 +375,21 @@
                 s3_path = destination.split("infer://")[1]
                 vol_id = volume_data["id"]
                 mapped_region = REGION_MAP_VOLUME[vol_region]
                 s3_path = s3_path.replace(
                     f"volumes/{mapped_region}/",
                     f"volumes_temp/{vol_region}/{workspace_id}/{vol_id}/",
                 )
-
                 try:
-                    base_temp_s3_path = os.path.join(
-                        "volumes_temp",
-                        volume_data["region"] if volume_data["region"] else "AZURE",
-                        workspace_id,
-                        volume_data["id"],
-                        volume_data["name"],
+                    base_path_region = (
+                        volume_data["region"] if volume_data["region"] else "AZURE"
                     )
+                    base_path_volume_id = volume_data["id"]
+                    base_path_volume_name = volume_data["name"]
+                    base_temp_s3_path = f"volumes_temp/{base_path_region}/{workspace_id}/{base_path_volume_id}/{base_path_volume_name}"
                     payload = {"s3_path": base_temp_s3_path, "volume_id": vol_id}
                     delete_volume_temp_dir(payload)
                 except Exception:
                     pass
 
                 volume_data["volume_id"] = volume_data["id"]
                 futures = []
@@ -421,21 +419,20 @@
                     )
                     payload = {"source": s3_path, "destination": s3_path_original}
                     try:
                         res = sync_s3_to_s3(payload)
                     except Exception as e:
                         rich.print(e)
                         raise typer.Exit(1)
-                    base_s3_path = os.path.join(
-                        "volumes",
-                        volume_data["region"] if volume_data["region"] else "AZURE",
-                        workspace_id,
-                        volume_data["id"],
-                        volume_data["name"],
+                    base_s3_path_region = (
+                        volume_data["region"] if volume_data["region"] else "AZURE"
                     )
+                    base_s3_path_volume_id = volume_data["id"]
+                    base_s3_path_volume_name = volume_data["name"]
+                    base_s3_path = f"volumes/{base_s3_path_region}/{workspace_id}/{base_s3_path_volume_id}/{base_s3_path_volume_name}"
                     try:
                         sync_s3_to_nfs({"s3_path": base_s3_path, "volume_id": vol_id})
                     except Exception as e:
                         rich.print(e)
                         raise typer.Exit(1)
                     rich.print("\n[green]Upload successful[/green]\n\n")
                 else:
@@ -556,16 +553,21 @@
 
 def process_file(path: str, s3_path, root_path):
     try:
         if root_path == path:
             temp = os.path.basename(path)
             save_path = s3_path
         else:
-            temp = path.split(root_path)[-1].lstrip("/")
-            save_path = os.path.join(s3_path, temp)
+            if os.name == "nt":
+                temp = path.split(root_path)[-1].lstrip("\\")
+            else:
+                temp = path.split(root_path)[-1].lstrip("/")
+
+            save_path = f"{s3_path}/{temp}"
+
         if save_path.startswith("/"):
             save_path = save_path[1:]
         file_size = os.path.getsize(path)
 
         if file_size > 5 * 1024**3:  # File size is more than 5GB
             with open(path, "rb") as file:
                 rich.print(f"Uploading {path}")
```

### Comparing `inferless_cli-1.1.2/inferless_cli/prompts/workspace.py` & `inferless_cli-1.1.3/inferless_cli/prompts/workspace.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/utils/api.py` & `inferless_cli-1.1.3/inferless_cli/utils/api.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/utils/constants.py` & `inferless_cli-1.1.3/inferless_cli/utils/constants.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/utils/convertors.py` & `inferless_cli-1.1.3/inferless_cli/utils/convertors.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/utils/credentials.py` & `inferless_cli-1.1.3/inferless_cli/utils/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 KEYRING = keyring
 
 
 def is_keyring_supported():
     if keyring is None:
         return False
     elif keyring_backend is not None and isinstance(keyring_backend, null.Keyring):
-        print("Using null backend. Keyring functionality is disabled.")
+        rich.print("Using null backend. Keyring functionality is disabled.")
         return False
     else:
         return True
 
 
 # Define a function to load the encryption key from an environment variable
 def load_key():
```

### Comparing `inferless_cli-1.1.2/inferless_cli/utils/helpers.py` & `inferless_cli-1.1.3/inferless_cli/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/utils/services.py` & `inferless_cli-1.1.3/inferless_cli/utils/services.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/inferless_cli/utils/validators.py` & `inferless_cli-1.1.3/inferless_cli/utils/validators.py`

 * *Files identical despite different names*

### Comparing `inferless_cli-1.1.2/pyproject.toml` & `inferless_cli-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inferless-cli"
-version = "1.1.2"
+version = "1.1.3"
 description = "Inferless - Deploy Machine Learning Models in Minutes."
 authors = ["Naveen <naveen@inferless.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 inferless = "inferless_cli.main:app"
```

### Comparing `inferless_cli-1.1.2/PKG-INFO` & `inferless_cli-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferless-cli
-Version: 1.1.2
+Version: 1.1.3
 Summary: Inferless - Deploy Machine Learning Models in Minutes.
 Author: Naveen
 Author-email: naveen@inferless.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

