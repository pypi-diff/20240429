# Comparing `tmp/passwork-0.1.4.tar.gz` & `tmp/passwork-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwork-0.1.4.tar", last modified: Sun Apr 28 14:42:29 2024, max compression
+gzip compressed data, was "passwork-0.1.5.tar", last modified: Mon Apr 29 19:51:11 2024, max compression
```

## Comparing `passwork-0.1.4.tar` & `passwork-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.700727 passwork-0.1.4/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1065 2024-04-23 15:05:31.000000 passwork-0.1.4/LICENSE
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-28 14:42:29.700672 passwork-0.1.4/PKG-INFO
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     5814 2024-04-23 15:05:31.000000 passwork-0.1.4/README.md
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.696071 passwork-0.1.4/passwork/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       42 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/main.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.697903 passwork-0.1.4/passwork/password_crud/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      219 2024-04-28 14:39:47.000000 passwork-0.1.4/passwork/password_crud/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2908 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/password_crud/add_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      799 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/password_crud/delete_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2121 2024-04-27 14:02:55.000000 passwork-0.1.4/passwork/password_crud/get_inbox_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     2248 2024-04-27 12:13:16.000000 passwork-0.1.4/passwork/password_crud/get_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1658 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/password_crud/search_password.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     8159 2024-04-27 13:34:55.000000 passwork-0.1.4/passwork/passwork_api.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.698899 passwork-0.1.4/passwork/rest_modules/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1056 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/rest_modules/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4646 2024-04-27 12:34:52.000000 passwork-0.1.4/passwork/rest_modules/passwords.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1808 2024-04-27 13:02:05.000000 passwork-0.1.4/passwork/rest_modules/users.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      431 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/rest_modules/vaults.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     1362 2024-04-27 13:22:16.000000 passwork-0.1.4/passwork/session_options.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.700179 passwork-0.1.4/passwork/utils/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      116 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/utils/__init__.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3954 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/utils/base32.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3200 2024-04-23 15:05:31.000000 passwork-0.1.4/passwork/utils/crypto_file.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     4679 2024-04-27 13:36:30.000000 passwork-0.1.4/passwork/utils/crypto_interface.py
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     3552 2024-04-27 12:57:05.000000 passwork-0.1.4/passwork/utils/passwork_utils.py
-drwxr-xr-x   0 timur.anoyatsoev   (501) staff       (20)        0 2024-04-28 14:42:29.700456 passwork-0.1.4/passwork.egg-info/
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)     6227 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/PKG-INFO
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      810 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/SOURCES.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        1 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/dependency_links.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       52 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/requires.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)        9 2024-04-28 14:42:29.000000 passwork-0.1.4/passwork.egg-info/top_level.txt
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)       38 2024-04-28 14:42:29.700941 passwork-0.1.4/setup.cfg
--rw-r--r--   0 timur.anoyatsoev   (501) staff       (20)      638 2024-04-28 14:39:47.000000 passwork-0.1.4/setup.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-29 19:51:11.304890 passwork-0.1.5/
+-rw-r--r--   0 dima       (501) staff       (20)     1065 2024-04-19 21:19:47.000000 passwork-0.1.5/LICENSE
+-rw-r--r--   0 dima       (501) staff       (20)     6130 2024-04-29 19:51:11.304996 passwork-0.1.5/PKG-INFO
+-rw-r--r--   0 dima       (501) staff       (20)     5814 2024-04-23 11:44:31.000000 passwork-0.1.5/README.md
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-29 19:51:11.299487 passwork-0.1.5/passwork/
+-rw-r--r--   0 dima       (501) staff       (20)        0 2024-04-21 12:36:33.000000 passwork-0.1.5/passwork/__init__.py
+-rw-r--r--   0 dima       (501) staff       (20)      330 2024-04-29 19:41:53.000000 passwork-0.1.5/passwork/main.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-29 19:51:11.302176 passwork-0.1.5/passwork/password_crud/
+-rw-r--r--   0 dima       (501) staff       (20)      219 2024-04-28 19:43:15.000000 passwork-0.1.5/passwork/password_crud/__init__.py
+-rw-r--r--   0 dima       (501) staff       (20)     2908 2024-04-23 13:33:55.000000 passwork-0.1.5/passwork/password_crud/add_password.py
+-rw-r--r--   0 dima       (501) staff       (20)      799 2024-04-23 13:17:38.000000 passwork-0.1.5/passwork/password_crud/delete_password.py
+-rw-r--r--   0 dima       (501) staff       (20)     3248 2024-04-29 19:49:45.000000 passwork-0.1.5/passwork/password_crud/get_inbox_password.py
+-rw-r--r--   0 dima       (501) staff       (20)     2248 2024-04-28 19:43:15.000000 passwork-0.1.5/passwork/password_crud/get_password.py
+-rw-r--r--   0 dima       (501) staff       (20)     1658 2024-04-23 13:33:55.000000 passwork-0.1.5/passwork/password_crud/search_password.py
+-rw-r--r--   0 dima       (501) staff       (20)     8263 2024-04-29 19:24:14.000000 passwork-0.1.5/passwork/passwork_api.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-29 19:51:11.303402 passwork-0.1.5/passwork/rest_modules/
+-rw-r--r--   0 dima       (501) staff       (20)     1056 2024-04-19 21:19:47.000000 passwork-0.1.5/passwork/rest_modules/__init__.py
+-rw-r--r--   0 dima       (501) staff       (20)     4646 2024-04-28 19:43:15.000000 passwork-0.1.5/passwork/rest_modules/passwords.py
+-rw-r--r--   0 dima       (501) staff       (20)     1808 2024-04-28 19:43:15.000000 passwork-0.1.5/passwork/rest_modules/users.py
+-rw-r--r--   0 dima       (501) staff       (20)      431 2024-04-22 23:02:06.000000 passwork-0.1.5/passwork/rest_modules/vaults.py
+-rw-r--r--   0 dima       (501) staff       (20)     1362 2024-04-28 19:43:15.000000 passwork-0.1.5/passwork/session_options.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-29 19:51:11.304700 passwork-0.1.5/passwork/utils/
+-rw-r--r--   0 dima       (501) staff       (20)      116 2024-04-19 21:19:47.000000 passwork-0.1.5/passwork/utils/__init__.py
+-rw-r--r--   0 dima       (501) staff       (20)     3954 2024-04-19 21:19:47.000000 passwork-0.1.5/passwork/utils/base32.py
+-rw-r--r--   0 dima       (501) staff       (20)     3203 2024-04-29 19:24:14.000000 passwork-0.1.5/passwork/utils/crypto_file.py
+-rw-r--r--   0 dima       (501) staff       (20)     4679 2024-04-28 19:43:15.000000 passwork-0.1.5/passwork/utils/crypto_interface.py
+-rw-r--r--   0 dima       (501) staff       (20)     3552 2024-04-28 19:43:15.000000 passwork-0.1.5/passwork/utils/passwork_utils.py
+drwxr-xr-x   0 dima       (501) staff       (20)        0 2024-04-29 19:51:11.300409 passwork-0.1.5/passwork.egg-info/
+-rw-r--r--   0 dima       (501) staff       (20)     6130 2024-04-29 19:51:11.000000 passwork-0.1.5/passwork.egg-info/PKG-INFO
+-rw-r--r--   0 dima       (501) staff       (20)      810 2024-04-29 19:51:11.000000 passwork-0.1.5/passwork.egg-info/SOURCES.txt
+-rw-r--r--   0 dima       (501) staff       (20)        1 2024-04-29 19:51:11.000000 passwork-0.1.5/passwork.egg-info/dependency_links.txt
+-rw-r--r--   0 dima       (501) staff       (20)       52 2024-04-29 19:51:11.000000 passwork-0.1.5/passwork.egg-info/requires.txt
+-rw-r--r--   0 dima       (501) staff       (20)        9 2024-04-29 19:51:11.000000 passwork-0.1.5/passwork.egg-info/top_level.txt
+-rw-r--r--   0 dima       (501) staff       (20)       38 2024-04-29 19:51:11.305532 passwork-0.1.5/setup.cfg
+-rw-r--r--   0 dima       (501) staff       (20)      638 2024-04-29 19:50:13.000000 passwork-0.1.5/setup.py
```

### Comparing `passwork-0.1.4/LICENSE` & `passwork-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/PKG-INFO` & `passwork-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: passwork
-Version: 0.1.4
-Summary: Passwork connector
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: cryptography>=42.0.5
-Requires-Dist: loguru>=0.7.2
-
 ## About the API
 Passwork API lets you retrieve, create, update passwords, folders and vaults. It is an easy way how you can integrate Passwork with your infrastructure. Use our Passwork Python Connector to make the integration smoother. The API operates behalf of the user whom API Key is used.
 Check for all available methods in
 [Passwork API Methods](passwork/passwork_api.py)
 
 ## How to install
 ⚠️<b style='color:YELLOW'>WARNING</b> the connector will not work with python version less than <b>3.10</b>
