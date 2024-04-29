# Comparing `tmp/PyCourrier-0.1.3.tar.gz` & `tmp/PyCourrier-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCourrier-0.1.3.tar", last modified: Mon Apr 29 17:56:03 2024, max compression
+gzip compressed data, was "PyCourrier-0.1.4.tar", last modified: Mon Apr 29 19:26:26 2024, max compression
```

## Comparing `PyCourrier-0.1.3.tar` & `PyCourrier-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:56:03.951079 PyCourrier-0.1.3/
--rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2956 2024-04-29 17:56:03.946199 PyCourrier-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 17:56:03.890057 PyCourrier-0.1.3/PyCourrier/
--rw-rw-rw-   0        0        0     4086 2024-04-29 17:46:44.000000 PyCourrier-0.1.3/PyCourrier/MailSender.py
--rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.3/PyCourrier/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:56:03.943282 PyCourrier-0.1.3/PyCourrier.egg-info/
--rw-rw-rw-   0        0        0     2956 2024-04-29 17:56:03.000000 PyCourrier-0.1.3/PyCourrier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-29 17:56:03.000000 PyCourrier-0.1.3/PyCourrier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:56:03.000000 PyCourrier-0.1.3/PyCourrier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-29 17:56:03.000000 PyCourrier-0.1.3/PyCourrier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2516 2024-04-29 17:54:10.000000 PyCourrier-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 17:56:03.952055 PyCourrier-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      686 2024-04-29 17:55:38.000000 PyCourrier-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:26:26.541402 PyCourrier-0.1.4/
+-rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3098 2024-04-29 19:26:26.538408 PyCourrier-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 19:26:26.502212 PyCourrier-0.1.4/PyCourrier/
+-rw-rw-rw-   0        0        0     4392 2024-04-29 19:17:51.000000 PyCourrier-0.1.4/PyCourrier/MailSender.py
+-rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.4/PyCourrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 19:26:26.536414 PyCourrier-0.1.4/PyCourrier.egg-info/
+-rw-rw-rw-   0        0        0     3098 2024-04-29 19:26:26.000000 PyCourrier-0.1.4/PyCourrier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-29 19:26:26.000000 PyCourrier-0.1.4/PyCourrier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 19:26:26.000000 PyCourrier-0.1.4/PyCourrier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 19:26:26.000000 PyCourrier-0.1.4/PyCourrier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2658 2024-04-29 19:21:38.000000 PyCourrier-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 19:26:26.542398 PyCourrier-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      686 2024-04-29 19:24:51.000000 PyCourrier-0.1.4/setup.py
```

### Comparing `PyCourrier-0.1.3/LICENSE` & `PyCourrier-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCourrier-0.1.3/PKG-INFO` & `PyCourrier-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCourrier
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple email sender utility
 Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,33 +34,33 @@
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
 from PyCourrier import MailSender
 
-# Initialize MailSender with your SMTP server credentials
-mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
+# Create a MailSender instance within a context manager
+with MailSender('your_email@gmail.com', 'your_generated_app_password') as mailSender:
 
-# Set email message content
-mailer.set_message(
-    in_subject='Hello from MailSender!',
+    # Set recipients
+    recipients = ['Abdelmajiid.habouch@gmail.com']
+    mailSender.set_recipients(recipients)
+
+    # Set email message details
+    in_subject='Hello from PyCourrier!',
     in_plaintext='This is the plain text content of the email.',
-    in_from='your_email@gmail.com',
-    in_htmltext='<p>This is the HTML content of the email.</p>',
-    attachment="path/to/file",
-    filename="filename_for_the_attachment"
-)
-
-# Add recipients
-mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
-
-# Send the email to all recipients
-mailer.connect()  # Connect to the SMTP server
-mailer.send_all()  # Send the email and disconnect
+    in_from='your_email@gmail.com (optioanl)',
+    in_htmltext='<p>This is the HTML content of the email.</p> (optional)',
+    attachment="path/to/file (optional)",
+    filename="filename_for_the_attachment (optional)"
+
+    mailSender.set_message(in_plaintext=plaintext_body, in_subject=in_subject, in_from=in_from, in_htmltext=in_htmltext, attachment=attachment, filename=filename)
+
+    # Send the email to all recipients
+    mailSender.send_all()
 ```
 
 ## Constructor Parameters
 - **in_username**: Your email address used for SMTP login.
 - **in_password**: Your Generated app password.
 - **in_server**: Tuple containing the SMTP server address and port (default is Gmail).
 - **use_SSL**: Boolean indicating whether to use SSL (True) or TLS (False, default) for the connection.
```

