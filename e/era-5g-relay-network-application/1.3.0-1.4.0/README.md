# Comparing `tmp/era_5g_relay_network_application-1.3.0.tar.gz` & `tmp/era_5g_relay_network_application-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_relay_network_application-1.3.0.tar", last modified: Tue Mar  5 07:52:00 2024, max compression
+gzip compressed data, was "era_5g_relay_network_application-1.4.0.tar", last modified: Mon Apr 29 08:58:11 2024, max compression
```

## Comparing `era_5g_relay_network_application-1.3.0.tar` & `era_5g_relay_network_application-1.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-03-05 07:52:00.396816 era_5g_relay_network_application-1.3.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      431 2024-03-05 07:52:00.396816 era_5g_relay_network_application-1.3.0/PKG-INFO
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/backend_shim.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-03-05 07:52:00.396816 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      353 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    15859 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/client.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-03-05 07:52:00.396816 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/compatibility/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/compatibility/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2128 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2028 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/compatibility/rosbridge_action_loader.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-03-05 07:52:00.396816 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/data/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/data/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/py.typed
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    18918 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/server.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5643 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/utils.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1402 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_clock.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1374 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_image_publisher.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3319 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_image_subscriber.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5740 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_publisher.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6841 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_service.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4654 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_service_server.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1354 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_socketio.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      868 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_socketio_server.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5962 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_subscriber.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1213 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_tf.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-03-05 07:52:00.396816 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      431 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     1390 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      119 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       33 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/era_5g_relay_network_application.egg-info/top_level.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-03-05 07:52:00.396816 era_5g_relay_network_application-1.3.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1182 2024-03-05 07:52:00.000000 era_5g_relay_network_application-1.3.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      431 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/PKG-INFO
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/backend_shim.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.473980 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      353 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    16864 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/client.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2128 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     2028 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/rosbridge_action_loader.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/data/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/data/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/py.typed
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    19727 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/server.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5643 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/utils.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1402 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_clock.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1374 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_image_publisher.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3401 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_image_subscriber.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     5741 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_publisher.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6841 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_service.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     4654 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_service_server.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1537 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_socketio.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1087 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_socketio_server.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     6609 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_subscriber.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1213 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_tf.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:58:11.473980 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      431 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)     1390 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      150 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       33 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/top_level.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-29 08:58:11.477980 era_5g_relay_network_application-1.4.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1224 2024-04-29 08:58:11.000000 era_5g_relay_network_application-1.4.0/setup.py
```

### Comparing `era_5g_relay_network_application-1.3.0/backend_shim.py` & `era_5g_relay_network_application-1.4.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/client.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import sys
 from functools import partial
 from queue import Full, Queue
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import rclpy  # pants: no-infer-dep
 from cv_bridge import CvBridge  # pants: no-infer-dep
 from rclpy.executors import MultiThreadedExecutor  # pants: no-infer-dep
 from rclpy.node import Node  # pants: no-infer-dep
 from rclpy.parameter import Parameter  # pants: no-infer-dep
 from rclpy.qos import QoSHistoryPolicy, QoSProfile, QoSReliabilityPolicy  # pants: no-infer-dep
@@ -186,15 +186,24 @@
 ):
     """Create services and topics related to a ROS action."""
 
     def create_action_topic(action_topic_variant: ActionTopicVariant):
         """Create action-related topic (i.e. Feedback and Status topics)."""
 
         queue: Queue = Queue(QUEUE_LENGTH_TOPICS)
-        worker = WorkerPublisher(queue, action_name, action_type, node, None, None, action_topic_variant)
+        worker = WorkerPublisher(
+            queue,
+            action_name,
+            action_type,
+            node,
+            None,
+            None,
+            action_topic_variant,
+            extended_measuring=EXTENDED_MEASURING,
+        )
 
         callback = partial(json_callback, queue=queue)
 
         # Topic name is changed by worker in case of action-related topics, so worker.topic_name must be used
         callbacks_info[f"topic/{worker.topic_name}"] = CallbackInfoClient(ChannelType.JSON, callback)
 
         topics_workers[worker.topic_name] = worker
