# Comparing `tmp/echo_endpoints-0.0.4.tar.gz` & `tmp/echo_endpoints-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echo_endpoints-0.0.4.tar", last modified: Fri Apr 26 07:08:55 2024, max compression
+gzip compressed data, was "echo_endpoints-0.0.5.tar", last modified: Mon Apr 29 06:44:22 2024, max compression
```

## Comparing `echo_endpoints-0.0.4.tar` & `echo_endpoints-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-26 07:08:55.368140 echo_endpoints-0.0.4/
--rw-r--r--   0 jheaminoff   (501) staff       (20)     1066 2024-04-23 05:50:31.000000 echo_endpoints-0.0.4/LICENSE
--rw-r--r--   0 jheaminoff   (501) staff       (20)     1280 2024-04-26 07:08:55.367388 echo_endpoints-0.0.4/PKG-INFO
--rw-r--r--   0 jheaminoff   (501) staff       (20)      890 2024-04-23 06:10:50.000000 echo_endpoints-0.0.4/README.md
--rw-r--r--   0 jheaminoff   (501) staff       (20)      386 2024-04-26 07:08:47.000000 echo_endpoints-0.0.4/pyproject.toml
--rw-r--r--   0 jheaminoff   (501) staff       (20)       38 2024-04-26 07:08:55.368320 echo_endpoints-0.0.4/setup.cfg
-drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-26 07:08:55.356864 echo_endpoints-0.0.4/src/
-drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-26 07:08:55.360132 echo_endpoints-0.0.4/src/echo_endpoints/
--rw-r--r--   0 jheaminoff   (501) staff       (20)       41 2024-04-26 07:07:38.000000 echo_endpoints-0.0.4/src/echo_endpoints/__init__.py
--rw-r--r--   0 jheaminoff   (501) staff       (20)     5552 2024-04-26 07:05:15.000000 echo_endpoints-0.0.4/src/echo_endpoints/echo_endpoints.py
-drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-26 07:08:55.366621 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/
--rw-r--r--   0 jheaminoff   (501) staff       (20)     1280 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/PKG-INFO
--rw-r--r--   0 jheaminoff   (501) staff       (20)      309 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/SOURCES.txt
--rw-r--r--   0 jheaminoff   (501) staff       (20)        1 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/dependency_links.txt
--rw-r--r--   0 jheaminoff   (501) staff       (20)        9 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/requires.txt
--rw-r--r--   0 jheaminoff   (501) staff       (20)       15 2024-04-26 07:08:55.000000 echo_endpoints-0.0.4/src/echo_endpoints.egg-info/top_level.txt
+drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-29 06:44:22.874089 echo_endpoints-0.0.5/
+-rw-r--r--   0 jheaminoff   (501) staff       (20)     1066 2024-04-23 05:50:31.000000 echo_endpoints-0.0.5/LICENSE
+-rw-r--r--   0 jheaminoff   (501) staff       (20)     1280 2024-04-29 06:44:22.873383 echo_endpoints-0.0.5/PKG-INFO
+-rw-r--r--   0 jheaminoff   (501) staff       (20)      890 2024-04-23 06:10:50.000000 echo_endpoints-0.0.5/README.md
+-rw-r--r--   0 jheaminoff   (501) staff       (20)      386 2024-04-29 06:43:53.000000 echo_endpoints-0.0.5/pyproject.toml
+-rw-r--r--   0 jheaminoff   (501) staff       (20)       38 2024-04-29 06:44:22.874229 echo_endpoints-0.0.5/setup.cfg
+drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-29 06:44:22.864712 echo_endpoints-0.0.5/src/
+drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-29 06:44:22.868034 echo_endpoints-0.0.5/src/echo_endpoints/
+-rw-r--r--   0 jheaminoff   (501) staff       (20)       41 2024-04-26 07:07:38.000000 echo_endpoints-0.0.5/src/echo_endpoints/__init__.py
+-rw-r--r--   0 jheaminoff   (501) staff       (20)     5726 2024-04-29 06:43:18.000000 echo_endpoints-0.0.5/src/echo_endpoints/echo_endpoints.py
+drwxr-xr-x   0 jheaminoff   (501) staff       (20)        0 2024-04-29 06:44:22.872543 echo_endpoints-0.0.5/src/echo_endpoints.egg-info/
+-rw-r--r--   0 jheaminoff   (501) staff       (20)     1280 2024-04-29 06:44:22.000000 echo_endpoints-0.0.5/src/echo_endpoints.egg-info/PKG-INFO
+-rw-r--r--   0 jheaminoff   (501) staff       (20)      309 2024-04-29 06:44:22.000000 echo_endpoints-0.0.5/src/echo_endpoints.egg-info/SOURCES.txt
+-rw-r--r--   0 jheaminoff   (501) staff       (20)        1 2024-04-29 06:44:22.000000 echo_endpoints-0.0.5/src/echo_endpoints.egg-info/dependency_links.txt
+-rw-r--r--   0 jheaminoff   (501) staff       (20)        9 2024-04-29 06:44:22.000000 echo_endpoints-0.0.5/src/echo_endpoints.egg-info/requires.txt
+-rw-r--r--   0 jheaminoff   (501) staff       (20)       15 2024-04-29 06:44:22.000000 echo_endpoints-0.0.5/src/echo_endpoints.egg-info/top_level.txt
```

### Comparing `echo_endpoints-0.0.4/LICENSE` & `echo_endpoints-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `echo_endpoints-0.0.4/PKG-INFO` & `echo_endpoints-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echo_endpoints
-Version: 0.0.4
+Version: 0.0.5
 Summary: Requests formatter
 Author-email: JHEAminoff <jheaminoff@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `echo_endpoints-0.0.4/README.md` & `echo_endpoints-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `echo_endpoints-0.0.4/src/echo_endpoints/echo_endpoints.py` & `echo_endpoints-0.0.5/src/echo_endpoints/echo_endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,38 +18,40 @@
 
 # Define the API call function
 def api_call(
     url: str,
     method: str,
     headers: Optional[Dict[str, str]] = None,
     data: Optional[Dict[str, Any]] = None,
+    params: Optional[Dict[str, Any]] = None,
     timeout: int = 10,
 ) -> Optional[requests.Response]:
     """
     Sends a request to a specified URL and logs the response.
 
     Parameters:
     - url (str): The URL to send the request to.
     - method (str): The HTTP method to use (e.g., 'GET', 'POST').
     - headers (Optional[Dict[str, str]]): Optional headers to include in the request.
     - data (Optional[Dict[str, Any]]): Optional JSON payload for the request.
+    - params (Optional[Dict[str, Any]]): Optional URL parameters for the request.
     - timeout (int): The timeout for the request in seconds.
 
     Returns:
     Optional[requests.Response]: The response object from requests if successful, None otherwise.
 
     Raises:
     - requests.exceptions.HTTPError: For HTTP errors.
     - requests.exceptions.ConnectionError: For connection problems.
     - requests.exceptions.Timeout: For timeouts.
     - requests.exceptions.RequestException: For other types of request-related errors.
     """
     try:
         response = requests.request(
-            method, url, headers=headers, json=data, timeout=timeout
+            method, url, headers=headers, json=data, params=params, timeout=timeout
         )
         response.raise_for_status()
         return response
     except requests.exceptions.HTTPError as e:
         return e
     except requests.exceptions.ConnectionError as e:
         return e
@@ -114,14 +116,15 @@
 
 # Define the echo_endpoint function, the main entrypoint
 def echo_endpoint(
     url: str,
     method: str,
     headers: Optional[Dict[str, str]] = None,
     data: Optional[Dict[str, Any]] = None,
+    params: Optional[Dict[str, Any]] = None,
     timeout: int = 10,
     print_full_response: bool = True,
 ):
     """
     Calls the API using the provided parameters and prints the response.
 
     Parameters:
@@ -131,15 +134,15 @@
     - data (Optional[Dict[str, Any]]): Optional JSON payload for the request.
     - timeout (int): The timeout for the request in seconds.
     - print_full_response (bool): Whether to print the full response text or just a snippet.
 
     The function handles making the API call, error handling, and printing the response.
     """
     # Make the API call
-    response = api_call(url, method, headers=headers, data=data, timeout=timeout)
+    response = api_call(url, method, headers, data, params, timeout)
 
     # Check if the response is not None
     if response:
         # Check for errors in the response:
         if isinstance(response, requests.exceptions.RequestException):
             print(f"{ANSIColors.RED}Request failed. Check the error message for details{ANSIColors.RESET}")
             print(f"{ANSIColors.RED}{response}{ANSIColors.RESET}")
```

### Comparing `echo_endpoints-0.0.4/src/echo_endpoints.egg-info/PKG-INFO` & `echo_endpoints-0.0.5/src/echo_endpoints.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echo_endpoints
-Version: 0.0.4
+Version: 0.0.5
 Summary: Requests formatter
 Author-email: JHEAminoff <jheaminoff@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

