# Comparing `tmp/xmonkey_namonica-0.1.3.tar.gz` & `tmp/xmonkey_namonica-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmonkey_namonica-0.1.3.tar", last modified: Sun Apr 28 18:25:14 2024, max compression
+gzip compressed data, was "xmonkey_namonica-0.1.4.tar", last modified: Mon Apr 29 21:43:04 2024, max compression
```

## Comparing `xmonkey_namonica-0.1.3.tar` & `xmonkey_namonica-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-28 18:25:14.628571 xmonkey_namonica-0.1.3/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.3/LICENSE
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-28 18:25:14.628372 xmonkey_namonica-0.1.3/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      555 2024-04-28 18:24:45.000000 xmonkey_namonica-0.1.3/README.md
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-28 18:25:14.628605 xmonkey_namonica-0.1.3/setup.cfg
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      352 2024-04-28 18:23:52.000000 xmonkey_namonica-0.1.3/setup.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-28 18:25:14.626663 xmonkey_namonica-0.1.3/xmonkey_namonica/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2135 2024-04-28 18:13:38.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/cli.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3716 2024-04-26 18:36:04.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/common.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-28 18:25:14.628073 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/__init__.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/base_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 22:27:16.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/cargo_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3918 2024-04-26 22:48:45.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/gen_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     3696 2024-04-28 18:23:26.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/github_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2200 2024-04-26 22:48:11.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/npm_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 17:48:03.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/nuget_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     2218 2024-04-26 17:49:28.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/pypi_handler.py
--rw-r--r--   0 ovalenzuela   (501) staff       (20)     1609 2024-04-26 18:40:38.000000 xmonkey_namonica-0.1.3/xmonkey_namonica/utils.py
-drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-28 18:25:14.628214 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       82 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/PKG-INFO
--rw-r--r--   0 ovalenzuela   (501) staff       (20)      669 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/SOURCES.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/dependency_links.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/entry_points.txt
--rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-28 18:25:14.000000 xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/top_level.txt
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-29 21:43:04.682138 xmonkey_namonica-0.1.4/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)    11357 2024-04-25 02:09:33.000000 xmonkey_namonica-0.1.4/LICENSE
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-04-29 21:43:04.681952 xmonkey_namonica-0.1.4/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1966 2024-04-29 20:51:13.000000 xmonkey_namonica-0.1.4/README.md
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       38 2024-04-29 21:43:04.682174 xmonkey_namonica-0.1.4/setup.cfg
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      343 2024-04-29 21:42:49.000000 xmonkey_namonica-0.1.4/setup.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-29 21:43:04.679287 xmonkey_namonica-0.1.4/xmonkey_namonica/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:08.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2135 2024-04-28 18:13:38.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/cli.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3716 2024-04-26 18:36:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/common.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-29 21:43:04.681467 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        0 2024-04-25 06:28:41.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/__init__.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      956 2024-04-25 07:37:41.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/base_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 22:27:16.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/cargo_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     4011 2024-04-29 20:48:00.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/gen_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     3696 2024-04-28 18:23:26.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/github_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2200 2024-04-26 22:48:11.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/npm_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2148 2024-04-26 17:48:03.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/nuget_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     2218 2024-04-26 17:49:28.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/pypi_handler.py
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)     1609 2024-04-26 18:40:38.000000 xmonkey_namonica-0.1.4/xmonkey_namonica/utils.py
+drwxr-xr-x   0 ovalenzuela   (501) staff       (20)        0 2024-04-29 21:43:04.681756 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      129 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/PKG-INFO
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)      708 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/SOURCES.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)        1 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/dependency_links.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       63 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/entry_points.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/requires.txt
+-rw-r--r--   0 ovalenzuela   (501) staff       (20)       17 2024-04-29 21:43:04.000000 xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/top_level.txt
```

### Comparing `xmonkey_namonica-0.1.3/LICENSE` & `xmonkey_namonica-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/cli.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/cli.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/common.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/common.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/base_handler.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/cargo_handler.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/cargo_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/gen_handler.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/gen_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,16 @@
                 repo_url = repo_url[4:]
             if '@' in repo_url:
                 repo_url, commit = repo_url.rsplit('@', 1)
             else:
                 commit = None
             subprocess.run(
                 ["git", "clone", repo_url, self.temp_dir],
-                check=True
+                check=True,
+                stdout=subprocess.DEVNULL,
+                stderr=subprocess.DEVNULL
             )
-            print(f"Repository cloned successfully to {self.temp_dir}")
+            logging.info(f"Repository cloned successfully to {self.temp_dir}")
         except subprocess.CalledProcessError as e:
             print(f"Failed to clone repository: {e}")
             shutil.rmtree(self.temp_dir)
             raise
```

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/github_handler.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/github_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/npm_handler.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/npm_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/nuget_handler.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/nuget_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/handlers/pypi_handler.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/handlers/pypi_handler.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica/utils.py` & `xmonkey_namonica-0.1.4/xmonkey_namonica/utils.py`

 * *Files identical despite different names*

### Comparing `xmonkey_namonica-0.1.3/xmonkey_namonica.egg-info/SOURCES.txt` & `xmonkey_namonica-0.1.4/xmonkey_namonica.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 xmonkey_namonica/cli.py
 xmonkey_namonica/common.py
 xmonkey_namonica/utils.py
 xmonkey_namonica.egg-info/PKG-INFO
 xmonkey_namonica.egg-info/SOURCES.txt
 xmonkey_namonica.egg-info/dependency_links.txt
 xmonkey_namonica.egg-info/entry_points.txt
+xmonkey_namonica.egg-info/requires.txt
 xmonkey_namonica.egg-info/top_level.txt
 xmonkey_namonica/handlers/__init__.py
 xmonkey_namonica/handlers/base_handler.py
 xmonkey_namonica/handlers/cargo_handler.py
 xmonkey_namonica/handlers/gen_handler.py
 xmonkey_namonica/handlers/github_handler.py
 xmonkey_namonica/handlers/npm_handler.py
```

