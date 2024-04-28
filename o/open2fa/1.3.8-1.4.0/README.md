# Comparing `tmp/open2fa-1.3.8-py3-none-any.whl.zip` & `tmp/open2fa-1.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20605 bytes, number of entries: 17
+Zip file size: 20670 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      113 b- defN 24-Feb-12 01:03 open2fa/__init__.py
 -rw-r--r--  2.0 unx    10069 b- defN 24-Mar-25 23:32 open2fa/cli.py
--rw-r--r--  2.0 unx     4747 b- defN 24-Mar-19 13:19 open2fa/cli_utils.py
+-rw-r--r--  2.0 unx     4747 b- defN 24-Apr-27 23:38 open2fa/cli_utils.py
 -rw-r--r--  2.0 unx     4334 b- defN 24-Mar-24 22:21 open2fa/common.py
 -rw-r--r--  2.0 unx      660 b- defN 24-Apr-11 22:49 open2fa/config.py
 -rw-r--r--  2.0 unx      923 b- defN 24-Mar-21 19:32 open2fa/ex.py
--rw-r--r--  2.0 unx    17949 b- defN 24-Apr-14 18:43 open2fa/main.py
--rw-r--r--  2.0 unx     1742 b- defN 24-Mar-23 03:26 open2fa/msgs.py
+-rw-r--r--  2.0 unx    17991 b- defN 24-Apr-28 22:53 open2fa/main.py
+-rw-r--r--  2.0 unx     1814 b- defN 24-Apr-28 22:58 open2fa/msgs.py
 -rw-r--r--  2.0 unx     2248 b- defN 24-Apr-16 18:10 open2fa/totp.py
 -rw-r--r--  2.0 unx     2139 b- defN 24-Mar-21 19:36 open2fa/utils.py
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-18 05:10 open2fa/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Apr-18 05:10 open2fa-1.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx    11088 b- defN 24-Apr-18 05:10 open2fa-1.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-18 05:10 open2fa-1.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-18 05:10 open2fa-1.3.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-18 05:10 open2fa-1.3.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1284 b- defN 24-Apr-18 05:10 open2fa-1.3.8.dist-info/RECORD
-17 files, 58538 bytes uncompressed, 18535 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-28 23:02 open2fa/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11088 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1284 b- defN 24-Apr-28 23:03 open2fa-1.4.0.dist-info/RECORD
+17 files, 58652 bytes uncompressed, 18600 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: open2fa/utils.py
 Comment: 
 
 Filename: open2fa/version.py
 Comment: 
 
-Filename: open2fa-1.3.8.dist-info/LICENSE
+Filename: open2fa-1.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: open2fa-1.3.8.dist-info/METADATA
+Filename: open2fa-1.4.0.dist-info/METADATA
 Comment: 
 
-Filename: open2fa-1.3.8.dist-info/WHEEL
+Filename: open2fa-1.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: open2fa-1.3.8.dist-info/entry_points.txt
+Filename: open2fa-1.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: open2fa-1.3.8.dist-info/top_level.txt
+Filename: open2fa-1.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: open2fa-1.3.8.dist-info/RECORD
+Filename: open2fa-1.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## open2fa/main.py

```diff
@@ -181,14 +181,15 @@
         prev_lines = 0
         try:
             _sep = '    '
             name_pool = [str(s.name) for s in self.secrets]
             if name is not None:
                 name_pool = [n for n in name_pool if n.find(name) != -1]
             MAXH = 0
+            print(f'\n{MSGS.CTRL_C}\n')
             while repeat is None or repeat > 0:
                 tsize = get_terminal_size()
                 TW, TH = tsize.columns, tsize.lines
                 TW, TH = max(TW, 30), max(TH, 4)
                 MAXH = max(MAXH, TH)
 
                 name_w = max(10, max(len(n) for n in name_pool))
@@ -246,15 +247,15 @@
 
                 if repeat is not None:
                     repeat -= 1
                 if repeat != 0:
                     time.sleep(delay)
 
         except KeyboardInterrupt:
-            print("\nCancelled by user.")
+            print(f"\n{MSGS.SIGINT_MSG}\n")
 
     @logf()
     def write_secrets(self) -> None:
         """Write the secrets to the secrets.json file."""
         write_secrets_json(
             self.secrets_json_path, [s.json() for s in self.secrets]
         )
```

## open2fa/msgs.py

```diff
@@ -52,7 +52,10 @@
 
 
 ADD_NO_NAME_SEC = 'open2fa add was called without name or secret.'
 ADD_SEC_PROMPT = 'Enter TOTP secret: '
 ADD_NAME_PROMPT = 'Enter name for secret: '
 ADD_INVALID_SECRET = 'Invalid TOTP secret: {} enter a valid secret.'
 ADD_SEC_NAME = '\nAdded TOTP secret: {} with name {}\n'
+
+CTRL_C = 'Press Ctrl+C to exit... '
+SIGINT_MSG = '(SIGINT) Exiting...'
```

