# Comparing `tmp/smtp_proxy-0.1.7.tar.gz` & `tmp/smtp_proxy-0.1.8.tar.gz`

## Comparing `smtp_proxy-0.1.7.tar` & `smtp_proxy-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/CHANGES.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/src/smtp_proxy/__init__.py
--rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/src/smtp_proxy/smtp_proxy.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/tests/test_smtp_proxy.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/CHANGES.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/src/smtp_proxy/__init__.py
+-rw-r--r--   0        0        0     9446 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/src/smtp_proxy/smtp_proxy.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/tests/test_smtp_proxy.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.8/PKG-INFO
```

### Comparing `smtp_proxy-0.1.7/src/smtp_proxy/smtp_proxy.py` & `smtp_proxy-0.1.8/src/smtp_proxy/smtp_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import signal
 import os
 
 from aiosmtpd.controller import Controller
 from aiosmtpd.smtp import Envelope
 from async_sendgrid import SendgridAPI
 from sendgrid import SendGridAPIClient
-from sendgrid.helpers.mail import Mail
+from sendgrid.helpers.mail import Attachment, Mail
 
 # from azure.identity import DeviceCodeCredential
 # from msgraph import GraphServiceClient
 # from msgraph.generated.users.item.send_mail.send_mail_post_request_body import (
 #     SendMailPostRequestBody,
 # )
 # from msgraph.generated.models.message import Message
@@ -61,32 +61,49 @@
         msg = email.parser.BytesParser(email.message.EmailMessage).parsebytes(envelope.content)
         log.debug(f"Parsed Message: {vars(msg)}")
 
         payload = msg.get_payload()
 
         plain_text_content = None
         html_content = None
+        attachments = []
 
         if isinstance(payload, str):
             plain_text_content = payload
 
         if isinstance(payload, list):
-            payloads = payload[0].get_payload()
-            for payload in payloads:
-                if payload.get_content_type() == 'text/plain':
-                    plain_text_content = payload.get_payload()
-                elif payload.get_content_type() == 'text/html':
-                    html_content = payload.get_payload()
+            messagesToProcess = [*payload]
+            while messagesToProcess:
+                message = messagesToProcess.pop(0)
+                messagePayload = message.get_payload()
+                if isinstance(messagePayload, list):
+                    messagesToProcess.extend(messagePayload)
+                elif (message.get_content_disposition() or '').lower() in ('attachment', 'inline'):
+                    # Remove any added new line characters
+                    messagePayload = messagePayload.replace('\r', '')
+                    messagePayload = messagePayload.replace('\n', '')
+
+                    attachments.append({
+                        'file_content': messagePayload,
+                        'file_name': message.get_filename(),
+                        'file_type': message.get_content_type(),
+                        'disposition': message.get_content_disposition(),
+                    })
+                elif message.get_content_type() == 'text/plain':
+                    plain_text_content = messagePayload
+                elif message.get_content_type() == 'text/html':
+                    html_content = messagePayload
 
         return {
             "mail_from": envelope.mail_from,
             "rcpt_tos": envelope.rcpt_tos,
             "subject": msg["Subject"],
             "plain_text_content": plain_text_content,
             "html_content": html_content,
+            "attachments": attachments
         }
 
     async def handleQueue(self):
         while True:
             mailArgs = await self.getMailFromQueue()
 
             payload = self.processPayload(mailArgs)
@@ -135,14 +152,18 @@
         sg_msg = Mail(
             from_email=mailArgs["mail_from"],
             to_emails=mailArgs["rcpt_tos"],
             subject=mailArgs["subject"],
             plain_text_content=mailArgs["plain_text_content"],
             html_content=mailArgs["html_content"],
         )
+        for attachment in mailArgs['attachments']:
+            sg_msg.add_attachment(Attachment(
+                **attachment,
+            ))
         log.debug("Payload proceessed as: " + str(sg_msg))
         return sg_msg
 
     async def sendMail(self, payload):
         return await self.client.send(payload)
```

### Comparing `smtp_proxy-0.1.7/tests/test_smtp_proxy.py` & `smtp_proxy-0.1.8/tests/test_smtp_proxy.py`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.7/LICENSE` & `smtp_proxy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.7/pyproject.toml` & `smtp_proxy-0.1.8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smtp-proxy"
-version = "0.1.7"
+version = "0.1.8"
 description = "SMTP server meant to redirect SMTP requests to a third-party email provider"
 readme = "README.md"
 requires-python = ">=3"
 keywords = ["smtp", "email", "proxy"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `smtp_proxy-0.1.7/PKG-INFO` & `smtp_proxy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtp-proxy
-Version: 0.1.7
+Version: 0.1.8
 Summary: SMTP server meant to redirect SMTP requests to a third-party email provider
 License-File: LICENSE
 Keywords: email,proxy,smtp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

