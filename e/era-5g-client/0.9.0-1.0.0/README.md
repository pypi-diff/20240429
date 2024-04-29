# Comparing `tmp/era_5g_client-0.9.0.tar.gz` & `tmp/era_5g_client-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "era_5g_client-0.9.0.tar", last modified: Mon Dec 18 07:22:05 2023, max compression
+gzip compressed data, was "era_5g_client-1.0.0.tar", last modified: Mon Apr 29 08:03:41 2024, max compression
```

## Comparing `era_5g_client-0.9.0.tar` & `era_5g_client-1.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-18 07:22:05.229623 era_5g_client-0.9.0/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/MANIFEST.in
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2023-12-18 07:22:05.225623 era_5g_client-0.9.0/PKG-INFO
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/backend_shim.py
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-18 07:22:05.221623 era_5g_client-0.9.0/era_5g_client/
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/era_5g_client/__init__.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    13812 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/era_5g_client/client.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    13022 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/era_5g_client/client_base.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      559 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/era_5g_client/dataclasses.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      940 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/era_5g_client/exceptions.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3584 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/era_5g_client/middleware_resource_checker.py
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/era_5g_client/py.typed
-drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2023-12-18 07:22:05.225623 era_5g_client-0.9.0/era_5g_client.egg-info/
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2023-12-18 07:22:05.000000 era_5g_client-0.9.0/era_5g_client.egg-info/PKG-INFO
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      470 2023-12-18 07:22:05.000000 era_5g_client-0.9.0/era_5g_client.egg-info/SOURCES.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2023-12-18 07:22:05.000000 era_5g_client-0.9.0/era_5g_client.egg-info/dependency_links.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2023-12-18 07:22:05.000000 era_5g_client-0.9.0/era_5g_client.egg-info/namespace_packages.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      133 2023-12-18 07:22:05.000000 era_5g_client-0.9.0/era_5g_client.egg-info/requires.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       14 2023-12-18 07:22:05.000000 era_5g_client-0.9.0/era_5g_client.egg-info/top_level.txt
--rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2023-12-18 07:22:05.229623 era_5g_client-0.9.0/setup.cfg
--rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1028 2023-12-18 07:22:03.000000 era_5g_client-0.9.0/setup.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:41.008369 era_5g_client-1.0.0/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)       12 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/MANIFEST.in
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-04-29 08:03:41.008369 era_5g_client-1.0.0/PKG-INFO
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      762 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/backend_shim.py
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:41.004369 era_5g_client-1.0.0/era_5g_client/
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/__init__.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    14764 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/client.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)    13441 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/client_base.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      559 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/dataclasses.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)      784 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/exceptions.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     3748 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/middleware_resource_checker.py
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/era_5g_client/py.typed
+drwxrwxr-x   0 zdenekm   (1000) zdenekm   (1000)        0 2024-04-29 08:03:41.004369 era_5g_client-1.0.0/era_5g_client.egg-info/
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      427 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/PKG-INFO
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      470 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)        1 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/namespace_packages.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)      134 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/requires.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       14 2024-04-29 08:03:41.000000 era_5g_client-1.0.0/era_5g_client.egg-info/top_level.txt
+-rw-rw-r--   0 zdenekm   (1000) zdenekm   (1000)       38 2024-04-29 08:03:41.008369 era_5g_client-1.0.0/setup.cfg
+-rw-r--r--   0 zdenekm   (1000) zdenekm   (1000)     1029 2024-04-29 08:03:40.000000 era_5g_client-1.0.0/setup.py
```

### Comparing `era_5g_client-0.9.0/backend_shim.py` & `era_5g_client-1.0.0/backend_shim.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.9.0/era_5g_client/client.py` & `era_5g_client-1.0.0/era_5g_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any, Callable, Dict, Optional
 
 import requests
 from requests import HTTPError
 
 from era_5g_client.client_base import NetAppClientBase
 from era_5g_client.dataclasses import MiddlewareInfo
-from era_5g_client.exceptions import FailedToConnect, FailedToDeleteResource, FailedToObtainPlan, NetAppNotReady
+from era_5g_client.exceptions import FailedToConnect, FailedToDeleteResource, NetAppNotReady
 from era_5g_client.middleware_resource_checker import MiddlewareResourceChecker
 from era_5g_interface.channels import CallbackInfoClient
 
 
 class RunTaskMode(Enum):
     """Run task mode."""
 