```

### Comparing `passwork-0.1.4/README.md` & `passwork-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: passwork
+Version: 0.1.5
+Summary: Passwork connector
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ## About the API
 Passwork API lets you retrieve, create, update passwords, folders and vaults. It is an easy way how you can integrate Passwork with your infrastructure. Use our Passwork Python Connector to make the integration smoother. The API operates behalf of the user whom API Key is used.
 Check for all available methods in
 [Passwork API Methods](passwork/passwork_api.py)
 
 ## How to install
 ⚠️<b style='color:YELLOW'>WARNING</b> the connector will not work with python version less than <b>3.10</b>
```

### Comparing `passwork-0.1.4/passwork/password_crud/add_password.py` & `passwork-0.1.5/passwork/password_crud/add_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/password_crud/delete_password.py` & `passwork-0.1.5/passwork/password_crud/delete_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/password_crud/get_inbox_password.py` & `passwork-0.1.5/passwork/password_crud/get_inbox_password.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+# import os
 import json
 from loguru import logger
 from passwork.passwork_api import PassworkAPI
 
 
-def get_inbox_password(api: PassworkAPI, inbox_password_id: str, log_pretty_data: bool = True) -> dict:
+def get_inbox_password(
+        api: PassworkAPI,
+        inbox_password_id: str = "",
+        download_attachments_path: str = "",
+        log_pretty_data: bool = True,
+) -> dict | None:
 
     """
     Retrieve inbox password information from Passwork API.
 
     Args:
         api (PassworkAPI): An instance of PassworkAPI class initialized with appropriate credentials.
         inbox_password_id (str): The unique identifier of the password to retrieve.
+        download_attachments_path (str): Path for downloading attachments.
         log_pretty_data (bool): Whether to log the retrieved password information. Defaults to True.
 
     Returns:
         dict: A dictionary containing the retrieved inbox password information.
+        None: if inbox_password_id is not specified.
 
     This function authenticates with the Passwork API, retrieves inbox password details, including associated vault,
     custom fields, attachments, and plaintext value. If specified, it
     logs this information using the logger.
 
     Example usage:
         api = PassworkAPI(credentials)\n
@@ -27,26 +35,46 @@
     Raises:
         ValueError: If inbox_password_id is empty or None.
     """
 
     api.login()
     api.get_user_info()
 