### Comparing `PyCourrier-0.1.3/PyCourrier/MailSender.py` & `PyCourrier-0.1.4/PyCourrier/MailSender.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import smtplib
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.mime.base import MIMEBase
 from email import encoders
+from contextlib import AbstractContextManager
 
-class MailSender:
+class MailSender(AbstractContextManager):
     """
     A class that facilitates composing and sending emails via SMTP.
 
     :param in_username: Username for mail server login
     :param in_password: Password for mail server login
     :param in_server: SMTP server to connect to (default is Gmail)
     :param use_SSL: Use SSL (True) or TLS (False, default) for connection
     """
     def __init__(self, in_username, in_password, in_server=("smtp.gmail.com", 587), use_SSL=False):
         self.username = in_username
         self.password = in_password
         self.server_name, self.server_port = in_server
         self.use_SSL = use_SSL
-        self.smtpserver = smtplib.SMTP_SSL(self.server_name, self.server_port) if self.use_SSL else smtplib.SMTP(self.server_name, self.server_port)
+        self.smtpserver = None
         self.connected = False
         self.recipients = []
 
+    def __enter__(self):
+        self.connect()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.disconnect()
+
     def __str__(self):
         return f"MailSender connected to {self.server_name}:{self.server_port}, Connected: {self.connected}"
 
     def set_message(self, in_plaintext="", in_subject="", in_from=None, in_htmltext=None, attachment=None, filename=None):
         """
         Compose an email message.
 
@@ -68,26 +76,33 @@
     def add_recipient(self, in_recipient):
         """Add a recipient to the list of recipients."""
         self.recipients.append(in_recipient)
 
     def connect(self):
         """Connect to the SMTP server."""
         try:
-            self.smtpserver.starttls() if not self.use_SSL else None
+            if self.use_SSL:
+                self.smtpserver = smtplib.SMTP_SSL(self.server_name, self.server_port)
+            else:
+                self.smtpserver = smtplib.SMTP(self.server_name, self.server_port)
+                self.smtpserver.starttls()
+
             self.smtpserver.login(self.username, self.password)
             self.connected = True
             print(f"Connected to {self.server_name}")
-        except smtplib.SMTPException as error:
-            print(f"SMTP Error: {error}")
+        except (smtplib.SMTPException, ConnectionError) as error:
             self.connected = False
+            raise ConnectionError(f"Failed to connect to {self.server_name}: {error}")
+
 
     def disconnect(self):
         """Disconnect from the SMTP server."""
-        self.smtpserver.quit()
-        self.connected = False
+        if self.smtpserver:
+            self.smtpserver.quit()
+            self.connected = False
 
     def send_all(self, close_connection=True):
         """Send the email to all recipients."""
         if not self.connected:
             raise ConnectionError("Not connected to any server. Please connect first.")
 
         for recipient in self.recipients:
@@ -95,10 +110,7 @@
             print(f"Sending to {recipient}")
 
             # Convert the message to a string and then send it
             self.smtpserver.sendmail(self.username, recipient, self.msg.as_string())
 
         print("All messages sent")
 
-        if close_connection:
-            self.disconnect()
-            print("Connection closed")
```

### Comparing `PyCourrier-0.1.3/PyCourrier.egg-info/PKG-INFO` & `PyCourrier-0.1.4/PyCourrier.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCourrier
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple email sender utility
 Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,33 +34,33 @@
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
 from PyCourrier import MailSender
 
-# Initialize MailSender with your SMTP server credentials
-mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
+# Create a MailSender instance within a context manager
+with MailSender('your_email@gmail.com', 'your_generated_app_password') as mailSender:
 
-# Set email message content
-mailer.set_message(
-    in_subject='Hello from MailSender!',
+    # Set recipients
+    recipients = ['Abdelmajiid.habouch@gmail.com']
+    mailSender.set_recipients(recipients)
+
+    # Set email message details
+    in_subject='Hello from PyCourrier!',
     in_plaintext='This is the plain text content of the email.',
-    in_from='your_email@gmail.com',
-    in_htmltext='<p>This is the HTML content of the email.</p>',
-    attachment="path/to/file",
-    filename="filename_for_the_attachment"
-)
-
-# Add recipients
-mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
-
-# Send the email to all recipients
-mailer.connect()  # Connect to the SMTP server
-mailer.send_all()  # Send the email and disconnect
+    in_from='your_email@gmail.com (optioanl)',
+    in_htmltext='<p>This is the HTML content of the email.</p> (optional)',
+    attachment="path/to/file (optional)",
+    filename="filename_for_the_attachment (optional)"
+
+    mailSender.set_message(in_plaintext=plaintext_body, in_subject=in_subject, in_from=in_from, in_htmltext=in_htmltext, attachment=attachment, filename=filename)
+
+    # Send the email to all recipients
+    mailSender.send_all()
 ```
 
 ## Constructor Parameters
 - **in_username**: Your email address used for SMTP login.
 - **in_password**: Your Generated app password.
 - **in_server**: Tuple containing the SMTP server address and port (default is Gmail).
 - **use_SSL**: Boolean indicating whether to use SSL (True) or TLS (False, default) for the connection.
```

### Comparing `PyCourrier-0.1.3/README.md` & `PyCourrier-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
 from PyCourrier import MailSender
 
-# Initialize MailSender with your SMTP server credentials
-mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
+# Create a MailSender instance within a context manager
+with MailSender('your_email@gmail.com', 'your_generated_app_password') as mailSender:
 
-# Set email message content
-mailer.set_message(
-    in_subject='Hello from MailSender!',
+    # Set recipients
+    recipients = ['Abdelmajiid.habouch@gmail.com']
+    mailSender.set_recipients(recipients)
+
+    # Set email message details
+    in_subject='Hello from PyCourrier!',
     in_plaintext='This is the plain text content of the email.',
-    in_from='your_email@gmail.com',
-    in_htmltext='<p>This is the HTML content of the email.</p>',
-    attachment="path/to/file",
-    filename="filename_for_the_attachment"
-)
-
-# Add recipients
-mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
-
-# Send the email to all recipients
-mailer.connect()  # Connect to the SMTP server
-mailer.send_all()  # Send the email and disconnect
+    in_from='your_email@gmail.com (optioanl)',
+    in_htmltext='<p>This is the HTML content of the email.</p> (optional)',
+    attachment="path/to/file (optional)",
+    filename="filename_for_the_attachment (optional)"
+
+    mailSender.set_message(in_plaintext=plaintext_body, in_subject=in_subject, in_from=in_from, in_htmltext=in_htmltext, attachment=attachment, filename=filename)
+
+    # Send the email to all recipients
+    mailSender.send_all()
 ```
 
 ## Constructor Parameters
 - **in_username**: Your email address used for SMTP login.
 - **in_password**: Your Generated app password.
 - **in_server**: Tuple containing the SMTP server address and port (default is Gmail).
 - **use_SSL**: Boolean indicating whether to use SSL (True) or TLS (False, default) for the connection.
```

### Comparing `PyCourrier-0.1.3/setup.py` & `PyCourrier-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='PyCourrier',
-    version='0.1.3',
+    version='0.1.4',
     packages=find_packages(),
     description='A simple email sender utility',
     author='Abdelmajid Habouch',
     author_email='Habush1610@gmail.com',
     url='https://github.com/mjiid/PyCourrier',
     license='MIT',
     install_requires=[
```

