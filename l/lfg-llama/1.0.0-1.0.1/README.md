# Comparing `tmp/lfg_llama-1.0.0.tar.gz` & `tmp/lfg_llama-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.0.0.tar", last modified: Sun Apr 28 18:18:03 2024, max compression
+gzip compressed data, was "lfg_llama-1.0.1.tar", last modified: Mon Apr 29 05:42:57 2024, max compression
```

## Comparing `lfg_llama-1.0.0.tar` & `lfg_llama-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-28 18:18:03.760511 lfg_llama-1.0.0/
--rw-r--r--   0 ob907      (502) staff       (20)     1082 2024-04-28 18:18:03.760321 lfg_llama-1.0.0/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      865 2024-04-28 18:13:56.000000 lfg_llama-1.0.0/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-28 18:18:03.759367 lfg_llama-1.0.0/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.0.0/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     1177 2024-04-28 18:11:14.000000 lfg_llama-1.0.0/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-28 18:18:03.760112 lfg_llama-1.0.0/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1082 2024-04-28 18:18:03.000000 lfg_llama-1.0.0/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      213 2024-04-28 18:18:03.000000 lfg_llama-1.0.0/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-04-28 18:18:03.000000 lfg_llama-1.0.0/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-04-28 18:18:03.000000 lfg_llama-1.0.0/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-04-28 18:18:03.000000 lfg_llama-1.0.0/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-04-28 18:18:03.760568 lfg_llama-1.0.0/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      696 2024-04-28 18:17:38.000000 lfg_llama-1.0.0/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 05:42:57.779185 lfg_llama-1.0.1/
+-rw-r--r--   0 ob907      (502) staff       (20)     1592 2024-04-29 05:42:57.779001 lfg_llama-1.0.1/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      871 2024-04-28 18:18:21.000000 lfg_llama-1.0.1/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 05:42:57.777771 lfg_llama-1.0.1/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.0.1/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     1177 2024-04-28 18:11:14.000000 lfg_llama-1.0.1/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-04-29 05:42:57.778807 lfg_llama-1.0.1/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     1592 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      260 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       33 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       14 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-04-29 05:42:57.000000 lfg_llama-1.0.1/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)      876 2024-04-29 05:41:33.000000 lfg_llama-1.0.1/pyproject.toml
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-04-29 05:42:57.779229 lfg_llama-1.0.1/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      684 2024-04-29 05:42:02.000000 lfg_llama-1.0.1/setup.py
```

### Comparing `lfg_llama-1.0.0/README.md` & `lfg_llama-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # install the llama3 LLM
 ollama run llama3
 
 # start ollama
 ollama server
 
 # install LFG
-pip install lfg
+pip install lfg-llama
 ```
 
 ## Usage
 
 ```bash
 lfg kill port 3000
```

### Comparing `lfg_llama-1.0.0/lfg/cli.py` & `lfg_llama-1.0.1/lfg/cli.py`

 * *Files identical despite different names*

### Comparing `lfg_llama-1.0.0/setup.py` & `lfg_llama-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,10 +15,10 @@
     version="1.0.0",
     description="LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bjarne Oeverli",
     author_email="bjarneocodes@gmail.com",
     packages=find_packages(),
-    install_requires=get_install_requires(),
+    install_requires=["ollama"],
     entry_points={"console_scripts": ["lfg=lfg.cli:main"]},
 )
```