## open2fa/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.3.8"
+__version__ = "1.4.0"
```

## Comparing `open2fa-1.3.8.dist-info/LICENSE` & `open2fa-1.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `open2fa-1.3.8.dist-info/METADATA` & `open2fa-1.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open2fa
-Version: 1.3.8
+Version: 1.4.0
 Summary: A 2FA CLI tool for generating 2FA codes using TOTP secrets, with an optional SECURE remote api, and an optional web ui enabling 2FA code generation from any device
 Author-email: Cary Carter <ccarterdev@gmail.com>
 Project-URL: Homepage, https://open2fa.liberfy.ai
 Project-URL: Repository, https://github.com/cc-d/open2fa
 Project-URL: Issues, https://github.com/cc-d/open2fa/issues
 Project-URL: Server, https://github.com/cc-d/open2fa-server
 Project-URL: Documentation, https://github.com/cc-d/open2fa
```

## Comparing `open2fa-1.3.8.dist-info/RECORD` & `open2fa-1.4.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 open2fa/__init__.py,sha256=-I3NORVmVqf-xgcfaF3KRHZEidP6u0HyV3sMkhAO5RA,113
 open2fa/cli.py,sha256=srswxrGSgQIa0rVYd1xfT7cl9sVJahkrv3t_okYp_a4,10069
 open2fa/cli_utils.py,sha256=OU_M-MNDYNx6dIVw1vSmXBk2mYxYmC098DQ9YxcivR4,4747
 open2fa/common.py,sha256=44pDlWVJhfGbCW_TczO7Urc_0JFpynfEkP6FJYd6r-Y,4334
 open2fa/config.py,sha256=VixFalMSdS2vOtVhs6D2Jh1-wIeo98fMvD1BZIJbJog,660
 open2fa/ex.py,sha256=nc_q0UdNdbk-KFR0XmcQbpdhtqbs1SnWcus4XzqAq70,923
-open2fa/main.py,sha256=FA878v5GxJj3Co8Vvoms1zNWXIRgtM1HveoZY28SJwU,17949
-open2fa/msgs.py,sha256=iMBtZbL-a1zro4FgeYneo1Q6MsfNrGafCL-isbv38Qw,1742
+open2fa/main.py,sha256=CWU1iJC2Gt78I8AdL_BAB7VH5Ad3GYUS3smhbdbWEq8,17991
+open2fa/msgs.py,sha256=xdQ_tdhopmJz2qJqVkdk-0QCwLFkoNo5y7UBeUl0rno,1814
 open2fa/totp.py,sha256=WKZXQlGlaa7eZK5SR3yBIfUq6PhDAUJpWAiwWJewmMY,2248
 open2fa/utils.py,sha256=j6Nom2zc51aDsY79d1sW6qmSyXrGirIa0cP7AE_wNDg,2139
-open2fa/version.py,sha256=47xEhOdVR5Y8-pZH8aVP6Z2UhhY8jGWTQ-rJHt5fIeU,22
-open2fa-1.3.8.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
-open2fa-1.3.8.dist-info/METADATA,sha256=1Nkv0wqBrGE0v8l3VuZVY2kQkP3E4udC1x_vu29Hzys,11088
-open2fa-1.3.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-open2fa-1.3.8.dist-info/entry_points.txt,sha256=zPU8uscEguG4dPJRNgafME-18JtTcsovmVrjylRQcIU,52
-open2fa-1.3.8.dist-info/top_level.txt,sha256=c_HZ2KecVkcZ3f3dF-SOX7eyDBn9UpLe8IYmZZjXvdA,8
-open2fa-1.3.8.dist-info/RECORD,,
+open2fa/version.py,sha256=8UhoYEXHs1Oai7BW_ExBmuwWnRI-yMG_u1fQAXMizHQ,22
+open2fa-1.4.0.dist-info/LICENSE,sha256=Oqp_kvYTcHXculbJJhyN32EDhEOA5omV6gG9fRpSKmA,1068
+open2fa-1.4.0.dist-info/METADATA,sha256=U6aenzSOPNuBxUy4g2PiGATQdbg4kpUq62-EwUOQ8Cw,11088
+open2fa-1.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+open2fa-1.4.0.dist-info/entry_points.txt,sha256=zPU8uscEguG4dPJRNgafME-18JtTcsovmVrjylRQcIU,52
+open2fa-1.4.0.dist-info/top_level.txt,sha256=c_HZ2KecVkcZ3f3dF-SOX7eyDBn9UpLe8IYmZZjXvdA,8
+open2fa-1.4.0.dist-info/RECORD,,
```

