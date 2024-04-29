# Comparing `tmp/smtp_proxy-0.1.3.tar.gz` & `tmp/smtp_proxy-0.1.4.tar.gz`

## Comparing `smtp_proxy-0.1.3.tar` & `smtp_proxy-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/CHANGES.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/src/smtp_proxy/__init__.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/src/smtp_proxy/smtp_proxy.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/tests/test_smtp_proxy.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/CHANGES.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/src/smtp_proxy/__init__.py
+-rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/src/smtp_proxy/smtp_proxy.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/tests/test_smtp_proxy.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.4/PKG-INFO
```

### Comparing `smtp_proxy-0.1.3/src/smtp_proxy/smtp_proxy.py` & `smtp_proxy-0.1.4/src/smtp_proxy/smtp_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,19 +57,36 @@
     async def getMailFromQueue(self):
         log.debug("Waiting on Queue...")
         envelope = await self.queue.get()
         log.debug(f"Received envelope: {vars(envelope)}")
         msg = email.parser.BytesParser(email.message.EmailMessage).parsebytes(envelope.content)
         log.debug(f"Parsed Message: {vars(msg)}")
 
+        payload = msg.get_payload()
+
+        plain_text_content = None
+        html_content = None
+
+        if isinstance(payload, str):
+            plain_text_content = payload
+
+        if isinstance(payload, list):
+            payloads = payload[0].get_payload()
+            for payload in payloads:
+                if payload.get_content_type() == 'text/plain':
+                    plain_text_content = payload.get_payload()
+                elif payload.get_content_type() == 'text/html':
+                    html_content = payload.get_payload()
+
         return {
             "mail_from": envelope.mail_from,
             "rcpt_tos": envelope.rcpt_tos,
             "subject": msg["Subject"],
-            "body": msg.get_payload(),
+            "plain_text_content": plain_text_content,
+            "html_content": html_content,
         }
 
     async def handleQueue(self):
         while True:
             mailArgs = await self.getMailFromQueue()
 
             payload = self.processPayload(mailArgs)
@@ -106,15 +123,16 @@
 
     def processPayload(self, mailArgs):
         log.debug("Processing Payload for:" + str(mailArgs))
         sg_msg = Mail(
             from_email=mailArgs["mail_from"],
             to_emails=mailArgs["rcpt_tos"],
             subject=mailArgs["subject"],
-            html_content=mailArgs["body"],
+            plain_text_content=mailArgs["plain_text_content"],
+            html_content=mailArgs["html_content"],
         )
         log.debug("Payload proceessed as: " + str(sg_msg))
         return sg_msg
 
     async def sendMail(self, payload):
         return await self.client.send(payload)
```

### Comparing `smtp_proxy-0.1.3/tests/test_smtp_proxy.py` & `smtp_proxy-0.1.4/tests/test_smtp_proxy.py`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.3/LICENSE` & `smtp_proxy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.3/pyproject.toml` & `smtp_proxy-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smtp-proxy"
-version = "0.1.3"
+version = "0.1.4"
 description = "SMTP server meant to redirect SMTP requests to a third-party email provider"
 readme = "README.md"
 requires-python = ">=3"
 keywords = ["smtp", "email", "proxy"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `smtp_proxy-0.1.3/PKG-INFO` & `smtp_proxy-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtp-proxy
-Version: 0.1.3
+Version: 0.1.4
 Summary: SMTP server meant to redirect SMTP requests to a third-party email provider
 License-File: LICENSE
 Keywords: email,proxy,smtp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