+    # script_path = os.path.dirname(os.path.abspath(__file__))
+    # download_attachments_path = os.path.join(script_path, download_attachments_path)
+
+    if not inbox_password_id:
+        inbox_passwords = api.get_inbox_passwords()
+
+        if not inbox_passwords:
+            logger.error("Inbox passwords not found")
+            raise Exception
+
+        logger.warning("inbox_password_id is not specified, here is information about existing passwords in the inbox:")
+
+        found_inbox_passwords_ids = [inbox_password["id"] for inbox_password in inbox_passwords]
+        logger.success(f"Found inbox password IDs: {', '.join(found_inbox_passwords_ids)}")
+        for numb, inbox_password in enumerate(inbox_passwords):
+            logger.success(f"Found inbox password #{numb + 1}/{len(inbox_passwords)}: {inbox_password}")
+        return
+
     inbox_item = api.get_inbox_password(inbox_password_id)
     inbox_password_item = inbox_item["password"]
     encryption_key = api.get_inbox_encryption_key(inbox_item)
 
     # get inbox password customs
     inbox_password_item["custom"] = api.get_customs(
         password_item=inbox_password_item, password_encryption_key=encryption_key
     )
 
     # download inbox password attachments
     api.get_attachments(
-        password_item=inbox_password_item, password_encryption_key=encryption_key
+        password_item=inbox_password_item,
+        password_encryption_key=encryption_key,
+        download_path=download_attachments_path,
     )
 
     # get inbox password plain text
     password_plain_text = api.get_password_plain_text(
         password_item=inbox_password_item, password_encryption_key=encryption_key
     )
