# Comparing `tmp/pipelinepy-1.0.4.tar.gz` & `tmp/pipelinepy-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinepy-1.0.4.tar", max compression
+gzip compressed data, was "pipelinepy-1.0.5.tar", max compression
```

## Comparing `pipelinepy-1.0.4.tar` & `pipelinepy-1.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3262 2024-04-26 16:19:30.715659 pipelinepy-1.0.4/README.md
--rw-r--r--   0        0        0     1734 2024-04-26 16:03:08.953663 pipelinepy-1.0.4/pipelinepy/ImsTokenProvider.py
--rw-r--r--   0        0        0      108 2024-04-26 16:03:08.950496 pipelinepy-1.0.4/pipelinepy/__init__.py
--rw-r--r--   0        0        0      475 2024-04-26 16:24:22.156946 pipelinepy-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 pipelinepy-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3426 2024-04-29 07:18:32.226114 pipelinepy-1.0.5/README.md
+-rw-r--r--   0        0        0     1734 2024-04-26 16:03:08.953663 pipelinepy-1.0.5/pipelinepy/ImsTokenProvider.py
+-rw-r--r--   0        0        0      108 2024-04-26 16:03:08.950496 pipelinepy-1.0.5/pipelinepy/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-29 07:18:32.241572 pipelinepy-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4238 1970-01-01 00:00:00.000000 pipelinepy-1.0.5/PKG-INFO
```

### Comparing `pipelinepy-1.0.4/README.md` & `pipelinepy-1.0.5/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # pipelinepy
 
-This is a Python client callback for the Adobe Pipeline Kafka. It is designed to provide a 
-simple and straightforward interface for authenticating IMS users into Kafka.
+This is an OAuth Python client callback for the kafka-python-ng client implementation. It is designed to provide a 
+simple and straightforward interface for authenticating Adobe IMS (Identity Management System) users into Kafka.
 
 ## Installation
 
-To install the pipelinepy, you can use pip:
+Install pipelinepy using pip:
 
 ```bash
 pip install pipelinepy
 ```
 
 ## Usage
 
-To use the pipelinepy, you need to import the specified requirements. 
-You can then create a Kafka producer and consumer, and use them to send and receive messages to/ from a Kafka topic.
+Pipelinepy is designed to be used with the kafka-python-ng client implementation. 
+To use it, you need to create an instance of the `ImsTokenProvider` class and pass it to 
+the `sasl_oauth_token_provider` parameter of the Kafka producer and consumer.
 
 ```bash
-pip install -r requirements.txt
+pip install kafka-python-ng pipelinepy
 ```
 
 ```python
 #!/usr/bin/env python
 import threading, time
 
 from kafka import KafkaConsumer, KafkaProducer
@@ -104,15 +105,15 @@
 
 ```
 
 ## Environment Variables
 
 The following environment variables need to be set:
 
-- `IMS_URL`: The URL of the IMS service.
+- `IMS_URL`: The base URL of the IMS service (does not include the '/ims/token/v1' part).
 - `IMS_CLIENT_ID`: The client ID for the IMS service.
 - `IMS_CLIENT_SECRET`: The client secret for the IMS service.
 - `IMS_CLIENT_CODE`: The client code for the IMS service.
 
 ## Contributing
 
 Contributions are welcome. Please submit a pull request or create an issue to discuss the changes you want to make.
```

### Comparing `pipelinepy-1.0.4/pipelinepy/ImsTokenProvider.py` & `pipelinepy-1.0.5/pipelinepy/ImsTokenProvider.py`

 * *Files identical despite different names*

### Comparing `pipelinepy-1.0.4/PKG-INFO` & `pipelinepy-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pipelinepy
-Version: 1.0.4
-Summary: An Adobe IMS authorization code flow used with the Kafka client for Python (kafka-python-ng).
+Version: 1.0.5
+Summary: An Adobe IMS authorization code flow used with the OAuth Kafka client for Python (kafka-python-ng).
 Home-page: https://github.com/cristianpetrache/pipelinepy
 Author: Petrut Petrache
 Author-email: cpetrache@adobe.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,32 +15,33 @@
 Requires-Dist: kafka-python-ng (>=2.2.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/cristianpetrache/pipelinepy
 Description-Content-Type: text/markdown
 
 # pipelinepy
 
-This is a Python client callback for the Adobe Pipeline Kafka. It is designed to provide a 
-simple and straightforward interface for authenticating IMS users into Kafka.
+This is an OAuth Python client callback for the kafka-python-ng client implementation. It is designed to provide a 
+simple and straightforward interface for authenticating Adobe IMS (Identity Management System) users into Kafka.
 
 ## Installation
 
-To install the pipelinepy, you can use pip:
+Install pipelinepy using pip:
 
 ```bash
 pip install pipelinepy
 ```
 
 ## Usage
 
-To use the pipelinepy, you need to import the specified requirements. 
-You can then create a Kafka producer and consumer, and use them to send and receive messages to/ from a Kafka topic.
+Pipelinepy is designed to be used with the kafka-python-ng client implementation. 
+To use it, you need to create an instance of the `ImsTokenProvider` class and pass it to 
+the `sasl_oauth_token_provider` parameter of the Kafka producer and consumer.
 
 ```bash
-pip install -r requirements.txt
+pip install kafka-python-ng pipelinepy
 ```
 
 ```python
 #!/usr/bin/env python
 import threading, time
 
 from kafka import KafkaConsumer, KafkaProducer
@@ -123,15 +124,15 @@
 
 ```
 
 ## Environment Variables
 
 The following environment variables need to be set:
 
-- `IMS_URL`: The URL of the IMS service.
+- `IMS_URL`: The base URL of the IMS service (does not include the '/ims/token/v1' part).
 - `IMS_CLIENT_ID`: The client ID for the IMS service.
 - `IMS_CLIENT_SECRET`: The client secret for the IMS service.
 - `IMS_CLIENT_CODE`: The client code for the IMS service.
 
 ## Contributing
 
 Contributions are welcome. Please submit a pull request or create an issue to discuss the changes you want to make.
```

