# Comparing `tmp/pisa_ssh-0.0.1.tar.gz` & `tmp/pisa_ssh-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisa_ssh-0.0.1.tar", last modified: Mon Apr 29 19:57:13 2024, max compression
+gzip compressed data, was "pisa_ssh-0.0.2.tar", last modified: Mon Apr 29 20:07:58 2024, max compression
```

## Comparing `pisa_ssh-0.0.1.tar` & `pisa_ssh-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-29 19:57:13.163167 pisa_ssh-0.0.1/
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-04-29 19:12:27.000000 pisa_ssh-0.0.1/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     2619 2024-04-29 19:57:13.163167 pisa_ssh-0.0.1/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     1456 2024-04-29 19:28:53.000000 pisa_ssh-0.0.1/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1940 2024-04-29 19:53:00.000000 pisa_ssh-0.0.1/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2024-04-29 19:57:13.163167 pisa_ssh-0.0.1/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-29 19:57:13.159834 pisa_ssh-0.0.1/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-29 19:57:13.159834 pisa_ssh-0.0.1/src/pisa/
--rw-r--r--   0 michael   (1000) michael   (1000)       22 2024-04-29 19:31:14.000000 pisa_ssh-0.0.1/src/pisa/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-29 19:57:13.163167 pisa_ssh-0.0.1/src/pisa_ssh.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     2619 2024-04-29 19:57:13.000000 pisa_ssh-0.0.1/src/pisa_ssh.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      232 2024-04-29 19:57:13.000000 pisa_ssh-0.0.1/src/pisa_ssh.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-29 19:57:13.000000 pisa_ssh-0.0.1/src/pisa_ssh.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       19 2024-04-29 19:57:13.000000 pisa_ssh-0.0.1/src/pisa_ssh.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-04-29 19:57:13.000000 pisa_ssh-0.0.1/src/pisa_ssh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 20:07:40.000000 pisa_ssh-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-29 20:07:40.000000 pisa_ssh-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-29 20:07:40.000000 pisa_ssh-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:58.186134 pisa_ssh-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/src/pisa/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 20:07:40.000000 pisa_ssh-0.0.2/src/pisa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:07:58.190134 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 20:07:58.000000 pisa_ssh-0.0.2/src/pisa_ssh.egg-info/top_level.txt
```

### Comparing `pisa_ssh-0.0.1/LICENSE` & `pisa_ssh-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.0.1/PKG-INFO` & `pisa_ssh-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SSH Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
-Project-URL: Homepage, https://github.com/MitchiLaser/pisa/docs/README.md
+Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pisa_ssh-0.0.1/README.md` & `pisa_ssh-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pisa_ssh-0.0.1/pyproject.toml` & `pisa_ssh-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     #"black",
     #"isort",
     "build",
     "twine", 
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/MitchiLaser/pisa/docs/README.md"
+"Homepage" = "https://github.com/MitchiLaser/pisa/blob/main/docs/README.md" # TODO: Maybe provide github pages build and HTML page
 "Repository" = "https://github.com/MitchiLaser/pisa"
 
 #[project.scripts]
 #kafe2go = "kafe2.fit.tools.kafe2go:kafe2go" # TODO: Update for pisa dispatcher
 
 ########## TODO ???? ##############
```

### Comparing `pisa_ssh-0.0.1/src/pisa_ssh.egg-info/PKG-INFO` & `pisa_ssh-0.0.2/src/pisa_ssh.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pisa-ssh
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SSH Infrastructure for Scalable Applications (PISA)
 Author-email: Michael Hohenstein <michael@hohenste.in>
 License: MIT
-Project-URL: Homepage, https://github.com/MitchiLaser/pisa/docs/README.md
+Project-URL: Homepage, https://github.com/MitchiLaser/pisa/blob/main/docs/README.md
 Project-URL: Repository, https://github.com/MitchiLaser/pisa
 Keywords: data,analysis,education,university,students,physics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
```

