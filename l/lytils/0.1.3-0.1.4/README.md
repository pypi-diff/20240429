# Comparing `tmp/lytils-0.1.3.tar.gz` & `tmp/lytils-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lytils-0.1.3.tar", max compression
+gzip compressed data, was "lytils-0.1.4.tar", max compression
```

## Comparing `lytils-0.1.3.tar` & `lytils-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.3/LICENSE
--rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.3/lytils/__init__.py
--rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.3/lytils/app.py
--rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.3/lytils/classes/__init__.py
--rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.3/lytils/classes/Regex.py
--rw-r--r--   0        0        0     1112 2023-10-18 01:09:58.336249 lytils-0.1.3/lytils/common.py
--rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.3/lytils/discord/__init__.py
--rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.3/lytils/discord/DiscordBot.py
--rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.3/lytils/email/__init__.py
--rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.3/lytils/email/Email.py
--rw-r--r--   0        0        0     1582 2024-04-18 01:20:59.205826 lytils-0.1.3/lytils/file.py
--rw-r--r--   0        0        0      127 2024-04-10 19:52:11.636510 lytils-0.1.3/lytils/google_sheets/__init__.py
--rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.3/lytils/google_sheets/Column.py
--rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.3/lytils/google_sheets/format.py
--rw-r--r--   0        0        0      590 2024-01-29 19:06:31.147970 lytils-0.1.3/lytils/google_sheets/GoogleSheets.py
--rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.3/lytils/google_sheets/helpers.py
--rw-r--r--   0        0        0      263 2024-01-27 02:33:06.209559 lytils-0.1.3/lytils/google_sheets/Sheet.py
--rw-r--r--   0        0        0     7541 2024-04-18 01:07:42.696739 lytils-0.1.3/lytils/google_sheets/Tab.py
--rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.3/lytils/input.py
--rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.3/lytils/logging.py
--rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.3/lytils/print.py
--rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.3/lytils/regex.py
--rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.3/lytils/surfshark.py
--rw-r--r--   0        0        0      318 2024-04-18 01:21:16.793797 lytils-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.3/README.md
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11558 2024-04-10 19:18:21.187313 lytils-0.1.4/LICENSE
+-rw-r--r--   0        0        0      111 2024-02-21 21:27:17.496125 lytils-0.1.4/lytils/__init__.py
+-rw-r--r--   0        0        0     2766 2024-03-11 19:56:01.645968 lytils-0.1.4/lytils/app.py
+-rw-r--r--   0        0        0       56 2023-08-27 21:31:43.244103 lytils-0.1.4/lytils/classes/__init__.py
+-rw-r--r--   0        0        0      926 2023-08-27 22:42:07.795890 lytils-0.1.4/lytils/classes/Regex.py
+-rw-r--r--   0        0        0     1220 2024-04-29 06:18:46.279205 lytils-0.1.4/lytils/common.py
+-rw-r--r--   0        0        0       36 2023-10-16 01:49:34.901392 lytils-0.1.4/lytils/discord/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-10 19:21:06.136630 lytils-0.1.4/lytils/discord/DiscordBot.py
+-rw-r--r--   0        0        0       37 2024-04-04 00:00:24.647508 lytils-0.1.4/lytils/email/__init__.py
+-rw-r--r--   0        0        0     2384 2024-04-12 07:06:16.170788 lytils-0.1.4/lytils/email/Email.py
+-rw-r--r--   0        0        0     1582 2024-04-18 01:20:59.205826 lytils-0.1.4/lytils/file.py
+-rw-r--r--   0        0        0      127 2024-04-10 19:52:11.636510 lytils-0.1.4/lytils/google_sheets/__init__.py
+-rw-r--r--   0        0        0      550 2024-01-30 18:05:03.141133 lytils-0.1.4/lytils/google_sheets/Column.py
+-rw-r--r--   0        0        0     3672 2024-02-22 21:29:15.946213 lytils-0.1.4/lytils/google_sheets/format.py
+-rw-r--r--   0        0        0      590 2024-01-29 19:06:31.147970 lytils-0.1.4/lytils/google_sheets/GoogleSheets.py
+-rw-r--r--   0        0        0      308 2024-04-10 19:21:06.136630 lytils-0.1.4/lytils/google_sheets/helpers.py
+-rw-r--r--   0        0        0      263 2024-01-27 02:33:06.209559 lytils-0.1.4/lytils/google_sheets/Sheet.py
+-rw-r--r--   0        0        0     7541 2024-04-18 01:07:42.696739 lytils-0.1.4/lytils/google_sheets/Tab.py
+-rw-r--r--   0        0        0      653 2024-01-23 06:16:04.647379 lytils-0.1.4/lytils/input.py
+-rw-r--r--   0        0        0      616 2024-03-12 00:24:52.524374 lytils-0.1.4/lytils/logging.py
+-rw-r--r--   0        0        0     1048 2023-12-31 07:36:14.446133 lytils-0.1.4/lytils/print.py
+-rw-r--r--   0        0        0      419 2024-02-25 07:04:04.187197 lytils-0.1.4/lytils/regex.py
+-rw-r--r--   0        0        0     1253 2024-04-12 07:03:04.806336 lytils-0.1.4/lytils/surfshark.py
+-rw-r--r--   0        0        0      318 2024-04-29 06:19:09.382747 lytils-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-10 19:18:21.187313 lytils-0.1.4/README.md
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 lytils-0.1.4/PKG-INFO
```

### Comparing `lytils-0.1.3/LICENSE` & `lytils-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/app.py` & `lytils-0.1.4/lytils/app.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/classes/Regex.py` & `lytils-0.1.4/lytils/classes/Regex.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/common.py` & `lytils-0.1.4/lytils/common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import datetime
 import subprocess
 from .print import cprint
 
