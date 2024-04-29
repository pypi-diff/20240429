# Comparing `tmp/nucleus_driver-1.5.8.tar.gz` & `tmp/nucleus_driver-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucleus_driver-1.5.8.tar", last modified: Mon Sep 11 09:10:53 2023, max compression
+gzip compressed data, was "nucleus_driver-1.5.9.tar", last modified: Thu Sep 21 09:34:20 2023, max compression
```

## Comparing `nucleus_driver-1.5.8.tar` & `nucleus_driver-1.5.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-09-11 09:10:53.893756 nucleus_driver-1.5.8/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.8/LICENSE.txt
--rw-r--r--   0 martin    (1000) martin    (1000)     9514 2023-09-11 09:10:53.893756 nucleus_driver-1.5.8/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.8/README.md
--rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.8/pyproject.toml
--rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-09-11 09:10:53.893756 nucleus_driver-1.5.8/setup.cfg
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-09-11 09:10:53.889756 nucleus_driver-1.5.8/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-09-11 09:10:53.893756 nucleus_driver-1.5.8/src/nucleus_driver/
--rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.8/src/nucleus_driver/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.8/src/nucleus_driver/_assert.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    54767 2023-09-11 08:40:18.000000 nucleus_driver-1.5.8/src/nucleus_driver/_commands.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    17100 2023-08-03 07:58:07.000000 nucleus_driver-1.5.8/src/nucleus_driver/_connection.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    25406 2023-06-26 13:48:04.000000 nucleus_driver-1.5.8/src/nucleus_driver/_download.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-26 13:48:04.000000 nucleus_driver-1.5.8/src/nucleus_driver/_flash.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-26 13:48:04.000000 nucleus_driver-1.5.8/src/nucleus_driver/_logger.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.8/src/nucleus_driver/_messages.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    39943 2023-08-30 08:04:48.000000 nucleus_driver-1.5.8/src/nucleus_driver/_parser.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.8/src/nucleus_driver/_syslog.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    19462 2023-09-11 09:08:01.000000 nucleus_driver-1.5.8/src/nucleus_driver/app.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11213 2023-07-31 12:03:10.000000 nucleus_driver-1.5.8/src/nucleus_driver/nucleus_driver.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-09-11 09:10:53.893756 nucleus_driver-1.5.8/src/nucleus_driver.egg-info/
--rw-r--r--   0 martin    (1000) martin    (1000)     9514 2023-09-11 09:10:53.000000 nucleus_driver-1.5.8/src/nucleus_driver.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-09-11 09:10:53.000000 nucleus_driver-1.5.8/src/nucleus_driver.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-09-11 09:10:53.000000 nucleus_driver-1.5.8/src/nucleus_driver.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-09-11 09:10:53.000000 nucleus_driver-1.5.8/src/nucleus_driver.egg-info/entry_points.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-09-11 09:10:53.000000 nucleus_driver-1.5.8/src/nucleus_driver.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-09-11 09:10:53.000000 nucleus_driver-1.5.8/src/nucleus_driver.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-09-21 09:34:20.895445 nucleus_driver-1.5.9/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1063 2023-03-27 14:20:11.000000 nucleus_driver-1.5.9/LICENSE.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)     9514 2023-09-21 09:34:20.895445 nucleus_driver-1.5.9/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8987 2023-03-27 14:20:11.000000 nucleus_driver-1.5.9/README.md
+-rw-rw-r--   0 martin    (1000) martin    (1000)      105 2023-03-27 14:20:11.000000 nucleus_driver-1.5.9/pyproject.toml
+-rw-rw-r--   0 martin    (1000) martin    (1000)      737 2023-09-21 09:34:20.895445 nucleus_driver-1.5.9/setup.cfg
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-09-21 09:34:20.895445 nucleus_driver-1.5.9/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-09-21 09:34:20.895445 nucleus_driver-1.5.9/src/nucleus_driver/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       71 2023-03-27 14:20:11.000000 nucleus_driver-1.5.9/src/nucleus_driver/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-03-27 14:20:11.000000 nucleus_driver-1.5.9/src/nucleus_driver/_assert.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    54767 2023-09-11 08:40:18.000000 nucleus_driver-1.5.9/src/nucleus_driver/_commands.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17100 2023-08-03 07:58:07.000000 nucleus_driver-1.5.9/src/nucleus_driver/_connection.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    25794 2023-09-21 09:20:32.000000 nucleus_driver-1.5.9/src/nucleus_driver/_download.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    16602 2023-06-26 13:48:04.000000 nucleus_driver-1.5.9/src/nucleus_driver/_flash.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10853 2023-06-26 13:48:04.000000 nucleus_driver-1.5.9/src/nucleus_driver/_logger.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      470 2023-03-27 14:20:11.000000 nucleus_driver-1.5.9/src/nucleus_driver/_messages.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    39943 2023-08-30 08:04:48.000000 nucleus_driver-1.5.9/src/nucleus_driver/_parser.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2523 2023-03-27 14:20:11.000000 nucleus_driver-1.5.9/src/nucleus_driver/_syslog.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    19462 2023-09-11 09:08:01.000000 nucleus_driver-1.5.9/src/nucleus_driver/app.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11213 2023-07-31 12:03:10.000000 nucleus_driver-1.5.9/src/nucleus_driver/nucleus_driver.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-09-21 09:34:20.895445 nucleus_driver-1.5.9/src/nucleus_driver.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     9514 2023-09-21 09:34:20.000000 nucleus_driver-1.5.9/src/nucleus_driver.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)      673 2023-09-21 09:34:20.000000 nucleus_driver-1.5.9/src/nucleus_driver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-09-21 09:34:20.000000 nucleus_driver-1.5.9/src/nucleus_driver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       77 2023-09-21 09:34:20.000000 nucleus_driver-1.5.9/src/nucleus_driver.egg-info/entry_points.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       26 2023-09-21 09:34:20.000000 nucleus_driver-1.5.9/src/nucleus_driver.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       15 2023-09-21 09:34:20.000000 nucleus_driver-1.5.9/src/nucleus_driver.egg-info/top_level.txt
```

### Comparing `nucleus_driver-1.5.8/LICENSE.txt` & `nucleus_driver-1.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/PKG-INFO` & `nucleus_driver-1.5.9/src/nucleus_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nucleus_driver
-Version: 1.5.8
+Name: nucleus-driver
+Version: 1.5.9
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.5.8/README.md` & `nucleus_driver-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/setup.cfg` & `nucleus_driver-1.5.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nucleus_driver
-version = 1.5.8
+version = 1.5.9
 author = Martin Bergene Johansen
 author_email = martin.johansen@nortekgroup.com
 description = driver for the Nortek Nucleus
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nortekgroup/nucleus_driver
 classifiers =