```

### Comparing `passwork-0.1.4/passwork/password_crud/get_password.py` & `passwork-0.1.5/passwork/password_crud/get_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/password_crud/search_password.py` & `passwork-0.1.5/passwork/password_crud/search_password.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/passwork_api.py` & `passwork-0.1.5/passwork/passwork_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,28 +110,30 @@
             password_encryption_key: The encryption key
 
         Returns:
             The decrypted custom fields
         """
         return get_customs(password_item, password_encryption_key, self.session_options)
 
-    def get_attachments(self, password_item: dict, password_encryption_key: str):
+    def get_attachments(self, password_item: dict, password_encryption_key: str, download_path: str):
         """Retrieves and decrypts attachments for a password item
         than saves results into downloaded_attachments folder.
 
         REST Endpoint: GET /passwords/{id}/attachment/{attachmentId}
 
         Args:
             password_item: The item containing encrypted attachments
             password_encryption_key: The encryption key
+            download_path: Path for downloading attachments
         """
         attachments = get_attachments(password_item=password_item, options=self.session_options)
         if not attachments:
             return None
-        [decrypt_and_save_password_attachment(attachment, password_encryption_key) for attachment in attachments]
+        [decrypt_and_save_password_attachment(attachment, password_encryption_key, download_path)
+         for attachment in attachments]
 
     def delete_password(self, password_id: str):
         """Deletes a password by its identifier.
 
         Args:
             password_id: The identifier of the password to be deleted
         """
```

### Comparing `passwork-0.1.4/passwork/rest_modules/__init__.py` & `passwork-0.1.5/passwork/rest_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/rest_modules/passwords.py` & `passwork-0.1.5/passwork/rest_modules/passwords.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/rest_modules/users.py` & `passwork-0.1.5/passwork/rest_modules/users.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/session_options.py` & `passwork-0.1.5/passwork/session_options.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/utils/base32.py` & `passwork-0.1.5/passwork/utils/base32.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/utils/crypto_file.py` & `passwork-0.1.5/passwork/utils/crypto_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,31 +75,30 @@
                 **encrypt_password_attachment(file_buffer, password_encryption_key),
                 "name": name if name else Path(path).stem,
             }
         )
     return result
 
 
-def save_attachment(byte_data_content: bytes, filename: str):
-    download_folder = f"downloaded_attachments"
-    Path(download_folder).mkdir(parents=True, exist_ok=True)
-    download_path = os.path.join(download_folder, filename)
+def save_attachment(byte_data_content: bytes, filename: str, download_path: str):
+    Path(download_path).mkdir(parents=True, exist_ok=True)
+    download_path = os.path.join(download_path, filename)
     with open(download_path, "wb") as file:
         file.write(byte_data_content)
 
     logger.success(f"Decrypted file saved to {download_path}")
 
 
-def decrypt_and_save_password_attachment(attachment: dict, password_encryption_key: str):
+def decrypt_and_save_password_attachment(attachment: dict, password_encryption_key: str, download_path: str):
     if not attachment:
         return None
 
     key = decrypt_aes(attachment["encryptedKey"], password_encryption_key) if password_encryption_key else None
     byte_data = decode_file(attachment["encryptedData"], key)
 
     blob_string = get_string_from_blob(byte_data)
     computed_hash = hashlib.sha256(blob_string.encode()).hexdigest()
 
     if computed_hash != attachment["hash"]:
         raise Exception("Can't decrypt attachment: hashes are not equal")
 
-    save_attachment(byte_data, attachment["name"])
+    save_attachment(byte_data, attachment["name"], download_path)
```

### Comparing `passwork-0.1.4/passwork/utils/crypto_interface.py` & `passwork-0.1.5/passwork/utils/crypto_interface.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork/utils/passwork_utils.py` & `passwork-0.1.5/passwork/utils/passwork_utils.py`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/passwork.egg-info/PKG-INFO` & `passwork-0.1.5/passwork.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: passwork
-Version: 0.1.4
+Version: 0.1.5
 Summary: Passwork connector
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: cryptography>=42.0.5
-Requires-Dist: loguru>=0.7.2
 
 ## About the API
 Passwork API lets you retrieve, create, update passwords, folders and vaults. It is an easy way how you can integrate Passwork with your infrastructure. Use our Passwork Python Connector to make the integration smoother. The API operates behalf of the user whom API Key is used.
 Check for all available methods in
 [Passwork API Methods](passwork/passwork_api.py)
 
 ## How to install
```

### Comparing `passwork-0.1.4/passwork.egg-info/SOURCES.txt` & `passwork-0.1.5/passwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `passwork-0.1.4/setup.py` & `passwork-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='passwork',
-    version='0.1.4',
+    version='0.1.5',
     description='Passwork connector',
     long_description=readme(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'requests>=2.31.0',
         'cryptography>=42.0.5',
```

