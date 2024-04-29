# Comparing `tmp/smtp_proxy-0.1.6.tar.gz` & `tmp/smtp_proxy-0.1.7.tar.gz`

## Comparing `smtp_proxy-0.1.6.tar` & `smtp_proxy-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/CHANGES.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/src/smtp_proxy/__init__.py
--rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/src/smtp_proxy/smtp_proxy.py
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/tests/test_smtp_proxy.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/LICENSE
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/README.md
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/CHANGES.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/src/smtp_proxy/__init__.py
+-rw-r--r--   0        0        0     8405 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/src/smtp_proxy/smtp_proxy.py
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/tests/test_smtp_proxy.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/LICENSE
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/README.md
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 smtp_proxy-0.1.7/PKG-INFO
```

### Comparing `smtp_proxy-0.1.6/src/smtp_proxy/smtp_proxy.py` & `smtp_proxy-0.1.7/src/smtp_proxy/smtp_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
             self.queue.task_done()
 
 
 class SendgridHandler(BaseHandler):
     def getClient(self, **kwargs):
         log.debug(f"called getClient with {kwargs}")
         environKey = os.environ.get("SENDGRID_API_KEY")
-        apiKey = kwargs.get("sendgrid_api_key", environKey)
+        apiKey = kwargs.get("sendgrid_api_key") or environKey
         log.debug(f"API Key: {apiKey}")
 
         for var in [
                 'no_proxy', 'NO_PROXY', 'http_proxy',
                 'HTTP_PROXY', 'https_proxy', 'HTTPS_PROXY']:
             log.debug(f"{var}: {os.environ.get(var)}")
         return SendgridAPI(apiKey)
```

### Comparing `smtp_proxy-0.1.6/tests/test_smtp_proxy.py` & `smtp_proxy-0.1.7/tests/test_smtp_proxy.py`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.6/LICENSE` & `smtp_proxy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `smtp_proxy-0.1.6/pyproject.toml` & `smtp_proxy-0.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "smtp-proxy"
-version = "0.1.6"
+version = "0.1.7"
 description = "SMTP server meant to redirect SMTP requests to a third-party email provider"
 readme = "README.md"
 requires-python = ">=3"
 keywords = ["smtp", "email", "proxy"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `smtp_proxy-0.1.6/PKG-INFO` & `smtp_proxy-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtp-proxy
-Version: 0.1.6
+Version: 0.1.7
 Summary: SMTP server meant to redirect SMTP requests to a third-party email provider
 License-File: LICENSE
 Keywords: email,proxy,smtp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