```

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/_assert.py` & `nucleus_driver-1.5.9/src/nucleus_driver/_assert.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/_commands.py` & `nucleus_driver-1.5.9/src/nucleus_driver/_commands.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/_connection.py` & `nucleus_driver-1.5.9/src/nucleus_driver/_connection.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/_download.py` & `nucleus_driver-1.5.9/src/nucleus_driver/_download.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
         self._path = str(Path.cwd()) + '/download'
 
         self.dvl_download_statistics = dict()
         self.dvl_download_statistics['successful bytes'] = 0
         self.dvl_download_statistics['failed bytes'] = 0
 
-        self.PACKET_LENGTH = 1024 * 1024
+        self.PACKET_LENGTH_TCP = 1024 * 1024
+        self.PACKET_LENGTH_SERIAL = 1024 * 10
 
     @staticmethod
     def _handle_crc(dvl_data: bytes):
 
         crc_fail_data = b''
 
         while True:
@@ -382,15 +383,15 @@
         def _download_data() -> (bool, bytes):
 
             failed_attempt = False
             for attempt in range(1, 11):
                 
                 timeout = min(2 + attempt, 10)  # First iteration is 3s, 3 last iterations are 10s
 
-                status, package = self.download_data(fid=download_parameters['fid'], src=1, sa=index, length=min(download_parameters['end'] - index, self.PACKET_LENGTH), timeout=timeout)
+                status, package = self.download_data(fid=download_parameters['fid'], src=1, sa=index, length=min(download_parameters['end'] - index, packet_length), timeout=timeout)
 
                 if status:
                     if failed_attempt:
                         self.messages.write_message('successfully received packet at index {}'.format(index))
                     break
                 else:
                     failed_attempt = True
@@ -451,14 +452,19 @@
 
                 else:
                     return _data
 
         if not _check_arguments():
             return False
 
+        if self.connection.get_connection_type() == 'tcp':
+            packet_length = self.PACKET_LENGTH_TCP
+        else:
+            packet_length = self.PACKET_LENGTH_SERIAL
+
         status, download_parameters = self.get_download_parameters(src=1, fid=fid, sa=sa, length=length)
         if not status:
             return False
 
         status, get_all = _download_get_all()
 
         if status:
@@ -477,15 +483,15 @@
 
             with open(file_path + '/dvl_data.bin', 'wb') as file, open(file_path + '/dvl_crc_fails.bin', 'wb') as fail_file:
 
                 file.write(get_all)
 
                 downloaded_bytes = 0
                 data = b''
-                for index in range(download_parameters['sa'], download_parameters['end'], self.PACKET_LENGTH):
+                for index in range(download_parameters['sa'], download_parameters['end'], packet_length):
 
                     status, package = _download_data()
 
                     downloaded_bytes += len(package)
                     percentage = downloaded_bytes * 100 / (download_parameters['end'] - download_parameters['sa'])
                     if percentage > percentage_previous + 1:
                         if percentage > 99:
@@ -525,15 +531,15 @@
         def _download_data() -> (bool, bytes):
 
             failed_attempt = False
             for attempt in range(1, 11):
 
                 timeout = min(2 + attempt, 10)  # First iteration is 3s, 3 last iterations are 10s
 
-                status, package = self.download_data(fid=download_parameters['fid'], src=0, sa=index, length=min(download_parameters['end'] - index, self.PACKET_LENGTH), timeout=timeout)
+                status, package = self.download_data(fid=download_parameters['fid'], src=0, sa=index, length=min(download_parameters['end'] - index, packet_length), timeout=timeout)
 
                 if status:
                     if failed_attempt:
                         self.messages.write_message('successfully received packet at index {}'.format(index))
                     break
                 else:
                     failed_attempt = True
@@ -557,14 +563,19 @@
                 return False, b''
 
             return True, get_all
 
         if not _check_arguments():
             return False
 
+        if self.connection.get_connection_type() == 'tcp':
+            packet_length = self.PACKET_LENGTH_TCP
+        else:
+            packet_length = self.PACKET_LENGTH_SERIAL
+
         status, download_parameters = self.get_download_parameters(src=0, fid=fid, sa=sa, length=length)
         if not status:
             return False
 
         status, get_all = _download_get_all()
 
         if status:
@@ -580,15 +591,15 @@
             with open(file_path + '/get_all.txt', 'w') as file:
                 file.writelines(get_all.decode())
 
             with open(file_path + '/nucleus_data.bin', 'wb') as file:
                 file.write(get_all)
                 percentage_previous = -1
                 downloaded_bytes = 0
-                for index in range(download_parameters['sa'], download_parameters['end'], self.PACKET_LENGTH):
+                for index in range(download_parameters['sa'], download_parameters['end'], packet_length):
 
                     status, package = _download_data()
 
                     downloaded_bytes += len(package)
                     percentage = downloaded_bytes * 100 / (download_parameters['end'] - download_parameters['sa'])
                     if percentage > percentage_previous + 1:
                         if percentage > 99:
```

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/_flash.py` & `nucleus_driver-1.5.9/src/nucleus_driver/_flash.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/_logger.py` & `nucleus_driver-1.5.9/src/nucleus_driver/_logger.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/_parser.py` & `nucleus_driver-1.5.9/src/nucleus_driver/_parser.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/_syslog.py` & `nucleus_driver-1.5.9/src/nucleus_driver/_syslog.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/app.py` & `nucleus_driver-1.5.9/src/nucleus_driver/app.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver/nucleus_driver.py` & `nucleus_driver-1.5.9/src/nucleus_driver/nucleus_driver.py`

 * *Files identical despite different names*

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver.egg-info/PKG-INFO` & `nucleus_driver-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: nucleus-driver
-Version: 1.5.8
+Name: nucleus_driver
+Version: 1.5.9
 Summary: driver for the Nortek Nucleus
 Home-page: https://github.com/nortekgroup/nucleus_driver
 Author: Martin Bergene Johansen
 Author-email: martin.johansen@nortekgroup.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nucleus_driver-1.5.8/src/nucleus_driver.egg-info/SOURCES.txt` & `nucleus_driver-1.5.9/src/nucleus_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

