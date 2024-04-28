# Comparing `tmp/scrippy-mail-2.0.0.tar.gz` & `tmp/scrippy_mail-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrippy-mail-2.0.0.tar", last modified: Wed Oct 11 12:44:41 2023, max compression
+gzip compressed data, was "scrippy_mail-2.0.1.tar", last modified: Sun Apr 28 22:35:26 2024, max compression
```

## Comparing `scrippy-mail-2.0.0.tar` & `scrippy_mail-2.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.422563 scrippy-mail-2.0.0/
--rwxr-xr-x   0 root         (0) root         (0)     1179 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8376 2023-10-11 12:44:41.422563 scrippy-mail-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6842 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      210 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1303 2023-10-11 12:44:41.423563 scrippy-mail-2.0.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)       38 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.409564 scrippy-mail-2.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.412564 scrippy-mail-2.0.0/src/scrippy_mail/
--rw-r--r--   0 root         (0) root         (0)      219 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/src/scrippy_mail/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.414564 scrippy-mail-2.0.0/src/scrippy_mail/ciphers/
--rw-r--r--   0 root         (0) root         (0)      221 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/src/scrippy_mail/ciphers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.414564 scrippy-mail-2.0.0/src/scrippy_mail/files/
--rw-r--r--   0 root         (0) root         (0)      860 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/src/scrippy_mail/files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.415564 scrippy-mail-2.0.0/src/scrippy_mail/imap/
--rw-r--r--   0 root         (0) root         (0)    19146 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/src/scrippy_mail/imap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.415564 scrippy-mail-2.0.0/src/scrippy_mail/pop/
--rw-r--r--   0 root         (0) root         (0)     7477 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/src/scrippy_mail/pop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.416564 scrippy-mail-2.0.0/src/scrippy_mail/smtp/
--rw-r--r--   0 root         (0) root         (0)     7980 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/src/scrippy_mail/smtp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.414564 scrippy-mail-2.0.0/src/scrippy_mail.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8376 2023-10-11 12:44:41.000000 scrippy-mail-2.0.0/src/scrippy_mail.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      471 2023-10-11 12:44:41.000000 scrippy-mail-2.0.0/src/scrippy_mail.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-11 12:44:41.000000 scrippy-mail-2.0.0/src/scrippy_mail.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      264 2023-10-11 12:44:41.000000 scrippy-mail-2.0.0/src/scrippy_mail.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-11 12:44:41.000000 scrippy-mail-2.0.0/src/scrippy_mail.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-11 12:44:41.416564 scrippy-mail-2.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)     3617 2023-10-11 12:43:38.000000 scrippy-mail-2.0.0/tests/test_mail.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.897558 scrippy_mail-2.0.1/
+-rwxr-xr-x   0 root         (0) root         (0)     1179 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8376 2024-04-28 22:35:26.897558 scrippy_mail-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6842 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      210 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1303 2024-04-28 22:35:26.909558 scrippy_mail-2.0.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)       38 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.883559 scrippy_mail-2.0.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.887559 scrippy_mail-2.0.1/src/scrippy_mail/
+-rw-r--r--   0 root         (0) root         (0)      219 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/src/scrippy_mail/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.889559 scrippy_mail-2.0.1/src/scrippy_mail/ciphers/
+-rw-r--r--   0 root         (0) root         (0)      221 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/src/scrippy_mail/ciphers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.889559 scrippy_mail-2.0.1/src/scrippy_mail/files/
+-rw-r--r--   0 root         (0) root         (0)      860 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/src/scrippy_mail/files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.889559 scrippy_mail-2.0.1/src/scrippy_mail/imap/
+-rw-r--r--   0 root         (0) root         (0)    19146 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/src/scrippy_mail/imap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.890559 scrippy_mail-2.0.1/src/scrippy_mail/pop/
+-rw-r--r--   0 root         (0) root         (0)     7477 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/src/scrippy_mail/pop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.890559 scrippy_mail-2.0.1/src/scrippy_mail/smtp/
+-rw-r--r--   0 root         (0) root         (0)     8200 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/src/scrippy_mail/smtp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.891559 scrippy_mail-2.0.1/src/scrippy_mail.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8376 2024-04-28 22:35:26.000000 scrippy_mail-2.0.1/src/scrippy_mail.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      471 2024-04-28 22:35:26.000000 scrippy_mail-2.0.1/src/scrippy_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-28 22:35:26.000000 scrippy_mail-2.0.1/src/scrippy_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      264 2024-04-28 22:35:26.000000 scrippy_mail-2.0.1/src/scrippy_mail.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-28 22:35:26.000000 scrippy_mail-2.0.1/src/scrippy_mail.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-28 22:35:26.890559 scrippy_mail-2.0.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     3617 2024-04-28 22:34:29.000000 scrippy_mail-2.0.1/tests/test_mail.py
```

### Comparing `scrippy-mail-2.0.0/LICENSE` & `scrippy_mail-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrippy-mail-2.0.0/PKG-INFO` & `scrippy_mail-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-mail
-Version: 2.0.0
+Version: 2.0.1
 Summary: "Client SMTP, POP3 et SpamAssassin pour le cadriciel Scrippy"
 Home-page: https://codeberg.org/scrippy/scrippy-mail
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrippy-mail-2.0.0/README.md` & `scrippy_mail-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `scrippy-mail-2.0.0/setup.cfg` & `scrippy_mail-2.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 2.0.0
+version = 2.0.1
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Intended Audience :: Developers
 	Intended Audience :: System Administrators
```

