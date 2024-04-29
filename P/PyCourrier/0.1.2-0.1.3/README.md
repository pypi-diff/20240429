# Comparing `tmp/PyCourrier-0.1.2.tar.gz` & `tmp/PyCourrier-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCourrier-0.1.2.tar", last modified: Mon Apr 29 17:51:56 2024, max compression
+gzip compressed data, was "PyCourrier-0.1.3.tar", last modified: Mon Apr 29 17:56:03 2024, max compression
```

## Comparing `PyCourrier-0.1.2.tar` & `PyCourrier-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 17:51:56.393719 PyCourrier-0.1.2/
--rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2911 2024-04-29 17:51:56.377213 PyCourrier-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 17:51:56.115434 PyCourrier-0.1.2/PyCourrier/
--rw-rw-rw-   0        0        0     4086 2024-04-29 17:46:44.000000 PyCourrier-0.1.2/PyCourrier/MailSender.py
--rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.2/PyCourrier/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 17:51:56.371355 PyCourrier-0.1.2/PyCourrier.egg-info/
--rw-rw-rw-   0        0        0     2911 2024-04-29 17:51:55.000000 PyCourrier-0.1.2/PyCourrier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-29 17:51:56.000000 PyCourrier-0.1.2/PyCourrier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 17:51:55.000000 PyCourrier-0.1.2/PyCourrier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-29 17:51:55.000000 PyCourrier-0.1.2/PyCourrier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2471 2024-04-29 17:47:40.000000 PyCourrier-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 17:51:56.395671 PyCourrier-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      686 2024-04-29 17:51:52.000000 PyCourrier-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:56:03.951079 PyCourrier-0.1.3/
+-rw-rw-rw-   0        0        0     1096 2024-04-29 15:53:14.000000 PyCourrier-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2956 2024-04-29 17:56:03.946199 PyCourrier-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 17:56:03.890057 PyCourrier-0.1.3/PyCourrier/
+-rw-rw-rw-   0        0        0     4086 2024-04-29 17:46:44.000000 PyCourrier-0.1.3/PyCourrier/MailSender.py
+-rw-rw-rw-   0        0        0       34 2024-04-29 16:41:54.000000 PyCourrier-0.1.3/PyCourrier/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 17:56:03.943282 PyCourrier-0.1.3/PyCourrier.egg-info/
+-rw-rw-rw-   0        0        0     2956 2024-04-29 17:56:03.000000 PyCourrier-0.1.3/PyCourrier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-29 17:56:03.000000 PyCourrier-0.1.3/PyCourrier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 17:56:03.000000 PyCourrier-0.1.3/PyCourrier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 17:56:03.000000 PyCourrier-0.1.3/PyCourrier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2516 2024-04-29 17:54:10.000000 PyCourrier-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 17:56:03.952055 PyCourrier-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      686 2024-04-29 17:55:38.000000 PyCourrier-0.1.3/setup.py
```

### Comparing `PyCourrier-0.1.2/LICENSE` & `PyCourrier-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCourrier-0.1.2/PKG-INFO` & `PyCourrier-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,44 @@
-Metadata-Version: 2.1
-Name: PyCourrier
-Version: 0.1.2
-Summary: A simple email sender utility
-Home-page: https://github.com/mjiid/PyCourrier
-Author: Abdelmajid Habouch
-Author-email: Habush1610@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyCourrier
 
 PyCourrier is a Python package that simplifies composing and sending emails using SMTP. This package allows you to connect to an SMTP server, set up email content (including plain text, HTML, and attachments), specify recipients, and send emails seamlessly.
 
 ## Features
 
 - Connect to SMTP servers (supports both SSL and TLS connections).
 - Compose emails with plaintext, HTML, and attachments.
 - Set multiple recipients for each email.
 - Easily send emails to all recipients with a single function call.
 
 ## Installation
 
-You can install pycourrier using pip:
+You can install PyCourrier using pip:
 
 ```bash
-pip install pycourrier
+pip install PyCourrier
 ```
 
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
-from pycourrier import MailSender
+from PyCourrier import MailSender
 
 # Initialize MailSender with your SMTP server credentials
 mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
 
 # Set email message content
 mailer.set_message(
     in_subject='Hello from MailSender!',
     in_plaintext='This is the plain text content of the email.',
     in_from='your_email@gmail.com',
     in_htmltext='<p>This is the HTML content of the email.</p>',
-    attachment="path/to/file"
+    attachment="path/to/file",
+    filename="filename_for_the_attachment"
 )
 
 # Add recipients
 mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
 
 # Send the email to all recipients
 mailer.connect()  # Connect to the SMTP server
@@ -68,11 +55,11 @@
 - **set_recipients**: Set the list of email recipients.
 - **add_recipient**: Add a single recipient to the list of recipients.
 - **connect**: Connect to the SMTP server.
 - **disconnect**: Disconnect from the SMTP server.
 - **send_all**: Send the composed email to all recipients.
 
 ## Contribution
