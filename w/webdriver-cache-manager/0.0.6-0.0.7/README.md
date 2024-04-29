# Comparing `tmp/webdriver_cache_manager-0.0.6.tar.gz` & `tmp/webdriver_cache_manager-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdriver_cache_manager-0.0.6.tar", last modified: Sat Apr 27 21:33:23 2024, max compression
+gzip compressed data, was "webdriver_cache_manager-0.0.7.tar", last modified: Mon Apr 29 16:57:13 2024, max compression
```

## Comparing `webdriver_cache_manager-0.0.6.tar` & `webdriver_cache_manager-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:33:23.933195 webdriver_cache_manager-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-27 21:33:19.000000 webdriver_cache_manager-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-27 21:33:23.933195 webdriver_cache_manager-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-27 21:33:19.000000 webdriver_cache_manager-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-27 21:33:19.000000 webdriver_cache_manager-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 21:33:23.933195 webdriver_cache_manager-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:33:23.933195 webdriver_cache_manager-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:33:23.933195 webdriver_cache_manager-0.0.6/src/webdriver_cache_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 21:33:19.000000 webdriver_cache_manager-0.0.6/src/webdriver_cache_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-27 21:33:19.000000 webdriver_cache_manager-0.0.6/src/webdriver_cache_manager/webdriver_cache_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 21:33:23.933195 webdriver_cache_manager-0.0.6/src/webdriver_cache_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-27 21:33:23.000000 webdriver_cache_manager-0.0.6/src/webdriver_cache_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-27 21:33:23.000000 webdriver_cache_manager-0.0.6/src/webdriver_cache_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 21:33:23.000000 webdriver_cache_manager-0.0.6/src/webdriver_cache_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 21:33:23.000000 webdriver_cache_manager-0.0.6/src/webdriver_cache_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:13.033099 webdriver_cache_manager-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-29 16:57:13.029099 webdriver_cache_manager-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:57:13.033099 webdriver_cache_manager-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:13.029099 webdriver_cache_manager-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:13.029099 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-29 16:57:06.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager/webdriver_cache_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:57:13.029099 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-29 16:57:13.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-29 16:57:13.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:57:13.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 16:57:13.000000 webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/top_level.txt
```

### Comparing `webdriver_cache_manager-0.0.6/LICENSE` & `webdriver_cache_manager-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.6/PKG-INFO` & `webdriver_cache_manager-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.6
+Version: 0.0.7
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `webdriver_cache_manager-0.0.6/README.md` & `webdriver_cache_manager-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `webdriver_cache_manager-0.0.6/pyproject.toml` & `webdriver_cache_manager-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "webdriver_cache_manager"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Muhammad Nawaz", email="MNawaz6935@gmail.com" },
 ]
 description = "Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `webdriver_cache_manager-0.0.6/src/webdriver_cache_manager/webdriver_cache_manager.py` & `webdriver_cache_manager-0.0.7/src/webdriver_cache_manager/webdriver_cache_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import csv
 import logging
 import os
 import subprocess
+import threading
 import time
 import traceback
 import psutil
 
 CSV_FILE_PATH = os.path.join(os.path.expanduser("~"), ".wcm")
 os.makedirs(CSV_FILE_PATH, exist_ok=True)
 temp_file_path = os.path.join(CSV_FILE_PATH, "temp.csv")
@@ -16,14 +17,23 @@
     global CSV_FILE_PATH
     with open(CSV_FILE_PATH, 'a+', newline='') as csvfile:
         fieldnames = ['File Path', 'ChromeDriver PID', 'Chrome PID']
         writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
         writer.writerow({'File Path': file_path, 'ChromeDriver PID': chrome_driver_pid, 'Chrome PID': chrome_pid})
 
 