### Comparing `scrippy-mail-2.0.0/src/scrippy_mail/files/__init__.py` & `scrippy_mail-2.0.1/src/scrippy_mail/files/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-mail-2.0.0/src/scrippy_mail/imap/__init__.py` & `scrippy_mail-2.0.1/src/scrippy_mail/imap/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-mail-2.0.0/src/scrippy_mail/pop/__init__.py` & `scrippy_mail-2.0.1/src/scrippy_mail/pop/__init__.py`

 * *Files identical despite different names*

### Comparing `scrippy-mail-2.0.0/src/scrippy_mail/smtp/__init__.py` & `scrippy_mail-2.0.1/src/scrippy_mail/smtp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,22 +27,23 @@
     Note: The ``ssl`` and ``starttls`` arguments are mutually exclusive. You may user either one of them or none but not both at the same time.
   """
   @property
   def connected(self):
     return self.client is not None and self._connected
 
   def __init__(self, host, port=110, username=None, password=None,
-               ssl=False, starttls=False, ssl_verify=True,
+               helo=None, ssl=False, starttls=False, ssl_verify=True,
                timeout=60, exit_on_error=True):
     self.client = None
     self._connected = False
     self.username = username
     self.password = password
     self.host = host
     self.port = port
+    self.local_hostname = helo
     self.ssl = ssl
     self.starttls = starttls
     self.ssl_verify = ssl_verify
     self.timeout = timeout
     self.exit_on_error = exit_on_error
 
   def __enter__(self):
@@ -81,22 +82,24 @@
       if self.ssl_verify:
         ctx.verify_mode = ssl.CERT_REQUIRED
         ctx.check_hostname = True
         ctx.set_default_verify_paths()
         ctx.load_default_certs()
     logger.info(f"Connecting to {self.host}:{self.port}")
     if self.ssl:
-      self.client = smtplib.SMTP_SSL(self.host,
-                                     self.port,
-                                     self.timeout,
+      self.client = smtplib.SMTP_SSL(host=self.host,
+                                     port=self.port,
+                                     timeout=self.timeout,
+                                     local_hostname=self.local_hostname,
                                      context=ctx)
     else:
-      self.client = smtplib.SMTP(self.host,
-                                 self.port,
-                                 self.timeout)
+      self.client = smtplib.SMTP(host=self.host,
+                                 port=self.port,
+                                 local_hostname=self.local_hostname,
+                                 timeout=self.timeout)
       if self.starttls:
         logger.info("Using STARTTLS")
         response = self.client.starttls(context=ctx)
     if self.starttls is None or self.starttls is False:
       response = self.client.connect(self.host,
                                      self.port)
     self.client.ehlo_or_helo_if_needed()
```

### Comparing `scrippy-mail-2.0.0/src/scrippy_mail.egg-info/PKG-INFO` & `scrippy_mail-2.0.1/src/scrippy_mail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrippy-mail
-Version: 2.0.0
+Version: 2.0.1
 Summary: "Client SMTP, POP3 et SpamAssassin pour le cadriciel Scrippy"
 Home-page: https://codeberg.org/scrippy/scrippy-mail
 Author: Michael Costa, Florent Chevalier
 Author-email: michael.costa@mcos.nc, florent.chevalier.nc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scrippy-mail-2.0.0/tests/test_mail.py` & `scrippy_mail-2.0.1/tests/test_mail.py`

 * *Files identical despite different names*

