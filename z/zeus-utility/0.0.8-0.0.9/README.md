# Comparing `tmp/zeus_utility-0.0.8.tar.gz` & `tmp/zeus_utility-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeus_utility-0.0.8.tar", last modified: Tue Mar 19 17:03:04 2024, max compression
+gzip compressed data, was "zeus_utility-0.0.9.tar", last modified: Tue Mar 19 17:26:04 2024, max compression
```

## Comparing `zeus_utility-0.0.8.tar` & `zeus_utility-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 17:03:04.425296 zeus_utility-0.0.8/
--rw-rw-rw-   0        0        0     1091 2023-11-13 08:55:50.000000 zeus_utility-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1189 2024-03-19 17:03:04.425296 zeus_utility-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-01-15 10:14:05.000000 zeus_utility-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 17:03:04.426296 zeus_utility-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3310 2024-03-19 17:02:31.000000 zeus_utility-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 17:03:04.412512 zeus_utility-0.0.8/zeus_utility/
--rw-rw-rw-   0        0        0        0 2023-05-22 03:12:01.000000 zeus_utility-0.0.8/zeus_utility/__init__.py
--rw-rw-rw-   0        0        0      671 2024-03-15 10:32:04.000000 zeus_utility-0.0.8/zeus_utility/io.py
--rw-rw-rw-   0        0        0     3293 2024-03-19 17:01:50.000000 zeus_utility-0.0.8/zeus_utility/parallel_executor.py
-drwxrwxrwx   0        0        0        0 2024-03-19 17:03:04.424310 zeus_utility-0.0.8/zeus_utility.egg-info/
--rw-rw-rw-   0        0        0     1189 2024-03-19 17:03:04.000000 zeus_utility-0.0.8/zeus_utility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2024-03-19 17:03:04.000000 zeus_utility-0.0.8/zeus_utility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 17:03:04.000000 zeus_utility-0.0.8/zeus_utility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 17:03:04.000000 zeus_utility-0.0.8/zeus_utility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-19 17:03:04.000000 zeus_utility-0.0.8/zeus_utility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-19 17:26:04.105517 zeus_utility-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2023-11-13 08:55:50.000000 zeus_utility-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1189 2024-03-19 17:26:04.095991 zeus_utility-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-01-15 10:14:05.000000 zeus_utility-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-19 17:26:04.105517 zeus_utility-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3310 2024-03-19 17:12:17.000000 zeus_utility-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-19 17:26:04.089470 zeus_utility-0.0.9/zeus_utility/
+-rw-rw-rw-   0        0        0        0 2023-05-22 03:12:01.000000 zeus_utility-0.0.9/zeus_utility/__init__.py
+-rw-rw-rw-   0        0        0      671 2024-03-15 10:32:04.000000 zeus_utility-0.0.9/zeus_utility/io.py
+-rw-rw-rw-   0        0        0     3301 2024-03-19 17:09:06.000000 zeus_utility-0.0.9/zeus_utility/parallel_executor.py
+drwxrwxrwx   0        0        0        0 2024-03-19 17:26:04.095002 zeus_utility-0.0.9/zeus_utility.egg-info/
+-rw-rw-rw-   0        0        0     1189 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-03-19 17:26:04.000000 zeus_utility-0.0.9/zeus_utility.egg-info/top_level.txt
```

### Comparing `zeus_utility-0.0.8/LICENSE` & `zeus_utility-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zeus_utility-0.0.8/PKG-INFO` & `zeus_utility-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeus_utility
-Version: 0.0.8
+Version: 0.0.9
 Summary: Just some useful utilities Zeus will use in almost every projects.
 Home-page: https://github.com/zeuscsc/zeus_utility.git
 Author: Zeus Chiu
 Author-email: zeuscsc@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `zeus_utility-0.0.8/setup.py` & `zeus_utility-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 NAME = 'zeus_utility'
 DESCRIPTION = 'Just some useful utilities Zeus will use in almost every projects.'
 URL = 'https://github.com/zeuscsc/zeus_utility.git'
 EMAIL = 'zeuscsc@gmail.com'
 AUTHOR = 'Zeus Chiu'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 with open('requirements.txt') as f:
     required_packages = f.readlines()
     required_packages = [pkg.strip() for pkg in required_packages]
 
 EXTRAS = {
 }
```

### Comparing `zeus_utility-0.0.8/zeus_utility/io.py` & `zeus_utility-0.0.9/zeus_utility/io.py`

 * *Files identical despite different names*

### Comparing `zeus_utility-0.0.8/zeus_utility/parallel_executor.py` & `zeus_utility-0.0.9/zeus_utility/parallel_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,23 +64,23 @@
                     kwargs=parameters
                 if not slience:
                     print(f"Running {args}")
                 run_task(task,*args, **kwargs)
                 if not slience:
                     print(f"Task done.")
                 queue.task_done()
+                if progress_bar is not None:
+                    progress_bar.update(1)
             except KeyboardInterrupt:
                 print("Main process terminated externally.")
                 break
             except BaseException as e:
                 continue_running=False
                 raise e
     for i in range(WORKERS_COUNT):
         Thread(target=worker, daemon=True).start()
     def start():
         for row in iterator:
             queue.put(row)
-            if progress_bar is not None:
-                progress_bar.update(1)
             time.sleep(waiting_time)
         queue.join()
     return start()
```

### Comparing `zeus_utility-0.0.8/zeus_utility.egg-info/PKG-INFO` & `zeus_utility-0.0.9/zeus_utility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zeus-utility
-Version: 0.0.8
+Name: zeus_utility
+Version: 0.0.9
 Summary: Just some useful utilities Zeus will use in almost every projects.
 Home-page: https://github.com/zeuscsc/zeus_utility.git
 Author: Zeus Chiu
 Author-email: zeuscsc@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