@@ -261,21 +270,37 @@
         channel_type = get_channel_type(topic_in.compression, topic_in.type)
         worker: WorkerPublisher
         if channel_type in IMAGE_CHANNEL_TYPES:
             callback = partial(
                 image_callback,
                 queue=queue,
             )
-            worker = WorkerImagePublisher(queue, topic_in.name, topic_in.type, node, topic_in.compression, topic_in.qos)
+            worker = WorkerImagePublisher(
+                queue,
+                topic_in.name,
+                topic_in.type,
+                node,
+                topic_in.compression,
+                topic_in.qos,
+                extended_measuring=EXTENDED_MEASURING,
+            )
         else:
             callback = partial(
                 json_callback,
                 queue=queue,
             )
-            worker = WorkerPublisher(queue, topic_in.name, topic_in.type, node, topic_in.compression, topic_in.qos)
+            worker = WorkerPublisher(
+                queue,
+                topic_in.name,
+                topic_in.type,
+                node,
+                topic_in.compression,
+                topic_in.qos,
+                extended_measuring=EXTENDED_MEASURING,
+            )
 
         callbacks_info[f"topic/{topic_in.name}"] = CallbackInfoClient(channel_type, callback)
 
         topics_workers[topic_in.name] = worker
         worker.daemon = True
         worker.start()
 
@@ -314,32 +339,48 @@
             worker_clock.daemon = True
             worker_clock.start()
 
         # create socketio workers for all topics and services to be sent to the relay server
         for topic_out in topics_outgoing_list:
             subscriber_queue: Queue = Queue(QUEUE_LENGTH_TOPICS)
             channel_type = get_channel_type(topic_out.compression, topic_out.type)
-
+            w: Union[WorkerImageSubscriber, WorkerSubscriber]
             if channel_type in IMAGE_CHANNEL_TYPES:
-                WorkerImageSubscriber(topic_out.name, topic_out.type, node, subscriber_queue, topic_out.qos)
+                w = WorkerImageSubscriber(
+                    topic_out.name,
+                    topic_out.type,
+                    node,
+                    subscriber_queue,
+                    topic_out.qos,
+                    extended_measuring=EXTENDED_MEASURING,
+                )
                 send_function: SendFunctionProtocol = partial(
                     send_image,
                     event=f"topic/{topic_out.name}",
                     client=client,
                     channel_type=channel_type,
                     can_be_dropped=True,
                 )
             else:
-                WorkerSubscriber(
-                    topic_out.name, topic_out.type, node, subscriber_queue, topic_out.compression, topic_out.qos
+                w = WorkerSubscriber(
+                    topic_out.name,
+                    topic_out.type,
+                    node,
+                    subscriber_queue,
+                    topic_out.compression,
+                    topic_out.qos,
+                    extended_measuring=EXTENDED_MEASURING,
                 )
                 send_function: SendFunctionProtocol = partial(  # type: ignore  # deals with "name already defined"
                     client.send_data, event=f"topic/{topic_out.name}", channel_type=channel_type, can_be_dropped=True
                 )
 
+            if w.memory is not None:
+                for msg in w.memory:
+                    send_function(msg)
             worker_socketio = WorkerSocketIO(subscriber_queue, send_function)
             worker_socketio.daemon = True
             worker_socketio.start()
 
             socketio_workers.append(worker_socketio)
 
         for service_name, service_worker in services_workers.items():
```

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/point_cloud_msg_conv.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/compatibility/rosbridge_action_loader.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/compatibility/rosbridge_action_loader.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/server.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,19 +84,30 @@
         super().__init__(topic_name, topic_type, channel_type, compression, qos)
 
         # this sucks, the classes should have some common ancestor or there should be two properties
         self.worker: Union[WorkerImagePublisher, WorkerPublisher]
 
         if self.channel_type in IMAGE_CHANNEL_TYPES:
             self.worker = WorkerImagePublisher(
-                self.queue, self.topic_name, self.topic_type, compression=compression, node=node
+                self.queue,
+                self.topic_name,
+                self.topic_type,
+                compression=compression,
+                node=node,
+                extended_measuring=EXTENDED_MEASURING,
             )
         else:
             self.worker = WorkerPublisher(
-                self.queue, self.topic_name, self.topic_type, node, self.compression, self.qos
+                self.queue,
+                self.topic_name,
+                self.topic_type,
+                node,
+                self.compression,
+                self.qos,
+                extended_measuring=EXTENDED_MEASURING,
             )
         self.worker.daemon = True
         self.worker.start()
 
 
 class RelayTopicOutgoing(RelayTopic):
     """Class that holds information about outgoing topic (i.e. topic that is subscribed to be sent to the relay client),
@@ -117,18 +128,28 @@
 
         self.action_topic_variant = action_topic_variant
 
         # this sucks, the classes should have some common ancestor or there should be two properties
         self.worker: Union[WorkerImageSubscriber, WorkerSubscriber]
 
         if self.channel_type in IMAGE_CHANNEL_TYPES:
-            self.worker = WorkerImageSubscriber(topic_name, topic_type, node, self.queue)
+            self.worker = WorkerImageSubscriber(
+                topic_name, topic_type, node, self.queue, extended_measuring=EXTENDED_MEASURING
+            )
         else:
             self.worker = WorkerSubscriber(
-                topic_name, topic_type, node, self.queue, compression, qos, action_topic_variant, action_subscribers
+                topic_name,
+                topic_type,
+                node,
+                self.queue,
+                compression,
+                qos,
+                action_topic_variant,
+                action_subscribers,
+                extended_measuring=EXTENDED_MEASURING,
             )
             # Topic name may be changed in case of action-related topics
             self.channel_name = f"topic/{self.worker.topic_name}"
             self.topic_name = self.worker.topic_name
 
 
 class RelayService:
@@ -336,15 +357,20 @@
         """
 
         if command and command.cmd_type == ControlCmdType.INIT:
             args = command.data
             if args:
                 sr = args.get("subscribe_results")
                 if sr:
-                    self.result_subscribers.add(self.get_sid_of_data(self.get_eio_sid_of_control(sid)))
+                    sid = self.get_sid_of_data(self.get_eio_sid_of_control(sid))
+                    self.result_subscribers.add(sid)
+                    for topic_out in self.topics_outgoing.values():
+                        if topic_out.worker.memory is not None:
+                            for msg in topic_out.worker.memory:
+                                self.send_data_with_sid((sid, msg), topic_out.channel_name)
         return True, ""
 
     def disconnect_callback(self, eio_sid):
         """Removes the client from the list of result subscribers."""
         self.result_subscribers.discard(eio_sid)
 
 
@@ -388,15 +414,15 @@
 
 def main(args=None) -> None:
     """Main function that starts the relay server and all workers."""
     topics_outgoing_list = load_entities_list("TOPICS_TO_CLIENT")  # Topics from server that are sent to the client
     topics_incoming_list = load_entities_list("TOPICS_FROM_CLIENT")  # Topics that are received from the client
     services_incoming_list = load_entities_list("SERVICES_FROM_CLIENT")  # Services that are called from the client
     actions_to_provide = load_entities_list("ACTIONS_FROM_CLIENT")  # Actions provided by this server to the client
-    transforms_to_listen = load_transform_list("TRANSFORMS_FROM_CLIENT")  # TFs that are received from the client
+    transforms_to_listen = load_transform_list("TRANSFORMS_TO_CLIENT")  # TFs that should be send to the client
 
     rclpy.init(args=args)
     node = rclpy.create_node("relay_netapp")
     use_sim_time = Parameter("use_sim_time", Parameter.Type.BOOL, USE_SIM_TIME)
     node.set_parameters([use_sim_time])
     node.get_logger().set_level(logging.DEBUG)
     node.get_logger().debug(f"Loaded outgoing topics: {topics_outgoing_list}")
```

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/utils.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/utils.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_clock.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_clock.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_image_publisher.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_image_publisher.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_image_subscriber.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_image_subscriber.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 from queue import Full
-from typing import Any, Optional
+from typing import Any, Deque, Optional
 
 from cv_bridge import CvBridge  # pants: no-infer-dep
 from rclpy.callback_groups import MutuallyExclusiveCallbackGroup  # pants: no-infer-dep
 from rclpy.node import Node  # pants: no-infer-dep
 from rclpy.qos import QoSProfile  # pants: no-infer-dep
 from rclpy.time import Time  # pants: no-infer-dep
 from rosbridge_library.internal import ros_loader  # pants: no-infer-dep
@@ -23,15 +23,15 @@
     def __init__(
         self,
         topic_name: str,
         topic_type: str,
         node: Node,
         queue: AnyQueue,
         qos: Optional[QoSProfile] = None,
-        extended_measuring: bool = True,
+        extended_measuring: bool = False,
         **kw,
     ):
         """Constructor.
 
         Args:
             topic_name (str): The name of the topic to subscribe to.
             topic_type (str): The type of the topic to subscribe to in the string format.
@@ -59,14 +59,15 @@
             callback_group=self._cb_group,
         )
         self.inst = inst
         self.queue = queue
         self.topic_name = topic_name
         self.topic_type = topic_type
         self.bridge = CvBridge()
+        self.memory: Optional[Deque[Any]] = None  # compatibility reasons
 
         self._extended_measuring = extended_measuring
         self._measuring = Measuring(
             measuring_items={
                 "key_timestamp": 0,
                 "before_callback_timestamp": 0,
                 "after_callback_timestamp": 0,
```

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_publisher.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_publisher.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         queue: AnyQueue,
         topic_name: str,
         topic_type: str,
         node: Node,
         compression: Optional[Compressions],
         qos: Optional[QoSProfile] = None,
         action_topic_variant: ActionTopicVariant = ActionTopicVariant.NONE,
-        extended_measuring: bool = True,
+        extended_measuring: bool = False,
         **kw,
     ) -> None:
         """
 
         Args:
             extended_measuring (bool): Enable logging of measuring.
         """
```

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_service.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_service.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_service_server.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_service_server.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_socketio.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_socketio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
 from queue import Empty
 from threading import Event, Thread
 from typing import Any, Optional
 
+from socketio.exceptions import BadNamespaceError
+
 from era_5g_interface.exceptions import BackPressureException
 from era_5g_relay_network_application import AnyQueue, SendFunctionProtocol
 
 
 class WorkerSocketIO(Thread):
     """Worker object for sending data over socket io."""
 
@@ -38,7 +40,9 @@
 
     def send_data(self, data: Any) -> None:
         assert self.send_function is not None
         try:
             self.send_function(data)
         except BackPressureException:
             logging.warning("Backpressure applied.")
+        except BadNamespaceError:
+            logging.warning("Trying to send data while not connected to the network application")
```

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_socketio_server.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_socketio_server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import logging
 from multiprocessing.queues import Queue
 from typing import Any, Optional
 
+from socketio.exceptions import BadNamespaceError
+
 from era_5g_interface.exceptions import BackPressureException
 from era_5g_relay_network_application import SendFunctionProtocol
 from era_5g_relay_network_application.worker_socketio import WorkerSocketIO
 
 
 class WorkerSocketIOServer(WorkerSocketIO):
     """Worker object for sending data to multiple subscribed clients over socket io."""
@@ -16,8 +19,10 @@
     def send_data(self, data: Any):
         assert self.send_function
 
         for s in self.subscribers:
             try:
                 self.send_function(data, sid=s)
             except BackPressureException:
-                print("apply backpressure")
+                logging.warning("Backpressure applied.")
+            except BadNamespaceError:
+                logging.warning("Trying to send data while not connected to the network application")
```

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_subscriber.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_subscriber.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import time
+from collections import deque
 from queue import Full
-from typing import Any, Optional
+from typing import Any, Deque, Optional
 
 import DracoPy
 from rclpy.callback_groups import MutuallyExclusiveCallbackGroup  # pants: no-infer-dep
 from rclpy.node import Node  # pants: no-infer-dep
-from rclpy.qos import QoSProfile  # pants: no-infer-dep
+from rclpy.qos import DurabilityPolicy, HistoryPolicy, QoSProfile  # pants: no-infer-dep
 from rosbridge_library.internal import ros_loader  # pants: no-infer-dep
 from rosbridge_library.internal.message_conversion import extract_values  # pants: no-infer-dep
 from sensor_msgs.msg import PointCloud2  # pants: no-infer-dep
 
 from era_5g_interface.channels import Channels
 from era_5g_interface.measuring import Measuring
 
@@ -42,15 +43,15 @@
         topic_type: str,
         node: Node,
         queue: AnyQueue,
         compression: Optional[Compressions] = None,
         qos: Optional[QoSProfile] = None,
         action_topic_variant: ActionTopicVariant = ActionTopicVariant.NONE,
         action_subscribers: Optional[ActionSubscribers] = None,
-        extended_measuring: bool = True,
+        extended_measuring: bool = False,
         **kw,
     ):
         """Constructor.
 
         Args:
             topic_name (str): The name of the topic for which the subscriber is created.
             topic_type (str): The type of the topic as a string.
@@ -70,14 +71,22 @@
         self.topic_name = topic_name
         self.topic_type = topic_type
         self.compression = compression
         self.node = node
         self.queue = queue
         self.action_topic_variant = action_topic_variant
         self.action_subscribers = action_subscribers
+        self.memory: Optional[Deque[Any]] = None
+        if qos and qos.durability == DurabilityPolicy.TRANSIENT_LOCAL:
+            if qos.history == HistoryPolicy.KEEP_ALL:
+                self.node.get_logger().debug(f"Latched topic {self.topic_name} with infinite depth")
+                self.memory = deque()
+            else:
+                self.node.get_logger().debug(f"Latched topic {self.topic_name} with depth: {qos.depth}")
+                self.memory = deque(maxlen=qos.depth)
 
         # each topic has its own group
         # callbacks for different topics can overlap
         # there will be only one running callback for particular topic
         self._cb_group = MutuallyExclusiveCallbackGroup()
 
         if action_topic_variant == ActionTopicVariant.NONE:
@@ -121,24 +130,24 @@
         msg = extract_values(data)
         timestamp = Channels.get_timestamp_from_data(msg)
 
         if isinstance(data, PointCloud2) and self.compression == Compressions.DRACO:
             np_arr = read_points_numpy(data, field_names=["x", "y", "z"], skip_nans=True)  # drop intensity, etc....
             cpc = DracoPy.encode(np_arr, compression_level=1)
             msg["data"] = cpc
-
         try:
             if self.action_topic_variant == ActionTopicVariant.ACTION_FEEDBACK:
                 # Send action feedback only to the client that sent the corresponding action goal
                 goal_uuid = msg["goal_id"]["uuid"]
                 assert self.action_subscribers is not None  # prevents mypy error
                 sid = self.action_subscribers.get_sid_for_goal_id(goal_uuid)
-
                 self.queue.put_nowait((sid, msg))
             else:
+                if self.memory is not None:
+                    self.memory.append(msg)
                 self.queue.put_nowait(msg)
 
         except Full:
             pass
         self._measuring.log_measuring(timestamp, "before_callback_timestamp", before_callback_timestamp)
         self._measuring.log_timestamp(timestamp, "after_callback_timestamp")
         self._measuring.store_measuring(timestamp)
```

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application/worker_tf.py` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application/worker_tf.py`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/era_5g_relay_network_application.egg-info/SOURCES.txt` & `era_5g_relay_network_application-1.4.0/era_5g_relay_network_application.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `era_5g_relay_network_application-1.3.0/setup.py` & `era_5g_relay_network_application-1.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,19 @@
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
     ],
     'description': 'Relay Network Application',
     'install_requires': (
         'DracoPy>=1.3.0',
         'era-5g-tf2json~=0.2.0',
-        'era_5g_client~=0.11.0',
-        'era_5g_interface~=0.10.0',
+        'era_5g_client~=1.0.0',
+        'era_5g_interface~=0.10.1',
         'era_5g_server~=0.4.0',
         'numpy>=1.24.4',
+        'python-socketio[client]>=5.11.1',
     ),
     'license': 'LGPL',
     'name': 'era_5g_relay_network_application',
     'namespace_packages': (
     ),
     'package_data': {
         'era_5g_relay_network_application': (
@@ -33,9 +34,9 @@
     },
     'packages': (
         'era_5g_relay_network_application',
         'era_5g_relay_network_application.compatibility',
         'era_5g_relay_network_application.data',
     ),
     'python_requires': '>=3.8',
-    'version': '1.3.0',
+    'version': '1.4.0',
 })
```