-def get_todays_date(format='%m-%d-%Y'):
-    # Return today's date
-    # Default format: mm/dd/yyyy
-    today = datetime.date.today()
-    today = today.strftime(format)
-    return today
+
+def get_current_datetime(format="%Y-%m-%d %H:%M:%S"):
+    # Return current date and time
+    # Default format: yyyy-mm-dd HH:MM:SS
+    # "%Y-%m-%d %H:%M:%S" -> yyyy-mm-dd HH:MM:SS
+    # "%m-%d-%Y" -> mm-dd-yyyy
+    now = datetime.datetime.now()
+    now = now.strftime(format)
+    return now
+
 
 def format_date(input_date, input_format, output_format):
     # Parse the input string as a date
     date_object = datetime.datetime.strptime(input_date, input_format)
 
     # Format the date in the desired format
     return date_object.strftime(output_format)
 
+
 def has_numbers(input):
     return any(char.isdigit() for char in input)
 
+
 def terminate_app(app_name):
     try:
         # Use the 'taskkill' command on Windows to terminate the application
-        subprocess.run(['taskkill', '/F', '/IM', app_name], check=True)
+        subprocess.run(["taskkill", "/F", "/IM", app_name], check=True)
 
         # If you're on a Unix-based system (Linux or macOS), you can use 'pkill'
         # subprocess.run(['pkill', app_name], check=True)
 
-        cprint(f'<g>Successfully terminated {app_name}')
+        cprint(f"<g>Successfully terminated {app_name}")
     except subprocess.CalledProcessError as e:
-        cprint(f'<r>Failed to terminate {app_name}: {e}')
-        
+        cprint(f"<r>Failed to terminate {app_name}: {e}")
```

### Comparing `lytils-0.1.3/lytils/discord/DiscordBot.py` & `lytils-0.1.4/lytils/discord/DiscordBot.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/email/Email.py` & `lytils-0.1.4/lytils/email/Email.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/file.py` & `lytils-0.1.4/lytils/file.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/google_sheets/Column.py` & `lytils-0.1.4/lytils/google_sheets/Column.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/google_sheets/format.py` & `lytils-0.1.4/lytils/google_sheets/format.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/google_sheets/GoogleSheets.py` & `lytils-0.1.4/lytils/google_sheets/GoogleSheets.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/google_sheets/Tab.py` & `lytils-0.1.4/lytils/google_sheets/Tab.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/input.py` & `lytils-0.1.4/lytils/input.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/logging.py` & `lytils-0.1.4/lytils/logging.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/print.py` & `lytils-0.1.4/lytils/print.py`

 * *Files identical despite different names*

### Comparing `lytils-0.1.3/lytils/surfshark.py` & `lytils-0.1.4/lytils/surfshark.py`

 * *Files identical despite different names*

