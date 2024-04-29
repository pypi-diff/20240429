# Comparing `tmp/websocket_server_lib-0.0.2.tar.gz` & `tmp/websocket_server_lib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "websocket_server_lib-0.0.2.tar", last modified: Wed Apr 24 11:38:45 2024, max compression
+gzip compressed data, was "websocket_server_lib-0.0.3.tar", last modified: Mon Apr 29 20:44:01 2024, max compression
```

## Comparing `websocket_server_lib-0.0.2.tar` & `websocket_server_lib-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rohanjulka   (501) staff       (20)        0 2024-04-24 11:38:45.920232 websocket_server_lib-0.0.2/
--rw-r--r--   0 rohanjulka   (501) staff       (20)    35148 2024-04-24 10:02:14.000000 websocket_server_lib-0.0.2/LICENSE.txt
--rw-r--r--   0 rohanjulka   (501) staff       (20)      385 2024-04-24 11:38:45.920129 websocket_server_lib-0.0.2/PKG-INFO
--rw-r--r--   0 rohanjulka   (501) staff       (20)       61 2024-04-24 10:30:11.000000 websocket_server_lib-0.0.2/README.md
--rw-r--r--   0 rohanjulka   (501) staff       (20)      376 2024-04-24 11:37:41.000000 websocket_server_lib-0.0.2/pyproject.toml
--rw-r--r--   0 rohanjulka   (501) staff       (20)       78 2024-04-24 11:38:45.920545 websocket_server_lib-0.0.2/setup.cfg
--rw-r--r--   0 rohanjulka   (501) staff       (20)      308 2024-04-24 10:35:15.000000 websocket_server_lib-0.0.2/setup.py
-drwxr-xr-x   0 rohanjulka   (501) staff       (20)        0 2024-04-24 11:38:45.919814 websocket_server_lib-0.0.2/websocket_server_lib.egg-info/
--rw-r--r--   0 rohanjulka   (501) staff       (20)      385 2024-04-24 11:38:45.000000 websocket_server_lib-0.0.2/websocket_server_lib.egg-info/PKG-INFO
--rw-r--r--   0 rohanjulka   (501) staff       (20)      276 2024-04-24 11:38:45.000000 websocket_server_lib-0.0.2/websocket_server_lib.egg-info/SOURCES.txt
--rw-r--r--   0 rohanjulka   (501) staff       (20)        1 2024-04-24 11:38:45.000000 websocket_server_lib-0.0.2/websocket_server_lib.egg-info/dependency_links.txt
--rw-r--r--   0 rohanjulka   (501) staff       (20)        3 2024-04-24 11:38:45.000000 websocket_server_lib-0.0.2/websocket_server_lib.egg-info/top_level.txt
-drwxr-xr-x   0 rohanjulka   (501) staff       (20)        0 2024-04-24 11:38:45.919338 websocket_server_lib-0.0.2/ws/
--rw-r--r--   0 rohanjulka   (501) staff       (20)       35 2024-04-24 09:47:37.000000 websocket_server_lib-0.0.2/ws/__init__.py
--rw-r--r--   0 rohanjulka   (501) staff       (20)     4019 2024-04-24 11:34:41.000000 websocket_server_lib-0.0.2/ws/connection.py
--rw-r--r--   0 rohanjulka   (501) staff       (20)     1985 2024-04-24 11:34:47.000000 websocket_server_lib-0.0.2/ws/server.py
+drwxr-xr-x   0 rohanjulka   (501) staff       (20)        0 2024-04-29 20:44:01.951350 websocket_server_lib-0.0.3/
+-rw-r--r--   0 rohanjulka   (501) staff       (20)    35148 2024-04-24 10:02:14.000000 websocket_server_lib-0.0.3/LICENSE.txt
+-rw-r--r--   0 rohanjulka   (501) staff       (20)      385 2024-04-29 20:44:01.951286 websocket_server_lib-0.0.3/PKG-INFO
+-rw-r--r--   0 rohanjulka   (501) staff       (20)       61 2024-04-24 10:30:11.000000 websocket_server_lib-0.0.3/README.md
+-rw-r--r--   0 rohanjulka   (501) staff       (20)      376 2024-04-29 20:43:58.000000 websocket_server_lib-0.0.3/pyproject.toml
+-rw-r--r--   0 rohanjulka   (501) staff       (20)       78 2024-04-29 20:44:01.951561 websocket_server_lib-0.0.3/setup.cfg
+-rw-r--r--   0 rohanjulka   (501) staff       (20)      308 2024-04-24 10:35:15.000000 websocket_server_lib-0.0.3/setup.py
+drwxr-xr-x   0 rohanjulka   (501) staff       (20)        0 2024-04-29 20:44:01.951090 websocket_server_lib-0.0.3/websocket_server_lib.egg-info/
+-rw-r--r--   0 rohanjulka   (501) staff       (20)      385 2024-04-29 20:44:01.000000 websocket_server_lib-0.0.3/websocket_server_lib.egg-info/PKG-INFO
+-rw-r--r--   0 rohanjulka   (501) staff       (20)      276 2024-04-29 20:44:01.000000 websocket_server_lib-0.0.3/websocket_server_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 rohanjulka   (501) staff       (20)        1 2024-04-29 20:44:01.000000 websocket_server_lib-0.0.3/websocket_server_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 rohanjulka   (501) staff       (20)        3 2024-04-29 20:44:01.000000 websocket_server_lib-0.0.3/websocket_server_lib.egg-info/top_level.txt
+drwxr-xr-x   0 rohanjulka   (501) staff       (20)        0 2024-04-29 20:44:01.950811 websocket_server_lib-0.0.3/ws/
+-rw-r--r--   0 rohanjulka   (501) staff       (20)       35 2024-04-24 09:47:37.000000 websocket_server_lib-0.0.3/ws/__init__.py
+-rw-r--r--   0 rohanjulka   (501) staff       (20)     6961 2024-04-29 20:42:56.000000 websocket_server_lib-0.0.3/ws/connection.py
+-rw-r--r--   0 rohanjulka   (501) staff       (20)     2545 2024-04-29 20:40:00.000000 websocket_server_lib-0.0.3/ws/server.py
```

### Comparing `websocket_server_lib-0.0.2/LICENSE.txt` & `websocket_server_lib-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `websocket_server_lib-0.0.2/ws/server.py` & `websocket_server_lib-0.0.3/ws/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import socket
 
 import threading
 from .connection import WebSocketConnection
 
 class WebSocketServer:
+    '''
+        Main Server class which starts a TCP server to Listen to Sockets
+    '''
     def __init__(self, host="localhost", port=8910):
         self.host = host
         self.port = port
         self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.clients = []
         self.message_received_callback = None
         self.client_connected_callback = None
         self.client_closed_callback = None
 
     def start(self):
+        '''
+            Constantly Listen for connections on the specified host and Port 
+            Once the connection is established 
+            Spawn another thread to handle websocket handshake 
+            And listen for websocket frames on that Socket
+        '''
         try:
             self.server_socket.bind((self.host, self.port))
             self.server_socket.listen(10)
             print(f"WebSocket server listening on {self.host}:{self.port}")
             while True:
                 client_socket, addr = self.server_socket.accept()
                 ws_conn = WebSocketConnection(client_socket, addr, self.message_received_callback, self.client_closed_callback)
@@ -27,19 +36,25 @@
                 threading.Thread(target=self.handle_client, args=(ws_conn,), daemon=True).start()
         except KeyboardInterrupt:
             print("Stopping the server")
             self.stop()
 
 
     def stop(self):
+        '''
+            Send Close Frames to all the sockets before stopping the server 
+        '''
         for ws_conn in self.clients:
             ws_conn.close()
         self.server_socket.close()
 
     def handle_client(self, ws_conn):
+        '''
+            Complete WebSocket handshake and Listen for WebSocket Frames
+        '''
         ws_conn.handle_handshake()
         while True:
             try:
                 ws_conn.handle_message()
             except Exception as e:
                 print("Error:", e)
                 ws_conn.close()
```