-Contributions to pycourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/pycourrier/issues).
+Contributions to PyCourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/PyCourrier/issues).
 
 ## License
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `PyCourrier-0.1.2/PyCourrier/MailSender.py` & `PyCourrier-0.1.3/PyCourrier/MailSender.py`

 * *Files identical despite different names*

### Comparing `PyCourrier-0.1.2/PyCourrier.egg-info/PKG-INFO` & `PyCourrier-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCourrier
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple email sender utility
 Home-page: https://github.com/mjiid/PyCourrier
 Author: Abdelmajid Habouch
 Author-email: Habush1610@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,37 +21,38 @@
 - Connect to SMTP servers (supports both SSL and TLS connections).
 - Compose emails with plaintext, HTML, and attachments.
 - Set multiple recipients for each email.
 - Easily send emails to all recipients with a single function call.
 
 ## Installation
 
-You can install pycourrier using pip:
+You can install PyCourrier using pip:
 
 ```bash
-pip install pycourrier
+pip install PyCourrier
 ```
 
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
-from pycourrier import MailSender
+from PyCourrier import MailSender
 
 # Initialize MailSender with your SMTP server credentials
 mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
 
 # Set email message content
 mailer.set_message(
     in_subject='Hello from MailSender!',
     in_plaintext='This is the plain text content of the email.',
     in_from='your_email@gmail.com',
     in_htmltext='<p>This is the HTML content of the email.</p>',
-    attachment="path/to/file"
+    attachment="path/to/file",
+    filename="filename_for_the_attachment"
 )
 
 # Add recipients
 mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
 
 # Send the email to all recipients
 mailer.connect()  # Connect to the SMTP server
@@ -68,11 +69,11 @@
 - **set_recipients**: Set the list of email recipients.
 - **add_recipient**: Add a single recipient to the list of recipients.
 - **connect**: Connect to the SMTP server.
 - **disconnect**: Disconnect from the SMTP server.
 - **send_all**: Send the composed email to all recipients.
 
 ## Contribution
-Contributions to pycourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/pycourrier/issues).
+Contributions to PyCourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/PyCourrier/issues).
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `PyCourrier-0.1.2/README.md` & `PyCourrier-0.1.3/PyCourrier.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,58 @@
+Metadata-Version: 2.1
+Name: PyCourrier
+Version: 0.1.3
+Summary: A simple email sender utility
+Home-page: https://github.com/mjiid/PyCourrier
+Author: Abdelmajid Habouch
+Author-email: Habush1610@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyCourrier
 
 PyCourrier is a Python package that simplifies composing and sending emails using SMTP. This package allows you to connect to an SMTP server, set up email content (including plain text, HTML, and attachments), specify recipients, and send emails seamlessly.
 
 ## Features
 
 - Connect to SMTP servers (supports both SSL and TLS connections).
 - Compose emails with plaintext, HTML, and attachments.
 - Set multiple recipients for each email.
 - Easily send emails to all recipients with a single function call.
 
 ## Installation
 
-You can install pycourrier using pip:
+You can install PyCourrier using pip:
 
 ```bash
-pip install pycourrier
+pip install PyCourrier
 ```
 
 ## Usage
 
 Here's a quick guide on how to use MailSender:
 
 ```python
-from pycourrier import MailSender
+from PyCourrier import MailSender
 
 # Initialize MailSender with your SMTP server credentials
 mailer = MailSender(in_username='your_email@gmail.com', in_password='your_password')
 
 # Set email message content
 mailer.set_message(
     in_subject='Hello from MailSender!',
     in_plaintext='This is the plain text content of the email.',
     in_from='your_email@gmail.com',
     in_htmltext='<p>This is the HTML content of the email.</p>',
-    attachment="path/to/file"
+    attachment="path/to/file",
+    filename="filename_for_the_attachment"
 )
 
 # Add recipients
 mailer.set_recipients(['recipient1@example.com', 'recipient2@example.com'])
 
 # Send the email to all recipients
 mailer.connect()  # Connect to the SMTP server
@@ -54,11 +69,11 @@
 - **set_recipients**: Set the list of email recipients.
 - **add_recipient**: Add a single recipient to the list of recipients.
 - **connect**: Connect to the SMTP server.
 - **disconnect**: Disconnect from the SMTP server.
 - **send_all**: Send the composed email to all recipients.
 
 ## Contribution
-Contributions to pycourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/pycourrier/issues).
+Contributions to PyCourrier are welcome! If you encounter any issues or have suggestions for improvements, please open an [issue on GitHub](https://github.com/mjiid/PyCourrier/issues).
 
 ## License
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `PyCourrier-0.1.2/setup.py` & `PyCourrier-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='PyCourrier',
-    version='0.1.2',
+    version='0.1.3',
     packages=find_packages(),
     description='A simple email sender utility',
     author='Abdelmajid Habouch',
     author_email='Habush1610@gmail.com',
     url='https://github.com/mjiid/PyCourrier',
     license='MIT',
     install_requires=[
```