@@ -33,16 +33,17 @@
         self,
         callbacks_info=Dict[str, CallbackInfoClient],
         command_result_callback: Optional[Callable] = None,
         command_error_callback: Optional[Callable] = None,
         logging_level: int = logging.INFO,
         socketio_debug: bool = False,
         stats: bool = False,
+        extended_measuring: bool = False,
         back_pressure_size: int = 5,
-        recreate_h264_attempts_count: int = 5,
+        recreate_coder_attempts_count: int = 5,
         reconnection_attempts: int = 3,
         disconnect_on_unhandled: bool = True,
     ) -> None:
         """Constructor.
 
         Args:
             callbacks_info (Dict[str, CallbackInfoClient]): Callbacks Info dictionary, key is custom event name.
@@ -50,38 +51,42 @@
             command_result_callback (Callable, optional): Callback for receiving data that are sent as a result of
                 performing a control command (e.g. 5G-ERA Network Application state obtained by get-state command).
             command_error_callback (Callable, optional): Callback which is emitted when server failed to process the
                 incoming control command.
             logging_level (int): Logging level.
             socketio_debug (bool): Socket.IO debug flag.
             stats (bool): Store output data sizes.
+            extended_measuring (bool): Enable logging of measuring.
             back_pressure_size (int): Back pressure size - max size of eio.queue.qsize().
-            recreate_h264_attempts_count (int): How many times try to recreate the H.264 encoder/decoder.
+            recreate_coder_attempts_count (int): How many times try to recreate the frame encoder/decoder.
             reconnection_attempts (int): How many times to try to reconnect if the connection to the server is lost.
             disconnect_on_unhandled (bool): Whether to call self.disconnect() if unhandled exception occurs.
         """
 
         super().__init__(
-            callbacks_info,
-            command_result_callback,
-            command_error_callback,
-            logging_level,
-            socketio_debug,
-            stats,
-            back_pressure_size,
-            recreate_h264_attempts_count,
-            reconnection_attempts,
-            disconnect_on_unhandled,
+            callbacks_info=callbacks_info,
+            command_result_callback=command_result_callback,
+            command_error_callback=command_error_callback,
+            logging_level=logging_level,
+            socketio_debug=socketio_debug,
+            stats=stats,
+            extended_measuring=extended_measuring,
+            back_pressure_size=back_pressure_size,
+            recreate_coder_attempts_count=recreate_coder_attempts_count,
+            reconnection_attempts=reconnection_attempts,
+            disconnect_on_unhandled=disconnect_on_unhandled,
         )
 
         self.host: Optional[str] = None
         self.action_plan_id: Optional[str] = None
         self.resource_checker: Optional[MiddlewareResourceChecker] = None
         self.middleware_info: Optional[MiddlewareInfo] = None
         self.token: Optional[str] = None
+        self.args: Optional[Dict[str, Any]] = None
+        self._switching: bool = False
 
     def connect_to_middleware(self, middleware_info: MiddlewareInfo) -> None:
         """Authenticates with the Middleware and obtains a token for future calls.
 
         Args:
             middleware_info (MiddlewareInfo): Middleware info, i.e. dataclass with address, user's id and password.
 
@@ -114,30 +119,30 @@
             robot_id (str): The GUID of the robot that deploys the 5G-ERA Network Application.
             resource_lock (bool): TBA.
             mode (RunTaskMode): Specify the mode in which the run_task works.
             args (Dict[str, Any], optional): 5G-ERA Network Application specific arguments. Applied only if register
                 is True. Defaults to None.
 
         Raises:
-            FailedToObtainPlan: Raised when could not get the plan.
             FailedToConnect: Raised when running the task failed.
         """
 
         assert self.middleware_info
         try:
             self.action_plan_id = self.gateway_get_plan(
                 task_id, resource_lock, robot_id
             )  # Get the plan_id by sending the token and task_id.
             if not self.action_plan_id:
-                raise FailedToObtainPlan("Failed to obtain action plan id...")
+                raise FailedToConnect("Failed to obtain action plan id...")
 
             self.resource_checker = MiddlewareResourceChecker(
                 str(self.token),
                 self.action_plan_id,
                 self.middleware_info.build_api_endpoint("orchestrate/orchestrate/plan"),
+                self.netapp_address_changed,
                 daemon=True,
             )
 
             self.resource_checker.start()
             if mode in [RunTaskMode.WAIT, RunTaskMode.WAIT_AND_REGISTER]:
                 self.wait_until_netapp_ready()
                 self.load_netapp_address()
@@ -174,24 +179,39 @@
         """
 
         if not self.resource_checker:
             raise NetAppNotReady("Not connected to the Middleware.")
 
         if not self.resource_checker.is_ready():
             raise NetAppNotReady("Not ready.")
-
+        self.args = args
         super().register(netapp_address, args, wait_until_available, wait_timeout)
 
+    @property
+    def switching(self) -> bool:
+        """Specify if the client is in the process of the edge switchover (reconnecting from one server to another)."""
+        return self._switching
+
+    def netapp_address_changed(self):
+        """Invoked when the resource checker detects a change in the address of the network application."""
+        self._switching = True
+        self.resource_checker.wait_until_resource_ready()
+        self.load_netapp_address()
+        self.disconnect()
+        self.register(self.netapp_address, self.args, True)
+        self._switching = False
+
     def disconnect(self) -> None:
         """Disconnects the WebSocket connection, stop resource checker and delete resources."""
 
         super().disconnect()
-        if self.resource_checker is not None:
-            self.resource_checker.stop()
-        self.delete_all_resources()
+        if not self._switching:
+            if self.resource_checker is not None:
+                self.resource_checker.stop()
+            self.delete_all_resources()
 
     def wait_until_netapp_ready(self) -> None:
         """Blocking wait until the 5G-ERA Network Application is running.
 
         Raises:
             FailedToConnect: Raised when resource_checker si None.
         """
@@ -263,37 +283,36 @@
             Action plan ID.
         Raises:
             FailedToConnect: Raised when could not get the plan.
         """
 
         assert self.middleware_info
         # Request plan.
-        try:
-            self.logger.debug("Goal task is: " + str(taskid))
-            hed = {"Authorization": f"Bearer {str(self.token)}"}
-            data = {
-                "TaskId": str(taskid),
-                "LockResourceReUse": resource_lock,
-                "RobotId": robot_id,
-            }
-            r = requests.post(self.middleware_info.build_api_endpoint("Task/Plan"), json=data, headers=hed)
-            response = r.json()
+        self.logger.debug("Goal task is: " + str(taskid))
+        hed = {"Authorization": f"Bearer {str(self.token)}"}
+        data = {
+            "TaskId": str(taskid),
+            "DisableResourceReuse": resource_lock,
+            "RobotId": robot_id,
+        }
+        r = requests.post(self.middleware_info.build_api_endpoint("Task/Plan"), json=data, headers=hed)
+        response = r.json()
 
-            if not isinstance(response, Dict):
-                raise FailedToConnect("Invalid response.")
+        if not isinstance(response, dict):
+            raise FailedToConnect("Invalid response.")
 
-            if "statusCode" in response and (response["statusCode"] == 500 or response["statusCode"] == 400):
-                raise FailedToConnect(f"response {response['statusCode']}: {response['message']}")
-            # TODO: if "errors" in response:
-            #           raise FailedToConnect(str(response["errors"]))
+        if "statusCode" in response and (response["statusCode"] == 500 or response["statusCode"] == 400):
+            raise FailedToConnect(f"response {response['statusCode']}: {response['message']}")
+
+        try:
             action_plan_id = str(response["ActionPlanId"])
             self.logger.debug("ActionPlanId ** is: " + str(action_plan_id))
             return action_plan_id
         except KeyError as e:
-            raise FailedToObtainPlan(f"Could not get the plan: {e}")
+            raise FailedToConnect(f"Could not get the plan: {e}")
 
     def delete_all_resources(self) -> None:
         """Delete all resources.
 
         Returns:
             None
 
@@ -310,16 +329,17 @@
                 url = self.middleware_info.build_api_endpoint(
                     f"orchestrate/orchestrate/plan/{str(self.action_plan_id)}"
                 )
                 response = requests.delete(url, headers=hed)
 
                 if response.ok:
                     self.logger.debug("Resource deleted")
+                    self.action_plan_id = None
                 else:
-                    self.logger.warning(f"Resource deletion response: {response}")
+                    self.logger.warning(f"Resource deletion response: {response}, {response.text}")
         except HTTPError as e:
             if e.response:
                 self.logger.debug(e.response.status_code)
             else:
                 self.logger.debug(e)
             raise FailedToDeleteResource(
                 f"Error, could not delete the resource, revisit the log files for more details. {e}"
```

### Comparing `era_5g_client-0.9.0/era_5g_client/client_base.py` & `era_5g_client-1.0.0/era_5g_client/client_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import logging
+import os
 import statistics
 import time
 from collections.abc import Callable
 from dataclasses import asdict
 from typing import Any, Dict, Optional, Tuple, Union
 
 import socketio
 import ujson
 from socketio.exceptions import ConnectionError
 
-from era_5g_client.exceptions import FailedToConnect, FailedToInitialize
+from era_5g_client.exceptions import FailedToConnect
 from era_5g_interface.channels import (
     COMMAND_ERROR_EVENT,
     COMMAND_EVENT,
     COMMAND_RESULT_EVENT,
     CONTROL_NAMESPACE,
     DATA_NAMESPACE,
     CallbackInfoClient,
@@ -44,16 +45,17 @@
         self,
         callbacks_info=Dict[str, CallbackInfoClient],
         command_result_callback: Optional[Callable] = None,
         command_error_callback: Optional[Callable] = None,
         logging_level: int = logging.INFO,
         socketio_debug: bool = False,
         stats: bool = False,
+        extended_measuring: bool = False,
         back_pressure_size: Optional[int] = 5,
-        recreate_h264_attempts_count: int = 5,
+        recreate_coder_attempts_count: int = 5,
         reconnection_attempts: int = 3,
         disconnect_on_unhandled: bool = True,
     ) -> None:
         """Constructor.
 
         Args:
             callbacks_info (Dict[str, CallbackInfoClient]): Callbacks Info dictionary, key is custom event name.
@@ -61,16 +63,17 @@
             command_result_callback (Callable, optional): Callback for receiving data that are sent as a result of
                 performing a control command (e.g. 5G-ERA Network Application state obtained by get-state command).
             command_error_callback (Callable, optional): Callback which is emitted when server failed to process the
                 incoming control command.
             logging_level (int): Logging level.
             socketio_debug (bool): Socket.IO debug flag.
             stats (bool): Store output data sizes.
+            extended_measuring (bool): Enable logging of measuring.
             back_pressure_size (int, optional): Back pressure size - max size of eio.queue.qsize().
-            recreate_h264_attempts_count (int): How many times try to recreate the H.264 encoder/decoder.
+            recreate_coder_attempts_count (int): How many times try to recreate the frame encoder/decoder.
             reconnection_attempts (int): How many times to try to reconnect if the connection to the server is lost.
             disconnect_on_unhandled (bool): Whether to call self.disconnect() if unhandled exception occurs.
         """
 
         # Create Socket.IO Client.
         self._sio = socketio.Client(
             logger=socketio_debug, reconnection_attempts=reconnection_attempts, handle_sigint=False, json=ujson
@@ -93,16 +96,17 @@
         # Create channels - custom callbacks and send functions including encoding.
         # NOTE: DATA_NAMESPACE is assumed to be or will be a connected namespace.
         self._channels = ClientChannels(
             self._sio,
             callbacks_info=callbacks_info,
             disconnect_callback=self.disconnect if disconnect_on_unhandled else None,
             back_pressure_size=back_pressure_size,
-            recreate_h264_attempts_count=recreate_h264_attempts_count,
+            recreate_coder_attempts_count=recreate_coder_attempts_count,
             stats=stats,
+            extended_measuring=extended_measuring,
         )
 
         # Save custom command callbacks.
         self._command_result_callback = command_result_callback
         self._command_error_callback = command_error_callback
 
         # Set logger.
@@ -136,15 +140,14 @@
             wait_until_available: If True, the client will repeatedly try to register with the Network Application
                 until it is available. Defaults to False.
             wait_timeout: How long the client will try to connect to network application. Only used if
                 wait_until_available is True. If negative, the client will wait indefinitely. Defaults to -1.
 
         Raises:
             FailedToConnect: Failed to connect to network application exception.
-            FailedToInitialize: Failed to initialize the network application.
 
         Returns:
             Response: response from the 5G-ERA Network Application.
         """
 
         # Store args for repeat registration.
         self._args = args