+def save_pids_list_to_csv(file_path, chrome_driver_pid, chrome_pid_list):
+    global CSV_FILE_PATH
+    with open(CSV_FILE_PATH, 'a+', newline='') as csvfile:
+        fieldnames = ['File Path', 'ChromeDriver PID', 'Chrome PID']
+        writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
+        for chrome_pid in chrome_pid_list:
+            writer.writerow({'File Path': file_path, 'ChromeDriver PID': chrome_driver_pid, 'Chrome PID': chrome_pid})
+
+
 def read_pids_from_csv(file_path):
     global CSV_FILE_PATH
     chrome_driver_pid = []
     chrome_pid = []
     if not os.path.exists(CSV_FILE_PATH):
         return chrome_driver_pid, chrome_pid
     try:
@@ -59,24 +69,29 @@
     try:
         subprocess.run(['taskkill', '/pid', str(pid), '/f'], check=True)
         logging.info(f"Process with PID {pid} killed successfully.")
     except subprocess.CalledProcessError as e:
         logging.info(f"Failed to kill process with PID {pid}. Error: {e}")
 
 
-def KillChromeAndDriverCache(file_path):
-    chrome_driver_pids, chrome_pids = read_pids_from_csv(file_path)
+def start_killing_processes(chrome_driver_pids, chrome_pids):
     if chrome_driver_pids:
         for pid in chrome_driver_pids:
             kill_process_by_pid(pid)
     if chrome_pids:
         for pid in chrome_pids:
             kill_process_by_pid(pid)
 
 
+def KillChromeAndDriverCache(file_path):
+    chrome_driver_pids, chrome_pids = read_pids_from_csv(file_path)
+    t = threading.Thread(target=start_killing_processes, args=(chrome_driver_pids, chrome_pids,))
+    t.start()
+
+
 def ManageChromeDriverCache(driver, file_path):
     try:
         # Get the ChromeDriver process ID
         chrome_driver_pid = driver.service.process.pid
         logging.info(f"ChromeDriver Process ID: {chrome_driver_pid}")
 
         # Find the PID of the Chrome process opened by the WebDriver
@@ -85,16 +100,32 @@
             if 'chrome.exe' in process.info['name']:
                 try:
                     if chrome_driver_pid == psutil.Process(process.info['pid']).ppid():
                         chrome_pid = process.info['pid']
                         break
                 except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
                     pass
-
+        linked_pids = set()  # Set to store unique process IDs
         if chrome_pid:
             logging.info(f"Chrome Process ID:{chrome_pid}")
+
+            def traverse_process_tree(pid):
+                try:
+                    process = psutil.Process(pid)
+                    children = process.children(recursive=True)
+                    linked_pids.add(pid)
+                    for child in children:
+                        linked_pids.add(child.pid)
+                        traverse_process_tree(child.pid)
+                except psutil.NoSuchProcess:
+                    pass
+
+            traverse_process_tree(chrome_pid)
+            print("Linked Process IDs:", linked_pids)
         else:
             logging.info("Chrome process not found for this WebDriver instance.")
         KillChromeAndDriverCache(file_path)
         save_pids_to_csv(file_path, chrome_driver_pid, chrome_pid)
+        if linked_pids:
+            save_pids_list_to_csv(file_path, chrome_driver_pid, linked_pids)
     except Exception as e:
         logging.error(traceback.format_exc())
```

### Comparing `webdriver_cache_manager-0.0.6/src/webdriver_cache_manager.egg-info/PKG-INFO` & `webdriver_cache_manager-0.0.7/src/webdriver_cache_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webdriver_cache_manager
-Version: 0.0.6
+Version: 0.0.7
 Summary: Optimize WebDriver usage in Selenium with Python. Manage processes, terminate efficiently, and handle PIDs using CSV. Simplify automation!
 Author-email: Muhammad Nawaz <MNawaz6935@gmail.com>
 Project-URL: Homepage, https://github.com/mnawaz6935/webdriver_cache_manager
 Project-URL: Issues, https://github.com/mnawaz6935/webdriver_cache_manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

