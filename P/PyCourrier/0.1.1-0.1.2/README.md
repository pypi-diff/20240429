# Comparing `tmp/pycourrier-0.1.1.tar.gz` & `tmp/PyCourrier-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycourrier-0.1.1.tar", last modified: Mon Apr 29 17:18:37 2024, max compression
+gzip compressed data, was "PyCourrier-0.1.2.tar", last modified: Mon Apr 29 17:51:56 2024, max compression
```

## Comparing `pycourrier-0.1.1.tar` & `PyCourrier-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:18:36.980414 pycourrier-0.1.1/
--rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 pycourrier-0.1.1/LICENSE
-drwxrwxrwx   0        0        0        0 2024-04-29 17:18:36.889303 pycourrier-0.1.1/MailSender/
--rw-rw-rw-   0        0        0     4086 2024-04-29 16:54:54.000000 pycourrier-0.1.1/MailSender/MailSender.py
--rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 pycourrier-0.1.1/MailSender/__init__.py
--rw-rw-rw-   0        0        0     2878 2024-04-29 17:18:36.970338 pycourrier-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2439 2024-04-29 17:09:37.000000 pycourrier-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 17:18:36.965287 pycourrier-0.1.1/pycourrier.egg-info/
--rw-rw-rw-   0        0        0     2878 2024-04-29 17:18:36.000000 pycourrier-0.1.1/pycourrier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-29 17:18:36.000000 pycourrier-0.1.1/pycourrier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:18:36.000000 pycourrier-0.1.1/pycourrier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-29 17:18:36.000000 pycourrier-0.1.1/pycourrier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 17:18:36.981389 pycourrier-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      685 2024-04-29 17:18:04.000000 pycourrier-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:51:56.393719 PyCourrier-0.1.2/
+-rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2911 2024-04-29 17:51:56.377213 PyCourrier-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 17:51:56.115434 PyCourrier-0.1.2/PyCourrier/
+-rw-rw-rw-   0        0        0     4086 2024-04-29 17:46:44.000000 PyCourrier-0.1.2/PyCourrier/MailSender.py
+-rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.2/PyCourrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:51:56.371355 PyCourrier-0.1.2/PyCourrier.egg-info/
+-rw-rw-rw-   0        0        0     2911 2024-04-29 17:51:55.000000 PyCourrier-0.1.2/PyCourrier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-29 17:51:56.000000 PyCourrier-0.1.2/PyCourrier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:51:55.000000 PyCourrier-0.1.2/PyCourrier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 17:51:55.000000 PyCourrier-0.1.2/PyCourrier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2471 2024-04-29 17:47:40.000000 PyCourrier-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:51:56.395671 PyCourrier-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      686 2024-04-29 17:51:52.000000 PyCourrier-0.1.2/setup.py
```

### Comparing `pycourrier-0.1.1/LICENSE` & `PyCourrier-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycourrier-0.1.1/MailSender/MailSender.py` & `PyCourrier-0.1.2/PyCourrier/MailSender.py`

 * *Files identical despite different names*

### Comparing `pycourrier-0.1.1/PKG-INFO` & `PyCourrier-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: pycourrier
-Version: 0.1.1
+Name: PyCourrier
+Version: 0.1.2
 Summary: A simple email sender utility
-Home-page: https://github.com/mjiid/pycourier
+Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -42,15 +42,16 @@
 mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
 
 # Set email message content
 mailer.set_message(
     in_subject='Hello from MailSender!',
     in_plaintext='This is the plain text content of the email.',
     in_from='your_email@gmail.com',
-    in_htmltext='<p>This is the HTML content of the email.</p>'
+    in_htmltext='<p>This is the HTML content of the email.</p>',
+    attachment="path/to/file"
 )
 
 # Add recipients
 mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
 
 # Send the email to all recipients
 mailer.connect()  # Connect to the SMTP server
```

### Comparing `pycourrier-0.1.1/README.md` & `PyCourrier-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
 
 # Set email message content
 mailer.set_message(
     in_subject='Hello from MailSender!',
     in_plaintext='This is the plain text content of the email.',
     in_from='your_email@gmail.com',
-    in_htmltext='<p>This is the HTML content of the email.</p>'
+    in_htmltext='<p>This is the HTML content of the email.</p>',
+    attachment="path/to/file"
 )
 
 # Add recipients
 mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
 
 # Send the email to all recipients
 mailer.connect()  # Connect to the SMTP server
```

### Comparing `pycourrier-0.1.1/pycourrier.egg-info/PKG-INFO` & `PyCourrier-0.1.2/PyCourrier.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: pycourrier
-Version: 0.1.1
+Name: PyCourrier
+Version: 0.1.2
 Summary: A simple email sender utility
-Home-page: https://github.com/mjiid/pycourier
+Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -42,15 +42,16 @@
 mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
 
 # Set email message content
 mailer.set_message(
     in_subject='Hello from MailSender!',
     in_plaintext='This is the plain text content of the email.',
     in_from='your_email@gmail.com',
-    in_htmltext='<p>This is the HTML content of the email.</p>'
+    in_htmltext='<p>This is the HTML content of the email.</p>',
+    attachment="path/to/file"
 )
 
 # Add recipients
 mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
 
 # Send the email to all recipients
 mailer.connect()  # Connect to the SMTP server
```

### Comparing `pycourrier-0.1.1/setup.py` & `PyCourrier-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
-    name='pycourrier',
-    version='0.1.1',
+    name='PyCourrier',
+    version='0.1.2',
     packages=find_packages(),
     description='A simple email sender utility',
     author='Abdelmajid Habouch',
     author_email='Habush1610@gmail.com',
-    url='https://github.com/mjiid/pycourier',
+    url='https://github.com/mjiid/PyCourrier',
     license='MIT',
     install_requires=[
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

