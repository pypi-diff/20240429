# Comparing `tmp/lfg_llama-1.0.1.tar.gz` & `tmp/lfg_llama-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.0.1.tar", last modified: Mon Apr 29 05:42:57 2024, max compression
+gzip compressed data, was "lfg_llama-1.0.2.tar", last modified: Mon Apr 29 06:43:34 2024, max compression
```

## Comparing `lfg_llama-1.0.1.tar` & `lfg_llama-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 05:42:57.779185 lfg_llama-1.0.1/
--rw-r--r--   0 ob907      (502) staff       (20)     1592 2024-04-29 05:42:57.779001 lfg_llama-1.0.1/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      871 2024-04-28 18:18:21.000000 lfg_llama-1.0.1/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 05:42:57.777771 lfg_llama-1.0.1/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.0.1/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     1177 2024-04-28 18:11:14.000000 lfg_llama-1.0.1/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 05:42:57.778807 lfg_llama-1.0.1/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1592 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      260 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       33 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)       14 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)      876 2024-04-29 05:41:33.000000 lfg_llama-1.0.1/pyproject.toml
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-04-29 05:42:57.779229 lfg_llama-1.0.1/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      684 2024-04-29 05:42:02.000000 lfg_llama-1.0.1/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 06:43:34.257384 lfg_llama-1.0.2/
+-rw-r--r--   0 ob907      (502) staff       (20)     1592 2024-04-29 06:43:34.257197 lfg_llama-1.0.2/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      871 2024-04-28 18:18:21.000000 lfg_llama-1.0.2/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 06:43:34.256085 lfg_llama-1.0.2/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.0.2/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     1146 2024-04-29 06:42:22.000000 lfg_llama-1.0.2/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 06:43:34.257015 lfg_llama-1.0.2/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1592 2024-04-29 06:43:34.000000 lfg_llama-1.0.2/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      260 2024-04-29 06:43:34.000000 lfg_llama-1.0.2/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-04-29 06:43:34.000000 lfg_llama-1.0.2/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       33 2024-04-29 06:43:34.000000 lfg_llama-1.0.2/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       14 2024-04-29 06:43:34.000000 lfg_llama-1.0.2/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-04-29 06:43:34.000000 lfg_llama-1.0.2/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)      876 2024-04-29 06:43:31.000000 lfg_llama-1.0.2/pyproject.toml
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-04-29 06:43:34.257432 lfg_llama-1.0.2/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      684 2024-04-29 06:43:05.000000 lfg_llama-1.0.2/setup.py
```

### Comparing `lfg_llama-1.0.1/PKG-INFO` & `lfg_llama-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.0.1
+Version: 1.0.2
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: Bjarne Oeverli <bjarneocodes@gmail.com>
 Maintainer-email: Bjarne Oeverli <bjarneocodes@gmail.com>
 Project-URL: Homepage, https://github.com/bjarneo/lfg-llama
 Project-URL: Documentation, https://github.com/bjarneo/lfg-llama
 Project-URL: Repository, https://github.com/bjarneo/lfg-llama
```

### Comparing `lfg_llama-1.0.1/README.md` & `lfg_llama-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.0.1/lfg/cli.py` & `lfg_llama-1.0.2/lfg/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,9 +27,8 @@
         description="Use LFG to chat with the Llama as a sysadmin / haxor. \nExample: lfg 'how to kill a process in linux?'"
     )
 
     if arg:
         chat(" ".join(arg))
 
 
-if __name__ == "__main__":
-    sys.exit(main(sys.argv[1:]))
+sys.exit(main(sys.argv[1:]))
```

### Comparing `lfg_llama-1.0.1/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-1.0.2/lfg_llama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.0.1
+Version: 1.0.2
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: Bjarne Oeverli <bjarneocodes@gmail.com>
 Maintainer-email: Bjarne Oeverli <bjarneocodes@gmail.com>
 Project-URL: Homepage, https://github.com/bjarneo/lfg-llama
 Project-URL: Documentation, https://github.com/bjarneo/lfg-llama
 Project-URL: Repository, https://github.com/bjarneo/lfg-llama
```

### Comparing `lfg_llama-1.0.1/pyproject.toml` & `lfg_llama-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lfg-llama"
-version = "1.0.1"
+version = "1.0.2"
 dependencies = [
   "ollama==0.1.9",
 ]
 requires-python = ">=3.8"
 authors = [
   {name = "Bjarne Oeverli", email = "bjarneocodes@gmail.com"}
 ]
```

### Comparing `lfg_llama-1.0.1/setup.py` & `lfg_llama-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         install_requires = map(lambda s: s.strip(), req_txt.readlines()[2:])
 
     return list(install_requires)
 
 
 setup(
     name="lfg-llama",
-    version="1.0.0",
+    version="1.0.2",
     description="LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bjarne Oeverli",
     author_email="bjarneocodes@gmail.com",
     packages=find_packages(),
     install_requires=["ollama"],
```