@@ -171,23 +174,27 @@
         self.logger.info(f"Client connected to namespaces: {namespaces_to_connect}")
 
     def disconnect(self) -> None:
         """Disconnects the WebSocket connection."""
 
         if self._sio.connected:
             self._sio.disconnect()
+
+    def print_stats(self):
+        """Print stats info - transferred bytes."""
+
         if self._channels.stats:
-            # Print stats info - transferred bytes.
-            self.logger.info(
-                f"Transferred bytes sum: {sum(self._channels.sizes)} "
-                f"median: {statistics.median(self._channels.sizes)} "
-                f"mean: {statistics.mean(self._channels.sizes)} "
-                f"min: {min(self._channels.sizes)} "
-                f"max: {max(self._channels.sizes)} "
-            )
+            if len(self._channels.sizes) > 0:
+                self.logger.info(
+                    f"Transferred bytes sum: {sum(self._channels.sizes)} "
+                    f"median: {statistics.median(self._channels.sizes):.3f} "
+                    f"mean: {statistics.mean(self._channels.sizes):.3f} "
+                    f"min: {min(self._channels.sizes)} "
+                    f"max: {max(self._channels.sizes)} "
+                )
 
     def wait(self) -> None:
         """Blocking infinite waiting."""
 
         self._sio.wait()
 
     def data_connect_callback(self) -> None:
@@ -206,15 +213,19 @@
         )
 
         # Initialize the network application with desired parameters using the init command.
         control_command = ControlCommand(ControlCmdType.INIT, clear_queue=False, data=self._args)
         self.logger.info(f"Initialize the network application using the init command {control_command}")
         initialized, message = self.send_control_command(control_command)
         if not initialized:
-            raise FailedToInitialize(f"Failed to initialize the network application: {message}")
+            self.disconnect()
+            self.logger.error(f"Failed to initialize the network application: {message}")
+            logging.shutdown()  # should flush the logger
+            os._exit(1)
+            # raise FailedToInitialize(f"Failed to initialize the network application: {message}")
 
     def data_disconnect_callback(self) -> None:
         """The callback called once the connection to the 5G-ERA Network Application DATA_NAMESPACE is lost."""
 
         self.logger.info(
             f"Disconnected from server {DATA_NAMESPACE}, eio_sid "
             f"{self._channels.get_client_eio_sid(DATA_NAMESPACE)}"
@@ -225,14 +236,15 @@
         """The callback called once the connection to the 5G-ERA Network Application DATA_NAMESPACE is lost."""
 
         self.logger.info(
             f"Finally disconnected from server {DATA_NAMESPACE}, eio_sid "
             f"{self._channels.get_client_eio_sid(DATA_NAMESPACE)}"
         )
         self.disconnect()
+        self.print_stats()
 
     def control_disconnect_callback(self) -> None:
         """The callback called once the connection to the 5G-ERA Network Application CONTROL_NAMESPACE is lost."""
 
         self.logger.info(
             f"Disconnected from server {CONTROL_NAMESPACE}, eio_sid "
             f"{self._channels.get_client_eio_sid(CONTROL_NAMESPACE)}"
```

### Comparing `era_5g_client-0.9.0/era_5g_client/dataclasses.py` & `era_5g_client-1.0.0/era_5g_client/dataclasses.py`

 * *Files identical despite different names*

### Comparing `era_5g_client-0.9.0/era_5g_client/exceptions.py` & `era_5g_client-1.0.0/era_5g_client/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,20 +12,14 @@
 
 class FailedToInitialize(Era5gClientException):
     """Exception which is raised when the client could not initialize the 5G-ERA Network Application."""
 
     pass
 
 
-class FailedToObtainPlan(Era5gClientException):
-    """Exception which is raised when the client could not get the plan from the Middleware."""
-
-    pass
-
-
 class FailedToDeleteResource(Era5gClientException):
     """Exception which is raised when the client could not when could not delete Middleware resource."""
 
     pass
 
 
 class NetAppNotReady(Era5gClientException):
```

### Comparing `era_5g_client-0.9.0/era_5g_client/middleware_resource_checker.py` & `era_5g_client-1.0.0/era_5g_client/middleware_resource_checker.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,32 +11,37 @@
 logger = logging.getLogger(__name__)
 
 
 class MiddlewareResourceChecker(Thread):
     """Class for checking Middleware resources."""
 
     def __init__(
-        self, token: str, action_plan_id: str, status_endpoint: str, state_callback: Optional[Callable] = None, **kw
+        self,
+        token: str,
+        action_plan_id: str,
+        status_endpoint: str,
+        url_changed_callback: Optional[Callable] = None,
+        **kw,
     ) -> None:
         """Constructor.
 
         Args:
             token (str): Login token.
             action_plan_id (str): Action plan ID.
             status_endpoint (str): Status endpoint.
-            state_callback (Callable, optional): Optional state callback.
+            url_changed_callback (Callable, optional): Triggered if the received URL has changed.
             **kw: Thread arguments.
         """
 
         super().__init__(**kw)
         self.stop_event = Event()
         self.token = token
         self.action_plan_id = action_plan_id
         self.resource_state: Optional[Dict] = None
-        self.state_callback = state_callback
+        self.url_changed_callback = url_changed_callback
         self.status_endpoint = status_endpoint
         self.status: Optional[str] = None  # TODO define as enum?
         self.url: Optional[str] = None
 
     def stop(self) -> None:
         """Stop thread."""
 
@@ -46,26 +51,26 @@
         """Run thread.
 
         Check resource status in loop.
         """
 
         while not self.stop_event.is_set():
             resource_state = self.get_resource_status()
-
             seq = resource_state.get("actionSequence", [])
             if seq:
                 services = seq[0].get("Services", [])
                 if services:
                     self.resource_state = services[0]
                     assert isinstance(self.resource_state, dict)
                     self.status = self.resource_state.get("serviceStatus", None)
+                    old_url = self.url
                     self.url = self.resource_state.get("serviceUrl", None)
-                    logging.debug(f"{self.status=}, {self.url=}")
-            if self.state_callback:
-                self.state_callback(self.resource_state)
+                    if old_url and self.url_changed_callback and old_url != self.url:
+                        self.url_changed_callback()
+                    logger.debug(f"{self.status=}, {self.url=}")
             time.sleep(0.5)  # TODO: adjust or use something similar to rospy.rate.sleep()
 
     def get_resource_status(self) -> Dict:
         """Get resource status.
 
         Returns:
             resource status in dictionary.
@@ -78,15 +83,14 @@
             response = requests.get(url, headers=hed)
         except HTTPError as e:
             if e.response:
                 logger.debug(e.response.status_code)
             else:
                 logger.debug(e)
             raise FailedToConnect(f"Could not get the resource status, revisit the log files for more details. {e}")
-
         resp = response.json()
         if isinstance(resp, dict):
             return resp
         else:
             raise FailedToConnect("Invalid response.")
 
     def wait_until_resource_ready(self, timeout: int = -1) -> None:
```

### Comparing `era_5g_client-0.9.0/setup.py` & `era_5g_client-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,16 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
     ],
     'description': 'A client for 5G-ERA Network Applications',
     'install_requires': (
-        'era-5g-interface~=0.8.0',
-        'python-socketio[client]>=5.10.0',
+        'era-5g-interface~=0.10.0',
+        'python-socketio[client]>=5.11.1',
         'requests>=2.31.0',
         'types-requests>=2.31.0.10',
         'types-ujson>=5.8.0.1',
         'ujson>=5.8.0',
     ),
     'license': 'LGPL',
     'name': 'era_5g_client',
@@ -31,9 +31,9 @@
             'py.typed',
         ),
     },
     'packages': (
         'era_5g_client',
     ),
     'python_requires': '>=3.8',
-    'version': '0.9.0',
+    'version': '1.0.0',
 })
```

