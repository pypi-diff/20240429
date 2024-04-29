# Comparing `tmp/codedepot_depot-0.0.7.tar.gz` & `tmp/codedepot_depot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_depot-0.0.7.tar", last modified: Fri Apr 19 12:46:16 2024, max compression
+gzip compressed data, was "codedepot_depot-0.0.8.tar", last modified: Mon Apr 29 09:53:27 2024, max compression
```

## Comparing `codedepot_depot-0.0.7.tar` & `codedepot_depot-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.7/depot/__init__.py
--rw-r--r--   0        0        0     7611 2024-04-19 12:34:20.957819 codedepot_depot-0.0.7/depot/api.py
--rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.7/depot/cluster_spec.py
--rw-r--r--   0        0        0     3713 2024-04-19 09:37:38.563990 codedepot_depot-0.0.7/depot/config.py
--rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.7/depot/jobfile.py
--rw-r--r--   0        0        0     4283 2024-04-19 12:45:28.404084 codedepot_depot-0.0.7/depot/main.py
--rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.7/depot/provider_spec.py
--rw-r--r--   0        0        0      817 2024-04-19 12:46:16.964352 codedepot_depot-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.7/test/__init__.py
--rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.7/test/resources/cluster_test.yaml
--rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.7/test/resources/config.json
--rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.7/test/resources/local_cred.json
--rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.7/test/resources/provider_test.yaml
--rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.7/test/test_client.py
--rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.7/test/test_provider.py
--rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.7/test/utils.py
--rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 codedepot_depot-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-04-15 07:13:36.336177 codedepot_depot-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 13:02:27.184638 codedepot_depot-0.0.8/depot/__init__.py
+-rw-r--r--   0        0        0     7623 2024-04-29 09:50:26.764206 codedepot_depot-0.0.8/depot/api.py
+-rw-r--r--   0        0        0      624 2024-04-18 08:11:02.116570 codedepot_depot-0.0.8/depot/cluster_spec.py
+-rw-r--r--   0        0        0     3998 2024-04-21 22:00:24.992845 codedepot_depot-0.0.8/depot/config.py
+-rw-r--r--   0        0        0      507 2024-04-18 06:56:25.799963 codedepot_depot-0.0.8/depot/jobfile.py
+-rw-r--r--   0        0        0     4283 2024-04-29 09:51:52.234881 codedepot_depot-0.0.8/depot/main.py
+-rw-r--r--   0        0        0      616 2024-04-16 05:00:55.267184 codedepot_depot-0.0.8/depot/provider_spec.py
+-rw-r--r--   0        0        0      817 2024-04-29 09:53:27.801464 codedepot_depot-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 20:33:04.196404 codedepot_depot-0.0.8/test/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-16 05:02:59.830823 codedepot_depot-0.0.8/test/resources/cluster_test.yaml
+-rw-r--r--   0        0        0       87 2024-04-15 20:48:31.758568 codedepot_depot-0.0.8/test/resources/config.json
+-rw-r--r--   0        0        0       80 2024-04-15 20:35:06.454038 codedepot_depot-0.0.8/test/resources/local_cred.json
+-rw-r--r--   0        0        0       96 2024-04-16 04:58:41.947831 codedepot_depot-0.0.8/test/resources/provider_test.yaml
+-rw-r--r--   0        0        0        0 2024-04-16 04:06:38.432329 codedepot_depot-0.0.8/test/test_client.py
+-rw-r--r--   0        0        0      408 2024-04-16 05:35:56.755146 codedepot_depot-0.0.8/test/test_provider.py
+-rw-r--r--   0        0        0      666 2024-04-16 05:28:37.442814 codedepot_depot-0.0.8/test/utils.py
+-rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 codedepot_depot-0.0.8/PKG-INFO
```

### Comparing `codedepot_depot-0.0.7/depot/api.py` & `codedepot_depot-0.0.8/depot/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,16 @@
         if not repo_folder:
             print("Cannot find a git repository in the current folder. Please run this command from a git repository.")
             return
 
         repo = AIRepo(repo_folder)
         job_spec = JobSpec.from_file(
             os.path.join(repo.workdir, '.jobfile.yaml'))
-        job_instance_name = get_new_exp_name(repo)
+        
+        job_instance_name = repo.head.target.hex[0:8]
         clusters = config.api().list_clusters_clusters_get()
         cluster = [c for c in clusters if c['name'] == cluster_name]
         if not cluster:
             print(f"Cluster {cluster_name} does not exist.")
             return
         cluster = cluster[0]
         repo_url = __http_to_ssh(repo.remotes['origin'].url)
```

### Comparing `codedepot_depot-0.0.7/depot/cluster_spec.py` & `codedepot_depot-0.0.8/depot/cluster_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.7/depot/config.py` & `codedepot_depot-0.0.8/depot/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from email.policy import default
 import json
 import os
 from prompt_toolkit import prompt
 
 from depot_api.api.default_api import DefaultApi
 from depot_api.api_client import ApiClient, Configuration
 
@@ -70,17 +71,19 @@
                 'You are already logged in. Do you want to log in again? [y/N]: ')
             if r.lower() != 'y':
                 return
             with open(DepotConfig.default_config_path(), 'r') as file:
                 y = json.load(file)
             default_endpoint = y['endpoint']
             default_login = y['login']
+            default_email = y['email']
         else:
             default_endpoint = 'https://depot.staging.codedepot.ai'
             default_login = None
+            default_email = None
         endpoint = prompt(
             f'Enter your API endpoint [{default_endpoint}]: ')
         if not endpoint:
             endpoint = default_endpoint
 
         if not default_login:
             username = prompt('Enter your login: ')
@@ -90,15 +93,20 @@
                 username = default_login
 
         # Check if the username is empty TODO: check if the username is valid
         if not username:
             print('Username is required')
             return None
 
-        email = prompt('Enter your email: ')
+        if not default_email:
+            email = prompt('Enter your email: ')
+        else:
+            email = prompt(f'Enter your email [{default_email}]: ')
+            if not email:
+                email = default_email
         # Check if the username is empty TODO: check if the username is valid
         if not email:
             print('Email is required')
             return None
 
         password = prompt(
             f'Enter the password for {username}: ', is_password=True)
```

### Comparing `codedepot_depot-0.0.7/depot/main.py` & `codedepot_depot-0.0.8/depot/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     # Parse the arguments
     return parser.parse_args()
 
 
 def main():
     args = parse_args()
     if args.version:
-        print("0.0.7")
+        print("0.0.8")
         return
 
     if args.command == 'login':
         DepotConfig.create()
         return
 
     config = DepotConfig.default()
```

### Comparing `codedepot_depot-0.0.7/depot/provider_spec.py` & `codedepot_depot-0.0.8/depot/provider_spec.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.7/pyproject.toml` & `codedepot_depot-0.0.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "codedepot-depot"
-version = "0.0.7"
+version = "0.0.8"
 description = "Job launch support for Git AI"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `codedepot_depot-0.0.7/test/utils.py` & `codedepot_depot-0.0.8/test/utils.py`

 * *Files identical despite different names*

### Comparing `codedepot_depot-0.0.7/PKG-INFO` & `codedepot_depot-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedepot-depot
-Version: 0.0.7
+Version: 0.0.8
 Summary: Job launch support for Git AI
 Author-Email: CodeDepot <contact@codedepot.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Requires-Python: >=3.10
```

