# Comparing `tmp/pycheckers-0.0.1.tar.gz` & `tmp/pycheckers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycheckers-0.0.1.tar", last modified: Mon Apr 29 06:45:40 2024, max compression
+gzip compressed data, was "pycheckers-0.0.2.tar", last modified: Mon Apr 29 07:56:39 2024, max compression
```

## Comparing `pycheckers-0.0.1.tar` & `pycheckers-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 caryl     (1000) caryl     (1000)        0 2024-04-29 06:45:40.549226 pycheckers-0.0.1/
--rw-r--r--   0 caryl     (1000) caryl     (1000)      190 2024-04-29 06:45:40.549226 pycheckers-0.0.1/PKG-INFO
--rw-r--r--   0 caryl     (1000) caryl     (1000)       83 2024-04-17 05:06:40.000000 pycheckers-0.0.1/README.md
-drwxr-xr-x   0 caryl     (1000) caryl     (1000)        0 2024-04-29 06:45:40.549226 pycheckers-0.0.1/pycheckers/
--rw-r--r--   0 caryl     (1000) caryl     (1000)        0 2024-04-29 06:39:18.000000 pycheckers-0.0.1/pycheckers/__init__.py
--rw-r--r--   0 caryl     (1000) caryl     (1000)    16380 2024-04-29 04:46:18.000000 pycheckers-0.0.1/pycheckers/checkers.py
--rwxr-xr-x   0 caryl     (1000) caryl     (1000)     5919 2024-04-29 06:09:08.000000 pycheckers-0.0.1/pycheckers/host.py
-drwxr-xr-x   0 caryl     (1000) caryl     (1000)        0 2024-04-29 06:45:40.549226 pycheckers-0.0.1/pycheckers.egg-info/
--rw-r--r--   0 caryl     (1000) caryl     (1000)      190 2024-04-29 06:45:40.000000 pycheckers-0.0.1/pycheckers.egg-info/PKG-INFO
--rw-r--r--   0 caryl     (1000) caryl     (1000)      252 2024-04-29 06:45:40.000000 pycheckers-0.0.1/pycheckers.egg-info/SOURCES.txt
--rw-r--r--   0 caryl     (1000) caryl     (1000)        1 2024-04-29 06:45:40.000000 pycheckers-0.0.1/pycheckers.egg-info/dependency_links.txt
--rw-r--r--   0 caryl     (1000) caryl     (1000)       46 2024-04-29 06:45:40.000000 pycheckers-0.0.1/pycheckers.egg-info/requires.txt
--rw-r--r--   0 caryl     (1000) caryl     (1000)       11 2024-04-29 06:45:40.000000 pycheckers-0.0.1/pycheckers.egg-info/top_level.txt
--rw-r--r--   0 caryl     (1000) caryl     (1000)       38 2024-04-29 06:45:40.549226 pycheckers-0.0.1/setup.cfg
--rw-r--r--   0 caryl     (1000) caryl     (1000)      225 2024-04-29 06:35:18.000000 pycheckers-0.0.1/setup.py
+drwxr-xr-x   0 caryl     (1000) caryl     (1000)        0 2024-04-29 07:56:39.649218 pycheckers-0.0.2/
+-rw-r--r--   0 caryl     (1000) caryl     (1000)       81 2024-04-29 07:56:39.649218 pycheckers-0.0.2/PKG-INFO
+-rw-r--r--   0 caryl     (1000) caryl     (1000)       83 2024-04-17 05:06:40.000000 pycheckers-0.0.2/README.md
+drwxr-xr-x   0 caryl     (1000) caryl     (1000)        0 2024-04-29 07:56:39.649218 pycheckers-0.0.2/pycheckers/
+-rw-r--r--   0 caryl     (1000) caryl     (1000)        0 2024-04-29 06:39:18.000000 pycheckers-0.0.2/pycheckers/__init__.py
+-rw-r--r--   0 caryl     (1000) caryl     (1000)    16380 2024-04-29 04:46:18.000000 pycheckers-0.0.2/pycheckers/checkers.py
+-rwxr-xr-x   0 caryl     (1000) caryl     (1000)     5944 2024-04-29 07:49:50.000000 pycheckers-0.0.2/pycheckers/host.py
+drwxr-xr-x   0 caryl     (1000) caryl     (1000)        0 2024-04-29 07:56:39.649218 pycheckers-0.0.2/pycheckers.egg-info/
+-rw-r--r--   0 caryl     (1000) caryl     (1000)       81 2024-04-29 07:56:39.000000 pycheckers-0.0.2/pycheckers.egg-info/PKG-INFO
+-rw-r--r--   0 caryl     (1000) caryl     (1000)      289 2024-04-29 07:56:39.000000 pycheckers-0.0.2/pycheckers.egg-info/SOURCES.txt
+-rw-r--r--   0 caryl     (1000) caryl     (1000)        1 2024-04-29 07:56:39.000000 pycheckers-0.0.2/pycheckers.egg-info/dependency_links.txt
+-rw-r--r--   0 caryl     (1000) caryl     (1000)       50 2024-04-29 07:56:39.000000 pycheckers-0.0.2/pycheckers.egg-info/entry_points.txt
+-rw-r--r--   0 caryl     (1000) caryl     (1000)       12 2024-04-29 07:56:39.000000 pycheckers-0.0.2/pycheckers.egg-info/requires.txt
+-rw-r--r--   0 caryl     (1000) caryl     (1000)       11 2024-04-29 07:56:39.000000 pycheckers-0.0.2/pycheckers.egg-info/top_level.txt
+-rw-r--r--   0 caryl     (1000) caryl     (1000)       38 2024-04-29 07:56:39.649218 pycheckers-0.0.2/setup.cfg
+-rw-r--r--   0 caryl     (1000) caryl     (1000)      278 2024-04-29 07:56:29.000000 pycheckers-0.0.2/setup.py
```

### Comparing `pycheckers-0.0.1/pycheckers/checkers.py` & `pycheckers-0.0.2/pycheckers/checkers.py`

 * *Files identical despite different names*

### Comparing `pycheckers-0.0.1/pycheckers/host.py` & `pycheckers-0.0.2/pycheckers/host.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             if move == "loss":
                 print("You lost...")
                 break
     
     return True # success
 
 
-if __name__ == "__main__":
+def main():
     while True:
         try:
             players = int(input("How many players? "))
             if players in (0,1,2):
                 break
             else:
                 print("Enter either 0, 1, or 2.")
@@ -199,8 +199,12 @@
 
             else:
                 # Nothing entered
                 print("Enter an option.")
 
     else:
         # Single player or sim
-        Board(players)
+        Board(players)
+
+
+if __name__ == "__main__":
+    main()
```

